# Comparing `tmp/dune_rivals-0.3.8.tar.gz` & `tmp/dune_rivals-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_rivals-0.3.8.tar", last modified: Sat Apr 13 22:08:50 2024, max compression
+gzip compressed data, was "dune_rivals-0.3.9.tar", last modified: Sat Apr 13 22:10:40 2024, max compression
```

## Comparing `dune_rivals-0.3.8.tar` & `dune_rivals-0.3.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 22:08:50.524283 dune_rivals-0.3.8/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 22:08:50.523773 dune_rivals-0.3.8/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.3.8/README.md
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 22:08:50.523162 dune_rivals-0.3.8/dune_rivals.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 22:08:50.000000 dune_rivals-0.3.8/dune_rivals.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-13 22:08:50.000000 dune_rivals-0.3.8/dune_rivals.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-13 22:08:50.000000 dune_rivals-0.3.8/dune_rivals.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-13 22:08:50.000000 dune_rivals-0.3.8/dune_rivals.egg-info/top_level.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)    23544 2024-04-13 22:08:30.000000 dune_rivals-0.3.8/dune_rivals.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-13 22:08:45.000000 dune_rivals-0.3.8/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-13 22:08:50.524416 dune_rivals-0.3.8/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 22:10:40.172351 dune_rivals-0.3.9/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 22:10:40.171927 dune_rivals-0.3.9/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.3.9/README.md
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 22:10:40.171458 dune_rivals-0.3.9/dune_rivals.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 22:10:40.000000 dune_rivals-0.3.9/dune_rivals.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-13 22:10:40.000000 dune_rivals-0.3.9/dune_rivals.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-13 22:10:40.000000 dune_rivals-0.3.9/dune_rivals.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-13 22:10:40.000000 dune_rivals-0.3.9/dune_rivals.egg-info/top_level.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    23543 2024-04-13 22:10:03.000000 dune_rivals-0.3.9/dune_rivals.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-13 22:10:35.000000 dune_rivals-0.3.9/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-13 22:10:40.172443 dune_rivals-0.3.9/setup.cfg
```

### Comparing `dune_rivals-0.3.8/dune_rivals.py` & `dune_rivals-0.3.9/dune_rivals.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,15 +377,15 @@
         print(f"FeydRautha{self.id} num_singletons is: {self.num_singletons}")
 
         # get num_singletons from every warrior to determine who leader will be (later);
         # everyone will compute the same leader
         leader, fewest_singletons = -1, self.num_singletons
         for id in [_id for _id in range(1, 5) if _id != self.id]:
             warrior = ray.get_actor(f"FeydRautha{id}")
-            num_singletons is None
+            num_singletons = None
             while num_singletons is None:
                 num_singletons = ray.get(warrior.get_num_singletons.remote())
                 if num_singletons is None:
                     print(f"FeydRautha{self.id} waiting on: {id}")
                 time.sleep(1e-3)
 
             if num_singletons < fewest_singletons:
```

