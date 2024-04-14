# Comparing `tmp/sciveo-0.0.45.tar.gz` & `tmp/sciveo-0.0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciveo-0.0.45.tar", last modified: Sat Apr 13 06:54:38 2024, max compression
+gzip compressed data, was "sciveo-0.0.46.tar", last modified: Sun Apr 14 08:57:35 2024, max compression
```

## Comparing `sciveo-0.0.45.tar` & `sciveo-0.0.46.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-13 06:54:38.931099 sciveo-0.0.45/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6168 2024-04-13 06:54:38.930920 sciveo-0.0.45/PKG-INFO
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6055 2024-04-10 20:04:28.000000 sciveo-0.0.45/README.md
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-13 06:54:38.902453 sciveo-0.0.45/sciveo/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1297 2024-04-13 06:50:59.000000 sciveo-0.0.45/sciveo/__init__.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-13 06:54:38.913643 sciveo-0.0.45/sciveo/api/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:04:12.000000 sciveo-0.0.45/sciveo/api/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1788 2024-04-07 18:52:23.000000 sciveo-0.0.45/sciveo/api/base.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1815 2024-04-05 16:37:24.000000 sciveo-0.0.45/sciveo/api/upload.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-13 06:54:38.916382 sciveo-0.0.45/sciveo/common/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:03:59.000000 sciveo-0.0.45/sciveo/common/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2043 2024-03-14 17:02:24.000000 sciveo-0.0.45/sciveo/common/configuration.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1583 2024-03-14 17:02:24.000000 sciveo-0.0.45/sciveo/common/model.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3842 2024-04-07 18:52:23.000000 sciveo-0.0.45/sciveo/common/optimizers.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)    10567 2024-03-19 14:47:24.000000 sciveo-0.0.45/sciveo/common/sampling.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-13 06:54:38.920070 sciveo-0.0.45/sciveo/common/tools/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:07:07.000000 sciveo-0.0.45/sciveo/common/tools/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1416 2024-04-13 06:51:43.000000 sciveo-0.0.45/sciveo/common/tools/daemon.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1053 2023-11-17 12:42:35.000000 sciveo-0.0.45/sciveo/common/tools/formating.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1552 2024-04-08 15:42:14.000000 sciveo-0.0.45/sciveo/common/tools/hardware.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1071 2023-11-15 15:21:05.000000 sciveo-0.0.45/sciveo/common/tools/logger.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1102 2023-12-10 07:08:19.000000 sciveo-0.0.45/sciveo/common/tools/synchronized.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-13 06:54:38.926544 sciveo-0.0.45/sciveo/content/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:14:23.000000 sciveo-0.0.45/sciveo/content/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      827 2024-03-14 17:02:24.000000 sciveo-0.0.45/sciveo/content/dataset.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     5859 2024-04-07 18:52:23.000000 sciveo-0.0.45/sciveo/content/experiment.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3129 2024-04-07 18:52:23.000000 sciveo-0.0.45/sciveo/content/project.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2015 2024-03-19 14:47:07.000000 sciveo-0.0.45/sciveo/content/runner.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-13 06:54:38.928869 sciveo-0.0.45/sciveo/monitoring/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2024-04-07 18:52:23.000000 sciveo-0.0.45/sciveo/monitoring/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3684 2024-04-13 06:01:12.000000 sciveo-0.0.45/sciveo/monitoring/monitor.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1440 2024-04-13 06:48:20.000000 sciveo-0.0.45/sciveo/monitoring/start.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       24 2024-04-13 05:14:12.000000 sciveo-0.0.45/sciveo/version.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-13 06:54:38.912673 sciveo-0.0.45/sciveo.egg-info/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6168 2024-04-13 06:54:38.000000 sciveo-0.0.45/sciveo.egg-info/PKG-INFO
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      906 2024-04-13 06:54:38.000000 sciveo-0.0.45/sciveo.egg-info/SOURCES.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        1 2024-04-13 06:54:38.000000 sciveo-0.0.45/sciveo.egg-info/dependency_links.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       50 2024-04-13 06:54:38.000000 sciveo-0.0.45/sciveo.egg-info/requires.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        7 2024-04-13 06:54:38.000000 sciveo-0.0.45/sciveo.egg-info/top_level.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       38 2024-04-13 06:54:38.931153 sciveo-0.0.45/setup.cfg
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      418 2024-04-07 18:52:23.000000 sciveo-0.0.45/setup.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-13 06:54:38.930564 sciveo-0.0.45/test/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      521 2024-03-14 17:02:24.000000 sciveo-0.0.45/test/test_configuration.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3256 2024-04-10 18:44:45.000000 sciveo-0.0.45/test/test_monitoring.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1554 2024-03-19 14:47:07.000000 sciveo-0.0.45/test/test_runner.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     9045 2024-03-19 14:47:24.000000 sciveo-0.0.45/test/test_sampling.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-14 08:57:35.724767 sciveo-0.0.46/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6168 2024-04-14 08:57:35.724595 sciveo-0.0.46/PKG-INFO
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6055 2024-04-10 20:04:28.000000 sciveo-0.0.46/README.md
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-14 08:57:35.702818 sciveo-0.0.46/sciveo/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1297 2024-04-13 06:50:59.000000 sciveo-0.0.46/sciveo/__init__.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-14 08:57:35.712092 sciveo-0.0.46/sciveo/api/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:04:12.000000 sciveo-0.0.46/sciveo/api/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1788 2024-04-07 18:52:23.000000 sciveo-0.0.46/sciveo/api/base.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1815 2024-04-05 16:37:24.000000 sciveo-0.0.46/sciveo/api/upload.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-14 08:57:35.714940 sciveo-0.0.46/sciveo/common/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:03:59.000000 sciveo-0.0.46/sciveo/common/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2043 2024-03-14 17:02:24.000000 sciveo-0.0.46/sciveo/common/configuration.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1583 2024-03-14 17:02:24.000000 sciveo-0.0.46/sciveo/common/model.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3842 2024-04-07 18:52:23.000000 sciveo-0.0.46/sciveo/common/optimizers.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)    10567 2024-03-19 14:47:24.000000 sciveo-0.0.46/sciveo/common/sampling.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-14 08:57:35.718237 sciveo-0.0.46/sciveo/common/tools/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:07:07.000000 sciveo-0.0.46/sciveo/common/tools/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1416 2024-04-13 06:51:43.000000 sciveo-0.0.46/sciveo/common/tools/daemon.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1053 2023-11-17 12:42:35.000000 sciveo-0.0.46/sciveo/common/tools/formating.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1654 2024-04-14 08:49:26.000000 sciveo-0.0.46/sciveo/common/tools/hardware.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1071 2023-11-15 15:21:05.000000 sciveo-0.0.46/sciveo/common/tools/logger.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1102 2023-12-10 07:08:19.000000 sciveo-0.0.46/sciveo/common/tools/synchronized.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-14 08:57:35.720799 sciveo-0.0.46/sciveo/content/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:14:23.000000 sciveo-0.0.46/sciveo/content/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      827 2024-03-14 17:02:24.000000 sciveo-0.0.46/sciveo/content/dataset.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     5859 2024-04-07 18:52:23.000000 sciveo-0.0.46/sciveo/content/experiment.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3129 2024-04-07 18:52:23.000000 sciveo-0.0.46/sciveo/content/project.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2015 2024-03-19 14:47:07.000000 sciveo-0.0.46/sciveo/content/runner.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-14 08:57:35.722396 sciveo-0.0.46/sciveo/monitoring/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2024-04-07 18:52:23.000000 sciveo-0.0.46/sciveo/monitoring/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3712 2024-04-14 08:55:29.000000 sciveo-0.0.46/sciveo/monitoring/monitor.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1440 2024-04-13 06:48:20.000000 sciveo-0.0.46/sciveo/monitoring/start.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       24 2024-04-14 08:54:39.000000 sciveo-0.0.46/sciveo/version.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-14 08:57:35.710812 sciveo-0.0.46/sciveo.egg-info/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6168 2024-04-14 08:57:35.000000 sciveo-0.0.46/sciveo.egg-info/PKG-INFO
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      906 2024-04-14 08:57:35.000000 sciveo-0.0.46/sciveo.egg-info/SOURCES.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        1 2024-04-14 08:57:35.000000 sciveo-0.0.46/sciveo.egg-info/dependency_links.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       50 2024-04-14 08:57:35.000000 sciveo-0.0.46/sciveo.egg-info/requires.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        7 2024-04-14 08:57:35.000000 sciveo-0.0.46/sciveo.egg-info/top_level.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       38 2024-04-14 08:57:35.724829 sciveo-0.0.46/setup.cfg
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      418 2024-04-07 18:52:23.000000 sciveo-0.0.46/setup.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-14 08:57:35.724217 sciveo-0.0.46/test/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      521 2024-03-14 17:02:24.000000 sciveo-0.0.46/test/test_configuration.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3256 2024-04-10 18:44:45.000000 sciveo-0.0.46/test/test_monitoring.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1554 2024-03-19 14:47:07.000000 sciveo-0.0.46/test/test_runner.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     9045 2024-03-19 14:47:24.000000 sciveo-0.0.46/test/test_sampling.py
```

### Comparing `sciveo-0.0.45/PKG-INFO` & `sciveo-0.0.46/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciveo
-Version: 0.0.45
+Version: 0.0.46
 Description-Content-Type: text/markdown
 Provides-Extra: mon
 
 # SCIVEO - ML/Scientific Experiments Management Client
 
 `sciveo` is a Python library that serves as a client for managing machine learning and scientific experiments on the sciveo.com platform. This library provides a convenient interface to interact with the sciveo.com API, enabling users to organize, track, and analyze their experiments efficiently.
 There are few configuration params samplers, which allows easy parameter tuning. The "auto" sampler perhaps is the easiest to use, but also
