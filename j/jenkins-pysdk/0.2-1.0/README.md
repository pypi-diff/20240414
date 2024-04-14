# Comparing `tmp/jenkins_pysdk-0.2.tar.gz` & `tmp/jenkins_pysdk-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jenkins_pysdk-0.2.tar", last modified: Sun Apr 14 10:01:09 2024, max compression
+gzip compressed data, was "jenkins_pysdk-1.0.tar", last modified: Sun Apr 14 10:43:51 2024, max compression
```

## Comparing `jenkins_pysdk-0.2.tar` & `jenkins_pysdk-1.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 10:01:09.984090 jenkins_pysdk-0.2/
--rw-rw-rw-   0        0        0     1087 2024-03-22 18:07:50.000000 jenkins_pysdk-0.2/LICENSE
--rw-rw-rw-   0        0        0      246 2024-04-14 10:01:09.983586 jenkins_pysdk-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1311 2024-04-14 08:57:58.000000 jenkins_pysdk-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 10:01:09.978066 jenkins_pysdk-0.2/jenkins_pysdk/
--rw-rw-rw-   0        0        0       88 2024-04-13 17:22:49.000000 jenkins_pysdk-0.2/jenkins_pysdk/__init__.py
--rw-rw-rw-   0        0        0      842 2024-04-11 20:11:04.000000 jenkins_pysdk-0.2/jenkins_pysdk/_logger.py
--rw-rw-rw-   0        0        0     4733 2024-04-14 09:10:48.000000 jenkins_pysdk-0.2/jenkins_pysdk/builders.py
--rw-rw-rw-   0        0        0    11470 2024-04-13 10:15:06.000000 jenkins_pysdk-0.2/jenkins_pysdk/builds.py
--rw-rw-rw-   0        0        0     3195 2024-04-14 09:44:14.000000 jenkins_pysdk-0.2/jenkins_pysdk/consts.py
--rw-rw-rw-   0        0        0     7333 2024-04-14 08:57:58.000000 jenkins_pysdk-0.2/jenkins_pysdk/core.py
--rw-rw-rw-   0        0        0    12951 2024-04-14 09:43:04.000000 jenkins_pysdk-0.2/jenkins_pysdk/credentials.py
--rw-rw-rw-   0        0        0     1910 2024-04-13 21:55:53.000000 jenkins_pysdk-0.2/jenkins_pysdk/exceptions.py
--rw-rw-rw-   0        0        0    22962 2024-04-14 09:48:21.000000 jenkins_pysdk-0.2/jenkins_pysdk/jenkins.py
--rw-rw-rw-   0        0        0    30250 2024-04-14 09:59:19.000000 jenkins_pysdk-0.2/jenkins_pysdk/jobs.py
--rw-rw-rw-   0        0        0     2548 2024-04-14 08:57:58.000000 jenkins_pysdk-0.2/jenkins_pysdk/objects.py
--rw-rw-rw-   0        0        0      183 2024-04-09 19:53:47.000000 jenkins_pysdk-0.2/jenkins_pysdk/plugins.py
--rw-rw-rw-   0        0        0     9323 2024-04-13 22:38:05.000000 jenkins_pysdk-0.2/jenkins_pysdk/users.py
--rw-rw-rw-   0        0        0     4951 2024-04-13 18:56:35.000000 jenkins_pysdk-0.2/jenkins_pysdk/utils.py
--rw-rw-rw-   0        0        0    12156 2024-04-14 08:57:58.000000 jenkins_pysdk-0.2/jenkins_pysdk/views.py
-drwxrwxrwx   0        0        0        0 2024-04-14 10:01:09.982582 jenkins_pysdk-0.2/jenkins_pysdk.egg-info/
--rw-rw-rw-   0        0        0      246 2024-04-14 10:01:09.000000 jenkins_pysdk-0.2/jenkins_pysdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      580 2024-04-14 10:01:09.000000 jenkins_pysdk-0.2/jenkins_pysdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 10:01:09.000000 jenkins_pysdk-0.2/jenkins_pysdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-14 10:01:09.000000 jenkins_pysdk-0.2/jenkins_pysdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-14 10:01:09.000000 jenkins_pysdk-0.2/jenkins_pysdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 10:01:09.984090 jenkins_pysdk-0.2/setup.cfg
--rw-rw-rw-   0        0        0      428 2024-04-14 09:51:14.000000 jenkins_pysdk-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 10:43:51.535094 jenkins_pysdk-1.0/
+-rw-rw-rw-   0        0        0     1087 2024-03-22 18:07:50.000000 jenkins_pysdk-1.0/LICENSE
+-rw-rw-rw-   0        0        0      285 2024-04-14 10:43:51.535094 jenkins_pysdk-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1330 2024-04-14 10:24:47.000000 jenkins_pysdk-1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 10:43:51.530082 jenkins_pysdk-1.0/jenkins_pysdk/
+-rw-rw-rw-   0        0        0      129 2024-04-14 10:35:39.000000 jenkins_pysdk-1.0/jenkins_pysdk/__init__.py
+-rw-rw-rw-   0        0        0      842 2024-04-11 20:11:04.000000 jenkins_pysdk-1.0/jenkins_pysdk/_logger.py
+-rw-rw-rw-   0        0        0     4733 2024-04-14 09:10:48.000000 jenkins_pysdk-1.0/jenkins_pysdk/builders.py
+-rw-rw-rw-   0        0        0    11470 2024-04-13 10:15:06.000000 jenkins_pysdk-1.0/jenkins_pysdk/builds.py
+-rw-rw-rw-   0        0        0     3195 2024-04-14 09:44:14.000000 jenkins_pysdk-1.0/jenkins_pysdk/consts.py
+-rw-rw-rw-   0        0        0     7346 2024-04-14 10:39:39.000000 jenkins_pysdk-1.0/jenkins_pysdk/core.py
+-rw-rw-rw-   0        0        0    12951 2024-04-14 09:43:04.000000 jenkins_pysdk-1.0/jenkins_pysdk/credentials.py
+-rw-rw-rw-   0        0        0     1910 2024-04-13 21:55:53.000000 jenkins_pysdk-1.0/jenkins_pysdk/exceptions.py
+-rw-rw-rw-   0        0        0    22862 2024-04-14 10:30:15.000000 jenkins_pysdk-1.0/jenkins_pysdk/jenkins.py
+-rw-rw-rw-   0        0        0    30250 2024-04-14 09:59:19.000000 jenkins_pysdk-1.0/jenkins_pysdk/jobs.py
+-rw-rw-rw-   0        0        0     2548 2024-04-14 08:57:58.000000 jenkins_pysdk-1.0/jenkins_pysdk/objects.py
+-rw-rw-rw-   0        0        0      183 2024-04-09 19:53:47.000000 jenkins_pysdk-1.0/jenkins_pysdk/plugins.py
+-rw-rw-rw-   0        0        0     9323 2024-04-13 22:38:05.000000 jenkins_pysdk-1.0/jenkins_pysdk/users.py
+-rw-rw-rw-   0        0        0     4965 2024-04-14 10:28:54.000000 jenkins_pysdk-1.0/jenkins_pysdk/utils.py
+-rw-rw-rw-   0        0        0       86 2024-04-14 10:38:14.000000 jenkins_pysdk-1.0/jenkins_pysdk/version.py
+-rw-rw-rw-   0        0        0    12156 2024-04-14 08:57:58.000000 jenkins_pysdk-1.0/jenkins_pysdk/views.py
+drwxrwxrwx   0        0        0        0 2024-04-14 10:43:51.534094 jenkins_pysdk-1.0/jenkins_pysdk.egg-info/
+-rw-rw-rw-   0        0        0      285 2024-04-14 10:43:51.000000 jenkins_pysdk-1.0/jenkins_pysdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      605 2024-04-14 10:43:51.000000 jenkins_pysdk-1.0/jenkins_pysdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 10:43:51.000000 jenkins_pysdk-1.0/jenkins_pysdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-14 10:43:51.000000 jenkins_pysdk-1.0/jenkins_pysdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-14 10:43:51.000000 jenkins_pysdk-1.0/jenkins_pysdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 10:43:51.535094 jenkins_pysdk-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      475 2024-04-14 10:43:32.000000 jenkins_pysdk-1.0/setup.py
```

### Comparing `jenkins_pysdk-0.2/LICENSE` & `jenkins_pysdk-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-0.2/README.md` & `jenkins_pysdk-1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ### Supported for python 3.6+
 
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/installation/) and 
-[pypi.org](https://pypi.org/project/jenkins-pysdk/) to install jenkins-pysdk.
+[JenkinsPythonSDK | pypi.org](https://pypi.org/project/jenkins-pysdk/) to install jenkins-pysdk.
 
 ```bash
 pip install jenkins-pysdk
 ```
 
 ## Quick Usage
```

### Comparing `jenkins_pysdk-0.2/jenkins_pysdk/_logger.py` & `jenkins_pysdk-1.0/jenkins_pysdk/_logger.py`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-0.2/jenkins_pysdk/builders.py` & `jenkins_pysdk-1.0/jenkins_pysdk/builders.py`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-0.2/jenkins_pysdk/builds.py` & `jenkins_pysdk-1.0/jenkins_pysdk/builds.py`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-0.2/jenkins_pysdk/consts.py` & `jenkins_pysdk-1.0/jenkins_pysdk/consts.py`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-0.2/jenkins_pysdk/core.py` & `jenkins_pysdk-1.0/jenkins_pysdk/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from jenkins_pysdk.consts import Endpoints
 from jenkins_pysdk.utils import interact_http, interact_http_session
 from jenkins_pysdk.consts import HTTP_HEADER_DEFAULT
 from jenkins_pysdk.objects import HTTPSessionRequestObject, HTTPSessionResponseObject, \
     HTTPRequestObject, HTTPResponseObject
 from jenkins_pysdk.exceptions import JenkinsConnectionException
-from __init__ import version, python_name
+from jenkins_pysdk.version import version, python_name
 
 __all__ = ["Core"]
 
 
 # noinspection PyUnresolvedReferences
 class Core:  # TODO: Revise these messy methods
     def _set_schema(self, url):
```

### Comparing `jenkins_pysdk-0.2/jenkins_pysdk/credentials.py` & `jenkins_pysdk-1.0/jenkins_pysdk/credentials.py`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-0.2/jenkins_pysdk/exceptions.py` & `jenkins_pysdk-1.0/jenkins_pysdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-0.2/jenkins_pysdk/jenkins.py` & `jenkins_pysdk-1.0/jenkins_pysdk/jenkins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 from __future__ import annotations
 
-import os, sys
-project_root = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
-sys.path.insert(0, project_root)
-
 import re
 import time
 
 from typing import Optional
 import threading
 
 from jenkins_pysdk.core import Core
@@ -159,28 +155,28 @@
         """
         return r_jobs(value=Class.Freestyle)
 
     # @property
     # def UsernamePassword(self) -> r_builder.Credential:
     #     return r_builder.Credential(value=Class.UsernamePassword)
 
-    @property
-    def enable_logging(self):
-        """
-        Get the logging level.
-        """
-        return self.Enable_Logging
-
-    @enable_logging.setter
-    def enable_logging(self, value: int):
-        """
-        Enable a logging level.
-        """
-        # TODO: Add logging and enhance with logger per component/more levels etc etc
-        self.Enable_Logging = value
+    # @property
+    # def enable_logging(self):
+    #     """
+    #     Get the logging level.
+    #     """
+    #     return self.Enable_Logging
+    #
+    # @enable_logging.setter
+    # def enable_logging(self, value: int):
+    #     """
+    #     Enable a logging level.
+    #     """
+    #     # TODO: Add logging and enhance with logger per component/more levels etc etc
+    #     self.Enable_Logging = value
 
     def connect(self) -> JenkinsConnectObject:
         """
         Test the connection to the Jenkins instance.
 
         :return: Object containing connection information.
         :rtype: :class:`objects.JenkinsConnectObject`
```

### Comparing `jenkins_pysdk-0.2/jenkins_pysdk/jobs.py` & `jenkins_pysdk-1.0/jenkins_pysdk/jobs.py`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-0.2/jenkins_pysdk/objects.py` & `jenkins_pysdk-1.0/jenkins_pysdk/objects.py`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-0.2/jenkins_pysdk/users.py` & `jenkins_pysdk-1.0/jenkins_pysdk/users.py`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-0.2/jenkins_pysdk/utils.py` & `jenkins_pysdk-1.0/jenkins_pysdk/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from httpx import Client, Request, ConnectError, BasicAuth
 from pydantic import HttpUrl
 
 from jenkins_pysdk.consts import HTTP_RETRY_COUNT, HOST_MATCH_REGEX_PATTERN
 from jenkins_pysdk.objects import HTTPRequestObject, HTTPResponseObject, HTTPSessionRequestObject, \
     HTTPSessionResponseObject
 from jenkins_pysdk.exceptions import JenkinsInvalidHost
-from _logger import logger
+# from _logger import logger
 
 __all__ = ["validate_connect_host", "validate_http_url", "interact_http", "interact_http_session"]
 
 
 def validate_connect_host(host: str) -> bool:
     """
 
@@ -45,56 +45,56 @@
     req = Request(
         method=request.method,
         url=str(request.url),
         headers=request.headers if request.headers else None,
         data=request.data if request.data else None,
         params=request.params if request.params else None
     )
-    logger.debugu(req.url)
+    # logger.debugu(req.url)
     exception = None
     for retry in range(HTTP_RETRY_COUNT):
         try:
             # TODO: SSL/certs
             # TODO: Dynamically add these parameters from the request object
             # TODO: TIDY
             with Client(auth=BasicAuth(request.username, request.passw_or_token),
                         verify=request.verify, proxies=request.proxy, timeout=request.timeout) as conn:
                 response = conn.send(request=req, follow_redirects=True)
                 return_object = HTTPResponseObject(request=req, content=response.text,
                                                    status_code=int(response.status_code))
                 return_object._raw = response
-                logger.debuge(response.content)
+                # logger.debuge(response.content)
                 return return_object
         except (EnvironmentError, ConnectError) as error:
             # TODO: below lines suck
             exception = error
             time.sleep(1)
             continue
         except TimeoutError as error:
             raise error
     else:
         msg = "Request failed due to an exception. See _raw field."
         return_object = HTTPResponseObject(request=req, content=msg, status_code=-1)
         return_object._raw = exception
-        logger.debuge(exception)
+        # logger.debuge(exception)
         return return_object
 
 
 def interact_http_session(request: HTTPSessionRequestObject) -> HTTPSessionResponseObject:
     if validate_http_url(request.url) is False:
         raise JenkinsInvalidHost(f"{request.url.host} is not a valid target.")
 
     req = Request(
         method=request.method,
         url=str(request.url),
         headers=request.headers,
         data=request.data,
         params=request.params,
     )
-    logger.debugu(req.url)
+    # logger.debugu(req.url)
     exception: Exception = Exception()
     for retry in range(HTTP_RETRY_COUNT):
         # TODO: SSL/certs
         # TODO: Dynamically add these parameters from the request object
         # TODO: TIDY
         if request.session:
             session = request.session
@@ -102,25 +102,25 @@
             session = Client(auth=BasicAuth(request.username, request.passw_or_token),
                              verify=request.verify, proxies=request.proxy, timeout=request.timeout)
         try:
             response = session.send(request=req, follow_redirects=True)
             return_object = HTTPSessionResponseObject(request=req, content=response.text,
                                                       status_code=int(response.status_code), session=session)
             return_object._raw = response
-            logger.debuge(response.content)
+            # logger.debuge(response.content)
             return return_object
         except (EnvironmentError, ConnectError) as error:
             # TODO: below lines suck
             exception = error
             time.sleep(1)
             continue
             # TODO: Add statistics on response times etc as debug
         finally:
             if request.keep_session is False:
                 session.close()
     else:
         msg = "Request failed due to an exception. See _raw field."
         return_object = HTTPSessionResponseObject(request=req, content=msg, status_code=-1, session=None)
         return_object._raw = exception
-        logger.debuge(exception)
+        # logger.debuge(exception)
         return return_object
```

### Comparing `jenkins_pysdk-0.2/jenkins_pysdk/views.py` & `jenkins_pysdk-1.0/jenkins_pysdk/views.py`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-0.2/jenkins_pysdk.egg-info/SOURCES.txt` & `jenkins_pysdk-1.0/jenkins_pysdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,13 +11,14 @@
 jenkins_pysdk/exceptions.py
 jenkins_pysdk/jenkins.py
 jenkins_pysdk/jobs.py
 jenkins_pysdk/objects.py
 jenkins_pysdk/plugins.py
 jenkins_pysdk/users.py
 jenkins_pysdk/utils.py
+jenkins_pysdk/version.py
 jenkins_pysdk/views.py
 jenkins_pysdk.egg-info/PKG-INFO
 jenkins_pysdk.egg-info/SOURCES.txt
 jenkins_pysdk.egg-info/dependency_links.txt
 jenkins_pysdk.egg-info/requires.txt
 jenkins_pysdk.egg-info/top_level.txt
```

