# Comparing `tmp/ansar_connect-0.1.159.tar.gz` & `tmp/ansar_connect-0.1.160.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.159.tar", last modified: Sun Apr 14 15:23:59 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.160.tar", last modified: Sun Apr 14 16:03:51 2024, max compression
```

## Comparing `ansar_connect-0.1.159.tar` & `ansar_connect-0.1.160.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 15:23:59.789293 ansar_connect-0.1.159/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.159/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-14 15:23:59.789293 ansar_connect-0.1.159/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.159/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar_connect-0.1.159/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-14 15:23:59.789293 ansar_connect-0.1.159/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar_connect-0.1.159/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 15:23:59.785293 ansar_connect-0.1.159/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 15:23:59.785293 ansar_connect-0.1.159/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 15:23:59.785293 ansar_connect-0.1.159/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar_connect-0.1.159/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar_connect-0.1.159/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.159/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar_connect-0.1.159/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 15:23:59.785293 ansar_connect-0.1.159/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3055 2024-04-14 15:23:56.000000 ansar_connect-0.1.159/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14167 2024-04-14 15:15:11.000000 ansar_connect-0.1.159/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    78025 2024-04-13 03:14:49.000000 ansar_connect-0.1.159/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.159/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.159/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar_connect-0.1.159/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.159/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.159/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.159/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.159/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.159/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.159/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar_connect-0.1.159/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar_connect-0.1.159/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    38767 2024-04-14 15:20:34.000000 ansar_connect-0.1.159/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.159/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2205 2024-04-14 02:42:33.000000 ansar_connect-0.1.159/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar_connect-0.1.159/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 15:23:59.789293 ansar_connect-0.1.159/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-14 15:23:59.000000 ansar_connect-0.1.159/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-14 15:23:59.000000 ansar_connect-0.1.159/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-14 15:23:59.000000 ansar_connect-0.1.159/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-14 15:23:59.000000 ansar_connect-0.1.159/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-14 15:23:59.000000 ansar_connect-0.1.159/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-14 15:23:59.000000 ansar_connect-0.1.159/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 16:03:51.526149 ansar_connect-0.1.160/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.160/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-14 16:03:51.526149 ansar_connect-0.1.160/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.160/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar_connect-0.1.160/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-14 16:03:51.526149 ansar_connect-0.1.160/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar_connect-0.1.160/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 16:03:51.522149 ansar_connect-0.1.160/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 16:03:51.522149 ansar_connect-0.1.160/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 16:03:51.522149 ansar_connect-0.1.160/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar_connect-0.1.160/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar_connect-0.1.160/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.160/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar_connect-0.1.160/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 16:03:51.526149 ansar_connect-0.1.160/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3055 2024-04-14 16:03:48.000000 ansar_connect-0.1.160/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14167 2024-04-14 15:15:11.000000 ansar_connect-0.1.160/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    78025 2024-04-13 03:14:49.000000 ansar_connect-0.1.160/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.160/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.160/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar_connect-0.1.160/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.160/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.160/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.160/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.160/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.160/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.160/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar_connect-0.1.160/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar_connect-0.1.160/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    38783 2024-04-14 16:02:47.000000 ansar_connect-0.1.160/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.160/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2205 2024-04-14 02:42:33.000000 ansar_connect-0.1.160/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar_connect-0.1.160/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 16:03:51.526149 ansar_connect-0.1.160/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-14 16:03:51.000000 ansar_connect-0.1.160/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-14 16:03:51.000000 ansar_connect-0.1.160/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-14 16:03:51.000000 ansar_connect-0.1.160/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-14 16:03:51.000000 ansar_connect-0.1.160/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-14 16:03:51.000000 ansar_connect-0.1.160/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-14 16:03:51.000000 ansar_connect-0.1.160/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.159/LICENSE` & `ansar_connect-0.1.160/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.159/PKG-INFO` & `ansar_connect-0.1.160/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.159
+Version: 0.1.160
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.159/README.md` & `ansar_connect-0.1.160/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.159/pyproject.toml` & `ansar_connect-0.1.160/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.159/setup.py` & `ansar_connect-0.1.160/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.159/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.160/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.159/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.160/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.159/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.160/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.159/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.160/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.159/src/ansar/connect/__init__.py` & `ansar_connect-0.1.160/src/ansar/connect/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 9e01b36cb1697f613df52ae9a7c74e93ef8f0c06
-Version: 0.1.158 (2024-04-15@03:23:56+NZST)
+Commit: bcceeb8bbe9d750e84492a489565dc7c13084929
+Version: 0.1.159 (2024-04-15@04:03:48+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.159/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.160/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.159/src/ansar/connect/directory.py` & `ansar_connect-0.1.160/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.159/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.160/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.159/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.160/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.159/src/ansar/connect/group_if.py` & `ansar_connect-0.1.160/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.159/src/ansar/connect/grouping.py` & `ansar_connect-0.1.160/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.159/src/ansar/connect/moving.py` & `ansar_connect-0.1.160/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.159/src/ansar/connect/networking.py` & `ansar_connect-0.1.160/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.159/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.160/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.159/src/ansar/connect/node.py` & `ansar_connect-0.1.160/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.159/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.160/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.159/src/ansar/connect/procedure.py` & `ansar_connect-0.1.160/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.159/src/ansar/connect/product.py` & `ansar_connect-0.1.160/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.159/src/ansar/connect/socketry.py` & `ansar_connect-0.1.160/src/ansar/connect/socketry.py`

 * *Files 0% similar despite different names*

```diff
@@ -672,14 +672,15 @@
 
 def ControlChannel_BrokenTransport(self, control, s):
 	self.fault('The control channel to the selector is broken.')
 	self.clear(s, ControlChannel)
 
 # The rest of them handle the simulated receive of the
 # actual message.
+ListenForStream
 def ControlChannel_ListenForStream(self, control, mr):
 	m, r = mr
 	requested_ipp = m.requested_ipp
 	try:
 		server = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 	except socket.error as e:
 		self.send(NotListening(requested_ipp, e.errno, str(e), m.tag), r)
@@ -706,15 +707,15 @@
 	except OverflowError as e:
 		server.close()
 		self.send(NotListening(requested_ipp, 0, str(e), m.tag), r)
 		return
 
 	hap = server.getsockname()
 
-	if isinstance(m.encrypted, TcpServer):
+	if isinstance(m.encrypted, TlsServer):
 		context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
 		context.load_cert_chain(m.encrypted.certificate_file, keyfile=m.encrypted.key_file)
 		self.trace(f'Encrypting as TLS server "{m.encrypted.certificate_file}"')
 		server = context.wrap_socket(server, server_side=True, do_handshake_on_connect=False)
 	else:
 		context = None
```

### Comparing `ansar_connect-0.1.159/src/ansar/connect/standard.py` & `ansar_connect-0.1.160/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.159/src/ansar/connect/transporting.py` & `ansar_connect-0.1.160/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.159/src/ansar/connect/wan.py` & `ansar_connect-0.1.160/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.159/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.160/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.159
+Version: 0.1.160
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.159/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.160/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