```

### Comparing `sciveo-0.0.45/README.md` & `sciveo-0.0.46/README.md`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.45/sciveo/__init__.py` & `sciveo-0.0.46/sciveo/__init__.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.45/sciveo/api/base.py` & `sciveo-0.0.46/sciveo/api/base.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.45/sciveo/api/upload.py` & `sciveo-0.0.46/sciveo/api/upload.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.45/sciveo/common/configuration.py` & `sciveo-0.0.46/sciveo/common/configuration.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.45/sciveo/common/model.py` & `sciveo-0.0.46/sciveo/common/model.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.45/sciveo/common/optimizers.py` & `sciveo-0.0.46/sciveo/common/optimizers.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.45/sciveo/common/sampling.py` & `sciveo-0.0.46/sciveo/common/sampling.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.45/sciveo/common/tools/daemon.py` & `sciveo-0.0.46/sciveo/common/tools/daemon.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.45/sciveo/common/tools/formating.py` & `sciveo-0.0.46/sciveo/common/tools/formating.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.45/sciveo/common/tools/hardware.py` & `sciveo-0.0.46/sciveo/common/tools/hardware.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,27 +28,33 @@
 
 def new_guid(num_characters=32):
   return datetime.datetime.now().strftime("%Y%m%d%H%M%S") + "-" + random_token(num_characters)
 
 
 class HardwareInfo:
   def __init__(self):
-    self.data = {
-      "CPU": {"count": os.cpu_count()},
-      "RAM": format_memory_size(os.sysconf('SC_PAGE_SIZE') * os.sysconf('SC_PHYS_PAGES'))
-    }
+    self.data = {}
 
     self.get_cpu()
+    self.get_ram()
 
   def __call__(self):
     return self.data
 
+  def get_ram(self):
+    try:
+      self.data["RAM"] = format_memory_size(os.sysconf('SC_PAGE_SIZE') * os.sysconf('SC_PHYS_PAGES'))
+    except Exception:
+      pass
+
   def get_cpu(self):
     list_keys = ["model name", "stepping", "cpu MHz", "cache size", "siblings", "cpu cores", "bogomips"]
     try:
+      self.data["CPU"] = {"count": os.cpu_count()}
+
       cpu_info = {}
       with open('/proc/cpuinfo', 'r') as file:
         lines = file.readlines()
 
       for line in lines:
         if ':' in line:
           key, value = map(str.strip, line.split(':', 1))
```

