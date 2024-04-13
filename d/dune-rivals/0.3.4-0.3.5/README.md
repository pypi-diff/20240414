# Comparing `tmp/dune_rivals-0.3.4.tar.gz` & `tmp/dune_rivals-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_rivals-0.3.4.tar", last modified: Sat Apr 13 21:49:52 2024, max compression
+gzip compressed data, was "dune_rivals-0.3.5.tar", last modified: Sat Apr 13 21:53:07 2024, max compression
```

## Comparing `dune_rivals-0.3.4.tar` & `dune_rivals-0.3.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 21:49:52.488554 dune_rivals-0.3.4/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 21:49:52.488136 dune_rivals-0.3.4/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.3.4/README.md
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 21:49:52.487688 dune_rivals-0.3.4/dune_rivals.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 21:49:52.000000 dune_rivals-0.3.4/dune_rivals.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-13 21:49:52.000000 dune_rivals-0.3.4/dune_rivals.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-13 21:49:52.000000 dune_rivals-0.3.4/dune_rivals.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-13 21:49:52.000000 dune_rivals-0.3.4/dune_rivals.egg-info/top_level.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)    23266 2024-04-13 21:49:10.000000 dune_rivals-0.3.4/dune_rivals.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-13 21:49:43.000000 dune_rivals-0.3.4/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-13 21:49:52.488643 dune_rivals-0.3.4/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 21:53:07.470840 dune_rivals-0.3.5/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 21:53:07.470408 dune_rivals-0.3.5/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.3.5/README.md
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 21:53:07.469992 dune_rivals-0.3.5/dune_rivals.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 21:53:07.000000 dune_rivals-0.3.5/dune_rivals.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-13 21:53:07.000000 dune_rivals-0.3.5/dune_rivals.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-13 21:53:07.000000 dune_rivals-0.3.5/dune_rivals.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-13 21:53:07.000000 dune_rivals-0.3.5/dune_rivals.egg-info/top_level.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    23273 2024-04-13 21:52:49.000000 dune_rivals-0.3.5/dune_rivals.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-13 21:53:02.000000 dune_rivals-0.3.5/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-13 21:53:07.470939 dune_rivals-0.3.5/setup.cfg
```

### Comparing `dune_rivals-0.3.4/dune_rivals.py` & `dune_rivals-0.3.5/dune_rivals.py`

 * *Files 0% similar despite different names*

```diff
@@ -336,15 +336,15 @@
         return self.spice_loc_map
 
     def get_num_singletons(self, id):
         if id == self.id:
             return self.num_singletons
         else:
             warrior = ray.get_actor(f"FeydRautha{id}")
-            return ray.get(warrior.get_num_singletons(id))
+            return ray.get(warrior.get_num_singletons.remote(id))
 
     def is_free(self):
         return self.free
 
     def destroy_spice_field_with_retry(self):
         self.free = False
         destroyed = False
```

