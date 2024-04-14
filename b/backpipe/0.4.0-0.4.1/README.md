# Comparing `tmp/backpipe-0.4.0.tar.gz` & `tmp/backpipe-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backpipe-0.4.0.tar", last modified: Fri Mar 29 03:02:59 2024, max compression
+gzip compressed data, was "backpipe-0.4.1.tar", last modified: Sun Apr 14 10:33:54 2024, max compression
```

## Comparing `backpipe-0.4.0.tar` & `backpipe-0.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-03-29 03:02:59.656815 backpipe-0.4.0/
--rw-r--r--   0 simon     (1000) simon     (1000)    35129 2023-11-04 20:14:40.000000 backpipe-0.4.0/LICENSE
--rw-r--r--   0 simon     (1000) simon     (1000)     3091 2024-03-29 03:02:59.656815 backpipe-0.4.0/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)     2438 2024-03-28 18:05:17.000000 backpipe-0.4.0/README.md
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-03-29 03:02:59.655815 backpipe-0.4.0/backpipe/
--rw-r--r--   0 simon     (1000) simon     (1000)      381 2024-03-28 18:14:22.000000 backpipe-0.4.0/backpipe/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)     4104 2023-11-12 10:54:02.000000 backpipe-0.4.0/backpipe/__main__.py
--rw-r--r--   0 simon     (1000) simon     (1000)     5628 2024-03-29 01:51:33.000000 backpipe-0.4.0/backpipe/app.py
--rw-r--r--   0 simon     (1000) simon     (1000)     3206 2024-03-29 01:54:16.000000 backpipe-0.4.0/backpipe/builder.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1257 2024-03-28 19:06:16.000000 backpipe-0.4.0/backpipe/config.py
--rw-r--r--   0 simon     (1000) simon     (1000)      364 2024-03-29 01:51:22.000000 backpipe-0.4.0/backpipe/defaults.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1651 2024-03-29 01:51:05.000000 backpipe-0.4.0/backpipe/host.py
--rw-r--r--   0 simon     (1000) simon     (1000)      849 2024-03-13 17:17:04.000000 backpipe-0.4.0/backpipe/rq.py
--rw-r--r--   0 simon     (1000) simon     (1000)     6124 2024-03-29 01:49:52.000000 backpipe-0.4.0/backpipe/server.py
--rw-r--r--   0 simon     (1000) simon     (1000)      137 2023-11-14 15:08:41.000000 backpipe-0.4.0/backpipe/uptime.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-03-29 03:02:59.656815 backpipe-0.4.0/backpipe.egg-info/
--rw-r--r--   0 simon     (1000) simon     (1000)     3091 2024-03-29 03:02:59.000000 backpipe-0.4.0/backpipe.egg-info/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)      408 2024-03-29 03:02:59.000000 backpipe-0.4.0/backpipe.egg-info/SOURCES.txt
--rw-r--r--   0 simon     (1000) simon     (1000)        1 2024-03-29 03:02:59.000000 backpipe-0.4.0/backpipe.egg-info/dependency_links.txt
--rw-r--r--   0 simon     (1000) simon     (1000)       52 2024-03-29 03:02:59.000000 backpipe-0.4.0/backpipe.egg-info/entry_points.txt
--rw-r--r--   0 simon     (1000) simon     (1000)       19 2024-03-29 03:02:59.000000 backpipe-0.4.0/backpipe.egg-info/requires.txt
--rw-r--r--   0 simon     (1000) simon     (1000)        9 2024-03-29 03:02:59.000000 backpipe-0.4.0/backpipe.egg-info/top_level.txt
--rw-r--r--   0 simon     (1000) simon     (1000)       38 2024-03-29 03:02:59.656815 backpipe-0.4.0/setup.cfg
--rw-r--r--   0 simon     (1000) simon     (1000)     1277 2024-03-28 17:08:11.000000 backpipe-0.4.0/setup.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-14 10:33:54.507292 backpipe-0.4.1/
+-rw-r--r--   0 simon     (1000) simon     (1000)    35129 2023-11-04 20:14:40.000000 backpipe-0.4.1/LICENSE
+-rw-r--r--   0 simon     (1000) simon     (1000)     3353 2024-04-14 10:33:54.507292 backpipe-0.4.1/PKG-INFO
+-rw-r--r--   0 simon     (1000) simon     (1000)     2700 2024-04-03 20:39:35.000000 backpipe-0.4.1/README.md
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-14 10:33:54.506292 backpipe-0.4.1/backpipe/
+-rw-r--r--   0 simon     (1000) simon     (1000)      458 2024-04-14 10:27:00.000000 backpipe-0.4.1/backpipe/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     6194 2024-04-14 10:30:45.000000 backpipe-0.4.1/backpipe/__main__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     6095 2024-04-14 09:49:40.000000 backpipe-0.4.1/backpipe/app.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     3244 2024-03-30 02:36:58.000000 backpipe-0.4.1/backpipe/builder.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1257 2024-03-28 19:06:16.000000 backpipe-0.4.1/backpipe/config.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      364 2024-03-29 01:51:22.000000 backpipe-0.4.1/backpipe/defaults.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1916 2024-03-30 04:22:44.000000 backpipe-0.4.1/backpipe/host.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1233 2024-04-14 09:53:29.000000 backpipe-0.4.1/backpipe/rq.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     6476 2024-03-30 04:30:41.000000 backpipe-0.4.1/backpipe/server.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      137 2023-11-14 15:08:41.000000 backpipe-0.4.1/backpipe/uptime.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-14 10:33:54.507292 backpipe-0.4.1/backpipe.egg-info/
+-rw-r--r--   0 simon     (1000) simon     (1000)     3353 2024-04-14 10:33:54.000000 backpipe-0.4.1/backpipe.egg-info/PKG-INFO
+-rw-r--r--   0 simon     (1000) simon     (1000)      408 2024-04-14 10:33:54.000000 backpipe-0.4.1/backpipe.egg-info/SOURCES.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)        1 2024-04-14 10:33:54.000000 backpipe-0.4.1/backpipe.egg-info/dependency_links.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)       52 2024-04-14 10:33:54.000000 backpipe-0.4.1/backpipe.egg-info/entry_points.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)       19 2024-04-14 10:33:54.000000 backpipe-0.4.1/backpipe.egg-info/requires.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)        9 2024-04-14 10:33:54.000000 backpipe-0.4.1/backpipe.egg-info/top_level.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)       38 2024-04-14 10:33:54.507292 backpipe-0.4.1/setup.cfg
+-rw-r--r--   0 simon     (1000) simon     (1000)     1277 2024-03-28 17:08:11.000000 backpipe-0.4.1/setup.py
```

### Comparing `backpipe-0.4.0/LICENSE` & `backpipe-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `backpipe-0.4.0/PKG-INFO` & `backpipe-0.4.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backpipe
-Version: 0.4.0
+Version: 0.4.1
 Summary: A backend HTTP framework for Python.
 Home-page: https://github.com/Simoso68/backpipe
 Author: Simoso68
 Maintainer: Simoso68
 License: GNU GPL v3
 Keywords: framework,http,web,api,server
 Classifier: Development Status :: 4 - Beta
@@ -120,10 +120,19 @@
 ```
 
 ## Known issues
 
 - URI-too-long message raises error on client-side when using Python requests
 - Limited client information on URI-too-long message (probably unfixable.)
 
