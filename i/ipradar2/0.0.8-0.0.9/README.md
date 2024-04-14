# Comparing `tmp/ipradar2-0.0.8.tar.gz` & `tmp/ipradar2-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipradar2-0.0.8.tar", last modified: Sat Feb 17 15:09:52 2024, max compression
+gzip compressed data, was "ipradar2-0.0.9.tar", last modified: Sun Apr 14 10:36:09 2024, max compression
```

## Comparing `ipradar2-0.0.8.tar` & `ipradar2-0.0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2024-02-17 15:09:52.254733 ipradar2-0.0.8/
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2024-02-17 15:09:52.244928 ipradar2-0.0.8/IPRadar2/
--rwxrwxrwx   0 marco     (1000) marco     (1000)     4528 2024-01-27 08:54:56.000000 ipradar2-0.0.8/IPRadar2/CheckableComboBox.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2024-02-17 15:09:52.245557 ipradar2-0.0.8/IPRadar2/Config/
--rwxrwxrwx   0 marco     (1000) marco     (1000)     5604 2024-02-17 08:39:27.000000 ipradar2-0.0.8/IPRadar2/Config/config.ini
--rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2024-02-17 08:35:04.000000 ipradar2-0.0.8/IPRadar2/Config/locationsResolved.json
--rwxrwxrwx   0 marco     (1000) marco     (1000)      830 2024-02-04 17:05:43.000000 ipradar2-0.0.8/IPRadar2/IPRadar2.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2024-02-17 15:09:52.246149 ipradar2-0.0.8/IPRadar2/Icons/
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1466 2024-01-13 08:17:35.000000 ipradar2-0.0.8/IPRadar2/Icons/marker-dot-icon.png
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1676 2024-01-13 08:24:32.000000 ipradar2-0.0.8/IPRadar2/Icons/marker-icon.png
--rwxrwxrwx   0 marco     (1000) marco     (1000)    34548 2024-02-17 15:07:55.000000 ipradar2-0.0.8/IPRadar2/Ui_mainWindow.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)       54 2024-02-03 07:56:47.000000 ipradar2-0.0.8/IPRadar2/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)    18430 2024-02-14 09:00:41.000000 ipradar2-0.0.8/IPRadar2/badConnectionKiller.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     8738 2024-02-04 15:41:39.000000 ipradar2-0.0.8/IPRadar2/configuration.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     4278 2024-02-14 09:01:10.000000 ipradar2-0.0.8/IPRadar2/firewallManager.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3804 2024-02-14 08:58:31.000000 ipradar2-0.0.8/IPRadar2/helper_functions.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     6459 2024-02-14 09:02:50.000000 ipradar2-0.0.8/IPRadar2/hostResolver.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2024-02-17 15:09:52.248766 ipradar2-0.0.8/IPRadar2/img/
--rwxrwxrwx   0 marco     (1000) marco     (1000)   626393 2024-01-27 13:33:58.000000 ipradar2-0.0.8/IPRadar2/img/app1.jpg
--rwxrwxrwx   0 marco     (1000) marco     (1000)  1149607 2024-01-27 13:31:40.000000 ipradar2-0.0.8/IPRadar2/img/app2.jpg
--rwxrwxrwx   0 marco     (1000) marco     (1000)    17918 2024-02-04 15:57:49.000000 ipradar2-0.0.8/IPRadar2/init_app.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)    41001 2024-02-17 09:51:38.000000 ipradar2-0.0.8/IPRadar2/mainAppWindow.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      928 2024-01-27 09:20:57.000000 ipradar2-0.0.8/IPRadar2/node.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     5586 2024-02-14 09:06:17.000000 ipradar2-0.0.8/IPRadar2/pingResolver.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)   103328 2024-02-17 15:08:13.000000 ipradar2-0.0.8/IPRadar2/processor.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)    14329 2024-02-17 09:52:35.000000 ipradar2-0.0.8/IPRadar2/pysharkSniffer.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      185 2024-01-27 13:55:27.000000 ipradar2-0.0.8/IPRadar2/updateRequirements.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1070 2024-01-27 09:19:20.000000 ipradar2-0.0.8/LICENSE
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2949 2024-02-17 15:09:52.254377 ipradar2-0.0.8/PKG-INFO
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1445 2024-02-04 10:58:03.000000 ipradar2-0.0.8/README.md
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2024-02-17 15:09:52.254022 ipradar2-0.0.8/ipradar2.egg-info/
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2949 2024-02-17 15:09:52.000000 ipradar2-0.0.8/ipradar2.egg-info/PKG-INFO
--rwxrwxrwx   0 marco     (1000) marco     (1000)      803 2024-02-17 15:09:52.000000 ipradar2-0.0.8/ipradar2.egg-info/SOURCES.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)       36 2024-02-17 15:09:52.000000 ipradar2-0.0.8/ipradar2.egg-info/dependency_links.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)       52 2024-02-17 15:09:52.000000 ipradar2-0.0.8/ipradar2.egg-info/entry_points.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)      180 2024-02-17 15:09:52.000000 ipradar2-0.0.8/ipradar2.egg-info/requires.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)        9 2024-02-17 15:09:52.000000 ipradar2-0.0.8/ipradar2.egg-info/top_level.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)       38 2024-02-17 15:09:52.254783 ipradar2-0.0.8/setup.cfg
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2917 2024-02-17 15:08:24.000000 ipradar2-0.0.8/setup.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2024-04-14 10:36:09.820997 ipradar2-0.0.9/
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2024-04-14 10:36:09.811136 ipradar2-0.0.9/IPRadar2/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     4528 2024-01-27 08:54:56.000000 ipradar2-0.0.9/IPRadar2/CheckableComboBox.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2024-04-14 10:36:09.811781 ipradar2-0.0.9/IPRadar2/Config/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     5604 2024-04-14 10:03:09.000000 ipradar2-0.0.9/IPRadar2/Config/config.ini
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2024-04-14 10:03:17.000000 ipradar2-0.0.9/IPRadar2/Config/locationsResolved.json
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      830 2024-04-08 16:09:32.000000 ipradar2-0.0.9/IPRadar2/IPRadar2.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2024-04-14 10:36:09.812430 ipradar2-0.0.9/IPRadar2/Icons/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1466 2024-01-13 08:17:35.000000 ipradar2-0.0.9/IPRadar2/Icons/marker-dot-icon.png
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1676 2024-01-13 08:24:32.000000 ipradar2-0.0.9/IPRadar2/Icons/marker-icon.png
+-rwxrwxrwx   0 marco     (1000) marco     (1000)    34548 2024-02-17 15:01:50.000000 ipradar2-0.0.9/IPRadar2/Ui_mainWindow.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)       54 2024-02-03 07:56:47.000000 ipradar2-0.0.9/IPRadar2/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)    18430 2024-02-14 09:00:41.000000 ipradar2-0.0.9/IPRadar2/badConnectionKiller.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     8807 2024-02-18 09:37:39.000000 ipradar2-0.0.9/IPRadar2/configuration.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     4278 2024-02-14 09:01:10.000000 ipradar2-0.0.9/IPRadar2/firewallManager.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3804 2024-02-14 08:58:31.000000 ipradar2-0.0.9/IPRadar2/helper_functions.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     6459 2024-02-14 09:02:50.000000 ipradar2-0.0.9/IPRadar2/hostResolver.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2024-04-14 10:36:09.814927 ipradar2-0.0.9/IPRadar2/img/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)   626393 2024-01-27 13:33:58.000000 ipradar2-0.0.9/IPRadar2/img/app1.jpg
+-rwxrwxrwx   0 marco     (1000) marco     (1000)  1149607 2024-01-27 13:31:40.000000 ipradar2-0.0.9/IPRadar2/img/app2.jpg
+-rwxrwxrwx   0 marco     (1000) marco     (1000)    17918 2024-02-04 15:57:49.000000 ipradar2-0.0.9/IPRadar2/init_app.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)    41615 2024-04-01 09:09:24.000000 ipradar2-0.0.9/IPRadar2/mainAppWindow.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      928 2024-04-07 15:34:00.000000 ipradar2-0.0.9/IPRadar2/node.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     5586 2024-02-14 09:06:17.000000 ipradar2-0.0.9/IPRadar2/pingResolver.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)   105489 2024-04-08 16:10:40.000000 ipradar2-0.0.9/IPRadar2/processor.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)    14329 2024-02-17 09:33:36.000000 ipradar2-0.0.9/IPRadar2/pysharkSniffer.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      185 2024-01-27 13:55:27.000000 ipradar2-0.0.9/IPRadar2/updateRequirements.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1070 2024-01-27 09:19:20.000000 ipradar2-0.0.9/LICENSE
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2949 2024-04-14 10:36:09.820617 ipradar2-0.0.9/PKG-INFO
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1445 2024-02-04 10:58:03.000000 ipradar2-0.0.9/README.md
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2024-04-14 10:36:09.820219 ipradar2-0.0.9/ipradar2.egg-info/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2949 2024-04-14 10:36:09.000000 ipradar2-0.0.9/ipradar2.egg-info/PKG-INFO
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      803 2024-04-14 10:36:09.000000 ipradar2-0.0.9/ipradar2.egg-info/SOURCES.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)       36 2024-04-14 10:36:09.000000 ipradar2-0.0.9/ipradar2.egg-info/dependency_links.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)       52 2024-04-14 10:36:09.000000 ipradar2-0.0.9/ipradar2.egg-info/entry_points.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      180 2024-04-14 10:36:09.000000 ipradar2-0.0.9/ipradar2.egg-info/requires.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        9 2024-04-14 10:36:09.000000 ipradar2-0.0.9/ipradar2.egg-info/top_level.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)       38 2024-04-14 10:36:09.821053 ipradar2-0.0.9/setup.cfg
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2917 2024-02-18 09:47:15.000000 ipradar2-0.0.9/setup.py
```

### Comparing `ipradar2-0.0.8/IPRadar2/CheckableComboBox.py` & `ipradar2-0.0.9/IPRadar2/CheckableComboBox.py`

 * *Files identical despite different names*

### Comparing `ipradar2-0.0.8/IPRadar2/Config/config.ini` & `ipradar2-0.0.9/IPRadar2/Config/config.ini`

 * *Files identical despite different names*

### Comparing `ipradar2-0.0.8/IPRadar2/IPRadar2.py` & `ipradar2-0.0.9/IPRadar2/IPRadar2.py`

 * *Files identical despite different names*

### Comparing `ipradar2-0.0.8/IPRadar2/Icons/marker-dot-icon.png` & `ipradar2-0.0.9/IPRadar2/Icons/marker-dot-icon.png`

 * *Files identical despite different names*

### Comparing `ipradar2-0.0.8/IPRadar2/Icons/marker-icon.png` & `ipradar2-0.0.9/IPRadar2/Icons/marker-icon.png`

 * *Files identical despite different names*

### Comparing `ipradar2-0.0.8/IPRadar2/Ui_mainWindow.py` & `ipradar2-0.0.9/IPRadar2/Ui_mainWindow.py`

 * *Files identical despite different names*

### Comparing `ipradar2-0.0.8/IPRadar2/badConnectionKiller.py` & `ipradar2-0.0.9/IPRadar2/badConnectionKiller.py`

 * *Files identical despite different names*

### Comparing `ipradar2-0.0.8/IPRadar2/configuration.py` & `ipradar2-0.0.9/IPRadar2/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,16 @@
 # *********************************************
 USE_DOUBLE_BUFFER = False
 
 # check period in seconds
 # to check: hosts resolutions, kill IPs, report updates, active connections
 # the GUI will be updated every (CHECK_PERIOD_IN_SEC * 2) seconds
 CHECK_PERIOD_IN_SEC = 0.5