### Comparing `sciveo-0.0.45/sciveo/common/tools/logger.py` & `sciveo-0.0.46/sciveo/common/tools/logger.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.45/sciveo/common/tools/synchronized.py` & `sciveo-0.0.46/sciveo/common/tools/synchronized.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.45/sciveo/content/dataset.py` & `sciveo-0.0.46/sciveo/content/dataset.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.45/sciveo/content/experiment.py` & `sciveo-0.0.46/sciveo/content/experiment.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.45/sciveo/content/project.py` & `sciveo-0.0.46/sciveo/content/project.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.45/sciveo/content/runner.py` & `sciveo-0.0.46/sciveo/content/runner.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.45/sciveo/monitoring/monitor.py` & `sciveo-0.0.46/sciveo/monitoring/monitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,17 +27,15 @@
 
 class BaseMonitor(DaemonBase):
   def __init__(self, period=5):
     super().__init__(period=period)
 
     self.data = HardwareInfo()()
     self.data.setdefault("CPU", {})
-    self.data["RAM"] = {
-      "installed": self.data["RAM"]
-    }
+    self.data["RAM"] = {}
     self.data["LOG"] = {}
     self.list_logs = []
 
     self.api = APIRemoteClient()
 
     # Warmup the psutil cpu usage
     psutil.cpu_percent(interval=0.3, percpu=True)
