# Comparing `tmp/Xdcheckin-2.0.4.tar.gz` & `tmp/xdcheckin-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Xdcheckin-2.0.4.tar", last modified: Tue Apr  9 14:44:59 2024, max compression
+gzip compressed data, was "xdcheckin-2.0.5.tar", last modified: Sun Apr 14 13:14:21 2024, max compression
```

## Comparing `Xdcheckin-2.0.4.tar` & `xdcheckin-2.0.5.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:44:59.497891 Xdcheckin-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-09 14:44:54.000000 Xdcheckin-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-09 14:44:59.497891 Xdcheckin-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-09 14:44:54.000000 Xdcheckin-2.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-09 14:44:54.000000 Xdcheckin-2.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 14:44:59.497891 Xdcheckin-2.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:44:59.489891 Xdcheckin-2.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:44:59.497891 Xdcheckin-2.0.4/src/Xdcheckin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-09 14:44:59.000000 Xdcheckin-2.0.4/src/Xdcheckin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-09 14:44:59.000000 Xdcheckin-2.0.4/src/Xdcheckin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:44:59.000000 Xdcheckin-2.0.4/src/Xdcheckin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-09 14:44:59.000000 Xdcheckin-2.0.4/src/Xdcheckin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-09 14:44:59.000000 Xdcheckin-2.0.4/src/Xdcheckin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 14:44:59.000000 Xdcheckin-2.0.4/src/Xdcheckin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:44:59.493891 Xdcheckin-2.0.4/src/xdcheckin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:44:54.000000 Xdcheckin-2.0.4/src/xdcheckin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-09 14:44:54.000000 Xdcheckin-2.0.4/src/xdcheckin/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:44:59.493891 Xdcheckin-2.0.4/src/xdcheckin/core/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-09 14:44:54.000000 Xdcheckin-2.0.4/src/xdcheckin/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33281 2024-04-09 14:44:54.000000 Xdcheckin-2.0.4/src/xdcheckin/core/chaoxing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-09 14:44:54.000000 Xdcheckin-2.0.4/src/xdcheckin/core/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-04-09 14:44:54.000000 Xdcheckin-2.0.4/src/xdcheckin/core/xidian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:44:59.493891 Xdcheckin-2.0.4/src/xdcheckin/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:44:54.000000 Xdcheckin-2.0.4/src/xdcheckin/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-04-09 14:44:54.000000 Xdcheckin-2.0.4/src/xdcheckin/server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:44:59.497891 Xdcheckin-2.0.4/src/xdcheckin/server/static/
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-09 14:44:54.000000 Xdcheckin-2.0.4/src/xdcheckin/server/static/activity.js
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-09 14:44:54.000000 Xdcheckin-2.0.4/src/xdcheckin/server/static/classroom.js
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-09 14:44:54.000000 Xdcheckin-2.0.4/src/xdcheckin/server/static/curriculum.js
--rw-r--r--   0 runner    (1001) docker     (127)   249304 2024-04-09 14:44:54.000000 Xdcheckin-2.0.4/src/xdcheckin/server/static/g_classroom_urls.js
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-09 14:44:54.000000 Xdcheckin-2.0.4/src/xdcheckin/server/static/global.js
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-09 14:44:54.000000 Xdcheckin-2.0.4/src/xdcheckin/server/static/location.js
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-09 14:44:54.000000 Xdcheckin-2.0.4/src/xdcheckin/server/static/login.js
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-09 14:44:54.000000 Xdcheckin-2.0.4/src/xdcheckin/server/static/misc.js
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-09 14:44:54.000000 Xdcheckin-2.0.4/src/xdcheckin/server/static/player.js
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-09 14:44:54.000000 Xdcheckin-2.0.4/src/xdcheckin/server/static/style.css
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-09 14:44:54.000000 Xdcheckin-2.0.4/src/xdcheckin/server/static/util.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:44:59.497891 Xdcheckin-2.0.4/src/xdcheckin/server/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-09 14:44:54.000000 Xdcheckin-2.0.4/src/xdcheckin/server/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:44:59.497891 Xdcheckin-2.0.4/src/xdcheckin/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:44:54.000000 Xdcheckin-2.0.4/src/xdcheckin/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-09 14:44:54.000000 Xdcheckin-2.0.4/src/xdcheckin/util/chaoxing_captcha.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:14:21.140514 xdcheckin-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-14 13:14:21.140514 xdcheckin-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 13:14:21.140514 xdcheckin-2.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:14:21.132514 xdcheckin-2.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:14:21.136514 xdcheckin-2.0.5/src/Xdcheckin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-14 13:14:21.000000 xdcheckin-2.0.5/src/Xdcheckin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-14 13:14:21.000000 xdcheckin-2.0.5/src/Xdcheckin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 13:14:21.000000 xdcheckin-2.0.5/src/Xdcheckin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-14 13:14:21.000000 xdcheckin-2.0.5/src/Xdcheckin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-14 13:14:21.000000 xdcheckin-2.0.5/src/Xdcheckin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-14 13:14:21.000000 xdcheckin-2.0.5/src/Xdcheckin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:14:21.136514 xdcheckin-2.0.5/src/xdcheckin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:14:21.136514 xdcheckin-2.0.5/src/xdcheckin/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33581 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/core/chaoxing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/core/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/core/xidian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:14:21.136514 xdcheckin-2.0.5/src/xdcheckin/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11913 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:14:21.136514 xdcheckin-2.0.5/src/xdcheckin/server/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/server/static/activity.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/server/static/classroom.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/server/static/curriculum.js
+-rw-r--r--   0 runner    (1001) docker     (127)   249304 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/server/static/g_classroom_urls.js
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/server/static/global.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/server/static/location.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/server/static/login.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/server/static/misc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/server/static/player.js
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/server/static/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/server/static/util.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:14:21.136514 xdcheckin-2.0.5/src/xdcheckin/server/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/server/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:14:21.136514 xdcheckin-2.0.5/src/xdcheckin/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/util/chaoxing_captcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/util/encryption.py
```

### Comparing `Xdcheckin-2.0.4/LICENSE` & `xdcheckin-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.4/PKG-INFO` & `xdcheckin-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xdcheckin
-Version: 2.0.4
+Version: 2.0.5
 Summary: Chaoxing Checkin Tool for XDU.
 Author-email: Pairman <pairmanxlr@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Pairman/Xdcheckin
 Project-URL: Changelog, https://github.com/Pairman/Xdcheckin/blob/main/CHANGELOG.md
 Keywords: xdu,xidian,chaoxing,livestream
 Classifier: Framework :: Flask
```

### Comparing `Xdcheckin-2.0.4/README.md` & `xdcheckin-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.4/pyproject.toml` & `xdcheckin-2.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
 00000020: 7570 746f 6f6c 7322 2c20 2277 6865 656c  uptools", "wheel
 00000030: 225d 0d0a 6275 696c 642d 6261 636b 656e  "]..build-backen
 00000040: 6420 3d20 2273 6574 7570 746f 6f6c 732e  d = "setuptools.
 00000050: 6275 696c 645f 6d65 7461 220d 0a0d 0a5b  build_meta"....[
 00000060: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000070: 2022 5864 6368 6563 6b69 6e22 0d0a 7665   "Xdcheckin"..ve
-00000080: 7273 696f 6e20 3d20 2232 2e30 2e34 220d  rsion = "2.0.4".
+00000080: 7273 696f 6e20 3d20 2232 2e30 2e35 220d  rsion = "2.0.5".
 00000090: 0a61 7574 686f 7273 203d 205b 0d0a 097b  .authors = [...{
 000000a0: 6e61 6d65 203d 2022 5061 6972 6d61 6e22  name = "Pairman"
 000000b0: 2c20 656d 6169 6c20 3d20 2270 6169 726d  , email = "pairm
 000000c0: 616e 786c 7240 676d 6169 6c2e 636f 6d22  anxlr@gmail.com"
 000000d0: 7d0d 0a5d 0d0a 7265 6164 6d65 203d 2022  }..]..readme = "
 000000e0: 5245 4144 4d45 2e6d 6422 0d0a 6465 7363  README.md"..desc
 000000f0: 7269 7074 696f 6e20 3d20 2243 6861 6f78  ription = "Chaox