+## HTTPS notice
+
+When activating HTTPS, you need to sign your certificate file \
+with a key provided by a trusted authority. \
+\
+Self-signing your certificate will make tools such as \
+CURL, your Browser, etc. raise a warning, \
+that the website may be unsafe.
+
 ## License
 
 Backpipe is licensed under the GNU GPL v3.
```

### Comparing `backpipe-0.4.0/README.md` & `backpipe-0.4.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -101,10 +101,19 @@
 ```
 
 ## Known issues
 
 - URI-too-long message raises error on client-side when using Python requests
 - Limited client information on URI-too-long message (probably unfixable.)
 
+## HTTPS notice
+
+When activating HTTPS, you need to sign your certificate file \
+with a key provided by a trusted authority. \
+\
+Self-signing your certificate will make tools such as \
+CURL, your Browser, etc. raise a warning, \
+that the website may be unsafe.
+
 ## License
 
 Backpipe is licensed under the GNU GPL v3.
```

### Comparing `backpipe-0.4.0/backpipe/app.py` & `backpipe-0.4.1/backpipe/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,22 @@
             set_port = port
             
         self.__builder__ = BackPipeBuilder(set_address, set_port)
     def __str__(self) -> str:
         return f"BackPipe(address={self.__builder__.addr.__repr__()}, port={self.__builder__.port})"
     def __repr__(self) -> str:
         return self.__str__()