+# plot after PLOT_PERIODS times CHECK_PERIOD_IN_SEC
+PLOT_PERIODS = 8
 
 # poll packet queue in seconds
 POLL_PACKET_QUEUE_IN_SEC = 0.0001
 
 # packed visualization of output to terminal
 PACKED_OUTPUT = False
```

### Comparing `ipradar2-0.0.8/IPRadar2/firewallManager.py` & `ipradar2-0.0.9/IPRadar2/firewallManager.py`

 * *Files identical despite different names*

### Comparing `ipradar2-0.0.8/IPRadar2/helper_functions.py` & `ipradar2-0.0.9/IPRadar2/helper_functions.py`

 * *Files identical despite different names*

### Comparing `ipradar2-0.0.8/IPRadar2/hostResolver.py` & `ipradar2-0.0.9/IPRadar2/hostResolver.py`

 * *Files identical despite different names*

### Comparing `ipradar2-0.0.8/IPRadar2/img/app1.jpg` & `ipradar2-0.0.9/IPRadar2/img/app1.jpg`

 * *Files identical despite different names*

### Comparing `ipradar2-0.0.8/IPRadar2/img/app2.jpg` & `ipradar2-0.0.9/IPRadar2/img/app2.jpg`

 * *Files identical despite different names*

### Comparing `ipradar2-0.0.8/IPRadar2/init_app.py` & `ipradar2-0.0.9/IPRadar2/init_app.py`

 * *Files identical despite different names*

### Comparing `ipradar2-0.0.8/IPRadar2/mainAppWindow.py` & `ipradar2-0.0.9/IPRadar2/mainAppWindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -426,46 +426,58 @@
             flags |= QtCore.Qt.WindowStaysOnBottomHint
         self.setWindowFlags(flags)
         self.show()
 
     @pyqtSlot()
     def on_pbLiveCapture_clicked(self):
         if self.pbLiveCapture.text() == "exit":
