# Comparing `tmp/fplab-0.0.2.2.tar.gz` & `tmp/fplab-0.0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fplab-0.0.2.2.tar", last modified: Sun Apr  7 10:05:57 2024, max compression
+gzip compressed data, was "fplab-0.0.2.3.tar", last modified: Sun Apr 14 15:01:36 2024, max compression
```

## Comparing `fplab-0.0.2.2.tar` & `fplab-0.0.2.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 10:05:57.018202 fplab-0.0.2.2/
--rw-rw-rw-   0        0        0     1090 2024-03-31 02:38:30.000000 fplab-0.0.2.2/LICENSE.txt
--rw-rw-rw-   0        0        0      523 2024-04-07 10:05:57.018202 fplab-0.0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      862 2024-04-06 15:56:56.000000 fplab-0.0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 10:05:56.986450 fplab-0.0.2.2/fplab/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.2/fplab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 10:05:57.002562 fplab-0.0.2.2/fplab/enhancement/
--rw-rw-rw-   0        0        0        0 2024-03-31 08:36:57.000000 fplab-0.0.2.2/fplab/enhancement/__init__.py
--rw-rw-rw-   0        0        0     4472 2024-03-31 08:36:57.000000 fplab-0.0.2.2/fplab/enhancement/frequency.py
--rw-rw-rw-   0        0        0     4454 2024-03-31 13:48:46.000000 fplab-0.0.2.2/fplab/enhancement/spatial.py
-drwxrwxrwx   0        0        0        0 2024-04-07 10:05:57.002562 fplab-0.0.2.2/fplab/generation/
--rw-rw-rw-   0        0        0        0 2024-04-02 15:51:38.000000 fplab-0.0.2.2/fplab/generation/__init__.py
--rw-rw-rw-   0        0        0     6948 2024-04-06 06:07:55.000000 fplab-0.0.2.2/fplab/generation/tps.py
-drwxrwxrwx   0        0        0        0 2024-04-07 10:05:57.002562 fplab-0.0.2.2/fplab/intrinsic/
--rw-rw-rw-   0        0        0        0 2024-03-23 06:49:44.000000 fplab-0.0.2.2/fplab/intrinsic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 10:05:57.002562 fplab-0.0.2.2/fplab/intrinsic/frequency/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.2/fplab/intrinsic/frequency/__init__.py
--rw-rw-rw-   0        0        0     7577 2024-03-31 08:36:57.000000 fplab-0.0.2.2/fplab/intrinsic/frequency/projection.py
--rw-rw-rw-   0        0        0    10795 2024-03-31 08:36:57.000000 fplab-0.0.2.2/fplab/intrinsic/frequency/tools.py
--rw-rw-rw-   0        0        0     3116 2024-04-07 04:59:12.000000 fplab-0.0.2.2/fplab/intrinsic/frequency/transform.py
-drwxrwxrwx   0        0        0        0 2024-04-07 10:05:57.002562 fplab-0.0.2.2/fplab/intrinsic/mask/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.2/fplab/intrinsic/mask/__init__.py
--rw-rw-rw-   0        0        0      855 2024-04-06 15:25:34.000000 fplab-0.0.2.2/fplab/intrinsic/mask/mask.py
-drwxrwxrwx   0        0        0        0 2024-04-07 10:05:57.002562 fplab-0.0.2.2/fplab/intrinsic/multiple/
--rw-rw-rw-   0        0        0        0 2024-03-23 07:06:33.000000 fplab-0.0.2.2/fplab/intrinsic/multiple/__init__.py
--rw-rw-rw-   0        0        0     6990 2024-04-07 05:24:47.000000 fplab-0.0.2.2/fplab/intrinsic/multiple/transform.py
-drwxrwxrwx   0        0        0        0 2024-04-07 10:05:57.002562 fplab-0.0.2.2/fplab/intrinsic/orientation/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.2/fplab/intrinsic/orientation/__init__.py
--rw-rw-rw-   0        0        0     6640 2024-04-06 09:18:53.000000 fplab-0.0.2.2/fplab/intrinsic/orientation/gradient.py
--rw-rw-rw-   0        0        0     6215 2024-04-07 04:39:10.000000 fplab-0.0.2.2/fplab/intrinsic/orientation/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-07 10:05:57.002562 fplab-0.0.2.2/fplab/intrinsic/skeleton/
--rw-rw-rw-   0        0        0        0 2024-04-06 15:22:02.000000 fplab-0.0.2.2/fplab/intrinsic/skeleton/__init__.py
--rw-rw-rw-   0        0        0     1752 2024-04-06 16:14:50.000000 fplab-0.0.2.2/fplab/intrinsic/skeleton/skeleton.py
-drwxrwxrwx   0        0        0        0 2024-04-07 10:05:57.002562 fplab-0.0.2.2/fplab/matching/
--rw-rw-rw-   0        0        0        0 2024-03-29 01:34:29.000000 fplab-0.0.2.2/fplab/matching/__init__.py
--rw-rw-rw-   0        0        0     6956 2024-03-30 03:40:09.000000 fplab-0.0.2.2/fplab/matching/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-07 10:05:57.018202 fplab-0.0.2.2/fplab/minutiae/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.2/fplab/minutiae/__init__.py
--rw-rw-rw-   0        0        0     6198 2024-04-07 07:52:40.000000 fplab-0.0.2.2/fplab/minutiae/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-07 10:05:57.018202 fplab-0.0.2.2/fplab/tools/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.2/fplab/tools/__init__.py
--rw-rw-rw-   0        0        0    13732 2024-04-06 14:10:17.000000 fplab-0.0.2.2/fplab/tools/array.py
--rw-rw-rw-   0        0        0     5367 2024-04-06 14:01:28.000000 fplab-0.0.2.2/fplab/tools/image.py
--rw-rw-rw-   0        0        0    15076 2024-04-06 09:13:19.000000 fplab-0.0.2.2/fplab/tools/nbis.py
--rw-rw-rw-   0        0        0    15788 2024-04-06 14:10:17.000000 fplab-0.0.2.2/fplab/tools/tensor.py
-drwxrwxrwx   0        0        0        0 2024-04-07 10:05:56.988050 fplab-0.0.2.2/fplab.egg-info/
--rw-rw-rw-   0        0        0      523 2024-04-07 10:05:56.000000 fplab-0.0.2.2/fplab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1025 2024-04-07 10:05:56.000000 fplab-0.0.2.2/fplab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 10:05:56.000000 fplab-0.0.2.2/fplab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-07 10:05:56.000000 fplab-0.0.2.2/fplab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 10:05:57.018202 fplab-0.0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      801 2024-04-07 10:05:00.000000 fplab-0.0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:01:36.276972 fplab-0.0.2.3/
+-rw-rw-rw-   0        0        0     1090 2024-03-31 02:38:30.000000 fplab-0.0.2.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      523 2024-04-14 15:01:36.276972 fplab-0.0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      862 2024-04-06 15:56:56.000000 fplab-0.0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 15:01:36.166254 fplab-0.0.2.3/fplab/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.3/fplab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:01:36.198217 fplab-0.0.2.3/fplab/enhancement/
+-rw-rw-rw-   0        0        0        0 2024-03-31 08:36:57.000000 fplab-0.0.2.3/fplab/enhancement/__init__.py
+-rw-rw-rw-   0        0        0     4472 2024-03-31 08:36:57.000000 fplab-0.0.2.3/fplab/enhancement/frequency.py
+-rw-rw-rw-   0        0        0     4454 2024-03-31 13:48:46.000000 fplab-0.0.2.3/fplab/enhancement/spatial.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:01:36.198720 fplab-0.0.2.3/fplab/generation/
+-rw-rw-rw-   0        0        0        0 2024-04-02 15:51:38.000000 fplab-0.0.2.3/fplab/generation/__init__.py
+-rw-rw-rw-   0        0        0     6948 2024-04-06 06:07:55.000000 fplab-0.0.2.3/fplab/generation/tps.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:01:36.198720 fplab-0.0.2.3/fplab/intrinsic/
+-rw-rw-rw-   0        0        0        0 2024-03-23 06:49:44.000000 fplab-0.0.2.3/fplab/intrinsic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:01:36.217119 fplab-0.0.2.3/fplab/intrinsic/frequency/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.3/fplab/intrinsic/frequency/__init__.py
+-rw-rw-rw-   0        0        0     7577 2024-03-31 08:36:57.000000 fplab-0.0.2.3/fplab/intrinsic/frequency/projection.py
+-rw-rw-rw-   0        0        0    10795 2024-03-31 08:36:57.000000 fplab-0.0.2.3/fplab/intrinsic/frequency/tools.py
+-rw-rw-rw-   0        0        0     3116 2024-04-07 04:59:12.000000 fplab-0.0.2.3/fplab/intrinsic/frequency/transform.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:01:36.217119 fplab-0.0.2.3/fplab/intrinsic/mask/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.3/fplab/intrinsic/mask/__init__.py
+-rw-rw-rw-   0        0        0      855 2024-04-06 15:25:34.000000 fplab-0.0.2.3/fplab/intrinsic/mask/mask.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:01:36.231854 fplab-0.0.2.3/fplab/intrinsic/multiple/
+-rw-rw-rw-   0        0        0        0 2024-03-23 07:06:33.000000 fplab-0.0.2.3/fplab/intrinsic/multiple/__init__.py
+-rw-rw-rw-   0        0        0     6990 2024-04-07 05:24:47.000000 fplab-0.0.2.3/fplab/intrinsic/multiple/transform.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:01:36.233058 fplab-0.0.2.3/fplab/intrinsic/orientation/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.3/fplab/intrinsic/orientation/__init__.py
+-rw-rw-rw-   0        0        0     6640 2024-04-06 09:18:53.000000 fplab-0.0.2.3/fplab/intrinsic/orientation/gradient.py
+-rw-rw-rw-   0        0        0     6215 2024-04-07 04:39:10.000000 fplab-0.0.2.3/fplab/intrinsic/orientation/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:01:36.248014 fplab-0.0.2.3/fplab/intrinsic/skeleton/
+-rw-rw-rw-   0        0        0        0 2024-04-06 15:22:02.000000 fplab-0.0.2.3/fplab/intrinsic/skeleton/__init__.py
+-rw-rw-rw-   0        0        0     1752 2024-04-06 16:14:50.000000 fplab-0.0.2.3/fplab/intrinsic/skeleton/skeleton.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:01:36.250504 fplab-0.0.2.3/fplab/matching/
+-rw-rw-rw-   0        0        0        0 2024-03-29 01:34:29.000000 fplab-0.0.2.3/fplab/matching/__init__.py
+-rw-rw-rw-   0        0        0     6956 2024-03-30 03:40:09.000000 fplab-0.0.2.3/fplab/matching/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:01:36.250504 fplab-0.0.2.3/fplab/minutiae/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.3/fplab/minutiae/__init__.py
+-rw-rw-rw-   0        0        0     6782 2024-04-14 14:52:02.000000 fplab-0.0.2.3/fplab/minutiae/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:01:36.267968 fplab-0.0.2.3/fplab/tools/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.3/fplab/tools/__init__.py
+-rw-rw-rw-   0        0        0    13732 2024-04-06 14:10:17.000000 fplab-0.0.2.3/fplab/tools/array.py
+-rw-rw-rw-   0        0        0     5367 2024-04-06 14:01:28.000000 fplab-0.0.2.3/fplab/tools/image.py
+-rw-rw-rw-   0        0        0    15076 2024-04-06 09:13:19.000000 fplab-0.0.2.3/fplab/tools/nbis.py
+-rw-rw-rw-   0        0        0    15788 2024-04-06 14:10:17.000000 fplab-0.0.2.3/fplab/tools/tensor.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:01:36.181050 fplab-0.0.2.3/fplab.egg-info/
+-rw-rw-rw-   0        0        0      523 2024-04-14 15:01:36.000000 fplab-0.0.2.3/fplab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1025 2024-04-14 15:01:36.000000 fplab-0.0.2.3/fplab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 15:01:36.000000 fplab-0.0.2.3/fplab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-14 15:01:36.000000 fplab-0.0.2.3/fplab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 15:01:36.278076 fplab-0.0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      801 2024-04-07 13:12:45.000000 fplab-0.0.2.3/setup.py
```

### Comparing `fplab-0.0.2.2/LICENSE.txt` & `fplab-0.0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.2/PKG-INFO` & `fplab-0.0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fplab
-Version: 0.0.2.2
+Version: 0.0.2.3
 Summary: Python3 Package for Fingerprint Processing
 Author: Yurun Wang
 Author-email: wangyurun@mail.sdu.edu.cn
 License: MIT
 Keywords: python,fingerprint
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fplab-0.0.2.2/README.md` & `fplab-0.0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.2/fplab/enhancement/frequency.py` & `fplab-0.0.2.3/fplab/enhancement/frequency.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.2/fplab/enhancement/spatial.py` & `fplab-0.0.2.3/fplab/enhancement/spatial.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.2/fplab/generation/tps.py` & `fplab-0.0.2.3/fplab/generation/tps.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.2/fplab/intrinsic/frequency/projection.py` & `fplab-0.0.2.3/fplab/intrinsic/frequency/projection.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.2/fplab/intrinsic/frequency/tools.py` & `fplab-0.0.2.3/fplab/intrinsic/frequency/tools.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.2/fplab/intrinsic/frequency/transform.py` & `fplab-0.0.2.3/fplab/intrinsic/frequency/transform.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.2/fplab/intrinsic/mask/mask.py` & `fplab-0.0.2.3/fplab/intrinsic/mask/mask.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.2/fplab/intrinsic/multiple/transform.py` & `fplab-0.0.2.3/fplab/intrinsic/multiple/transform.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.2/fplab/intrinsic/orientation/gradient.py` & `fplab-0.0.2.3/fplab/intrinsic/orientation/gradient.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.2/fplab/intrinsic/orientation/tools.py` & `fplab-0.0.2.3/fplab/intrinsic/orientation/tools.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.2/fplab/intrinsic/skeleton/skeleton.py` & `fplab-0.0.2.3/fplab/intrinsic/skeleton/skeleton.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.2/fplab/matching/tools.py` & `fplab-0.0.2.3/fplab/matching/tools.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.2/fplab/minutiae/tools.py` & `fplab-0.0.2.3/fplab/minutiae/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """指纹细节点相关函数
 xyt2array       从xyt文件中读取细节点
 array2xyt       将细节点保存到xyt文件
 show_mnt        展示细节点
 select_mnt      根据质量选取细节点
+mask_mnt        根据mask选取细节点
 mnt2map         根据细节点分布生成权重图
 """
 import cv2
