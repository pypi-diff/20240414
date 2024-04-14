# Comparing `tmp/vacuum_map_parser_base-0.1.2.tar.gz` & `tmp/vacuum_map_parser_base-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vacuum_map_parser_base-0.1.2.tar", max compression
+gzip compressed data, was "vacuum_map_parser_base-0.1.3.tar", max compression
```

## Comparing `vacuum_map_parser_base-0.1.2.tar` & `vacuum_map_parser_base-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11345 2023-10-30 03:40:04.628897 vacuum_map_parser_base-0.1.2/LICENSE
--rw-r--r--   0        0        0     5375 2023-10-30 03:40:04.628897 vacuum_map_parser_base-0.1.2/README.md
--rw-r--r--   0        0        0     1865 2023-10-30 03:40:22.677307 vacuum_map_parser_base-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       69 2023-10-30 03:40:04.628897 vacuum_map_parser_base-0.1.2/src/vacuum_map_parser_base/__init__.py
--rw-r--r--   0        0        0       49 2023-10-30 03:40:04.628897 vacuum_map_parser_base-0.1.2/src/vacuum_map_parser_base/config/__init__.py
--rw-r--r--   0        0        0     5913 2023-10-30 03:40:04.628897 vacuum_map_parser_base-0.1.2/src/vacuum_map_parser_base/config/color.py
--rw-r--r--   0        0        0      754 2023-10-30 03:40:04.628897 vacuum_map_parser_base-0.1.2/src/vacuum_map_parser_base/config/drawable.py
--rw-r--r--   0        0        0      412 2023-10-30 03:40:04.628897 vacuum_map_parser_base-0.1.2/src/vacuum_map_parser_base/config/image_config.py
--rw-r--r--   0        0        0     1194 2023-10-30 03:40:04.628897 vacuum_map_parser_base-0.1.2/src/vacuum_map_parser_base/config/size.py
--rw-r--r--   0        0        0      323 2023-10-30 03:40:04.628897 vacuum_map_parser_base-0.1.2/src/vacuum_map_parser_base/config/text.py
--rw-r--r--   0        0        0    19048 2023-10-30 03:40:04.628897 vacuum_map_parser_base-0.1.2/src/vacuum_map_parser_base/image_generator.py
--rw-r--r--   0        0        0     9099 2023-10-30 03:40:04.628897 vacuum_map_parser_base-0.1.2/src/vacuum_map_parser_base/map_data.py
--rw-r--r--   0        0        0     1357 2023-10-30 03:40:04.628897 vacuum_map_parser_base-0.1.2/src/vacuum_map_parser_base/map_data_parser.py
--rw-r--r--   0        0        0        0 2023-10-30 03:40:04.628897 vacuum_map_parser_base-0.1.2/src/vacuum_map_parser_base/py.typed
--rw-r--r--   0        0        0     6389 1970-01-01 00:00:00.000000 vacuum_map_parser_base-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11345 2024-04-14 00:45:01.119876 vacuum_map_parser_base-0.1.3/LICENSE
+-rw-r--r--   0        0        0     5375 2024-04-14 00:45:01.119876 vacuum_map_parser_base-0.1.3/README.md
+-rw-r--r--   0        0        0     1865 2024-04-14 00:45:16.999854 vacuum_map_parser_base-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       69 2024-04-14 00:45:01.119876 vacuum_map_parser_base-0.1.3/src/vacuum_map_parser_base/__init__.py
+-rw-r--r--   0        0        0       49 2024-04-14 00:45:01.119876 vacuum_map_parser_base-0.1.3/src/vacuum_map_parser_base/config/__init__.py
+-rw-r--r--   0        0        0     6623 2024-04-14 00:45:01.119876 vacuum_map_parser_base-0.1.3/src/vacuum_map_parser_base/config/color.py
+-rw-r--r--   0        0        0      754 2024-04-14 00:45:01.119876 vacuum_map_parser_base-0.1.3/src/vacuum_map_parser_base/config/drawable.py
+-rw-r--r--   0        0        0      412 2024-04-14 00:45:01.119876 vacuum_map_parser_base-0.1.3/src/vacuum_map_parser_base/config/image_config.py
+-rw-r--r--   0        0        0     1194 2024-04-14 00:45:01.119876 vacuum_map_parser_base-0.1.3/src/vacuum_map_parser_base/config/size.py
+-rw-r--r--   0        0        0      323 2024-04-14 00:45:01.119876 vacuum_map_parser_base-0.1.3/src/vacuum_map_parser_base/config/text.py
+-rw-r--r--   0        0        0    19048 2024-04-14 00:45:01.119876 vacuum_map_parser_base-0.1.3/src/vacuum_map_parser_base/image_generator.py
+-rw-r--r--   0        0        0     9099 2024-04-14 00:45:01.119876 vacuum_map_parser_base-0.1.3/src/vacuum_map_parser_base/map_data.py
+-rw-r--r--   0        0        0     1357 2024-04-14 00:45:01.119876 vacuum_map_parser_base-0.1.3/src/vacuum_map_parser_base/map_data_parser.py
+-rw-r--r--   0        0        0        0 2024-04-14 00:45:01.119876 vacuum_map_parser_base-0.1.3/src/vacuum_map_parser_base/py.typed
+-rw-r--r--   0        0        0     6389 1970-01-01 00:00:00.000000 vacuum_map_parser_base-0.1.3/PKG-INFO
```

### Comparing `vacuum_map_parser_base-0.1.2/LICENSE` & `vacuum_map_parser_base-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vacuum_map_parser_base-0.1.2/README.md` & `vacuum_map_parser_base-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `vacuum_map_parser_base-0.1.2/pyproject.toml` & `vacuum_map_parser_base-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "vacuum-map-parser-base"
 # The version is set by GH action on release
-version = "0.1.2"
+version = "0.1.3"
 license = "Apache-2.0"
 description = "Common code for vacuum map parsers"
 readme = "README.md"
 authors = ["Piotr Machowski <piotr.machowski.dev@gmail.com>"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

### Comparing `vacuum_map_parser_base-0.1.2/src/vacuum_map_parser_base/config/color.py` & `vacuum_map_parser_base-0.1.3/src/vacuum_map_parser_base/config/color.py`

 * *Files 8% similar despite different names*

```diff
@@ -113,39 +113,55 @@
             self._overriden_colors = {}
         else:
             self._overriden_colors = colors_dict
         if room_colors is None:
             self._overriden_room_colors = {}
         else:
             self._overriden_room_colors = room_colors