@@ -73,14 +71,15 @@
     self.data["CPU"]["usage"] = np.array(usage_per_core).mean()
 
   def get_memory(self):
     memory = psutil.virtual_memory()
     self.data["RAM"]["used"] = memory.used
     self.data["RAM"]["total"] = memory.total
     self.data["RAM"]["free"] = memory.free
+    self.data["RAM"]["installed"] = format_memory_size(memory.total)
     self.data["RAM"]["print"] = f"total: {format_memory_size(memory.total)} used: {format_memory_size(memory.used)}"
 
   def getserial(self):
     machine_serial = None
     try:
       machine_serial = f"{socket.gethostname()}-{uuid.getnode()}"
     except Exception:
```

### Comparing `sciveo-0.0.45/sciveo/monitoring/start.py` & `sciveo-0.0.46/sciveo/monitoring/start.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.45/sciveo.egg-info/PKG-INFO` & `sciveo-0.0.46/sciveo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciveo
-Version: 0.0.45
+Version: 0.0.46
 Description-Content-Type: text/markdown
 Provides-Extra: mon
 
 # SCIVEO - ML/Scientific Experiments Management Client
 
 `sciveo` is a Python library that serves as a client for managing machine learning and scientific experiments on the sciveo.com platform. This library provides a convenient interface to interact with the sciveo.com API, enabling users to organize, track, and analyze their experiments efficiently.
 There are few configuration params samplers, which allows easy parameter tuning. The "auto" sampler perhaps is the easiest to use, but also
```

### Comparing `sciveo-0.0.45/sciveo.egg-info/SOURCES.txt` & `sciveo-0.0.46/sciveo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.45/test/test_configuration.py` & `sciveo-0.0.46/test/test_configuration.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.45/test/test_monitoring.py` & `sciveo-0.0.46/test/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.45/test/test_runner.py` & `sciveo-0.0.46/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.45/test/test_sampling.py` & `sciveo-0.0.46/test/test_sampling.py`

 * *Files identical despite different names*