+import copy
 import numpy as np
 from pathlib import Path
 from functools import partial
 from fplab.tools.image import type_as
 from fplab.tools.array import IMA, ima_gaussian
 
 
@@ -27,15 +29,15 @@
     with open(xyt_d, 'r') as xyt_f:
         mts = xyt_f.readlines()
     # 行索引、列索引、弧度和质量
     ind_h, ind_w, angle, quality = [], [], [], []
     for i in range(len(mts)):
         mt = mts[i].strip().split()
         # xy直角坐标系转化为hw坐标系
-        ind_h.append(h-int(mt[1])-1)
+        ind_h.append(h-int(mt[1]))
         ind_w.append(int(mt[0]))
         # 转化为弧度
         angle.append(int(mt[2])/180.*np.pi)
         # 考虑xyt可能无质量信息
         if len(mt) == 3:
             quality.append(1.)
         else:
@@ -51,19 +53,19 @@
     """将细节点mt保存到xyt文件
     mt      字典，格式需要与xyt2array的输出格式相同
     xyt_d   xyt文件地址，字符串形式或Path形式"""
     if isinstance(xyt_d, str):
         xyt_p = Path(xyt_d)
     else:
         xyt_p = xyt_d
-    xyt_p.parent.mkdir(parents=True,exist_ok=True)
+    xyt_p.parent.mkdir(parents=True, exist_ok=True)
     with open(xyt_p, 'w') as xyt_f:
         for i in range(mt["ind_hw"].shape[1]):
             x = mt["ind_hw"][1, i]
