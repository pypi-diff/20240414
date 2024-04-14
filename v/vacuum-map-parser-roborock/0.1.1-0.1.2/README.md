# Comparing `tmp/vacuum_map_parser_roborock-0.1.1.tar.gz` & `tmp/vacuum_map_parser_roborock-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vacuum_map_parser_roborock-0.1.1.tar", max compression
+gzip compressed data, was "vacuum_map_parser_roborock-0.1.2.tar", max compression
```

## Comparing `vacuum_map_parser_roborock-0.1.1.tar` & `vacuum_map_parser_roborock-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11345 2023-10-31 01:13:36.998592 vacuum_map_parser_roborock-0.1.1/LICENSE
--rw-r--r--   0        0        0     6095 2023-10-31 01:13:36.998592 vacuum_map_parser_roborock-0.1.1/README.md
--rw-r--r--   0        0        0     1953 2023-10-31 01:13:58.791502 vacuum_map_parser_roborock-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       55 2023-10-31 01:13:36.998592 vacuum_map_parser_roborock-0.1.1/src/vacuum_map_parser_roborock/__init__.py
--rw-r--r--   0        0        0     4527 2023-10-31 01:13:36.998592 vacuum_map_parser_roborock-0.1.1/src/vacuum_map_parser_roborock/image_parser.py
--rw-r--r--   0        0        0    17974 2023-10-31 01:13:36.998592 vacuum_map_parser_roborock-0.1.1/src/vacuum_map_parser_roborock/map_data_parser.py
--rw-r--r--   0        0        0        0 2023-10-31 01:13:36.998592 vacuum_map_parser_roborock-0.1.1/src/vacuum_map_parser_roborock/py.typed
--rw-r--r--   0        0        0     7190 1970-01-01 00:00:00.000000 vacuum_map_parser_roborock-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11345 2024-04-14 01:13:42.766067 vacuum_map_parser_roborock-0.1.2/LICENSE
+-rw-r--r--   0        0        0     6095 2024-04-14 01:13:42.770067 vacuum_map_parser_roborock-0.1.2/README.md
+-rw-r--r--   0        0        0     1953 2024-04-14 01:13:56.974103 vacuum_map_parser_roborock-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       55 2024-04-14 01:13:42.770067 vacuum_map_parser_roborock-0.1.2/src/vacuum_map_parser_roborock/__init__.py
+-rw-r--r--   0        0        0     5051 2024-04-14 01:13:42.770067 vacuum_map_parser_roborock-0.1.2/src/vacuum_map_parser_roborock/image_parser.py
+-rw-r--r--   0        0        0    18242 2024-04-14 01:13:42.770067 vacuum_map_parser_roborock-0.1.2/src/vacuum_map_parser_roborock/map_data_parser.py
+-rw-r--r--   0        0        0        0 2024-04-14 01:13:42.770067 vacuum_map_parser_roborock-0.1.2/src/vacuum_map_parser_roborock/py.typed
+-rw-r--r--   0        0        0     7190 1970-01-01 00:00:00.000000 vacuum_map_parser_roborock-0.1.2/PKG-INFO
```

### Comparing `vacuum_map_parser_roborock-0.1.1/LICENSE` & `vacuum_map_parser_roborock-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vacuum_map_parser_roborock-0.1.1/README.md` & `vacuum_map_parser_roborock-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `vacuum_map_parser_roborock-0.1.1/pyproject.toml` & `vacuum_map_parser_roborock-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "vacuum-map-parser-roborock"
 # The version is set by GH action on release
-version = "0.1.1"
+version = "0.1.2"
 license = "Apache-2.0"
 description = "Functionalities for Roborock vacuum map parsing"
 readme = "README.md"
 authors = ["Piotr Machowski <piotr.machowski.dev@gmail.com>"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -22,15 +22,15 @@
 "Repository" = "https://github.com/PiotrMachowski/Python-package-vacuum-map-parser-roborock"
 "Bug Tracker" = "https://github.com/PiotrMachowski/Python-package-vacuum-map-parser-roborock/issues"
 "Changelog" = "https://github.com/PiotrMachowski/Python-package-vacuum-map-parser-roborock/releases"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 Pillow = "*"
-vacuum-map-parser-base = "0.1.2"
+vacuum-map-parser-base = "0.1.3"
 
 [tool.poetry.dev-dependencies]
 black = "*"
 mypy = "*"
 ruff = "*"
 isort = "*"
 pylint = "*"
```

