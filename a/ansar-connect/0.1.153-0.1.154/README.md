# Comparing `tmp/ansar_connect-0.1.153.tar.gz` & `tmp/ansar_connect-0.1.154.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.153.tar", last modified: Sun Apr 14 14:06:24 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.154.tar", last modified: Sun Apr 14 14:41:00 2024, max compression
```

## Comparing `ansar_connect-0.1.153.tar` & `ansar_connect-0.1.154.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 14:06:24.106085 ansar_connect-0.1.153/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.153/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-14 14:06:24.106085 ansar_connect-0.1.153/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.153/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar_connect-0.1.153/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-14 14:06:24.106085 ansar_connect-0.1.153/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar_connect-0.1.153/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 14:06:24.102085 ansar_connect-0.1.153/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 14:06:24.102085 ansar_connect-0.1.153/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 14:06:24.102085 ansar_connect-0.1.153/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar_connect-0.1.153/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar_connect-0.1.153/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.153/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar_connect-0.1.153/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 14:06:24.106085 ansar_connect-0.1.153/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3055 2024-04-14 14:06:20.000000 ansar_connect-0.1.153/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14167 2024-04-14 08:27:58.000000 ansar_connect-0.1.153/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    78025 2024-04-13 03:14:49.000000 ansar_connect-0.1.153/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.153/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.153/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar_connect-0.1.153/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.153/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.153/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.153/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.153/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.153/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.153/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar_connect-0.1.153/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar_connect-0.1.153/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    38666 2024-04-14 14:05:31.000000 ansar_connect-0.1.153/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.153/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2205 2024-04-14 02:42:33.000000 ansar_connect-0.1.153/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar_connect-0.1.153/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 14:06:24.106085 ansar_connect-0.1.153/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-14 14:06:24.000000 ansar_connect-0.1.153/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-14 14:06:24.000000 ansar_connect-0.1.153/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-14 14:06:24.000000 ansar_connect-0.1.153/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-14 14:06:24.000000 ansar_connect-0.1.153/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-14 14:06:24.000000 ansar_connect-0.1.153/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-14 14:06:24.000000 ansar_connect-0.1.153/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 14:41:00.501734 ansar_connect-0.1.154/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.154/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-14 14:41:00.501734 ansar_connect-0.1.154/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.154/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar_connect-0.1.154/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-14 14:41:00.501734 ansar_connect-0.1.154/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar_connect-0.1.154/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 14:41:00.501734 ansar_connect-0.1.154/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 14:41:00.501734 ansar_connect-0.1.154/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 14:41:00.501734 ansar_connect-0.1.154/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar_connect-0.1.154/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar_connect-0.1.154/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.154/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar_connect-0.1.154/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 14:41:00.501734 ansar_connect-0.1.154/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3055 2024-04-14 14:40:57.000000 ansar_connect-0.1.154/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14167 2024-04-14 08:27:58.000000 ansar_connect-0.1.154/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    78025 2024-04-13 03:14:49.000000 ansar_connect-0.1.154/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.154/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.154/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar_connect-0.1.154/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.154/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.154/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.154/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.154/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.154/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.154/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar_connect-0.1.154/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar_connect-0.1.154/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    38667 2024-04-14 14:39:54.000000 ansar_connect-0.1.154/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.154/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2205 2024-04-14 02:42:33.000000 ansar_connect-0.1.154/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar_connect-0.1.154/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 14:41:00.501734 ansar_connect-0.1.154/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-14 14:41:00.000000 ansar_connect-0.1.154/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-14 14:41:00.000000 ansar_connect-0.1.154/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-14 14:41:00.000000 ansar_connect-0.1.154/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-14 14:41:00.000000 ansar_connect-0.1.154/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-14 14:41:00.000000 ansar_connect-0.1.154/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-14 14:41:00.000000 ansar_connect-0.1.154/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.153/LICENSE` & `ansar_connect-0.1.154/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.153/PKG-INFO` & `ansar_connect-0.1.154/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.153
+Version: 0.1.154
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.153/README.md` & `ansar_connect-0.1.154/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.153/pyproject.toml` & `ansar_connect-0.1.154/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.153/setup.py` & `ansar_connect-0.1.154/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.153/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.154/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.153/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.154/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.153/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.154/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.153/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.154/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.153/src/ansar/connect/__init__.py` & `ansar_connect-0.1.154/src/ansar/connect/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 0105c349b14b556b6a4d77caaade00a23d8dfee0
-Version: 0.1.152 (2024-04-15@02:06:20+NZST)
+Commit: 0e0d17d684b5352bf1ed9e8885ffe3641a766a71
+Version: 0.1.153 (2024-04-15@02:40:57+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.153/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.154/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.153/src/ansar/connect/directory.py` & `ansar_connect-0.1.154/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.153/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.154/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.153/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.154/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.153/src/ansar/connect/group_if.py` & `ansar_connect-0.1.154/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.153/src/ansar/connect/grouping.py` & `ansar_connect-0.1.154/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.153/src/ansar/connect/moving.py` & `ansar_connect-0.1.154/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.153/src/ansar/connect/networking.py` & `ansar_connect-0.1.154/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.153/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.154/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.153/src/ansar/connect/node.py` & `ansar_connect-0.1.154/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.153/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.154/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.153/src/ansar/connect/procedure.py` & `ansar_connect-0.1.154/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.153/src/ansar/connect/product.py` & `ansar_connect-0.1.154/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.153/src/ansar/connect/socketry.py` & `ansar_connect-0.1.154/src/ansar/connect/socketry.py`

 * *Files 0% similar despite different names*

```diff
@@ -767,15 +767,15 @@
 	except socket.error as e:
 		self.send(NotConnected(requested_ipp, e.errno, str(e), m.tag), r)
 		return
 
 	if isinstance(m.encrypted, TlsClient):
 		context = ssl.create_default_context()
 		#context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
-		context.verify_mode = ssl.CERT_OPTIONAL
+		#context.verify_mode = ssl.CERT_OPTIONAL
 		client = context.wrap_socket(client, server_side=False, do_handshake_on_connect=False, server_hostname=m.encrypted.SNI)
 		self.trace(f'Encrypting as TLS client "{m.encrypted.SNI}"')
 
 	def client_not_connected(e):
 		client.close()
 		self.send(NotConnected(requested_ipp, e.errno, str(e), m.tag), r)
```

### Comparing `ansar_connect-0.1.153/src/ansar/connect/standard.py` & `ansar_connect-0.1.154/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.153/src/ansar/connect/transporting.py` & `ansar_connect-0.1.154/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.153/src/ansar/connect/wan.py` & `ansar_connect-0.1.154/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.153/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.154/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.153
+Version: 0.1.154
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.153/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.154/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

