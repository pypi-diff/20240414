# Comparing `tmp/typed_stream-0.8.1.tar.gz` & `tmp/typed_stream-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typed_stream-0.8.1.tar", last modified: Sat Feb 18 00:07:14 2023, max compression
+gzip compressed data, was "typed_stream-0.8.2.tar", last modified: Sat Feb 18 11:51:04 2023, max compression
```

## Comparing `typed_stream-0.8.1.tar` & `typed_stream-0.8.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    34523 2023-02-18 00:07:00.083927 typed_stream-0.8.1/LICENSE
--rw-r--r--   0        0        0      125 2023-02-18 00:07:00.083927 typed_stream-0.8.1/README.md
--rw-r--r--   0        0        0     1214 2023-02-18 00:07:00.083927 typed_stream-0.8.1/pyproject.toml
--rw-r--r--   0        0        0    20065 2023-02-18 00:07:00.083927 typed_stream-0.8.1/typed_stream/__init__.py
--rw-r--r--   0        0        0     4073 2023-02-18 00:07:00.083927 typed_stream-0.8.1/typed_stream/lazy_file_iterators.py
--rw-r--r--   0        0        0        0 2023-02-18 00:07:00.083927 typed_stream-0.8.1/typed_stream/py.typed
--rwxr-xr-x   0        0        0      224 2023-02-18 00:07:00.083927 typed_stream-0.8.1/typed_stream/version.py
--rw-r--r--   0        0        0      992 1970-01-01 00:00:00.000000 typed_stream-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-02-18 11:50:55.832903 typed_stream-0.8.2/LICENSE
+-rw-r--r--   0        0        0      125 2023-02-18 11:50:55.832903 typed_stream-0.8.2/README.md
+-rw-r--r--   0        0        0     1214 2023-02-18 11:50:55.832903 typed_stream-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0    20755 2023-02-18 11:50:55.832903 typed_stream-0.8.2/typed_stream/__init__.py
+-rw-r--r--   0        0        0     4073 2023-02-18 11:50:55.832903 typed_stream-0.8.2/typed_stream/lazy_file_iterators.py
+-rw-r--r--   0        0        0        0 2023-02-18 11:50:55.832903 typed_stream-0.8.2/typed_stream/py.typed
+-rwxr-xr-x   0        0        0      224 2023-02-18 11:50:55.832903 typed_stream-0.8.2/typed_stream/version.py
+-rw-r--r--   0        0        0      992 1970-01-01 00:00:00.000000 typed_stream-0.8.2/PKG-INFO
```

### Comparing `typed_stream-0.8.1/LICENSE` & `typed_stream-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `typed_stream-0.8.1/pyproject.toml` & `typed_stream-0.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typed_stream-0.8.1/typed_stream/__init__.py` & `typed_stream-0.8.2/typed_stream/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,27 +74,53 @@
         return Stream(self)
 
 
 class StreamableSequence(tuple[T, ...], Streamable[T]):
     """A streamable immutable Sequence."""
 
 
-def chunked(
-    iterable: Iterable[T], size: int
-) -> Iterable[StreamableSequence[T]]:
+class ValueIterator(Iterator[T], Streamable[T]):
+    """An iterable that always yields the value."""
+
+    _value: T
+    __slots__ = ("_value",)
+
+    def __init__(self, value: T) -> None:
+        self._value = value
+
+    def __next__(self) -> T:
+        return self._value
+
+
+class Chunked(
+    Iterator[StreamableSequence[T]], Streamable[StreamableSequence[T]]
+):
     """Chunk data into Sequences of length size. The last chunk may be shorter.
 
     Inspired by batched from:
     https://docs.python.org/3/library/itertools.html?highlight=callable#itertools-recipes
     """
-    if size < 1:
-        raise ValueError("size must be at least one")
-    iterator = iter(iterable)
-    while chunk := StreamableSequence(itertools.islice(iterator, size)):
-        yield chunk
+
+    _iterator: Iterator[T]
+    chunk_size: int
+
+    __slots__ = "_iterator", "chunk_size"
+
+    def __init__(self, iterable: Iterable[T], chunk_size: int) -> None:
+        if chunk_size < 1:
+            raise ValueError("size must be at least one")
+        self._iterator = iter(iterable)
+        self.chunk_size = chunk_size
+
+    def __next__(self) -> StreamableSequence[T]:
+        if chunk := StreamableSequence(
+            itertools.islice(self._iterator, self.chunk_size)
+        ):
+            return chunk
+        raise StopIteration()
 
 
 class Peeker(Generic[T]):
     """Peek values."""
 
     fun: Callable[[T], Any]
 
@@ -230,15 +256,15 @@
     def counting(start: int = 0, step: int = 1) -> "Stream[int]":
         """Create an endless counting Stream."""
         return Stream(itertools.count(start, step))
 
     @staticmethod
     def from_value(value: K) -> "Stream[K]":
         """Create an endless Stream of the same value."""
-        return Stream(itertools.repeat(value))
+        return ValueIterator(value).stream()
 
     def _check_finished(self) -> None:
         """Raise a StreamFinishedError if the stream is finished."""
         if self._is_finished():
             raise StreamFinishedError()
 
     def _close_source(self) -> None:
@@ -273,15 +299,15 @@
         self._check_finished()
         self._data = itertools.chain(self._data, iterable)
         return self
 
     def chunk(self, size: int) -> "Stream[StreamableSequence[T]]":
         """Split stream into chunks of the specified size."""
         self._check_finished()
-        return Stream(chunked(self, size))
+        return self._finish(Chunked(self._data, size).stream())
 
     if TYPE_CHECKING:  # noqa: C901
 
         @overload
         def collect(
             self, fun: type[StreamableSequence[T]]
         ) -> StreamableSequence[T]:
@@ -461,17 +487,22 @@
     ) -> "Stream[K]":
         """Map each value to another.
 
         This lazily finishes the current Stream and creates a new one.
 
         Example:
             - Stream([1, 4, 7]).flat_map(lambda x: [x, x + 1, x + 2])
+            - Stream(["abc", "def"]).flat_map(str.encode, "ASCII")
         """
         self._check_finished()
-        return Stream(itertools.chain.from_iterable(self.map(fun, *args)))
+        return Stream(
+            itertools.chain.from_iterable(
+                map(fun, self._data, *(ValueIterator(arg) for arg in args))
+            )
+        )
 
     def for_each(self, fun: Callable[[T], Any] = noop) -> None:
         """Consume all the values of the Stream with the callable."""
         self._check_finished()
         for value in self:
             fun(value)
 
@@ -539,19 +570,15 @@
 
         Example:
             - Stream([1, 2, 3]).map(lambda x: x * 3)
             - Stream([1, 2, 3]).map(operator.mul, 3)
         """
         self._check_finished()
         return self._finish(
-            Stream(
-                map(fun, self._data, *(Stream.from_value(arg) for arg in args))
-                if args
-                else map(fun, self._data)
-            )
+            Stream(map(fun, self._data, *(ValueIterator(arg) for arg in args)))
         )
 
     def max(self: "Stream[SLT]") -> SLT:
         """Return the biggest element of the stream."""
         return self.reduce(bigger_one)
 
     def min(self: "Stream[SLT]") -> SLT:
@@ -581,16 +608,16 @@
         self._data = map(Peeker(fun), self._data)
         return self
 
     def reduce(self, fun: Callable[[T, T], T]) -> T:
         """Reduce the values of this stream. This finishes the Stream.
 
         Examples:
-            - Stream([1, 2, 3]).accumulate(lambda x, y: x + y)
-            - Stream([1, 2, 3]).accumulate(lambda x, y: x * y)
+            - Stream([1, 2, 3]).accumulate(operator.add)
+            - Stream([1, 2, 3]).accumulate(operator.mul)
         """
         self._check_finished()
         return self._finish(
             functools.reduce(fun, self._data), close_source=True
         )
 
     def starcollect(self, fun: StarCallable[T, K]) -> K:
```

### Comparing `typed_stream-0.8.1/typed_stream/lazy_file_iterators.py` & `typed_stream-0.8.2/typed_stream/lazy_file_iterators.py`

 * *Files identical despite different names*

### Comparing `typed_stream-0.8.1/PKG-INFO` & `typed_stream-0.8.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typed_stream
-Version: 0.8.1
+Version: 0.8.2
 Summary: Java-like typed Stream class for easier handling of generators.
 Author-email: Joshix <joshix@asozial.org>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

