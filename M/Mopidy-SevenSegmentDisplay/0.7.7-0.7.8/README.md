# Comparing `tmp/Mopidy-SevenSegmentDisplay-0.7.7.tar.gz` & `tmp/mopidy_sevensegmentdisplay-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mopidy-SevenSegmentDisplay-0.7.7.tar", last modified: Sun Apr  7 18:29:39 2024, max compression
+gzip compressed data, was "mopidy_sevensegmentdisplay-0.7.8.tar", last modified: Sun Apr 14 08:57:46 2024, max compression
```

## Comparing `Mopidy-SevenSegmentDisplay-0.7.7.tar` & `mopidy_sevensegmentdisplay-0.7.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:29:39.677513 Mopidy-SevenSegmentDisplay-0.7.7/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:29:39.677513 Mopidy-SevenSegmentDisplay-0.7.7/Mopidy_SevenSegmentDisplay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-07 18:29:39.000000 Mopidy-SevenSegmentDisplay-0.7.7/Mopidy_SevenSegmentDisplay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-07 18:29:39.000000 Mopidy-SevenSegmentDisplay-0.7.7/Mopidy_SevenSegmentDisplay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 18:29:39.000000 Mopidy-SevenSegmentDisplay-0.7.7/Mopidy_SevenSegmentDisplay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-07 18:29:39.000000 Mopidy-SevenSegmentDisplay-0.7.7/Mopidy_SevenSegmentDisplay.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 18:29:39.000000 Mopidy-SevenSegmentDisplay-0.7.7/Mopidy_SevenSegmentDisplay.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-07 18:29:39.000000 Mopidy-SevenSegmentDisplay-0.7.7/Mopidy_SevenSegmentDisplay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-07 18:29:39.000000 Mopidy-SevenSegmentDisplay-0.7.7/Mopidy_SevenSegmentDisplay.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-07 18:29:39.677513 Mopidy-SevenSegmentDisplay-0.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:29:39.677513 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/actor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/animation.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/cava.config
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/clock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/equalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/ext.conf
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/gpio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/ir.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/led.py
--rw-r--r--   0 runner    (1001) docker     (127)    25861 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/lib_nrf24.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/light_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/max7219.py
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)    14070 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/music.py
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:29:39.677513 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/static/
--rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/static/alwan.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    11556 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/static/alwan.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    18860 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/static/bootstrap-theme.css
--rw-r--r--   0 runner    (1001) docker     (127)   109518 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/static/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)    31819 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/static/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (127)    95786 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/static/jquery.js
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/static/theme.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:29:39.677513 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/threader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13591 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-07 18:29:39.677513 Mopidy-SevenSegmentDisplay-0.7.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-07 18:29:35.000000 Mopidy-SevenSegmentDisplay-0.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:57:46.363793 mopidy_sevensegmentdisplay-0.7.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:57:46.363793 mopidy_sevensegmentdisplay-0.7.8/Mopidy_SevenSegmentDisplay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-14 08:57:46.000000 mopidy_sevensegmentdisplay-0.7.8/Mopidy_SevenSegmentDisplay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-14 08:57:46.000000 mopidy_sevensegmentdisplay-0.7.8/Mopidy_SevenSegmentDisplay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 08:57:46.000000 mopidy_sevensegmentdisplay-0.7.8/Mopidy_SevenSegmentDisplay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-14 08:57:46.000000 mopidy_sevensegmentdisplay-0.7.8/Mopidy_SevenSegmentDisplay.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 08:57:46.000000 mopidy_sevensegmentdisplay-0.7.8/Mopidy_SevenSegmentDisplay.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-14 08:57:46.000000 mopidy_sevensegmentdisplay-0.7.8/Mopidy_SevenSegmentDisplay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-14 08:57:46.000000 mopidy_sevensegmentdisplay-0.7.8/Mopidy_SevenSegmentDisplay.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-14 08:57:46.363793 mopidy_sevensegmentdisplay-0.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:57:46.363793 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/cava.config
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/equalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/ext.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/led.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25861 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/lib_nrf24.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/light_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/max7219.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14070 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/music.py
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:57:46.363793 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/static/alwan.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    11556 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/static/alwan.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18860 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/static/bootstrap-theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)   109518 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/static/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)    31819 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/static/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)    95786 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/static/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/static/theme.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:57:46.363793 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/threader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13572 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-14 08:57:46.363793 mopidy_sevensegmentdisplay-0.7.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-14 08:57:42.000000 mopidy_sevensegmentdisplay-0.7.8/setup.py
```

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/LICENSE` & `mopidy_sevensegmentdisplay-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/Mopidy_SevenSegmentDisplay.egg-info/PKG-INFO` & `mopidy_sevensegmentdisplay-0.7.8/Mopidy_SevenSegmentDisplay.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mopidy-SevenSegmentDisplay
-Version: 0.7.7
+Version: 0.7.8
 Summary: A Mopidy extension for using it with seven segment display.
 Home-page: https://github.com/JumalIO/mopidy-sevensegmentdisplay
 Author: Julius
 Author-email: spamjulius@mail.com
 Maintainer: Julius
 Maintainer-email: spamjulius@mail.com
 License: Apache License, Version 2.0
```

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/Mopidy_SevenSegmentDisplay.egg-info/SOURCES.txt` & `mopidy_sevensegmentdisplay-0.7.8/Mopidy_SevenSegmentDisplay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/PKG-INFO` & `mopidy_sevensegmentdisplay-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mopidy-SevenSegmentDisplay
-Version: 0.7.7
+Version: 0.7.8
 Summary: A Mopidy extension for using it with seven segment display.
 Home-page: https://github.com/JumalIO/mopidy-sevensegmentdisplay
 Author: Julius
 Author-email: spamjulius@mail.com
 Maintainer: Julius
 Maintainer-email: spamjulius@mail.com
 License: Apache License, Version 2.0
