# Comparing `tmp/svgen-0.6.5.tar.gz` & `tmp/svgen-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svgen-0.6.5.tar", last modified: Thu Apr  4 03:55:54 2024, max compression
+gzip compressed data, was "svgen-0.6.6.tar", last modified: Sun Apr 14 18:40:52 2024, max compression
```

## Comparing `svgen-0.6.5.tar` & `svgen-0.6.6.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:55:54.688024 svgen-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 03:54:44.000000 svgen-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-04 03:55:54.688024 svgen-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-04 03:54:44.000000 svgen-0.6.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-04 03:54:44.000000 svgen-0.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 03:55:54.688024 svgen-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-04 03:54:44.000000 svgen-0.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:55:54.680024 svgen-0.6.5/svgen/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:55:54.684024 svgen-0.6.5/svgen/attribute/
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/attribute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/attribute/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/attribute/viewbox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:55:54.684024 svgen-0.6.5/svgen/cartesian/
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/cartesian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/cartesian/circle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/cartesian/mutate.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/cartesian/plane.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/cartesian/point.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:55:54.684024 svgen-0.6.5/svgen/cartesian/rectangle/
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/cartesian/rectangle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/cartesian/rectangle/corner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/cartesian/rectangle/grid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:55:54.684024 svgen-0.6.5/svgen/color/
--rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/color/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/color/alpha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/color/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/color/hsl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/color/numbers.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/color/resolve.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/color/rgb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:55:54.684024 svgen-0.6.5/svgen/color/theme/
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/color/theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/color/theme/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/color/theme/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:55:54.680024 svgen-0.6.5/svgen/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:55:54.684024 svgen-0.6.5/svgen/data/themes/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/data/themes/blue_gray.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/data/themes/gray.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/display.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:55:54.688024 svgen-0.6.5/svgen/element/
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/element/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/element/circle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:55:54.688024 svgen-0.6.5/svgen/element/html/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/element/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/element/line.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/element/rect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/element/svg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:55:54.688024 svgen-0.6.5/svgen/generation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/generation/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/inkscape.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:55:54.688024 svgen-0.6.5/svgen/shapes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/shapes/chip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-04 03:54:44.000000 svgen-0.6.5/svgen/shapes/pins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:55:54.688024 svgen-0.6.5/svgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-04 03:55:54.000000 svgen-0.6.5/svgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-04 03:55:54.000000 svgen-0.6.5/svgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 03:55:54.000000 svgen-0.6.5/svgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-04 03:55:54.000000 svgen-0.6.5/svgen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-04 03:55:54.000000 svgen-0.6.5/svgen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 03:55:54.000000 svgen-0.6.5/svgen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:55:54.688024 svgen-0.6.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-04 03:54:44.000000 svgen-0.6.5/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-04 03:54:44.000000 svgen-0.6.5/tests/test_entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:40:52.381490 svgen-0.6.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-14 18:39:48.000000 svgen-0.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-14 18:40:52.381490 svgen-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-14 18:39:48.000000 svgen-0.6.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-14 18:39:48.000000 svgen-0.6.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 18:40:52.381490 svgen-0.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-14 18:39:48.000000 svgen-0.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:40:52.373490 svgen-0.6.6/svgen/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:40:52.373490 svgen-0.6.6/svgen/attribute/
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/attribute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/attribute/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/attribute/viewbox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:40:52.377490 svgen-0.6.6/svgen/cartesian/
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/cartesian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/cartesian/circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/cartesian/mutate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/cartesian/plane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/cartesian/point.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:40:52.377490 svgen-0.6.6/svgen/cartesian/rectangle/
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/cartesian/rectangle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/cartesian/rectangle/corner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/cartesian/rectangle/grid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:40:52.377490 svgen-0.6.6/svgen/color/
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/color/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/color/alpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/color/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/color/hsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/color/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/color/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/color/rgb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:40:52.377490 svgen-0.6.6/svgen/color/theme/
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/color/theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/color/theme/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/color/theme/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:40:52.369490 svgen-0.6.6/svgen/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:40:52.377490 svgen-0.6.6/svgen/data/themes/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/data/themes/blue_gray.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/data/themes/gray.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:40:52.377490 svgen-0.6.6/svgen/element/
+-rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/element/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/element/circle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:40:52.377490 svgen-0.6.6/svgen/element/html/
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/element/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/element/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/element/rect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/element/svg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:40:52.377490 svgen-0.6.6/svgen/generation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/generation/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/inkscape.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:40:52.381490 svgen-0.6.6/svgen/shapes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/shapes/chip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-14 18:39:48.000000 svgen-0.6.6/svgen/shapes/pins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:40:52.381490 svgen-0.6.6/svgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-14 18:40:52.000000 svgen-0.6.6/svgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-14 18:40:52.000000 svgen-0.6.6/svgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 18:40:52.000000 svgen-0.6.6/svgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-14 18:40:52.000000 svgen-0.6.6/svgen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-14 18:40:52.000000 svgen-0.6.6/svgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 18:40:52.000000 svgen-0.6.6/svgen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:40:52.381490 svgen-0.6.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-14 18:39:48.000000 svgen-0.6.6/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-14 18:39:48.000000 svgen-0.6.6/tests/test_entry.py
```

### Comparing `svgen-0.6.5/LICENSE` & `svgen-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/PKG-INFO` & `svgen-0.6.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svgen
-Version: 0.6.5
+Version: 0.6.6
 Summary: A tool for working with scalable vector graphics.
 Home-page: https://github.com/vkottler/svgen
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -34,19 +34,19 @@
 Requires-Dist: setuptools-wrapper; extra == "test"
 Requires-Dist: pytest; extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=30d78f3303f01ea73226bdd52314b30b
