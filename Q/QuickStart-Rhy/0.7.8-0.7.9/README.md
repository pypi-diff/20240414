# Comparing `tmp/quickstart_rhy-0.7.8.tar.gz` & `tmp/quickstart_rhy-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart_rhy-0.7.8.tar", max compression
+gzip compressed data, was "quickstart_rhy-0.7.9.tar", max compression
```

## Comparing `quickstart_rhy-0.7.8.tar` & `quickstart_rhy-0.7.9.tar`

### file list

```diff
@@ -1,51 +1,50 @@
--rw-r--r--   0        0        0     1067 2019-09-20 01:32:29.136250 quickstart_rhy-0.7.8/LICENSE
--rw-r--r--   0        0        0     5952 2023-02-05 05:20:04.108908 quickstart_rhy-0.7.8/QuickStart_Rhy/API/AliCloud.py
--rw-r--r--   0        0        0     3525 2023-03-27 00:35:40.568103 quickstart_rhy-0.7.8/QuickStart_Rhy/API/BaiduCloud.py
--rw-r--r--   0        0        0     4041 2023-05-18 09:09:18.744642 quickstart_rhy-0.7.8/QuickStart_Rhy/API/ChatGPT.py
--rw-r--r--   0        0        0      462 2023-02-24 04:34:17.917996 quickstart_rhy-0.7.8/QuickStart_Rhy/API/DeepL.py
--rw-r--r--   0        0        0     2121 2023-10-31 07:38:02.371310 quickstart_rhy-0.7.8/QuickStart_Rhy/API/DeepLX.py
--rw-r--r--   0        0        0     1191 2023-04-30 06:41:55.816233 quickstart_rhy-0.7.8/QuickStart_Rhy/API/Lolicon.py
--rw-r--r--   0        0        0     6264 2023-01-22 11:43:21.457920 quickstart_rhy-0.7.8/QuickStart_Rhy/API/QiniuOSS.py
--rw-r--r--   0        0        0     9434 2023-01-22 17:11:40.937202 quickstart_rhy-0.7.8/QuickStart_Rhy/API/SimpleAPI.py
--rw-r--r--   0        0        0     7276 2023-02-22 02:46:13.021767 quickstart_rhy-0.7.8/QuickStart_Rhy/API/TencentCloud.py
--rw-r--r--   0        0        0     1701 2023-03-04 05:55:10.455205 quickstart_rhy-0.7.8/QuickStart_Rhy/API/__init__.py
--rw-r--r--   0        0        0    15327 2023-07-12 06:46:26.939473 quickstart_rhy-0.7.8/QuickStart_Rhy/API/alapi.py
--rw-r--r--   0        0        0     2426 2023-09-28 08:49:11.404905 quickstart_rhy-0.7.8/QuickStart_Rhy/ImageTools/ColorTools.py
--rw-r--r--   0        0        0    13292 2023-04-18 12:58:33.288943 quickstart_rhy-0.7.8/QuickStart_Rhy/ImageTools/ImagePreview.py
--rw-r--r--   0        0        0     3805 2023-04-18 12:54:35.211459 quickstart_rhy-0.7.8/QuickStart_Rhy/ImageTools/ImageTools.py
--rw-r--r--   0        0        0     4035 2023-01-16 12:04:31.734545 quickstart_rhy-0.7.8/QuickStart_Rhy/ImageTools/VideoTools.py
--rw-r--r--   0        0        0       75 2021-01-14 15:40:19.416041 quickstart_rhy-0.7.8/QuickStart_Rhy/ImageTools/__init__.py
--rw-r--r--   0        0        0     1768 2022-11-18 20:23:12.379800 quickstart_rhy-0.7.8/QuickStart_Rhy/NetTools/HttpServer.py
--rw-r--r--   0        0        0     5133 2023-01-22 12:27:25.009662 quickstart_rhy-0.7.8/QuickStart_Rhy/NetTools/M3u8DL.py
--rw-r--r--   0        0        0     8885 2023-07-02 12:33:01.241267 quickstart_rhy-0.7.8/QuickStart_Rhy/NetTools/MultiSingleDL.py
--rw-r--r--   0        0        0    14748 2023-04-04 03:26:04.977775 quickstart_rhy-0.7.8/QuickStart_Rhy/NetTools/NormalDL.py
--rw-r--r--   0        0        0     3818 2022-11-18 20:23:25.282202 quickstart_rhy-0.7.8/QuickStart_Rhy/NetTools/WiFi.py
--rw-r--r--   0        0        0     3227 2022-11-18 20:23:28.660759 quickstart_rhy-0.7.8/QuickStart_Rhy/NetTools/WiFiDarwin.py
--rw-r--r--   0        0        0     6001 2023-02-16 12:56:59.801774 quickstart_rhy-0.7.8/QuickStart_Rhy/NetTools/__init__.py
--rw-r--r--   0        0        0     1075 2023-05-04 07:12:24.212283 quickstart_rhy-0.7.8/QuickStart_Rhy/NumbaTools/__init__.py
--rw-r--r--   0        0        0     8935 2023-01-16 13:31:49.562044 quickstart_rhy-0.7.8/QuickStart_Rhy/SystemTools/Compress.py
--rw-r--r--   0        0        0     5145 2023-01-16 13:34:40.162030 quickstart_rhy-0.7.8/QuickStart_Rhy/SystemTools/Diff.py
--rw-r--r--   0        0        0     1377 2022-11-18 19:05:09.495382 quickstart_rhy-0.7.8/QuickStart_Rhy/SystemTools/DiskMac.py
--rw-r--r--   0        0        0     1130 2022-11-18 20:23:45.475865 quickstart_rhy-0.7.8/QuickStart_Rhy/SystemTools/FileHash.py
--rw-r--r--   0        0        0      795 2023-01-29 05:36:58.386300 quickstart_rhy-0.7.8/QuickStart_Rhy/SystemTools/__init__.py
--rw-r--r--   0        0        0     3255 2023-01-17 09:56:11.282076 quickstart_rhy-0.7.8/QuickStart_Rhy/ThreadTools/__init__.py
--rw-r--r--   0        0        0     1603 2023-04-22 06:36:51.515102 quickstart_rhy-0.7.8/QuickStart_Rhy/TuiTools/Bar.py
--rw-r--r--   0        0        0     1268 2022-11-18 20:24:15.189225 quickstart_rhy-0.7.8/QuickStart_Rhy/TuiTools/Line.py
--rw-r--r--   0        0        0     1753 2023-01-16 10:23:26.070865 quickstart_rhy-0.7.8/QuickStart_Rhy/TuiTools/Table.py
--rw-r--r--   0        0        0       18 2022-05-03 07:21:41.109725 quickstart_rhy-0.7.8/QuickStart_Rhy/TuiTools/__init__.py
--rw-r--r--   0        0        0     3782 2023-01-22 07:37:58.889811 quickstart_rhy-0.7.8/QuickStart_Rhy/Wrapper/__init__.py
--rw-r--r--   0        0        0      772 2022-11-18 20:24:38.518900 quickstart_rhy-0.7.8/QuickStart_Rhy/__cache__.py
--rw-r--r--   0        0        0     8625 2023-05-04 11:46:15.495588 quickstart_rhy-0.7.8/QuickStart_Rhy/__config__.py
--rw-r--r--   0        0        0    15011 2023-09-28 03:12:22.566371 quickstart_rhy-0.7.8/QuickStart_Rhy/__init__.py
--rw-r--r--   0        0        0    38976 2023-09-27 03:28:23.619310 quickstart_rhy-0.7.8/QuickStart_Rhy/apiTools.py
--rw-r--r--   0        0        0     6720 2023-05-04 11:42:01.250240 quickstart_rhy-0.7.8/QuickStart_Rhy/funcList.py
--rw-r--r--   0        0        0     5856 2023-09-28 08:49:11.404948 quickstart_rhy-0.7.8/QuickStart_Rhy/imageDeal.py
--rw-r--r--   0        0        0    35036 2023-05-18 15:01:45.230103 quickstart_rhy-0.7.8/QuickStart_Rhy/lang.json
--rw-r--r--   0        0        0     1729 2023-05-18 14:59:51.881230 quickstart_rhy-0.7.8/QuickStart_Rhy/main.py
--rw-r--r--   0        0        0    11808 2023-05-04 08:04:12.459408 quickstart_rhy-0.7.8/QuickStart_Rhy/netTools.py
--rw-r--r--   0        0        0     1957 2023-01-22 12:33:43.387980 quickstart_rhy-0.7.8/QuickStart_Rhy/qsLesson.py
--rw-r--r--   0        0        0     6096 2023-03-16 03:09:08.732591 quickstart_rhy-0.7.8/QuickStart_Rhy/system.py
--rw-r--r--   0        0        0      701 2023-01-16 10:30:39.811901 quickstart_rhy-0.7.8/README.md
--rw-r--r--   0        0        0      548 2023-10-31 07:39:02.888615 quickstart_rhy-0.7.8/pyproject.toml
--rw-r--r--   0        0        0     1846 1970-01-01 00:00:00.000000 quickstart_rhy-0.7.8/setup.py
--rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 quickstart_rhy-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2019-09-20 01:32:29.136250 quickstart_rhy-0.7.9/LICENSE
+-rw-r--r--   0        0        0     5952 2023-02-05 05:20:04.108908 quickstart_rhy-0.7.9/QuickStart_Rhy/API/AliCloud.py
+-rw-r--r--   0        0        0     3525 2023-03-27 00:35:40.568103 quickstart_rhy-0.7.9/QuickStart_Rhy/API/BaiduCloud.py
+-rw-r--r--   0        0        0     4041 2023-05-18 09:09:18.744642 quickstart_rhy-0.7.9/QuickStart_Rhy/API/ChatGPT.py
+-rw-r--r--   0        0        0      462 2023-02-24 04:34:17.917996 quickstart_rhy-0.7.9/QuickStart_Rhy/API/DeepL.py
+-rw-r--r--   0        0        0     2121 2023-10-31 07:38:02.371310 quickstart_rhy-0.7.9/QuickStart_Rhy/API/DeepLX.py
+-rw-r--r--   0        0        0     1191 2023-04-30 06:41:55.816233 quickstart_rhy-0.7.9/QuickStart_Rhy/API/Lolicon.py
+-rw-r--r--   0        0        0     6264 2023-01-22 11:43:21.457920 quickstart_rhy-0.7.9/QuickStart_Rhy/API/QiniuOSS.py
+-rw-r--r--   0        0        0     9434 2023-01-22 17:11:40.937202 quickstart_rhy-0.7.9/QuickStart_Rhy/API/SimpleAPI.py
+-rw-r--r--   0        0        0     7225 2023-11-06 16:13:37.371665 quickstart_rhy-0.7.9/QuickStart_Rhy/API/TencentCloud.py
+-rw-r--r--   0        0        0     1701 2023-03-04 05:55:10.455205 quickstart_rhy-0.7.9/QuickStart_Rhy/API/__init__.py
+-rw-r--r--   0        0        0    15327 2023-07-12 06:46:26.939473 quickstart_rhy-0.7.9/QuickStart_Rhy/API/alapi.py
+-rw-r--r--   0        0        0     2426 2023-09-28 08:49:11.404905 quickstart_rhy-0.7.9/QuickStart_Rhy/ImageTools/ColorTools.py
+-rw-r--r--   0        0        0    13292 2023-04-18 12:58:33.288943 quickstart_rhy-0.7.9/QuickStart_Rhy/ImageTools/ImagePreview.py
+-rw-r--r--   0        0        0     3805 2023-04-18 12:54:35.211459 quickstart_rhy-0.7.9/QuickStart_Rhy/ImageTools/ImageTools.py
+-rw-r--r--   0        0        0     4035 2023-01-16 12:04:31.734545 quickstart_rhy-0.7.9/QuickStart_Rhy/ImageTools/VideoTools.py
+-rw-r--r--   0        0        0       75 2021-01-14 15:40:19.416041 quickstart_rhy-0.7.9/QuickStart_Rhy/ImageTools/__init__.py
+-rw-r--r--   0        0        0     1768 2022-11-18 20:23:12.379800 quickstart_rhy-0.7.9/QuickStart_Rhy/NetTools/HttpServer.py
+-rw-r--r--   0        0        0     5133 2023-01-22 12:27:25.009662 quickstart_rhy-0.7.9/QuickStart_Rhy/NetTools/M3u8DL.py
+-rw-r--r--   0        0        0     8885 2023-07-02 12:33:01.241267 quickstart_rhy-0.7.9/QuickStart_Rhy/NetTools/MultiSingleDL.py
+-rw-r--r--   0        0        0    14748 2023-04-04 03:26:04.977775 quickstart_rhy-0.7.9/QuickStart_Rhy/NetTools/NormalDL.py
+-rw-r--r--   0        0        0     3818 2022-11-18 20:23:25.282202 quickstart_rhy-0.7.9/QuickStart_Rhy/NetTools/WiFi.py
+-rw-r--r--   0        0        0     3227 2022-11-18 20:23:28.660759 quickstart_rhy-0.7.9/QuickStart_Rhy/NetTools/WiFiDarwin.py
+-rw-r--r--   0        0        0     6001 2023-02-16 12:56:59.801774 quickstart_rhy-0.7.9/QuickStart_Rhy/NetTools/__init__.py
+-rw-r--r--   0        0        0     1075 2023-05-04 07:12:24.212283 quickstart_rhy-0.7.9/QuickStart_Rhy/NumbaTools/__init__.py
+-rw-r--r--   0        0        0     8935 2023-01-16 13:31:49.562044 quickstart_rhy-0.7.9/QuickStart_Rhy/SystemTools/Compress.py
+-rw-r--r--   0        0        0     5145 2023-01-16 13:34:40.162030 quickstart_rhy-0.7.9/QuickStart_Rhy/SystemTools/Diff.py
+-rw-r--r--   0        0        0     1377 2022-11-18 19:05:09.495382 quickstart_rhy-0.7.9/QuickStart_Rhy/SystemTools/DiskMac.py
+-rw-r--r--   0        0        0     1130 2022-11-18 20:23:45.475865 quickstart_rhy-0.7.9/QuickStart_Rhy/SystemTools/FileHash.py
+-rw-r--r--   0        0        0      795 2023-01-29 05:36:58.386300 quickstart_rhy-0.7.9/QuickStart_Rhy/SystemTools/__init__.py
+-rw-r--r--   0        0        0     3255 2023-01-17 09:56:11.282076 quickstart_rhy-0.7.9/QuickStart_Rhy/ThreadTools/__init__.py
+-rw-r--r--   0        0        0     1603 2023-04-22 06:36:51.515102 quickstart_rhy-0.7.9/QuickStart_Rhy/TuiTools/Bar.py
+-rw-r--r--   0        0        0     1268 2022-11-18 20:24:15.189225 quickstart_rhy-0.7.9/QuickStart_Rhy/TuiTools/Line.py
+-rw-r--r--   0        0        0     1753 2023-01-16 10:23:26.070865 quickstart_rhy-0.7.9/QuickStart_Rhy/TuiTools/Table.py
+-rw-r--r--   0        0        0       18 2022-05-03 07:21:41.109725 quickstart_rhy-0.7.9/QuickStart_Rhy/TuiTools/__init__.py
+-rw-r--r--   0        0        0     3782 2023-01-22 07:37:58.889811 quickstart_rhy-0.7.9/QuickStart_Rhy/Wrapper/__init__.py
+-rw-r--r--   0        0        0      772 2022-11-18 20:24:38.518900 quickstart_rhy-0.7.9/QuickStart_Rhy/__cache__.py
+-rw-r--r--   0        0        0     8625 2023-05-04 11:46:15.495588 quickstart_rhy-0.7.9/QuickStart_Rhy/__config__.py
+-rw-r--r--   0        0        0    15011 2023-09-28 03:12:22.566371 quickstart_rhy-0.7.9/QuickStart_Rhy/__init__.py
+-rw-r--r--   0        0        0    38976 2023-09-27 03:28:23.619310 quickstart_rhy-0.7.9/QuickStart_Rhy/apiTools.py
+-rw-r--r--   0        0        0     6720 2023-05-04 11:42:01.250240 quickstart_rhy-0.7.9/QuickStart_Rhy/funcList.py
+-rw-r--r--   0        0        0     5856 2023-09-28 08:49:11.404948 quickstart_rhy-0.7.9/QuickStart_Rhy/imageDeal.py
+-rw-r--r--   0        0        0    35036 2023-05-18 15:01:45.230103 quickstart_rhy-0.7.9/QuickStart_Rhy/lang.json
+-rw-r--r--   0        0        0     1729 2023-05-18 14:59:51.881230 quickstart_rhy-0.7.9/QuickStart_Rhy/main.py
+-rw-r--r--   0        0        0    11808 2023-05-04 08:04:12.459408 quickstart_rhy-0.7.9/QuickStart_Rhy/netTools.py
+-rw-r--r--   0        0        0     1957 2023-01-22 12:33:43.387980 quickstart_rhy-0.7.9/QuickStart_Rhy/qsLesson.py
+-rw-r--r--   0        0        0     6096 2023-03-16 03:09:08.732591 quickstart_rhy-0.7.9/QuickStart_Rhy/system.py
+-rw-r--r--   0        0        0      701 2023-01-16 10:30:39.811901 quickstart_rhy-0.7.9/README.md
+-rw-r--r--   0        0        0      548 2023-11-06 16:14:04.763954 quickstart_rhy-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0     1539 1970-01-01 00:00:00.000000 quickstart_rhy-0.7.9/PKG-INFO
```

### Comparing `quickstart_rhy-0.7.8/LICENSE` & `quickstart_rhy-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/API/AliCloud.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/API/AliCloud.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/API/BaiduCloud.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/API/BaiduCloud.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/API/ChatGPT.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/API/ChatGPT.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/API/DeepLX.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/API/DeepLX.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/API/Lolicon.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/API/Lolicon.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/API/QiniuOSS.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/API/QiniuOSS.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/API/SimpleAPI.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/API/SimpleAPI.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/API/TencentCloud.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/API/TencentCloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,16 +148,14 @@
             else "https://" + bucket + ".cos." + self.region + ".myqcloud.com/",
         )
         qs_default_console.print(tb, justify="center")
 
 
 class Translate:
 
