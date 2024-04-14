# Comparing `tmp/ansar_connect-0.1.154.tar.gz` & `tmp/ansar_connect-0.1.156.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.154.tar", last modified: Sun Apr 14 14:41:00 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.156.tar", last modified: Sun Apr 14 15:03:29 2024, max compression
```

## Comparing `ansar_connect-0.1.154.tar` & `ansar_connect-0.1.156.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 14:41:00.501734 ansar_connect-0.1.154/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.154/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-14 14:41:00.501734 ansar_connect-0.1.154/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.154/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar_connect-0.1.154/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-14 14:41:00.501734 ansar_connect-0.1.154/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar_connect-0.1.154/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 14:41:00.501734 ansar_connect-0.1.154/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 14:41:00.501734 ansar_connect-0.1.154/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 14:41:00.501734 ansar_connect-0.1.154/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar_connect-0.1.154/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar_connect-0.1.154/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.154/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar_connect-0.1.154/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 14:41:00.501734 ansar_connect-0.1.154/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3055 2024-04-14 14:40:57.000000 ansar_connect-0.1.154/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14167 2024-04-14 08:27:58.000000 ansar_connect-0.1.154/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    78025 2024-04-13 03:14:49.000000 ansar_connect-0.1.154/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.154/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.154/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar_connect-0.1.154/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.154/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.154/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.154/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.154/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.154/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.154/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar_connect-0.1.154/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar_connect-0.1.154/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    38667 2024-04-14 14:39:54.000000 ansar_connect-0.1.154/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.154/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2205 2024-04-14 02:42:33.000000 ansar_connect-0.1.154/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar_connect-0.1.154/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 14:41:00.501734 ansar_connect-0.1.154/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-14 14:41:00.000000 ansar_connect-0.1.154/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-14 14:41:00.000000 ansar_connect-0.1.154/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-14 14:41:00.000000 ansar_connect-0.1.154/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-14 14:41:00.000000 ansar_connect-0.1.154/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-14 14:41:00.000000 ansar_connect-0.1.154/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-14 14:41:00.000000 ansar_connect-0.1.154/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 15:03:29.793143 ansar_connect-0.1.156/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.156/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-14 15:03:29.793143 ansar_connect-0.1.156/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.156/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar_connect-0.1.156/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-14 15:03:29.793143 ansar_connect-0.1.156/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar_connect-0.1.156/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 15:03:29.793143 ansar_connect-0.1.156/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 15:03:29.793143 ansar_connect-0.1.156/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 15:03:29.793143 ansar_connect-0.1.156/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar_connect-0.1.156/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar_connect-0.1.156/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.156/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar_connect-0.1.156/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 15:03:29.793143 ansar_connect-0.1.156/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3051 2024-04-14 15:03:26.000000 ansar_connect-0.1.156/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14142 2024-04-14 15:00:38.000000 ansar_connect-0.1.156/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    78025 2024-04-13 03:14:49.000000 ansar_connect-0.1.156/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.156/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.156/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar_connect-0.1.156/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.156/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.156/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.156/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.156/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.156/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.156/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar_connect-0.1.156/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar_connect-0.1.156/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    38262 2024-04-14 15:00:38.000000 ansar_connect-0.1.156/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.156/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2205 2024-04-14 02:42:33.000000 ansar_connect-0.1.156/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar_connect-0.1.156/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-14 15:03:29.793143 ansar_connect-0.1.156/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-14 15:03:29.000000 ansar_connect-0.1.156/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-14 15:03:29.000000 ansar_connect-0.1.156/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-14 15:03:29.000000 ansar_connect-0.1.156/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-14 15:03:29.000000 ansar_connect-0.1.156/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-14 15:03:29.000000 ansar_connect-0.1.156/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-14 15:03:29.000000 ansar_connect-0.1.156/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.154/LICENSE` & `ansar_connect-0.1.156/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.154/PKG-INFO` & `ansar_connect-0.1.156/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.154
+Version: 0.1.156
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.154/README.md` & `ansar_connect-0.1.156/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.154/pyproject.toml` & `ansar_connect-0.1.156/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.154/setup.py` & `ansar_connect-0.1.156/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.154/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.156/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.154/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.156/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.154/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.156/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.154/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.156/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.154/src/ansar/connect/__init__.py` & `ansar_connect-0.1.156/src/ansar/connect/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
-Branch: main
-Commit: 0e0d17d684b5352bf1ed9e8885ffe3641a766a71
-Version: 0.1.153 (2024-04-15@02:40:57+NZST)
+Branch: 
+Commit: 86f8c043401c5029f0265ff7414d615c43bc61f6
+Version: 0.1.155 (2024-04-15@03:03:26+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.154/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.156/src/ansar/connect/connect_directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 class INITIAL: pass
 class DISABLED: pass
 class PENDING: pass
 class CONNECTED: pass
 class PRODUCING: pass
 class GLANCING: pass
 class CLOUDY: pass
-class INTERRUPTION: pass
 class LOOKING: pass
 class RECONNECTING: pass
 class GLARING: pass
 class CONNECTING: pass
 class REDIRECTING: pass
 class ASSIGNING: pass
 class CLOSING: pass
```

### Comparing `ansar_connect-0.1.154/src/ansar/connect/directory.py` & `ansar_connect-0.1.156/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.154/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.156/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.154/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.156/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.154/src/ansar/connect/group_if.py` & `ansar_connect-0.1.156/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.154/src/ansar/connect/grouping.py` & `ansar_connect-0.1.156/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.154/src/ansar/connect/moving.py` & `ansar_connect-0.1.156/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.154/src/ansar/connect/networking.py` & `ansar_connect-0.1.156/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.154/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.156/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.154/src/ansar/connect/node.py` & `ansar_connect-0.1.156/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.154/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.156/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.154/src/ansar/connect/procedure.py` & `ansar_connect-0.1.156/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.154/src/ansar/connect/product.py` & `ansar_connect-0.1.156/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.154/src/ansar/connect/socketry.py` & `ansar_connect-0.1.156/src/ansar/connect/socketry.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,19 +159,19 @@
 
 class StopListening(object):
 	def __init__(self, listening_ipp=None):
 		self.listening_ipp = listening_ipp or HostPort()
 
 # Update messages from sockets thread to app.
 class Listening(object):
-	def __init__(self, requested_ipp=None, listening_ipp=None, tag=None, encrypted=None):
+	def __init__(self, requested_ipp=None, listening_ipp=None, tag=None, context=None):
 		self.requested_ipp = requested_ipp or HostPort()
 		self.listening_ipp = listening_ipp or HostPort()
 		self.tag = tag
-		self.encrypted = encrypted
+		self.context = context
 
 class Accepted(object):
 	def __init__(self, listening_ipp=None, accepted_ipp=None, remote_address=None, opened_at=None, tag=None):
 		self.listening_ipp = listening_ipp or HostPort()
 		self.accepted_ipp = accepted_ipp or HostPort()
 		self.remote_address = remote_address
 		self.opened_at = opened_at
@@ -230,14 +230,15 @@
 	'listening_ipp': ar.UserDefined(HostPort),
 	'accepted_ipp': ar.UserDefined(HostPort),
 	'condition': ar.Unicode(),
 	'explanation': ar.Unicode(),
 	'error_code': ar.Integer8(),
 	'error_text': ar.Unicode(),
 	'encrypted': ar.Any(),
+	'context': ar.Any(),
 }
 
 ar.bind(ListenForStream, object_schema=CONTROL_SCHEMA)
 ar.bind(ConnectStream, object_schema=CONTROL_SCHEMA)
 ar.bind(StopListening, object_schema=CONTROL_SCHEMA)
 ar.bind(Listening, object_schema=CONTROL_SCHEMA, copy_before_sending=False)
 ar.bind(Accepted, object_schema=CONTROL_SCHEMA)
