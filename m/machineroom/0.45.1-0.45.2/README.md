# Comparing `tmp/machineroom-0.45.1.tar.gz` & `tmp/machineroom-0.45.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "machineroom-0.45.1.tar", last modified: Sat Apr 13 17:13:32 2024, max compression
+gzip compressed data, was "machineroom-0.45.2.tar", last modified: Sat Apr 13 18:03:27 2024, max compression
```

## Comparing `machineroom-0.45.1.tar` & `machineroom-0.45.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-13 17:13:32.539594 machineroom-0.45.1/
--rw-r--r--   0 root         (0) staff       (20)     2358 2024-02-29 11:53:06.000000 machineroom-0.45.1/.gitignore
--rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 machineroom-0.45.1/LICENSE
--rw-r--r--   0 root         (0) staff       (20)     4392 2024-04-13 17:13:32.539328 machineroom-0.45.1/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     3597 2024-02-29 11:21:25.000000 machineroom-0.45.1/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-13 17:13:32.528636 machineroom-0.45.1/cmdbin/
--rw-r--r--   0 root         (0) staff       (20)      586 2024-02-29 11:48:22.000000 machineroom-0.45.1/cmdbin/connect
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-13 17:13:32.535496 machineroom-0.45.1/machineroom/
--rw-r--r--   0 root         (0) staff       (20)     1301 2024-04-13 17:13:32.000000 machineroom-0.45.1/machineroom/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     7488 2024-04-13 17:01:00.000000 machineroom-0.45.1/machineroom/const.py
--rw-r--r--   0 root         (0) staff       (20)      996 2024-03-01 05:35:23.000000 machineroom-0.45.1/machineroom/schema.json
--rw-r--r--   0 root         (0) staff       (20)    13510 2024-04-13 15:24:08.000000 machineroom-0.45.1/machineroom/sql.py
--rw-r--r--   0 root         (0) staff       (20)    22572 2024-04-13 17:12:48.000000 machineroom-0.45.1/machineroom/taskbase.py
--rw-r--r--   0 root         (0) staff       (20)    14368 2024-04-08 17:07:54.000000 machineroom-0.45.1/machineroom/util.py
--rw-r--r--   0 root         (0) staff       (20)     2759 2024-03-23 02:51:57.000000 machineroom-0.45.1/machineroom/worker.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-13 17:13:32.538606 machineroom-0.45.1/machineroom.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     4392 2024-04-13 17:13:32.000000 machineroom-0.45.1/machineroom.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      371 2024-04-13 17:13:32.000000 machineroom-0.45.1/machineroom.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-04-13 17:13:32.000000 machineroom-0.45.1/machineroom.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       12 2024-04-13 17:13:32.000000 machineroom-0.45.1/machineroom.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       79 2024-04-13 17:13:32.540535 machineroom-0.45.1/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     2569 2024-03-01 08:09:46.000000 machineroom-0.45.1/setup.py
--rw-r--r--   0 root         (0) staff       (20)     1532 2024-04-13 11:13:43.000000 machineroom-0.45.1/update
--rw-r--r--   0 root         (0) staff       (20)        7 2024-04-13 17:13:20.000000 machineroom-0.45.1/version
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-13 18:03:27.972213 machineroom-0.45.2/
+-rw-r--r--   0 root         (0) staff       (20)     2358 2024-02-29 11:53:06.000000 machineroom-0.45.2/.gitignore
+-rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 machineroom-0.45.2/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)     4392 2024-04-13 18:03:27.971971 machineroom-0.45.2/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     3597 2024-02-29 11:21:25.000000 machineroom-0.45.2/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-13 18:03:27.960189 machineroom-0.45.2/cmdbin/
+-rw-r--r--   0 root         (0) staff       (20)      586 2024-02-29 11:48:22.000000 machineroom-0.45.2/cmdbin/connect
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-13 18:03:27.968225 machineroom-0.45.2/machineroom/
+-rw-r--r--   0 root         (0) staff       (20)     1301 2024-04-13 18:03:27.000000 machineroom-0.45.2/machineroom/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     7516 2024-04-13 18:03:05.000000 machineroom-0.45.2/machineroom/const.py
+-rw-r--r--   0 root         (0) staff       (20)      996 2024-03-01 05:35:23.000000 machineroom-0.45.2/machineroom/schema.json
+-rw-r--r--   0 root         (0) staff       (20)    13510 2024-04-13 15:24:08.000000 machineroom-0.45.2/machineroom/sql.py
+-rw-r--r--   0 root         (0) staff       (20)    22749 2024-04-13 18:03:05.000000 machineroom-0.45.2/machineroom/taskbase.py
+-rw-r--r--   0 root         (0) staff       (20)    14368 2024-04-08 17:07:54.000000 machineroom-0.45.2/machineroom/util.py
+-rw-r--r--   0 root         (0) staff       (20)     2759 2024-03-23 02:51:57.000000 machineroom-0.45.2/machineroom/worker.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-13 18:03:27.971163 machineroom-0.45.2/machineroom.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     4392 2024-04-13 18:03:27.000000 machineroom-0.45.2/machineroom.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      371 2024-04-13 18:03:27.000000 machineroom-0.45.2/machineroom.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-04-13 18:03:27.000000 machineroom-0.45.2/machineroom.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       12 2024-04-13 18:03:27.000000 machineroom-0.45.2/machineroom.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       79 2024-04-13 18:03:27.972827 machineroom-0.45.2/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     2569 2024-03-01 08:09:46.000000 machineroom-0.45.2/setup.py
+-rw-r--r--   0 root         (0) staff       (20)     1532 2024-04-13 11:13:43.000000 machineroom-0.45.2/update
+-rw-r--r--   0 root         (0) staff       (20)        7 2024-04-13 18:03:19.000000 machineroom-0.45.2/version
```

### Comparing `machineroom-0.45.1/.gitignore` & `machineroom-0.45.2/.gitignore`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.1/LICENSE` & `machineroom-0.45.2/LICENSE`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.1/PKG-INFO` & `machineroom-0.45.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineroom
-Version: 0.45.1
+Version: 0.45.2
 Summary: A Python package to manage all my machines in the fingertip.
 Home-page: https://github.com/jjhesk/mymachineroom/
 Author: Jun-You Liu & Heskemo
 Author-email: meowmeow@gmail.com
 License: MIT
 Keywords: ssh machine room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `machineroom-0.45.1/README.md` & `machineroom-0.45.2/README.md`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.1/cmdbin/connect` & `machineroom-0.45.2/cmdbin/connect`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.1/machineroom/__init__.py` & `machineroom-0.45.2/machineroom/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 logger5 = logging.getLogger("invoke")
 logger2.setLevel(logging.ERROR)
 logger1.setLevel(logging.ERROR)
 logger3.setLevel(logging.ERROR)
 logger4.setLevel(logging.ERROR)
 logger5.setLevel(logging.ERROR)
 
-__version__ = '0.45.1'
+__version__ = '0.45.2'
```

