# Comparing `tmp/leaf_BasedLabs-0.0.8.tar.gz` & `tmp/leaf_basedlabs-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leaf_BasedLabs-0.0.8.tar", last modified: Sun Apr  7 11:29:20 2024, max compression
+gzip compressed data, was "leaf_basedlabs-0.0.9.tar", last modified: Sun Apr 14 09:37:41 2024, max compression
```

## Comparing `leaf_BasedLabs-0.0.8.tar` & `leaf_basedlabs-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 jt        (1000) jt        (1000)        0 2024-04-07 11:29:20.198776 leaf_BasedLabs-0.0.8/
--rw-rw-r--   0 jt        (1000) jt        (1000)    11357 2024-04-03 22:08:11.000000 leaf_BasedLabs-0.0.8/LICENSE
--rw-r--r--   0 jt        (1000) jt        (1000)     1987 2024-04-07 11:29:20.198776 leaf_BasedLabs-0.0.8/PKG-INFO
--rw-rw-r--   0 jt        (1000) jt        (1000)     1442 2024-04-03 22:08:11.000000 leaf_BasedLabs-0.0.8/README.md
--rw-rw-r--   0 jt        (1000) jt        (1000)      526 2024-04-07 11:29:15.000000 leaf_BasedLabs-0.0.8/pyproject.toml
--rw-rw-r--   0 jt        (1000) jt        (1000)       38 2024-04-07 11:29:20.198776 leaf_BasedLabs-0.0.8/setup.cfg
-drwxrwxr-x   0 jt        (1000) jt        (1000)        0 2024-04-07 11:29:20.194776 leaf_BasedLabs-0.0.8/src/
--rw-rw-r--   0 jt        (1000) jt        (1000)        0 2024-04-03 22:08:11.000000 leaf_BasedLabs-0.0.8/src/__init__.py
--rw-rw-r--   0 jt        (1000) jt        (1000)     1331 2024-04-03 22:08:11.000000 leaf_BasedLabs-0.0.8/src/example.py
-drwxrwxr-x   0 jt        (1000) jt        (1000)        0 2024-04-07 11:29:20.198776 leaf_BasedLabs-0.0.8/src/leaf/
--rw-rw-r--   0 jt        (1000) jt        (1000)       63 2024-04-03 22:08:11.000000 leaf_BasedLabs-0.0.8/src/leaf/__init__.py
--rw-rw-r--   0 jt        (1000) jt        (1000)      471 2024-04-03 22:08:11.000000 leaf_BasedLabs-0.0.8/src/leaf/exception.py
--rw-rw-r--   0 jt        (1000) jt        (1000)     9355 2024-04-07 11:28:44.000000 leaf_BasedLabs-0.0.8/src/leaf/filesystem.py
-drwxrwxr-x   0 jt        (1000) jt        (1000)        0 2024-04-07 11:29:20.198776 leaf_BasedLabs-0.0.8/src/leaf_BasedLabs.egg-info/
--rw-r--r--   0 jt        (1000) jt        (1000)     1987 2024-04-07 11:29:20.000000 leaf_BasedLabs-0.0.8/src/leaf_BasedLabs.egg-info/PKG-INFO
--rw-rw-r--   0 jt        (1000) jt        (1000)      316 2024-04-07 11:29:20.000000 leaf_BasedLabs-0.0.8/src/leaf_BasedLabs.egg-info/SOURCES.txt
--rw-rw-r--   0 jt        (1000) jt        (1000)        1 2024-04-07 11:29:20.000000 leaf_BasedLabs-0.0.8/src/leaf_BasedLabs.egg-info/dependency_links.txt
--rw-rw-r--   0 jt        (1000) jt        (1000)       28 2024-04-07 11:29:20.000000 leaf_BasedLabs-0.0.8/src/leaf_BasedLabs.egg-info/top_level.txt
-drwxrwxr-x   0 jt        (1000) jt        (1000)        0 2024-04-07 11:29:20.198776 leaf_BasedLabs-0.0.8/src/tests/
--rw-rw-r--   0 jt        (1000) jt        (1000)     3602 2024-04-03 22:08:11.000000 leaf_BasedLabs-0.0.8/src/tests/tests.py
+drwxrwxr-x   0 jt        (1000) jt        (1000)        0 2024-04-14 09:37:41.845239 leaf_basedlabs-0.0.9/
+-rw-rw-r--   0 jt        (1000) jt        (1000)    11357 2024-04-03 22:08:11.000000 leaf_basedlabs-0.0.9/LICENSE
+-rw-r--r--   0 jt        (1000) jt        (1000)     1987 2024-04-14 09:37:41.845239 leaf_basedlabs-0.0.9/PKG-INFO
+-rw-rw-r--   0 jt        (1000) jt        (1000)     1442 2024-04-03 22:08:11.000000 leaf_basedlabs-0.0.9/README.md
+-rw-rw-r--   0 jt        (1000) jt        (1000)      526 2024-04-14 09:37:34.000000 leaf_basedlabs-0.0.9/pyproject.toml
+-rw-rw-r--   0 jt        (1000) jt        (1000)       38 2024-04-14 09:37:41.845239 leaf_basedlabs-0.0.9/setup.cfg
+drwxrwxr-x   0 jt        (1000) jt        (1000)        0 2024-04-14 09:37:41.845239 leaf_basedlabs-0.0.9/src/
+-rw-rw-r--   0 jt        (1000) jt        (1000)        0 2024-04-03 22:08:11.000000 leaf_basedlabs-0.0.9/src/__init__.py
+-rw-rw-r--   0 jt        (1000) jt        (1000)     1331 2024-04-03 22:08:11.000000 leaf_basedlabs-0.0.9/src/example.py
+drwxrwxr-x   0 jt        (1000) jt        (1000)        0 2024-04-14 09:37:41.845239 leaf_basedlabs-0.0.9/src/leaf/
+-rw-rw-r--   0 jt        (1000) jt        (1000)       63 2024-04-03 22:08:11.000000 leaf_basedlabs-0.0.9/src/leaf/__init__.py
+-rw-rw-r--   0 jt        (1000) jt        (1000)      471 2024-04-03 22:08:11.000000 leaf_basedlabs-0.0.9/src/leaf/exception.py
+-rw-rw-r--   0 jt        (1000) jt        (1000)    10851 2024-04-14 09:37:07.000000 leaf_basedlabs-0.0.9/src/leaf/filesystem.py
+drwxrwxr-x   0 jt        (1000) jt        (1000)        0 2024-04-14 09:37:41.845239 leaf_basedlabs-0.0.9/src/leaf_BasedLabs.egg-info/
+-rw-r--r--   0 jt        (1000) jt        (1000)     1987 2024-04-14 09:37:41.000000 leaf_basedlabs-0.0.9/src/leaf_BasedLabs.egg-info/PKG-INFO
+-rw-rw-r--   0 jt        (1000) jt        (1000)      316 2024-04-14 09:37:41.000000 leaf_basedlabs-0.0.9/src/leaf_BasedLabs.egg-info/SOURCES.txt
+-rw-rw-r--   0 jt        (1000) jt        (1000)        1 2024-04-14 09:37:41.000000 leaf_basedlabs-0.0.9/src/leaf_BasedLabs.egg-info/dependency_links.txt
+-rw-rw-r--   0 jt        (1000) jt        (1000)       28 2024-04-14 09:37:41.000000 leaf_basedlabs-0.0.9/src/leaf_BasedLabs.egg-info/top_level.txt
+drwxrwxr-x   0 jt        (1000) jt        (1000)        0 2024-04-14 09:37:41.845239 leaf_basedlabs-0.0.9/src/tests/
+-rw-rw-r--   0 jt        (1000) jt        (1000)     3602 2024-04-03 22:08:11.000000 leaf_basedlabs-0.0.9/src/tests/tests.py
```

### Comparing `leaf_BasedLabs-0.0.8/LICENSE` & `leaf_basedlabs-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `leaf_BasedLabs-0.0.8/PKG-INFO` & `leaf_basedlabs-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leaf_BasedLabs
-Version: 0.0.8
+Version: 0.0.9
 Summary: Leaf is a small (just two .py files) on-demand hierachical filesystem database.
 Author-email: Igor Bruev <jaktenstid1@gmail.com>
 Project-URL: Homepage, https://github.com/BasedLabs/leaf
 Project-URL: Issues, https://github.com/BasedLabs/leaf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `leaf_BasedLabs-0.0.8/README.md` & `leaf_basedlabs-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `leaf_BasedLabs-0.0.8/pyproject.toml` & `leaf_basedlabs-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "leaf_BasedLabs"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Igor Bruev", email="jaktenstid1@gmail.com" },
 ]
 description = "Leaf is a small (just two .py files) on-demand hierachical filesystem database."
 readme = "README.md"
 requires-python = ">=3"
 classifiers = [
```