```

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/README.md` & `mopidy_sevensegmentdisplay-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/__init__.py` & `mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from mopidy import config, ext
 from .http import factory_decorator
 from .actor import Frontend
 
-__version__ = '0.7.7'
+__version__ = '0.7.8'
 
 
 class Extension(ext.Extension):
     dist_name = 'Mopidy-SevenSegmentDisplay'
     ext_name = 'sevensegmentdisplay'
     version = __version__
 
@@ -31,14 +31,15 @@
         schema['light_sensor_time_from'] = config.Integer()
         schema['light_sensor_time_to'] = config.Integer()
         schema['alert_files'] = config.String(optional=True)
         schema['display_min_brightness'] = config.Integer()
         schema['display_max_brightness'] = config.Integer()
         schema['equalizer_enabled'] = config.Boolean()
         schema['led_enabled'] = config.Boolean()
+        schema['led_pipes'] = config.String(optional=True)
         return schema
 
     def setup(self, registry):
         registry.add('frontend', Frontend)
         registry.add('http:app', {
             'name': self.ext_name,
             'factory': factory_decorator(Frontend.worker),
```

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/actor.py` & `mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/actor.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/alert.py` & `mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/alert.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/animation.py` & `mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/animation.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/clock.py` & `mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/clock.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/display.py` & `mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/display.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/equalizer.py` & `mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/equalizer.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/ext.conf` & `mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/ext.conf`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 light_sensor_time_to = 4
 
 display_min_brightness = 2
 display_max_brightness = 15
 
 equalizer_enabled = true
 led_enabled = true
+led_pipes = [[135, 34, 67, 64, 72], [135, 3, 18, 56, 72]]
 
 alert_files = [
 				  { "name": "sounds/01.mp3", "volume": 15000, "repeat": 1, "enabled": true, "rating": "++" },
 				  { "name": "sounds/02.mp3", "volume": 15000, "repeat": 1, "enabled": true, "rating": "++" },
 				  { "name": "sounds/03.mp3", "volume": 15000, "repeat": 1, "enabled": true, "rating": "++" },
 				  { "name": "sounds/04.mp3", "volume": 15000, "repeat": 1, "enabled": true, "rating": "++" },
 				  { "name": "sounds/05.mp3", "volume": 15000, "repeat": 1, "enabled": true, "rating": "++" },
```

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/gpio.py` & `mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/gpio.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/http.py` & `mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/http.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/ir.py` & `mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/ir.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/led.py` & `mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/led.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import colorsys
 import random
+import json
 import logging
+import time
 import RPi.GPIO as GPIO
 from .lib_nrf24 import NRF24
+from .threader import Threader
 
 
-class Led:
+class Led(Threader):
 
-    def __init__(self, led_enabled):
+    def __init__(self, led_enabled, pipes):
         self._radio = None
-        self._pipes = []
+        self._pipes = json.loads(pipes)
         self._size = 8
 
         if (not led_enabled):
             return
 
         GPIO.setmode(GPIO.BCM)
 
@@ -34,54 +37,62 @@
         self._radio.setDataRate(NRF24.BR_1MBPS)
         self._radio.setPALevel(NRF24.PA_MAX)
         self._radio.setAutoAck(True)
         self._radio.openReadingPipe(1, readingPipe)
 
         self._radio.startListening()
 
+        super(Led, self).start()
+
     def run(self):
-        if self._radio.available():
-            r = []
+        while (True):
+            if (self.stopped()):
+                break
 
-            self._radio.read(r, self._size)
+            if (self._radio.available()):
+                data = []
 
-            logging.info(r)
+                self._radio.read(data, self._size)
 
-            if (r[0] != 1):
-                return
+                logging.info(data)
 
-            for pipe in self._pipes:
-                if (pipe[0] == r[1] and
-                    pipe[1] == r[2] and
-                    pipe[2] == r[3] and
-                    pipe[3] == r[4] and
-                    pipe[4] == r[5]):
+                if (data[0] != 1):
                     return
 