### Comparing `machineroom-0.45.1/machineroom/const.py` & `machineroom-0.45.2/machineroom/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,12 +219,12 @@
 if [ -f "$configuration_yaml_xsh" ]; then
     echo "$configuration_yaml_xsh is a file."
 else
     echo "$configuration_yaml_xsh is not a file."
     echo "wait until you have the correct configuration file install first."
     exit;
 fi
-
+cd /home/clashperfectoctopus
 echo "start up the service"
 bash clash_up.sh
 
 """
```

### Comparing `machineroom-0.45.1/machineroom/schema.json` & `machineroom-0.45.2/machineroom/schema.json`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.1/machineroom/sql.py` & `machineroom-0.45.2/machineroom/sql.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.1/machineroom/taskbase.py` & `machineroom-0.45.2/machineroom/taskbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -443,29 +443,38 @@
         selector: str,
         tst_endpoint: str
 ):
     # network config is yaml file format
     docker_file = DOCKER_COMPOSE_XCLASH \
         .replace("X_CLASH_CONFIG_YAML_NM", network_config_file) \
         .replace("X_CLASH_GALXE_HELPER_VER", "1.2.1291" if helper_version == "" else helper_version)
+
+
+    processed_selector = selector.encode('utf-16', 'surrogatepass').decode(
+        'utf-16').encode("raw_unicode_escape").decode("utf-8")
+
     resrc = CLASH_HELPER_RESOURCE \
         .replace("___SECRET___", external_token_access) \
-        .replace("___SELECTOR___", selector).replace(
+        .replace("___SELECTOR___", processed_selector).replace(
         "__TEST_ENDPOINT__", tst_endpoint)
-    network_cfg = os.path.join("home", "clashperfectoctopus", "clash_conf", network_config_file)
+
+    network_cfg = os.path.join("/home", "clashperfectoctopus", "clash_conf", network_config_file)
     network_cfg_local = os.path.join(Config.DATAPATH_BASE, "clash_config", network_config_file)
     content = CLASH_SETUP_1 \
         .replace("_CONTENT_DOCKER_COMPOSE", docker_file) \
         .replace("_RESOURCE_JSON", resrc)
+
     exec_shell_program(c, "/tmp", content)
     if os.path.isfile(network_cfg_local) is False:
         print("aborted the network config file is not found from", network_cfg_local)
         return
-    ensure_path_exist()
-    c.put(network_cfg_local, network_cfg)
+
+    if exists(c, network_cfg) is False:
+        c.put(network_cfg_local, network_cfg)
+
     content2 = CLASH_SETUP_2 \
         .replace("_PATH_CLASH", network_cfg)
     exec_shell_program(c, "/tmp", content2)
 
 
 class DeploymentBotFoundation:
     # the text file servers that recorded the authentications and some basic information
```

### Comparing `machineroom-0.45.1/machineroom/util.py` & `machineroom-0.45.2/machineroom/util.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.1/machineroom/worker.py` & `machineroom-0.45.2/machineroom/worker.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.1/machineroom.egg-info/PKG-INFO` & `machineroom-0.45.2/machineroom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineroom
-Version: 0.45.1
+Version: 0.45.2
 Summary: A Python package to manage all my machines in the fingertip.
 Home-page: https://github.com/jjhesk/mymachineroom/
 Author: Jun-You Liu & Heskemo
 Author-email: meowmeow@gmail.com
 License: MIT
 Keywords: ssh machine room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `machineroom-0.45.1/setup.py` & `machineroom-0.45.2/setup.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.1/update` & `machineroom-0.45.2/update`

 * *Files identical despite different names*