### Comparing `leaf_BasedLabs-0.0.8/src/example.py` & `leaf_basedlabs-0.0.9/src/example.py`

 * *Files identical despite different names*

### Comparing `leaf_BasedLabs-0.0.8/src/leaf/filesystem.py` & `leaf_basedlabs-0.0.9/src/leaf/filesystem.py`

 * *Files 7% similar despite different names*

```diff
@@ -140,14 +140,25 @@
     def where(self, predicate: Callable[[FileObject], bool], recursive=False) -> Iterable[FileObject]:
         for child in self.parent.children:
             if isinstance(child, FileObject) and predicate(child):
                 yield child
             if recursive and isinstance(child, DirectoryObject):
                 yield from child.files.where(predicate)
 
+    def by_name(self, name: str, recursive=False) -> FileObject | None:
+        """Returns the first or None object in the tree by predicate"""
+        for child in self.parent.children:
+            if isinstance(child, FileObject) and child.name == name:
+                return child
+            if recursive and isinstance(child, DirectoryObject):
+                found = child.files.by_name(name, recursive=recursive)
+                if found:
+                    return found
+        return None
+
     def first_or_default(self, predicate: Callable[[FileObject], bool], recursive=False) -> FileObject | None:
         """Returns the first or None object in the tree by predicate"""
         for child in self.parent.children:
             if isinstance(child, FileObject) and predicate(child):
                 return child
             if recursive and isinstance(child, DirectoryObject):
                 found = child.files.first_or_default(predicate, recursive=recursive)
@@ -171,14 +182,26 @@
     def where(self, predicate: Callable[[DirectoryObject], bool], recursive=False) -> Iterable[DirectoryObject]:
         for child in self.parent.children:
             if isinstance(child, DirectoryObject) and predicate(child):
                 yield child
                 if recursive:
                     yield from child.directories.where(predicate)
 
+    def by_name(self, name: str, recursive=False) -> DirectoryObject | None:
+        """Returns the first or None object in the tree by predicate"""
+        for child in self.parent.children:
+            if isinstance(child, DirectoryObject):
+                if name == child.name:
+                    return child
+                if recursive:
+                    found = child.directories.by_name(name, recursive=recursive)
+                    if found:
+                        return found
+        return None
+
     def first_or_default(self, predicate: Callable[[DirectoryObject], bool], recursive=False) -> DirectoryObject | None:
         """Returns the first or None object in the tree by predicate"""
         for child in self.parent.children:
             if isinstance(child, DirectoryObject):
                 if predicate(child):
                     return child
                 if recursive:
@@ -281,14 +304,27 @@
             if predicate(child):
                 return True
             if recursive and isinstance(child, DirectoryObject) and child.exists(predicate, recursive=recursive):
                 return True
 
         return False
 
+    def by_name(self, name: str, recursive=False) -> Object | None:
+        """Returns the first or None object in the tree by predicate"""
+        self._ensure_exists()
+
+        for child in self.children:
+            if child.name == name:
+                return child
+            if recursive and isinstance(child, DirectoryObject):
+                found = child.by_name(name, recursive=recursive)
+                if found:
+                    return found
+        return None
+
     def first_or_default(self, predicate: Callable[[Object], bool], recursive=False) -> Object | None:
         """Returns the first or None object in the tree by predicate"""
         self._ensure_exists()
 
         for child in self.children:
             if predicate(child):
                 return child
```

### Comparing `leaf_BasedLabs-0.0.8/src/leaf_BasedLabs.egg-info/PKG-INFO` & `leaf_basedlabs-0.0.9/src/leaf_BasedLabs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leaf_BasedLabs
-Version: 0.0.8
+Version: 0.0.9
 Summary: Leaf is a small (just two .py files) on-demand hierachical filesystem database.
 Author-email: Igor Bruev <jaktenstid1@gmail.com>
 Project-URL: Homepage, https://github.com/BasedLabs/leaf
 Project-URL: Issues, https://github.com/BasedLabs/leaf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `leaf_BasedLabs-0.0.8/src/tests/tests.py` & `leaf_basedlabs-0.0.9/src/tests/tests.py`

 * *Files identical despite different names*

