# Comparing `tmp/a2y_hidcom-1.1.0-cp38-cp38-win_amd64.whl.zip` & `tmp/a2y_hidcom-1.1.2-cp38-cp38-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 129243 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat   299520 b- defN 24-Feb-07 13:18 a2y_hidcom.cp38-win_amd64.pyd
--rw-rw-rw-  2.0 fat      704 b- defN 24-Feb-07 13:18 a2y_hidcom-1.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      827 b- defN 24-Feb-07 13:18 a2y_hidcom-1.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Feb-07 13:18 a2y_hidcom-1.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 24-Feb-07 13:18 a2y_hidcom-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      488 b- defN 24-Feb-07 13:18 a2y_hidcom-1.1.0.dist-info/RECORD
-6 files, 301650 bytes uncompressed, 128359 bytes compressed:  57.4%
+Zip file size: 124861 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat   280576 b- defN 24-Apr-14 14:15 a2y_hidcom.cp38-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      718 b- defN 24-Apr-14 14:15 a2y_hidcom-1.1.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      846 b- defN 24-Apr-14 14:15 a2y_hidcom-1.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-14 14:15 a2y_hidcom-1.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 24-Apr-14 14:15 a2y_hidcom-1.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      488 b- defN 24-Apr-14 14:15 a2y_hidcom-1.1.2.dist-info/RECORD
+6 files, 282739 bytes uncompressed, 123977 bytes compressed:  56.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: a2y_hidcom.cp38-win_amd64.pyd
 Comment: 
 
-Filename: a2y_hidcom-1.1.0.dist-info/LICENSE
+Filename: a2y_hidcom-1.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: a2y_hidcom-1.1.0.dist-info/METADATA
+Filename: a2y_hidcom-1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: a2y_hidcom-1.1.0.dist-info/WHEEL
+Filename: a2y_hidcom-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: a2y_hidcom-1.1.0.dist-info/top_level.txt
+Filename: a2y_hidcom-1.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: a2y_hidcom-1.1.0.dist-info/RECORD
+Filename: a2y_hidcom-1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `a2y_hidcom-1.1.0.dist-info/LICENSE` & `a2y_hidcom-1.1.2.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-This is private software.
-
-Anyone without authorization is NOT allowed to copy, modify, publish, use, compile, sell, or
-distribute this software, either in source code form or as a compiled
-binary, for any purpose, commercial or non-commercial, and by any
-means.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
-IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
-OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
-ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
-OTHER DEALINGS IN THE SOFTWARE.
+This is private software.
+
+Anyone without authorization is NOT allowed to copy, modify, publish, use, compile, sell, or
+distribute this software, either in source code form or as a compiled
+binary, for any purpose, commercial or non-commercial, and by any
+means.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
+OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+OTHER DEALINGS IN THE SOFTWARE.
```

## Comparing `a2y_hidcom-1.1.0.dist-info/METADATA` & `a2y_hidcom-1.1.2.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: a2y-hidcom
-Version: 1.1.0
+Version: 1.1.2
 Summary: 此模块实现内核科技 USB（HID）转多通道UART 的驱动程序。
 Home-page: http://www.sorobust.com/a2y/hidcom.html
 Author: Yu Han
 Author-email: hanjunyu@163.com
 License: Private
 Platform: Windows
 Platform: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: Free For Educational Use
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: pyusb >=1.2
 Requires-Dist: libusb-package >=1.0.26.0
 
 # Python Module: a2y_hidcom
 a2y_hidcom 实现内核科技 USB（HID）转多通道UART 的驱动程序。
-
-
```