+        # Create it once so that it can be accessed in get_color in the future
         self._cached_colors: dict[SupportedColor, Color] = {}
-        self._cached_room_colors: dict[int, Color] = {}
+        for color in self.COLORS:
+            self.get_color(color)
+        # Create it once so that it can be accessed in get_room_color in the future
+        self._cached_room_colors: dict[int | str, Color] = {}
+        for room in self.ROOM_COLORS:
+            self.get_room_color(room)
 
     def get_color(self, color_name: SupportedColor) -> Color:
         if color_name not in self._cached_colors:
             if color_name in self._overriden_colors:
                 val = self._overriden_colors[color_name]
             elif color_name in ColorsPalette.COLORS:
                 val = ColorsPalette.COLORS[color_name]
             elif SupportedColor.UNKNOWN in ColorsPalette.COLORS:
                 val = ColorsPalette.COLORS[SupportedColor.UNKNOWN]
             else:
-                val = (0,0,0)
+                val = (0, 0, 0)
             self._cached_colors[color_name] = val
         return self._cached_colors[color_name]
 
+    @property
+    def cached_colors(self) -> dict[SupportedColor, Color]:
+        return self._cached_colors
+
     def get_room_color(self, room_id: str | int) -> Color:
-        if isinstance(room_id, str):
-            room_id = int(room_id)
         if room_id not in self._cached_room_colors:
+            if isinstance(room_id, str):
+                room_id = int(room_id)
             if room_id > len(ColorsPalette.ROOM_COLORS):
                 room_id = (room_id - 1) % len(ColorsPalette.ROOM_COLORS) + 1
 
             key = str(room_id)
             if key in self._overriden_room_colors:
                 val = self._overriden_room_colors[key]
             elif key in ColorsPalette.ROOM_COLORS:
                 val = ColorsPalette.ROOM_COLORS[key]
             else:
                 val = ColorsPalette.ROOM_COLORS.get(str(self._random.randint(1, 16)), (0, 0, 0))
-            self._cached_room_colors[room_id] = val
+            # ensure we have both str and int in the dictionary so we don't have to always convert.
+            self._cached_room_colors[str(room_id)] = val
+            self._cached_room_colors[int(room_id)] = val
         return self._cached_room_colors[room_id]
+
+    @property
+    def cached_room_colors(self) -> dict[str | int, Color]:
+        return self._cached_room_colors
```

### Comparing `vacuum_map_parser_base-0.1.2/src/vacuum_map_parser_base/config/drawable.py` & `vacuum_map_parser_base-0.1.3/src/vacuum_map_parser_base/config/drawable.py`

 * *Files identical despite different names*

### Comparing `vacuum_map_parser_base-0.1.2/src/vacuum_map_parser_base/config/size.py` & `vacuum_map_parser_base-0.1.3/src/vacuum_map_parser_base/config/size.py`

 * *Files identical despite different names*

### Comparing `vacuum_map_parser_base-0.1.2/src/vacuum_map_parser_base/image_generator.py` & `vacuum_map_parser_base-0.1.3/src/vacuum_map_parser_base/image_generator.py`

 * *Files identical despite different names*

### Comparing `vacuum_map_parser_base-0.1.2/src/vacuum_map_parser_base/map_data.py` & `vacuum_map_parser_base-0.1.3/src/vacuum_map_parser_base/map_data.py`

 * *Files identical despite different names*

### Comparing `vacuum_map_parser_base-0.1.2/src/vacuum_map_parser_base/map_data_parser.py` & `vacuum_map_parser_base-0.1.3/src/vacuum_map_parser_base/map_data_parser.py`

 * *Files identical despite different names*

### Comparing `vacuum_map_parser_base-0.1.2/PKG-INFO` & `vacuum_map_parser_base-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vacuum-map-parser-base
-Version: 0.1.2
+Version: 0.1.3
 Summary: Common code for vacuum map parsers
 License: Apache-2.0
 Author: Piotr Machowski
 Author-email: piotr.machowski.dev@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vacuum-map-parser-base Version: 0.1.2 Summary:
+Metadata-Version: 2.1 Name: vacuum-map-parser-base Version: 0.1.3 Summary:
 Common code for vacuum map parsers License: Apache-2.0 Author: Piotr Machowski
 Author-email: piotr.machowski.dev@gmail.com Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic :: Home
 Automation Requires-Dist: Pillow Project-URL: Bug Tracker, https://github.com/
```

