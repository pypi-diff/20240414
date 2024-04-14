# Comparing `tmp/mousepad-0.1.1.tar.gz` & `tmp/mousepad-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mousepad-0.1.1.tar", last modified: Sun Apr 14 01:02:17 2024, max compression
+gzip compressed data, was "mousepad-0.1.2.tar", last modified: Sun Apr 14 01:37:13 2024, max compression
```

## Comparing `mousepad-0.1.1.tar` & `mousepad-0.1.2.tar`

### file list

```diff
@@ -1,96 +1,87 @@
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.185560 mousepad-0.1.1/
--rw-r--r--   0 neetish    (501) staff       (20)     1070 2024-04-13 21:42:28.000000 mousepad-0.1.1/LICENSE
--rw-r--r--   0 neetish    (501) staff       (20)     1634 2024-04-14 01:02:17.185318 mousepad-0.1.1/PKG-INFO
--rw-r--r--   0 neetish    (501) staff       (20)      972 2024-04-13 21:44:17.000000 mousepad-0.1.1/README.md
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.086873 mousepad-0.1.1/mousepad/
--rw-r--r--   0 neetish    (501) staff       (20)     6148 2024-04-14 00:55:41.000000 mousepad-0.1.1/mousepad/.DS_Store
--rw-r--r--   0 neetish    (501) staff       (20)     5832 2024-04-14 00:55:14.000000 mousepad-0.1.1/mousepad/__main__.py
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.084940 mousepad-0.1.1/mousepad/webbuild/
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.092798 mousepad-0.1.1/mousepad/webbuild/flutter_assets/
--rw-r--r--   0 neetish    (501) staff       (20)     6148 2024-04-14 00:57:30.000000 mousepad-0.1.1/mousepad/webbuild/flutter_assets/.DS_Store
--rw-r--r--   0 neetish    (501) staff       (20)      764 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/flutter_assets/AssetManifest.bin
--rw-r--r--   0 neetish    (501) staff       (20)     1022 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/flutter_assets/AssetManifest.bin.json
--rw-r--r--   0 neetish    (501) staff       (20)      707 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/flutter_assets/AssetManifest.json
--rw-r--r--   0 neetish    (501) staff       (20)      670 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/flutter_assets/FontManifest.json
--rw-r--r--   0 neetish    (501) staff       (20)  1729644 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/flutter_assets/NOTICES
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.084356 mousepad-0.1.1/mousepad/webbuild/flutter_assets/assets/
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.096296 mousepad-0.1.1/mousepad/webbuild/flutter_assets/assets/images/
--rw-r--r--   0 neetish    (501) staff       (20)     4980 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/flutter_assets/assets/images/AirDrop.svg
--rw-r--r--   0 neetish    (501) staff       (20)      974 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/flutter_assets/assets/images/display.svg
--rw-r--r--   0 neetish    (501) staff       (20)     1574 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/flutter_assets/assets/images/gaming.svg
--rw-r--r--   0 neetish    (501) staff       (20)     3805 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/flutter_assets/assets/images/keyboard.svg
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.096803 mousepad-0.1.1/mousepad/webbuild/flutter_assets/fonts/
--rw-rw-r--   0 neetish    (501) staff       (20)  1645184 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/flutter_assets/fonts/MaterialIcons-Regular.otf
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.099579 mousepad-0.1.1/mousepad/webbuild/flutter_assets/packages/
--rw-r--r--   0 neetish    (501) staff       (20)     6148 2024-04-14 00:57:30.000000 mousepad-0.1.1/mousepad/webbuild/flutter_assets/packages/.DS_Store
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.084625 mousepad-0.1.1/mousepad/webbuild/flutter_assets/packages/cupertino_icons/
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.099976 mousepad-0.1.1/mousepad/webbuild/flutter_assets/packages/cupertino_icons/assets/
--rw-r--r--   0 neetish    (501) staff       (20)   283452 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/flutter_assets/packages/cupertino_icons/assets/CupertinoIcons.ttf
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.084751 mousepad-0.1.1/mousepad/webbuild/flutter_assets/packages/font_awesome_flutter/
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.084805 mousepad-0.1.1/mousepad/webbuild/flutter_assets/packages/font_awesome_flutter/lib/
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.106793 mousepad-0.1.1/mousepad/webbuild/flutter_assets/packages/font_awesome_flutter/lib/fonts/
--rw-r--r--   0 neetish    (501) staff       (20)   207972 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/flutter_assets/packages/font_awesome_flutter/lib/fonts/fa-brands-400.ttf
--rw-r--r--   0 neetish    (501) staff       (20)    68004 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/flutter_assets/packages/font_awesome_flutter/lib/fonts/fa-regular-400.ttf
--rw-r--r--   0 neetish    (501) staff       (20)   419720 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/flutter_assets/packages/font_awesome_flutter/lib/fonts/fa-solid-900.ttf
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.109365 mousepad-0.1.1/mousepad/webbuild/flutter_assets/shaders/
--rw-r--r--   0 neetish    (501) staff       (20)     8867 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/flutter_assets/shaders/ink_sparkle.frag
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.115098 mousepad-0.1.1/mousepad/webbuild/web/
--rw-r--r--   0 neetish    (501) staff       (20)       32 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/.last_build_id
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.120369 mousepad-0.1.1/mousepad/webbuild/web/assets/
--rw-r--r--   0 neetish    (501) staff       (20)      764 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/assets/AssetManifest.bin
--rw-r--r--   0 neetish    (501) staff       (20)     1022 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/assets/AssetManifest.bin.json
--rw-r--r--   0 neetish    (501) staff       (20)      707 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/assets/AssetManifest.json
--rw-r--r--   0 neetish    (501) staff       (20)      670 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/assets/FontManifest.json
--rw-r--r--   0 neetish    (501) staff       (20)  1729644 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/assets/NOTICES
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.085133 mousepad-0.1.1/mousepad/webbuild/web/assets/assets/
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.124501 mousepad-0.1.1/mousepad/webbuild/web/assets/assets/images/
--rw-r--r--   0 neetish    (501) staff       (20)     4980 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/assets/assets/images/AirDrop.svg
--rw-r--r--   0 neetish    (501) staff       (20)      974 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/assets/assets/images/display.svg
--rw-r--r--   0 neetish    (501) staff       (20)     1574 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/assets/assets/images/gaming.svg
--rw-r--r--   0 neetish    (501) staff       (20)     3805 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/assets/assets/images/keyboard.svg
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.124777 mousepad-0.1.1/mousepad/webbuild/web/assets/fonts/
--rw-r--r--   0 neetish    (501) staff       (20)     8340 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/assets/fonts/MaterialIcons-Regular.otf
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.085452 mousepad-0.1.1/mousepad/webbuild/web/assets/packages/
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.085380 mousepad-0.1.1/mousepad/webbuild/web/assets/packages/cupertino_icons/
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.125122 mousepad-0.1.1/mousepad/webbuild/web/assets/packages/cupertino_icons/assets/
--rw-r--r--   0 neetish    (501) staff       (20)     1272 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/assets/packages/cupertino_icons/assets/CupertinoIcons.ttf
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.085513 mousepad-0.1.1/mousepad/webbuild/web/assets/packages/font_awesome_flutter/
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.085567 mousepad-0.1.1/mousepad/webbuild/web/assets/packages/font_awesome_flutter/lib/
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.126300 mousepad-0.1.1/mousepad/webbuild/web/assets/packages/font_awesome_flutter/lib/fonts/
--rw-r--r--   0 neetish    (501) staff       (20)     2096 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/assets/packages/font_awesome_flutter/lib/fonts/fa-brands-400.ttf
--rw-r--r--   0 neetish    (501) staff       (20)    68004 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/assets/packages/font_awesome_flutter/lib/fonts/fa-regular-400.ttf
--rw-r--r--   0 neetish    (501) staff       (20)     1532 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/assets/packages/font_awesome_flutter/lib/fonts/fa-solid-900.ttf
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.126543 mousepad-0.1.1/mousepad/webbuild/web/assets/shaders/
--rw-r--r--   0 neetish    (501) staff       (20)     8867 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/assets/shaders/ink_sparkle.frag
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.161494 mousepad-0.1.1/mousepad/webbuild/web/canvaskit/
--rw-r--r--   0 neetish    (501) staff       (20)    93469 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/canvaskit/canvaskit.js
--rw-r--r--   0 neetish    (501) staff       (20)  1305998 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/canvaskit/canvaskit.js.symbols
--rwxr-xr-x   0 neetish    (501) staff       (20)  6719234 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/canvaskit/canvaskit.wasm
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.170826 mousepad-0.1.1/mousepad/webbuild/web/canvaskit/chromium/
--rw-r--r--   0 neetish    (501) staff       (20)    93161 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/canvaskit/chromium/canvaskit.js
--rw-r--r--   0 neetish    (501) staff       (20)  1227753 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/canvaskit/chromium/canvaskit.js.symbols
--rwxr-xr-x   0 neetish    (501) staff       (20)  5306867 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/canvaskit/chromium/canvaskit.wasm
--rw-r--r--   0 neetish    (501) staff       (20)    69076 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/canvaskit/skwasm.js
--rw-r--r--   0 neetish    (501) staff       (20)  1432193 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/canvaskit/skwasm.js.symbols
--rwxr-xr-x   0 neetish    (501) staff       (20)  3183440 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/canvaskit/skwasm.wasm
--rw-r--r--   0 neetish    (501) staff       (20)     2916 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/canvaskit/skwasm.worker.js
--rw-r--r--   0 neetish    (501) staff       (20)      917 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/favicon.png
--rw-r--r--   0 neetish    (501) staff       (20)     3891 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/flutter.js
--rw-r--r--   0 neetish    (501) staff       (20)     8661 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/flutter_service_worker.js
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.181066 mousepad-0.1.1/mousepad/webbuild/web/icons/
--rw-r--r--   0 neetish    (501) staff       (20)     5292 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/icons/Icon-192.png
--rw-r--r--   0 neetish    (501) staff       (20)     8252 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/icons/Icon-512.png
--rw-r--r--   0 neetish    (501) staff       (20)     5594 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/icons/Icon-maskable-192.png
--rw-r--r--   0 neetish    (501) staff       (20)    20998 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/icons/Icon-maskable-512.png
--rw-r--r--   0 neetish    (501) staff       (20)     1844 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/index.html
--rw-r--r--   0 neetish    (501) staff       (20)  2670120 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/main.dart.js
--rw-r--r--   0 neetish    (501) staff       (20)      912 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/manifest.json
--rw-r--r--   0 neetish    (501) staff       (20)       86 2024-04-13 22:38:51.000000 mousepad-0.1.1/mousepad/webbuild/web/version.json
-drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:02:17.185027 mousepad-0.1.1/mousepad.egg-info/
--rw-r--r--   0 neetish    (501) staff       (20)     1634 2024-04-14 01:02:17.000000 mousepad-0.1.1/mousepad.egg-info/PKG-INFO
--rw-r--r--   0 neetish    (501) staff       (20)     3169 2024-04-14 01:02:17.000000 mousepad-0.1.1/mousepad.egg-info/SOURCES.txt
--rw-r--r--   0 neetish    (501) staff       (20)        1 2024-04-14 01:02:17.000000 mousepad-0.1.1/mousepad.egg-info/dependency_links.txt
--rw-r--r--   0 neetish    (501) staff       (20)       44 2024-04-14 01:02:17.000000 mousepad-0.1.1/mousepad.egg-info/requires.txt
--rw-r--r--   0 neetish    (501) staff       (20)        9 2024-04-14 01:02:17.000000 mousepad-0.1.1/mousepad.egg-info/top_level.txt
--rw-r--r--   0 neetish    (501) staff       (20)       38 2024-04-14 01:02:17.185605 mousepad-0.1.1/setup.cfg
--rw-r--r--   0 neetish    (501) staff       (20)     1169 2024-04-14 01:00:34.000000 mousepad-0.1.1/setup.py
+drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:37:13.026040 mousepad-0.1.2/
+-rw-r--r--   0 neetish    (501) staff       (20)     1070 2024-04-14 01:18:36.000000 mousepad-0.1.2/LICENSE
+-rw-r--r--   0 neetish    (501) staff       (20)     2393 2024-04-14 01:37:13.025783 mousepad-0.1.2/PKG-INFO
+-rw-r--r--   0 neetish    (501) staff       (20)     1731 2024-04-14 01:36:27.000000 mousepad-0.1.2/README.md
+drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:37:12.963371 mousepad-0.1.2/mousepad/
+-rw-r--r--   0 neetish    (501) staff       (20)     6148 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/.DS_Store
+-rw-r--r--   0 neetish    (501) staff       (20)     5832 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/__main__.py
+drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:37:12.964468 mousepad-0.1.2/mousepad/webbuild/
+-rw-r--r--   0 neetish    (501) staff       (20)     6148 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/.DS_Store
+drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:37:12.966176 mousepad-0.1.2/mousepad/webbuild/flutter_assets/
+-rw-r--r--   0 neetish    (501) staff       (20)     6148 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/flutter_assets/.DS_Store
+-rw-r--r--   0 neetish    (501) staff       (20)      764 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/flutter_assets/AssetManifest.bin
+-rw-r--r--   0 neetish    (501) staff       (20)     1022 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/flutter_assets/AssetManifest.bin.json
+-rw-r--r--   0 neetish    (501) staff       (20)      707 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/flutter_assets/AssetManifest.json
+-rw-r--r--   0 neetish    (501) staff       (20)      670 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/flutter_assets/FontManifest.json
+-rw-r--r--   0 neetish    (501) staff       (20)  1729644 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/flutter_assets/NOTICES
+drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:37:12.961260 mousepad-0.1.2/mousepad/webbuild/flutter_assets/assets/
+drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:37:12.968407 mousepad-0.1.2/mousepad/webbuild/flutter_assets/assets/images/
+-rw-r--r--   0 neetish    (501) staff       (20)     4980 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/flutter_assets/assets/images/AirDrop.svg
+-rw-r--r--   0 neetish    (501) staff       (20)      974 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/flutter_assets/assets/images/display.svg
+-rw-r--r--   0 neetish    (501) staff       (20)     1574 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/flutter_assets/assets/images/gaming.svg
+-rw-r--r--   0 neetish    (501) staff       (20)     3805 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/flutter_assets/assets/images/keyboard.svg
+drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:37:12.968604 mousepad-0.1.2/mousepad/webbuild/flutter_assets/fonts/
+-rw-r--r--   0 neetish    (501) staff       (20)  1645184 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/flutter_assets/fonts/MaterialIcons-Regular.otf
+drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:37:12.969768 mousepad-0.1.2/mousepad/webbuild/flutter_assets/packages/
+-rw-r--r--   0 neetish    (501) staff       (20)     6148 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/flutter_assets/packages/.DS_Store
+drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:37:12.961524 mousepad-0.1.2/mousepad/webbuild/flutter_assets/packages/cupertino_icons/
+drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:37:12.970328 mousepad-0.1.2/mousepad/webbuild/flutter_assets/packages/cupertino_icons/assets/
+-rw-r--r--   0 neetish    (501) staff       (20)   283452 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/flutter_assets/packages/cupertino_icons/assets/CupertinoIcons.ttf
+drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:37:12.974243 mousepad-0.1.2/mousepad/webbuild/flutter_assets/shaders/
+-rw-r--r--   0 neetish    (501) staff       (20)     8867 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/flutter_assets/shaders/ink_sparkle.frag
+drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:37:12.980326 mousepad-0.1.2/mousepad/webbuild/web/
+-rw-r--r--   0 neetish    (501) staff       (20)     6148 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/.DS_Store
+-rw-r--r--   0 neetish    (501) staff       (20)       32 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/.last_build_id
+drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:37:12.982920 mousepad-0.1.2/mousepad/webbuild/web/assets/
+-rw-r--r--   0 neetish    (501) staff       (20)     6148 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/assets/.DS_Store
+-rw-r--r--   0 neetish    (501) staff       (20)      764 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/assets/AssetManifest.bin
+-rw-r--r--   0 neetish    (501) staff       (20)     1022 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/assets/AssetManifest.bin.json
+-rw-r--r--   0 neetish    (501) staff       (20)      707 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/assets/AssetManifest.json
+-rw-r--r--   0 neetish    (501) staff       (20)      670 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/assets/FontManifest.json
+-rw-r--r--   0 neetish    (501) staff       (20)  1729644 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/assets/NOTICES
+drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:37:12.961854 mousepad-0.1.2/mousepad/webbuild/web/assets/assets/
+drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:37:12.986595 mousepad-0.1.2/mousepad/webbuild/web/assets/assets/images/
+-rw-r--r--   0 neetish    (501) staff       (20)     4980 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/assets/assets/images/AirDrop.svg
+-rw-r--r--   0 neetish    (501) staff       (20)      974 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/assets/assets/images/display.svg
+-rw-r--r--   0 neetish    (501) staff       (20)     1574 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/assets/assets/images/gaming.svg
+-rw-r--r--   0 neetish    (501) staff       (20)     3805 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/assets/assets/images/keyboard.svg
+drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:37:12.986751 mousepad-0.1.2/mousepad/webbuild/web/assets/fonts/
+-rw-r--r--   0 neetish    (501) staff       (20)     8340 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/assets/fonts/MaterialIcons-Regular.otf
+drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:37:12.962046 mousepad-0.1.2/mousepad/webbuild/web/assets/packages/
+drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:37:12.962099 mousepad-0.1.2/mousepad/webbuild/web/assets/packages/cupertino_icons/
+drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:37:12.987034 mousepad-0.1.2/mousepad/webbuild/web/assets/packages/cupertino_icons/assets/
+-rw-r--r--   0 neetish    (501) staff       (20)     1272 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/assets/packages/cupertino_icons/assets/CupertinoIcons.ttf
+drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:37:12.987185 mousepad-0.1.2/mousepad/webbuild/web/assets/shaders/
+-rw-r--r--   0 neetish    (501) staff       (20)     8867 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/assets/shaders/ink_sparkle.frag
+drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:37:13.005765 mousepad-0.1.2/mousepad/webbuild/web/canvaskit/
+-rw-r--r--   0 neetish    (501) staff       (20)    93469 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/canvaskit/canvaskit.js
+-rw-r--r--   0 neetish    (501) staff       (20)  1305998 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/canvaskit/canvaskit.js.symbols
+-rwxr-xr-x   0 neetish    (501) staff       (20)  6719234 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/canvaskit/canvaskit.wasm
+drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:37:13.014526 mousepad-0.1.2/mousepad/webbuild/web/canvaskit/chromium/
+-rw-r--r--   0 neetish    (501) staff       (20)    93161 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/canvaskit/chromium/canvaskit.js
+-rw-r--r--   0 neetish    (501) staff       (20)  1227753 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/canvaskit/chromium/canvaskit.js.symbols
+-rwxr-xr-x   0 neetish    (501) staff       (20)  5306867 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/canvaskit/chromium/canvaskit.wasm
+-rw-r--r--   0 neetish    (501) staff       (20)    69076 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/canvaskit/skwasm.js
+-rw-r--r--   0 neetish    (501) staff       (20)  1432193 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/canvaskit/skwasm.js.symbols
+-rwxr-xr-x   0 neetish    (501) staff       (20)  3183440 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/canvaskit/skwasm.wasm
+-rw-r--r--   0 neetish    (501) staff       (20)     2916 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/canvaskit/skwasm.worker.js
+-rw-r--r--   0 neetish    (501) staff       (20)      917 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/favicon.png
+-rw-r--r--   0 neetish    (501) staff       (20)     3891 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/flutter.js
+-rw-r--r--   0 neetish    (501) staff       (20)     8661 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/flutter_service_worker.js
+drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:37:13.021662 mousepad-0.1.2/mousepad/webbuild/web/icons/
+-rw-r--r--   0 neetish    (501) staff       (20)     5292 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/icons/Icon-192.png
+-rw-r--r--   0 neetish    (501) staff       (20)     8252 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/icons/Icon-512.png
+-rw-r--r--   0 neetish    (501) staff       (20)     5594 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/icons/Icon-maskable-192.png
+-rw-r--r--   0 neetish    (501) staff       (20)    20998 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/icons/Icon-maskable-512.png
+-rw-r--r--   0 neetish    (501) staff       (20)     1844 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/index.html
+-rw-r--r--   0 neetish    (501) staff       (20)  2670120 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/main.dart.js
+-rw-r--r--   0 neetish    (501) staff       (20)      912 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/manifest.json
+-rw-r--r--   0 neetish    (501) staff       (20)       86 2024-04-14 01:18:36.000000 mousepad-0.1.2/mousepad/webbuild/web/version.json
+drwxr-xr-x   0 neetish    (501) staff       (20)        0 2024-04-14 01:37:13.025441 mousepad-0.1.2/mousepad.egg-info/
+-rw-r--r--   0 neetish    (501) staff       (20)     2393 2024-04-14 01:37:12.000000 mousepad-0.1.2/mousepad.egg-info/PKG-INFO
+-rw-r--r--   0 neetish    (501) staff       (20)     2734 2024-04-14 01:37:12.000000 mousepad-0.1.2/mousepad.egg-info/SOURCES.txt
+-rw-r--r--   0 neetish    (501) staff       (20)        1 2024-04-14 01:37:12.000000 mousepad-0.1.2/mousepad.egg-info/dependency_links.txt
+-rw-r--r--   0 neetish    (501) staff       (20)       44 2024-04-14 01:37:12.000000 mousepad-0.1.2/mousepad.egg-info/requires.txt
+-rw-r--r--   0 neetish    (501) staff       (20)        9 2024-04-14 01:37:12.000000 mousepad-0.1.2/mousepad.egg-info/top_level.txt
+-rw-r--r--   0 neetish    (501) staff       (20)       38 2024-04-14 01:37:13.026084 mousepad-0.1.2/setup.cfg
+-rw-r--r--   0 neetish    (501) staff       (20)     1169 2024-04-14 01:36:44.000000 mousepad-0.1.2/setup.py
```

### Comparing `mousepad-0.1.1/LICENSE` & `mousepad-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/PKG-INFO` & `mousepad-0.1.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mousepad
-Version: 0.1.1
+Version: 0.1.2
 Summary: Multidevice controller using python
 Home-page: https://github.com/neetishsingh/mousepad
 Author: Neetish Singh
 Author-email: neetishsingh97@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
