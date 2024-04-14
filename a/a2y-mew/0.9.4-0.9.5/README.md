# Comparing `tmp/a2y_mew-0.9.4-cp38-cp38-win_amd64.whl.zip` & `tmp/a2y_mew-0.9.5-cp38-cp38-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 214389 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat   561664 b- defN 24-Feb-02 08:58 a2y_mew.cp38-win_amd64.pyd
--rw-rw-rw-  2.0 fat      704 b- defN 24-Feb-02 08:58 a2y_mew-0.9.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1251 b- defN 24-Feb-02 08:58 a2y_mew-0.9.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Feb-02 08:58 a2y_mew-0.9.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-Feb-02 08:58 a2y_mew-0.9.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      470 b- defN 24-Feb-02 08:58 a2y_mew-0.9.4.dist-info/RECORD
-6 files, 564197 bytes uncompressed, 213541 bytes compressed:  62.2%
+Zip file size: 208387 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat   529920 b- defN 24-Apr-14 14:19 a2y_mew.cp38-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      718 b- defN 24-Apr-14 14:19 a2y_mew-0.9.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1272 b- defN 24-Apr-14 14:19 a2y_mew-0.9.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-14 14:19 a2y_mew-0.9.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-14 14:19 a2y_mew-0.9.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      470 b- defN 24-Apr-14 14:19 a2y_mew-0.9.5.dist-info/RECORD
+6 files, 532488 bytes uncompressed, 207539 bytes compressed:  61.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: a2y_mew.cp38-win_amd64.pyd
 Comment: 
 
-Filename: a2y_mew-0.9.4.dist-info/LICENSE
+Filename: a2y_mew-0.9.5.dist-info/LICENSE
 Comment: 
 
-Filename: a2y_mew-0.9.4.dist-info/METADATA
+Filename: a2y_mew-0.9.5.dist-info/METADATA
 Comment: 
 
-Filename: a2y_mew-0.9.4.dist-info/WHEEL
+Filename: a2y_mew-0.9.5.dist-info/WHEEL
 Comment: 
 
-Filename: a2y_mew-0.9.4.dist-info/top_level.txt
+Filename: a2y_mew-0.9.5.dist-info/top_level.txt
 Comment: 
 
-Filename: a2y_mew-0.9.4.dist-info/RECORD
+Filename: a2y_mew-0.9.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `a2y_mew-0.9.4.dist-info/LICENSE` & `a2y_mew-0.9.5.dist-info/LICENSE`

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

## Comparing `a2y_mew-0.9.4.dist-info/METADATA` & `a2y_mew-0.9.5.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: a2y-mew
-Version: 0.9.4
+Version: 0.9.5
 Summary: A module that implements improved Mewtocol.
 Home-page: http://www.sorobust.com/a2y/mew.html
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
 Requires-Dist: pyserial >=3.0
-Requires-Dist: a2y-hidcom >=0.9.2
+Requires-Dist: a2y-hidcom >=1.1.2
 
 # Python Module: a2y_mew
 a2y_mew模块实现了扩展的Mewtocol通信协议。原始的Mewtocol来自Panasonic，用于其FP系列PLC与上位机、触摸屏等设备通信。
 本模块在以下方面对Mewtocol进行了扩展：
 - 地址空间从8位整数扩展为不定长，最高可达32位。为了兼容性，最小为8位，在报文中至少占两个字节。
 - 通讯方式从半双工增强为全双工，即主从双方可以同时发送数据。当从设备发生了某个事件（例如，输入点发生了变化），可以主动给主机发送报文。
-
```

