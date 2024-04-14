# Comparing `tmp/dune_rivals-0.3.9.tar.gz` & `tmp/dune_rivals-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_rivals-0.3.9.tar", last modified: Sat Apr 13 22:10:40 2024, max compression
+gzip compressed data, was "dune_rivals-0.4.0.tar", last modified: Sun Apr 14 15:20:57 2024, max compression
```

## Comparing `dune_rivals-0.3.9.tar` & `dune_rivals-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 22:10:40.172351 dune_rivals-0.3.9/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 22:10:40.171927 dune_rivals-0.3.9/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.3.9/README.md
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 22:10:40.171458 dune_rivals-0.3.9/dune_rivals.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 22:10:40.000000 dune_rivals-0.3.9/dune_rivals.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-13 22:10:40.000000 dune_rivals-0.3.9/dune_rivals.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-13 22:10:40.000000 dune_rivals-0.3.9/dune_rivals.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-13 22:10:40.000000 dune_rivals-0.3.9/dune_rivals.egg-info/top_level.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)    23543 2024-04-13 22:10:03.000000 dune_rivals-0.3.9/dune_rivals.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-13 22:10:35.000000 dune_rivals-0.3.9/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-13 22:10:40.172443 dune_rivals-0.3.9/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-14 15:20:57.362324 dune_rivals-0.4.0/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-14 15:20:57.361707 dune_rivals-0.4.0/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.4.0/README.md
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-14 15:20:57.361005 dune_rivals-0.4.0/dune_rivals.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-14 15:20:57.000000 dune_rivals-0.4.0/dune_rivals.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-14 15:20:57.000000 dune_rivals-0.4.0/dune_rivals.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-14 15:20:57.000000 dune_rivals-0.4.0/dune_rivals.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-14 15:20:57.000000 dune_rivals-0.4.0/dune_rivals.egg-info/top_level.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    23786 2024-04-14 15:20:09.000000 dune_rivals-0.4.0/dune_rivals.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-14 15:20:42.000000 dune_rivals-0.4.0/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-14 15:20:57.362507 dune_rivals-0.4.0/setup.cfg
```

### Comparing `dune_rivals-0.3.9/dune_rivals.py` & `dune_rivals-0.4.0/dune_rivals.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import ray
 import time
 import numpy as np
 import scipy as sp
 
-# TODO: double check that obj. store read is < 0.1 (S3 read time)
 # DEFINITIONS
 SLEEP_SECONDS_PER_TRAVEL_COORD = 1e-5
 SLEEP_SECONDS_READ_FROM_S3     = 0.100
 SLEEP_SECONDS_NOT_ON_SPICE     = 1.000
 
 MAP_DIM = int(1e3)
 SPICE_FIELD_PROB = 0.01
@@ -63,21 +62,16 @@
         if self.spice_file_map[(self.i, self.j)] == S3_FILE:
             print(f"{self.name} fetching spice field object from S3 for {(self.i, self.j)}")
             time.sleep(SLEEP_SECONDS_READ_FROM_S3)
         else:
             print(f"{self.name} fetching spice field object from OBJECT STORE for {(self.i, self.j)}")
 
         # get spice field object
-        t0 = time.time()
         spice_field_ref = ray.get(self.gamestate.get_spice_field_ref.remote("southern", self.i, self.j))  # TODO: fix for h2h
-        t1 = time.time()
         spice_field = ray.get(spice_field_ref)
-        t2 = time.time()
-        print(f"FETCH SPICE FIELD REFS: {t1 - t0}")
-        print(f"FETCH SPICE FIELD: {t2 - t1}")
 
         # check if spice field object can be written to
         write_order = self.order_map[(self.i, self.j)]
         try:
             write_idx = np.where(write_order == self.id)[0][0]
         except:
             print(f"{self.name} tried to destroy spice at {(self.i, self.j)} but is not a valid destroyer ({list(write_order)})")
@@ -116,16 +110,14 @@
         # sleep for travel duration
         time.sleep(total_dist * SLEEP_SECONDS_PER_TRAVEL_COORD)
 
         # update coordinates
         self.i = new_i
         self.j = new_j
 
-        print(f"movement sleep for: {total_dist * SLEEP_SECONDS_PER_TRAVEL_COORD}")
-
 
 @ray.remote(num_cpus=0.1, resources={"worker3": 1e-4})
 class Noop12(BaseRivalActor):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 12
         self.name = "Noop12"
@@ -326,37 +318,35 @@
 ################################         Feyd Rautha          ################################
 ##############################################################################################
 class BaseFeydRautha(BaseRivalActor):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = None
         self.free = None
-        self.num_singletons = None
+        self.num_singletons = {}
 
     def get_spice_loc_map(self):
         return self.spice_loc_map
 
     def is_free(self):
         return self.free
 
-    def get_num_singletons(self):
-        return self.num_singletons
+    def set_num_singletons(self, id, num_singletons):
+        self.num_singletons[id] = num_singletons
 
-    def destroy_spice_field_with_retry(self):
-        self.free = False
+    def destroy_spice_field_with_retry(self, leader):
+        self.gamestate.send_message.remote(leader, self.id, {"free": False}, "rival")
         destroyed = False
         while not destroyed:
             destroyed = self._destroy_spice_field()
             time.sleep(0.0001)
         
-        self.free = True
+        self.gamestate.send_message.remote(leader, self.id, {"free": True}, "rival")
 
     def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