+    # HTTPS support still in Development, uncomment it, if you want to test it.
+    #def enable_https(self, certfile, keyfile):
+    #    """
+    #    Offers integrated SSL support.
+    #    Certfiles and Keyfiles can be generated using OpenSSL.
+    #    Tools such as CURL or your web browser will raise warnings, that the connection is unsafe if you self-sign your certificate.
+    #    """
+    #    self.__builder__.https = {"certfile":certfile, "keyfile":keyfile}
     def set_ratelimit(self, limit: int):
         """
         Set a rate limit for how many requests from one IP address are allowed per minute.
         Set it to a number below 0 to disable rate limiting.
         Default rate limit is -1 (No limit.).
         """
         if not isinstance(limit, int):
```

### Comparing `backpipe-0.4.0/backpipe/builder.py` & `backpipe-0.4.1/backpipe/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from signal import SIGTERM
 from .defaults import *
 
 class BackPipeBuilder():
     def __init__(self, addr, port) -> None:
         self.addr = addr
         self.port = port
+        self.https = None
         self.get = undefined
         self.post = undefined
         self.put = undefined
         self.patch = undefined
         self.delete = undefined
         self.unknown = unknown_method
         self.uri_limit = 65536
@@ -57,15 +58,15 @@
         self.uri_limit_message = message
     def run(self):
         try:
             if system() == "Windows":
                 print(f"\r{Back.YELLOW}{Fore.BLACK} COMPATIBILITY {Back.RESET}{Fore.RESET} Running Backpipe servers on Windows might lead to issues")
             print(f"\r{Back.YELLOW}{Fore.BLACK} INFO {Back.RESET}{Fore.RESET} Starting server ...")
             print(f"\r{Back.YELLOW}{Fore.BLACK} INFO {Back.RESET}{Fore.RESET} Press {Fore.LIGHTRED_EX}Ctrl + C{Fore.RESET} to quit.\n")
-            backpipe_server = Server(self, self.get, self.post, self.put, self.patch, self.delete, self.unknown, self.uri_limit, self.uri_limit_message, self.blocked_msg, self.block_addrs, ratelimit=(self.ratelimit, self.ratelimit_message, self.ratelimit_reset, self.ratelimit_exc_addrs, self.ratelimit_exc_paths), server_address=(self.addr, self.port), RequestHandlerClass=BackPipeServer)
+            backpipe_server = Server(self, self.https, self.get, self.post, self.put, self.patch, self.delete, self.unknown, self.uri_limit, self.uri_limit_message, self.blocked_msg, self.block_addrs, ratelimit=(self.ratelimit, self.ratelimit_message, self.ratelimit_reset, self.ratelimit_exc_addrs, self.ratelimit_exc_paths), server_address=(self.addr, self.port), RequestHandlerClass=BackPipeServer)
             backpipe_server.serve_forever()
         except KeyboardInterrupt:
             print(f"\r{Back.LIGHTRED_EX}{Fore.BLACK} EXIT {Back.RESET}{Fore.RESET} Received Keyboard interrupt, shutting down server.")
             kill(getpid(), SIGTERM)
         except Exception as x:
             print(f"\r{Back.LIGHTRED_EX}{Fore.BLACK} CRASH {Back.RESET}{Fore.RESET} {Fore.BLUE}{type(x).__name__}{Fore.RESET}: {Fore.LIGHTBLUE_EX}{x}{Fore.RESET}")
             try:
