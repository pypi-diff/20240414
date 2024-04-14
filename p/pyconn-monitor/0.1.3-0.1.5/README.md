# Comparing `tmp/pyconn-monitor-0.1.3.tar.gz` & `tmp/pyconn-monitor-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyconn-monitor-0.1.3.tar", last modified: Sun Apr 14 15:38:36 2024, max compression
+gzip compressed data, was "pyconn-monitor-0.1.5.tar", last modified: Sun Apr 14 15:55:46 2024, max compression
```

## Comparing `pyconn-monitor-0.1.3.tar` & `pyconn-monitor-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 15:38:36.386783 pyconn-monitor-0.1.3/
--rw-rw-rw-   0        0        0    11558 2024-04-14 12:24:33.000000 pyconn-monitor-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     4759 2024-04-14 15:38:36.384789 pyconn-monitor-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3818 2024-04-14 15:15:44.000000 pyconn-monitor-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 15:38:36.364759 pyconn-monitor-0.1.3/pyconn_monitor/
--rw-rw-rw-   0        0        0      232 2024-04-14 12:26:06.000000 pyconn-monitor-0.1.3/pyconn_monitor/__init__.py
--rw-rw-rw-   0        0        0     2321 2024-04-14 15:00:35.000000 pyconn-monitor-0.1.3/pyconn_monitor/cli.py
--rw-rw-rw-   0        0        0     7037 2024-04-14 15:38:22.000000 pyconn-monitor-0.1.3/pyconn_monitor/connection_monitor.py
-drwxrwxrwx   0        0        0        0 2024-04-14 15:38:36.383782 pyconn-monitor-0.1.3/pyconn_monitor.egg-info/
--rw-rw-rw-   0        0        0     4759 2024-04-14 15:38:36.000000 pyconn-monitor-0.1.3/pyconn_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2024-04-14 15:38:36.000000 pyconn-monitor-0.1.3/pyconn_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 15:38:36.000000 pyconn-monitor-0.1.3/pyconn_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-04-14 15:38:36.000000 pyconn-monitor-0.1.3/pyconn_monitor.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2024-04-14 15:38:36.000000 pyconn-monitor-0.1.3/pyconn_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-14 15:38:36.000000 pyconn-monitor-0.1.3/pyconn_monitor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 15:38:36.386783 pyconn-monitor-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1354 2024-04-14 15:38:33.000000 pyconn-monitor-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-14 15:38:36.382783 pyconn-monitor-0.1.3/tests/
--rw-rw-rw-   0        0        0      182 2024-04-14 14:50:33.000000 pyconn-monitor-0.1.3/tests/test_connection_monitor.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:55:46.215424 pyconn-monitor-0.1.5/
+-rw-rw-rw-   0        0        0    11558 2024-04-14 12:24:33.000000 pyconn-monitor-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     4759 2024-04-14 15:55:46.213845 pyconn-monitor-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3818 2024-04-14 15:15:44.000000 pyconn-monitor-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 15:55:46.199272 pyconn-monitor-0.1.5/pyconn_monitor/
+-rw-rw-rw-   0        0        0      232 2024-04-14 12:26:06.000000 pyconn-monitor-0.1.5/pyconn_monitor/__init__.py
+-rw-rw-rw-   0        0        0     2321 2024-04-14 15:00:35.000000 pyconn-monitor-0.1.5/pyconn_monitor/cli.py
+-rw-rw-rw-   0        0        0     7119 2024-04-14 15:43:38.000000 pyconn-monitor-0.1.5/pyconn_monitor/connection_monitor.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:55:46.213308 pyconn-monitor-0.1.5/pyconn_monitor.egg-info/
+-rw-rw-rw-   0        0        0     4759 2024-04-14 15:55:45.000000 pyconn-monitor-0.1.5/pyconn_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2024-04-14 15:55:46.000000 pyconn-monitor-0.1.5/pyconn_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 15:55:45.000000 pyconn-monitor-0.1.5/pyconn_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-04-14 15:55:45.000000 pyconn-monitor-0.1.5/pyconn_monitor.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2024-04-14 15:55:45.000000 pyconn-monitor-0.1.5/pyconn_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-14 15:55:45.000000 pyconn-monitor-0.1.5/pyconn_monitor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 15:55:46.215424 pyconn-monitor-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1354 2024-04-14 15:41:26.000000 pyconn-monitor-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:55:46.211713 pyconn-monitor-0.1.5/tests/
+-rw-rw-rw-   0        0        0      182 2024-04-14 14:50:33.000000 pyconn-monitor-0.1.5/tests/test_connection_monitor.py
```

### Comparing `pyconn-monitor-0.1.3/LICENSE` & `pyconn-monitor-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyconn-monitor-0.1.3/PKG-INFO` & `pyconn-monitor-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyconn-monitor
-Version: 0.1.3
+Version: 0.1.5
 Summary: A Python library to monitor and log network connections of untrusted programs
 Home-page: https://github.com/ParisNeo/pyconn-monitor
 Author: ParisNeo
 Author-email: parisneoai@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyconn-monitor-0.1.3/README.md` & `pyconn-monitor-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pyconn-monitor-0.1.3/pyconn_monitor/cli.py` & `pyconn-monitor-0.1.5/pyconn_monitor/cli.py`

 * *Files identical despite different names*

### Comparing `pyconn-monitor-0.1.3/pyconn_monitor/connection_monitor.py` & `pyconn-monitor-0.1.5/pyconn_monitor/connection_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,36 +95,36 @@
                     # Get the current network connections for the process
                     current_connections = set((conn.laddr, conn.raddr, conn.status) for conn in process.connections())
 
                     # Log new connections
                     new_connections = current_connections - existing_connections
                     for laddr, raddr, status in new_connections:
                         if status == 'LISTEN':
