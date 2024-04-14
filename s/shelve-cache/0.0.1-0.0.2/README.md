# Comparing `tmp/shelve_cache-0.0.1.tar.gz` & `tmp/shelve_cache-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/shelve_cache-0.0.1.tar", last modified: Sun Apr 14 12:11:12 2024, max compression
+gzip compressed data, was "dist/shelve_cache-0.0.2.tar", last modified: Sun Apr 14 12:23:37 2024, max compression
```

## Comparing `shelve_cache-0.0.1.tar` & `shelve_cache-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sanchitsingh   (501) staff       (20)        0 2024-04-14 12:11:12.230848 shelve_cache-0.0.1/
--rw-r--r--   0 sanchitsingh   (501) staff       (20)     1070 2024-04-14 11:46:21.000000 shelve_cache-0.0.1/LICENSE
--rw-r--r--   0 sanchitsingh   (501) staff       (20)     2253 2024-04-14 12:11:12.230442 shelve_cache-0.0.1/PKG-INFO
--rw-r--r--   0 sanchitsingh   (501) staff       (20)     1713 2024-04-14 11:51:49.000000 shelve_cache-0.0.1/README.md
--rw-r--r--   0 sanchitsingh   (501) staff       (20)       38 2024-04-14 12:11:12.230936 shelve_cache-0.0.1/setup.cfg
--rw-r--r--   0 sanchitsingh   (501) staff       (20)     1044 2024-04-14 12:10:06.000000 shelve_cache-0.0.1/setup.py
-drwxr-xr-x   0 sanchitsingh   (501) staff       (20)        0 2024-04-14 12:11:12.230025 shelve_cache-0.0.1/shelve_cache.egg-info/
--rw-r--r--   0 sanchitsingh   (501) staff       (20)     2253 2024-04-14 12:11:12.000000 shelve_cache-0.0.1/shelve_cache.egg-info/PKG-INFO
--rw-r--r--   0 sanchitsingh   (501) staff       (20)      221 2024-04-14 12:11:12.000000 shelve_cache-0.0.1/shelve_cache.egg-info/SOURCES.txt
--rw-r--r--   0 sanchitsingh   (501) staff       (20)        1 2024-04-14 12:11:12.000000 shelve_cache-0.0.1/shelve_cache.egg-info/dependency_links.txt
--rw-r--r--   0 sanchitsingh   (501) staff       (20)       12 2024-04-14 12:11:12.000000 shelve_cache-0.0.1/shelve_cache.egg-info/top_level.txt
-drwxr-xr-x   0 sanchitsingh   (501) staff       (20)        0 2024-04-14 12:11:12.229690 shelve_cache-0.0.1/shelvecache/
--rw-r--r--   0 sanchitsingh   (501) staff       (20)       74 2024-04-14 11:47:44.000000 shelve_cache-0.0.1/shelvecache/__init__.py
--rw-r--r--   0 sanchitsingh   (501) staff       (20)      929 2024-04-14 11:46:21.000000 shelve_cache-0.0.1/shelvecache/shelvecache.py
+drwxr-xr-x   0 sanchitsingh   (501) staff       (20)        0 2024-04-14 12:23:37.983154 shelve_cache-0.0.2/
+-rw-r--r--   0 sanchitsingh   (501) staff       (20)     1070 2024-04-14 11:46:21.000000 shelve_cache-0.0.2/LICENSE
+-rw-r--r--   0 sanchitsingh   (501) staff       (20)     2253 2024-04-14 12:23:37.982766 shelve_cache-0.0.2/PKG-INFO
+-rw-r--r--   0 sanchitsingh   (501) staff       (20)     1713 2024-04-14 11:51:49.000000 shelve_cache-0.0.2/README.md
+-rw-r--r--   0 sanchitsingh   (501) staff       (20)       38 2024-04-14 12:23:37.983262 shelve_cache-0.0.2/setup.cfg
+-rw-r--r--   0 sanchitsingh   (501) staff       (20)     1044 2024-04-14 12:23:30.000000 shelve_cache-0.0.2/setup.py
+drwxr-xr-x   0 sanchitsingh   (501) staff       (20)        0 2024-04-14 12:23:37.982309 shelve_cache-0.0.2/shelve_cache.egg-info/
+-rw-r--r--   0 sanchitsingh   (501) staff       (20)     2253 2024-04-14 12:23:37.000000 shelve_cache-0.0.2/shelve_cache.egg-info/PKG-INFO
+-rw-r--r--   0 sanchitsingh   (501) staff       (20)      221 2024-04-14 12:23:37.000000 shelve_cache-0.0.2/shelve_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 sanchitsingh   (501) staff       (20)        1 2024-04-14 12:23:37.000000 shelve_cache-0.0.2/shelve_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 sanchitsingh   (501) staff       (20)       12 2024-04-14 12:23:37.000000 shelve_cache-0.0.2/shelve_cache.egg-info/top_level.txt
+drwxr-xr-x   0 sanchitsingh   (501) staff       (20)        0 2024-04-14 12:23:37.981868 shelve_cache-0.0.2/shelvecache/
+-rw-r--r--   0 sanchitsingh   (501) staff       (20)       74 2024-04-14 11:47:44.000000 shelve_cache-0.0.2/shelvecache/__init__.py
+-rw-r--r--   0 sanchitsingh   (501) staff       (20)      984 2024-04-14 12:14:22.000000 shelve_cache-0.0.2/shelvecache/shelvecache.py
```

### Comparing `shelve_cache-0.0.1/LICENSE` & `shelve_cache-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shelve_cache-0.0.1/PKG-INFO` & `shelve_cache-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shelve_cache
-Version: 0.0.1
+Version: 0.0.2
 Summary: Persistant decorator
 Author: Sanchit Singh
 Author-email: <sanchitsingh849@gmail.com>
 Keywords: python,cache,shelve,decorator,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `shelve_cache-0.0.1/README.md` & `shelve_cache-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `shelve_cache-0.0.1/setup.py` & `shelve_cache-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages, setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 DESCRIPTION = "Persistant decorator"
 LONG_DESCRIPTION = "This will allow to save cached output on disk."
 
 # Setting up
 setup(
     name="shelve_cache",
     version=VERSION,
```

### Comparing `shelve_cache-0.0.1/shelve_cache.egg-info/PKG-INFO` & `shelve_cache-0.0.2/shelve_cache.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shelve_cache
-Version: 0.0.1
+Version: 0.0.2
 Summary: Persistant decorator
 Author: Sanchit Singh
 Author-email: <sanchitsingh849@gmail.com>
 Keywords: python,cache,shelve,decorator,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `shelve_cache-0.0.1/shelvecache/shelvecache.py` & `shelve_cache-0.0.2/shelvecache/shelvecache.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import shelve
 import functools
+import shelve
+
 
 def persistent_cache(filename):
     def decorator(func):
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
             with shelve.open(filename) as cache:
                 key = (args, frozenset(kwargs.items()))
@@ -11,19 +12,27 @@
                     print("Cache hit!")
                     return cache[key]
                 else:
                     print("Cache miss!")
                     result = func(*args, **kwargs)
                     cache[key] = result
                     return result
+
         return wrapper
+
     return decorator
 
+
 # Example usage:
 @persistent_cache("cache.db")
 def expensive_operation(x, y):
     print("Performing expensive operation...")
     return x * y
 
+
 # Test the decorated function
-print(expensive_operation(2, 3))  # Output: Performing expensive operation... Cache miss! 6
-print(expensive_operation(2, 3))  # Output: Cache hit! 6
+
+if __name__ == "__main__":
+    print(
+        expensive_operation(2, 3)
+    )  # Output: Performing expensive operation... Cache miss! 6
+    print(expensive_operation(2, 3))  # Output: Cache hit! 6
```

