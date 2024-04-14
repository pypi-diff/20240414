# Comparing `tmp/jenkins_pysdk-0.1.1.1.dev0.tar.gz` & `tmp/jenkins_pysdk-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jenkins_pysdk-0.1.1.1.dev0.tar", last modified: Tue Apr  9 19:26:35 2024, max compression
+gzip compressed data, was "jenkins_pysdk-0.2.tar", last modified: Sun Apr 14 10:01:09 2024, max compression
```

## Comparing `jenkins_pysdk-0.1.1.1.dev0.tar` & `jenkins_pysdk-0.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 19:26:35.384378 jenkins_pysdk-0.1.1.1.dev0/
--rw-rw-rw-   0        0        0     1087 2024-03-22 18:07:50.000000 jenkins_pysdk-0.1.1.1.dev0/LICENSE
--rw-rw-rw-   0        0        0      255 2024-04-09 19:26:35.384378 jenkins_pysdk-0.1.1.1.dev0/PKG-INFO
--rw-rw-rw-   0        0        0     1101 2024-04-09 18:57:29.000000 jenkins_pysdk-0.1.1.1.dev0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 19:26:35.378731 jenkins_pysdk-0.1.1.1.dev0/jenkins_pysdk/
--rw-rw-rw-   0        0        0        0 2024-03-22 18:18:56.000000 jenkins_pysdk-0.1.1.1.dev0/jenkins_pysdk/__init__.py
--rw-rw-rw-   0        0        0     2272 2024-04-08 21:56:31.000000 jenkins_pysdk-0.1.1.1.dev0/jenkins_pysdk/builders.py
--rw-rw-rw-   0        0        0     6710 2024-04-09 18:42:09.000000 jenkins_pysdk-0.1.1.1.dev0/jenkins_pysdk/builds.py
--rw-rw-rw-   0        0        0     2745 2024-04-09 18:42:09.000000 jenkins_pysdk-0.1.1.1.dev0/jenkins_pysdk/consts.py
--rw-rw-rw-   0        0        0     7365 2024-04-09 18:42:09.000000 jenkins_pysdk-0.1.1.1.dev0/jenkins_pysdk/core.py
--rw-rw-rw-   0        0        0     5875 2024-04-09 18:42:09.000000 jenkins_pysdk-0.1.1.1.dev0/jenkins_pysdk/credentials.py
--rw-rw-rw-   0        0        0    19799 2024-04-09 19:25:57.000000 jenkins_pysdk-0.1.1.1.dev0/jenkins_pysdk/jenkins.py
--rw-rw-rw-   0        0        0     1228 2024-04-07 17:43:03.000000 jenkins_pysdk-0.1.1.1.dev0/jenkins_pysdk/jenkins_exceptions.py
--rw-rw-rw-   0        0        0    22907 2024-04-09 18:42:09.000000 jenkins_pysdk-0.1.1.1.dev0/jenkins_pysdk/jobs.py
--rw-rw-rw-   0        0        0      155 2024-04-09 18:24:43.000000 jenkins_pysdk-0.1.1.1.dev0/jenkins_pysdk/plugins.py
--rw-rw-rw-   0        0        0     5807 2024-04-09 19:22:01.000000 jenkins_pysdk-0.1.1.1.dev0/jenkins_pysdk/response_objects.py
--rw-rw-rw-   0        0        0     5745 2024-04-09 18:42:09.000000 jenkins_pysdk-0.1.1.1.dev0/jenkins_pysdk/users.py
--rw-rw-rw-   0        0        0     5080 2024-04-09 18:42:09.000000 jenkins_pysdk-0.1.1.1.dev0/jenkins_pysdk/utils.py
--rw-rw-rw-   0        0        0     9399 2024-04-09 18:42:09.000000 jenkins_pysdk-0.1.1.1.dev0/jenkins_pysdk/views.py
-drwxrwxrwx   0        0        0        0 2024-04-09 19:26:35.383378 jenkins_pysdk-0.1.1.1.dev0/jenkins_pysdk.egg-info/
--rw-rw-rw-   0        0        0      255 2024-04-09 19:26:35.000000 jenkins_pysdk-0.1.1.1.dev0/jenkins_pysdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      572 2024-04-09 19:26:35.000000 jenkins_pysdk-0.1.1.1.dev0/jenkins_pysdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 19:26:35.000000 jenkins_pysdk-0.1.1.1.dev0/jenkins_pysdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-09 19:26:35.000000 jenkins_pysdk-0.1.1.1.dev0/jenkins_pysdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-09 19:26:35.000000 jenkins_pysdk-0.1.1.1.dev0/jenkins_pysdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 19:26:35.384878 jenkins_pysdk-0.1.1.1.dev0/setup.cfg
--rw-rw-rw-   0        0        0      384 2024-04-09 19:26:15.000000 jenkins_pysdk-0.1.1.1.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 10:01:09.984090 jenkins_pysdk-0.2/
+-rw-rw-rw-   0        0        0     1087 2024-03-22 18:07:50.000000 jenkins_pysdk-0.2/LICENSE
+-rw-rw-rw-   0        0        0      246 2024-04-14 10:01:09.983586 jenkins_pysdk-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1311 2024-04-14 08:57:58.000000 jenkins_pysdk-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 10:01:09.978066 jenkins_pysdk-0.2/jenkins_pysdk/
+-rw-rw-rw-   0        0        0       88 2024-04-13 17:22:49.000000 jenkins_pysdk-0.2/jenkins_pysdk/__init__.py
+-rw-rw-rw-   0        0        0      842 2024-04-11 20:11:04.000000 jenkins_pysdk-0.2/jenkins_pysdk/_logger.py
+-rw-rw-rw-   0        0        0     4733 2024-04-14 09:10:48.000000 jenkins_pysdk-0.2/jenkins_pysdk/builders.py
+-rw-rw-rw-   0        0        0    11470 2024-04-13 10:15:06.000000 jenkins_pysdk-0.2/jenkins_pysdk/builds.py
+-rw-rw-rw-   0        0        0     3195 2024-04-14 09:44:14.000000 jenkins_pysdk-0.2/jenkins_pysdk/consts.py
+-rw-rw-rw-   0        0        0     7333 2024-04-14 08:57:58.000000 jenkins_pysdk-0.2/jenkins_pysdk/core.py
+-rw-rw-rw-   0        0        0    12951 2024-04-14 09:43:04.000000 jenkins_pysdk-0.2/jenkins_pysdk/credentials.py
+-rw-rw-rw-   0        0        0     1910 2024-04-13 21:55:53.000000 jenkins_pysdk-0.2/jenkins_pysdk/exceptions.py
+-rw-rw-rw-   0        0        0    22962 2024-04-14 09:48:21.000000 jenkins_pysdk-0.2/jenkins_pysdk/jenkins.py
+-rw-rw-rw-   0        0        0    30250 2024-04-14 09:59:19.000000 jenkins_pysdk-0.2/jenkins_pysdk/jobs.py
+-rw-rw-rw-   0        0        0     2548 2024-04-14 08:57:58.000000 jenkins_pysdk-0.2/jenkins_pysdk/objects.py
+-rw-rw-rw-   0        0        0      183 2024-04-09 19:53:47.000000 jenkins_pysdk-0.2/jenkins_pysdk/plugins.py
+-rw-rw-rw-   0        0        0     9323 2024-04-13 22:38:05.000000 jenkins_pysdk-0.2/jenkins_pysdk/users.py
+-rw-rw-rw-   0        0        0     4951 2024-04-13 18:56:35.000000 jenkins_pysdk-0.2/jenkins_pysdk/utils.py
+-rw-rw-rw-   0        0        0    12156 2024-04-14 08:57:58.000000 jenkins_pysdk-0.2/jenkins_pysdk/views.py
+drwxrwxrwx   0        0        0        0 2024-04-14 10:01:09.982582 jenkins_pysdk-0.2/jenkins_pysdk.egg-info/
+-rw-rw-rw-   0        0        0      246 2024-04-14 10:01:09.000000 jenkins_pysdk-0.2/jenkins_pysdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      580 2024-04-14 10:01:09.000000 jenkins_pysdk-0.2/jenkins_pysdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 10:01:09.000000 jenkins_pysdk-0.2/jenkins_pysdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-14 10:01:09.000000 jenkins_pysdk-0.2/jenkins_pysdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-14 10:01:09.000000 jenkins_pysdk-0.2/jenkins_pysdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 10:01:09.984090 jenkins_pysdk-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      428 2024-04-14 09:51:14.000000 jenkins_pysdk-0.2/setup.py
```

### Comparing `jenkins_pysdk-0.1.1.1.dev0/LICENSE` & `jenkins_pysdk-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jenkins_pysdk-0.1.1.1.dev0/jenkins_pysdk/consts.py` & `jenkins_pysdk-0.2/jenkins_pysdk/consts.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,91 +2,99 @@
            "References", "XML_HEADER_DEFAULT", "FORM_HEADER_DEFAULT", "XML_POST_HEADER", "Class"]
 
 HTTP_RETRY_COUNT = 1
 HTTP_HEADER_DEFAULT = {"Content-Type": "application/json"}
 XML_HEADER_DEFAULT = {"Content-Type": "application/xml"}
 XML_POST_HEADER = {"Content-Type": "text/xml"}
 FORM_HEADER_DEFAULT = {"Content-Type": "application/x-www-form-urlencoded"}
-HTTP_REQUEST_PARAMETERS = ['method', 'url', 'headers', 'data', 'verify', 'auth']
+# HTTP_REQUEST_PARAMETERS = ['method', 'url', 'headers', 'data', 'verify', 'auth']
 
 HOST_MATCH_REGEX_PATTERN = r"^[a-zA-Z0-9.-]+$"
 
 
 class Endpoints:
     class Instance:
         Crumb = "crumbIssuer/api/json"
         Connect = "login"
-        Jobs = "api/json?tree="  # TODO: Change ?tree= maybe?
+        # Jobs = "api/json?tree="  # TODO: Change ?tree= maybe?
         Standard = "api/json"
         About = "about"  # For plugins list etc
         OverallLoad = "overallLoad/api/json"
         Computer = "computer/api/json"
 
     class Manage:
         Reload = "manage/#"
         CredentialStore = "manage/credentials/store/system"
 
     class Jobs:
         Create = "createItem"
         Enable = "enable"
         Disable = "disable"
         Xml = "config.xml"
+        Iter = "jobs[fullName,url,jobs[fullName,url,jobs]]"
 
     class Builds:
         BuildNumber = "buildNumber"
         BuildConsoleText = "consoleText"
         ProgressiveConsoleText = "progressiveText"
         ProgressiveHtml = "progressiveHtml"
         Delete = "doDelete"
         Changes = "changes"
         Build = "build"
 
     class Views:
         View = "view"
         Create = "createView"
+        Iter = "views[name,url,jobs[fullName,url,jobs]]"
 
     class Credential:
         Create = "createCredentials"
+        Get = "credential/{cred_id}"
+        Move = "doMove"
 
     class Credentials:
         Domain = "manage/credentials/store/system/domain/{domain}"
         Create = "manage/credentials/store/system/newDomain"
+        CreateDomain = "manage/credentials/store/system/createDomain"
 
     class Maintenance:
         Restart = "restart"
         SafeRestart = "safeRestart"
         QuietDown = "quietDown"
         NoQuietDown = "cancelQuietDown"
         Shutdown = "exit"
         SafeShutdown = "safeExit"
 
     class Users:
         List = "asynchPeople"
         User = "user/{username}"
         Create = "manage/securityRealm/addUser"
+        CreateByAdmin = "/securityRealm/createAccountByAdmin"
 
     class User:
         Logout = "logout"
         Delete = "doDelete"
         Builds = "builds"
         Views = "my-views/view/all"
         Credentials = "credentials/store/user/domain/{domain}/"
         Me = "me"
+        Boot = "user/{user}/descriptorByName/jenkins.security.seed.UserSeedProperty/renewSessionSeed"
 
     class Plugins:
         pass
 
 
 class Class:
     Folder = "com.cloudbees.hudson.plugins.folder.Folder"
     Freestyle = "hudson.model.FreeStyleProject"
     JenkinsFile = ""
     ListView = "hudson.model.ListView"
     MyView = "hudson.model.MyView"
     Dashboard = "hudson.plugins.view.dashboard.Dashboard"