-            self._pipes.append([r[1], r[2], r[3], r[4], r[5]])
+                newPipe = [data[1], data[2], data[3], data[4], data[5]]
+
+                self._radio.stopListening()
+                self._send(newPipe, data)
+                self._radio.startListening()
+
+                for pipe in self._pipes:
+                    if (pipe[0] == newPipe[1] and
+                        pipe[1] == newPipe[2] and
+                        pipe[2] == newPipe[3] and
+                        pipe[3] == newPipe[4] and
+                        pipe[4] == newPipe[5]):
+                        return
+
+                self._pipes.append(newPipe)
+
+            time.sleep(0.2)
+
+    def stop(self):
+        self.set_none_color()
+        super(Led, self).stop()
 
     def set_color(self, red, green, blue):
         try:
             if self._radio is None:
                 return
 
             self._radio.stopListening()
 
             for pipe in self._pipes:
-                self._radio.openWritingPipe(pipe);
-
-                self._radio.write([0, red, green, blue])
-
-                if self._radio.isAckPayloadAvailable():
-                    buffer = []
-                    self._radio.read(buffer, self._radio.getDynamicPayloadSize())
-                    logging.info("NRF24 ACK Received:"),
-                    logging.info(buffer)
-                else:
-                    logging.info("Received: Ack only, no payload")
+                self._send(pipe, [0, red, green, blue])
 
             self._radio.startListening()
         except Exception as inst:
             logging.error(inst)
 
     def set_color_hsv(self, hue, sat = 1, val = 1):
         c = colorsys.hsv_to_rgb(hue / 360.0, sat, val)
@@ -89,7 +100,20 @@
         self.set_color(int(c[0] * 255), int(c[1] * 255), int(c[2] * 255))
 
     def set_random_color(self):
         self.set_color_hsv(random.random() * 360)
 
     def set_none_color(self):
         self.set_color(0, 0, 0)
+
+    def _send(self, pipe, data):
+        self._radio.openWritingPipe(pipe);
+
+        self._radio.write(data)
+
+        if self._radio.isAckPayloadAvailable():
+            buffer = []
+            self._radio.read(buffer, self._radio.getDynamicPayloadSize())
+            logging.info("NRF24 ACK Received:"),
+            logging.info(buffer)
+        else:
+            logging.info("Received: Ack only, no payload")
```

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/lib_nrf24.py` & `mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/lib_nrf24.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/light_sensor.py` & `mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/light_sensor.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/max7219.py` & `mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/max7219.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/menu.py` & `mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/menu.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/music.py` & `mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/music.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/static/alwan.min.css` & `mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/static/alwan.min.css`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/static/alwan.min.js` & `mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/static/alwan.min.js`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/static/bootstrap-theme.css` & `mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/static/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/static/bootstrap.css` & `mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/static/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/static/bootstrap.js` & `mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/static/bootstrap.js`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/static/jquery.js` & `mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/static/jquery.js`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/templates/base.html` & `mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/templates/base.html`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/templates/index.html` & `mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/templates/index.html`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/timer.py` & `mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/timer.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/mopidy_sevensegmentdisplay/worker.py` & `mopidy_sevensegmentdisplay-0.7.8/mopidy_sevensegmentdisplay/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             self.gpio = Gpio(
                 self.config['buttons_enabled'],
                 self.play_stop_music,
                 self._on_menu_click,
                 self._on_menu_click_left,
                 self._on_menu_click_right,
                 self.config['relay_enabled'])
-            self.led = Led(self.config['led_enabled'])
+            self.led = Led(self.config['led_enabled'], self.config['led_pipes'])
             self.ir_sender = IrSender(self.config['ir_remote'], self.gpio.switch_relay)
             self.timer_on = TimerOn(self.play_music)
             self.timer_off = TimerOff(self.stop_music)
             self.alert = Alert(self.music,
                                self.ir_sender,
                                self.config['alert_files'])
             self.timer_alert = TimerAlert(self.run_alert)
@@ -80,23 +80,22 @@
                     break
 
                 if (self.equalizer.is_visible() and not self.menu.is_sub_menu_visible()):
                     self.equalizer.run()
                 else:
                     self.equalizer.stop()
                     self.menu.run()
-                    self.led.run()
                     sleep(1)
 
         except Exception as inst:
             logging.error(inst)
         finally:
             self.equalizer.stop()
             self.ir_sender.stop()
-            self.led.set_none_color()
+            self.led.stop()
             self.gpio.cleanup()
             self.display.stop()
             self.light_sensor.stop()
 
     def _init_menu(self):
         self.MENU = {
             "get_sub_menu": lambda: [
```

### Comparing `Mopidy-SevenSegmentDisplay-0.7.7/setup.py` & `mopidy_sevensegmentdisplay-0.7.8/setup.py`

 * *Files identical despite different names*