-            y = mt["shape"][0]-mt["ind_hw"][0, i]-1
+            y = mt["shape"][0]-mt["ind_hw"][0, i]
             t = round(mt["angle"][i]/np.pi*180)
             q = round(mt["quality"][i]*100)
             xyt_f.write(f"{x} {y} {t} {q}\n")
 
 
 def show_mnt(mt, im, th_q=0, q_flag=False, max_l=12,
              color=(255, 0, 0), thickness=1, tip_length=0.3,
@@ -123,14 +125,27 @@
     out = {"ind_hw": np.array([ind_h, ind_w], dtype=np.int32),
            "angle": angle.copy(),
            "quality": quality.copy(),
            "shape": shape}
     return out
 
 
+def mask_mnt(mt, mk):
+    """将mt中mask==0的细节点的质量设置为-1，然后使用select_mnt删除
+    mt              细节点，格式需要与xyt2array的输出相同。
+    mk              mask，非0像素认为是感兴趣区域"""
+    out = copy.deepcopy(mt)
+    mka = type_as(mk, "a")
+    for i in range(mt["ind_hw"].shape[1]):
+        ind_h, ind_w = mt["ind_hw"][0, i], mt["ind_hw"][1, i]
+        if abs(mka[ind_h, ind_w]) <= 1e-4:
+            out["quality"][i] = -1
+    return select_mnt(out, 0)
+
+
 def mnt2map(mt, th_q=0.2, fix_v=1., use_quality=False, filter_fn=None):
     """根据细节点mt生成权重图
     mt              细节点，格式需要与xyt2array的输出相同。
     th_q            质量阈值，去除质量小于该值的细节点
     fix_v           初始细节点图细节点处的值
     use_quality     使用细节点质量还是fix_v作为初始细节点图细节点处的值
     filter_fn       处理初始细节点的函数，接受细节点（np.ndarray）作为参数
```

### Comparing `fplab-0.0.2.2/fplab/tools/array.py` & `fplab-0.0.2.3/fplab/tools/array.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.2/fplab/tools/image.py` & `fplab-0.0.2.3/fplab/tools/image.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.2/fplab/tools/nbis.py` & `fplab-0.0.2.3/fplab/tools/nbis.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.2/fplab/tools/tensor.py` & `fplab-0.0.2.3/fplab/tools/tensor.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.2/fplab.egg-info/PKG-INFO` & `fplab-0.0.2.3/fplab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fplab
-Version: 0.0.2.2
+Version: 0.0.2.3
 Summary: Python3 Package for Fingerprint Processing
 Author: Yurun Wang
 Author-email: wangyurun@mail.sdu.edu.cn
 License: MIT
 Keywords: python,fingerprint
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fplab-0.0.2.2/fplab.egg-info/SOURCES.txt` & `fplab-0.0.2.3/fplab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.2/setup.py` & `fplab-0.0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2.2'
+VERSION = '0.0.2.3'
 DESCRIPTION = 'Python3 Package for Fingerprint Processing'
 LONG_DESCRIPTION = ('This is a python3 package for fingerprint processing,'
                     ' which can be used for fingerprint enhancement.')
 
 setup(
     name="fplab",
     version=VERSION,
```