-            self.pbLiveCapture.setEnabled(False)
-            self.close()
+            if hf.show_popup_question("Stop capture and exit?") == QMessageBox.Yes:
+                self.pbLiveCapture.setEnabled(False)
+                self.close()
         else:
             self.pbOpenFile.setEnabled(False)
             self.comboBoxInterface.setEnabled(False)
             self.sniffer.sniff(self.currentInterface)
             # deactivate button
             self.pbLiveCapture.setText("exit")
             self.pbKill.setEnabled(True)
             self.pbPing.setEnabled(True)
             currentTime = strftime("%Y.%m.%d %H:%M:%S", gmtime())
             self.setWindowTitle("IPRadar2 - capture started on " + currentTime)
 
     @pyqtSlot()
     def on_pbOpenFile_clicked(self):
         if self.pbOpenFile.text() == "exit":
-            self.close()
+            if hf.show_popup_question("Close file(s) and exit?") == QMessageBox.Yes:
+                self.close()
         else:
+            self.pbLiveCapture.setEnabled(False)
+            self.pbOpenFile.setEnabled(False)
             fname = QFileDialog.getOpenFileName(
                 self, 'Open file', self.fpath, "Packet capture file (*.pcapng *.pcap *.cap)")
             if len(fname) != 0:
                 fname = fname[0]
                 if fname != "":
                     fileNameInfo = QFileInfo(fname)
                     # use same folder in next call
                     self.fpath = fileNameInfo.absolutePath()
                     self.sniffer.sniff(0, fname)
                     self.pbLiveCapture.setEnabled(False)
                     self.pbOpenFile.setEnabled(False)
                     self.comboBoxInterface.setEnabled(False)
                     self.pbOpenFile.setEnabled(True)
                     self.pbOpenFile.setText("open file")