-                            open_ports.append(laddr.port)
+                            open_ports.append(f"{laddr.port}")
                             log.write(f"Detected new local open port: {laddr.port}" + "\n")
-                            
-                        local_hostname, local_ipv4_addr, local_port_number = get_hostname_and_ipv4(laddr)
-                        local_infos = f"{local_hostname} ({local_ipv4_addr}):{local_port_number}"
-                        remote_hostname, remote_ipv4_addr, remote_port_number = get_hostname_and_ipv4(raddr)
-                        remote_infos = f"{remote_hostname} ({remote_ipv4_addr}):{remote_port_number}"
-                        # Determine the connection initiator
-                        if len(raddr)>0 and laddr == raddr[0]:
-                            initiator = "local"
-                        elif len(raddr)>0:
-                            initiator = "remote"  
                         else:
-                            initiator = "unknown"  
-                        # Skip logging for local to local connections if suppress_local is True
-                        if suppress_local and remote_ipv4_addr == local_ipv4_addr:
-                            continue                                             
-                        # Get the connection status
-                        timestamp = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
-                        log_entry = f"{timestamp}: initiator: {initiator}, status: {get_conn_status_str(status)}, local: {local_infos}, remote: {remote_infos}"
-                        ASCIIColors.red(log_entry)
-                        log.write(log_entry + "\n")
+                            local_hostname, local_ipv4_addr, local_port_number = get_hostname_and_ipv4(laddr)
+                            local_infos = f"{local_hostname} ({local_ipv4_addr}):{local_port_number}"
+                            remote_hostname, remote_ipv4_addr, remote_port_number = get_hostname_and_ipv4(raddr)
+                            remote_infos = f"{remote_hostname} ({remote_ipv4_addr}):{remote_port_number}"
+                            # Determine the connection initiator
+                            if len(raddr)>0 and laddr == raddr[0]:
+                                initiator = "local"
+                            elif len(raddr)>0:
+                                initiator = "remote"  
+                            else:
+                                initiator = "unknown"  
+                            # Skip logging for local to local connections if suppress_local is True
+                            if suppress_local and remote_ipv4_addr == local_ipv4_addr:
+                                continue                                             
+                            # Get the connection status
+                            timestamp = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
+                            log_entry = f"{timestamp}: initiator: {initiator}, status: {get_conn_status_str(status)}, local: {local_infos}, remote: {remote_infos}"
+                            ASCIIColors.red(log_entry)
+                            log.write(log_entry + "\n")
                         log.flush()
 
                     # Update the set of existing connections
                     existing_connections = current_connections
 
             except (psutil.NoSuchProcess, psutil.AccessDenied):
                 print(f"Process with pid {pid} has terminated or cannot be accessed.")
```

### Comparing `pyconn-monitor-0.1.3/pyconn_monitor.egg-info/PKG-INFO` & `pyconn-monitor-0.1.5/pyconn_monitor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyconn-monitor
-Version: 0.1.3
+Version: 0.1.5
 Summary: A Python library to monitor and log network connections of untrusted programs
 Home-page: https://github.com/ParisNeo/pyconn-monitor
 Author: ParisNeo
 Author-email: parisneoai@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyconn-monitor-0.1.3/setup.py` & `pyconn-monitor-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open('requirements.txt', 'r') as f:
     install_requires = f.read().splitlines()
 
 setup(
     name='pyconn-monitor',
-    version='0.1.3',
+    version='0.1.5',
     author='ParisNeo',
     author_email='parisneoai@gmail.com',
     description='A Python library to monitor and log network connections of untrusted programs',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ParisNeo/pyconn-monitor',
     packages=find_packages(),
```