### Comparing `vacuum_map_parser_roborock-0.1.1/src/vacuum_map_parser_roborock/image_parser.py` & `vacuum_map_parser_roborock-0.1.2/src/vacuum_map_parser_roborock/image_parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,62 +24,72 @@
         self._image_config = image_config
 
     def parse(
         self, raw_data: bytes, width: int, height: int, carpet_map: set[int] | None
     ) -> tuple[ImageType | None, dict[int, tuple[int, int, int, int]]]:
         rooms = {}
         scale = self._image_config.scale
+        cached_colors = self._colors_palette.cached_colors
+        cached_room_colors = self._colors_palette.cached_room_colors
         trim_left = int(self._image_config.trim.left * width / 100)
         trim_right = int(self._image_config.trim.right * width / 100)
         trim_top = int(self._image_config.trim.top * height / 100)
         trim_bottom = int(self._image_config.trim.bottom * height / 100)
         trimmed_height = height - trim_top - trim_bottom
         trimmed_width = width - trim_left - trim_right
+        trimmed_left_width = trim_left + width
         image = Image.new("RGBA", (trimmed_width, trimmed_height))
         if width == 0 or height == 0:
             return None, {}
         pixels = image.load()
         for img_y in range(trimmed_height):
+            img_x_offset = trimmed_left_width * (img_y + trim_bottom)
             for img_x in range(trimmed_width):
-                idx = img_x + trim_left + width * (img_y + trim_bottom)
+                idx = img_x + img_x_offset
                 pixel_type = raw_data[idx]
                 x = img_x
                 y = trimmed_height - img_y - 1
                 if carpet_map is not None and idx in carpet_map and (x + y) % 2:
-                    pixels[x, y] = self._colors_palette.get_color(SupportedColor.CARPETS)
+                    pixels[x, y] = cached_colors[SupportedColor.CARPETS]
                 elif pixel_type == RoborockImageParser.MAP_OUTSIDE:
-                    pixels[x, y] = self._colors_palette.get_color(SupportedColor.MAP_OUTSIDE)
+                    pixels[x, y] = cached_colors[SupportedColor.MAP_OUTSIDE]
                 elif pixel_type == RoborockImageParser.MAP_WALL:
-                    pixels[x, y] = self._colors_palette.get_color(SupportedColor.MAP_WALL)
+                    pixels[x, y] = cached_colors[SupportedColor.MAP_WALL]
                 elif pixel_type == RoborockImageParser.MAP_INSIDE:
-                    pixels[x, y] = self._colors_palette.get_color(SupportedColor.MAP_INSIDE)
+                    pixels[x, y] = cached_colors[SupportedColor.MAP_INSIDE]
                 elif pixel_type == RoborockImageParser.MAP_SCAN:
-                    pixels[x, y] = self._colors_palette.get_color(SupportedColor.SCAN)
+                    pixels[x, y] = cached_colors[SupportedColor.SCAN]
                 else:
                     obstacle = pixel_type & 0x07
                     if obstacle == 0:
-                        pixels[x, y] = self._colors_palette.get_color(SupportedColor.GREY_WALL)
+                        pixels[x, y] = cached_colors[SupportedColor.GREY_WALL]
                     elif obstacle == 1:
-                        pixels[x, y] = self._colors_palette.get_color(SupportedColor.MAP_WALL_V2)
+                        pixels[x, y] = cached_colors[SupportedColor.MAP_WALL_V2]
                     elif obstacle == 7:
                         room_number = RoborockImageParser._get_room_number(pixel_type)
                         room_x = img_x + trim_left
                         room_y = img_y + trim_bottom
                         if room_number not in rooms:
                             rooms[room_number] = (room_x, room_y, room_x, room_y)
                         else:
                             rooms[room_number] = (
                                 min(rooms[room_number][0], room_x),
                                 min(rooms[room_number][1], room_y),
                                 max(rooms[room_number][2], room_x),
                                 max(rooms[room_number][3], room_y),
                             )