+                else:
+                    if self.fpath == '/':
+                        self.pbLiveCapture.setEnabled(True)
+                    self.pbOpenFile.setEnabled(True)
+            else:
+                if self.fpath == '/':
+                    self.pbLiveCapture.setEnabled(True)
+                self.pbOpenFile.setEnabled(True)
 
     @pyqtSlot()
     def on_cbShowPopups_clicked(self):
         configuration.SHOW_POPUPS = not configuration.SHOW_POPUPS
 
     @pyqtSlot()
     def on_cbShowBad_clicked(self):
```

### Comparing `ipradar2-0.0.8/IPRadar2/node.py` & `ipradar2-0.0.9/IPRadar2/node.py`

 * *Files identical despite different names*

### Comparing `ipradar2-0.0.8/IPRadar2/pingResolver.py` & `ipradar2-0.0.9/IPRadar2/pingResolver.py`

 * *Files identical despite different names*

### Comparing `ipradar2-0.0.8/IPRadar2/processor.py` & `ipradar2-0.0.9/IPRadar2/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,18 @@
 from random import randint
 import ipaddress
 import fcntl
 import struct
 import os
 from getmac import get_mac_address
 import time
-# from memory_profiler import profile  # and use @profile in functions that may introduce memory leaks
+# to use the memory profiler add:
+#     from memory_profiler import profile
+# and use the decorator @profile in functions that may introduce memory leaks
+# you can also add this parameter to your configuration: -m memory_profiler
 
 
 
 # NOTE:
 #      code snippets for class GeodesicPolyLine adapted from:
 #      https://notebook.community/deeplook/notebooks/mapping/geodesic_polylines
 #      or