+    UsernamePassword = ""
 
 
 class References:
     class Jobs:
         JOBS = "jobs"
         VIEWS = "views"
```

### Comparing `jenkins_pysdk-0.1.1.1.dev0/jenkins_pysdk/core.py` & `jenkins_pysdk-0.2/jenkins_pysdk/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,52 @@
 from typing import Union, Tuple
-from abc import ABC, abstractmethod
 
 import orjson
 from pydantic import HttpUrl
 
 from jenkins_pysdk.consts import Endpoints
 from jenkins_pysdk.utils import interact_http, interact_http_session
 from jenkins_pysdk.consts import HTTP_HEADER_DEFAULT
-from jenkins_pysdk.response_objects import HTTPSessionRequestObject, HTTPSessionResponseObject, \
+from jenkins_pysdk.objects import HTTPSessionRequestObject, HTTPSessionResponseObject, \
     HTTPRequestObject, HTTPResponseObject
+from jenkins_pysdk.exceptions import JenkinsConnectionException
+from __init__ import version, python_name
 
 __all__ = ["Core"]
 
 
 # noinspection PyUnresolvedReferences
 class Core:  # TODO: Revise these messy methods
     def _set_schema(self, url):
         raise NotImplemented
 
-    # def _build_url(self, endpoint: str, prefix: str = None) -> HttpUrl:
-    #     endpoint = str(endpoint)
-    #     scheme = "https://" if self.verify else "http://"
-    #     if prefix:
-    #         prefix = str(prefix)
-    #         prefix = prefix[:-1] if prefix.endswith("/") else prefix
-    #         return HttpUrl(f"{prefix}/{endpoint}".replace("//", "/"))
-    #     return HttpUrl(f"{scheme}{self.host}/{endpoint}".replace("//", "/"))
-
     def _build_url(self, endpoint: str, prefix: str = None, suffix: str = None) -> HttpUrl:
-        scheme = "https://" if self.verify else "http://"
+        host = self.host.replace("http://", "https://") if self.verify else self.host
         if prefix:
-            prefix = str(prefix)
-            prefix = prefix[:-1] if prefix.endswith("/") else prefix
-            endpoint = HttpUrl(f"{prefix}/{endpoint}".replace("//", "/"))
+            prefix = str(prefix).replace("http://", "https://") if self.verify else str(prefix)
+            endpoint = f"{prefix.rstrip('/')}/{endpoint.replace('//', '/')}"
         else:
-            endpoint = HttpUrl(f"{scheme}{self.host}/{endpoint}".replace("//", "/"))
+            endpoint = f"{host}/{endpoint.replace('//', '/')}"
         if suffix:
-            endpoint = f"{str(endpoint)}/{suffix}".replace("//", "/")
-        return endpoint
+            endpoint = f"{endpoint.rstrip('/')}/{suffix.replace('//', '/')}"
+        return HttpUrl(endpoint)
 
     def _validate_url_returned_from_instance(self, data: orjson):
         """
         Handle returned endpoints when the Jenkins instance is not configured properly.
         :param data:
         :return:
         """
         if isinstance(data, dict):
             for key, value in data.items():
                 if key in ['url', 'absoluteUrl'] and isinstance(value, str):
                     if self.verify:
                         value = value.replace("http://", "https://")
-                    value = value.replace("localhost:8080", self.host)  # TODO: Make this work for non 8080
+                    # TODO: Make this work for non 8080
+                    value = value.replace("localhost:8080", self.host.lstrip("http://").lstrip("https://"))
                     data[key] = value
                 else:
                     data[key] = self._validate_url_returned_from_instance(value)
         elif isinstance(data, list):
             for i, item in enumerate(data):
                 data[i] = self._validate_url_returned_from_instance(item)
         return data
@@ -64,25 +56,25 @@
         import re
         if folder_path:
             job_path = f"{folder_path}/{job_path}".replace("//", "/")
         if not job_path.startswith("/"):
             job_path = "/" + job_path
         if job_path.endswith("/"):
             job_path = job_path[:-2]
-        job_path = re.sub(r"((\/)?\bjob\b(\/)?){1,}", "/", str(job_path))
+        job_path = re.sub(r"((/)?\bjob\b(/)?)+", "/", str(job_path))
         return job_path.replace("/", "/job/")
 
     @staticmethod
     def _build_view_http_path(view_path: str):
         import re
         if not view_path.startswith("/"):
             view_path = "/" + view_path
         if view_path.endswith("/"):
             view_path = view_path[:-2]
-        job_path = re.sub(r"((\/)?\bjob\b(\/)?){1,}", "/", str(view_path))
+        job_path = re.sub(r"((/)?\bjob\b(/)?)+", "/", str(view_path))
         return job_path.replace("/", "/view/")
 
     @staticmethod
     def _get_folder_parent(folder_path: str) -> (str, str):
         if folder_path.startswith("/"):
             folder_path = folder_path[1:]
         if folder_path.endswith("/"):
@@ -93,15 +85,15 @@
         return folder_name, folder_path
 
     @staticmethod
     def _get_job_level(path: str) -> int:
         levels = path.split('/')
         return len(levels)
 