```

### Comparing `backpipe-0.4.0/backpipe/config.py` & `backpipe-0.4.1/backpipe/config.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.4.0/backpipe/host.py` & `backpipe-0.4.1/backpipe/host.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 from socketserver import TCPServer
-from multiprocessing import Process
 from threading import Thread
 from time import sleep, time
 from colorama import Fore, Back
+import ssl
 
 class Server(TCPServer):
-    def __init__(self, context, get, post, put, patch, delete, unknown, uri_limit, uri_limited_msg, blocked_msg, blocked_addrs, server_address, ratelimit: tuple, RequestHandlerClass, bind_and_activate: bool = True) -> None:
+    def __init__(self, context, https: dict | None, get, post, put, patch, delete, unknown, uri_limit, uri_limited_msg, blocked_msg, blocked_addrs, server_address, ratelimit: tuple, RequestHandlerClass, bind_and_activate: bool = True) -> None:
         super().__init__(server_address, RequestHandlerClass, bind_and_activate)
 
+        if https != None:
+            self.ssl = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
+            self.ssl.load_cert_chain(https["certfile"], https["keyfile"])
+            self.socket = self.ssl.wrap_socket(self.socket, server_side=True)
+
+        self.https = https
+
         context.started_at = time()
 
         self.get = get
         self.post = post
         self.put = put
         self.patch = patch
         self.delete = delete
```

### Comparing `backpipe-0.4.0/backpipe/server.py` & `backpipe-0.4.1/backpipe/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,14 +87,22 @@
             method()
             self.wfile.flush()
         except TimeoutError as e:
             self.log_error("Request timed out: %r", e)
             self.close_connection = True
             return
     def handlerq(self, answer):
+        """TODO
+        if self.server.https != None:
+            if self.headers.get("X-Forwarded-Proto", "http") == "http":
+                print("YES")
+                self.send_response(301)
+                self.send_header('Location', 'https://{}{}'.format(self.server.server_address[0], self.path))
+                self.end_headers()
+        """
         if not isinstance(answer[0], int):
             raise TypeError(f"HTTP status code must be 'int' not '{type(answer[0]).__name__}'")
         self.send_response(answer[0])
         if config.use_html_header:
             self.send_header("Content-Type", "text/html")
         self.end_headers()
         if isinstance(answer[1], str):
```

### Comparing `backpipe-0.4.0/backpipe.egg-info/PKG-INFO` & `backpipe-0.4.1/backpipe.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backpipe
-Version: 0.4.0
+Version: 0.4.1
 Summary: A backend HTTP framework for Python.
 Home-page: https://github.com/Simoso68/backpipe
 Author: Simoso68
 Maintainer: Simoso68
 License: GNU GPL v3
 Keywords: framework,http,web,api,server
 Classifier: Development Status :: 4 - Beta
@@ -120,10 +120,19 @@
 ```
 
 ## Known issues
 
 - URI-too-long message raises error on client-side when using Python requests
 - Limited client information on URI-too-long message (probably unfixable.)
 
+## HTTPS notice
+
+When activating HTTPS, you need to sign your certificate file \
+with a key provided by a trusted authority. \
+\
+Self-signing your certificate will make tools such as \
+CURL, your Browser, etc. raise a warning, \
+that the website may be unsafe.
+
 ## License
 
 Backpipe is licensed under the GNU GPL v3.
```

### Comparing `backpipe-0.4.0/setup.py` & `backpipe-0.4.1/setup.py`

 * *Files identical despite different names*