@@ -86,28 +89,35 @@
             kwargs1 = dict(min_length_km=min_length_km, segment_length_km=segment_length_km)
             geodesic_locs = [intermediatePoints(start, end, **kwargs1) for start, end in pairwise(locations)]
             super().__init__(geodesic_locs, **kwargs)
         else:
             super().__init__(locations, **kwargs)
 
 
+# helper function
+def is_power_of_two(n):
+    return (n & (n - 1)) == 0 and n != 0
+
+
 class ProcessorClass(object):
     # TODO: check workaround using sanitized_ip[]
     sanitized_ip = []
     selected_ip = ""
     # variable used by pingRandom() and PingRandom2()
     randomIPList = []
     packetQueueA = 0  # will be a reference to pysharkSniffer's variable
     packetQueueB = 0  # will be a reference to pysharkSniffer's variable
     currentCallbackQueueIsA = [True]  # will be a reference to pysharkSniffer's variable
     locationsRead = [False]  # will be a reference to pysharkSniffer's variable
     processedPacketsCount = 0
     sizeOfProcessingQueue = 0
     node_dict = {}
     location_dict = {}
+    offset_dict = {}
+    curr_offset_degrees = {}
     node_dict_gui = {}  # current dict of new/modified nodes to be shown/updated in GUI
     __mutex = Lock()  # for processing or accessing node_dict_gui[]
     __mutex_question = Lock()
     __questionListComplete = []  # TODO: use dict instead?
     local = "local IP address"
     public = "public IP address"
     localHost = "local host"
@@ -1489,17 +1499,17 @@
                     mac_dst = self.mac_device
                 else:
                     mac_dst = get_mac_address(ip=destination)
             else:
                 mac_dst = ""
             # create nodes
             # cases:      src         dst         (exist)
-            # 1.a            x            x
-            # 1.b            x
-            # 2.a                         x
+            # 1.a         x            x
+            # 1.b         x
+            # 2.a                      x
             # 2.b
             ################
             case = ""
             if source in self.node_dict:
                 # add destination in comm_partner_list of source
                 self.node_dict[source].comm_partner_list.append(destination)
                 ####################
@@ -1521,15 +1531,16 @@
                     self.currentNodeNumber = self.currentNodeNumber + 1
                 else:
                     case = "1a"
             else:
                 # add source in node_dict
                 source_node = NodeDataClass(self.currentNodeNumber, source, mac_src, response_src.latitude,
                                             response_src.longitude, response_src.latitude, response_src.longitude, 1,
-                                            response_src.country, pycountry.countries.get(alpha_2=response_src.country),
+                                            response_src.country,
+                                            pycountry.countries.get(alpha_2=response_src.country),
                                             response_src.region, response_src.city, host_src, True, "",
                                             host_src_resolved, ping=False, bad=False, killed=False, killed_process="",
                                             local=src_is_local, conn_established=False,
                                             tx=0, rx=0, tx_kB=0, rx_kB=0, date=strftime("%Y.%m.%d", gmtime()),
                                             time=strftime("%H:%M:%S", gmtime()), comm_partner_list=[destination],
                                             comm_partner_list_killed=[])
                 self.node_dict[source] = source_node  # new value in dict with key source (its like an "append")
