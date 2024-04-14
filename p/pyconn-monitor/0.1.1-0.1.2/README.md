# Comparing `tmp/pyconn-monitor-0.1.1.tar.gz` & `tmp/pyconn-monitor-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyconn-monitor-0.1.1.tar", last modified: Sun Apr 14 15:19:22 2024, max compression
+gzip compressed data, was "pyconn-monitor-0.1.2.tar", last modified: Sun Apr 14 15:35:47 2024, max compression
```

## Comparing `pyconn-monitor-0.1.1.tar` & `pyconn-monitor-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 15:19:22.771501 pyconn-monitor-0.1.1/
--rw-rw-rw-   0        0        0    11558 2024-04-14 12:24:33.000000 pyconn-monitor-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     4759 2024-04-14 15:19:22.769501 pyconn-monitor-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3818 2024-04-14 15:15:44.000000 pyconn-monitor-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 15:19:22.746622 pyconn-monitor-0.1.1/pyconn_monitor/
--rw-rw-rw-   0        0        0      232 2024-04-14 12:26:06.000000 pyconn-monitor-0.1.1/pyconn_monitor/__init__.py
--rw-rw-rw-   0        0        0     2321 2024-04-14 15:00:35.000000 pyconn-monitor-0.1.1/pyconn_monitor/cli.py
--rw-rw-rw-   0        0        0     6625 2024-04-14 15:07:49.000000 pyconn-monitor-0.1.1/pyconn_monitor/connection_monitor.py
-drwxrwxrwx   0        0        0        0 2024-04-14 15:19:22.768506 pyconn-monitor-0.1.1/pyconn_monitor.egg-info/
--rw-rw-rw-   0        0        0     4759 2024-04-14 15:19:22.000000 pyconn-monitor-0.1.1/pyconn_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2024-04-14 15:19:22.000000 pyconn-monitor-0.1.1/pyconn_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 15:19:22.000000 pyconn-monitor-0.1.1/pyconn_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-04-14 15:19:22.000000 pyconn-monitor-0.1.1/pyconn_monitor.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2024-04-14 15:19:22.000000 pyconn-monitor-0.1.1/pyconn_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-14 15:19:22.000000 pyconn-monitor-0.1.1/pyconn_monitor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 15:19:22.771501 pyconn-monitor-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1354 2024-04-14 15:19:18.000000 pyconn-monitor-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-14 15:19:22.767503 pyconn-monitor-0.1.1/tests/
--rw-rw-rw-   0        0        0      182 2024-04-14 14:50:33.000000 pyconn-monitor-0.1.1/tests/test_connection_monitor.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:35:47.455040 pyconn-monitor-0.1.2/
+-rw-rw-rw-   0        0        0    11558 2024-04-14 12:24:33.000000 pyconn-monitor-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     4759 2024-04-14 15:35:47.453533 pyconn-monitor-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3818 2024-04-14 15:15:44.000000 pyconn-monitor-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 15:35:47.433506 pyconn-monitor-0.1.2/pyconn_monitor/
+-rw-rw-rw-   0        0        0      232 2024-04-14 12:26:06.000000 pyconn-monitor-0.1.2/pyconn_monitor/__init__.py
+-rw-rw-rw-   0        0        0     2321 2024-04-14 15:00:35.000000 pyconn-monitor-0.1.2/pyconn_monitor/cli.py
+-rw-rw-rw-   0        0        0     6874 2024-04-14 15:35:39.000000 pyconn-monitor-0.1.2/pyconn_monitor/connection_monitor.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:35:47.452533 pyconn-monitor-0.1.2/pyconn_monitor.egg-info/
+-rw-rw-rw-   0        0        0     4759 2024-04-14 15:35:47.000000 pyconn-monitor-0.1.2/pyconn_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2024-04-14 15:35:47.000000 pyconn-monitor-0.1.2/pyconn_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 15:35:47.000000 pyconn-monitor-0.1.2/pyconn_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-04-14 15:35:47.000000 pyconn-monitor-0.1.2/pyconn_monitor.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2024-04-14 15:35:47.000000 pyconn-monitor-0.1.2/pyconn_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-14 15:35:47.000000 pyconn-monitor-0.1.2/pyconn_monitor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 15:35:47.455040 pyconn-monitor-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1354 2024-04-14 15:35:43.000000 pyconn-monitor-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:35:47.450525 pyconn-monitor-0.1.2/tests/
+-rw-rw-rw-   0        0        0      182 2024-04-14 14:50:33.000000 pyconn-monitor-0.1.2/tests/test_connection_monitor.py
```

### Comparing `pyconn-monitor-0.1.1/LICENSE` & `pyconn-monitor-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyconn-monitor-0.1.1/PKG-INFO` & `pyconn-monitor-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyconn-monitor
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library to monitor and log network connections of untrusted programs
 Home-page: https://github.com/ParisNeo/pyconn-monitor
 Author: ParisNeo
 Author-email: parisneoai@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyconn-monitor-0.1.1/README.md` & `pyconn-monitor-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyconn-monitor-0.1.1/pyconn_monitor/cli.py` & `pyconn-monitor-0.1.2/pyconn_monitor/cli.py`

 * *Files identical despite different names*

### Comparing `pyconn-monitor-0.1.1/pyconn_monitor/connection_monitor.py` & `pyconn-monitor-0.1.2/pyconn_monitor/connection_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,27 +81,31 @@
             print(f"Process found with pid {pid}!")
             process_found = True
         else:
             time.sleep(interval)
 
     print("Starting to monitor new network connections...")
     existing_connections = set()
-
+    open_ports = []
     with open(log_file, "a", encoding="utf-8") as log:
         log.write(f"Connections test log file\n")
         log.write(f"Testing program {process.cmdline()} with pid: {process.pid}\n" )
         while True:
             try:
                     
                     # Get the current network connections for the process
                     current_connections = set((conn.laddr, conn.raddr, conn.status) for conn in process.connections())
 
                     # Log new connections
                     new_connections = current_connections - existing_connections
                     for laddr, raddr, status in new_connections:
+                        if status == 'LISTEN':
+                            open_ports.append(laddr.port)
+                            log.write(f"Detected new local open port: {laddr.port}" + "\n")
+                            
                         local_hostname, local_ipv4_addr, local_port_number = get_hostname_and_ipv4(laddr)
                         local_infos = f"{local_hostname} ({local_ipv4_addr}):{local_port_number}"
                         remote_hostname, remote_ipv4_addr, remote_port_number = get_hostname_and_ipv4(raddr)
                         remote_infos = f"{remote_hostname} ({remote_ipv4_addr}):{remote_port_number}"
                         # Determine the connection initiator
                         if len(raddr)>0 and laddr == raddr[0]:
                             initiator = "local"
```

### Comparing `pyconn-monitor-0.1.1/pyconn_monitor.egg-info/PKG-INFO` & `pyconn-monitor-0.1.2/pyconn_monitor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyconn-monitor
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library to monitor and log network connections of untrusted programs
 Home-page: https://github.com/ParisNeo/pyconn-monitor
 Author: ParisNeo
 Author-email: parisneoai@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyconn-monitor-0.1.1/setup.py` & `pyconn-monitor-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open('requirements.txt', 'r') as f:
     install_requires = f.read().splitlines()
 
 setup(
     name='pyconn-monitor',
-    version='0.1.1',
+    version='0.1.2',
     author='ParisNeo',
     author_email='parisneoai@gmail.com',
     description='A Python library to monitor and log network connections of untrusted programs',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ParisNeo/pyconn-monitor',
     packages=find_packages(),
```

