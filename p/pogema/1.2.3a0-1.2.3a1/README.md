# Comparing `tmp/pogema-1.2.3a0.tar.gz` & `tmp/pogema-1.2.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pogema-1.2.3a0.tar", last modified: Sat Apr 13 20:36:40 2024, max compression
+gzip compressed data, was "pogema-1.2.3a1.tar", last modified: Sat Apr 13 21:15:34 2024, max compression
```

## Comparing `pogema-1.2.3a0.tar` & `pogema-1.2.3a1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-13 20:36:40.374878 pogema-1.2.3a0/
--rw-r--r--   0 skrynnik   (503) staff       (20)     1073 2023-08-30 09:49:20.000000 pogema-1.2.3a0/LICENSE
--rw-r--r--   0 skrynnik   (503) staff       (20)     6855 2024-04-13 20:36:40.373587 pogema-1.2.3a0/PKG-INFO
--rw-r--r--   0 skrynnik   (503) staff       (20)     6472 2023-08-31 15:07:00.000000 pogema-1.2.3a0/README.md
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-13 20:36:40.355409 pogema-1.2.3a0/pogema/
--rw-r--r--   0 skrynnik   (503) staff       (20)      967 2024-04-13 20:36:05.000000 pogema-1.2.3a0/pogema/__init__.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     4029 2023-08-30 09:49:20.000000 pogema-1.2.3a0/pogema/a_star_policy.py
--rw-r--r--   0 skrynnik   (503) staff       (20)    23996 2024-04-13 20:36:05.000000 pogema-1.2.3a0/pogema/animation.py
--rw-r--r--   0 skrynnik   (503) staff       (20)    16259 2023-09-22 09:44:42.000000 pogema-1.2.3a0/pogema/envs.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     4800 2023-08-30 09:49:20.000000 pogema-1.2.3a0/pogema/generator.py
--rw-r--r--   0 skrynnik   (503) staff       (20)    11642 2023-09-22 09:44:42.000000 pogema-1.2.3a0/pogema/grid.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     8150 2023-09-22 09:44:42.000000 pogema-1.2.3a0/pogema/grid_config.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     3187 2023-08-30 09:49:20.000000 pogema-1.2.3a0/pogema/grid_registry.py
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-13 20:36:40.364682 pogema-1.2.3a0/pogema/integrations/
--rw-r--r--   0 skrynnik   (503) staff       (20)        0 2023-08-30 09:49:20.000000 pogema-1.2.3a0/pogema/integrations/__init__.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     2522 2023-08-30 09:49:20.000000 pogema-1.2.3a0/pogema/integrations/make_pogema.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     2607 2023-08-30 09:49:20.000000 pogema-1.2.3a0/pogema/integrations/pettingzoo.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     2603 2024-04-13 20:35:39.000000 pogema-1.2.3a0/pogema/integrations/pymarl.py
--rw-r--r--   0 skrynnik   (503) staff       (20)      936 2023-08-30 09:49:20.000000 pogema-1.2.3a0/pogema/integrations/sample_factory.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     1975 2024-04-13 20:36:05.000000 pogema-1.2.3a0/pogema/svg_objects.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     3254 2023-08-30 09:49:20.000000 pogema-1.2.3a0/pogema/utils.py
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-13 20:36:40.367926 pogema-1.2.3a0/pogema/wrappers/
--rw-r--r--   0 skrynnik   (503) staff       (20)        0 2023-08-30 09:49:20.000000 pogema-1.2.3a0/pogema/wrappers/__init__.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     3912 2023-08-30 09:49:20.000000 pogema-1.2.3a0/pogema/wrappers/metrics.py
--rw-r--r--   0 skrynnik   (503) staff       (20)      656 2023-08-30 09:49:20.000000 pogema-1.2.3a0/pogema/wrappers/multi_time_limit.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     3080 2023-08-30 09:49:20.000000 pogema-1.2.3a0/pogema/wrappers/persistence.py
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-13 20:36:40.373016 pogema-1.2.3a0/pogema.egg-info/
--rw-r--r--   0 skrynnik   (503) staff       (20)     6855 2024-04-13 20:36:40.000000 pogema-1.2.3a0/pogema.egg-info/PKG-INFO
--rw-r--r--   0 skrynnik   (503) staff       (20)      817 2024-04-13 20:36:40.000000 pogema-1.2.3a0/pogema.egg-info/SOURCES.txt
--rw-r--r--   0 skrynnik   (503) staff       (20)        1 2024-04-13 20:36:40.000000 pogema-1.2.3a0/pogema.egg-info/dependency_links.txt
--rw-r--r--   0 skrynnik   (503) staff       (20)       65 2024-04-13 20:36:40.000000 pogema-1.2.3a0/pogema.egg-info/requires.txt
--rw-r--r--   0 skrynnik   (503) staff       (20)        7 2024-04-13 20:36:40.000000 pogema-1.2.3a0/pogema.egg-info/top_level.txt
--rw-r--r--   0 skrynnik   (503) staff       (20)       38 2024-04-13 20:36:40.375004 pogema-1.2.3a0/setup.cfg
--rw-r--r--   0 skrynnik   (503) staff       (20)     1409 2023-08-30 09:49:20.000000 pogema-1.2.3a0/setup.py
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-13 20:36:40.372093 pogema-1.2.3a0/tests/
--rw-r--r--   0 skrynnik   (503) staff       (20)     7234 2023-08-31 15:07:00.000000 pogema-1.2.3a0/tests/test_deterministic_policy.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     8065 2023-11-28 11:12:00.000000 pogema-1.2.3a0/tests/test_grid.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     4693 2023-08-30 09:49:20.000000 pogema-1.2.3a0/tests/test_integrations.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     9497 2023-08-30 09:49:20.000000 pogema-1.2.3a0/tests/test_pogema_env.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-13 21:15:34.591159 pogema-1.2.3a1/
+-rw-r--r--   0 skrynnik   (503) staff       (20)     1073 2023-08-30 09:49:20.000000 pogema-1.2.3a1/LICENSE
+-rw-r--r--   0 skrynnik   (503) staff       (20)     6855 2024-04-13 21:15:34.590186 pogema-1.2.3a1/PKG-INFO
+-rw-r--r--   0 skrynnik   (503) staff       (20)     6472 2023-08-31 15:07:00.000000 pogema-1.2.3a1/README.md
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-13 21:15:34.574308 pogema-1.2.3a1/pogema/
+-rw-r--r--   0 skrynnik   (503) staff       (20)      967 2024-04-13 21:15:07.000000 pogema-1.2.3a1/pogema/__init__.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     4029 2023-08-30 09:49:20.000000 pogema-1.2.3a1/pogema/a_star_policy.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)    24008 2024-04-13 21:15:07.000000 pogema-1.2.3a1/pogema/animation.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)    16259 2023-09-22 09:44:42.000000 pogema-1.2.3a1/pogema/envs.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     4800 2023-08-30 09:49:20.000000 pogema-1.2.3a1/pogema/generator.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)    11642 2023-09-22 09:44:42.000000 pogema-1.2.3a1/pogema/grid.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     8150 2023-09-22 09:44:42.000000 pogema-1.2.3a1/pogema/grid_config.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     3187 2023-08-30 09:49:20.000000 pogema-1.2.3a1/pogema/grid_registry.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-13 21:15:34.581627 pogema-1.2.3a1/pogema/integrations/
+-rw-r--r--   0 skrynnik   (503) staff       (20)        0 2023-08-30 09:49:20.000000 pogema-1.2.3a1/pogema/integrations/__init__.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     2522 2023-08-30 09:49:20.000000 pogema-1.2.3a1/pogema/integrations/make_pogema.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     2607 2023-08-30 09:49:20.000000 pogema-1.2.3a1/pogema/integrations/pettingzoo.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     2603 2024-04-13 20:35:39.000000 pogema-1.2.3a1/pogema/integrations/pymarl.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)      936 2023-08-30 09:49:20.000000 pogema-1.2.3a1/pogema/integrations/sample_factory.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     1975 2024-04-13 20:36:05.000000 pogema-1.2.3a1/pogema/svg_objects.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     3254 2023-08-30 09:49:20.000000 pogema-1.2.3a1/pogema/utils.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-13 21:15:34.584744 pogema-1.2.3a1/pogema/wrappers/
+-rw-r--r--   0 skrynnik   (503) staff       (20)        0 2023-08-30 09:49:20.000000 pogema-1.2.3a1/pogema/wrappers/__init__.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     3912 2023-08-30 09:49:20.000000 pogema-1.2.3a1/pogema/wrappers/metrics.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)      656 2023-08-30 09:49:20.000000 pogema-1.2.3a1/pogema/wrappers/multi_time_limit.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     3080 2023-08-30 09:49:20.000000 pogema-1.2.3a1/pogema/wrappers/persistence.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-13 21:15:34.589626 pogema-1.2.3a1/pogema.egg-info/
+-rw-r--r--   0 skrynnik   (503) staff       (20)     6855 2024-04-13 21:15:34.000000 pogema-1.2.3a1/pogema.egg-info/PKG-INFO
+-rw-r--r--   0 skrynnik   (503) staff       (20)      817 2024-04-13 21:15:34.000000 pogema-1.2.3a1/pogema.egg-info/SOURCES.txt
+-rw-r--r--   0 skrynnik   (503) staff       (20)        1 2024-04-13 21:15:34.000000 pogema-1.2.3a1/pogema.egg-info/dependency_links.txt
+-rw-r--r--   0 skrynnik   (503) staff       (20)       65 2024-04-13 21:15:34.000000 pogema-1.2.3a1/pogema.egg-info/requires.txt
+-rw-r--r--   0 skrynnik   (503) staff       (20)        7 2024-04-13 21:15:34.000000 pogema-1.2.3a1/pogema.egg-info/top_level.txt
+-rw-r--r--   0 skrynnik   (503) staff       (20)       38 2024-04-13 21:15:34.591233 pogema-1.2.3a1/setup.cfg
+-rw-r--r--   0 skrynnik   (503) staff       (20)     1409 2023-08-30 09:49:20.000000 pogema-1.2.3a1/setup.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-13 21:15:34.588591 pogema-1.2.3a1/tests/
+-rw-r--r--   0 skrynnik   (503) staff       (20)     7234 2023-08-31 15:07:00.000000 pogema-1.2.3a1/tests/test_deterministic_policy.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     8065 2023-11-28 11:12:00.000000 pogema-1.2.3a1/tests/test_grid.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     4693 2023-08-30 09:49:20.000000 pogema-1.2.3a1/tests/test_integrations.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     9497 2023-08-30 09:49:20.000000 pogema-1.2.3a1/tests/test_pogema_env.py
```

### Comparing `pogema-1.2.3a0/LICENSE` & `pogema-1.2.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pogema-1.2.3a0/PKG-INFO` & `pogema-1.2.3a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pogema
-Version: 1.2.3a0
+Version: 1.2.3a1
 Summary: Partially Observable Grid Environment for Multiple Agents
 Home-page: https://github.com/AIRI-Institute/pogema
 Author: Alexey Skrynnik
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pogema-1.2.3a0/README.md` & `pogema-1.2.3a1/README.md`

 * *Files identical despite different names*

### Comparing `pogema-1.2.3a0/pogema/__init__.py` & `pogema-1.2.3a1/pogema/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pogema.a_star_policy import AStarAgent, BatchAStarAgent
 
 from pogema.grid_config import Easy8x8, Normal8x8, Hard8x8, ExtraHard8x8
 from pogema.grid_config import Easy16x16, Normal16x16, Hard16x16, ExtraHard16x16
 from pogema.grid_config import Easy32x32, Normal32x32, Hard32x32, ExtraHard32x32
 from pogema.grid_config import Easy64x64, Normal64x64, Hard64x64, ExtraHard64x64
 