-                        pixels[x, y] = self._colors_palette.get_room_color(room_number)
+                        try:
+                            pixels[x, y] = cached_room_colors[room_number]
+                        except KeyError:
+                            # Since rooms can go above the 16 we preprocess, we handle the key error here and add it to
+                            # our local version of the cache and the real cache.
+                            cached_room_colors[room_number] = self._colors_palette.get_room_color(room_number)
+                            pixels[x, y] = cached_room_colors[room_number]
                     else:
-                        pixels[x, y] = self._colors_palette.get_color(SupportedColor.UNKNOWN)
+                        pixels[x, y] = cached_colors[SupportedColor.UNKNOWN]
         if scale != 1 and width != 0 and height != 0:
             image = image.resize((int(trimmed_width * scale), int(trimmed_height * scale)), resample=Resampling.NEAREST)
         return image, rooms
 
     @staticmethod
     def get_room_at_pixel(raw_data: bytes, width: int, x: int, y: int) -> int | None:
         room_number = None
```

### Comparing `vacuum_map_parser_roborock-0.1.1/src/vacuum_map_parser_roborock/map_data_parser.py` & `vacuum_map_parser_roborock-0.1.2/src/vacuum_map_parser_roborock/map_data_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,19 +55,29 @@
 
 
 class RoborockMapDataParser(MapDataParser):
     """Roborock map parser."""
 
     KNOWN_OBSTACLE_TYPES = {
         0: "cable",
+        1: "pet waste",
         2: "shoes",
         3: "poop",
+        4: "pedestal",
         5: "extension cord",
         9: "weighting scale",
         10: "clothes",
+        25: "dustpan",
+        26: "furniture with a crossbar",
+        27: "furniture with a crossbar",
+        34: "clothes",
+        48: "cable",
+        49: "pet",
+        50: "pet",
+        51: "fabric/paper balls",
     }
 
     def __init__(
         self,
         palette: ColorsPalette,
         sizes: Sizes,
         drawables: list[Drawable],
```

### Comparing `vacuum_map_parser_roborock-0.1.1/PKG-INFO` & `vacuum_map_parser_roborock-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: vacuum-map-parser-roborock
-Version: 0.1.1
+Version: 0.1.2
 Summary: Functionalities for Roborock vacuum map parsing
 License: Apache-2.0
 Author: Piotr Machowski
 Author-email: piotr.machowski.dev@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Home Automation
 Requires-Dist: Pillow
-Requires-Dist: vacuum-map-parser-base (==0.1.2)
+Requires-Dist: vacuum-map-parser-base (==0.1.3)
 Project-URL: Bug Tracker, https://github.com/PiotrMachowski/Python-package-vacuum-map-parser-roborock/issues
 Project-URL: Changelog, https://github.com/PiotrMachowski/Python-package-vacuum-map-parser-roborock/releases
 Project-URL: Homepage, https://github.com/PiotrMachowski/Python-package-vacuum-map-parser-roborock
 Project-URL: Repository, https://github.com/PiotrMachowski/Python-package-vacuum-map-parser-roborock
 Description-Content-Type: text/markdown
 
 [![GitHub Latest Release][releases_shield]][latest_release]
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: vacuum-map-parser-roborock Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: vacuum-map-parser-roborock Version: 0.1.2 Summary:
 Functionalities for Roborock vacuum map parsing License: Apache-2.0 Author:
 Piotr Machowski Author-email: piotr.machowski.dev@gmail.com Requires-Python:
 >=3.11,<4.0 Classifier: Development Status :: 4 - Beta Classifier: Environment
 :: Console Classifier: Intended Audience :: Developers Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Home Automation Requires-Dist: Pillow Requires-Dist: vacuum-map-
-parser-base (==0.1.2) Project-URL: Bug Tracker, https://github.com/
+parser-base (==0.1.3) Project-URL: Bug Tracker, https://github.com/
 PiotrMachowski/Python-package-vacuum-map-parser-roborock/issues Project-URL:
 Changelog, https://github.com/PiotrMachowski/Python-package-vacuum-map-parser-
 roborock/releases Project-URL: Homepage, https://github.com/PiotrMachowski/
 Python-package-vacuum-map-parser-roborock Project-URL: Repository, https://
 github.com/PiotrMachowski/Python-package-vacuum-map-parser-roborock
 Description-Content-Type: text/markdown [![GitHub Latest Release]
 [releases_shield]][latest_release] [![PyPI][pypi_releases_shield]]
```

