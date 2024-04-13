# Comparing `tmp/dune_rivals-0.3.5.tar.gz` & `tmp/dune_rivals-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_rivals-0.3.5.tar", last modified: Sat Apr 13 21:53:07 2024, max compression
+gzip compressed data, was "dune_rivals-0.3.6.tar", last modified: Sat Apr 13 21:57:21 2024, max compression
```

## Comparing `dune_rivals-0.3.5.tar` & `dune_rivals-0.3.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 21:53:07.470840 dune_rivals-0.3.5/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 21:53:07.470408 dune_rivals-0.3.5/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.3.5/README.md
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 21:53:07.469992 dune_rivals-0.3.5/dune_rivals.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 21:53:07.000000 dune_rivals-0.3.5/dune_rivals.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-13 21:53:07.000000 dune_rivals-0.3.5/dune_rivals.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-13 21:53:07.000000 dune_rivals-0.3.5/dune_rivals.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-13 21:53:07.000000 dune_rivals-0.3.5/dune_rivals.egg-info/top_level.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)    23273 2024-04-13 21:52:49.000000 dune_rivals-0.3.5/dune_rivals.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-13 21:53:02.000000 dune_rivals-0.3.5/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-13 21:53:07.470939 dune_rivals-0.3.5/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 21:57:21.276356 dune_rivals-0.3.6/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 21:57:21.275952 dune_rivals-0.3.6/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.3.6/README.md
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 21:57:21.275492 dune_rivals-0.3.6/dune_rivals.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 21:57:21.000000 dune_rivals-0.3.6/dune_rivals.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-13 21:57:21.000000 dune_rivals-0.3.6/dune_rivals.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-13 21:57:21.000000 dune_rivals-0.3.6/dune_rivals.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-13 21:57:21.000000 dune_rivals-0.3.6/dune_rivals.egg-info/top_level.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    23404 2024-04-13 21:57:00.000000 dune_rivals-0.3.6/dune_rivals.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-13 21:57:16.000000 dune_rivals-0.3.6/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-13 21:57:21.276542 dune_rivals-0.3.6/setup.cfg
```

### Comparing `dune_rivals-0.3.5/dune_rivals.py` & `dune_rivals-0.3.6/dune_rivals.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,25 +379,29 @@
         obj_spice_arr, obj_singletons = get_warrior_spice_arr(file_type=OBJ_FILE)
         self.num_singletons = len(obj_singletons)
 
         # get num_singletons from every warrior to determine who leader will be (later);
         # everyone will compute the same leader
         leader, fewest_singletons = -1, np.inf
         for id in [1, 2, 3, 4]:
-            num_singletons = self.get_num_singletons(id)
+            num_singletons = None
+            while num_singletons is None:
+                num_singletons = self.get_num_singletons(id)
+                time.sleep(1e-6)
+
             if num_singletons < fewest_singletons:
                 fewest_singletons = num_singletons
                 leader = id
 
         print(f"LEADER WILL BE: {leader}")
 
         # destroy all the obj singletons associated with this warrior
         for i, j in obj_spice_arr[obj_singletons]:
             self._ride_sandworm(i, j)
-            self.destroy_block(self.id)
+            self.destroy_spice_field_with_retry(self.id)
 
         # remove deleted fields from obj_spice_arr
         obj_spice_arr = np.delete(obj_spice_arr, obj_singletons, axis=0)
 
         # once everyone is finished, leader will run the show
         self.free = True
         if self.id == leader:
```