@@ -1555,48 +1566,76 @@
                     case = "2a"
             ########################
             # update module variable location_dict (src)
             latlonsrc = "".join([str(self.node_dict[source].lat), ",", str(self.node_dict[source].lon)])
             if latlonsrc in self.location_dict:
                 if case == "2a" or case == "2b":
                     # increment count
-                    self.location_dict[latlonsrc] = self.location_dict[latlonsrc] + 1  # updates value
+                    self.location_dict[latlonsrc] = self.location_dict[latlonsrc] + 1
                     # update also  the source position in node_dict
                     self.node_dict[source].position = self.location_dict[latlonsrc]
                     # and update the drawing position
-                    # GeoLocationPhi = math.radians(360.0/self.node_dict[source].position)
-                    GeoLocationPhi = math.radians(6.28 * 360.0 / self.node_dict[source].position)
+                    GeoLocationPhi = math.radians(self.offset_dict[latlonsrc])
                     # set delta to CIRCLE in geo-location
                     latDelta = configuration.GeoLocationRadius * math.cos(GeoLocationPhi)
                     lonDelta = configuration.GeoLocationRadius * math.sin(GeoLocationPhi)
                     self.node_dict[source].lat_plot = self.node_dict[source].lat + latDelta
                     self.node_dict[source].lon_plot = self.node_dict[source].lon + lonDelta
+                    # update offset to evenly distribute nodes in a circle
+                    if self.node_dict[source].position % 4 == 0:
+                        if is_power_of_two(self.node_dict[source].position):
+                            self.offset_dict[latlonsrc] = (
+                                        self.offset_dict[latlonsrc] + 180.0 / self.node_dict[source].position) % 360.0
+                            self.curr_offset_degrees[latlonsrc] = 180.0 / self.node_dict[source].position
+                        else:
+                            self.offset_dict[latlonsrc] = (self.offset_dict[latlonsrc] + self.curr_offset_degrees[
+                                latlonsrc] * 2.0) % 360.0
+                    elif self.node_dict[source].position % 2 == 0:
+                        self.offset_dict[latlonsrc] = (self.offset_dict[latlonsrc] + 90.0) % 360.0
+                    else:
+                        self.offset_dict[latlonsrc] = (self.offset_dict[latlonsrc] + 180.0) % 360.0
             else:  # it must be case 2a or 2b
                 # add NEW location
-                self.location_dict[latlonsrc] = 1  # new value 1 in dict with key latlonsrc (its like an "append")
+                self.location_dict[latlonsrc] = 0  # new value 1 in dict with key latlonsrc (its like an "append")
+                self.offset_dict[latlonsrc] = 0.0
+                self.curr_offset_degrees[latlonsrc] = 90.0
                 # NOTE: self.node_dict[source].position already set to 1 by default
             # update module variable location_dict (dst)
             latlondst = "".join([str(self.node_dict[destination].lat), ",", str(self.node_dict[destination].lon)])
             if latlondst in self.location_dict:
                 if case == "1b" or case == "2b":
                     # increment count
-                    self.location_dict[latlondst] = self.location_dict[latlondst] + 1  # updates value
-                    # update also  the source position in node_dict
+                    self.location_dict[latlondst] = self.location_dict[latlondst] + 1
+                    # update also  the destination position in node_dict
                     self.node_dict[destination].position = self.location_dict[latlondst]
                     # and update the drawing position
