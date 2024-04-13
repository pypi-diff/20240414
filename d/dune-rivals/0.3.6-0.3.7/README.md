# Comparing `tmp/dune_rivals-0.3.6.tar.gz` & `tmp/dune_rivals-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_rivals-0.3.6.tar", last modified: Sat Apr 13 21:57:21 2024, max compression
+gzip compressed data, was "dune_rivals-0.3.7.tar", last modified: Sat Apr 13 22:04:53 2024, max compression
```

## Comparing `dune_rivals-0.3.6.tar` & `dune_rivals-0.3.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 21:57:21.276356 dune_rivals-0.3.6/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 21:57:21.275952 dune_rivals-0.3.6/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.3.6/README.md
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 21:57:21.275492 dune_rivals-0.3.6/dune_rivals.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 21:57:21.000000 dune_rivals-0.3.6/dune_rivals.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-13 21:57:21.000000 dune_rivals-0.3.6/dune_rivals.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-13 21:57:21.000000 dune_rivals-0.3.6/dune_rivals.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-13 21:57:21.000000 dune_rivals-0.3.6/dune_rivals.egg-info/top_level.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)    23404 2024-04-13 21:57:00.000000 dune_rivals-0.3.6/dune_rivals.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-13 21:57:16.000000 dune_rivals-0.3.6/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-13 21:57:21.276542 dune_rivals-0.3.6/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 22:04:53.560234 dune_rivals-0.3.7/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 22:04:53.559801 dune_rivals-0.3.7/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.3.7/README.md
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 22:04:53.559239 dune_rivals-0.3.7/dune_rivals.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 22:04:53.000000 dune_rivals-0.3.7/dune_rivals.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-13 22:04:53.000000 dune_rivals-0.3.7/dune_rivals.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-13 22:04:53.000000 dune_rivals-0.3.7/dune_rivals.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-13 22:04:53.000000 dune_rivals-0.3.7/dune_rivals.egg-info/top_level.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    23727 2024-04-13 22:04:29.000000 dune_rivals-0.3.7/dune_rivals.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-13 22:04:48.000000 dune_rivals-0.3.7/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-13 22:04:53.560346 dune_rivals-0.3.7/setup.cfg
```

### Comparing `dune_rivals-0.3.6/dune_rivals.py` & `dune_rivals-0.3.7/dune_rivals.py`

 * *Files 2% similar despite different names*

```diff
@@ -331,24 +331,20 @@
         self.id = None
         self.free = None
         self.num_singletons = None
 
     def get_spice_loc_map(self):
         return self.spice_loc_map
 
-    def get_num_singletons(self, id):
-        if id == self.id:
-            return self.num_singletons
-        else:
-            warrior = ray.get_actor(f"FeydRautha{id}")
-            return ray.get(warrior.get_num_singletons.remote(id))
-
     def is_free(self):
         return self.free
 
+    def get_num_singletons(self):
+        return self.num_singletons
+
     def destroy_spice_field_with_retry(self):
         self.free = False
         destroyed = False
         while not destroyed:
             destroyed = self._destroy_spice_field()
             time.sleep(0.0001)
         
@@ -375,22 +371,32 @@
                         singletons.append(idx)
                     idx += 1
             return np.array(locs), np.array(singletons)
 
         obj_spice_arr, obj_singletons = get_warrior_spice_arr(file_type=OBJ_FILE)
         self.num_singletons = len(obj_singletons)
 
+        # confirm that other actors have set num_singletons
+        all_ready = False
+        while not all_ready:
+            all_ready = True
+            for id in [2, 3, 4]:
+                warrior = ray.get_actor(f"FeydRautha{id}")
+                loc_map = ray.get(warrior.get_num_singletons.remote())
+                all_ready = all_ready and (loc_map is not None)
+
         # get num_singletons from every warrior to determine who leader will be (later);
         # everyone will compute the same leader
-        leader, fewest_singletons = -1, np.inf
-        for id in [1, 2, 3, 4]:
-            num_singletons = None
+        leader, fewest_singletons = -1, self.num_singletons
+        for id in [_id for _id in range(1, 5) if _id != self.id]:
+            warrior = ray.get_actor(f"FeydRautha{id}")
+            num_singletons is None
             while num_singletons is None:
-                num_singletons = self.get_num_singletons(id)
-                time.sleep(1e-6)
+                num_singletons = ray.get(warrior.get_num_singletons.remote())
+                time.sleep(1e-4)
 
             if num_singletons < fewest_singletons:
                 fewest_singletons = num_singletons
                 leader = id
 
         print(f"LEADER WILL BE: {leader}")
```