+    hash=43855c2a3e9dcda53e895aecb6a7ae61
     =====================================
 -->
 
-# svgen ([0.6.5](https://pypi.org/project/svgen/))
+# svgen ([0.6.6](https://pypi.org/project/svgen/))
 
 [![python](https://img.shields.io/pypi/pyversions/svgen.svg)](https://pypi.org/project/svgen/)
 ![Build Status](https://github.com/vkottler/svgen/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/svgen/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/svgen)
 ![PyPI - Status](https://img.shields.io/pypi/status/svgen)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/svgen)
 
@@ -80,15 +80,15 @@
 # Introduction
 
 This utility provides a means to work on graphics with a programmatic workflow.
 
 # Command-line Options
 
 ```
-$ ./venv3.11/bin/svgen -h
+$ ./venv3.12/bin/svgen -h
 
 usage: svgen [-h] [--version] [-v] [-q] [--curses] [--no-uvloop] [-C DIR]
              [-c CONFIG] [--height HEIGHT] [--width WIDTH] [--images]
              [-o OUTPUT]
              [scripts ...]
 
 A tool for working with scalable vector graphics.
```

### Comparing `svgen-0.6.5/README.md` & `svgen-0.6.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=30d78f3303f01ea73226bdd52314b30b
+    hash=43855c2a3e9dcda53e895aecb6a7ae61
     =====================================
 -->
 
-# svgen ([0.6.5](https://pypi.org/project/svgen/))
+# svgen ([0.6.6](https://pypi.org/project/svgen/))
 
 [![python](https://img.shields.io/pypi/pyversions/svgen.svg)](https://pypi.org/project/svgen/)
 ![Build Status](https://github.com/vkottler/svgen/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/svgen/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/svgen)
 ![PyPI - Status](https://img.shields.io/pypi/status/svgen)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/svgen)
 
@@ -44,15 +44,15 @@
 # Introduction
 
 This utility provides a means to work on graphics with a programmatic workflow.
 
 # Command-line Options
 
 ```
-$ ./venv3.11/bin/svgen -h
+$ ./venv3.12/bin/svgen -h
 
 usage: svgen [-h] [--version] [-v] [-q] [--curses] [--no-uvloop] [-C DIR]
              [-c CONFIG] [--height HEIGHT] [--width WIDTH] [--images]
              [-o OUTPUT]
              [scripts ...]
 
 A tool for working with scalable vector graphics.
```

### Comparing `svgen-0.6.5/pyproject.toml` & `svgen-0.6.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "svgen"
-version = "0.6.5"
+version = "0.6.6"
 description = "A tool for working with scalable vector graphics."
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `svgen-0.6.5/setup.py` & `svgen-0.6.6/setup.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/app.py` & `svgen-0.6.6/svgen/app.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/attribute/__init__.py` & `svgen-0.6.6/svgen/attribute/__init__.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/attribute/style.py` & `svgen-0.6.6/svgen/attribute/style.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/attribute/viewbox.py` & `svgen-0.6.6/svgen/attribute/viewbox.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/cartesian/__init__.py` & `svgen-0.6.6/svgen/cartesian/__init__.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/cartesian/circle.py` & `svgen-0.6.6/svgen/cartesian/circle.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/cartesian/mutate.py` & `svgen-0.6.6/svgen/cartesian/mutate.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/cartesian/plane.py` & `svgen-0.6.6/svgen/cartesian/plane.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/cartesian/point.py` & `svgen-0.6.6/svgen/cartesian/point.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/cartesian/rectangle/__init__.py` & `svgen-0.6.6/svgen/cartesian/rectangle/__init__.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/cartesian/rectangle/corner.py` & `svgen-0.6.6/svgen/cartesian/rectangle/corner.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/cartesian/rectangle/grid.py` & `svgen-0.6.6/svgen/cartesian/rectangle/grid.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/color/__init__.py` & `svgen-0.6.6/svgen/color/__init__.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/color/alpha.py` & `svgen-0.6.6/svgen/color/alpha.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/color/conversion.py` & `svgen-0.6.6/svgen/color/conversion.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/color/hsl.py` & `svgen-0.6.6/svgen/color/hsl.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/color/numbers.py` & `svgen-0.6.6/svgen/color/numbers.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/color/rgb.py` & `svgen-0.6.6/svgen/color/rgb.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/color/theme/__init__.py` & `svgen-0.6.6/svgen/color/theme/__init__.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/color/theme/manager.py` & `svgen-0.6.6/svgen/color/theme/manager.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/color/theme/visualize.py` & `svgen-0.6.6/svgen/color/theme/visualize.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/display.py` & `svgen-0.6.6/svgen/display.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/element/__init__.py` & `svgen-0.6.6/svgen/element/__init__.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/element/circle.py` & `svgen-0.6.6/svgen/element/circle.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/element/line.py` & `svgen-0.6.6/svgen/element/line.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/element/rect.py` & `svgen-0.6.6/svgen/element/rect.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/element/svg.py` & `svgen-0.6.6/svgen/element/svg.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/entry.py` & `svgen-0.6.6/svgen/entry.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/generation/images.py` & `svgen-0.6.6/svgen/generation/images.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/inkscape.py` & `svgen-0.6.6/svgen/inkscape.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/shapes/chip.py` & `svgen-0.6.6/svgen/shapes/chip.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen/shapes/pins.py` & `svgen-0.6.6/svgen/shapes/pins.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/svgen.egg-info/PKG-INFO` & `svgen-0.6.6/svgen.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svgen
-Version: 0.6.5
+Version: 0.6.6
 Summary: A tool for working with scalable vector graphics.
 Home-page: https://github.com/vkottler/svgen
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -34,19 +34,19 @@
 Requires-Dist: setuptools-wrapper; extra == "test"
 Requires-Dist: pytest; extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=30d78f3303f01ea73226bdd52314b30b
+    hash=43855c2a3e9dcda53e895aecb6a7ae61
     =====================================
 -->
 
-# svgen ([0.6.5](https://pypi.org/project/svgen/))
+# svgen ([0.6.6](https://pypi.org/project/svgen/))
 
 [![python](https://img.shields.io/pypi/pyversions/svgen.svg)](https://pypi.org/project/svgen/)
 ![Build Status](https://github.com/vkottler/svgen/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/svgen/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/svgen)
 ![PyPI - Status](https://img.shields.io/pypi/status/svgen)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/svgen)
 
@@ -80,15 +80,15 @@
 # Introduction
 
 This utility provides a means to work on graphics with a programmatic workflow.
 
 # Command-line Options
 
 ```
-$ ./venv3.11/bin/svgen -h
+$ ./venv3.12/bin/svgen -h
 
 usage: svgen [-h] [--version] [-v] [-q] [--curses] [--no-uvloop] [-C DIR]
              [-c CONFIG] [--height HEIGHT] [--width WIDTH] [--images]
              [-o OUTPUT]
              [scripts ...]
 
 A tool for working with scalable vector graphics.
```

### Comparing `svgen-0.6.5/svgen.egg-info/SOURCES.txt` & `svgen-0.6.6/svgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/tests/test_display.py` & `svgen-0.6.6/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `svgen-0.6.5/tests/test_entry.py` & `svgen-0.6.6/tests/test_entry.py`

 * *Files identical despite different names*