-        self.free = False
-
         # set these state variables
         self.spice_loc_map = spice_loc_map
         self.spice_file_map = spice_file_map
         self.order_map = order_map
 
         # construct spice arr w/this warrior's fields for finding nearest points quickly
         def get_warrior_spice_arr(file_type):
@@ -368,99 +358,102 @@
                 if self.id in warriors:
                     locs.append((i, j))
                     if len(warriors) == 1:
                         singletons.append(idx)
                     idx += 1
             return np.array(locs), np.array(singletons)
 
+        # compute location and number of singletons and update other warriors
         obj_spice_arr, obj_singletons = get_warrior_spice_arr(file_type=OBJ_FILE)
-        self.num_singletons = len(obj_singletons)
-        print(f"FeydRautha{self.id} num_singletons is: {self.num_singletons}")
+        num_singletons = len(obj_singletons)
+        for id in [_id for _id in range(1, 5) if _id != self.id]:
+            self.gamestate.send_message.remote(id, self.id, {"num_singletons": num_singletons}, "rival")
 
         # get num_singletons from every warrior to determine who leader will be (later);
         # everyone will compute the same leader
-        leader, fewest_singletons = -1, self.num_singletons
+        leader, fewest_singletons = self.id, num_singletons
         for id in [_id for _id in range(1, 5) if _id != self.id]:
-            warrior = ray.get_actor(f"FeydRautha{id}")
             num_singletons = None
             while num_singletons is None:
-                num_singletons = ray.get(warrior.get_num_singletons.remote())
-                if num_singletons is None:
-                    print(f"FeydRautha{self.id} waiting on: {id}")
-                time.sleep(1e-3)
+                msgs = ray.get(self.gamestate.get_messages.remote(self.id, id, "rival"))
+                if len(msgs) > 0:
+                    num_singletons = msgs[-1]["num_singletons"]
+                time.sleep(1e-4)
 
             if num_singletons < fewest_singletons:
                 fewest_singletons = num_singletons
                 leader = id
 
-        print(f"LEADER WILL BE: {leader}")
-
         # destroy all the obj singletons associated with this warrior
         for i, j in obj_spice_arr[obj_singletons]:
             self._ride_sandworm(i, j)
-            self.destroy_spice_field_with_retry(self.id)
+            self._destroy_spice_field()
 
         # remove deleted fields from obj_spice_arr
         obj_spice_arr = np.delete(obj_spice_arr, obj_singletons, axis=0)
 
         # once everyone is finished, leader will run the show
-        self.free = True
+        self.gamestate.send_message.remote(leader, self.id, {"free": True}, "rival")
         if self.id == leader:
             # destroy remaining obj spice
-            first_pass, skipped_lst = True, []
+            first_pass, skipped_lst, warrior_free_states = True, [], {id: False for id in range(1, 5)}
+            warrior_free_states[self.id] = True
             while first_pass or len(skipped_lst) > 0:
                 first_pass = False
 
                 for loc in obj_spice_arr:
                     i, j = loc[0], loc[1]
                     warrior_ids = self.order_map[(i,j)]
 
                     # if one of warrior_ids isn't free then skip
                     not_free = False
                     for warrior_id in warrior_ids:
-                        if not ray.get(ray.get_actor(f"FeydRautha{warrior_id}").is_free.remote()):
+                        msgs = ray.get(self.gamestate.get_messages.remote(self.id, warrior_id, "rival"))
+                        if len(msgs) > 0:
+                            warrior_free_states[warrior_id] = msgs[-1]["free"]
+                        if not warrior_free_states[warrior_id]:
                             skipped_lst.append(loc)
                             not_free = True
                             break
-                    
+
                     if not_free:
                         continue
 
                     # otherwise, move warriors that are needed to location (i,j)
                     for warrior_id in warrior_ids:
-                        if warrior_id != 1:
+                        if warrior_id != self.id:
                             warrior = ray.get_actor(f"FeydRautha{warrior_id}")
                             warrior._ride_sandworm.remote(i, j)
                         else:
                             self._ride_sandworm(i, j)
 
                     # destroy spice in asynchronous fashion
                     for warrior_id in warrior_ids:
-                        if warrior_id != 1:
+                        if warrior_id != self.id:
                             warrior = ray.get_actor(f"FeydRautha{warrior_id}")
-                            warrior.destroy_spice_field_with_retry.remote()
+                            warrior.destroy_spice_field_with_retry.remote(leader=self.id)
                         else:
-                            self.destroy_spice_field_with_retry()
+                            self.destroy_spice_field_with_retry(leader=self.id)
 
             # destroy s3 spice
             # get spice locations and iterate over them to destroy spice
             spice = np.where(spice_file_map==S3_FILE)
             for i, j in zip(spice[0], spice[1]):
                 # move warriors that are needed to location (i,j)
                 warrior_ids = self.order_map[(i,j)]
                 for warrior_id in warrior_ids:
-                    if warrior_id != 1:
+                    if warrior_id != self.id:
                         warrior = ray.get_actor(f"FeydRautha{warrior_id}")
                         warrior._ride_sandworm.remote(i, j)
                     else:
                         self._ride_sandworm(i, j)
 
                 # destroy spice in synchronous fashion
                 for warrior_id in warrior_ids:
-                    if warrior_id != 1:
+                    if warrior_id != self.id:
                         warrior = ray.get_actor(f"FeydRautha{warrior_id}")
                         ray.get(warrior._destroy_spice_field.remote())
                     else:
                         self._destroy_spice_field()
 
 
 @ray.remote(num_cpus=0.8, name="FeydRautha1", resources={"worker3": 1e-4})
```

