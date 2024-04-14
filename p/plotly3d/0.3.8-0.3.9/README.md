# Comparing `tmp/plotly3d-0.3.8.tar.gz` & `tmp/plotly3d-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotly3d-0.3.8.tar", last modified: Sat Apr  6 19:12:16 2024, max compression
+gzip compressed data, was "plotly3d-0.3.9.tar", last modified: Sat Apr  6 19:14:21 2024, max compression
```

## Comparing `plotly3d-0.3.8.tar` & `plotly3d-0.3.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-06 19:12:16.861240 plotly3d-0.3.8/
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     1058 2024-03-31 02:54:34.000000 plotly3d-0.3.8/LICENSE
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      310 2024-04-06 19:12:16.860337 plotly3d-0.3.8/PKG-INFO
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      100 2024-04-01 03:31:03.000000 plotly3d-0.3.8/README.md
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-06 19:12:16.855703 plotly3d-0.3.8/plotly3d/
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-02 02:59:03.000000 plotly3d-0.3.8/plotly3d/__init__.py
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     9576 2024-04-06 19:11:13.000000 plotly3d-0.3.8/plotly3d/plot.py
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-06 19:12:16.859675 plotly3d-0.3.8/plotly3d.egg-info/
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      310 2024-04-06 19:12:16.856371 plotly3d-0.3.8/plotly3d.egg-info/PKG-INFO
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      223 2024-04-06 19:12:16.857162 plotly3d-0.3.8/plotly3d.egg-info/SOURCES.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        1 2024-04-06 19:12:16.858547 plotly3d-0.3.8/plotly3d.egg-info/dependency_links.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       33 2024-04-06 19:12:16.859152 plotly3d-0.3.8/plotly3d.egg-info/requires.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        9 2024-04-06 19:12:16.859742 plotly3d-0.3.8/plotly3d.egg-info/top_level.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       38 2024-04-06 19:12:16.866969 plotly3d-0.3.8/setup.cfg
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      404 2024-04-06 19:11:40.000000 plotly3d-0.3.8/setup.py
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-06 19:14:20.994696 plotly3d-0.3.9/
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     1058 2024-03-31 02:54:34.000000 plotly3d-0.3.9/LICENSE
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      336 2024-04-06 19:14:20.993932 plotly3d-0.3.9/PKG-INFO
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      100 2024-04-01 03:31:03.000000 plotly3d-0.3.9/README.md
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-06 19:14:20.983416 plotly3d-0.3.9/plotly3d/
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-02 02:59:03.000000 plotly3d-0.3.9/plotly3d/__init__.py
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     9576 2024-04-06 19:11:13.000000 plotly3d-0.3.9/plotly3d/plot.py
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-06 19:14:20.992750 plotly3d-0.3.9/plotly3d.egg-info/
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      336 2024-04-06 19:14:20.989695 plotly3d-0.3.9/plotly3d.egg-info/PKG-INFO
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      223 2024-04-06 19:14:20.990313 plotly3d-0.3.9/plotly3d.egg-info/SOURCES.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        1 2024-04-06 19:14:20.991122 plotly3d-0.3.9/plotly3d.egg-info/dependency_links.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       44 2024-04-06 19:14:20.992201 plotly3d-0.3.9/plotly3d.egg-info/requires.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        9 2024-04-06 19:14:20.992806 plotly3d-0.3.9/plotly3d.egg-info/top_level.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       38 2024-04-06 19:14:20.995249 plotly3d-0.3.9/setup.cfg
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      425 2024-04-06 19:14:08.000000 plotly3d-0.3.9/setup.py
```

### Comparing `plotly3d-0.3.8/LICENSE` & `plotly3d-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `plotly3d-0.3.8/plotly3d/plot.py` & `plotly3d-0.3.9/plotly3d/plot.py`

 * *Files identical despite different names*

