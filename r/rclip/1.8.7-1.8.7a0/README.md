# Comparing `tmp/rclip-1.8.7.tar.gz` & `tmp/rclip-1.8.7a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rclip-1.8.7.tar", max compression
+gzip compressed data, was "rclip-1.8.7a0.tar", max compression
```

## Comparing `rclip-1.8.7.tar` & `rclip-1.8.7a0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1074 2024-04-13 20:14:27.326684 rclip-1.8.7/LICENSE
--rw-r--r--   0        0        0     7269 2024-04-13 20:14:27.326684 rclip-1.8.7/README.md
--rw-r--r--   0        0        0     1747 2024-04-13 20:14:27.326684 rclip-1.8.7/pyproject.toml
--rw-r--r--   0        0        0      158 2024-04-13 20:14:27.326684 rclip-1.8.7/rclip/const.py
--rw-r--r--   0        0        0     3830 2024-04-13 20:14:27.326684 rclip-1.8.7/rclip/db.py
--rw-r--r--   0        0        0      993 2024-04-13 20:14:27.326684 rclip-1.8.7/rclip/fs.py
--rw-r--r--   0        0        0     7002 2024-04-13 20:14:27.326684 rclip-1.8.7/rclip/main.py
--rw-r--r--   0        0        0     5412 2024-04-13 20:14:27.326684 rclip-1.8.7/rclip/model.py
--rw-r--r--   0        0        0     7230 2024-04-13 20:14:27.326684 rclip-1.8.7/rclip/utils/helpers.py
--rw-r--r--   0        0        0     1169 2024-04-13 20:14:27.326684 rclip-1.8.7/rclip/utils/preview.py
--rw-r--r--   0        0        0     1726 2024-04-13 20:14:27.326684 rclip-1.8.7/rclip/utils/snap.py
--rw-r--r--   0        0        0     8911 1970-01-01 00:00:00.000000 rclip-1.8.7/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-13 19:01:59.074395 rclip-1.8.7a0/LICENSE
+-rw-r--r--   0        0        0     7269 2024-04-13 19:01:59.074395 rclip-1.8.7a0/README.md
+-rw-r--r--   0        0        0     1749 2024-04-13 19:01:59.074395 rclip-1.8.7a0/pyproject.toml
+-rw-r--r--   0        0        0      158 2024-04-13 19:01:59.074395 rclip-1.8.7a0/rclip/const.py
+-rw-r--r--   0        0        0     3830 2024-04-13 19:01:59.074395 rclip-1.8.7a0/rclip/db.py
+-rw-r--r--   0        0        0      993 2024-04-13 19:01:59.074395 rclip-1.8.7a0/rclip/fs.py
+-rw-r--r--   0        0        0     7002 2024-04-13 19:01:59.074395 rclip-1.8.7a0/rclip/main.py
+-rw-r--r--   0        0        0     5412 2024-04-13 19:01:59.074395 rclip-1.8.7a0/rclip/model.py
+-rw-r--r--   0        0        0     7230 2024-04-13 19:01:59.074395 rclip-1.8.7a0/rclip/utils/helpers.py
+-rw-r--r--   0        0        0     1169 2024-04-13 19:01:59.074395 rclip-1.8.7a0/rclip/utils/preview.py
+-rw-r--r--   0        0        0     1726 2024-04-13 19:01:59.074395 rclip-1.8.7a0/rclip/utils/snap.py
+-rw-r--r--   0        0        0     8913 1970-01-01 00:00:00.000000 rclip-1.8.7a0/PKG-INFO
```

### Comparing `rclip-1.8.7/LICENSE` & `rclip-1.8.7a0/LICENSE`

 * *Files identical despite different names*

### Comparing `rclip-1.8.7/README.md` & `rclip-1.8.7a0/README.md`

 * *Files identical despite different names*

### Comparing `rclip-1.8.7/pyproject.toml` & `rclip-1.8.7a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rclip"
-version = "1.8.7"
+version = "1.8.7a0"
 description = "AI-Powered Command-Line Photo Search Tool"
 authors = ["Yurij Mikhalevich <yurij@mikhalevi.ch>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/yurijmikhalevich/rclip"
 keywords = ["image search", "computer vision", "photography"]
 classifiers = [
```

### Comparing `rclip-1.8.7/rclip/db.py` & `rclip-1.8.7a0/rclip/db.py`

 * *Files identical despite different names*

### Comparing `rclip-1.8.7/rclip/fs.py` & `rclip-1.8.7a0/rclip/fs.py`

 * *Files identical despite different names*

### Comparing `rclip-1.8.7/rclip/main.py` & `rclip-1.8.7a0/rclip/main.py`

 * *Files identical despite different names*

### Comparing `rclip-1.8.7/rclip/model.py` & `rclip-1.8.7a0/rclip/model.py`

 * *Files identical despite different names*

### Comparing `rclip-1.8.7/rclip/utils/helpers.py` & `rclip-1.8.7a0/rclip/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `rclip-1.8.7/rclip/utils/preview.py` & `rclip-1.8.7a0/rclip/utils/preview.py`

 * *Files identical despite different names*

### Comparing `rclip-1.8.7/rclip/utils/snap.py` & `rclip-1.8.7a0/rclip/utils/snap.py`

 * *Files identical despite different names*

### Comparing `rclip-1.8.7/PKG-INFO` & `rclip-1.8.7a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rclip
-Version: 1.8.7
+Version: 1.8.7a0
 Summary: AI-Powered Command-Line Photo Search Tool
 Home-page: https://github.com/yurijmikhalevich/rclip
 License: MIT
 Keywords: image search,computer vision,photography
 Author: Yurij Mikhalevich
 Author-email: yurij@mikhalevi.ch
 Requires-Python: >=3.9,<3.13
```