-    def _send_http(self, /,
+    def _send_http(self, *,
                    url: HttpUrl,
                    method: str = "GET",
                    headers: dict = HTTP_HEADER_DEFAULT,
                    params: dict = None,
                    data: dict = None,
                    username: str = None,
                    passw_or_token: str = None,
@@ -117,37 +109,42 @@
         :param params: request parameters
         :param data: request data
         :param username: user where authentication is needed
         :param passw_or_token: password or API token for authentication
         :param timeout: request timeout
         :return:
         """
+        headers.update({"User-Agent": f"{python_name}/{version}"})
         # TODO: Unit Test
         if self.token:
             request_obj = HTTPRequestObject(method=method, url=url, headers=headers, params=params, data=data,
                                             username=username if username else self.username,
                                             passw_or_token=self.token if self.token else self.passw,
                                             verify=self.verify,
                                             proxy=self.proxy,
                                             timeout=timeout if timeout else self.timeout)
-            return request_obj, interact_http(request_obj)
+            req, resp = request_obj, interact_http(request_obj)
+            if isinstance(resp._raw, Exception):
+                raise JenkinsConnectionException(resp._raw)
+            return req, resp
         else:
             crumbed_session_req = HTTPSessionRequestObject(
                 method="GET", url=self._build_url(Endpoints.Instance.Crumb), headers=headers,
                 username=username if username else self.username,
                 passw_or_token=passw_or_token if passw_or_token else self.passw,
                 verify=self.verify,
                 proxy=self.proxy,
                 timeout=timeout if timeout else self.timeout,
                 keep_session=True
             )
             crumbed_session = interact_http_session(crumbed_session_req)
+            if isinstance(crumbed_session._raw, Exception):
+                raise JenkinsConnectionException(crumbed_session._raw)
             crumbed_data = orjson.loads(crumbed_session.content)
-            add_crumb_header = {crumbed_data['crumbRequestField']: crumbed_data['crumb']}
-            headers.update(add_crumb_header)
+            headers.update({crumbed_data['crumbRequestField']: crumbed_data['crumb']})
             request_obj = HTTPSessionRequestObject(method=method, url=url, headers=headers, params=params, data=data,
                                                    username=username if username else self.username,
                                                    passw_or_token=passw_or_token if passw_or_token else self.passw,
                                                    verify=self.verify,
                                                    proxy=self.proxy,
                                                    timeout=timeout if timeout else self.timeout,
                                                    session=crumbed_session.session)
```

### Comparing `jenkins_pysdk-0.1.1.1.dev0/jenkins_pysdk/jenkins.py` & `jenkins_pysdk-0.2/jenkins_pysdk/jenkins.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,60 +3,65 @@
 import os, sys
 project_root = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
 sys.path.insert(0, project_root)
 
 import re
 import time
 
-import pprint
 from typing import Optional
 import threading
 
 from jenkins_pysdk.core import Core
 from jenkins_pysdk.consts import Endpoints, FORM_HEADER_DEFAULT, Class
-from jenkins_pysdk.jenkins_exceptions import JenkinsConnectionException, JenkinsUnauthorisedException, JenkinsRestartFailed, \
-    JenkinsActionFailed
-from jenkins_pysdk.response_objects import JenkinsConnectObject, JenkinsDataObject, JenkinsActionObject, \
-    HTTPSessionResponseObject, Views as r_views, Jobs as r_jobs
-from jenkins_pysdk.jobs import Jobs, Folders, Job, Folder
-from jenkins_pysdk.views import Views, View
+from jenkins_pysdk.exceptions import JenkinsConnectionException, JenkinsUnauthorisedException, \
+    JenkinsRestartFailed, JenkinsActionFailed, JenkinsGeneralException
+from jenkins_pysdk.objects import JenkinsConnectObject, JenkinsActionObject, Views as r_views, Jobs as r_jobs
+from jenkins_pysdk.jobs import Jobs, Folders
+from jenkins_pysdk.views import Views
 from jenkins_pysdk.users import Users, User
 from jenkins_pysdk.credentials import Credentials
+from jenkins_pysdk.plugins import Plugins
 
 import orjson
 
 
 __all__ = ["Jenkins"]
 
 
-import logging
-logging.basicConfig(handlers=[logging.StreamHandler()], format="func=%(funcName)s line=%(lineno)d | %(message)s")
-
-
 class Jenkins(Core):
-    Enable_Logging = 0
+    """
+    This is the main class for interacting with your Jenkins instance.
 
-    def __init__(self, /, *,
+    :param host: The hostname/IP/DNS of the Jenkins instance.
+    :type host: str
+    :param username: The username for authentication. Defaults to None.
+    :type username: str, optional
+    :param passw: The password for authentication. Defaults to None.
+    :type passw: str, optional
+    :param token: The API token for authentication. Defaults to None.
+    :type token: str, optional
+    :param verify: Enable or disable SSL verification. Defaults to True.
+    :type verify: bool, optional
+    :param proxy: Specify a proxy for routing requests. Supports both HTTP and HTTPS. Defaults to None.
+    :type proxy: dict, optional
+    :param port: The port number for connecting to the Jenkins instance. Defaults to 443.
+    :type port: int, optional
+    :param timeout: Specify the connection timeout in seconds. Defaults to 30.
+    :type timeout: int, optional
+    """
+
+    def __init__(self, *,
                  host: str,
                  username: Optional[str] = None,
                  passw: Optional[str] = None,
                  token: Optional[str] = None,
                  verify: Optional[bool] = True,
                  proxy: dict = None,
                  port: int = 443,
                  timeout: int = 30):
-        """
-
-        :param host:
-        :param username:
-        :param passw:
-        :param token:
-        :param verify:
-        :param timeout:
-        """
         self.host = host
         self.username = username
         self.passw = passw
         self.token = token
         self.verify = verify
         self.proxy = proxy
         self.port = port
@@ -64,63 +69,127 @@
 
         # Extend functionality
         self._jobs = Jobs(self)
         self._folders = Folders(self)
         self._views = Views(self)
         self._credentials = Credentials(self)
         self._users = Users(self)
+        self._plugins = Plugins(self)
+
+        self._logging_level = 0
 
         # Test connection
         self.connect()
 
     @property
-    def jobs(self) -> (Jobs, Job):
+    def jobs(self) -> Jobs:
+        """
+        Retrieve information about jobs.
+
+        :return: A Jobs object representing the jobs on the system.
+        :rtype: :class:`jobs.Jobs`
+        """
         return self._jobs
 
     @property
-    def folders(self) -> (Folders, Folder):
+    def folders(self) -> Folders:
+        """
+        Retrieve information about folders.
+
+        :return: A Folders object representing the folders on the system.
+        :rtype: :class:`jobs.Folders`
+        """
         return self._folders
 
     @property
-    def views(self) -> (Views, View):
+    def views(self) -> Views:
+        """
+        Retrieve information about views.
+
+        :return: A Views object representing the views on the system.
+        :rtype: :class:`views.Views`
+        """
         return self._views
 
     @property
-    def credentials(self):
+    def credentials(self) -> Credentials:
+        """
+        Retrieve information about credentials.
+
+        :return: A Credentials object representing the credentials on the system.
+        :rtype: :class:`credentials.Credentials`
+        """
         return self._credentials
 
-    def ApiRaw(self, query: str):
+    def api(self, query: str):
+        """
+        Run a custom query and return the relevant data objects.
+
+        :return: Data objects representing the resource requested.
+        """
         # TODO: Allow the user to enter their own query parameters
         raise NotImplementedError
 
     @property
     def ListView(self) -> r_views:
+        """
+        Flag used to create a ListView View in Views.create method.
+
+        :return: Flag for creating a ListView View
+        :rtype: :class:`objects.Flags.Views`
+        """
         return r_views(value=Class.ListView)
 
     @property
     def MyView(self) -> r_views:
+        """
+        Flag used to create a MyView View in Views.create method.
+
+        :return: Flag for creating a MyView View
+        :rtype: :class:`objects.Flags.Views`
+        """
         return r_views(value=Class.MyView)
 
     @property
     def FreeStyle(self) -> r_jobs:
+        """
+        Flag used to create FreeStyle jobs in Jobs.create method.
+
+        :return: Flag for creating FreeStyle jobs
+        :rtype: :class:`objects.Flags.Jobs`
+        """
         return r_jobs(value=Class.Freestyle)
 
+    # @property
+    # def UsernamePassword(self) -> r_builder.Credential:
+    #     return r_builder.Credential(value=Class.UsernamePassword)
+
     @property
     def enable_logging(self):
+        """
+        Get the logging level.
+        """
         return self.Enable_Logging
 
     @enable_logging.setter
-    def enable_logging(self, value: int or bool):
+    def enable_logging(self, value: int):
+        """
+        Enable a logging level.
+        """
         # TODO: Add logging and enhance with logger per component/more levels etc etc
         self.Enable_Logging = value
 
-    def connect(self) -> JenkinsConnectObject or JenkinsConnectionException:
+    def connect(self) -> JenkinsConnectObject:
         """
-        Connect to the Jenkins instance.
-        :return:
+        Test the connection to the Jenkins instance.
+
+        :return: Object containing connection information.
+        :rtype: :class:`objects.JenkinsConnectObject`
+        :raises JenkinsConnectionException: If a connection exception if it fails to connect.
+        :raises JenkinsUnauthorisedException: If the credentials aren't valid.
         """
         # TODO: Fix PORTING MAYBE?
         url = self._build_url(Endpoints.Instance.Connect)
         req_obj, response_obj = self._send_http(url=url)
         code = int(response_obj.status_code)
         if code == 200:
             msg = f"[{response_obj.status_code}] Successfully connected to {self.host}."
@@ -132,266 +201,256 @@
             msg = JenkinsConnectionException(f"[{response_obj.status_code}] Failed to connect to host.")
             return_object = JenkinsConnectObject(request=req_obj, response=response_obj, content=msg,
                                                  status_code=response_obj.status_code)
             return_object._raw = response_obj._raw
             return return_object
         elif code == 401:
             if self.username and self.passw:
-                msg = JenkinsUnauthorisedException(
-                    f"[{response_obj.status_code}] Wrong credentials supplied.")
+                raise JenkinsUnauthorisedException(f"[{response_obj.status_code}] Wrong credentials supplied.")
             elif not self.username:
-                msg = JenkinsUnauthorisedException(
-                    f"[{response_obj.status_code}] Unauthorised. No username supplied.")
+                raise JenkinsUnauthorisedException(f"[{response_obj.status_code}] Unauthorised. No username supplied.")
             elif not self.passw and not self.token:
-                msg = JenkinsUnauthorisedException(
-                    f"[{response_obj.status_code}] Unauthorised. No password supplied.")
+                raise JenkinsUnauthorisedException(f"[{response_obj.status_code}] Unauthorised. No password supplied.")
             else:
-                msg = JenkinsUnauthorisedException(
-                    f"[{response_obj.status_code}] Unauthorised. No credentials supplied.")
-            return_object = JenkinsConnectObject(request=req_obj, response=response_obj, content=msg,
-                                                 status_code=response_obj.status_code)
-            return_object._raw = response_obj._raw
-            return return_object
-        elif code == 500:
+                raise JenkinsUnauthorisedException(f"[{response_obj.status_code}] Unauthorised. No credentials supplied.")
+        elif code >= 500:
             # TODO: FIX THIS DUPLICATE CODE MESS
             msg = JenkinsConnectionException(f"[{response_obj.status_code}] Server error.")
             return_object = JenkinsConnectObject(request=req_obj, response=response_obj, content=msg,
                                                  status_code=response_obj.status_code)
             return_object._raw = response_obj._raw
             return return_object
         msg = "Unhandled response. See _raw field if request failed."
         if response_obj.status_code not in [200, 201]:
             raise JenkinsConnectionException(msg)
 
-    def use_crumb(self) -> HTTPSessionResponseObject:
-        """
-        Spawns a session with the crumb included.
-        Note: Crumbs are auto-applied to any requests that don't use an API token.
-        :return:
-        """
-        url = self._build_url(Endpoints.Instance.Crumb)
-        req_obj, resp_obj = self._send_http(url=url)
-        data = orjson.loads(resp_obj.content)
-        add_crumb_header = {data['crumbRequestField']: data['crumb']}
-        resp_obj.session.headers.update(add_crumb_header)
-        raise NotImplementedError
-
     @property
     def tree(self):
         """
         View all jobs in a pretty tree-like structure.
-        :return:
+
+        :return: Tree-like structure of all jobs.
         """
         raise NotImplemented
 
     @property
     def users(self) -> Users:
+        """
+        Retrieve information about users.
+
+        :return: A Users object representing the users on the system.
+        :rtype: :class:`users.Users`
+        """
         return self._users
 
     @property
-    def me(self):
+    def me(self) -> User:
         """
-        Return the authenticated users' information.
+        Retrieve information about the authenticated user.
+
+        :return: Information about the authenticated user
+        :rtype: :class:`users.User`
         """
         url = self._build_url(Endpoints.User.Me)
         return User(self, url)
 
     @property
-    def version(self):
-        # TODO: Finish me
-        url = self._build_url(Endpoints.Instance.Crumb)
-        req_obj, resp_obj = self._send_http(url)
-        print(resp_obj.content)
-        raise NotImplemented
+    def plugins(self) -> Plugins:
+        """
+        Retrieve information about plugins.
+
+        :return: A Plugins object representing the plugins on the system.
+        :rtype: :class:`plugins.Plugins`
+        """
+        return self._plugins
 
     @property
-    def plugins(self):
+    def version(self) -> str:
         """
-        Returns a list of all plugins on the Jenkins instance.
-        :return:
+        Get the version information of the Jenkins instance.
+
+        :return: Version information of the Jenkins instance
+        :rtype: str
         """
-        raise NotImplemented
+        # TODO: Finish me
+        url = self._build_url(Endpoints.Instance.Crumb)
+        req_obj, resp_obj = self._send_http(url)
+        return str(resp_obj._raw.headers['x-jenkins'])
 
     @property
-    def available_executors(self) -> JenkinsDataObject:
+    def available_executors(self) -> int:
         """
-        View the available executors on the instance.
-        :return:
+        View the number of available executors on the instance.
+
+        :return: Number of available executors
+        :rtype: int
+        :raises JenkinsGeneralException: If a general exception occurs.
         """
         # TODO: FIX CODE COPY & PASTE BELOW... maybe singledispatch
         _fields = ['_class', 'availableExecutors']
         url = self._build_url(Endpoints.Instance.OverallLoad)
         req_obj, resp_obj = self._send_http(url=url)
         data = orjson.loads(resp_obj.content)
         content = data['availableExecutors']
         if not content:
-            content = "No executors are available."
-        obj = JenkinsDataObject(request=req_obj, content=content)
-        obj._class = data['_class']
-        raw_data = {k: v for k, v in data.items() if k in _fields}
-        obj._raw = raw_data
-        return obj
+            raise JenkinsGeneralException("No executors are available.")
+        return content
 
     @property
-    def executors_in_use(self) -> JenkinsDataObject:
+    def executors_in_use(self) -> str:
         """
         View the executors that are currently being used on the instance.
-        :return:
+
+        :return: Information about the executors in use
+        :rtype: str
+        :raises JenkinsGeneralException: If a general exception occurs.
         """
         _fields = ['_class', 'busyExecutors']
         url = self._build_url(Endpoints.Instance.OverallLoad)
         req_obj, resp_obj = self._send_http(url=url)
         data = orjson.loads(resp_obj.content)
         content = data['busyExecutors']
         if not content:
-            content = "No executors are in-use."
-        obj = JenkinsDataObject(request=req_obj, content=content)
-        obj._class = data['_class']
-        raw_data = {k: v for k, v in data.items() if k in _fields}
-        obj._raw = raw_data
-        return obj
+            raise JenkinsGeneralException("No executors are in-use.")
+        return content
 
     @property
-    def pending_executors(self) -> JenkinsDataObject:
+    def pending_executors(self) -> int:
         """
-        View the executors that are about to run on the instance.
-        :return:
+        View the number of executors that are about to run on the instance.
+
+        :return: Number of pending executors
+        :rtype: int
+        :raises JenkinsGeneralException: If a general exception occurs.
         """
         _fields = ['_class', 'connectingExecutors']
         url = self._build_url(Endpoints.Instance.OverallLoad)
         req_obj, resp_obj = self._send_http(url=url)
         data = orjson.loads(resp_obj.content)
         content = data['connectingExecutors']
         if not content:
-            content = "No executors are connecting."
-        obj = JenkinsDataObject(request=req_obj, content=content)
-        obj._class = data['_class']
-        raw_data = {k: v for k, v in data.items() if k in _fields}
-        obj._raw = raw_data
-        return obj
+            raise JenkinsGeneralException("No executors are connecting.")
+        return content
 
     @property
-    def executor_info(self) -> JenkinsDataObject:
+    def executor_info(self) -> str:
         """
-        View the setup executors on the instance.
-        :return:
+        View information about the setup executors on the instance.
+
+        :return: Information about the setup executors
+        :rtype: str
+        :raises JenkinsGeneralException: If a general exception occurs.
         """
         _fields = ['_class', 'definedExecutors']
         url = self._build_url(Endpoints.Instance.OverallLoad)
         req_obj, resp_obj = self._send_http(url=url)
         data = orjson.loads(resp_obj.content)
         content = data['definedExecutors']
         if not content:
-            content = "No executors are defined."
-        obj = JenkinsDataObject(request=req_obj, content=content)
-        obj._class = data['_class']
-        raw_data = {k: v for k, v in data.items() if k in _fields}
-        obj._raw = raw_data
-        return obj
+            raise JenkinsGeneralException("No executors are defined.")
+        return content
 
     @property
-    def idle_executors(self) -> JenkinsDataObject:
+    def idle_executors(self) -> int:
         """
-        View the idle executors on the instance.
-        :return:
+        View the number of idle executors on the instance.
+
+        :return: Number of idle executors
+        :rtype: int
+        :raises JenkinsGeneralException: If a general exception occurs.
         """
         _fields = ['_class', 'idleExecutors']
         url = self._build_url(Endpoints.Instance.OverallLoad)
         req_obj, resp_obj = self._send_http(url=url)
         data = orjson.loads(resp_obj.content)
         content = data['idleExecutors']
         if not content:
-            content = "No executors are idle."
-        obj = JenkinsDataObject(request=req_obj, content=content)
-        obj._class = data['_class']
-        raw_data = {k: v for k, v in data.items() if k in _fields}
-        obj._raw = raw_data
-        return obj
+            raise JenkinsGeneralException("No executors are idle.")
+        return content
 
     @property
-    def online_executors(self) -> JenkinsDataObject:
+    def online_executors(self) -> int:
         """
-        View the executors that are online, on the instance.
-        :return:
+        View the number of executors that are currently online on the instance.
+
+        :return: Number of online executors
+        :rtype: int
+        :raises JenkinsGeneralException: If a general exception occurs.
         """
         _fields = ['_class', 'onlineExecutors']
         url = self._build_url(Endpoints.Instance.OverallLoad)
         req_obj, resp_obj = self._send_http(url=url)
         data = orjson.loads(resp_obj.content)
         content = data['onlineExecutors']
         if not content:
-            content = "No executors are online."
-        obj = JenkinsDataObject(request=req_obj, content=content)
-        obj._class = data['_class']
-        raw_data = {k: v for k, v in data.items() if k in _fields}
-        obj._raw = raw_data
-        return obj
+            raise JenkinsGeneralException("No executors are online.")
+        return content
 
     @property
-    def queue_size(self) -> JenkinsDataObject:
+    def queue_size(self) -> int:
         """
         View the current queue size on the instance.
-        :return:
+
+        :return: Current queue size
+        :rtype: int
+        :raises JenkinsGeneralException: If a general exception occurs.
         """
         _fields = ['_class', 'queueLength']
         url = self._build_url(Endpoints.Instance.OverallLoad)
         req_obj, resp_obj = self._send_http(url=url)
         data = orjson.loads(resp_obj.content)
         content = data['queueLength']
         if not content:
-            content = "No work in the queue."
-        obj = JenkinsDataObject(request=req_obj, content=content)
-        obj._class = data['_class']
-        raw_data = {k: v for k, v in data.items() if k in _fields}
-        obj._raw = raw_data
-        return obj
+            raise JenkinsGeneralException("No work in the queue.")
+        return content
 
     @property
-    def max_executors(self) -> JenkinsDataObject:
+    def max_executors(self) -> int:
         """
         View the total number of executors on the instance.
-        :return:
+
+        :return: Total number of executors
+        :rtype: int
+        :raises JenkinsGeneralException: If a general exception occurs.
         """
         _fields = ['_class', 'totalExecutors']
         url = self._build_url(Endpoints.Instance.OverallLoad)
         req_obj, resp_obj = self._send_http(url=url)
         data = orjson.loads(resp_obj.content)
         content = data['totalExecutors']
         if not content:
-            content = "No executors are setup."
-        obj = JenkinsDataObject(request=req_obj, content=content)
-        obj._class = data['_class']
-        raw_data = {k: v for k, v in data.items() if k in _fields}
-        obj._raw = raw_data
-        return obj
+            raise JenkinsGeneralException("No executors are setup.")
+        return content
 
     @property
-    def max_queue_size(self) -> JenkinsDataObject:
+    def max_queue_size(self) -> int:
         """
-        View the max queue size on the instance.
-        :return:
+        View the maximum queue size on the instance.
+
+        :return: Maximum queue size
+        :rtype: int
+        :raises JenkinsGeneralException: If a general exception occurs.
         """
         _fields = ['_class', 'totalQueueLength']
         url = self._build_url(Endpoints.Instance.OverallLoad)
         req_obj, resp_obj = self._send_http(url=url)
         data = orjson.loads(resp_obj.content)
         content = data['totalQueueLength']
         if not content:
-            content = "No executors are setup."
-        obj = JenkinsDataObject(request=req_obj, content=content)
-        obj._class = data['_class']
-        raw_data = {k: v for k, v in data.items() if k in _fields}
-        obj._raw = raw_data
-        return obj
+            raise JenkinsGeneralException("No executors are setup.")
+        return content
 
     def restart(self, graceful: bool = False) -> JenkinsActionObject:
         """
         Restart the Jenkins instance.
-        :param graceful: Restart after all jobs have finished.
-        :return: Request outcome.
+
+        :param graceful: (optional) If True, restart after all jobs have finished, defaults to False
+        :type graceful: bool
+        :return: Restart status
+        :rtype: :class:`objects.JenkinsActionObject`
         """
         # TODO: Unit Test
         url = self._build_url(Endpoints.Maintenance.Restart)
         if graceful:
             url = self._build_url(Endpoints.Maintenance.SafeRestart)
 
         req_obj, resp_obj = self._send_http(method="POST", url=url)
@@ -409,26 +468,40 @@
         else:
             msg = f"[{code}] Restarting the Jenkins instance... please wait..."
         restart_obj = JenkinsActionObject(request=req_obj, content=msg, status_code=code)
         restart_obj._raw = resp_obj._raw
         return restart_obj
 
     def _enable_quiet_mode(self) -> JenkinsActionObject:
+        """
+        Enable Quiet Mode on the Jenkins instance.
+
+        :return: Result of the request to enable Quiet Mode
+        :rtype: :class:`objects.JenkinsActionObject`
+        """
         url = self._build_url(Endpoints.Maintenance.QuietDown)
         req_obj, resp_obj = self._send_http(method="POST", url=url, headers=FORM_HEADER_DEFAULT)
         code = resp_obj.status_code
         if code != 200:
             msg = JenkinsActionFailed(f"[{code}] Failed to enable Quiet Mode.")
         else:
             msg = f"[{code}] Successfully enabled Quiet Mode."
         quiet_obj = JenkinsActionObject(request=req_obj, content=msg, status_code=code)
         quiet_obj._raw = resp_obj._raw
         return quiet_obj
 
     def _disable_quiet_mode(self, wait_time: int = 0) -> JenkinsActionObject:
+        """
+        Disable Quiet Mode on the Jenkins instance.
+
+        :param wait_time: (optional) Time to wait before disabling Quiet Mode, in seconds (default is 0)
+        :type wait_time: int
+        :return: Result of the request to disable Quiet Mode
+        :rtype: :class:`objects.JenkinsActionObject`
+        """
         time.sleep(wait_time)
         url = self._build_url(Endpoints.Maintenance.NoQuietDown)
         req_obj, resp_obj = self._send_http(method="POST", url=url, headers=FORM_HEADER_DEFAULT)
         code = resp_obj.status_code
         if code != 200:
             msg = JenkinsActionFailed(f"[{code}] Failed to disable Quiet Mode.")
         else:
@@ -436,23 +509,26 @@
 
         quiet_obj = JenkinsActionObject(request=req_obj, content=msg, status_code=code)
         quiet_obj._raw = resp_obj._raw
         return quiet_obj
 
     def quiet_mode(self, duration: int = None, disable: bool = False) -> JenkinsActionObject:
         """
-        Enable Quiet Mode on the Jenkins instance.
-        :param duration: (Optional) Enable Quiet Mode for X seconds
-        :param disable: Disable Quiet Mode
-        :return: Request outcome.
+        Enable or disable Quiet Mode on the Jenkins instance.
+
+        :param duration: (optional) Enable Quiet Mode for X seconds
+        :type duration: int
+        :param disable: (optional) If True, disable Quiet Mode, defaults to False
+        :type disable: bool
+        :return: Result of the request to enable or disable Quiet Mode
+        :rtype: :class:`objects.JenkinsActionObject`
         """
         # TODO: Fix 403 error
-        # TODO: Run second thread to enable quiet mode for x time
         # TODO: Unit Test
-        # TODO: Add banner message
+        # TODO: Add banner message param
         if disable:
             return self._disable_quiet_mode()
 
         quiet_obj = self._enable_quiet_mode()
         if not quiet_obj.status_code == 200:
             return quiet_obj
 
@@ -463,56 +539,66 @@
                 t_thread.join()
                 quiet_obj.content = f"[{quiet_obj.status_code}] Successfully enabled Quiet Mode for {duration} seconds."
             except:
                 quiet_obj = self._disable_quiet_mode()
                 # TODO: Add log message or something....
         return quiet_obj
 
-    def shutdown(self, graceful=False) -> JenkinsActionObject:
+    def shutdown(self, graceful: bool = False) -> JenkinsActionObject:
+        """
+        Terminate the user's session.
+
+        :param graceful: (Default: False) If True, pause new jobs and wait for all jobs to complete.
+        :type graceful: bool
+        :return: Result of the shutdown request
+        :rtype: :class:`objects.JenkinsActionObject`
+        """
         url = self._build_url(Endpoints.Maintenance.Shutdown)
         if graceful:
             url = self._build_url(Endpoints.Maintenance.SafeShutdown)
 
         req_obj, resp_obj = self._send_http(method="POST", url=url)
         if resp_obj.status_code == 200:
             msg = f"[{resp_obj.status_code}] Shutting down..."
         else:
             msg = f"[{resp_obj.status_code}] Failed to shutdown application."
         obj = JenkinsActionObject(request=req_obj, content=msg, status_code=resp_obj.status_code)
         obj._raw = resp_obj._raw
         return obj
 
-    @property
-    def logout(self) -> JenkinsActionObject:
+    def logout(self, boot: bool = False) -> JenkinsActionObject:
         """
-        Logout of your session.
+        Terminate the user's session.
+
+        :param boot: (Default: False) If True, terminate all the users' sessions. (Caution if it's a service account!)
+        :type boot: bool
+        :return: Result of the logout request
+        :rtype: :class:`objects.JenkinsActionObject`
         """
         url = self._build_url(Endpoints.User.Logout)
+        if boot:
+            url = self._build_url(Endpoints.User.Boot.format(user=self.username))
         req_obj, resp_obj = self._send_http(method="POST", url=url)
         if resp_obj.status_code == 200:
             msg = f"[{resp_obj.status_code}] Successfully logged out."
         else:
             msg = f"[{resp_obj.status_code}] Failed to logout."
         obj = JenkinsActionObject(request=req_obj, content=msg, status_code=resp_obj.status_code)
         obj._raw = resp_obj._raw
         return obj
 
     @property
     def reload(self) -> JenkinsActionObject:
         """
         Reload configuration from disk.
+
+        :return: Result of request
+        :rtype: :class:`objects.JenkinsActionObject`
         """
         url = self._build_url(Endpoints.Manage.Reload)
         req_obj, resp_obj = self._send_http(method="POST", url=url)
         msg = f"[{resp_obj.status_code}] Successfully reloaded configuration."
         if resp_obj.status_code != 200:
             msg = f"[{resp_obj.status_code}] Failed to reload configuration from disk."
         obj = JenkinsActionObject(request=req_obj, content=msg, status_code=resp_obj.status_code)
         obj._raw = resp_obj._raw
         return obj
-
-    class Plugins:
-        pass
-
-if __name__ == "__main__":
-    jenkins = Jenkins(host="http://c0ea-90-194-113-56.ngrok-free.app", username="admin", passw="jenkins")
-    print(jenkins.version)
```

### Comparing `jenkins_pysdk-0.1.1.1.dev0/jenkins_pysdk/jobs.py` & `jenkins_pysdk-0.2/jenkins_pysdk/jobs.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,64 +1,111 @@
 from collections.abc import Generator
 from typing import List
-import orjson
-import pprint
 
+import orjson
 from pydantic import HttpUrl
 
-from jenkins_pysdk.response_objects import JenkinsValidateJob, JenkinsActionObject, Jobs as r_jobs
-from jenkins_pysdk.jenkins_exceptions import JenkinsJobNotFound, JenkinsFolderNotFound, JenkinsGeneralException
+from jenkins_pysdk.objects import JenkinsValidateJob, JenkinsActionObject, Jobs as r_jobs
+from jenkins_pysdk.exceptions import JenkinsJobNotFound, JenkinsFolderNotFound, JenkinsGeneralException
 from jenkins_pysdk.consts import Endpoints, Class, XML_HEADER_DEFAULT, XML_POST_HEADER
 from jenkins_pysdk.builders import Builder
 from jenkins_pysdk.builds import Builds
 
-__all__ = ["Jobs", "Folders"]
+__all__ = ["Jobs", "Folders", "Job", "Folder"]
 
 
 class Job:
-    def __init__(self, /, *, jenkins, job_path, job_url):
+    """
+    Represents a job in Jenkins.
+
+    :param jenkins: The Jenkins instance associated with the job.
+    :type jenkins: Jenkins
+    :param job_path: The path of the job.
+    :type job_path: str
+    :param job_url: The URL of the job.
+    :type job_url: str
+    """
+
+    def __init__(self, *, jenkins, job_path, job_url):
         self._job_path = job_path
         self._job_url = job_url
         self._jenkins = jenkins
 
     @property
     def disable(self) -> JenkinsActionObject:
+        """
+        Disable the job.
+
+        :return: Result of the request to disable the job.
+        :rtype: :class:`objects.JenkinsActionObject`
+        :raises JenkinsGeneralException: If a general exception occurs.
+        """
         url = self._jenkins._build_url(Endpoints.Jobs.Disable, prefix=self._job_url)
         req_obj, resp_obj = self._jenkins._send_http(method="POST", url=url)
         msg = f"[{resp_obj.status_code}] Successfully disabled {self._job_path}."
         if resp_obj.status_code >= 500:
             raise JenkinsGeneralException(f"[{resp_obj.status_code}] Server error.")
         elif resp_obj.status_code != 200:
             msg = f"[{resp_obj.status_code}] Failed to disable {self._job_path}."
         obj = JenkinsActionObject(request=req_obj, content=msg, status_code=resp_obj.status_code)
         obj._raw = resp_obj._raw
         return obj
 
     @property
     def url(self) -> HttpUrl:
+        """
+        Get the URL of the job.
+
+        :return: The URL of the job.
+        :rtype: HttpUrl
+        """
         return HttpUrl(self._job_url)
 
     @property
     def path(self) -> str:
+        """
+        Get the path of the job.
+
+        :return: The path of the job.
+        :rtype: str
+        """
         return self._job_path
 
     @property
     def enable(self) -> JenkinsActionObject:
+        """
+        Enable the job.
+
+        :return: The outcome of enabling the job.
+        :rtype: :class:`objects.JenkinsActionObject`
+        :raises JenkinsGeneralException: If a general exception occurs.
+        """
         url = self._jenkins._build_url(Endpoints.Jobs.Enable, prefix=self._job_url)
         req_obj, resp_obj = self._jenkins._send_http(method="POST", url=url)
         msg = f"[{resp_obj.status_code}] Successfully enabled {self._job_path}."
         if resp_obj.status_code >= 500:
             raise JenkinsGeneralException(f"[{resp_obj.status_code}] Server error.")
         elif resp_obj.status_code != 200:
             msg = f"[{resp_obj.status_code}] Failed to enable {self._job_path}."
         obj = JenkinsActionObject(request=req_obj, content=msg, status_code=resp_obj.status_code)
         obj._raw = resp_obj._raw
         return obj
 
     def reconfig(self, xml: str = None, builder: Builder = None) -> JenkinsActionObject:
+        """
+        Reconfigure the job.
+
+        :param xml: The XML configuration to use for reconfiguration.
+        :type xml: str, optional
+        :param builder: The builder to use for generating XML configuration, defaults to None.
+        :type builder: Builder, optional
+        :return: The outcome of reconfiguring the job.
+        :rtype: :class:`objects.JenkinsActionObject`
+        :raises JenkinsGeneralException: If a general exception occurs.
+        """
         if not xml and not builder:
             raise JenkinsGeneralException("Missing job configuration.")
         url = self._jenkins._build_url(Endpoints.Jobs.Xml, prefix=self._job_url)
         req_obj, resp_obj = self._jenkins._send_http(method="POST", url=url, headers=XML_POST_HEADER,
                                                      data=xml)
         msg = f"[{resp_obj.status_code}] Successfully reconfigured {self._job_path}."
         if resp_obj.status_code >= 500:
@@ -67,56 +114,91 @@
             msg = f"[{resp_obj.status_code}] Failed to reconfigure {self._job_path}."
         obj = JenkinsActionObject(request=req_obj, content=msg, status_code=resp_obj.status_code)
         obj._raw = resp_obj._raw
         return obj
 
     @property
     def delete(self) -> JenkinsActionObject:
+        """
+        Delete the folder.
+
+        :return: Result of the delete operation.
+        :rtype: :class:`objects.JenkinsActionObject`
+        """
         url = self._jenkins._build_url("/", prefix=self._job_url)
         req_obj, resp_obj = self._jenkins._send_http(method="DELETE", url=url)
         msg = f"[{resp_obj.status_code}] Successfully deleted job."
         if resp_obj.status_code != 204:
             msg = f"[{resp_obj.status_code}] Failed to delete job."
         obj = JenkinsActionObject(request=req_obj, content=msg, status_code=resp_obj.status_code)
         obj._raw = resp_obj._raw
         return obj
 
     @property
-    def config(self) -> (str, Exception):
-        url = f"{self._job_url}/{Endpoints.Jobs.Xml}"  # TODO: Fix this
+    def config(self) -> str:
+        """
+        Get the XML configuration of the job.
+
+        :return: The XML configuration of the job.
+        :rtype: str
+        :raises JenkinsGeneralException: If a general exception occurs.
+        """
+        url = self._jenkins._build_url(Endpoints.Jobs.Xml, prefix=self._job_url)
         req_obj, resp_obj = self._jenkins._send_http(url=url, headers=XML_HEADER_DEFAULT)
         code = resp_obj.status_code
         if code != 200:
-            return JenkinsGeneralException(f"[{code}] Failed to download job XML.")
+            raise JenkinsGeneralException(f"[{code}] Failed to download job XML.")
         return resp_obj.content
 
     @property
-    def builds(self):
+    def builds(self) -> Builds:
+        """
+        Access the builds associated with this job.
+
+        :return: Builds associated with this job.
+        :rtype: :class:`builds.Builds`
+        """
         return Builds(self._jenkins, self._job_url)
 
 
 class Jobs:
     def __init__(self, jenkins):
         """
         Interact with Jobs on the Jenkins instance.
-        :param jenkins: Connection to Jenkins instance
+
+        :param jenkins: Connection to Jenkins instance.
+        :type jenkins: Jenkins
         """
         self._jenkins = jenkins
 
     def search(self, job_path: str) -> Job:
+        """
+        Search for a job within Jenkins.
+
+        :param job_path: The path of the job to search for.
+        :type job_path: str
+        :return: The job object.
+        :rtype: :class:`Job`
+        :raises: JenkinsJobNotFound: If the job wasn't found.
+        """
         validated = self._validate_job(job_path)
         if not validated.is_valid:
             raise JenkinsJobNotFound(f"Could not retrieve {job_path} because it doesn't exist.")
         return Job(jenkins=self._jenkins, job_path=job_path, job_url=validated.url)
 
     def is_job(self, path: str) -> bool:
         """
-        Checks if the path is a Folder.
-        :param path: The job path
-        :return:
+        Checks if the path corresponds to a job in Jenkins.
+
+        :param path: The path of the job to check.
+        :type path: str
+        :return: True if the path corresponds to a job, False otherwise.
+        :rtype: bool
+        :raises JenkinsGeneralException: If a general exception occurs.
+        :raises JenkinsJobNotFound: If the job is not found.
         """
         built = self._jenkins._build_job_http_path(path)
         endpoint = f"{built}/{Endpoints.Instance.Standard}"
         url = self._jenkins._build_url(endpoint)
         req_obj, resp_obj = self._jenkins._send_http(url=url)
         if resp_obj.status_code >= 500:
             raise JenkinsGeneralException(f"[{resp_obj.status_code}] Server error.")
@@ -124,15 +206,15 @@
             raise JenkinsJobNotFound(f"[{resp_obj.status_code}] {path} not found.")
         else:
             data = orjson.loads(resp_obj.content)
             if data['_class'] != Class.Folder:
                 return True
             return False
 
-    def _validate_job(self, job_path) -> JenkinsValidateJob:
+    def _validate_job(self, job_path: str) -> JenkinsValidateJob or JenkinsGeneralException:
         job = self._jenkins._build_job_http_path(job_path)
         url = self._jenkins._build_url(job)
         req_obj, resp_obj = self._jenkins._send_http(url=url)
         if resp_obj.status_code == 200:
             validated = True
         elif resp_obj.status_code in (400, 404):
             validated = False
@@ -141,15 +223,16 @@
         if not self.is_job(job_path):
             raise JenkinsGeneralException(f"{job_path} is a folder. Please use folders.")
 
         obj = JenkinsValidateJob(url=url, is_valid=validated)
         obj._raw = resp_obj
         return obj
 
-    def _create_job(self, job_name: str, xml, mode: r_jobs, folder_path: HttpUrl = None) -> JenkinsActionObject:
+    def _create_job(self, job_name: str, xml, mode: r_jobs, folder_path: HttpUrl = None) \
+            -> JenkinsActionObject or JenkinsFolderNotFound:
         create_endpoint = Endpoints.Jobs.Create
         endpoint = f"{folder_path}/{create_endpoint}" if folder_path else create_endpoint
         url = self._jenkins._build_url(endpoint)
         params = {"name": job_name, "mode": mode}
         req_obj, resp_obj = self._jenkins._send_http(method="POST", url=url, headers=XML_HEADER_DEFAULT,
                                                      params=params, data=xml)
         if resp_obj.status_code == 404:
@@ -158,42 +241,66 @@
             msg = f"[{resp_obj.status_code}] Successfully created {job_name}."
         else:
             msg = f"[{resp_obj.status_code}] Failed to create job {job_name}."
         obj = JenkinsActionObject(request=req_obj, content=msg, status_code=resp_obj.status_code)
         obj._raw = resp_obj._raw
         return obj
 
-    def create(self, job_path: str, xml: str or Builder.Freestyle, *args: r_jobs) -> JenkinsActionObject:
+    def create(self, job_path: str, xml: str, *args: r_jobs) -> JenkinsActionObject or JenkinsGeneralException:
+        """
+        Create a job on the Jenkins instance.
+
+        :param job_path: The path where the job should be created.
+        :type job_path: str
+        :param xml: XML configuration for the job.
+        :type xml: str
+        :param args: Additional parameters for job creation.
+        :type args: :class:`objects.Jobs` (Default: Freestyle)
+        :return: Object representing the result of the creation action.
+        :rtype: :class:`objects.JenkinsActionObject`
+        :raises JenkinsGeneralException: If a general exception occurs.
+        """
         try:
             self.is_job(job_path)
             raise JenkinsGeneralException(f"{job_path} already exists.")
         except JenkinsJobNotFound:
             pass
 
+        # TODO: Add all other jobs types
         mode = args[0].value if args else Class.Freestyle
         job_name, job_parent = self._jenkins._get_folder_parent(job_path)
         built = self._jenkins._build_job_http_path(job_parent)
         created = self._create_job(job_name, xml, mode, built)
         return created
 
-    def iter(self, /, folder=None, _paginate=0) -> Generator[Job]:
+    def iter(self, folder=None, _paginate=0) -> Generator[Job]:
+        """
+        Iterate through jobs in the Jenkins instance.
+
+        :param folder: The folder to iterate through. If None, iterate through all jobs.
+        :type folder: str, optional
+        :param _paginate: Pagination flag. Defaults to 0 (disabled).
+        :type _paginate: int, optional
+        :return: Generator yielding Job objects.
+        :rtype: Generator[:class:`Job`]
+        """
         if folder:
             path = self._jenkins._build_job_http_path(folder)
             url = self._jenkins._build_url(path + "/")
             yield from self._fetch_job_iter(url)
         else:
-            url = self._jenkins._build_url("")  # TODO: Remove copy & paste
             start = 0
 
             while True:
                 limit = _paginate + start
-                job_param = f"jobs[fullName,url,jobs[fullName,url,jobs]]"  # TODO: Remove hardcode
-                tree_param = f"{job_param}{{{start},{limit}}}"
-                params = {"tree": tree_param}
-                url = self._jenkins._build_url(Endpoints.Instance.Standard, prefix=url)
+                job_param = Endpoints.Jobs.Iter
+                if _paginate > 0:
+                    job_param = f"{job_param}{{{start},{limit}}}"
+                params = {"tree": job_param}
+                url = self._jenkins._build_url(Endpoints.Instance.Standard)
 
                 req_obj, resp_obj = self._jenkins._send_http(url=url, params=params)
                 if resp_obj.status_code > 200 and start > 0:
                     break  # Pagination finished, Jenkins doesn't return a nice response
 
                 data = orjson.loads(resp_obj.content)
                 data = self._jenkins._validate_url_returned_from_instance(data)
@@ -206,14 +313,16 @@
                         yield from self._fetch_job(item['url'])
 
                 if not jobs:
                     break
 
                 if _paginate > 0:
                     start += _paginate
+                elif _paginate == 0:
+                    break
 
     def _fetch_job_iter(self, job_url) -> Generator[Job]:
         # Pagination not needed here because function repeats itself if needed
         url = self._jenkins._build_url(Endpoints.Instance.Standard, prefix=job_url)
         req_obj, resp_obj = self._jenkins._send_http(url=url)
         data = orjson.loads(resp_obj.content)
         data = self._jenkins._validate_url_returned_from_instance(data)
@@ -231,67 +340,109 @@
         url = self._jenkins._build_url(Endpoints.Instance.Standard, prefix=job_url)
         req_obj, resp_obj = self._jenkins._send_http(url=url)
         data = orjson.loads(resp_obj.content)
         data = self._jenkins._validate_url_returned_from_instance(data)
         yield Job(jenkins=self._jenkins, job_path=data['fullName'], job_url=data['url'])
 
     def list(self, folder=None, _paginate=0) -> List[Job]:
+        """
+        Retrieve a list of jobs from Jenkins.
+
+        :param folder: (Optional) The folder from which to retrieve jobs.
+        :type folder: str or None
+        :param _paginate: (Optional) The number of jobs to retrieve per paginated request.
+            Set to 0 to disable pagination.
+        :type _paginate: int
+        :return: A list of Job objects representing the jobs in the specified folder.
+        :rtype: List[:class:`Job`]
+        """
         return [item for item in self.iter(folder=folder, _paginate=_paginate)]
 
     @property
     def tree(self):
         """
         View all jobs in a pretty tree-like structure.
-        :return:
+
+        :return: Tree-like structure of all jobs.
         """
         raise NotImplemented
 
     def api(self):
         """
         Run your own query and return jobs data objects.
-        :return:
+
+        :return: Jobs data objects.
         """
         raise NotImplemented
 
 
 class Folder:
-    def __init__(self, /, *, jenkins, folder_path, folder_url):
+    def __init__(self, *, jenkins, folder_path, folder_url):
         """
         Interact with Folders on the Jenkins instance.
+
         :param jenkins: Connection to Jenkins instance
         """
         self._folder_path = folder_path
         self._folder_url = folder_url
         self._jenkins = jenkins
 
     def reconfig(self, xml: str or Builder.Folder) -> JenkinsActionObject:
+        """
+        Reconfigure the folder.
+
+        :param xml: The XML configuration or Builder.Folder object.
+        :type xml: str or Builder.Folder
+        :return: Action outcome
+        :rtype: :class:`objects.JenkinsActionObject`
+        :raises JenkinsGeneralException: If a general exception occurs.
+        """
         url = self._jenkins._build_url(Endpoints.Jobs.Xml, prefix=self._folder_url)
         req_obj, resp_obj = self._jenkins._send_http(method="POST", url=url, headers=XML_POST_HEADER,
                                                      data=xml)
         msg = f"[{resp_obj.status_code}] Successfully reconfigured {self._folder_path}."
         if resp_obj.status_code >= 500:
             raise JenkinsGeneralException(f"[{resp_obj.status_code}] Server error.")
         elif resp_obj.status_code != 200:
             msg = f"[{resp_obj.status_code}] Failed to reconfigure {self._folder_path}."
         obj = JenkinsActionObject(request=req_obj, content=msg, status_code=resp_obj.status_code)
         obj._raw = resp_obj._raw
         return obj
 
     @property
     def url(self) -> HttpUrl:
+        """
+        Get the URL of the folder.
+
+        :return: The URL of the folder.
+        :rtype: HttpUrl
+        """
         return HttpUrl(self._folder_url)
 
     @property
     def path(self) -> str:
+        """
+        Get the path of the folder.
+
+        :return: The path of the folder.
+        :rtype: str
+        """
         return self._folder_path
 
     def copy(self, new_job_name: str, copy_job_name: str) -> JenkinsActionObject:
         """
         Copy an item into the existing path.
-        :return:
+
+        :param new_job_name: The name of the new job.
+        :type new_job_name: str
+        :param copy_job_name: The name of the job to copy.
+        :type copy_job_name: str
+        :return: Result of the copy operation.
+        :rtype: :class:`objects.JenkinsActionObject`
+        :raises JenkinsGeneralException: If a general exception occurs.
         """
         import re
         params = {"name": new_job_name, "mode": "copy", "from": copy_job_name}
         url = self._jenkins._build_url(Endpoints.Jobs.Create, prefix=self._folder_url)
         req_obj, resp_obj = self._jenkins._send_http(method="POST", url=url, params=params)
         msg = f"[{resp_obj.status_code}] Successfully copied {copy_job_name} to {new_job_name}."
         if resp_obj.status_code >= 500:
@@ -304,65 +455,91 @@
             msg = f"[{resp_obj.status_code}] Failed to copy folder."
         obj = JenkinsActionObject(request=req_obj, content=msg, status_code=resp_obj.status_code)
         obj._raw = resp_obj._raw
         return obj
 
     @property
     def delete(self) -> JenkinsActionObject:
+        """
+        Delete the folder.
+
+        :return: Result of the delete operation.
+        :rtype: :class:`objects.JenkinsActionObject`
+        :raises JenkinsGeneralException: If a general exception occurs.
+        """
         url = self._jenkins._build_url("/", prefix=self._folder_url)
         req_obj, resp_obj = self._jenkins._send_http(method="DELETE", url=url)
         msg = f"[{resp_obj.status_code}] Successfully deleted folder."
         if resp_obj.status_code >= 500:
             raise JenkinsGeneralException(f"[{resp_obj.status_code}] Server error.")
         elif resp_obj.status_code != 204:
             msg = f"[{resp_obj.status_code}] Failed to delete folder."
         obj = JenkinsActionObject(request=req_obj, content=msg, status_code=resp_obj.status_code)
         obj._raw = resp_obj._raw
         return obj
 
     def create(self, folder_name: str, xml: str or Builder.Folder) -> JenkinsActionObject:
         """
         Creates sub-folders in the current path.
-        :return:
-        """
-        # TODO: Test this!!!!!!!!!!!!! Folders(self)?
-        built_path = self._jenkins._build_job_http_path(folder_name)
-        try:
-            Folders(self).search(built_path)
-            raise JenkinsGeneralException(f"{folder_name} already exists.")
-        except JenkinsFolderNotFound:
-            pass
 
+        :param folder_name: The name of the folder to create.
+        :type folder_name: str
+        :param xml: The XML configuration for the folder. Can be a string or a Builder.Folder object.
+        :type xml: str or Builder.Folder
+        :return: The result of the action.
+        :rtype: :class:`objects.JenkinsActionObject`
+        :raises JenkinsGeneralException: If a general exception occurs.
+        """
         try:
-            return Folders(self)._create_folder(folder_name, xml, built_path)
+            return Folders(self._jenkins)._create_folder(folder_name, xml, self.path)
         except:
             raise
 
     @property
-    def config(self) -> (str, Exception):
+    def config(self) -> str:
+        """
+        Get the XML configuration of the folder.
+
+        :return: The XML configuration of the folder.
+        :rtype: str
+        :raises JenkinsGeneralException: If a general exception occurs.
+        """
         url = self._jenkins._build_url(Endpoints.Jobs.Xml, prefix=self._folder_url)
         req_obj, resp_obj = self._jenkins._send_http(url=url, headers=XML_HEADER_DEFAULT)
         code = resp_obj.status_code
         if code != 200:
-            return JenkinsGeneralException(f"[{code}] Failed to download job XML.")
+            raise JenkinsGeneralException(f"[{code}] Failed to download job XML.")
         return resp_obj.content
 
 
 class Folders:
     def __init__(self, jenkins):
+        """
+        Interact with Folders on the Jenkins instance.
+
+        :param jenkins: Connection to Jenkins instance.
+        """
         self._jenkins = jenkins
 
     def search(self, folder_path: str) -> Folder:
+        """
+        Search for a folder within the Jenkins instance.
+
+        :param folder_path: The path of the folder to search for.
+        :type folder_path: str
+        :return: The folder object if found.
+        :rtype: :class:`Folder`
+        :raises JenkinsFolderNotFound: If the folder was not found.
+        """
         validated = self._validate_job(folder_path)
         if not validated.is_valid:
             raise JenkinsFolderNotFound(f"Could not retrieve {folder_path} because it doesn't exist.")
         return Folder(jenkins=self._jenkins, folder_path=folder_path, folder_url=validated.url)
 
     def _validate_job(self, job_path) -> JenkinsValidateJob:
-        # TODO: Change to /checkJobName
         job = self._jenkins._build_job_http_path(job_path)
         url = self._jenkins._build_url(job)
         req_obj, resp_obj = self._jenkins._send_http(url=url)
         if resp_obj.status_code == 200:
             validated = True
         elif resp_obj.status_code in (400, 404):
             validated = False
@@ -371,111 +548,126 @@
         if not self.is_folder(job_path):
             raise JenkinsGeneralException(f"{job_path} is not a folder. Please use jobs.")
 
         obj = JenkinsValidateJob(url=url, is_valid=validated)
         obj._raw = resp_obj
         return obj
 
-    def is_folder(self, path: str) -> (bool, Exception):
+    def is_folder(self, path: str) -> bool:
         """
-        Checks if the path is a Folder.
-        :param path: The job path
-        :return:
+        Checks if the path corresponds to a folder in Jenkins.
+
+        :param path: The path to check.
+        :type path: str
+        :return: True if the path corresponds to a folder, False otherwise.
+        :rtype: bool
+        :raises JenkinsGeneralException: If a general exception occurs.
         """
         built = self._jenkins._build_job_http_path(path)
-        endpoint = f"{built}/{Endpoints.Instance.Standard}"
-        url = self._jenkins._build_url(endpoint)
+        url = self._jenkins._build_url(built, suffix=Endpoints.Instance.Standard)
         req_obj, resp_obj = self._jenkins._send_http(url=url)
         if resp_obj.status_code >= 500:
             raise JenkinsGeneralException(f"[{resp_obj.status_code}] Server error.")
         elif resp_obj.status_code != 200:
             raise JenkinsFolderNotFound(f"{path} not found.")
         data = orjson.loads(resp_obj.content)
         if data['_class'] == Class.Folder:
             return True
         return False
 
-    def _create_folder(self, folder_name: str, xml, folder_path: HttpUrl = None) -> JenkinsActionObject:
-        create_endpoint = Endpoints.Jobs.Create
-        endpoint = f"{folder_path}/{create_endpoint}" if folder_path else create_endpoint
-        url = self._jenkins._build_url(endpoint)
+    def _create_folder(self, folder_name: str, xml, folder_path: str = None) -> JenkinsActionObject:
+        endpoint = self._jenkins._build_job_http_path(folder_path)
+        url = self._jenkins._build_url(endpoint, suffix=Endpoints.Jobs.Create)
         params = {"name": folder_name, "mode": Class.Folder}
         req_obj, resp_obj = self._jenkins._send_http(method="POST", url=url, headers=XML_HEADER_DEFAULT,
                                                      params=params, data=xml)
         if resp_obj.status_code == 404:
             raise JenkinsFolderNotFound(f"Parent path {str(folder_path)} not found.")
         elif resp_obj.status_code == 200:
             msg = f"[{resp_obj.status_code}] Successfully created {folder_name}."
         else:
             msg = f"[{resp_obj.status_code}] Failed to create folder {folder_name}."
         obj = JenkinsActionObject(request=req_obj, content=msg, status_code=resp_obj.status_code)
         obj._raw = resp_obj._raw
         return obj
 
-    def create(self, folder_path: str, xml: str or Builder.Folder) -> (JenkinsActionObject, Exception):
+    def create(self, folder_path: str, xml: str or Builder.Folder) -> JenkinsActionObject:
         """
-        Creates sub-folders from the root path.
-        :param folder_path:
-        :param folder_path:
-        :param xml:
-        :return:
+        Creates a folder at the specified path with the given XML configuration.
+
+        :param folder_path: The path where the folder will be created.
+        :type folder_path: str
+        :param xml: The XML configuration for the folder.
+        :type xml: str or Builder.Folder
+        :return: The result of the folder creation operation.
+        :rtype: :class:`objects.JenkinsActionObject`
+        :raises JenkinsFolderNotFound: If the folder was not found.
         """
         folder_name, folder_parent = self._jenkins._get_folder_parent(folder_path)
-        
+
         try:
             built_path = self._jenkins._build_job_http_path(folder_name, folder_parent)
             self.search(built_path)
             raise JenkinsGeneralException(f"{folder_path} already exists.")
         except JenkinsFolderNotFound:
             pass
 
         try:
             built_path = self._jenkins._build_job_http_path(folder_parent)
             return self._create_folder(folder_name, xml, built_path)
         except JenkinsFolderNotFound as error:
             if not self.is_folder(folder_parent):
                 raise JenkinsFolderNotFound(f"Failed to create folder because parent path not found: {folder_parent}.")
             raise error
-        except Exception as e:
-            raise e
 
-    def iter(self, /, folder=None, _paginate=0) -> Generator[Folder]:
+    def iter(self, folder: str = None, _paginate: int = 0) -> Generator[Folder]:
+        """
+        Iterate over folders within the specified folder.
+
+        :param folder: The path of the parent folder. If None, iterate over all folders.
+        :type folder: str, optional
+        :param _paginate: Number of items to paginate. Default is 0 (no pagination).
+        :type _paginate: int, optional
+        :return: A generator yielding Folder objects.
+        :rtype: Generator[:class:`Folder`]
+        """
         if folder:
             path = self._jenkins._build_job_http_path(folder)
             url = self._jenkins._build_url(path + "/")
             yield from self._fetch_folder_iter(url)
         else:
-            url = self._jenkins._build_url("")  # TODO: Remove copy & paste
             start = 0
 
             while True:
                 limit = _paginate + start
-                job_param = f"jobs[fullName,url,jobs[fullName,url,jobs]]"  # TODO: Remove hardcode
-                tree_param = f"{job_param}{{{start},{limit}}}"
-                params = {"tree": tree_param}
-                json_url = self._jenkins._build_url(Endpoints.Instance.Standard, prefix=url)
+                job_param = Endpoints.Jobs.Iter
+                if _paginate > 0:
+                    job_param = f"{job_param}{{{start},{limit}}}"
+                params = {"tree": job_param}
+                json_url = self._jenkins._build_url(Endpoints.Instance.Standard)
 
                 req_obj, resp_obj = self._jenkins._send_http(url=json_url, params=params)
                 if resp_obj.status_code > 200 and start > 0:
                     break  # Pagination finished, Jenkins doesn't return a nice response
 
                 data = orjson.loads(resp_obj.content)
                 data = self._jenkins._validate_url_returned_from_instance(data)
 
                 folders = data.get('jobs', [])
                 for item in folders:
                     if item['_class'] == Class.Folder:
-                        yield from self._fetch_folder(item['url'])  # TODO: Revise.. do we want to return data like this?
                         yield from self._fetch_folder_iter(item['url'])
 
                 if not folders:
                     break
 
                 if _paginate > 0:
                     start += _paginate
+                elif _paginate == 0:
+                    break
 
     def _fetch_folder_iter(self, folder_url) -> Generator[Folder]:
         json_url = self._jenkins._build_url(Endpoints.Instance.Standard, prefix=folder_url)
         req_obj, resp_obj = self._jenkins._send_http(url=json_url)
         data = orjson.loads(resp_obj.content)
         data = self._jenkins._validate_url_returned_from_instance(data)
 
@@ -493,23 +685,36 @@
         json_url = self._jenkins._build_url(Endpoints.Instance.Standard, prefix=folder_url)
         req_obj, resp_obj = self._jenkins._send_http(url=json_url)
         data = orjson.loads(resp_obj.content)
         data = self._jenkins._validate_url_returned_from_instance(data)
         yield Folder(jenkins=self._jenkins, folder_path=data['fullName'], folder_url=data['url'])
 
     def list(self, folder=None, _paginate=0) -> List[Folder]:
+        """
+        Retrieve a list of folder from Jenkins.
+
+        :param folder: (Optional) The folder from which to retrieve jobs.
+        :type folder: str or None
+        :param _paginate: (Optional) The number of jobs to retrieve per paginated request.
+            Set to 0 to disable pagination.
+        :type _paginate: int
+        :return: A list of Job objects representing the jobs in the specified folder.
+        :rtype: List[:class:`Folder`]
+        """
         return [item for item in self.iter(folder=folder, _paginate=_paginate)]
 
     @property
     def tree(self):
         """
-        View all Folders in a pretty tree-like structure.
-        :return:
+        Get a hierarchical representation of all folders.
+
+        :return: A tree-like structure representing all folders.
         """
         raise NotImplemented
 
     def api(self):
         """
-        Run your own query and return folders' data objects.
-        :return:
+        Run a custom query and return folder data objects.
+
+        :return: Data objects representing folders.
         """
         raise NotImplemented
```

### Comparing `jenkins_pysdk-0.1.1.1.dev0/jenkins_pysdk/utils.py` & `jenkins_pysdk-0.2/jenkins_pysdk/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import re
 import time
 
 from httpx import Client, Request, ConnectError, BasicAuth
 from pydantic import HttpUrl
 
-from jenkins_pysdk.consts import HTTP_RETRY_COUNT, HOST_MATCH_REGEX_PATTERN, HTTP_REQUEST_PARAMETERS
-from jenkins_pysdk.response_objects import HTTPRequestObject, HTTPResponseObject, HTTPSessionRequestObject, \
+from jenkins_pysdk.consts import HTTP_RETRY_COUNT, HOST_MATCH_REGEX_PATTERN
+from jenkins_pysdk.objects import HTTPRequestObject, HTTPResponseObject, HTTPSessionRequestObject, \
     HTTPSessionResponseObject
-from jenkins_pysdk.jenkins_exceptions import JenkinsInvalidHost, JenkinsConnectionException
+from jenkins_pysdk.exceptions import JenkinsInvalidHost
+from _logger import logger
 
 __all__ = ["validate_connect_host", "validate_http_url", "interact_http", "interact_http_session"]
 
 
 def validate_connect_host(host: str) -> bool:
     """
 
@@ -32,102 +33,94 @@
     try:
         result = parse_url(str(url))
         return all([result.scheme, result.netloc])
     except ValueError:
         return False
 
 
-def interact_http(request: HTTPRequestObject) -> (HTTPResponseObject, Exception):
-    """
-
-    :param request:
-    :return:
-    """
+def interact_http(request: HTTPRequestObject) -> HTTPResponseObject:
     # TODO: Add retry option in HTTPRequestObject and Jenkins __init__??
     # TODO: should this be in utils :(
     if validate_http_url(request.url) is False:
-        return JenkinsInvalidHost(f"{request.url.host} is not a valid target.")
-
+        raise JenkinsInvalidHost(f"{request.url.host} is not a valid target.")
     req = Request(
         method=request.method,
         url=str(request.url),
         headers=request.headers if request.headers else None,
         data=request.data if request.data else None,
         params=request.params if request.params else None
     )
+    logger.debugu(req.url)
     exception = None
     for retry in range(HTTP_RETRY_COUNT):
         try:
             # TODO: SSL/certs
             # TODO: Dynamically add these parameters from the request object
             # TODO: TIDY
-            # TODO: ADD URLENCODE?
             with Client(auth=BasicAuth(request.username, request.passw_or_token),
-                        verify=request.verify, proxies=request.proxy) as conn:
+                        verify=request.verify, proxies=request.proxy, timeout=request.timeout) as conn:
                 response = conn.send(request=req, follow_redirects=True)
-                return_object = HTTPResponseObject(request=req, response=response, content=response.text,
+                return_object = HTTPResponseObject(request=req, content=response.text,
                                                    status_code=int(response.status_code))
-                return_object._raw = response.content
+                return_object._raw = response
+                logger.debuge(response.content)
                 return return_object
         except (EnvironmentError, ConnectError) as error:
             # TODO: below lines suck
             exception = error
             time.sleep(1)
             continue
         except TimeoutError as error:
             raise error
     else:
-        msg = "Request failed due to an exception."
-        return_object = HTTPResponseObject(request=req, response=exception, content=msg, status_code=-1)
+        msg = "Request failed due to an exception. See _raw field."
+        return_object = HTTPResponseObject(request=req, content=msg, status_code=-1)
         return_object._raw = exception
+        logger.debuge(exception)
         return return_object
 
 
-def interact_http_session(request: HTTPSessionRequestObject) -> (HTTPSessionResponseObject, Exception):
-    """
-
-    :param request:
-    :return:
-    """
+def interact_http_session(request: HTTPSessionRequestObject) -> HTTPSessionResponseObject:
     if validate_http_url(request.url) is False:
-        return JenkinsInvalidHost(f"{request.url.host} is not a valid target.")
+        raise JenkinsInvalidHost(f"{request.url.host} is not a valid target.")
 
     req = Request(
         method=request.method,
         url=str(request.url),
         headers=request.headers,
         data=request.data,
         params=request.params,
     )
-    exception = None
+    logger.debugu(req.url)
+    exception: Exception = Exception()
     for retry in range(HTTP_RETRY_COUNT):
         # TODO: SSL/certs
         # TODO: Dynamically add these parameters from the request object
         # TODO: TIDY
-        # TODO: ADD URLENCODE?
-        # TODO: Investigate max redirects a maybe fix for 503/restarting
         if request.session:
             session = request.session
         else:
             session = Client(auth=BasicAuth(request.username, request.passw_or_token),
                              verify=request.verify, proxies=request.proxy, timeout=request.timeout)
         try:
             response = session.send(request=req, follow_redirects=True)
-            return_object = HTTPSessionResponseObject(request=req, response=response, content=response.text,
+            return_object = HTTPSessionResponseObject(request=req, content=response.text,
                                                       status_code=int(response.status_code), session=session)
-            return_object._raw = response.content
+            return_object._raw = response
+            logger.debuge(response.content)
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
-        msg = "Request failed due to an exception. See _raw field..."
-        return_object = HTTPSessionResponseObject(request=req, response=exception, content=msg, status_code=-1)
+        msg = "Request failed due to an exception. See _raw field."
+        return_object = HTTPSessionResponseObject(request=req, content=msg, status_code=-1, session=None)
         return_object._raw = exception
+        logger.debuge(exception)
         return return_object
```

### Comparing `jenkins_pysdk-0.1.1.1.dev0/jenkins_pysdk/views.py` & `jenkins_pysdk-0.2/jenkins_pysdk/views.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,69 @@
 from collections.abc import Generator
 from typing import List
 import orjson
-import pprint
 
 from pydantic import HttpUrl
 
-from jenkins_pysdk.response_objects import JenkinsValidateJob, JenkinsActionObject, Views as r_views
-from jenkins_pysdk.jenkins_exceptions import JenkinsViewNotFound, JenkinsGeneralException
+from jenkins_pysdk.objects import JenkinsValidateJob, JenkinsActionObject
+from jenkins_pysdk.exceptions import JenkinsNotFound, JenkinsGeneralException
 from jenkins_pysdk.consts import Endpoints, Class, XML_HEADER_DEFAULT, XML_POST_HEADER
 from jenkins_pysdk.builders import Builder
 
 __all__ = ["Views"]
 
 
 class View:
-    def __init__(self, /, *, jenkins, name, url):
+    def __init__(self, *, jenkins, name, url):
+        """
+        Interact with Views on the Jenkins instance.
+
+        :param jenkins: Connection to Jenkins instance.
+        :type jenkins: Jenkins
+        :param name: The name of the view.
+        :type name: str
+        :param url: The URL of the view.
+        :type url: HttpUrl
+        """
         self._jenkins = jenkins
         self._view_name = name
         self._view_url = url
 
     @property
     def url(self) -> HttpUrl:
+        """
+        Get the URL of the view.
+
+        :return: The URL of the view.
+        :rtype: HttpUrl
+        """
         return HttpUrl(self._view_url)
 
     @property
     def name(self) -> str:
-        return self._view_name
+        """
+        Get the name of the view.
+
+        :return: The name of the view.
+        :rtype: str
+        """
+        return str(self._view_name)
 
     def reconfig(self, xml: str = None, builder: Builder.View = None) -> JenkinsActionObject:
+        """
+        Reconfigure the view with XML configuration or a builder.
+
+        :param xml: The XML configuration of the view, defaults to None.
+        :type xml: str, optional
+        :param builder: The builder object to build the view, defaults to None.
+        :type builder: Builder.View, optional
+        :return: Jenkins action object indicating the reconfiguration status.
+        :rtype: :class:`objects.JenkinsActionObject`
+        :raises JenkinsGeneralException: If a general exception occurs.
+        """
         if not xml and not builder:
             raise JenkinsGeneralException("Missing view configuration.")
         url = self._jenkins._build_url(Endpoints.Jobs.Xml, prefix=self._view_url)
         req_obj, resp_obj = self._jenkins._send_http(method="POST", url=url, headers=XML_POST_HEADER,
                                                      data=xml)
         msg = f"[{resp_obj.status_code}] Successfully reconfigured {self._view_name}."
         if resp_obj.status_code >= 500:
@@ -39,63 +71,89 @@
         elif resp_obj.status_code != 200:
             msg = f"[{resp_obj.status_code}] Failed to reconfigure {self._view_name}."
         obj = JenkinsActionObject(request=req_obj, content=msg, status_code=resp_obj.status_code)
         obj._raw = resp_obj._raw
         return obj
 
     @property
-    def delete(self):
+    def delete(self) -> JenkinsActionObject:
+        """
+        Delete the view.
+
+        :return: Jenkins action object indicating the delete status.
+        :rtype: :class:`objects.JenkinsActionObject`
+        """
         url = self._jenkins._build_url("/", prefix=self._view_url)
         req_obj, resp_obj = self._jenkins._send_http(method="DELETE", url=url)
         msg = f"[{resp_obj.status_code}] Successfully deleted view."
         if resp_obj.status_code != 204:
             msg = f"[{resp_obj.status_code}] Failed to delete view."
         obj = JenkinsActionObject(request=req_obj, content=msg, status_code=resp_obj.status_code)
         obj._raw = resp_obj._raw
         return obj
 
     @property
-    def config(self):
-        url = f"{self._view_url}/{Endpoints.Jobs.Xml}"  # TODO: Fix this
+    def config(self) -> str:
+        """
+        Get the XML configuration of the view.
+
+        :return: The XML configuration of the view.
+        :rtype: str
+        :raises JenkinsGeneralException: If a general exception occurs.
+        """
+        url = self._jenkins._build_url(Endpoints.Jobs.Xml, prefix=self._view_url)
         req_obj, resp_obj = self._jenkins._send_http(url=url, headers=XML_HEADER_DEFAULT)
         code = resp_obj.status_code
         if code != 200:
-            return JenkinsGeneralException(f"[{code}] Failed to download view XML.")
+            raise JenkinsGeneralException(f"[{code}] Failed to download view XML.")
         return resp_obj.content
 
 
 class Views:
     def __init__(self, jenkins):
         """
-        Interact with Jobs on the Jenkins instance.
-        :param jenkins: Connection to Jenkins instance
+        Interact with Views on the Jenkins instance.
+
+        :param jenkins: Connection to the Jenkins instance.
         """
         self._jenkins = jenkins
 
     def search(self, view_path: str) -> View:
-        # TODO: Get view_name from API as resutls are won't be consistent with User Views
+        """
+        Search for a view within Jenkins.
+
+        :param view_path: The path of the view to search for.
+        :type view_path: str
+        :return: The View object representing the found view.
+        :rtype: View
+        :raises JenkinsNotFound: If the view was not found.
+        """
+        # TODO: Get view_name from API as results won't be consistent with User Views
         validated = self._validate_view(view_path)
         if not validated.is_valid:
-            raise JenkinsViewNotFound(f"Could not retrieve {view_path} because it doesn't exist.")
+            raise JenkinsNotFound(f"Could not retrieve {view_path} because it doesn't exist.")
         return View(jenkins=self._jenkins, name=view_path, url=validated.url)
 
     def is_view(self, path: str) -> bool:
         """
-        Checks if the path is a Folder.
-        :param path: The job path
-        :return:
+        Check if the specified path is a view.
+
+        :param path: The path to check.
+        :type path: str
+        :return: True if the path corresponds to a view, False otherwise.
+        :rtype: bool
+        :raises JenkinsNotFound: If the view was not found.
         """
         built = self._jenkins._build_view_http_path(path)
-        endpoint = f"{built}/{Endpoints.Instance.Standard}"
-        url = self._jenkins._build_url(endpoint)
+        url = self._jenkins._build_url(built, suffix=Endpoints.Instance.Standard)
         req_obj, resp_obj = self._jenkins._send_http(url=url)
         if resp_obj.status_code >= 500:
             raise JenkinsGeneralException(f"[{resp_obj.status_code}] Server error.")
         elif resp_obj.status_code == 404:
-            raise JenkinsViewNotFound(f"[{resp_obj.status_code}] {path} not found.")
+            raise JenkinsNotFound(f"[{resp_obj.status_code}] {path} not found.")
         else:
             data = orjson.loads(resp_obj.content)
             if data['_class'] != Class.Folder:
                 return True
             return False
 
     def _validate_view(self, view_path) -> JenkinsValidateJob:  # TODO: Review what the heck this is doing?
@@ -111,112 +169,142 @@
         if not self.is_view(view_path):
             raise JenkinsGeneralException(f"{view_path} is not a view.")
 
         obj = JenkinsValidateJob(url=url, is_valid=validated)
         obj._raw = resp_obj
         return obj
 
-    def _create_view(self, view_name: str, xml, mode: r_views) -> JenkinsActionObject:
-        # TODO: Add mode with params
-
-        # url = self._jenkins._build_url(Endpoints.Views.Create)
-        # params = {"name": view_name, "mode": mode}
-        params = {"mode": mode}
-        url = self._jenkins._build_url(f"/{view_name}")
+    def _create_view(self, view_name: str, xml) -> JenkinsActionObject:
+        params = {"name": view_name}
+        url = self._jenkins._build_url(Endpoints.Views.Create)
 
         req_obj, resp_obj = self._jenkins._send_http(method="POST", url=url, headers=XML_POST_HEADER,
-                                                     params=params, data=xml)
+                                                     params=params, data=str(xml))
         if resp_obj.status_code == 200:
             msg = f"[{resp_obj.status_code}] Successfully created {view_name}."
+        elif resp_obj.status_code == 400:
+            msg = f"[{resp_obj.status_code}] Bad request for {view_name}."
         else:
             msg = f"[{resp_obj.status_code}] Failed to create view {view_name}."
         obj = JenkinsActionObject(request=req_obj, content=msg, status_code=resp_obj.status_code)
         obj._raw = resp_obj._raw
         return obj
 
-    def create(self, name: str, xml: str or Builder.View, *args: r_views) -> JenkinsActionObject:
+    def create(self, name: str, xml: str or Builder.View) -> JenkinsActionObject:
+        """
+        Create a new view.
+
+        :param name: The name of the new view.
+        :type name: str
+        :param xml: The XML configuration or Builder.View object for the new view.
+        :type xml: str or Builder.View
+        :return: JenkinsActionObject indicating the result of the creation.
+        :rtype: :class:`objects.JenkinsActionObject`
+        :raises JenkinsGeneralException: If a general exception occurs.
+        """
         try:
             self.is_view(name)
             raise JenkinsGeneralException(f"{name} already exists.")
-        except JenkinsViewNotFound:
+        except JenkinsNotFound:
             pass
 
-        mode = args[0].value if args else Class.ListView
-        created = self._create_view(name, xml, mode)
+        created = self._create_view(name, xml)
         return created
 
-    def iter(self, /, folder=None, _paginate=0) -> Generator[View]:
+    def iter(self, folder: str = None, _paginate=0) -> Generator[View]:
+        """
+        Iterate through views.
+
+        :param folder: Check if folder is in a view. Default is None.
+        :type folder: str, optional
+        :param _paginate: Pagination option. Default is 0 (no pagination).
+        :type _paginate: int, optional
+        :return: A generator yielding View objects.
+        :rtype: Generator[:class:`View`]
+        """
         if folder:
             path = self._jenkins._build_job_http_path(folder)
             url = self._jenkins._build_url(path + "/")
             yield from self._fetch_view_iter(url)
         else:
-            url = self._jenkins._build_url("")  # TODO: Remove copy & paste
             start = 0
 
             while True:
                 limit = _paginate + start
-                job_param = f"views[fullName,url,jobs[fullName,url,jobs]]"  # TODO: Remove hardcode
-                tree_param = f"{job_param}{{{start},{limit}}}"
-                params = {"tree": tree_param}
-                url = self._jenkins._build_url(Endpoints.Instance.Standard, prefix=url)
+                job_param = Endpoints.Views.Iter
+                if _paginate > 0:
+                    job_param = f"{job_param}{{{start},{limit}}}"
+                params = {"tree": job_param}
+                url = self._jenkins._build_url(Endpoints.Instance.Standard)
 
                 req_obj, resp_obj = self._jenkins._send_http(url=url, params=params)
                 if resp_obj.status_code > 200 and start > 0:
                     break  # Pagination finished, Jenkins doesn't return a nice response
 
                 data = orjson.loads(resp_obj.content)
                 data = self._jenkins._validate_url_returned_from_instance(data)
 
-                jobs = data.get('jobs', [])
-                for item in jobs:
-                    if item['_class'] == Class.Folder:
-                        yield from self._fetch_view_iter(item['url'])
-                    elif item['_class'] != Class.Folder:
-                        yield from self._fetch_view(item['url'])
-
-                if not jobs:
+                views = data.get('views', [])
+                if not views:
                     break
 
+                for item in views:
+                    # yield from self._fetch_view(item['url'])
+                    yield View(jenkins=self._jenkins, name=item['name'], url=item['url'])
+
                 if _paginate > 0:
                     start += _paginate
+                elif _paginate == 0:
+                    break
 
     def _fetch_view_iter(self, job_url) -> Generator[View]:
         # Pagination not needed here because function repeats itself if needed
         url = self._jenkins._build_url(Endpoints.Instance.Standard, prefix=job_url)
         req_obj, resp_obj = self._jenkins._send_http(url=url)
         data = orjson.loads(resp_obj.content)
         data = self._jenkins._validate_url_returned_from_instance(data)
 
-        try:
-            if data['_class'] != Class.Folder:
-                yield View(jenkins=self._jenkins, name=data['fullName'], url=data['url'])
-            elif data['_class'] == Class.Folder:
-                for item in data.get('jobs', []):
-                    yield from self._fetch_view_iter(item['url'])
-        except Exception as error:
-            print(error)
+        views = data.get('views', [])
+        if not views:
+            return
+
+        for item in views:
+            yield View(jenkins=self._jenkins, name=item['name'], url=item['url'])
 
     def _fetch_view(self, view_url) -> Generator[View]:
         url = self._jenkins._build_url(Endpoints.Instance.Standard, prefix=view_url)
         req_obj, resp_obj = self._jenkins._send_http(url=url)
         data = orjson.loads(resp_obj.content)
         data = self._jenkins._validate_url_returned_from_instance(data)
-        yield View(jenkins=self._jenkins, name=data['fullName'], url=data['url'])
+        yield View(jenkins=self._jenkins, name=data['name'], url=data['url'])
 
-    def list(self, folder=None, _paginate=0) -> List[View]:
+    def list(self, folder: str = None, _paginate=0) -> List[View]:
+        """
+        List all views.
+
+        :param folder: Folder to iterate through. Default is None.
+        :type folder: str, optional
+        :param _paginate: Pagination option. Default is 0 (no pagination).
+        :type _paginate: int, optional
+        :return: A list of View objects.
+        :rtype: List[:class:`View`]
+        """
         return [item for item in self.iter(folder=folder, _paginate=_paginate)]
 
     @property
     def tree(self):
         """
-        View all jobs in a pretty tree-like structure.
-        :return:
+        View all views in a pretty tree-like structure.
+
+        :return: None
+        :rtype: None
         """
         raise NotImplemented
 
     def api(self):
         """
-        Run your own query and return jobs data objects.
-        :return:
+        Run your own query and return views data objects.
+
+        :return: None
+        :rtype: None
         """
         raise NotImplemented
```

### Comparing `jenkins_pysdk-0.1.1.1.dev0/jenkins_pysdk.egg-info/SOURCES.txt` & `jenkins_pysdk-0.2/jenkins_pysdk.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 LICENSE
 README.md
 setup.py
 jenkins_pysdk/__init__.py
+jenkins_pysdk/_logger.py
 jenkins_pysdk/builders.py
 jenkins_pysdk/builds.py
 jenkins_pysdk/consts.py
 jenkins_pysdk/core.py
 jenkins_pysdk/credentials.py
+jenkins_pysdk/exceptions.py
 jenkins_pysdk/jenkins.py
-jenkins_pysdk/jenkins_exceptions.py
 jenkins_pysdk/jobs.py
+jenkins_pysdk/objects.py
 jenkins_pysdk/plugins.py
-jenkins_pysdk/response_objects.py
 jenkins_pysdk/users.py
 jenkins_pysdk/utils.py
 jenkins_pysdk/views.py
 jenkins_pysdk.egg-info/PKG-INFO
 jenkins_pysdk.egg-info/SOURCES.txt
 jenkins_pysdk.egg-info/dependency_links.txt
 jenkins_pysdk.egg-info/requires.txt
```