@@ -706,24 +707,25 @@
 	except OverflowError as e:
 		server.close()
 		self.send(NotListening(requested_ipp, 0, str(e), m.tag), r)
 		return
 
 	hap = server.getsockname()
 
-	if isinstance(m.encrypted, TcpServer):
-		context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
-		context.load_cert_chain(m.encrypted.certificate_file, keyfile=m.encrypted.key_file)
-		self.trace(f'Encrypting as TLS server "{m.encrypted.certificate_file}"')
-		server = context.wrap_socket(server, server_side=True, do_handshake_on_connect=False)
-
 	self.trace('Listening on "%s"(%d), requested "%s"(%d)' %
 		(hap[0], hap[1],
 		requested_ipp.host, requested_ipp.port))
-	listening = Listening(requested_ipp=requested_ipp, listening_ipp=HostPort(hap[0], hap[1]), tag=m.tag, encrypted=m.encrypted)
+
+	if isinstance(m.encrypted, TlsServer):
+		context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
+		context.load_cert_chain(m.encrypted.certificate_file, keyfile=m.encrypted.key_file)
+		self.trace(f'Encrypting as TLS server "{m.encrypted.certificate_file}"')
+	else:
+		context = None
+	listening = Listening(requested_ipp=requested_ipp, listening_ipp=HostPort(hap[0], hap[1]), tag=m.tag, context=context)
 
 	self.networking[server] = TcpServer(server, m, listening, r, m.upgrade)
 	self.receiving.append(server)
 	self.faulting.append(server)
 
 	self.send(listening, r)
 