@@ -73,293 +73,293 @@
 00000480: 0d0a 0922 7864 6368 6563 6b69 6e2e 636f  ..."xdcheckin.co
 00000490: 7265 2a22 2c0d 0a09 2278 6463 6865 636b  re*",..."xdcheck
 000004a0: 696e 2e73 6572 7665 722a 222c 0d0a 0922  in.server*",..."
 000004b0: 7864 6368 6563 6b69 6e2e 7574 696c 2a22  xdcheckin.util*"
 000004c0: 2c0d 0a5d 0d0a 6578 636c 7564 6520 3d20  ,..]..exclude = 
 000004d0: 5b0d 0a09 2278 6463 6865 636b 696e 2e61  [..."xdcheckin.a
 000004e0: 7070 2a22 2c0d 0a09 2278 6463 6865 636b  pp*",..."xdcheck
-000004f0: 696e 2e5f 5f6d 6169 6e5f 5f22 2c0d 0a20  in.__main__",.. 
-00000500: 5d0d 0a0d 0a5b 746f 6f6c 2e73 6574 7570  ]....[tool.setup
-00000510: 746f 6f6c 732e 7061 636b 6167 652d 6461  tools.package-da
-00000520: 7461 5d0d 0a22 7864 6368 6563 6b69 6e2e  ta].."xdcheckin.
-00000530: 7365 7276 6572 2220 3d20 5b22 7374 6174  server" = ["stat
-00000540: 6963 2f2a 222c 2022 7465 6d70 6c61 7465  ic/*", "template
-00000550: 732f 2a22 5d0d 0a0d 0a5b 746f 6f6c 2e62  s/*"]....[tool.b
-00000560: 7269 6566 6361 7365 5d0d 0a70 726f 6a65  riefcase]..proje
-00000570: 6374 5f6e 616d 6520 3d20 2258 6463 6865  ct_name = "Xdche
-00000580: 636b 696e 220d 0a62 756e 646c 6520 3d20  ckin"..bundle = 
-00000590: 226f 7267 2e65 752e 706e 786c 722e 6769  "org.eu.pnxlr.gi
-000005a0: 7422 0d0a 0d0a 5b74 6f6f 6c2e 6272 6965  t"....[tool.brie
-000005b0: 6663 6173 652e 6170 702e 7864 6368 6563  fcase.app.xdchec
-000005c0: 6b69 6e5d 0d0a 666f 726d 616c 5f6e 616d  kin]..formal_nam
-000005d0: 6520 3d20 2258 6463 6865 636b 696e 220d  e = "Xdcheckin".
-000005e0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-000005f0: 6e20 3d20 2222 2243 6861 6f78 696e 6720  n = """Chaoxing 
-00000600: 4368 6563 6b69 6e20 546f 6f6c 2066 6f72  Checkin Tool for
-00000610: 2058 4455 2e0d 0a22 2222 0d0a 6963 6f6e   XDU..."""..icon
-00000620: 203d 2022 7372 632f 7864 6368 6563 6b69   = "src/xdchecki
-00000630: 6e2f 6170 702f 7265 736f 7572 6365 732f  n/app/resources/
-00000640: 7864 6368 6563 6b69 6e22 0d0a 736f 7572  xdcheckin"..sour
-00000650: 6365 7320 3d20 5b0d 0a09 2273 7263 2f78  ces = [..."src/x
-00000660: 6463 6865 636b 696e 222c 0d0a 5d0d 0a23  dcheckin",..]..#
-00000670: 2074 6573 745f 736f 7572 6365 7320 3d20   test_sources = 
-00000680: 5b5d 0d0a 7265 7175 6972 6573 203d 205b  []..requires = [
-00000690: 0d0a 0922 666c 6173 6b20 3e3d 2033 2e30  ..."flask >= 3.0
-000006a0: 2e30 222c 0d0a 0922 666c 6173 6b2d 7365  .0",..."flask-se
-000006b0: 7373 696f 6e20 3d3d 2030 2e36 2e30 222c  ssion == 0.6.0",
-000006c0: 0d0a 0922 7069 6c6c 6f77 203e 3d20 382e  ..."pillow >= 8.
-000006d0: 342e 3022 2c0d 0a09 2270 7963 7279 7074  4.0",..."pycrypt
-000006e0: 6f64 6f6d 6520 3e3d 2033 2e39 2e34 222c  odome >= 3.9.4",
-000006f0: 0d0a 0922 7079 7a62 6172 203e 3d20 302e  ..."pyzbar >= 0.
-00000700: 312e 3822 2c0d 0a09 2272 6571 7565 7374  1.8",..."request
-00000710: 7320 3e3d 2032 2e33 312e 3022 2c0d 0a09  s >= 2.31.0",...
-00000720: 2272 6571 7565 7374 732d 6361 6368 6520  "requests-cache 
-00000730: 3e3d 2031 2e32 2e30 222c 0d0a 0922 7761  >= 1.2.0",..."wa
-00000740: 6974 7265 7373 203e 3d20 332e 302e 3022  itress >= 3.0.0"
-00000750: 2c0d 0a5d 0d0a 2320 7465 7374 5f72 6571  ,..]..# test_req
-00000760: 7569 7265 7320 3d20 5b5d 0d0a 0d0a 5b74  uires = []....[t
-00000770: 6f6f 6c2e 6272 6965 6663 6173 652e 6170  ool.briefcase.ap
-00000780: 702e 7864 6368 6563 6b69 6e2e 6d61 634f  p.xdcheckin.macO
-00000790: 535d 0d0a 756e 6976 6572 7361 6c5f 6275  S]..universal_bu
-000007a0: 696c 6420 3d20 7472 7565 0d0a 7265 7175  ild = true..requ
-000007b0: 6972 6573 203d 205b 0d0a 0922 746f 6761  ires = [..."toga
-000007c0: 2d63 6f63 6f61 7e3d 302e 342e 3022 2c0d  -cocoa~=0.4.0",.
-000007d0: 0a09 2273 7464 2d6e 736c 6f67 7e3d 312e  .."std-nslog~=1.
-000007e0: 302e 3022 2c0d 0a5d 0d0a 0d0a 5b74 6f6f  0.0",..]....[too
-000007f0: 6c2e 6272 6965 6663 6173 652e 6170 702e  l.briefcase.app.
-00000800: 7864 6368 6563 6b69 6e2e 6c69 6e75 785d  xdcheckin.linux]
-00000810: 0d0a 7265 7175 6972 6573 203d 205b 0d0a  ..requires = [..
-00000820: 0922 746f 6761 2d67 746b 7e3d 302e 342e  ."toga-gtk~=0.4.
-00000830: 3022 2c0d 0a5d 0d0a 0d0a 5b74 6f6f 6c2e  0",..]....[tool.
-00000840: 6272 6965 6663 6173 652e 6170 702e 7864  briefcase.app.xd
-00000850: 6368 6563 6b69 6e2e 6c69 6e75 782e 7379  checkin.linux.sy
-00000860: 7374 656d 2e64 6562 6961 6e5d 0d0a 7379  stem.debian]..sy
-00000870: 7374 656d 5f72 6571 7569 7265 7320 3d20  stem_requires = 
-00000880: 5b0d 0a09 2320 4e65 6564 6564 2074 6f20  [...# Needed to 
-00000890: 636f 6d70 696c 6520 7079 6361 6972 6f20  compile pycairo 
-000008a0: 7768 6565 6c0d 0a09 226c 6962 6361 6972  wheel..."libcair
-000008b0: 6f32 2d64 6576 222c 0d0a 0923 204e 6565  o2-dev",...# Nee
-000008c0: 6465 6420 746f 2063 6f6d 7069 6c65 2050  ded to compile P
-000008d0: 7947 4f62 6a65 6374 2077 6865 656c 0d0a  yGObject wheel..
-000008e0: 0922 6c69 6267 6972 6570 6f73 6974 6f72  ."libgirepositor
-000008f0: 7931 2e30 2d64 6576 222c 0d0a 5d0d 0a0d  y1.0-dev",..]...
-00000900: 0a73 7973 7465 6d5f 7275 6e74 696d 655f  .system_runtime_
-00000910: 7265 7175 6972 6573 203d 205b 0d0a 0923  requires = [...#
-00000920: 204e 6565 6465 6420 746f 2070 726f 7669   Needed to provi
-00000930: 6465 2047 544b 2061 6e64 2069 7473 2047  de GTK and its G
-00000940: 4920 6269 6e64 696e 6773 0d0a 0922 6769  I bindings..."gi
-00000950: 7231 2e32 2d67 746b 2d33 2e30 222c 0d0a  r1.2-gtk-3.0",..
-00000960: 0922 6c69 6267 6972 6570 6f73 6974 6f72  ."libgirepositor
-00000970: 792d 312e 302d 3122 2c0d 0a09 2320 4465  y-1.0-1",...# De
-00000980: 7065 6e64 656e 6369 6573 2074 6861 7420  pendencies that 
-00000990: 4754 4b20 6c6f 6f6b 7320 666f 7220 6174  GTK looks for at
-000009a0: 2072 756e 7469 6d65 0d0a 0922 6c69 6263   runtime..."libc
-000009b0: 616e 6265 7272 612d 6774 6b33 2d6d 6f64  anberra-gtk3-mod
-000009c0: 756c 6522 2c0d 0a09 2320 4e65 6564 6564  ule",...# Needed
-000009d0: 2074 6f20 7072 6f76 6964 6520 5765 624b   to provide WebK
-000009e0: 6974 3220 6174 2072 756e 7469 6d65 0d0a  it2 at runtime..
-000009f0: 0923 2022 6769 7231 2e32 2d77 6562 6b69  .# "gir1.2-webki
-00000a00: 7432 2d34 2e30 222c 0d0a 0923 204e 6565  t2-4.0",...# Nee
-00000a10: 6465 6420 666f 7220 7079 7a62 6172 2061  ded for pyzbar a
-00000a20: 7420 7275 6e74 696d 650d 0a09 226c 6962  t runtime..."lib
-00000a30: 7a62 6172 3022 2c0d 0a5d 0d0a 0d0a 5b74  zbar0",..]....[t
-00000a40: 6f6f 6c2e 6272 6965 6663 6173 652e 6170  ool.briefcase.ap
-00000a50: 702e 7864 6368 6563 6b69 6e2e 6c69 6e75  p.xdcheckin.linu
-00000a60: 782e 7379 7374 656d 2e72 6865 6c5d 0d0a  x.system.rhel]..
-00000a70: 7379 7374 656d 5f72 6571 7569 7265 7320  system_requires 
-00000a80: 3d20 5b0d 0a09 2320 4e65 6564 6564 2074  = [...# Needed t
-00000a90: 6f20 636f 6d70 696c 6520 7079 6361 6972  o compile pycair
-00000aa0: 6f20 7768 6565 6c0d 0a09 2263 6169 726f  o wheel..."cairo
-00000ab0: 2d67 6f62 6a65 6374 2d64 6576 656c 222c  -gobject-devel",
-00000ac0: 0d0a 0923 204e 6565 6465 6420 746f 2063  ...# Needed to c
-00000ad0: 6f6d 7069 6c65 2050 7947 4f62 6a65 6374  ompile PyGObject
-00000ae0: 2077 6865 656c 0d0a 0922 676f 626a 6563   wheel..."gobjec
-00000af0: 742d 696e 7472 6f73 7065 6374 696f 6e2d  t-introspection-
-00000b00: 6465 7665 6c22 2c0d 0a5d 0d0a 0d0a 7379  devel",..]....sy
-00000b10: 7374 656d 5f72 756e 7469 6d65 5f72 6571  stem_runtime_req
-00000b20: 7569 7265 7320 3d20 5b0d 0a09 2320 4e65  uires = [...# Ne
-00000b30: 6564 6564 2074 6f20 7375 7070 6f72 7420  eded to support 
-00000b40: 5079 7468 6f6e 2062 696e 6469 6e67 7320  Python bindings 
-00000b50: 746f 2047 544b 0d0a 0922 676f 626a 6563  to GTK..."gobjec
-00000b60: 742d 696e 7472 6f73 7065 6374 696f 6e22  t-introspection"
-00000b70: 2c0d 0a09 2320 4e65 6564 6564 2074 6f20  ,...# Needed to 
-00000b80: 7072 6f76 6964 6520 4754 4b0d 0a09 2267  provide GTK..."g
-00000b90: 746b 3322 2c0d 0a09 2320 4465 7065 6e64  tk3",...# Depend
-00000ba0: 656e 6369 6573 2074 6861 7420 4754 4b20  encies that GTK 
-00000bb0: 6c6f 6f6b 7320 666f 7220 6174 2072 756e  looks for at run
-00000bc0: 7469 6d65 0d0a 0922 6c69 6263 616e 6265  time..."libcanbe
-00000bd0: 7272 612d 6774 6b33 222c 0d0a 0923 204e  rra-gtk3",...# N
-00000be0: 6565 6465 6420 746f 2070 726f 7669 6465  eeded to provide
-00000bf0: 2057 6562 4b69 7432 2061 7420 7275 6e74   WebKit2 at runt
-00000c00: 696d 650d 0a09 2320 2277 6562 6b69 7432  ime...# "webkit2
-00000c10: 6774 6b33 222c 0d0a 0923 204e 6565 6465  gtk3",...# Neede
-00000c20: 6420 666f 7220 7079 7a62 6172 2061 7420  d for pyzbar at 
-00000c30: 7275 6e74 696d 650d 0a09 227a 6261 722d  runtime..."zbar-
-00000c40: 6c69 6273 222c 0d0a 5d0d 0a0d 0a5b 746f  libs",..]....[to
-00000c50: 6f6c 2e62 7269 6566 6361 7365 2e61 7070  ol.briefcase.app
-00000c60: 2e78 6463 6865 636b 696e 2e6c 696e 7578  .xdcheckin.linux
-00000c70: 2e73 7973 7465 6d2e 7375 7365 5d0d 0a73  .system.suse]..s
-00000c80: 7973 7465 6d5f 7265 7175 6972 6573 203d  ystem_requires =
-00000c90: 205b 0d0a 0923 204e 6565 6465 6420 746f   [...# Needed to
-00000ca0: 2063 6f6d 7069 6c65 2070 7963 6169 726f   compile pycairo
-00000cb0: 2077 6865 656c 0d0a 0922 6361 6972 6f2d   wheel..."cairo-
-00000cc0: 6465 7665 6c22 2c0d 0a09 2320 4e65 6564  devel",...# Need
-00000cd0: 6564 2074 6f20 636f 6d70 696c 6520 5079  ed to compile Py
-00000ce0: 474f 626a 6563 7420 7768 6565 6c0d 0a09  GObject wheel...
-00000cf0: 2267 6f62 6a65 6374 2d69 6e74 726f 7370  "gobject-introsp
-00000d00: 6563 7469 6f6e 2d64 6576 656c 222c 0d0a  ection-devel",..
-00000d10: 5d0d 0a0d 0a73 7973 7465 6d5f 7275 6e74  ]....system_runt
-00000d20: 696d 655f 7265 7175 6972 6573 203d 205b  ime_requires = [
-00000d30: 0d0a 0923 204e 6565 6465 6420 746f 2070  ...# Needed to p
-00000d40: 726f 7669 6465 2047 544b 0d0a 0922 6774  rovide GTK..."gt
-00000d50: 6b33 222c 0d0a 0923 204e 6565 6465 6420  k3",...# Needed 
-00000d60: 746f 2073 7570 706f 7274 2050 7974 686f  to support Pytho
-00000d70: 6e20 6269 6e64 696e 6773 2074 6f20 4754  n bindings to GT
-00000d80: 4b0d 0a09 2267 6f62 6a65 6374 2d69 6e74  K..."gobject-int
-00000d90: 726f 7370 6563 7469 6f6e 222c 2022 7479  rospection", "ty
-00000da0: 7065 6c69 6228 4774 6b29 3d33 2e30 222c  pelib(Gtk)=3.0",
-00000db0: 0d0a 0923 2044 6570 656e 6465 6e63 6965  ...# Dependencie
-00000dc0: 7320 7468 6174 2047 544b 206c 6f6f 6b73  s that GTK looks
-00000dd0: 2066 6f72 2061 7420 7275 6e74 696d 650d   for at runtime.
-00000de0: 0a09 226c 6962 6361 6e62 6572 7261 2d67  .."libcanberra-g
-00000df0: 746b 332d 3022 2c0d 0a09 2320 4e65 6564  tk3-0",...# Need
-00000e00: 6564 2074 6f20 7072 6f76 6964 6520 5765  ed to provide We
-00000e10: 624b 6974 3220 6174 2072 756e 7469 6d65  bKit2 at runtime
-00000e20: 0d0a 0923 2022 6c69 6277 6562 6b69 7432  ...# "libwebkit2
-00000e30: 6774 6b33 222c 0d0a 0923 2022 7479 7065  gtk3",...# "type
-00000e40: 6c69 6228 5765 624b 6974 3229 222c 0d0a  lib(WebKit2)",..
-00000e50: 0923 204e 6565 6465 6420 666f 7220 7079  .# Needed for py
-00000e60: 7a62 6172 2061 7420 7275 6e74 696d 650d  zbar at runtime.
-00000e70: 0a09 226c 6962 7a62 6172 3022 2c0d 0a5d  .."libzbar0",..]
-00000e80: 0d0a 0d0a 5b74 6f6f 6c2e 6272 6965 6663  ....[tool.briefc
-00000e90: 6173 652e 6170 702e 7864 6368 6563 6b69  ase.app.xdchecki
-00000ea0: 6e2e 6c69 6e75 782e 7379 7374 656d 2e61  n.linux.system.a
-00000eb0: 7263 685d 0d0a 7379 7374 656d 5f72 6571  rch]..system_req
-00000ec0: 7569 7265 7320 3d20 5b0d 0a09 2320 4e65  uires = [...# Ne
-00000ed0: 6564 6564 2074 6f20 636f 6d70 696c 6520  eded to compile 
-00000ee0: 7079 6361 6972 6f20 7768 6565 6c0d 0a09  pycairo wheel...
-00000ef0: 2263 6169 726f 222c 0d0a 0923 204e 6565  "cairo",...# Nee
-00000f00: 6465 6420 746f 2063 6f6d 7069 6c65 2050  ded to compile P
-00000f10: 7947 4f62 6a65 6374 2077 6865 656c 0d0a  yGObject wheel..
-00000f20: 0922 676f 626a 6563 742d 696e 7472 6f73  ."gobject-intros
-00000f30: 7065 6374 696f 6e22 2c0d 0a09 2320 5275  pection",...# Ru
-00000f40: 6e74 696d 6520 6465 7065 6e64 656e 6369  ntime dependenci
-00000f50: 6573 2074 6861 7420 6e65 6564 2074 6f20  es that need to 
-00000f60: 6578 6973 7420 736f 2074 6861 7420 7468  exist so that th
-00000f70: 650d 0a09 2320 4172 6368 2070 6163 6b61  e...# Arch packa
-00000f80: 6765 2070 6173 7365 7320 6669 6e61 6c20  ge passes final 
-00000f90: 7661 6c69 6461 7469 6f6e 2e0d 0a09 2320  validation....# 
-00000fa0: 4e65 6564 6564 2074 6f20 7072 6f76 6964  Needed to provid
-00000fb0: 6520 4754 4b0d 0a09 2267 746b 3322 2c0d  e GTK..."gtk3",.
-00000fc0: 0a09 2320 4465 7065 6e64 656e 6369 6573  ..# Dependencies
-00000fd0: 2074 6861 7420 4754 4b20 6c6f 6f6b 7320   that GTK looks 
-00000fe0: 666f 7220 6174 2072 756e 7469 6d65 0d0a  for at runtime..
-00000ff0: 0922 6c69 6263 616e 6265 7272 6122 2c0d  ."libcanberra",.
-00001000: 0a09 2320 4e65 6564 6564 2074 6f20 7072  ..# Needed to pr
-00001010: 6f76 6964 6520 5765 624b 6974 320d 0a09  ovide WebKit2...
-00001020: 2320 2277 6562 6b69 7432 6774 6b22 2c0d  # "webkit2gtk",.
-00001030: 0a5d 0d0a 0d0a 7379 7374 656d 5f72 756e  .]....system_run
-00001040: 7469 6d65 5f72 6571 7569 7265 7320 3d20  time_requires = 
-00001050: 5b0d 0a09 2320 4e65 6564 6564 2074 6f20  [...# Needed to 
-00001060: 7072 6f76 6964 6520 4754 4b0d 0a09 2267  provide GTK..."g
-00001070: 746b 3322 2c0d 0a09 2320 4e65 6564 6564  tk3",...# Needed
-00001080: 2074 6f20 7072 6f76 6964 6520 5079 474f   to provide PyGO
-00001090: 626a 6563 7420 6269 6e64 696e 6773 0d0a  bject bindings..
-000010a0: 0922 676f 626a 6563 742d 696e 7472 6f73  ."gobject-intros
-000010b0: 7065 6374 696f 6e2d 7275 6e74 696d 6522  pection-runtime"
-000010c0: 2c0d 0a09 2320 4465 7065 6e64 656e 6369  ,...# Dependenci
-000010d0: 6573 2074 6861 7420 4754 4b20 6c6f 6f6b  es that GTK look
-000010e0: 7320 666f 7220 6174 2072 756e 7469 6d65  s for at runtime
-000010f0: 0d0a 0922 6c69 6263 616e 6265 7272 6122  ..."libcanberra"
-00001100: 2c0d 0a09 2320 4e65 6564 6564 2074 6f20  ,...# Needed to 
-00001110: 7072 6f76 6964 6520 5765 624b 6974 3220  provide WebKit2 
-00001120: 6174 2072 756e 7469 6d65 0d0a 0923 2022  at runtime...# "
-00001130: 7765 626b 6974 3267 746b 222c 0d0a 0923  webkit2gtk",...#
-00001140: 204e 6565 6465 6420 666f 7220 7079 7a62   Needed for pyzb
-00001150: 6172 2061 7420 7275 6e74 696d 650d 0a09  ar at runtime...
-00001160: 227a 6261 7222 2c0d 0a5d 0d0a 0d0a 5b74  "zbar",..]....[t
-00001170: 6f6f 6c2e 6272 6965 6663 6173 652e 6170  ool.briefcase.ap
-00001180: 702e 7864 6368 6563 6b69 6e2e 6c69 6e75  p.xdcheckin.linu
-00001190: 782e 6170 7069 6d61 6765 5d0d 0a6d 616e  x.appimage]..man
-000011a0: 796c 696e 7578 203d 2022 6d61 6e79 6c69  ylinux = "manyli
-000011b0: 6e75 785f 325f 3238 220d 0a0d 0a73 7973  nux_2_28"....sys
-000011c0: 7465 6d5f 7265 7175 6972 6573 203d 205b  tem_requires = [
-000011d0: 0d0a 0923 204e 6565 6465 6420 746f 2063  ...# Needed to c
-000011e0: 6f6d 7069 6c65 2070 7963 6169 726f 2077  ompile pycairo w
-000011f0: 6865 656c 0d0a 0922 6361 6972 6f2d 676f  heel..."cairo-go
-00001200: 626a 6563 742d 6465 7665 6c22 2c0d 0a09  bject-devel",...
-00001210: 2320 4e65 6564 6564 2074 6f20 636f 6d70  # Needed to comp
-00001220: 696c 6520 5079 474f 626a 6563 7420 7768  ile PyGObject wh
-00001230: 6565 6c0d 0a09 2267 6f62 6a65 6374 2d69  eel..."gobject-i
-00001240: 6e74 726f 7370 6563 7469 6f6e 2d64 6576  ntrospection-dev
-00001250: 656c 222c 0d0a 0923 204e 6565 6465 6420  el",...# Needed 
-00001260: 746f 2070 726f 7669 6465 2047 544b 0d0a  to provide GTK..
-00001270: 0922 6774 6b33 2d64 6576 656c 222c 0d0a  ."gtk3-devel",..
-00001280: 0923 2044 6570 656e 6465 6e63 6965 7320  .# Dependencies 
-00001290: 7468 6174 2047 544b 206c 6f6f 6b73 2066  that GTK looks f
-000012a0: 6f72 2061 7420 7275 6e74 696d 652c 2074  or at runtime, t
-000012b0: 6861 7420 6e65 6564 2074 6f20 6265 0d0a  hat need to be..
-000012c0: 0923 2069 6e20 7468 6520 6275 696c 6420  .# in the build 
-000012d0: 656e 7669 726f 6e6d 656e 7420 746f 2062  environment to b
-000012e0: 6520 7069 636b 6564 2075 7020 6279 206c  e picked up by l
-000012f0: 696e 7578 6465 706c 6f79 0d0a 0922 6c69  inuxdeploy..."li
-00001300: 6263 616e 6265 7272 612d 6774 6b33 222c  bcanberra-gtk3",
-00001310: 0d0a 0922 5061 636b 6167 654b 6974 2d67  ..."PackageKit-g
-00001320: 746b 332d 6d6f 6475 6c65 222c 0d0a 0922  tk3-module",..."
-00001330: 6776 6673 2d63 6c69 656e 7422 2c0d 0a09  gvfs-client",...
-00001340: 2320 4e65 6564 6564 2066 6f72 2070 797a  # Needed for pyz
-00001350: 6261 7220 6174 2072 756e 7469 6d65 0d0a  bar at runtime..
-00001360: 0922 7a62 6172 222c 0d0a 5d0d 0a0d 0a6c  ."zbar",..]....l
-00001370: 696e 7578 6465 706c 6f79 5f70 6c75 6769  inuxdeploy_plugi
-00001380: 6e73 203d 205b 0d0a 0922 4445 504c 4f59  ns = [..."DEPLOY
-00001390: 5f47 544b 5f56 4552 5349 4f4e 3d33 2067  _GTK_VERSION=3 g
-000013a0: 746b 222c 0d0a 5d0d 0a0d 0a5b 746f 6f6c  tk",..]....[tool
-000013b0: 2e62 7269 6566 6361 7365 2e61 7070 2e78  .briefcase.app.x
-000013c0: 6463 6865 636b 696e 2e6c 696e 7578 2e66  dcheckin.linux.f
-000013d0: 6c61 7470 616b 5d0d 0a66 6c61 7470 616b  latpak]..flatpak
-000013e0: 5f72 756e 7469 6d65 203d 2022 6f72 672e  _runtime = "org.
-000013f0: 676e 6f6d 652e 506c 6174 666f 726d 220d  gnome.Platform".
-00001400: 0a66 6c61 7470 616b 5f72 756e 7469 6d65  .flatpak_runtime
-00001410: 5f76 6572 7369 6f6e 203d 2022 3435 220d  _version = "45".
-00001420: 0a66 6c61 7470 616b 5f73 646b 203d 2022  .flatpak_sdk = "
-00001430: 6f72 672e 676e 6f6d 652e 5364 6b22 0d0a  org.gnome.Sdk"..
-00001440: 0d0a 5b74 6f6f 6c2e 6272 6965 6663 6173  ..[tool.briefcas
-00001450: 652e 6170 702e 7864 6368 6563 6b69 6e2e  e.app.xdcheckin.
-00001460: 7769 6e64 6f77 735d 0d0a 7265 7175 6972  windows]..requir
-00001470: 6573 203d 205b 0d0a 0922 746f 6761 2d77  es = [..."toga-w
-00001480: 696e 666f 726d 737e 3d30 2e34 2e30 222c  informs~=0.4.0",
-00001490: 0d0a 5d0d 0a0d 0a23 204d 6f62 696c 6520  ..]....# Mobile 
-000014a0: 6465 706c 6f79 6d65 6e74 730d 0a5b 746f  deployments..[to
-000014b0: 6f6c 2e62 7269 6566 6361 7365 2e61 7070  ol.briefcase.app
-000014c0: 2e78 6463 6865 636b 696e 2e69 4f53 5d0d  .xdcheckin.iOS].
-000014d0: 0a72 6571 7569 7265 7320 3d20 5b0d 0a09  .requires = [...
-000014e0: 2274 6f67 612d 694f 537e 3d30 2e34 2e30  "toga-iOS~=0.4.0
-000014f0: 222c 0d0a 0922 7374 642d 6e73 6c6f 677e  ",..."std-nslog~
-00001500: 3d31 2e30 2e30 222c 0d0a 5d0d 0a0d 0a5b  =1.0.0",..]....[
-00001510: 746f 6f6c 2e62 7269 6566 6361 7365 2e61  tool.briefcase.a
-00001520: 7070 2e78 6463 6865 636b 696e 2e61 6e64  pp.xdcheckin.and
-00001530: 726f 6964 5d0d 0a72 6571 7569 7265 7320  roid]..requires 
-00001540: 3d20 5b0d 0a09 2274 6f67 612d 616e 6472  = [..."toga-andr
-00001550: 6f69 647e 3d30 2e34 2e30 222c 0d0a 5d0d  oid~=0.4.0",..].
-00001560: 0a0d 0a62 7569 6c64 5f67 7261 646c 655f  ...build_gradle_
-00001570: 6465 7065 6e64 656e 6369 6573 203d 205b  dependencies = [
-00001580: 0d0a 0922 616e 6472 6f69 6478 2e61 7070  ..."androidx.app
-00001590: 636f 6d70 6174 3a61 7070 636f 6d70 6174  compat:appcompat
-000015a0: 3a31 2e30 2e32 222c 0d0a 0922 616e 6472  :1.0.2",..."andr
-000015b0: 6f69 6478 2e63 6f6e 7374 7261 696e 746c  oidx.constraintl
-000015c0: 6179 6f75 743a 636f 6e73 7472 6169 6e74  ayout:constraint
-000015d0: 6c61 796f 7574 3a31 2e31 2e33 222c 0d0a  layout:1.1.3",..
-000015e0: 5d0d 0a0d 0a62 7569 6c64 5f67 7261 646c  ]....build_gradl
-000015f0: 655f 6578 7472 615f 636f 6e74 656e 7420  e_extra_content 
-00001600: 3d20 2222 220d 0a61 6e64 726f 6964 2e64  = """..android.d
-00001610: 6566 6175 6c74 436f 6e66 6967 2e6e 646b  efaultConfig.ndk
-00001620: 2e61 6269 4669 6c74 6572 7320 3d20 5b27  .abiFilters = ['
-00001630: 6172 6d36 342d 7638 6127 5d0d 0a22 2222  arm64-v8a'].."""
-00001640: 0d0a 0d0a 2320 5765 6220 6465 706c 6f79  ....# Web deploy
-00001650: 6d65 6e74 730d 0a5b 746f 6f6c 2e62 7269  ments..[tool.bri
-00001660: 6566 6361 7365 2e61 7070 2e78 6463 6865  efcase.app.xdche
-00001670: 636b 696e 2e77 6562 5d0d 0a72 6571 7569  ckin.web]..requi
-00001680: 7265 7320 3d20 5b0d 0a09 2274 6f67 612d  res = [..."toga-
-00001690: 7765 627e 3d30 2e34 2e30 222c 0d0a 5d0d  web~=0.4.0",..].
-000016a0: 0a0d 0a73 7479 6c65 5f66 7261 6d65 776f  ...style_framewo
-000016b0: 726b 203d 2022 5368 6f65 6c61 6365 2076  rk = "Shoelace v
-000016c0: 322e 3322 0d0a                           2.3"..
+000004f0: 696e 2e5f 5f6d 6169 6e5f 5f22 2c0d 0a5d  in.__main__",..]
+00000500: 0d0a 0d0a 5b74 6f6f 6c2e 7365 7475 7074  ....[tool.setupt
+00000510: 6f6f 6c73 2e70 6163 6b61 6765 2d64 6174  ools.package-dat
+00000520: 615d 0d0a 2278 6463 6865 636b 696e 2e73  a].."xdcheckin.s
+00000530: 6572 7665 7222 203d 205b 2273 7461 7469  erver" = ["stati
+00000540: 632f 2a22 2c20 2274 656d 706c 6174 6573  c/*", "templates
+00000550: 2f2a 225d 0d0a 0d0a 5b74 6f6f 6c2e 6272  /*"]....[tool.br
+00000560: 6965 6663 6173 655d 0d0a 7072 6f6a 6563  iefcase]..projec
+00000570: 745f 6e61 6d65 203d 2022 5864 6368 6563  t_name = "Xdchec
+00000580: 6b69 6e22 0d0a 6275 6e64 6c65 203d 2022  kin"..bundle = "
+00000590: 6f72 672e 6575 2e70 6e78 6c72 2e67 6974  org.eu.pnxlr.git
+000005a0: 220d 0a0d 0a5b 746f 6f6c 2e62 7269 6566  "....[tool.brief
+000005b0: 6361 7365 2e61 7070 2e78 6463 6865 636b  case.app.xdcheck
+000005c0: 696e 5d0d 0a66 6f72 6d61 6c5f 6e61 6d65  in]..formal_name
+000005d0: 203d 2022 5864 6368 6563 6b69 6e22 0d0a   = "Xdcheckin"..
+000005e0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+000005f0: 203d 2022 2222 4368 616f 7869 6e67 2043   = """Chaoxing C
+00000600: 6865 636b 696e 2054 6f6f 6c20 666f 7220  heckin Tool for 
+00000610: 5844 552e 0d0a 2222 220d 0a69 636f 6e20  XDU..."""..icon 
+00000620: 3d20 2273 7263 2f78 6463 6865 636b 696e  = "src/xdcheckin
+00000630: 2f61 7070 2f72 6573 6f75 7263 6573 2f78  /app/resources/x
+00000640: 6463 6865 636b 696e 220d 0a73 6f75 7263  dcheckin"..sourc
+00000650: 6573 203d 205b 0d0a 0922 7372 632f 7864  es = [..."src/xd
+00000660: 6368 6563 6b69 6e22 2c0d 0a5d 0d0a 2320  checkin",..]..# 
+00000670: 7465 7374 5f73 6f75 7263 6573 203d 205b  test_sources = [
+00000680: 5d0d 0a72 6571 7569 7265 7320 3d20 5b0d  ]..requires = [.
+00000690: 0a09 2266 6c61 736b 203e 3d20 332e 302e  .."flask >= 3.0.
+000006a0: 3022 2c0d 0a09 2266 6c61 736b 2d73 6573  0",..."flask-ses
+000006b0: 7369 6f6e 203d 3d20 302e 362e 3022 2c0d  sion == 0.6.0",.
+000006c0: 0a09 2270 696c 6c6f 7720 3e3d 2038 2e34  .."pillow >= 8.4
+000006d0: 2e30 222c 0d0a 0922 7079 6372 7970 746f  .0",..."pycrypto
+000006e0: 646f 6d65 203e 3d20 332e 392e 3422 2c0d  dome >= 3.9.4",.
+000006f0: 0a09 2270 797a 6261 7220 3e3d 2030 2e31  .."pyzbar >= 0.1
+00000700: 2e38 222c 0d0a 0922 7265 7175 6573 7473  .8",..."requests
+00000710: 203e 3d20 322e 3331 2e30 222c 0d0a 0922   >= 2.31.0",..."
+00000720: 7265 7175 6573 7473 2d63 6163 6865 203e  requests-cache >
+00000730: 3d20 312e 322e 3022 2c0d 0a09 2277 6169  = 1.2.0",..."wai
+00000740: 7472 6573 7320 3e3d 2033 2e30 2e30 222c  tress >= 3.0.0",
+00000750: 0d0a 5d0d 0a23 2074 6573 745f 7265 7175  ..]..# test_requ
+00000760: 6972 6573 203d 205b 5d0d 0a0d 0a5b 746f  ires = []....[to
+00000770: 6f6c 2e62 7269 6566 6361 7365 2e61 7070  ol.briefcase.app
+00000780: 2e78 6463 6865 636b 696e 2e6d 6163 4f53  .xdcheckin.macOS
+00000790: 5d0d 0a75 6e69 7665 7273 616c 5f62 7569  ]..universal_bui
+000007a0: 6c64 203d 2074 7275 650d 0a72 6571 7569  ld = true..requi
+000007b0: 7265 7320 3d20 5b0d 0a09 2274 6f67 612d  res = [..."toga-
+000007c0: 636f 636f 617e 3d30 2e34 2e30 222c 0d0a  cocoa~=0.4.0",..
+000007d0: 0922 7374 642d 6e73 6c6f 677e 3d31 2e30  ."std-nslog~=1.0
+000007e0: 2e30 222c 0d0a 5d0d 0a0d 0a5b 746f 6f6c  .0",..]....[tool
+000007f0: 2e62 7269 6566 6361 7365 2e61 7070 2e78  .briefcase.app.x
+00000800: 6463 6865 636b 696e 2e6c 696e 7578 5d0d  dcheckin.linux].
+00000810: 0a72 6571 7569 7265 7320 3d20 5b0d 0a09  .requires = [...
+00000820: 2274 6f67 612d 6774 6b7e 3d30 2e34 2e30  "toga-gtk~=0.4.0
+00000830: 222c 0d0a 5d0d 0a0d 0a5b 746f 6f6c 2e62  ",..]....[tool.b
+00000840: 7269 6566 6361 7365 2e61 7070 2e78 6463  riefcase.app.xdc
+00000850: 6865 636b 696e 2e6c 696e 7578 2e73 7973  heckin.linux.sys
+00000860: 7465 6d2e 6465 6269 616e 5d0d 0a73 7973  tem.debian]..sys
+00000870: 7465 6d5f 7265 7175 6972 6573 203d 205b  tem_requires = [
+00000880: 0d0a 0923 204e 6565 6465 6420 746f 2063  ...# Needed to c
+00000890: 6f6d 7069 6c65 2070 7963 6169 726f 2077  ompile pycairo w
+000008a0: 6865 656c 0d0a 0922 6c69 6263 6169 726f  heel..."libcairo
+000008b0: 322d 6465 7622 2c0d 0a09 2320 4e65 6564  2-dev",...# Need
+000008c0: 6564 2074 6f20 636f 6d70 696c 6520 5079  ed to compile Py
+000008d0: 474f 626a 6563 7420 7768 6565 6c0d 0a09  GObject wheel...
+000008e0: 226c 6962 6769 7265 706f 7369 746f 7279  "libgirepository
+000008f0: 312e 302d 6465 7622 2c0d 0a5d 0d0a 0d0a  1.0-dev",..]....
+00000900: 7379 7374 656d 5f72 756e 7469 6d65 5f72  system_runtime_r
+00000910: 6571 7569 7265 7320 3d20 5b0d 0a09 2320  equires = [...# 
+00000920: 4e65 6564 6564 2074 6f20 7072 6f76 6964  Needed to provid
+00000930: 6520 4754 4b20 616e 6420 6974 7320 4749  e GTK and its GI
+00000940: 2062 696e 6469 6e67 730d 0a09 2267 6972   bindings..."gir
+00000950: 312e 322d 6774 6b2d 332e 3022 2c0d 0a09  1.2-gtk-3.0",...
+00000960: 226c 6962 6769 7265 706f 7369 746f 7279  "libgirepository
+00000970: 2d31 2e30 2d31 222c 0d0a 0923 2044 6570  -1.0-1",...# Dep
+00000980: 656e 6465 6e63 6965 7320 7468 6174 2047  endencies that G
+00000990: 544b 206c 6f6f 6b73 2066 6f72 2061 7420  TK looks for at 
+000009a0: 7275 6e74 696d 650d 0a09 226c 6962 6361  runtime..."libca
+000009b0: 6e62 6572 7261 2d67 746b 332d 6d6f 6475  nberra-gtk3-modu
+000009c0: 6c65 222c 0d0a 0923 204e 6565 6465 6420  le",...# Needed 
+000009d0: 746f 2070 726f 7669 6465 2057 6562 4b69  to provide WebKi
+000009e0: 7432 2061 7420 7275 6e74 696d 650d 0a09  t2 at runtime...
+000009f0: 2320 2267 6972 312e 322d 7765 626b 6974  # "gir1.2-webkit
+00000a00: 322d 342e 3022 2c0d 0a09 2320 4e65 6564  2-4.0",...# Need
+00000a10: 6564 2066 6f72 2070 797a 6261 7220 6174  ed for pyzbar at
+00000a20: 2072 756e 7469 6d65 0d0a 0922 6c69 627a   runtime..."libz
+00000a30: 6261 7230 222c 0d0a 5d0d 0a0d 0a5b 746f  bar0",..]....[to
+00000a40: 6f6c 2e62 7269 6566 6361 7365 2e61 7070  ol.briefcase.app
+00000a50: 2e78 6463 6865 636b 696e 2e6c 696e 7578  .xdcheckin.linux
+00000a60: 2e73 7973 7465 6d2e 7268 656c 5d0d 0a73  .system.rhel]..s
+00000a70: 7973 7465 6d5f 7265 7175 6972 6573 203d  ystem_requires =
+00000a80: 205b 0d0a 0923 204e 6565 6465 6420 746f   [...# Needed to
+00000a90: 2063 6f6d 7069 6c65 2070 7963 6169 726f   compile pycairo
+00000aa0: 2077 6865 656c 0d0a 0922 6361 6972 6f2d   wheel..."cairo-
+00000ab0: 676f 626a 6563 742d 6465 7665 6c22 2c0d  gobject-devel",.
+00000ac0: 0a09 2320 4e65 6564 6564 2074 6f20 636f  ..# Needed to co
+00000ad0: 6d70 696c 6520 5079 474f 626a 6563 7420  mpile PyGObject 
+00000ae0: 7768 6565 6c0d 0a09 2267 6f62 6a65 6374  wheel..."gobject
+00000af0: 2d69 6e74 726f 7370 6563 7469 6f6e 2d64  -introspection-d
+00000b00: 6576 656c 222c 0d0a 5d0d 0a0d 0a73 7973  evel",..]....sys
+00000b10: 7465 6d5f 7275 6e74 696d 655f 7265 7175  tem_runtime_requ
+00000b20: 6972 6573 203d 205b 0d0a 0923 204e 6565  ires = [...# Nee
+00000b30: 6465 6420 746f 2073 7570 706f 7274 2050  ded to support P
+00000b40: 7974 686f 6e20 6269 6e64 696e 6773 2074  ython bindings t
+00000b50: 6f20 4754 4b0d 0a09 2267 6f62 6a65 6374  o GTK..."gobject
+00000b60: 2d69 6e74 726f 7370 6563 7469 6f6e 222c  -introspection",
+00000b70: 0d0a 0923 204e 6565 6465 6420 746f 2070  ...# Needed to p
+00000b80: 726f 7669 6465 2047 544b 0d0a 0922 6774  rovide GTK..."gt
+00000b90: 6b33 222c 0d0a 0923 2044 6570 656e 6465  k3",...# Depende
+00000ba0: 6e63 6965 7320 7468 6174 2047 544b 206c  ncies that GTK l
+00000bb0: 6f6f 6b73 2066 6f72 2061 7420 7275 6e74  ooks for at runt
+00000bc0: 696d 650d 0a09 226c 6962 6361 6e62 6572  ime..."libcanber
+00000bd0: 7261 2d67 746b 3322 2c0d 0a09 2320 4e65  ra-gtk3",...# Ne
+00000be0: 6564 6564 2074 6f20 7072 6f76 6964 6520  eded to provide 
+00000bf0: 5765 624b 6974 3220 6174 2072 756e 7469  WebKit2 at runti
+00000c00: 6d65 0d0a 0923 2022 7765 626b 6974 3267  me...# "webkit2g
+00000c10: 746b 3322 2c0d 0a09 2320 4e65 6564 6564  tk3",...# Needed
+00000c20: 2066 6f72 2070 797a 6261 7220 6174 2072   for pyzbar at r
+00000c30: 756e 7469 6d65 0d0a 0922 7a62 6172 2d6c  untime..."zbar-l
+00000c40: 6962 7322 2c0d 0a5d 0d0a 0d0a 5b74 6f6f  ibs",..]....[too
+00000c50: 6c2e 6272 6965 6663 6173 652e 6170 702e  l.briefcase.app.
+00000c60: 7864 6368 6563 6b69 6e2e 6c69 6e75 782e  xdcheckin.linux.
+00000c70: 7379 7374 656d 2e73 7573 655d 0d0a 7379  system.suse]..sy
+00000c80: 7374 656d 5f72 6571 7569 7265 7320 3d20  stem_requires = 
+00000c90: 5b0d 0a09 2320 4e65 6564 6564 2074 6f20  [...# Needed to 
+00000ca0: 636f 6d70 696c 6520 7079 6361 6972 6f20  compile pycairo 
+00000cb0: 7768 6565 6c0d 0a09 2263 6169 726f 2d64  wheel..."cairo-d
+00000cc0: 6576 656c 222c 0d0a 0923 204e 6565 6465  evel",...# Neede
+00000cd0: 6420 746f 2063 6f6d 7069 6c65 2050 7947  d to compile PyG
+00000ce0: 4f62 6a65 6374 2077 6865 656c 0d0a 0922  Object wheel..."
+00000cf0: 676f 626a 6563 742d 696e 7472 6f73 7065  gobject-introspe
+00000d00: 6374 696f 6e2d 6465 7665 6c22 2c0d 0a5d  ction-devel",..]
+00000d10: 0d0a 0d0a 7379 7374 656d 5f72 756e 7469  ....system_runti
+00000d20: 6d65 5f72 6571 7569 7265 7320 3d20 5b0d  me_requires = [.
+00000d30: 0a09 2320 4e65 6564 6564 2074 6f20 7072  ..# Needed to pr
+00000d40: 6f76 6964 6520 4754 4b0d 0a09 2267 746b  ovide GTK..."gtk
+00000d50: 3322 2c0d 0a09 2320 4e65 6564 6564 2074  3",...# Needed t
+00000d60: 6f20 7375 7070 6f72 7420 5079 7468 6f6e  o support Python
+00000d70: 2062 696e 6469 6e67 7320 746f 2047 544b   bindings to GTK
+00000d80: 0d0a 0922 676f 626a 6563 742d 696e 7472  ..."gobject-intr
+00000d90: 6f73 7065 6374 696f 6e22 2c20 2274 7970  ospection", "typ
+00000da0: 656c 6962 2847 746b 293d 332e 3022 2c0d  elib(Gtk)=3.0",.
+00000db0: 0a09 2320 4465 7065 6e64 656e 6369 6573  ..# Dependencies
+00000dc0: 2074 6861 7420 4754 4b20 6c6f 6f6b 7320   that GTK looks 
+00000dd0: 666f 7220 6174 2072 756e 7469 6d65 0d0a  for at runtime..
+00000de0: 0922 6c69 6263 616e 6265 7272 612d 6774  ."libcanberra-gt
+00000df0: 6b33 2d30 222c 0d0a 0923 204e 6565 6465  k3-0",...# Neede
+00000e00: 6420 746f 2070 726f 7669 6465 2057 6562  d to provide Web
+00000e10: 4b69 7432 2061 7420 7275 6e74 696d 650d  Kit2 at runtime.
+00000e20: 0a09 2320 226c 6962 7765 626b 6974 3267  ..# "libwebkit2g
+00000e30: 746b 3322 2c0d 0a09 2320 2274 7970 656c  tk3",...# "typel
+00000e40: 6962 2857 6562 4b69 7432 2922 2c0d 0a09  ib(WebKit2)",...
+00000e50: 2320 4e65 6564 6564 2066 6f72 2070 797a  # Needed for pyz
+00000e60: 6261 7220 6174 2072 756e 7469 6d65 0d0a  bar at runtime..
+00000e70: 0922 6c69 627a 6261 7230 222c 0d0a 5d0d  ."libzbar0",..].
+00000e80: 0a0d 0a5b 746f 6f6c 2e62 7269 6566 6361  ...[tool.briefca
+00000e90: 7365 2e61 7070 2e78 6463 6865 636b 696e  se.app.xdcheckin
+00000ea0: 2e6c 696e 7578 2e73 7973 7465 6d2e 6172  .linux.system.ar
+00000eb0: 6368 5d0d 0a73 7973 7465 6d5f 7265 7175  ch]..system_requ
+00000ec0: 6972 6573 203d 205b 0d0a 0923 204e 6565  ires = [...# Nee
+00000ed0: 6465 6420 746f 2063 6f6d 7069 6c65 2070  ded to compile p
+00000ee0: 7963 6169 726f 2077 6865 656c 0d0a 0922  ycairo wheel..."
+00000ef0: 6361 6972 6f22 2c0d 0a09 2320 4e65 6564  cairo",...# Need
+00000f00: 6564 2074 6f20 636f 6d70 696c 6520 5079  ed to compile Py
+00000f10: 474f 626a 6563 7420 7768 6565 6c0d 0a09  GObject wheel...
+00000f20: 2267 6f62 6a65 6374 2d69 6e74 726f 7370  "gobject-introsp
+00000f30: 6563 7469 6f6e 222c 0d0a 0923 2052 756e  ection",...# Run
+00000f40: 7469 6d65 2064 6570 656e 6465 6e63 6965  time dependencie
+00000f50: 7320 7468 6174 206e 6565 6420 746f 2065  s that need to e
+00000f60: 7869 7374 2073 6f20 7468 6174 2074 6865  xist so that the
+00000f70: 0d0a 0923 2041 7263 6820 7061 636b 6167  ...# Arch packag
+00000f80: 6520 7061 7373 6573 2066 696e 616c 2076  e passes final v
+00000f90: 616c 6964 6174 696f 6e2e 0d0a 0923 204e  alidation....# N
+00000fa0: 6565 6465 6420 746f 2070 726f 7669 6465  eeded to provide
+00000fb0: 2047 544b 0d0a 0922 6774 6b33 222c 0d0a   GTK..."gtk3",..
+00000fc0: 0923 2044 6570 656e 6465 6e63 6965 7320  .# Dependencies 
+00000fd0: 7468 6174 2047 544b 206c 6f6f 6b73 2066  that GTK looks f
+00000fe0: 6f72 2061 7420 7275 6e74 696d 650d 0a09  or at runtime...
+00000ff0: 226c 6962 6361 6e62 6572 7261 222c 0d0a  "libcanberra",..
+00001000: 0923 204e 6565 6465 6420 746f 2070 726f  .# Needed to pro
+00001010: 7669 6465 2057 6562 4b69 7432 0d0a 0923  vide WebKit2...#
+00001020: 2022 7765 626b 6974 3267 746b 222c 0d0a   "webkit2gtk",..
+00001030: 5d0d 0a0d 0a73 7973 7465 6d5f 7275 6e74  ]....system_runt
+00001040: 696d 655f 7265 7175 6972 6573 203d 205b  ime_requires = [
+00001050: 0d0a 0923 204e 6565 6465 6420 746f 2070  ...# Needed to p
+00001060: 726f 7669 6465 2047 544b 0d0a 0922 6774  rovide GTK..."gt
+00001070: 6b33 222c 0d0a 0923 204e 6565 6465 6420  k3",...# Needed 
+00001080: 746f 2070 726f 7669 6465 2050 7947 4f62  to provide PyGOb
+00001090: 6a65 6374 2062 696e 6469 6e67 730d 0a09  ject bindings...
+000010a0: 2267 6f62 6a65 6374 2d69 6e74 726f 7370  "gobject-introsp
+000010b0: 6563 7469 6f6e 2d72 756e 7469 6d65 222c  ection-runtime",
+000010c0: 0d0a 0923 2044 6570 656e 6465 6e63 6965  ...# Dependencie
+000010d0: 7320 7468 6174 2047 544b 206c 6f6f 6b73  s that GTK looks
+000010e0: 2066 6f72 2061 7420 7275 6e74 696d 650d   for at runtime.
+000010f0: 0a09 226c 6962 6361 6e62 6572 7261 222c  .."libcanberra",
+00001100: 0d0a 0923 204e 6565 6465 6420 746f 2070  ...# Needed to p
+00001110: 726f 7669 6465 2057 6562 4b69 7432 2061  rovide WebKit2 a
+00001120: 7420 7275 6e74 696d 650d 0a09 2320 2277  t runtime...# "w
+00001130: 6562 6b69 7432 6774 6b22 2c0d 0a09 2320  ebkit2gtk",...# 
+00001140: 4e65 6564 6564 2066 6f72 2070 797a 6261  Needed for pyzba
+00001150: 7220 6174 2072 756e 7469 6d65 0d0a 0922  r at runtime..."
+00001160: 7a62 6172 222c 0d0a 5d0d 0a0d 0a5b 746f  zbar",..]....[to
+00001170: 6f6c 2e62 7269 6566 6361 7365 2e61 7070  ol.briefcase.app
+00001180: 2e78 6463 6865 636b 696e 2e6c 696e 7578  .xdcheckin.linux
+00001190: 2e61 7070 696d 6167 655d 0d0a 6d61 6e79  .appimage]..many
+000011a0: 6c69 6e75 7820 3d20 226d 616e 796c 696e  linux = "manylin
+000011b0: 7578 5f32 5f32 3822 0d0a 0d0a 7379 7374  ux_2_28"....syst
+000011c0: 656d 5f72 6571 7569 7265 7320 3d20 5b0d  em_requires = [.
+000011d0: 0a09 2320 4e65 6564 6564 2074 6f20 636f  ..# Needed to co
+000011e0: 6d70 696c 6520 7079 6361 6972 6f20 7768  mpile pycairo wh
+000011f0: 6565 6c0d 0a09 2263 6169 726f 2d67 6f62  eel..."cairo-gob
+00001200: 6a65 6374 2d64 6576 656c 222c 0d0a 0923  ject-devel",...#
+00001210: 204e 6565 6465 6420 746f 2063 6f6d 7069   Needed to compi
+00001220: 6c65 2050 7947 4f62 6a65 6374 2077 6865  le PyGObject whe
+00001230: 656c 0d0a 0922 676f 626a 6563 742d 696e  el..."gobject-in
+00001240: 7472 6f73 7065 6374 696f 6e2d 6465 7665  trospection-deve
+00001250: 6c22 2c0d 0a09 2320 4e65 6564 6564 2074  l",...# Needed t
+00001260: 6f20 7072 6f76 6964 6520 4754 4b0d 0a09  o provide GTK...
+00001270: 2267 746b 332d 6465 7665 6c22 2c0d 0a09  "gtk3-devel",...
+00001280: 2320 4465 7065 6e64 656e 6369 6573 2074  # Dependencies t
+00001290: 6861 7420 4754 4b20 6c6f 6f6b 7320 666f  hat GTK looks fo
+000012a0: 7220 6174 2072 756e 7469 6d65 2c20 7468  r at runtime, th
+000012b0: 6174 206e 6565 6420 746f 2062 650d 0a09  at need to be...
+000012c0: 2320 696e 2074 6865 2062 7569 6c64 2065  # in the build e
+000012d0: 6e76 6972 6f6e 6d65 6e74 2074 6f20 6265  nvironment to be
+000012e0: 2070 6963 6b65 6420 7570 2062 7920 6c69   picked up by li
+000012f0: 6e75 7864 6570 6c6f 790d 0a09 226c 6962  nuxdeploy..."lib
+00001300: 6361 6e62 6572 7261 2d67 746b 3322 2c0d  canberra-gtk3",.
+00001310: 0a09 2250 6163 6b61 6765 4b69 742d 6774  .."PackageKit-gt
+00001320: 6b33 2d6d 6f64 756c 6522 2c0d 0a09 2267  k3-module",..."g
+00001330: 7666 732d 636c 6965 6e74 222c 0d0a 0923  vfs-client",...#
+00001340: 204e 6565 6465 6420 666f 7220 7079 7a62   Needed for pyzb
+00001350: 6172 2061 7420 7275 6e74 696d 650d 0a09  ar at runtime...
+00001360: 227a 6261 7222 2c0d 0a5d 0d0a 0d0a 6c69  "zbar",..]....li
+00001370: 6e75 7864 6570 6c6f 795f 706c 7567 696e  nuxdeploy_plugin
+00001380: 7320 3d20 5b0d 0a09 2244 4550 4c4f 595f  s = [..."DEPLOY_
+00001390: 4754 4b5f 5645 5253 494f 4e3d 3320 6774  GTK_VERSION=3 gt
+000013a0: 6b22 2c0d 0a5d 0d0a 0d0a 5b74 6f6f 6c2e  k",..]....[tool.
+000013b0: 6272 6965 6663 6173 652e 6170 702e 7864  briefcase.app.xd
+000013c0: 6368 6563 6b69 6e2e 6c69 6e75 782e 666c  checkin.linux.fl
+000013d0: 6174 7061 6b5d 0d0a 666c 6174 7061 6b5f  atpak]..flatpak_
+000013e0: 7275 6e74 696d 6520 3d20 226f 7267 2e67  runtime = "org.g
+000013f0: 6e6f 6d65 2e50 6c61 7466 6f72 6d22 0d0a  nome.Platform"..
+00001400: 666c 6174 7061 6b5f 7275 6e74 696d 655f  flatpak_runtime_
+00001410: 7665 7273 696f 6e20 3d20 2234 3522 0d0a  version = "45"..
+00001420: 666c 6174 7061 6b5f 7364 6b20 3d20 226f  flatpak_sdk = "o
+00001430: 7267 2e67 6e6f 6d65 2e53 646b 220d 0a0d  rg.gnome.Sdk"...
+00001440: 0a5b 746f 6f6c 2e62 7269 6566 6361 7365  .[tool.briefcase
+00001450: 2e61 7070 2e78 6463 6865 636b 696e 2e77  .app.xdcheckin.w
+00001460: 696e 646f 7773 5d0d 0a72 6571 7569 7265  indows]..require
+00001470: 7320 3d20 5b0d 0a09 2274 6f67 612d 7769  s = [..."toga-wi
+00001480: 6e66 6f72 6d73 7e3d 302e 342e 3022 2c0d  nforms~=0.4.0",.
+00001490: 0a5d 0d0a 0d0a 2320 4d6f 6269 6c65 2064  .]....# Mobile d
+000014a0: 6570 6c6f 796d 656e 7473 0d0a 5b74 6f6f  eployments..[too
+000014b0: 6c2e 6272 6965 6663 6173 652e 6170 702e  l.briefcase.app.
+000014c0: 7864 6368 6563 6b69 6e2e 694f 535d 0d0a  xdcheckin.iOS]..
+000014d0: 7265 7175 6972 6573 203d 205b 0d0a 0922  requires = [..."
+000014e0: 746f 6761 2d69 4f53 7e3d 302e 342e 3022  toga-iOS~=0.4.0"
+000014f0: 2c0d 0a09 2273 7464 2d6e 736c 6f67 7e3d  ,..."std-nslog~=
+00001500: 312e 302e 3022 2c0d 0a5d 0d0a 0d0a 5b74  1.0.0",..]....[t
+00001510: 6f6f 6c2e 6272 6965 6663 6173 652e 6170  ool.briefcase.ap
+00001520: 702e 7864 6368 6563 6b69 6e2e 616e 6472  p.xdcheckin.andr
+00001530: 6f69 645d 0d0a 7265 7175 6972 6573 203d  oid]..requires =
+00001540: 205b 0d0a 0922 746f 6761 2d61 6e64 726f   [..."toga-andro
+00001550: 6964 7e3d 302e 342e 3022 2c0d 0a5d 0d0a  id~=0.4.0",..]..
+00001560: 0d0a 6275 696c 645f 6772 6164 6c65 5f64  ..build_gradle_d
+00001570: 6570 656e 6465 6e63 6965 7320 3d20 5b0d  ependencies = [.
+00001580: 0a09 2261 6e64 726f 6964 782e 6170 7063  .."androidx.appc
+00001590: 6f6d 7061 743a 6170 7063 6f6d 7061 743a  ompat:appcompat:
+000015a0: 312e 302e 3222 2c0d 0a09 2261 6e64 726f  1.0.2",..."andro
+000015b0: 6964 782e 636f 6e73 7472 6169 6e74 6c61  idx.constraintla
+000015c0: 796f 7574 3a63 6f6e 7374 7261 696e 746c  yout:constraintl
+000015d0: 6179 6f75 743a 312e 312e 3322 2c0d 0a5d  ayout:1.1.3",..]
+000015e0: 0d0a 0d0a 6275 696c 645f 6772 6164 6c65  ....build_gradle
+000015f0: 5f65 7874 7261 5f63 6f6e 7465 6e74 203d  _extra_content =
+00001600: 2022 2222 0d0a 616e 6472 6f69 642e 6465   """..android.de
+00001610: 6661 756c 7443 6f6e 6669 672e 6e64 6b2e  faultConfig.ndk.
+00001620: 6162 6946 696c 7465 7273 203d 205b 2761  abiFilters = ['a
+00001630: 726d 3634 2d76 3861 275d 0d0a 2222 220d  rm64-v8a']..""".
+00001640: 0a0d 0a23 2057 6562 2064 6570 6c6f 796d  ...# Web deploym
+00001650: 656e 7473 0d0a 5b74 6f6f 6c2e 6272 6965  ents..[tool.brie
+00001660: 6663 6173 652e 6170 702e 7864 6368 6563  fcase.app.xdchec
+00001670: 6b69 6e2e 7765 625d 0d0a 7265 7175 6972  kin.web]..requir
+00001680: 6573 203d 205b 0d0a 0922 746f 6761 2d77  es = [..."toga-w
+00001690: 6562 7e3d 302e 342e 3022 2c0d 0a5d 0d0a  eb~=0.4.0",..]..
+000016a0: 0d0a 7374 796c 655f 6672 616d 6577 6f72  ..style_framewor
+000016b0: 6b20 3d20 2253 686f 656c 6163 6520 7632  k = "Shoelace v2
+000016c0: 2e33 220d 0a                             .3"..
```

### Comparing `Xdcheckin-2.0.4/src/Xdcheckin.egg-info/PKG-INFO` & `xdcheckin-2.0.5/src/Xdcheckin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xdcheckin
-Version: 2.0.4
+Version: 2.0.5
 Summary: Chaoxing Checkin Tool for XDU.
 Author-email: Pairman <pairmanxlr@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Pairman/Xdcheckin
 Project-URL: Changelog, https://github.com/Pairman/Xdcheckin/blob/main/CHANGELOG.md
 Keywords: xdu,xidian,chaoxing,livestream
 Classifier: Framework :: Flask
```

### Comparing `Xdcheckin-2.0.4/src/Xdcheckin.egg-info/SOURCES.txt` & `xdcheckin-2.0.5/src/Xdcheckin.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,8 +24,9 @@
 src/xdcheckin/server/static/login.js
 src/xdcheckin/server/static/misc.js
 src/xdcheckin/server/static/player.js
 src/xdcheckin/server/static/style.css
 src/xdcheckin/server/static/util.js
 src/xdcheckin/server/templates/index.html
 src/xdcheckin/util/__init__.py
-src/xdcheckin/util/chaoxing_captcha.py
+src/xdcheckin/util/chaoxing_captcha.py
+src/xdcheckin/util/encryption.py
```

### Comparing `Xdcheckin-2.0.4/src/xdcheckin/core/chaoxing.py` & `xdcheckin-2.0.5/src/xdcheckin/core/chaoxing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 # -*- coding: utf-8 -*-
 
-from ast import literal_eval
-from base64 import b64encode
-from Crypto.Cipher.AES import new as AES_new, block_size as AES_block_size, MODE_CBC as AES_MODE_CBC
-from Crypto.Util.Padding import pad
-from datetime import datetime
-from json import dumps
-from random import choice, uniform
-from re import findall, search, DOTALL
-from requests import Response
-from requests.exceptions import RequestException
-from requests_cache.session import CachedSession
-from threading import Thread
-from xdcheckin.util.chaoxing_captcha import generate_secrets
+from ast import literal_eval as _literal_eval
+from datetime import datetime as _datetime
+from json import dumps as _dumps
+from random import choice as _choice, uniform as _uniform
+from re import findall as _findall, search as _search, DOTALL as _DOTALL
+from requests import Response as _Response
+from requests.adapters import HTTPAdapter as _HTTPAdapter
+from requests.exceptions import RequestException as _RequestException
+from requests_cache.session import CachedSession as _CachedSession
+from threading import Thread as _Thread
+from xdcheckin.util.chaoxing_captcha import generate_secrets as _generate_secrets
+from xdcheckin.util.encryption import encrypt_aes as _encrypt_aes
 
 class Chaoxing:
 	"""Common Chaoxing APIs.
 	"""
 	requests_session = name = cookies = courses = logined = None
 	config = {
 		"requests_headers": {
-			"User-Agent": "Mozilla/5.0 (Linux; Android 10; K) Apple"
-				      "WebKit/537.36 (KHTML, like Gecko) Chrome"
-				      "/120.0.0.0 Mobile Safari/537.36 com.chao"
-				      "xing.mobile/ChaoXingStudy_3_6.1.0_androi"
-				      "d_phone_906_100"
+			"User-Agent":
+				"Mozilla/5.0 (Linux; Android 10; K) AppleWebKit"
+				"/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 M"
+				"obile Safari/537.36 com.chaoxing.mobile/ChaoXi"
+				"ngStudy_3_6.1.0_android_phone_906_100"
 		},
 		"requests_cache_enabled": True,
 		"chaoxing_course_get_activities_courses_limit": 32,
 		"chaoxing_course_get_activities_workers": 16,
 		"chaoxing_checkin_location_address_override_maxlen": 0,
 		"chaoxing_checkin_location_randomness": True
 	}
@@ -36,24 +35,24 @@
 	def __init__(
 		self, username: str = "", password: str = "", cookies = None,
 		config: dict = {}
 	):
 		"""Create a Chaoxing instance and login.
 		:param username: Chaoxing username. Unused if cookies are given.
 		:param password: Chaoxing password. Unused if cookies are given.
-		:param cookies: Cookies from previous login. Overrides username and password if given.
+		:param cookies: Cookies from previous login. 
+		Overrides username and password if given.
 		:param config: Configurations for the instance.
 		:return: None.
 		"""
 		if self.logined:
 			return
 		self.config.update(config)
-		self.requests_session = CachedSession(backend = "memory")
-		for adapter in self.requests_session.adapters.values():
-			adapter._pool_maxsize = 32
+		self.requests_session = _CachedSession(backend = "memory")
+		self.requests_session.mount("https://", _HTTPAdapter(pool_maxsize = 32))
 		account = {"username": username, "password": password, "cookies": cookies}
 		if cookies:
 			self.name, self.cookies, self.logined = self.login_cookies(account = account).values()
 		if not self.logined and username and password:
 			for func in (
 				self.login_username_fanya,
 				self.login_username_v2,
@@ -86,18 +85,18 @@
 				cookies = cookies or self.cookies,
 				headers = headers or self.config["requests_headers"],
 				expire_after = expire_after if self.config["requests_cache_enabled"] else 0,
 				**{"verify": False, **kwargs}
 			)
 			assert res.status_code in (200, 500), res.status_code
 		except AssertionError as e:
-			res = Response()
+			res = _Response()
 			res.status_code, res._content = int(str(e)), b"{}"
-		except RequestException:
-			res = Response()
+		except _RequestException:
+			res = _Response()
 			res.status_code, res._content = 404, b"{}"
 		finally:
 			return res
 
 	def post(
 		self, url: str = "", data: dict = {}, cookies: dict = None,
 		headers: dict = None, expire_after: int = 0, **kwargs
@@ -116,26 +115,27 @@
 				cookies = cookies or self.cookies,
 				headers = headers or self.config["requests_headers"],
 				expire_after = expire_after if self.config["requests_cache_enabled"] else 0,
 				**{"verify": False, **kwargs}
 			)
 			assert res.status_code in (200, 500), res.status_code
 		except AssertionError as e:
-			res = Response()
+			res = _Response()
 			res.status_code, res._content = int(str(e)), b"{}"
-		except RequestException:
-			res = Response()
+		except _RequestException:
+			res = _Response()
 			res.status_code, res._content = 404, b"{}"
 		finally:
 			return res
 
 	def login_username_v2(
 		self, account: dict = {"username": "", "password": ""}
 	):
-		"""Log into Chaoxing account with username and password via V2 API.
+		"""Log into Chaoxing account with username and password 
+		via V2 API.
 		:param account: Username and password in dictionary.
 		:return: Name, cookies and login state.
 		"""
 		url = "https://passport2.chaoxing.com/api/v2/loginbypwd"
 		params = {
 			"name": account["username"],
 			"pwd": account["password"]
@@ -154,15 +154,16 @@
 				"logined": True
 			})
 		return ret
 
 	def login_username_v3(
 		self, account: dict = {"username": "", "password": ""}
 	):
-		"""Log into Chaoxing account with username and password via V3 API.
+		"""Log into Chaoxing account with username and password 
+		via V3 API.
 		:param account: Same as login_username_v2().
 		:return: Name (placeholder), cookies and login state.
 		"""
 		url = "http://v3.chaoxing.com/vLogin"
 		data = {
 			"userNumber": account["username"],
 			"passWord": account["password"]
@@ -179,29 +180,30 @@
 				"logined": True
 			})
 		return ret
 
 	def login_username_v5(
 		self, account: dict = {"username": "", "password": ""}
 	):
-		"""Log into Chaoxing account with username and password via V5 API.
+		"""Log into Chaoxing account with username and password 
+		via V5 API.
 		:param account: Same as login_username_v2().
 		:return: Same as login_username_v2().
 		"""
 		url = "https://v5.chaoxing.com/login/passportLogin"
 		data = {
 			"userNumber": account["username"],
 			"passWord": account["password"]
 		}
 		ret = {
 			"name": "",
 			"cookies": None,
 			"logined": False
 		}
-		res = self.post(url = url, data = dumps(data), headers = {
+		res = self.post(url = url, data = _dumps(data), headers = {
 			**self.config["requests_headers"],
 			"Content-Type": "application/json;charset=UTF-8"
 		})
 		if res.status_code == 200 and res.cookies.get("p_auth_token"):
 			data = res.json()
 			ret.update({
 				"name": data["data"]["realname"],
@@ -209,15 +211,16 @@
 				"logined": True
 			})
 		return ret
 
 	def login_username_v11(
 		self, account: dict = {"username": "", "password": ""}
 	):
-		"""Log into Chaoxing account with username and password via V11 API.
+		"""Log into Chaoxing account with username and password 
+		via V11 API.
 		:param account: Same as login_username_v2().
 		:return: Same as login_username_v3().
 		"""
 		url = "https://passport2.chaoxing.com/v11/loginregister"
 		params = {
 			"uname": account["username"],
 			"code": account["password"]
@@ -234,15 +237,16 @@
 				"logined": True
 			})
 		return ret
 
 	def login_username_mylogin1(
 		self, account: dict = {"username": "", "password": ""}
 	):
-		"""Log into Chaoxing account with username and password via Mylogin1 API.
+		"""Log into Chaoxing account with username and password 
+		via Mylogin1 API.
 		:param account: Same as login_username_v2().
 		:return: Same as login_username_v3().
 		"""
 		url = "https://passport2.chaoxing.com/mylogin1"
 		data = {
 			"msg": account["username"],
 			"vercode": account["password"],
@@ -261,15 +265,16 @@
 				"logined": True
 			})
 		return ret
 
 	def login_username_xxk(
 		self, account: dict = {"username": "", "password": ""}
 	):
-		"""Log into Chaoxing account with username and password via XXK API.
+		"""Log into Chaoxing account with username and password 
+		via XXK API.
 		:param account: Same as login_username_v2().
 		:return: Same as login_username_v3().
 		"""
 		url = "http://xxk.chaoxing.com/api/front/user/login"
 		params = {
 			"username": account["username"],
 			"password": account["password"],
@@ -287,30 +292,31 @@
 				"logined": True
 			})
 		return ret
 
 	def login_username_fanya(
 		self, account: dict = {"username": "", "password": ""}
 	):
-		"""Log into Chaoxing account with username and password via Fanya API.
+		"""Log into Chaoxing account with username and password 
+		via Fanya API.
 		:param account: Same as login_username_v2().
 		:return: Same as login_username_v3().
 		"""
-		def _encrypt_aes(msg: str = "", key: str = "u2oh6Vu^HWe4_AES"):
-			enc = AES_new(
-				key.encode("utf-8"), AES_MODE_CBC,
-				key.encode("utf-8")
-			).encrypt(pad(
-				msg.encode("utf-8"), AES_block_size, "pkcs7"
-			))
-			return b64encode(enc).decode("utf-8")
 		url = "https://passport2.chaoxing.com/fanyalogin"
 		data = {
-				"uname": _encrypt_aes(msg = account["username"]),
-				"password": _encrypt_aes(msg = account["password"]),
+				"uname": _encrypt_aes(
+					msg = account["username"],
+					key = b"u2oh6Vu^HWe4_AES",
+					iv = b"u2oh6Vu^HWe4_AES"
+				),
+				"password": _encrypt_aes(
+					msg = account["password"],
+					key = b"u2oh6Vu^HWe4_AES",
+					iv = b"u2oh6Vu^HWe4_AES"
+				),
 				"t": True
 			}
 		ret = {
 			"name": "",
 			"cookies": None,
 			"logined": False
 		}
@@ -343,15 +349,17 @@
 					"logined": True
 				})
 		return ret
 
 	def curriculum_get_curriculum(self, week: str = ""):
 		"""Get curriculum.
 		:param week: Week number. Defaulted to the current week.
-		:return: Dictionary of curriculum details and lessons containing course IDs, names, classroom locations, teachers and time.
+		:return: Dictionary of curriculum details and lessons 
+		containing course IDs, names, classroom locations, teachers 
+		and time.
 		"""
 		def _add_lesson(lesson: dict = {}):
 			lesson_class_id = str(lesson["classId"])
 			lesson = {
 				"course_id": str(lesson["courseId"]),
 				"name": lesson["name"],
 				"locations": [lesson["location"]],
@@ -398,22 +406,28 @@
 			_add_lesson(lesson = lesson)
 			for conflict in lesson.get("conflictLessons") or {}:
 				_add_lesson(lesson = conflict)
 		return curriculum
 
 	def course_get_courses(self):
 		"""Get all courses in the root folder.
-		:return: Dictionary of class IDs to course containing course IDs, names, teachers, status, start and end time.
+		:return: Dictionary of class IDs to course containing 
+		course IDs, names, teachers, status, start and end time.
 		"""
 		url = "https://mooc1-1.chaoxing.com/visit/courselistdata"
 		params = {
 			"courseType": 1
 		}
 		res = self.get(url = url, params = params, expire_after = 86400)
-		matches = findall(r"course_(\d+)_(\d+).*?(?:(not-open).*?)?title=\"(.*?)\".*?title.*?title=\"(.*?)\"(?:.*?(\d+-\d+-\d+)～(\d+-\d+-\d+))?", res.text, DOTALL)
+		matches = _findall(
+			r"course_(\d+)_(\d+).*?(?:(not-open).*?)?title="
+			r"\"(.*?)\".*?title.*?title=\"(.*?)\""
+			r"(?:.*?(\d+-\d+-\d+)～(\d+-\d+-\d+))?",
+			res.text, _DOTALL
+		)
 		return {
 			match[1]: {
 				"class_id": match[1],
 				"course_id": match[0],
 				"name": match[3],
 				"teacher": match[4].split("，"),
 				"status": int(not bool(match[2])),
@@ -422,15 +436,16 @@
 			} for match in matches
 		}
 
 	def course_get_course_id(
 		self, course: dict = {"course_id": "", "class_id": ""}
 	):
 		"""Get course ID of a course.
-		:param course: Course ID (will be filled if not given) and clsss ID in dictionary.
+		:param course: Course ID (will be filled if not given) and 
+		clsss ID in dictionary.
 		:return: Course ID corresponding to the class ID.
 		"""
 		url = "https://mobilelearn.chaoxing.com/v2/apis/class/getClassDetail"
 		params = {
 			"fid": self.cookies.get("fid") or 0,
 			"courseId": "",
 			"classId": course["class_id"]
@@ -442,16 +457,18 @@
 			course_id = str(data.get("courseid") or 0)
 		return course_id
 
 	def course_get_location_log(
 		self, course: dict = {"course_id": "", "class_id": ""}
 	):
 		"""Get checkin location history of a course.
-		:param course: Course ID (will be filled if not given) and class ID in dictionary.
-		:return: Dictionary of activity IDs to checkin locations used by the course.
+		:param course: Course ID (will be filled if not given) and 
+		class ID in dictionary.
+		:return: Dictionary of activity IDs to checkin locations 
+		used by the course.
 		"""
 		url = "https://mobilelearn.chaoxing.com/v2/apis/sign/getLocationLog"
 		params = {
 			"DB_STRATEGY": "COURSEID",
 			"STRATEGY_PARA": "courseId",
 			"courseId": self.course_get_course_id(course = course),
 			"classId": course["class_id"]
@@ -468,16 +485,18 @@
 			} for location in data
 		}
 
 	def course_get_course_activities_v2(
 		self, course: dict = {"course_id": "", "class_id": ""}
 	):
 		"""Get activities of a course via V2 API.
-		:param course: Course ID (will be filled if not given) and class ID in dictionary.
-		:return: List of dictionaries of ongoing activities with type, name, activity ID, start, end and remaining time.
+		:param course: Course ID (will be filled if not given) and 
+		class ID in dictionary.
+		:return: List of dictionaries of ongoing activities with type, 
+		name, activity ID, start, end and remaining time.
 		"""
 		url = "https://mobilelearn.chaoxing.com/v2/apis/active/student/activelist"
 		params = {
 			"fid": self.cookies.get("fid") or 0,
 			"courseId": self.course_get_course_id(course = course),
 			"classId": course["class_id"],
 			"showNotStartedActive": 0
@@ -485,26 +504,30 @@
 		res = self.get(url = url, params = params, expire_after = 60)
 		data = (res.json().get("data") or {}).get("activeList") or []
 		return [
 			{
 				"active_id": str(activity["id"]),
 				"type": activity["otherId"],
 				"name": activity["nameOne"],
-				"time_start": str(datetime.fromtimestamp(activity["startTime"] // 1000)),
-				"time_end": str(datetime.fromtimestamp((activity["endTime"]) // 1000)) if activity["endTime"] else "",
+				"time_start": str(_datetime.fromtimestamp(activity["startTime"] // 1000)),
+				"time_end":
+					str(_datetime.fromtimestamp((activity["endTime"]) // 1000))
+					if activity["endTime"] else "",
 				"time_left": activity["nameFour"]
 			} for activity in data if activity["status"] == 1 and activity.get("otherId") in ("2", "4")
 		]
 
 	def course_get_course_activities_ppt(
 		self, course: dict = {"course_id": "", "class_id": ""}
 	):
 		"""Get activities of a course via PPT API.
-		:param course: Course ID (will be filled if not given) and class ID in dictionary.
-		:return: List of dictionaries of ongoing activities with type, name, activity ID, start, end and remaining time.
+		:param course: Course ID (will be filled if not given) and 
+		class ID in dictionary.
+		:return: List of dictionaries of ongoing activities with type, 
+		name, activity ID, start, end and remaining time.
 		"""
 		url = "https://mobilelearn.chaoxing.com/ppt/activeAPI/taskactivelist"
 		params = {
 			"courseId": self.course_get_course_id(course = course),
 			"classId": course["class_id"],
 			"showNotStartedActive": 0
 		}
@@ -513,23 +536,23 @@
 		activities = []
 		for activity in data:
 			if not activity["status"] == 1 or not activity["activeType"] == 2:
 				continue
 			activity_new = {
 				"active_id": str(activity["id"]),
 				"name": activity["nameOne"],
-				"time_start": str(datetime.fromtimestamp(activity["startTime"] // 1000)),
+				"time_start": str(_datetime.fromtimestamp(activity["startTime"] // 1000)),
 				"time_left": activity["nameFour"]
 			}
 			details = self.checkin_get_details(activity = activity_new)
 			if not details["otherId"] in (2, 4):
 				continue
 			activity_new.update({
 				"type": str(details["otherId"]),
-				"time_end": str(datetime.fromtimestamp(details["endTime"]["time"] // 1000))
+				"time_end": str(_datetime.fromtimestamp(details["endTime"]["time"] // 1000))
 			})
 			activities.append(activity_new)
 		return activities
 
 	def course_get_activities(self):
 		"""Get activities of all courses.
 		:return: Dictionary of class IDs to ongoing activities.
@@ -540,17 +563,18 @@
 				activities[course["class_id"]] = course_activities
 		activities = {}
 		nworkers = self.config["chaoxing_course_get_activities_workers"]
 		ncourses = min(self.config["chaoxing_course_get_activities_courses_limit"], len(self.courses))
 		courses = tuple(self.courses.values())[: ncourses]
 		threads = [
 			[
-				Thread(target = _get_course_activities, kwargs = {
+				_Thread(target = _get_course_activities, kwargs = {
 					"course": courses[j],
-					"func": self.course_get_course_activities_v2 if j % 2 else self.course_get_course_activities_ppt
+					"func": self.course_get_course_activities_v2 if j % 2
+						else self.course_get_course_activities_ppt
 				})
 				for j in range(i, min(i + nworkers, ncourses)) if courses[j]["status"]
 			]
 			for i in range(0, ncourses, nworkers)
 		]
 		for batch in threads:
 			for thread in batch:
@@ -571,35 +595,39 @@
 		}
 		res = self.get(url = url, params = params, expire_after = 300)
 		return res.json()
 
 	def checkin_get_pptactiveinfo(self, activity: dict = {"active_id": ""}):
 		"""Get PPT acitvity info.
 		:param activity: Activity ID in dictionary.
-		:return: Checkin PPT activity info including class ID and ranged option on success.
+		:return: Checkin PPT activity info including class ID and 
+		ranged option on success.
 		"""
 		url = "https://mobilelearn.chaoxing.com/v2/apis/active/getPPTActiveInfo"
 		params = {
 			"activeId": activity["active_id"]
 		}
 		res = self.get(url = url, params = params, expire_after = 60)
 		return res.json()["data"]
 
 	def checkin_format_location(
 		self,
 		location: dict = {"latitude": -1, "longitude": -1, "address": ""},
 		location_new: dict = {"latitude": -1, "longitude": -1, "address": ""}
 	):
 		"""Format checkin location.
-		:param location: Address, latitude and longitude in dictionary. Used for address override for checkin location.
-		:param location_new: Address, latitude and longitude in dictionary. The checkin location to upload.
-		:return: Checkin location containing address, latitude, longitude, range and ranged option.
+		:param location: Address, latitude and longitude in dictionary. 
+		Used for address override for checkin location.
+		:param location_new: Address, latitude and longitude 
+		in dictionary. The checkin location to upload.
+		:return: Checkin location containing address, latitude, 
+		longitude, range and ranged option.
 		"""
 		def _randomness(x: int | float = 0):
-			return round(x + choice((-1, 1)) * uniform(1, 5) * 0.0001, 6)
+			return round(x + _choice((-1, 1)) * _uniform(1, 5) * 0.0001, 6)
 		location_new = {
 			"ranged": 0,
 			"range": 0,
 			**location_new
 		}
 		if self.config["chaoxing_checkin_location_randomness"]:
 			location_new.update({
@@ -609,15 +637,17 @@
 		if len(location_new["address"]) < self.config["chaoxing_checkin_location_address_override_maxlen"]:
 			location_new["address"] = location["address"]
 		return location_new
 
 	def checkin_get_location_log(self, activity: dict = {"active_id": ""}):
 		"""Get checkin locations submitted by up to 100 students.
 		:param activity: Activity ID in dictionary.
-		:return: List of checkin locations containing address, latitude, longitude, range (placeholder) and ranged (placeholder) option.
+		:return: List of checkin locations containing address, 
+		latitude, longitude, range (placeholder) and 
+		ranged (placeholder) option.
 		"""
 		url = "https://mobilelearn.chaoxing.com/pptSign/autoRefeashSignList4Json2"
 		params = {
 			"activeId": activity["active_id"]
 		}
 		res = self.get(url = url, params = params)
 		data = res.json()["list"]
@@ -631,18 +661,21 @@
 			} for location in data
 		]
 
 	def checkin_get_location(
 		self, activity: dict = {"active_id": ""},
 		course: dict ={"course_id": "", "class_id": ""}
 	):
-		"""Get checkin location from the location log of its corresponding course.
+		"""Get checkin location from the location log of its 
+		corresponding course.
 		:param activity: Activity ID in dictionary.
-		:param course: Course ID (will be filled if not given) and class ID in dictionary.
-		:return: Checkin location containing address, latitude, longitude, range and ranged option.
+		:param course: Course ID (will be filled if not given) and 
+		class ID in dictionary.
+		:return: Checkin location containing address, latitude, 
+		longitude, range and ranged option.
 		"""
 		locations = self.course_get_location_log(course = course)
 		location = locations.get(activity["active_id"]) or next(iter(locations.values())) if locations else {
 				"latitude": -1,
 				"longitude": -1,
 				"address": "",
 				"ranged": 0,
@@ -663,79 +696,80 @@
 		}
 		url2 = "https://mobilelearn.chaoxing.com/pptSign/analysis2"
 		params2 = {
 			"DB_STRATEGY": "RANDOM",
 			"code": ""
 		}
 		res1 = self.get(url = url1, params = params1, expire_after = 1800)
-		params2["code"] = search(r"([0-9a-f]{32})", res1.text).group(1)
+		params2["code"] = _search(r"([0-9a-f]{32})", res1.text).group(1)
 		res2 = self.get(url = url2, params = params2, expire_after = 1800)
 		return res2.text == "success"
 
 	def checkin_get_captcha(self, captcha: dict = {"captcha_id": ""}):
 		"""Get CAPTCHA for checkin.
 		:param captcha: CAPTCHA ID in dictionary.
 		:return: CAPTCHA with CAPTCHA images and token.
 		"""
 		url1 = "https://captcha.chaoxing.com/captcha/get/conf"
 		params1 = {
 			"callback": "f",
 			"captchaId": captcha["captcha_id"],
-			"_": int(datetime.now().timestamp() * 1000)
+			"_": int(_datetime.now().timestamp() * 1000)
 		}
 		res1 = self.get(url = url1, params = params1, expire_after = 300)
-		server_time = search(r"t\":(\d+)", res1.text).group(1)
+		server_time = _search(r"t\":(\d+)", res1.text).group(1)
 		url2 = "https://captcha.chaoxing.com/captcha/get/verification/image"
 		params2 = {
 			"callback": "f",
 			"captchaId": captcha["captcha_id"],
 			"captchaKey": "",
 			"token": "",
 			"type": "slide",
 			"version": "1.1.16",
 			"referer": "https://mobilelearn.chaoxing.com",
-			"_": int(datetime.now().timestamp() * 1000)
+			"_": int(_datetime.now().timestamp() * 1000)
 		}
 		captcha_new = {
 			**captcha,
 			"server_time": server_time,
 			"type": "slide"
 		}
-		captcha_key, token = generate_secrets(captcha = captcha_new)
+		captcha_key, token = _generate_secrets(captcha = captcha_new)
 		params2.update({
 			"captchaKey": captcha_key,
 			"token": token
 		})
 		res2 = self.get(url = url2, params = params2)
-		data2 = literal_eval(res2.text[2 : -1])
+		data2 = _literal_eval(res2.text[2 : -1])
 		return {
 			**captcha_new,
 			"token": data2["token"],
 			"big_img_src": data2["imageVerificationVo"]["shadeImage"],
 			"small_img_src": data2["imageVerificationVo"]["cutoutImage"]
 		}
 
 	def checkin_submit_captcha(
 		self, captcha = {"captcha_id": "", "token": "", "vcode": ""}
 	):
 		"""Submit and verify CAPTCHA.
-		:param captcha: CAPTCHA ID, and verification code (e.g. slider offset) in dictionary.
+		:param captcha: CAPTCHA ID, and verification code (e.g. slider 
+		offset) in dictionary.
 		:return: CAPTCHA with validation code on success.
 		"""
 		url = "https://captcha.chaoxing.com/captcha/check/verification/result"
 		params = {
 			"callback": "f",
 			"captchaId": captcha["captcha_id"],
 			"token": captcha["token"],
 			"textClickArr": f"[{{\"x\": {captcha['vcode']}}}]",
 			"type": "slide",
 			"coordinate": "[]",
 			"version": "1.1.16",
 			"runEnv": 10,
-			"_": int(datetime.now().timestamp() * 1000)
+			"_": int(_datetime.now().timestamp() * 1000)
 		}
 		res = self.get(url = url, params = params, headers = {
 			**self.config["requests_headers"],
 			"Referer": "https://mobilelearn.chaoxing.com"
 		})
 		return "result\":true" in res.text, {
 			**captcha,
@@ -744,16 +778,18 @@
 
 	def checkin_do_presign(
 		self, activity: dict = {"active_id": ""},
 		course: dict ={"course_id": "", "class_id": ""}
 	):
 		"""Do checkin pre-sign.
 		:param activity: Activity ID in dictionary.
-		:param course: Course ID (will be filled if not given) and class ID in dictionary.
-		:return: Presign state (2 if checked-in and 1 on success), checkin location and CAPTCHA.
+		:param course: Course ID (will be filled if not given) and 
+		class ID in dictionary.
+		:return: Presign state (2 if checked-in and 1 on success), 
+		checkin location and CAPTCHA.
 		"""
 		url = "https://mobilelearn.chaoxing.com/newsign/preSign"
 		params = {
 			"courseId": self.course_get_course_id(course = course),
 			"classId": course["class_id"],
 			"activePrimaryId": activity["active_id"],
 			"general": 1,
@@ -774,15 +810,23 @@
 		captcha = {
 			"captcha_id": ""
 		}
 		res = self.get(url = url, params = params)
 		if res.status_code != 200:
 			return 0, location, captcha
 		state = 1
-		match = search(r"ifopenAddress\" value=\"(\d)\"(?:.*?locationText\" value=\"(.*?)\".*?locationLatitude\" value=\"(\d+\.\d+)\".*?locationLongitude\" value=\"(\d+\.\d+)\".*?locationRange\" value=\"(\d+))?.*?captchaId: '([0-9A-Za-z]{32})|(zsign_success)", res.text, DOTALL)
+		match = _search(
+			r"ifopenAddress\" value=\"(\d)\"(?:.*?locationText\" "
+			r"value=\"(.*?)\".*?locationLatitude\" value="
+			r"\"(\d+\.\d+)\".*?locationLongitude\" value="
+			r"\"(\d+\.\d+)\".*?locationRange\" value="
+			r"\"(\d+))?.*?captchaId: '([0-9A-Za-z]{32})|"
+			r"(zsign_success)",
+			res.text, _DOTALL
+		)
 		if match:
 			if match.group(7):
 				state = 2
 			if match.group(1) == "1":
 				location.update({
 					"latitude": float(match.group(3) or -1),
 					"longitude": float(match.group(4) or -1),
@@ -796,17 +840,20 @@
 	def checkin_do_sign(
 		self, activity: dict = {"active_id": "", "type": ""},
 		location: dict = {"latitude": -1, "longitude": -1, "address": "", "ranged": 0},
 		old_params: dict = {"name": "", "uid": "", "fid": "", "...": "..."}
 	):
 		"""Do checkin sign.
 		:param activity: Activity ID and type in dictionary.
-		:param location: Address, latitude, longitude and ranged option in dictionary.
-		:param prev_params: Reuse previously returned params. Overrides activity and location.
-		:return: Sign state (True on success), success / error message and payload.
+		:param location: Address, latitude, longitude and 
+		ranged option in dictionary.
+		:param prev_params: Reuse previously returned params. 
+		Overrides activity and location.
+		:return: Sign state (True on success), success / error message 
+		and payload.
 		"""
 		url = "https://mobilelearn.chaoxing.com/pptSign/stuSignajax"
 		params = old_params if old_params.get("activeId") else {
 			"name": self.name,
 			"uid": self.cookies["_uid"],
 			"fid": self.cookies.get("fid") or 0,
 			"activeId": activity["active_id"],
@@ -843,15 +890,15 @@
 			assert res.text in ("success", "您已签到过了"), res.text
 			return True, {
 				"msg": f"Checkin success. ({res.text})",
 				"params": params
 			}
 		except Exception as e:
 			if type(e) is AssertionError:
-				match = search(r"validate_([0-9A-Fa-f]{32})", str(e))
+				match = _search(r"validate_([0-9A-Fa-f]{32})", str(e))
 				if match:
 					params["enc2"] = match.group(1)
 				msg = f"Checkin failure. {params, str(e)}"
 			else:
 				msg = str(e)
 			return False, {
 				"msg": msg,
@@ -860,32 +907,37 @@
 
 	def checkin_checkin_location(
 		self, activity: dict = {"active_id": ""},
 		location: dict = {"latitude": -1, "longitude": -1, "address": ""}
 	):
 		"""Location checkin.
 		:param activity: Activity ID in dictionary.
-		:param location: Address, latitude and longitude in dictionary. Overriden by server-side location if any.
-		:return: Checkin state (True on success), message, params and captcha (placeholder if already checked-in or on failure).
+		:param location: Address, latitude and longitude in dictionary. 
+		Overriden by server-side location if any.
+		:return: Checkin state (True on success), message, params and 
+		captcha (placeholder if already checked-in or on failure).
 		"""
 		try:
-			thread_analysis = Thread(target = self.checkin_do_analysis, kwargs = {"activity": activity})
+			thread_analysis = _Thread(target = self.checkin_do_analysis, kwargs = {"activity": activity})
 			thread_analysis.start()
 			info = self.checkin_get_details(activity = activity)
 			assert info["status"] == 1 and not info["isDelete"], "Activity ended or deleted."
 			presign = self.checkin_do_presign(activity = activity, course = {"class_id": str(info["clazzId"])})
 			assert presign[0], f"Presign failure. {activity, presign}"
 			if presign[0] == 2:
 				return True, {
 					"msg": "Checkin success. (Already checked in.)",
 					"params": "",
 					"captcha": ""
 				}
 			location_new = {
-				**(self.checkin_format_location(location = location, location_new = presign[1]) if presign[1]["ranged"] else location),
+				**(
+					self.checkin_format_location(location = location, location_new = presign[1])
+					if presign[1]["ranged"] else location
+				),
 				"ranged": presign[1]["ranged"]
 			}
 			thread_analysis.join()
 			result = self.checkin_do_sign(activity = {**activity, "type": "4"}, location = location_new)
 			result[1]["captcha"] = presign[2]
 			return result
 		except Exception as e:
@@ -907,31 +959,35 @@
 		def _get_location():
 			nonlocal location_new
 			location_new = self.checkin_format_location(
 				location = location,
 				location_new = self.checkin_get_location(activity = activity, course = course)
 			)
 		try:
-			thread_analysis = Thread(target = self.checkin_do_analysis, kwargs = {"activity": activity})
+			thread_analysis = _Thread(target = self.checkin_do_analysis, kwargs = {"activity": activity})
 			thread_analysis.start()
 			info = self.checkin_get_details(activity = activity)
 			assert info["status"] == 1 and not info["isDelete"], "Activity ended or deleted."
 			course, location_new = {"class_id": str(info["clazzId"])}, {}
-			thread_location = Thread(target = _get_location)
+			thread_location = _Thread(target = _get_location)
 			thread_location.start()
 			presign = self.checkin_do_presign(activity = activity, course = course)
 			assert presign[0], f"Presign failure. {activity, presign}"
 			if presign[0] == 2:
 				return True, {
 					"msg": "Checkin success. (Already checked in.)",
 					"params": "",
 					"captcha": ""
 				}
 			location_new = {
-				**(thread_location.join() or self.checkin_format_location(location = location, location_new = location_new) if presign[1]["ranged"] else location),
+				**(
+					thread_location.join() or
+					self.checkin_format_location(location = location, location_new = location_new)
+					if presign[1]["ranged"] else location
+				),
 				"ranged": presign[1]["ranged"]
 			}
 			thread_analysis.join()
 			result = self.checkin_do_sign(activity = {**activity, "type": "2"}, location = location_new)
 			result[1]["captcha"] = presign[2]
 			return result
 		except Exception as e:
@@ -948,15 +1004,15 @@
 		"""Qrcode checkin.
 		:param url: URL from Qrcode.
 		:param location: Same as checkin_checkin_location().
 		:return: Same as checkin_checkin_location().
 		"""
 		try:
 			assert "mobilelearn.chaoxing.com/widget/sign/e" in url, f"Checkin failure. {'Invalid URL.', url}"
-			match = search(r"id=(\d+).*?([0-9A-F]{32})", url)
+			match = _search(r"id=(\d+).*?([0-9A-F]{32})", url)
 			return self.checkin_checkin_qrcode(activity = {
 				"active_id": match.group(1),
 				"enc": match.group(2)
 			}, location = location)
 		except Exception as e:
 			return False, {
 				"msg": str(e),
```

### Comparing `Xdcheckin-2.0.4/src/xdcheckin/core/locations.py` & `xdcheckin-2.0.5/src/xdcheckin/core/locations.py`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.4/src/xdcheckin/core/xidian.py` & `xdcheckin-2.0.5/src/xdcheckin/core/xidian.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # -*- coding: utf-8 -*-
 
-from base64 import b64encode
-from Crypto.Cipher.AES import new as AES_new, block_size as AES_block_size, MODE_CBC as AES_MODE_CBC
-from Crypto.Util.Padding import pad
-from re import search
-from requests import Response, Session
-from requests.exceptions import RequestException
-from threading import Thread
-from time import time
-from xdcheckin.core.chaoxing import Chaoxing
+from re import search as _search
+from requests import Response as _Response, Session as _Session
+from requests.exceptions import RequestException as _RequestException
+from threading import Thread as _Thread
+from time import time as _time
+from xdcheckin.core.chaoxing import Chaoxing as _Chaoxing
+from xdcheckin.util.encryption import encrypt_aes as _encrypt_aes
 
 class IDSSession:
 	requests_session = secrets = service = logined = None
 	config = {
 		"requests_headers": {
-			"User-Agent": "Mozilla/5.0 (Linux; Android 10; K) Apple"
-				      "WebKit/537.36 (KHTML, like Gecko) Chrome"
-				      "/120.0.0.0 Mobile Safari/537.36"
+			"User-Agent":
+				"Mozilla/5.0 (Linux; Android 10; K) AppleWebKit"
+				"/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 M"
+				"obile Safari/537.36"
 		}
 	}
 
 	def __init__(self, service: str = ""):
 		"""Initialize an IDS Session.
 		:param service: The SSO service for redirection.
 		"""
 		if self.logined:
 			return
-		self.requests_session, self.secrets, self.service = Session(), {}, service
+		self.requests_session = _Session()
+		self.secrets, self.service = {}, service
 
 	def get(
 		self, url: str = "", params: dict = {}, cookies: dict = None,
 		headers: dict = None, **kwargs
 	):
 		"""Wrapper for requests.get().
 		:param url: URL.
@@ -44,18 +44,18 @@
 			res = self.requests_session.get(
 				url = url, params = params, cookies = cookies,
 				headers = headers or self.config["requests_headers"],
 				**{"verify": False, **kwargs}
 			)
 			assert res.status_code in (200, 500), res.status_code
 		except AssertionError as e:
-			res = Response()
+			res = _Response()
 			res.status_code, res._content = int(str(e)), b"{}"
-		except RequestException:
-			res = Response()
+		except _RequestException:
+			res = _Response()
 			res.status_code, res._content = 404, b"{}"
 		finally:
 			return res
 
 	def post(
 		self, url: str = "", data: dict = {}, cookies: dict = None,
 		headers: dict = None, **kwargs
@@ -72,25 +72,26 @@
 			res = self.requests_session.post(
 				url = url, data = data, cookies = cookies,
 				headers = headers or self.config["requests_headers"],
 				**{"verify": False, **kwargs}
 			)
 			assert res.status_code in (200, 500), res.status_code
 		except AssertionError as e:
-			res = Response()
+			res = _Response()
 			res.status_code, res._content = int(str(e)), b"{}"
-		except RequestException:
-			res = Response()
+		except _RequestException:
+			res = _Response()
 			res.status_code, res._content = 404, b"{}"
 		finally:
 			return res
 
 	def login_username_prepare(self):
 		"""Prepare verification for username login.
-		:return: Base64 encoded captcha background and slider image string.
+		:return: Base64 encoded captcha background and 
+		slider image string.
 		"""
 		url1 = "https://ids.xidian.edu.cn/authserver/login"
 		params1 = {
 			"service": self.service
 		}
 		url2 = "https://ids.xidian.edu.cn/authserver/common/openSliderCaptcha.htl"
 		params2 = {
@@ -99,16 +100,20 @@
 		ret = {
 			"big_img_src": "",
 			"small_img_src": ""
 		}
 		res1 = self.get(url = url1, params = params1)
 		if not res1.status_code == 200:
 			return ret
-		s = search(r"\"pwdEncryptSalt\" value=\"(.*?)\".*?\"execution\" value=\"(.*?)\"", res1.text)
-		params2["_"] = str(int(1000 * time()))
+		s = _search(
+			r"\"pwdEncryptSalt\" value=\"(.*?)\".*?"
+			r"\"execution\" value=\"(.*?)\"",
+			res1.text
+		)
+		params2["_"] = str(int(1000 * _time()))
 		res2 = self.get(url = url2, params = params2)
 		if not res2.status_code == 200:
 			return ret
 		ret.update({
 			"big_img_src": res2.json()["bigImage"],
 			"small_img_src": res2.json()["smallImage"]
 		})
@@ -119,26 +124,18 @@
 		return ret
 
 	def login_username_finish(
 		self,
 		account: dict = {"username": "", "password": "", "vcode": ""}
 	):
 		"""Verify and finish username logging in.
-		:param account: Username, password and verification code (a.k.a. slider offset).
+		:param account: Username, password and verification 
+		code (a.k.a. slider offset).
 		:return: Cookies and login state.
 		"""
-		def _encrypt_aes(msg: str = "", key: str = ""):
-			enc = AES_new(
-				key.encode("utf-8"), AES_MODE_CBC,
-				b"xidianscriptsxdu"
-			).encrypt(pad(
-				4 * b"xidianscriptsxdu" + msg.encode("utf-8"),
-				AES_block_size
-			))
-			return b64encode(enc).decode("utf-8")
 		url1 = "https://ids.xidian.edu.cn/authserver/common/verifySliderCaptcha.htl"
 		data1 = {
 			"canvasLength": 280,
 			"moveLength": account["vcode"]
 		}
 		ret = {
 			"cookies": None,
@@ -147,16 +144,18 @@
 		res1 = self.post(url1, data = data1)
 		if not res1.status_code == 200 and res1.json()["errorCode"] == 1:
 			return ret
 		url2 = "https://ids.xidian.edu.cn/authserver/login"
 		data2 = {
 			"username": account["username"],
 			"password": _encrypt_aes(
-				account["password"],
-				self.secrets["login_prepare_salt"]
+				msg = account["password"],
+				key = self.secrets["login_prepare_salt"].encode("utf-8"),
+				iv = b"xidianscriptsxdu",
+				padding = lambda msg: 4 * b"xidianscriptsxdu" + msg.encode("utf-8")
 			),
 			"captcha": "",
 			"_eventId": "submit",
 			"cllt": "userNameLogin",
 			"dllt": "generalLogin",
 			"lt": "",
 			"execution": self.secrets["login_prepare_execution"],
@@ -180,88 +179,104 @@
 		:return: Cookies and login state.
 		"""
 		url = "http://ids.xidian.edu.cn/authserver/index.do"
 		ret = {
 			"cookies": None,
 			"logined": False
 		}
-		res = self.get(url = url, cookies = account["cookies"], allow_redirects = False)
+		res = self.get(
+			url = url, cookies = account["cookies"],
+			allow_redirects = False
+		)
 		if res.status_code != 302:
 			ret.update({
 				"cookies": account["cookies"],
 				"logined": True
 			})
 		return ret
 
 class Newesxidian:
 	"""XDU exclusive APIs for classroom livestreams.
 	"""
 	chaoxing_session = logined = None
 
-	def __init__(self, chaoxing: Chaoxing = None):
+	def __init__(self, chaoxing: _Chaoxing = None):
 		if self.logined or not chaoxing.logined or not chaoxing.cookies.get("fid") == "16820":
 			return
 		self.logined, self.chaoxing_session = True, chaoxing
 
 	def livestream_get_url(self, livestream: dict = {"live_id": ""}):
 		"""Get livestream URL.
 		:param livesteam: Live ID in dictionary.
-		:return: Livestream URL, live ID, device ID and classroom location (placeholder). URL will fallback to replay URL for non-ongoing live IDs.
+		:return: Livestream URL, live ID, device ID and 
+		classroom location (placeholder).
+		URL will fallback to replay URL for non-ongoing live IDs.
 		"""
 		url = "https://newesxidian.chaoxing.com/live/getViewUrlHls"
 		params = {
 			"liveId": livestream["live_id"]
 		}
-		res = self.chaoxing_session.get(url = url, params = params, expire_after = 86400)
+		res = self.chaoxing_session.get(
+			url = url, params = params, expire_after = 86400
+		)
 		return {
 			"url": res.text,
 			"live_id": livestream["live_id"],
 			"device": "",
 			"location": ""
 		}
 
 	def livestream_get_live_url(
 		self, livestream: dict = {"live_id": "", "device": "", "location": ""}
 	):
 		"""Get livestream URL.
-		:param livestream: Live ID (unused if device ID is present), device ID, and location (in case device ID is not present) in dictionary.
-		:return: Livestream URL, live ID (placeholder if not given), device ID and classroom location (placeholder if device ID not given).
+		:param livestream: Live ID (unused if device ID is present), device ID
+		and location (in case device ID is not present) in dictionary.
+		:return: Livestream URL, live ID (placeholder if not given), device ID
+		and classroom location (placeholder if device ID not given).
 		"""
 		url1 = "http://newesxidian.chaoxing.com/live/listSignleCourse"
 		params1 = {
 			"liveId": livestream.get("live_id") or ""
 		}
 		url2 = "http://newesxidian.chaoxing.com/live/getViewUrlNoCourseLive"
 		params2 = {
 			"deviceCode": livestream.get("device") or "",
 			"status": 1
 		}
 		location = livestream.get("location") or ""
 		if not livestream.get("device"):
-			res1 = self.chaoxing_session.get(url = url1, params = params1, expire_after = 86400)
+			res1 = self.chaoxing_session.get(
+				url = url1, params = params1, expire_after = 86400
+			)
 			data = res1.json() or []
 			for lesson in data:
 				if str(lesson["id"]) == livestream["live_id"]:
 					params2["deviceCode"] = lesson["deviceCode"]
 					location = lesson["schoolRoomName"].rstrip()
 					break
-		res2 = self.chaoxing_session.get(url = url2, params = params2, expire_after = 86400)
+		res2 = self.chaoxing_session.get(
+			url = url2, params = params2, expire_after = 86400
+		)
 		return {
 			"url": res2.text,
 			"live_id": params1["liveId"],
 			"device": params2["deviceCode"],
 			"location": location
 		}
 
 	def curriculum_get_curriculum(self, week: str = ""):
 		"""Get curriculum with livestreams.
 		:param week: Week number. Defaulted to the current week.
 		:return: Chaoxing curriculum with livestreams for lessons.
 		"""
-		def _get_livestream_wrapper(class_id: str = "", live_id: str = "", location: str = ""):
+		def _get_livestream_wrapper(
+			class_id: str = "", live_id: str = "",
+			location: str = ""
+		):
 			if not curriculum["lessons"].get(class_id):
 				return
 			if not curriculum["lessons"][class_id].get("livestreams"):
 				curriculum["lessons"][class_id]["livestreams"] = []
 			livestream = self.livestream_get_live_url(livestream = {
 				"live_id": live_id,
 				"location": location
@@ -280,18 +295,20 @@
 		}
 		curriculum = self.chaoxing_session.curriculum_get_curriculum(week = week)
 		params.update({
 			"termYear": curriculum["details"]["year"],
 			"termId": curriculum["details"]["semester"],
 			"week": week or curriculum["details"]["week"]
 		})
-		res = self.chaoxing_session.get(url = url, params = params, expire_after = 86400)
+		res = self.chaoxing_session.get(
+			url = url, params = params, expire_after = 86400
+		)
 		data = res.json() or []
 		threads = [
-			Thread(target = _get_livestream_wrapper, kwargs = {
+			_Thread(target = _get_livestream_wrapper, kwargs = {
 				"class_id": str(lesson["teachClazzId"]),
 				"live_id": str(lesson["id"]),
 				"location": lesson["place"]
 			}) for lesson in data
 		]
 		for thread in threads:
 			thread.start()
```

### Comparing `Xdcheckin-2.0.4/src/xdcheckin/server/server.py` & `xdcheckin-2.0.5/src/xdcheckin/server/server.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,292 +1,300 @@
-from flask import Flask, render_template, make_response, request, session
-from flask_session import Session
-from importlib.metadata import version
-from io import BytesIO
-from json import loads, dumps
-from os import listdir, remove, makedirs
-from os.path import exists, join
-from PIL.Image import open
-from pyzbar.pyzbar import decode, ZBarSymbol
-from requests import get, post
-from tempfile import gettempdir
-from urllib3 import disable_warnings
+from flask import Flask as _Flask, render_template as _render_template, \
+	make_response as _make_response, request as _request, session as _session
+from flask_session import Session as _Session
+from importlib.metadata import version as _version
+from io import BytesIO as _BytesIO
+from json import loads as _loads, dumps as _dumps
+from PIL.Image import open as _open
+from pyzbar.pyzbar import decode as _decode, ZBarSymbol as _ZBarSymbol
+from requests import get as _get
 from uuid import uuid4
-from waitress import serve
-from xdcheckin.core.chaoxing import Chaoxing
-from xdcheckin.core.xidian import IDSSession, Newesxidian
-from xdcheckin.core.locations import locations
+from xdcheckin.core.chaoxing import Chaoxing as _Chaoxing
+from xdcheckin.core.xidian import IDSSession as _IDSSession, Newesxidian as _Newesxidian
+from xdcheckin.core.locations import locations as _locations
 
 def create_server(config: dict = {}):
 	"""Create a Xdcheckin server.
 	:param config: Server config.
 	:return: Xdcheckin server.
 	"""
-	server = Flask(__name__)
+	server = _Flask(__name__)
 	server.config.update(config)
-	Session(server)
+	_Session(server)
 
 	@server.route("/")
 	def index_html():
-		return render_template("index.html")
+		return _render_template("index.html")
 
 	@server.route("/static/g_locations.js")
 	def xdcheckin_static_g_locations_js():
-		res = make_response(f"var g_locations = {dumps(locations).encode('ascii').decode('unicode-escape')};")
+		locations_str = _dumps(_locations).encode('ascii').decode('unicode-escape')
+		res = _make_response(f"var g_locations = {locations_str};")
 		res.status_code = 200
 		return res
 
 	@server.route("/xdcheckin/get/version", methods = ["POST"])
 	def xdcheckin_get_version():
-		res = make_response(version("Xdcheckin"))
+		res = _make_response(_version("Xdcheckin"))
 		res.status_code = 200
 		return res
 
 	@server.route("/xdcheckin/get/releases/latest", methods = ["POST"])
 	def xdcheckin_get_latest_release():
 		try:
-			res = get(url = "https://api.github.com/repos/Pairman/Xdcheckin/releases/latest")
+			res = _get(url = "https://api.github.com/repos/Pairman/Xdcheckin/releases/latest")
 			assert res.status_code == 200
 			data = res.json()
-			res = make_response(dumps({
+			res = _make_response(_dumps({
 				"tag_name": data["tag_name"],
 				"name": data["name"],
 				"author": data["author"]["login"],
 				"body": data["body"],
 				"published_at": data["published_at"],
 				"html_url": data["html_url"],
 				"assets": [{
 						"name": asset["name"],
 						"size": asset["size"],
-						"browser_download_url": asset["browser_download_url"]
+						"browser_download_url":
+							asset["browser_download_url"]
 					} for asset in data["assets"]]
 			}))
 			res.status_code = 200
 		except Exception:
-			res = make_response("")
+			res = _make_response("")
 			res.status_code = 500
 		finally:
 			return res
 
 	@server.route("/ids/login_prepare", methods = ["POST"])
 	def ids_login_prepare():
 		try:
-			ids = IDSSession(service = "https://learning.xidian.edu.cn/cassso/xidian")
-			if not session.get("xdcheckin_uuid"):
-				session["xdcheckin_uuid"] = str(uuid4())
-			if not server.config["XDCHECKIN_SESSION"].get(session["xdcheckin_uuid"]):
-				server.config["XDCHECKIN_SESSION"][session["xdcheckin_uuid"]] = {}
-			server.config["XDCHECKIN_SESSION"][session["xdcheckin_uuid"]]["ids"] =ids
-			res = make_response(dumps(ids.login_username_prepare()))
+			ids = _IDSSession(service = "https://learning.xidian.edu.cn/cassso/xidian")
+			if not _session.get("xdcheckin_uuid"):
+				_session["xdcheckin_uuid"] = str(uuid4())
+			if not server.config["XDCHECKIN_SESSION"].get(_session["xdcheckin_uuid"]):
+				server.config["XDCHECKIN_SESSION"][_session["xdcheckin_uuid"]] = {}
+			server.config["XDCHECKIN_SESSION"][_session["xdcheckin_uuid"]]["ids"] = ids
+			res = _make_response(_dumps(ids.login_username_prepare()))
 		except Exception as e:
-			res = make_response(dumps({"err": str(e)}))
+			res = _make_response(_dumps({"err": str(e)}))
 		finally:
 			res.status_code = 200
 			return res
 
 	@server.route("/ids/login_finish", methods = ["POST"])
 	def ids_login_finish():
 		try:
-			data = request.get_json(force = True)
+			data = _request.get_json(force = True)
 			username, password, vcode = data["username"], data["password"], data["vcode"]
 			assert username and password and vcode, "Missing username, password or verification code."
-			ids = server.config["XDCHECKIN_SESSION"][session["xdcheckin_uuid"]]["ids"]
-			finish = ids.login_username_finish(account = {"username": username, "password": password, "vcode": vcode})
+			ids = server.config["XDCHECKIN_SESSION"][_session["xdcheckin_uuid"]]["ids"]
+			finish = ids.login_username_finish(account = {
+				"username": username,
+				"password": password,
+				"vcode": vcode
+			})
 			assert finish["logined"], "IDS login failed."
 			for domain in finish["cookies"].list_domains():
 				if domain != ".chaoxing.com":
 					finish["cookies"].clear(domain = domain)
-			data = chaoxing_login({"username": "", "password": "", "cookies": dumps(dict(finish["cookies"]))})
-			res = make_response(dumps(data))
+			data = chaoxing_login(account = {
+				"username": "",
+				"password": "",
+				"cookies": _dumps(dict(finish["cookies"]))
+			})
+			res = _make_response(_dumps(data))
 		except Exception as e:
-			res = make_response(dumps({"err": str(e)}))
+			res = _make_response(_dumps({"err": str(e)}))
 		finally:
 			res.status_code = 200
 			return res
 
 	@server.route("/chaoxing/login", methods = ["POST"])
 	def chaoxing_login(account: dict = {}):
 		try:
-			data = account or request.get_json(force = True)
+			data = account or _request.get_json(force = True)
 			username, password, cookies = data["username"], data["password"], data["cookies"]
 			assert (username and password) or cookies, "Missing username, password or cookies."
-			chaoxing = Chaoxing(username = username, password = password, cookies = loads(cookies) if cookies else None, config = {
-				"chaoxing_course_get_activities_courses_limit": 36,
-				"chaoxing_checkin_location_address_override_maxlen": 13
-			})
+			chaoxing = _Chaoxing(
+				username = username, password = password,
+				cookies = _loads(cookies) if cookies else None,
+				config = {
+					"chaoxing_course_get_activities_courses_limit": 36,
+					"chaoxing_checkin_location_address_override_maxlen": 13
+				}
+			)
 			assert chaoxing.logined, "Chaoxing login failed."
-			newesxidian = Newesxidian(chaoxing = chaoxing)
-			if not session.get("xdcheckin_uuid"):
-				session["xdcheckin_uuid"] = str(uuid4())
-			if not server.config["XDCHECKIN_SESSION"].get(session["xdcheckin_uuid"]):
-				server.config["XDCHECKIN_SESSION"][session["xdcheckin_uuid"]] = {}
-			server.config["XDCHECKIN_SESSION"][session["xdcheckin_uuid"]].update({
+			newesxidian = _Newesxidian(chaoxing = chaoxing)
+			if not _session.get("xdcheckin_uuid"):
+				_session["xdcheckin_uuid"] = str(uuid4())
+			if not server.config["XDCHECKIN_SESSION"].get(_session["xdcheckin_uuid"]):
+				server.config["XDCHECKIN_SESSION"][_session["xdcheckin_uuid"]] = {}
+			server.config["XDCHECKIN_SESSION"][_session["xdcheckin_uuid"]].update({
 				"chaoxing": chaoxing,
 				"newesxidian": newesxidian
 			})
 			ret = {
 				"fid": chaoxing.cookies.get("fid") or "0",
 				"courses": chaoxing.courses,
-				"cookies": dumps(dict(chaoxing.cookies))
+				"cookies": _dumps(dict(chaoxing.cookies))
 			}
 		except Exception as e:
 			ret = {"err": str(e)}
 		finally:
 			if account:
 				return ret
-			res = make_response(dumps(ret))
+			res = _make_response(_dumps(ret))
 			res.status_code = 200
 			return res
 
 	@server.route("/chaoxing/extract_url", methods = ["POST"])
 	def chaoxing_extract_url():
 		try:
-			chaoxing = server.config["XDCHECKIN_SESSION"][session["xdcheckin_uuid"]]["chaoxing"]
-			newesxidian = server.config["XDCHECKIN_SESSION"][session["xdcheckin_uuid"]]["newesxidian"]
+			chaoxing = server.config["XDCHECKIN_SESSION"][_session["xdcheckin_uuid"]]["chaoxing"]
+			newesxidian = server.config["XDCHECKIN_SESSION"][_session["xdcheckin_uuid"]]["newesxidian"]
 			assert chaoxing.logined
-			data = request.get_json(force = True)
-			livestream = newesxidian.livestream_get_live_url(livestream = {"live_id": str(data)})
-			res = make_response(livestream["url"])
+			data = _request.get_json(force = True)
+			livestream = newesxidian.livestream_get_live_url(
+				livestream = {"live_id": str(data)}
+			)
+			res = _make_response(livestream["url"])
 			res.status_code = 200
 		except Exception:
-			res = make_response("")
+			res = _make_response("")
 			res.status_code = 500
 		finally:
 			return res
 
 	@server.route("/chaoxing/get_curriculum", methods = ["POST"])
 	def chaoxing_get_curriculum():
 		try:
-			chaoxing = server.config["XDCHECKIN_SESSION"][session["xdcheckin_uuid"]]["chaoxing"]
-			newesxidian = server.config["XDCHECKIN_SESSION"][session["xdcheckin_uuid"]]["newesxidian"]
+			chaoxing = server.config["XDCHECKIN_SESSION"][_session["xdcheckin_uuid"]]["chaoxing"]
+			newesxidian = server.config["XDCHECKIN_SESSION"][_session["xdcheckin_uuid"]]["newesxidian"]
 			assert chaoxing.logined
-			data = request.get_json(force = True)
+			data = _request.get_json(force = True)
 			curriculum = newesxidian.curriculum_get_curriculum() if data and newesxidian.logined else chaoxing.curriculum_get_curriculum()
-			res = make_response(dumps(curriculum))
+			res = _make_response(_dumps(curriculum))
 			res.status_code = 200
 		except Exception as e:
-			res = make_response("{}")
+			res = _make_response("{}")
 			res.status_code = 500
 		finally:
 			return res
 
 	@server.route("/chaoxing/get_activities", methods = ["POST"])
 	def chaoxing_get_activities():
 		try:
-			chaoxing = server.config["XDCHECKIN_SESSION"][session["xdcheckin_uuid"]]["chaoxing"]
+			chaoxing = server.config["XDCHECKIN_SESSION"][_session["xdcheckin_uuid"]]["chaoxing"]
 			assert chaoxing.logined
 			activities = chaoxing.course_get_activities()
-			res = make_response(dumps(activities))
+			res = _make_response(_dumps(activities))
 			res.status_code = 200
 		except Exception:
-			res = make_response("{}")
+			res = _make_response("{}")
 			res.status_code = 500
 		finally:
 			return res
 
 	@server.route("/chaoxing/checkin_get_captcha", methods = ["POST"])
 	def chaoxing_checkin_get_captcha():
 		try:
-			chaoxing = server.config["XDCHECKIN_SESSION"][session["xdcheckin_uuid"]]["chaoxing"]
+			chaoxing = server.config["XDCHECKIN_SESSION"][_session["xdcheckin_uuid"]]["chaoxing"]
 			assert chaoxing.logined
-			data = request.get_json(force = True)
+			data = _request.get_json(force = True)
 			assert data["captcha"]
 			captcha = chaoxing.checkin_get_captcha(captcha = data["captcha"])
-			res = make_response(dumps(captcha))
+			res = _make_response(_dumps(captcha))
 			res.status_code = 200
 		except Exception:
-			res = make_response("{}")
+			res = _make_response("{}")
 			res.status_code = 500
 		finally:
 			return res
 
 	@server.route("/chaoxing/checkin_submit_captcha", methods = ["POST"])
 	def chaoxing_checkin_submit_captcha():
 		try:
-			chaoxing = server.config["XDCHECKIN_SESSION"][session["xdcheckin_uuid"]]["chaoxing"]
+			chaoxing = server.config["XDCHECKIN_SESSION"][_session["xdcheckin_uuid"]]["chaoxing"]
 			assert chaoxing.logined
-			data = request.get_json(force = True)
+			data = _request.get_json(force = True)
 			assert data["captcha"]
 			result = chaoxing.checkin_submit_captcha(captcha = data["captcha"])
 			assert result[0]
-			res = make_response(dumps(result[1]))
+			res = _make_response(_dumps(result[1]))
 			res.status_code = 200
 		except Exception as e:
-			res = make_response("{}")
+			res = _make_response("{}")
 			res.status_code = 500
 		finally:
 			return res
 
 	@server.route("/chaoxing/checkin_do_sign", methods = ["POST"])
 	def chaoxing_checkin_do_sign():
 		try:
-			chaoxing = server.config["XDCHECKIN_SESSION"][session["xdcheckin_uuid"]]["chaoxing"]
+			chaoxing = server.config["XDCHECKIN_SESSION"][_session["xdcheckin_uuid"]]["chaoxing"]
 			assert chaoxing.logined, "Not logged in."
-			data = request.get_json(force = True)
+			data = _request.get_json(force = True)
 			assert data["params"], "No parameters given"
 			result = chaoxing.checkin_do_sign(old_params = data["params"])
-			res = make_response(dumps({
-				"msg": f"{result[1]['msg'][: -1]}, {data['params']['activeId']})",
-				"params": result[1]["params"]
-			}))
+			res = _make_response(_dumps(result[1]))
 		except Exception as e:
-			res = make_response(dumps({
+			res = _make_response(_dumps({
 				"msg": f"Checkin error. ({str(e)})",
 				"params": {}
 			}))
 		finally:
 			res.status_code = 200
 			return res
 						
 
 	@server.route("/chaoxing/checkin_checkin_location", methods = ["POST"])
 	def chaoxing_checkin_checkin_location():
 		try:
-			chaoxing = server.config["XDCHECKIN_SESSION"][session["xdcheckin_uuid"]]["chaoxing"]
+			chaoxing = server.config["XDCHECKIN_SESSION"][_session["xdcheckin_uuid"]]["chaoxing"]
 			assert chaoxing.logined, "Not logged in."
-			data = request.get_json(force = True)
+			data = _request.get_json(force = True)
 			assert data["activity"]["active_id"], "No activity ID given."
 			data["activity"]["active_id"] = str(data["activity"]["active_id"])
-			result = chaoxing.checkin_checkin_location(activity = data["activity"], location = data["location"])
-			res = make_response(dumps({
-				"msg": f"{result[1]['msg'][: -1]}, {data['activity']['active_id']})",
-				"params": result[1]["params"],
-				"captcha": result[1]["captcha"]
-			}))
+			result = chaoxing.checkin_checkin_location(
+				activity = data["activity"], location = data["location"]
+			)
+			res = _make_response(_dumps(result[1]))
 		except Exception as e:
-			res = make_response(dumps({
+			res = _make_response(_dumps({
 				"msg": f"Checkin error. ({str(e)})",
 				"params": {},
 				"captcha": {}
 			}))
 		finally:
 			res.status_code = 200
 			return res
 
 	@server.route("/chaoxing/checkin_checkin_qrcode_img", methods = ["POST"])
 	def chaoxing_checkin_checkin_qrcode_img():
 		try:
-			chaoxing = server.config["XDCHECKIN_SESSION"][session["xdcheckin_uuid"]]["chaoxing"]
+			chaoxing = server.config["XDCHECKIN_SESSION"][_session["xdcheckin_uuid"]]["chaoxing"]
 			assert chaoxing.logined, "Not logged in."
-			img_src = request.files["img_src"]
+			img_src = _request.files["img_src"]
 			assert img_src, "No image given."
-			with open(BytesIO(img_src.read())) as img:
+			with _open(_BytesIO(img_src.read())) as img:
 				assert img.height and img.width, "Empty image."
-				urls = decode(img, symbols = [ZBarSymbol.QRCODE])
+				urls = _decode(img, symbols = [_ZBarSymbol.QRCODE])
 			assert urls, "No Qrcode detected."
-			urls = [s.data.decode("utf-8") for s in urls if b"mobilelearn.chaoxing.com/widget/sign/e" in s.data]
+			urls = [
+				s.data.decode("utf-8") for s in urls
+				if b"mobilelearn.chaoxing.com/widget/sign/e" in s.data
+			]
 			assert urls, "No checkin URL found."
-			result = chaoxing.checkin_checkin_qrcode_url(url = urls[0], location = loads(request.form["location"]))
-			res = make_response(dumps({
-				"msg": f"{result[1]['msg'][: -1]}, {urls[0]})",
-				"params": result[1]["params"],
-				"captcha": result[1]["captcha"]
-			}))
+			result = chaoxing.checkin_checkin_qrcode_url(
+				url = urls[0], location = _loads(_request.form["location"])
+			)
+			res = _make_response(_dumps(result[1]))
 		except Exception as e:
-			res = make_response(dumps({
+			res = _make_response(_dumps({
 				"msg": f"Checkin error. ({str(e)})",
 				"params": {},
 				"captcha": {}
 			}))
 		finally:
 			res.status_code = 200
 			return res
@@ -294,14 +302,19 @@
 	return server
 
 def start_server(host: str = "127.0.0.1", port: int = 5001):
 	"""Run a Xdcheckin server.
 	:param host: IP address.
 	:param port: Port.
 	"""
+	from os import listdir, remove, makedirs
+	from os.path import exists, join
+	from tempfile import gettempdir
+	from urllib3 import disable_warnings
+	from waitress import serve
 	config = {
 		"SESSION_PERMANENT": False,
 		"SESSION_TYPE": "filesystem",
 		"SESSION_FILE_DIR": join(gettempdir(), "xdcheckin"),
 		"XDCHECKIN_SESSION": {}
 	}
 	if not exists(config["SESSION_FILE_DIR"]):
@@ -312,15 +325,15 @@
 	disable_warnings()
 	serve(app = create_server(config = config), host = host, port = port)
 
 def main():
 	from sys import argv
 
 	if not len(argv) in (1, 3):
-		print(f"xdcheckin-server - Xdcheckin Server Commandline Tool {version('Xdcheckin')}")
+		print(f"xdcheckin-server - Xdcheckin Server Commandline Tool {_version('Xdcheckin')}")
 		print(f"Usage: {argv[0]} <ip> <port>")
 		print(f"  or:  {argv[0]}")
 		return 1
 	ip, port = "0.0.0.0", 5001
 	if len(argv) == 3:
 		from socket import inet_aton
 		try:
```

### Comparing `Xdcheckin-2.0.4/src/xdcheckin/server/static/activity.js` & `xdcheckin-2.0.5/src/xdcheckin/server/static/activity.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.4/src/xdcheckin/server/static/classroom.js` & `xdcheckin-2.0.5/src/xdcheckin/server/static/classroom.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.4/src/xdcheckin/server/static/curriculum.js` & `xdcheckin-2.0.5/src/xdcheckin/server/static/curriculum.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.4/src/xdcheckin/server/static/g_classroom_urls.js` & `xdcheckin-2.0.5/src/xdcheckin/server/static/g_classroom_urls.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.4/src/xdcheckin/server/static/location.js` & `xdcheckin-2.0.5/src/xdcheckin/server/static/location.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.4/src/xdcheckin/server/static/login.js` & `xdcheckin-2.0.5/src/xdcheckin/server/static/login.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.4/src/xdcheckin/server/static/misc.js` & `xdcheckin-2.0.5/src/xdcheckin/server/static/misc.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.4/src/xdcheckin/server/static/player.js` & `xdcheckin-2.0.5/src/xdcheckin/server/static/player.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.4/src/xdcheckin/server/static/style.css` & `xdcheckin-2.0.5/src/xdcheckin/server/static/style.css`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.4/src/xdcheckin/server/static/util.js` & `xdcheckin-2.0.5/src/xdcheckin/server/static/util.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.4/src/xdcheckin/server/templates/index.html` & `xdcheckin-2.0.5/src/xdcheckin/server/templates/index.html`

 * *Files identical despite different names*