-    from tencentcloud.tmt.v20180321 import models
-
     def __init__(self, scid, sckey, region):
         """
         初始化并登陆腾讯翻译接口
 
         Initialize and log in Tencent translation interface
 
         :param scid: secret id
```

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/API/__init__.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/API/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/API/alapi.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/API/alapi.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/ImageTools/ColorTools.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/ImageTools/ColorTools.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/ImageTools/ImagePreview.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/ImageTools/ImagePreview.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/ImageTools/ImageTools.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/ImageTools/ImageTools.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/ImageTools/VideoTools.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/ImageTools/VideoTools.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/NetTools/HttpServer.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/NetTools/HttpServer.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/NetTools/M3u8DL.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/NetTools/M3u8DL.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/NetTools/MultiSingleDL.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/NetTools/MultiSingleDL.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/NetTools/NormalDL.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/NetTools/NormalDL.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/NetTools/WiFi.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/NetTools/WiFi.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/NetTools/WiFiDarwin.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/NetTools/WiFiDarwin.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/NetTools/__init__.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/NetTools/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/NumbaTools/__init__.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/NumbaTools/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/SystemTools/Compress.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/SystemTools/Compress.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/SystemTools/Diff.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/SystemTools/Diff.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/SystemTools/DiskMac.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/SystemTools/DiskMac.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/SystemTools/FileHash.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/SystemTools/FileHash.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/SystemTools/__init__.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/SystemTools/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/ThreadTools/__init__.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/ThreadTools/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/TuiTools/Bar.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/TuiTools/Bar.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/TuiTools/Line.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/TuiTools/Line.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/TuiTools/Table.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/TuiTools/Table.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/Wrapper/__init__.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/Wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/__cache__.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/__cache__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/__config__.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/__config__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/__init__.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/apiTools.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/apiTools.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/funcList.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/funcList.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/imageDeal.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/imageDeal.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/lang.json` & `quickstart_rhy-0.7.9/QuickStart_Rhy/lang.json`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/main.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/main.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/netTools.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/netTools.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/qsLesson.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/qsLesson.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/QuickStart_Rhy/system.py` & `quickstart_rhy-0.7.9/QuickStart_Rhy/system.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/README.md` & `quickstart_rhy-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.8/pyproject.toml` & `quickstart_rhy-0.7.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "QuickStart-Rhy"
-version = "0.7.8"
+version = "0.7.9"
 description = "A Command Line Toolbox"
 authors = ["Rhythmicc <rhythmlian.cn@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "QuickStart_Rhy"}, {include = "QuickStart_Rhy/lang.json"}]
 
 [tool.poetry.dependencies]
```

### Comparing `quickstart_rhy-0.7.8/PKG-INFO` & `quickstart_rhy-0.7.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
-Name: quickstart-rhy
-Version: 0.7.8
+Name: QuickStart-Rhy
+Version: 0.7.9
 Summary: A Command Line Toolbox
 License: MIT
 Author: Rhythmicc
 Author-email: rhythmlian.cn@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Qpro (>=0.12.1,<0.13.0)
 Requires-Dist: inquirer-rhy (>=0.1.2,<0.2.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.3.4,<14.0.0)
 Requires-Dist: urllib3 (>=1.26.15,<2.0.0)
 Description-Content-Type: text/markdown
```