@@ -766,16 +768,14 @@
 		client.setblocking(False)
 	except socket.error as e:
 		self.send(NotConnected(requested_ipp, e.errno, str(e), m.tag), r)
 		return
 
 	if isinstance(m.encrypted, TlsClient):
 		context = ssl.create_default_context()
-		#context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
-		#context.verify_mode = ssl.CERT_OPTIONAL
 		client = context.wrap_socket(client, server_side=False, do_handshake_on_connect=False, server_hostname=m.encrypted.SNI)
 		self.trace(f'Encrypting as TLS client "{m.encrypted.SNI}"')
 
 	def client_not_connected(e):
 		client.close()
 		self.send(NotConnected(requested_ipp, e.errno, str(e), m.tag), r)
 
@@ -916,19 +916,16 @@
 	try:
 		accepted, hap = s.accept()
 		accepted.setblocking(False)
 	except socket.error as e:
 		self.send(NotAccepted(listening.requested_ipp, e.errno, str(e), listening.tag), server.controller_address)
 		return
 
-	if isinstance(listening.encrypted, TlsServer):
-		#context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
-		#context.load_cert_chain(listening.encrypted.certificate_file, keyfile=listening.encrypted.key_file)
-		self.trace(f'Encrypting as TLS server "{listening.encrypted.certificate_file}"')
-		#accepted = context.wrap_socket(accepted, server_side=True, do_handshake_on_connect=False)
+	if listening.context:
+		accepted = listening.context.wrap_socket(accepted, server_side=True, do_handshake_on_connect=False)
 
 	self.trace( 'Accepted "%s"(%d), server at "%s"(%d)' %
 				   (hap[0], hap[1],
 				   listening.listening_ipp.host, listening.listening_ipp.port))
 
 	opened_at = ar.world_now()
 	stream, proxy_address = open_stream(self, server, accepted, None)
```

### Comparing `ansar_connect-0.1.154/src/ansar/connect/standard.py` & `ansar_connect-0.1.156/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.154/src/ansar/connect/transporting.py` & `ansar_connect-0.1.156/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.154/src/ansar/connect/wan.py` & `ansar_connect-0.1.156/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.154/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.156/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.154
+Version: 0.1.156
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.154/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.156/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