-                    # GeoLocationPhi = math.radians(360.0/self.node_dict[destination].position)
-                    GeoLocationPhi = math.radians(6.28 * 360.0 / self.node_dict[destination].position)
+                    GeoLocationPhi = math.radians(self.offset_dict[latlondst])
                     # set delta to CIRCLE in geo-location
                     latDelta = configuration.GeoLocationRadius * math.cos(GeoLocationPhi)
                     lonDelta = configuration.GeoLocationRadius * math.sin(GeoLocationPhi)
                     self.node_dict[destination].lat_plot = self.node_dict[destination].lat + latDelta
                     self.node_dict[destination].lon_plot = self.node_dict[destination].lon + lonDelta
+                    # update offset to evenly distribute nodes in a circle
+                    if self.node_dict[destination].position % 4 == 0:
+                        if is_power_of_two(self.node_dict[destination].position):
+                            self.offset_dict[latlondst] = (
+                                        self.offset_dict[latlondst] + 180.0 / self.node_dict[destination].position)% 360.0
+                            self.curr_offset_degrees[latlondst] = 180.0 / self.node_dict[destination].position
+                        else:
+                            self.offset_dict[latlondst] = (self.offset_dict[latlondst] + self.curr_offset_degrees[
+                                latlondst] * 2.0) % 360.0
+                    elif self.node_dict[destination].position % 2 == 0:
+                        self.offset_dict[latlondst] = (self.offset_dict[latlondst] + 90.0) % 360.0
+                    else:
+                        self.offset_dict[latlondst] = (self.offset_dict[latlondst] + 180.0) % 360.0
             else:  # it must be case 1b or 2b
                 # add NEW location
-                self.location_dict[latlondst] = 1  # new value (its like an "append")
+                self.location_dict[latlondst] = 0  # new value (its like an "append")
+                self.offset_dict[latlondst] = 0.0
+                self.curr_offset_degrees[latlondst] = 90.0
                 # NOTE: self.node_dict[destination].position already set to 1 by default
             # src in black list / NOT in white list?
             if configuration.USE_WHITE_LIST:
                 badIP = ((response_src.country not in configuration.WhiteList) and (
                             response_src.city not in configuration.WhiteListCity)) or (
                                     response_src.city in configuration.BlackListCity)
             else:
@@ -1729,25 +1768,24 @@
             # we switch queue
             # self.inputPacketsCount = 0
             self.processedPacketsCount = 0
             self.currentCallbackQueueIsA[0] = False
             logging.debug("\nLog level X: switch to callback queue B")
         # start time
         startTime = time.time()
+        periods_for_plot = 0
         # main loop
         ###########
         # poll queue as fast as we can, but make small pauses to not consume too much CPU,
         # execute periodic tasks cooperatively
         while self.close_app == False:
             sleep_before_next_queue_poll = True
             if self.currentCallbackQueueIsA[0] == False:
                 if self.packetQueueA.empty() == False:
                     try:
-                        # NOTE: we may use get_nowait() i.o. get(block_=True,..)
-                        #       packet = self.packetQueueA.get_nowait()
                         packet = self.packetQueueA.get(block=True, timeout=configuration.POLL_PACKET_QUEUE_IN_SEC)
                         if packet != None:
                             self.processedPacketsCount = self.processedPacketsCount + 1
                             logging.debug("\nmain loop(A) pkt-nr = " + str(self.processedPacketsCount))
                             self.sizeOfProcessingQueue = self.packetQueueA.qsize()
                             self.processPacket(packet)
                             sleep_before_next_queue_poll = False
@@ -1757,44 +1795,45 @@
                                 if self.packetQueueB.empty() == False:
                                     self.switchQueues()
                     except Exception as e:
                         logging.exception("Exception in packet processing in Queue A: " + str(e))
             else:
                 if self.packetQueueB.empty() == False:
                     try:
-                        # NOTE: we may use get_nowait() i.o. get(block_=True,..)
-                        #       packet = self.packetQueueB.get_nowait()
                         packet = self.packetQueueB.get(block=True, timeout=configuration.POLL_PACKET_QUEUE_IN_SEC)
                         if packet != None:
                             self.processedPacketsCount = self.processedPacketsCount + 1
                             logging.debug("\nmain loop(B) pkt-nr = " + str(self.processedPacketsCount))
                             self.sizeOfProcessingQueue = self.packetQueueB.qsize()
                             self.processPacket(packet)
                             sleep_before_next_queue_poll = False
                         if self.packetQueueB.empty() == True:
                             if configuration.USE_DOUBLE_BUFFER == True:
                                 # switch only if the other queue is NOT empty, otherwise continue with queueB
                                 if self.packetQueueA.empty() == False:
                                     self.switchQueues()