@@ -16,17 +16,45 @@
 License-File: LICENSE
 Requires-Dist: fastapi
 Requires-Dist: uvicorn[standard]
 Requires-Dist: asyncio
 Requires-Dist: pyautogui
 
 # Mousepad
+
+[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
+
 Mousepad is a Python-based library designed to facilitate seamless connectivity between multiple devices on the same network such as wifi, enabling users to interact with each other in various ways, including mouse control, keypad input, joystick emulation, screen sharing, file sharing like Airdrop, and multiplayer gaming.
 
 ## Features
 - **Device Integration:** Connect and manage multiple devices on the same network.
 - **Mouse Control:** Utilize devices as a mouse for precise control.
 - **Keypad Input:** Input text or commands using connected devices.
 - **Joystick Emulation:** Transform devices into game controllers for gaming applications.
 - **Screen Sharing:** Share screens across devices for collaborative work or presentations.
 - **Airdrop File Sharing:** Seamlessly share files between devices using Airdrop functionality.
 - **Multiplayer Gaming:** Enable multiplayer gaming experiences over the same network, such as WiFi, for enhanced gameplay.
+
+
+## How to run
+
+Best part of mousepad is you just need two lines of code to initiate it.
+
+1.To install mousepad python package.
+```bash
+  pip install mousepad
+```
+
+2.Now start the app
+```bash
+  python -m mousepad
+```
+or if you have python3 installed then 
+```bash
+  python3 -m mousepad
+```
+
+3. In Browser you will see a QR which you can scan through any kind of device and any kind of os for ex. Mobile.
+4. You can select the feature you want to use i.e Mouse, Keyboard, Joystick and it's configured. 
+
+
+Note: The only requirement to take benifit of this sharing framework in that you need to have python installed in any of the device atleast.
```

### Comparing `mousepad-0.1.1/mousepad/.DS_Store` & `mousepad-0.1.2/mousepad/.DS_Store`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/__main__.py` & `mousepad-0.1.2/mousepad/__main__.py`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/flutter_assets/.DS_Store` & `mousepad-0.1.2/mousepad/webbuild/flutter_assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/flutter_assets/AssetManifest.bin` & `mousepad-0.1.2/mousepad/webbuild/flutter_assets/AssetManifest.bin`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/flutter_assets/AssetManifest.bin.json` & `mousepad-0.1.2/mousepad/webbuild/flutter_assets/AssetManifest.bin.json`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/flutter_assets/AssetManifest.json` & `mousepad-0.1.2/mousepad/webbuild/flutter_assets/AssetManifest.json`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/flutter_assets/FontManifest.json` & `mousepad-0.1.2/mousepad/webbuild/flutter_assets/FontManifest.json`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/flutter_assets/NOTICES` & `mousepad-0.1.2/mousepad/webbuild/flutter_assets/NOTICES`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/flutter_assets/assets/images/AirDrop.svg` & `mousepad-0.1.2/mousepad/webbuild/flutter_assets/assets/images/AirDrop.svg`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/flutter_assets/assets/images/display.svg` & `mousepad-0.1.2/mousepad/webbuild/flutter_assets/assets/images/display.svg`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/flutter_assets/assets/images/gaming.svg` & `mousepad-0.1.2/mousepad/webbuild/flutter_assets/assets/images/gaming.svg`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/flutter_assets/assets/images/keyboard.svg` & `mousepad-0.1.2/mousepad/webbuild/flutter_assets/assets/images/keyboard.svg`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/flutter_assets/fonts/MaterialIcons-Regular.otf` & `mousepad-0.1.2/mousepad/webbuild/flutter_assets/fonts/MaterialIcons-Regular.otf`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/flutter_assets/packages/.DS_Store` & `mousepad-0.1.2/mousepad/webbuild/flutter_assets/packages/.DS_Store`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/flutter_assets/packages/cupertino_icons/assets/CupertinoIcons.ttf` & `mousepad-0.1.2/mousepad/webbuild/flutter_assets/packages/cupertino_icons/assets/CupertinoIcons.ttf`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/flutter_assets/shaders/ink_sparkle.frag` & `mousepad-0.1.2/mousepad/webbuild/flutter_assets/shaders/ink_sparkle.frag`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/assets/AssetManifest.bin` & `mousepad-0.1.2/mousepad/webbuild/web/assets/AssetManifest.bin`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/assets/AssetManifest.bin.json` & `mousepad-0.1.2/mousepad/webbuild/web/assets/AssetManifest.bin.json`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/assets/AssetManifest.json` & `mousepad-0.1.2/mousepad/webbuild/web/assets/AssetManifest.json`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/assets/FontManifest.json` & `mousepad-0.1.2/mousepad/webbuild/web/assets/FontManifest.json`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/assets/NOTICES` & `mousepad-0.1.2/mousepad/webbuild/web/assets/NOTICES`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/assets/assets/images/AirDrop.svg` & `mousepad-0.1.2/mousepad/webbuild/web/assets/assets/images/AirDrop.svg`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/assets/assets/images/display.svg` & `mousepad-0.1.2/mousepad/webbuild/web/assets/assets/images/display.svg`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/assets/assets/images/gaming.svg` & `mousepad-0.1.2/mousepad/webbuild/web/assets/assets/images/gaming.svg`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/assets/assets/images/keyboard.svg` & `mousepad-0.1.2/mousepad/webbuild/web/assets/assets/images/keyboard.svg`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/assets/fonts/MaterialIcons-Regular.otf` & `mousepad-0.1.2/mousepad/webbuild/web/assets/fonts/MaterialIcons-Regular.otf`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/assets/packages/cupertino_icons/assets/CupertinoIcons.ttf` & `mousepad-0.1.2/mousepad/webbuild/web/assets/packages/cupertino_icons/assets/CupertinoIcons.ttf`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/assets/shaders/ink_sparkle.frag` & `mousepad-0.1.2/mousepad/webbuild/web/assets/shaders/ink_sparkle.frag`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/canvaskit/canvaskit.js` & `mousepad-0.1.2/mousepad/webbuild/web/canvaskit/canvaskit.js`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/canvaskit/canvaskit.js.symbols` & `mousepad-0.1.2/mousepad/webbuild/web/canvaskit/canvaskit.js.symbols`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/canvaskit/canvaskit.wasm` & `mousepad-0.1.2/mousepad/webbuild/web/canvaskit/canvaskit.wasm`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/canvaskit/chromium/canvaskit.js` & `mousepad-0.1.2/mousepad/webbuild/web/canvaskit/chromium/canvaskit.js`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/canvaskit/chromium/canvaskit.js.symbols` & `mousepad-0.1.2/mousepad/webbuild/web/canvaskit/chromium/canvaskit.js.symbols`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/canvaskit/chromium/canvaskit.wasm` & `mousepad-0.1.2/mousepad/webbuild/web/canvaskit/chromium/canvaskit.wasm`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/canvaskit/skwasm.js` & `mousepad-0.1.2/mousepad/webbuild/web/canvaskit/skwasm.js`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/canvaskit/skwasm.js.symbols` & `mousepad-0.1.2/mousepad/webbuild/web/canvaskit/skwasm.js.symbols`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/canvaskit/skwasm.wasm` & `mousepad-0.1.2/mousepad/webbuild/web/canvaskit/skwasm.wasm`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/canvaskit/skwasm.worker.js` & `mousepad-0.1.2/mousepad/webbuild/web/canvaskit/skwasm.worker.js`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/favicon.png` & `mousepad-0.1.2/mousepad/webbuild/web/favicon.png`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/flutter.js` & `mousepad-0.1.2/mousepad/webbuild/web/flutter.js`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/flutter_service_worker.js` & `mousepad-0.1.2/mousepad/webbuild/web/flutter_service_worker.js`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/icons/Icon-192.png` & `mousepad-0.1.2/mousepad/webbuild/web/icons/Icon-192.png`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/icons/Icon-512.png` & `mousepad-0.1.2/mousepad/webbuild/web/icons/Icon-512.png`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/icons/Icon-maskable-192.png` & `mousepad-0.1.2/mousepad/webbuild/web/icons/Icon-maskable-192.png`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/icons/Icon-maskable-512.png` & `mousepad-0.1.2/mousepad/webbuild/web/icons/Icon-maskable-512.png`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/index.html` & `mousepad-0.1.2/mousepad/webbuild/web/index.html`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/main.dart.js` & `mousepad-0.1.2/mousepad/webbuild/web/main.dart.js`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad/webbuild/web/manifest.json` & `mousepad-0.1.2/mousepad/webbuild/web/manifest.json`

 * *Files identical despite different names*

### Comparing `mousepad-0.1.1/mousepad.egg-info/PKG-INFO` & `mousepad-0.1.2/mousepad.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mousepad
-Version: 0.1.1
+Version: 0.1.2
 Summary: Multidevice controller using python
 Home-page: https://github.com/neetishsingh/mousepad
 Author: Neetish Singh
 Author-email: neetishsingh97@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
@@ -16,17 +16,45 @@
 License-File: LICENSE
 Requires-Dist: fastapi
 Requires-Dist: uvicorn[standard]
 Requires-Dist: asyncio
 Requires-Dist: pyautogui
 
 # Mousepad
+
+[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
+
 Mousepad is a Python-based library designed to facilitate seamless connectivity between multiple devices on the same network such as wifi, enabling users to interact with each other in various ways, including mouse control, keypad input, joystick emulation, screen sharing, file sharing like Airdrop, and multiplayer gaming.
 
 ## Features
 - **Device Integration:** Connect and manage multiple devices on the same network.
 - **Mouse Control:** Utilize devices as a mouse for precise control.
 - **Keypad Input:** Input text or commands using connected devices.
 - **Joystick Emulation:** Transform devices into game controllers for gaming applications.
 - **Screen Sharing:** Share screens across devices for collaborative work or presentations.
 - **Airdrop File Sharing:** Seamlessly share files between devices using Airdrop functionality.
 - **Multiplayer Gaming:** Enable multiplayer gaming experiences over the same network, such as WiFi, for enhanced gameplay.
+
+
+## How to run
+
+Best part of mousepad is you just need two lines of code to initiate it.
+
+1.To install mousepad python package.
+```bash
+  pip install mousepad
+```
+
+2.Now start the app
+```bash
+  python -m mousepad
+```
+or if you have python3 installed then 
+```bash
+  python3 -m mousepad
+```
+
+3. In Browser you will see a QR which you can scan through any kind of device and any kind of os for ex. Mobile.
+4. You can select the feature you want to use i.e Mouse, Keyboard, Joystick and it's configured. 
+
+
+Note: The only requirement to take benifit of this sharing framework in that you need to have python installed in any of the device atleast.
```

### Comparing `mousepad-0.1.1/setup.py` & `mousepad-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return paths
 
 
 extra_files = package_files('mousepad')
 
 setup(
     name='mousepad',
-    version='0.1.1',
+    version='0.1.2',
     description='Multidevice controller using python',
     url='https://github.com/neetishsingh/mousepad',
     author='Neetish Singh',
     author_email='neetishsingh97@gmail.com',
     license='MIT License',
     packages=['mousepad'],
     package_data={'mousepad': extra_files},
```