-__version__ = '1.2.3a0'
+__version__ = '1.2.3a1'
 
 __all__ = [
     'GridConfig',
     'pogema_v0',
     'AStarAgent', 'BatchAStarAgent',
     'Easy8x8', 'Normal8x8', 'Hard8x8', 'ExtraHard8x8',
     'Easy16x16', 'Normal16x16', 'Hard16x16', 'ExtraHard16x16',
```

### Comparing `pogema-1.2.3a0/pogema/a_star_policy.py` & `pogema-1.2.3a1/pogema/a_star_policy.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.3a0/pogema/animation.py` & `pogema-1.2.3a1/pogema/animation.py`

 * *Files 0% similar despite different names*

```diff
@@ -359,15 +359,15 @@
         """
         gh: GridHolder = grid_holder
         cfg = self.svg_settings
         for agent_idx, agent in enumerate(agents):
             x_path = []
             y_path = []
             opacity = []
-            for agent_state in gh.history[agent_idx]:
+            for idx, agent_state in enumerate(gh.history[agent_idx]):
                 x, y = agent_state.get_xy()
 
                 x_path.append(str(cfg.draw_start + y * cfg.scale_size))
                 y_path.append(str(-cfg.draw_start + -(gh.width - x - 1) * cfg.scale_size))
 
                 if egocentric_idx is not None:
                     ego_x, ego_y = gh.history[egocentric_idx][idx].get_xy()
@@ -549,15 +549,15 @@
         ego_idx = animation_config.egocentric_idx
         agents = []
 
         for idx, (x, y) in enumerate(initial_positions):
             circle_settings = {
                 'cx': self.svg_settings.draw_start + y * self.svg_settings.scale_size,
                 'cy': self.svg_settings.draw_start + (grid_holder.width - x - 1) * self.svg_settings.scale_size,
-                # 'r': self.svg_settings.r,
+                'r': self.svg_settings.r,
                 'fill': grid_holder.colors[idx],
                 'class': 'agent',
             }
 
             if ego_idx is not None:
                 ego_x, ego_y = initial_positions[ego_idx]
                 is_out_of_radius = not self.check_in_radius(x, y, ego_x, ego_y, self.grid_config.obs_radius)
@@ -588,15 +588,15 @@
 
             if not any([agent_state.is_active() for agent_state in gh.history[agent_idx]]):
                 continue
 
             circle_settings = {"class": 'target'}
             circle_settings.update(cx=cfg.draw_start + x * cfg.scale_size,
                                    cy=cfg.draw_start + y * cfg.scale_size,
-                                   # r=cfg.r,
+                                   r=cfg.r,
                                    stroke=gh.colors[agent_idx],
                                    # stroke_width=cfg.stroke_width,
                                    # fill='none'
                                    )
             if animation_config.egocentric_idx is not None:
                 if animation_config.egocentric_idx != agent_idx:
                     continue
```

### Comparing `pogema-1.2.3a0/pogema/envs.py` & `pogema-1.2.3a1/pogema/envs.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.3a0/pogema/generator.py` & `pogema-1.2.3a1/pogema/generator.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.3a0/pogema/grid.py` & `pogema-1.2.3a1/pogema/grid.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.3a0/pogema/grid_config.py` & `pogema-1.2.3a1/pogema/grid_config.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.3a0/pogema/grid_registry.py` & `pogema-1.2.3a1/pogema/grid_registry.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.3a0/pogema/integrations/make_pogema.py` & `pogema-1.2.3a1/pogema/integrations/make_pogema.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.3a0/pogema/integrations/pettingzoo.py` & `pogema-1.2.3a1/pogema/integrations/pettingzoo.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.3a0/pogema/integrations/pymarl.py` & `pogema-1.2.3a1/pogema/integrations/pymarl.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.3a0/pogema/integrations/sample_factory.py` & `pogema-1.2.3a1/pogema/integrations/sample_factory.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.3a0/pogema/svg_objects.py` & `pogema-1.2.3a1/pogema/svg_objects.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.3a0/pogema/utils.py` & `pogema-1.2.3a1/pogema/utils.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.3a0/pogema/wrappers/metrics.py` & `pogema-1.2.3a1/pogema/wrappers/metrics.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.3a0/pogema/wrappers/multi_time_limit.py` & `pogema-1.2.3a1/pogema/wrappers/multi_time_limit.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.3a0/pogema/wrappers/persistence.py` & `pogema-1.2.3a1/pogema/wrappers/persistence.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.3a0/pogema.egg-info/PKG-INFO` & `pogema-1.2.3a1/pogema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pogema
-Version: 1.2.3a0
+Version: 1.2.3a1
 Summary: Partially Observable Grid Environment for Multiple Agents
 Home-page: https://github.com/AIRI-Institute/pogema
 Author: Alexey Skrynnik
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pogema-1.2.3a0/pogema.egg-info/SOURCES.txt` & `pogema-1.2.3a1/pogema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pogema-1.2.3a0/setup.py` & `pogema-1.2.3a1/setup.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.3a0/tests/test_deterministic_policy.py` & `pogema-1.2.3a1/tests/test_deterministic_policy.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.3a0/tests/test_grid.py` & `pogema-1.2.3a1/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.3a0/tests/test_integrations.py` & `pogema-1.2.3a1/tests/test_integrations.py`

 * *Files identical despite different names*

### Comparing `pogema-1.2.3a0/tests/test_pogema_env.py` & `pogema-1.2.3a1/tests/test_pogema_env.py`

 * *Files identical despite different names*