-                    except Exception:  # as e:
+                    except Exception as e:
                         logging.exception("Exception in packet processing in Queue B: " + str(e))
             # currentTime
             timeDiff = time.time() - startTime
             # periodic tasks
             ################
-            if timeDiff > configuration.CHECK_PERIOD_IN_SEC*4.0:
+            if timeDiff > configuration.CHECK_PERIOD_IN_SEC:
                 # start time
                 startTime = time.time()
                 logging.debug("Checking processing status..")
                 self.checkForHostsPinged()
                 self.checkForHostsResolution()
                 self.checkKilledConnections()
                 self.checkActiveConnections()
                 # plot map
-                if configuration.PLOT and self.needUpdate:
-                    self.plotMap()
+                periods_for_plot = periods_for_plot + 1
+                if periods_for_plot == configuration.PLOT_PERIODS:
+                    periods_for_plot = 0
+                    if configuration.PLOT and self.needUpdate:
+                        self.plotMap()
                 sleep_before_next_queue_poll = False
             # we need to wait a little bit in order to not consume too much CPU
             if sleep_before_next_queue_poll:
                 time.sleep(configuration.POLL_PACKET_QUEUE_IN_SEC)
         # end of processingThread()
         logging.info("leaving processingThread..")
```

### Comparing `ipradar2-0.0.8/IPRadar2/pysharkSniffer.py` & `ipradar2-0.0.9/IPRadar2/pysharkSniffer.py`

 * *Files identical despite different names*

### Comparing `ipradar2-0.0.8/LICENSE` & `ipradar2-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ipradar2-0.0.8/PKG-INFO` & `ipradar2-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipradar2
-Version: 0.0.8
+Version: 0.0.9
 Summary: Intrusion Detection and Prevention in real time based e.g. on geographical locations of hosts
 Home-page: https://www.codeproject.com/Articles/5269206/IP-Radar-2-Real-Time-Detection-and-Defense
 Author: Clark Fieseln
 Author-email: 
 License: MIT
 Project-URL: Source, https://github.com/ClarkFieseln/IPRadar2ForLinux
 Keywords: cybersecurity,cyber security,cyber-security,security,IDS,IDPS,NW-IDS,NW IDS,network IDS,network-IDS,pyqt5,open streetmap,open-streetmap,network-analysis,firewall,pyshark,tshark,pyqt
```

### Comparing `ipradar2-0.0.8/README.md` & `ipradar2-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ipradar2-0.0.8/ipradar2.egg-info/PKG-INFO` & `ipradar2-0.0.9/ipradar2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipradar2
-Version: 0.0.8
+Version: 0.0.9
 Summary: Intrusion Detection and Prevention in real time based e.g. on geographical locations of hosts
 Home-page: https://www.codeproject.com/Articles/5269206/IP-Radar-2-Real-Time-Detection-and-Defense
 Author: Clark Fieseln
 Author-email: 
 License: MIT
 Project-URL: Source, https://github.com/ClarkFieseln/IPRadar2ForLinux
 Keywords: cybersecurity,cyber security,cyber-security,security,IDS,IDPS,NW-IDS,NW IDS,network IDS,network-IDS,pyqt5,open streetmap,open-streetmap,network-analysis,firewall,pyshark,tshark,pyqt
```

### Comparing `ipradar2-0.0.8/ipradar2.egg-info/SOURCES.txt` & `ipradar2-0.0.9/ipradar2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipradar2-0.0.8/setup.py` & `ipradar2-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 # This call to setup() does all the work
 setup(
     name="ipradar2",
     version=__version__,
     description = "Intrusion Detection and Prevention in real time based e.g. on geographical locations of hosts",
     long_description=README,
```

