# Comparing `tmp/SecLoadSDK-1.0.0.tar.gz` & `tmp/SecLoadSDK-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SecLoadSDK-1.0.0.tar", last modified: Thu Apr 11 00:07:29 2024, max compression
+gzip compressed data, was "SecLoadSDK-1.0.1.tar", last modified: Thu Apr 11 03:29:16 2024, max compression
```

## Comparing `SecLoadSDK-1.0.0.tar` & `SecLoadSDK-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 equsjd    (1000) equsjd    (1000)        0 2024-04-11 00:07:29.838088 SecLoadSDK-1.0.0/
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      303 2024-04-11 00:07:29.838088 SecLoadSDK-1.0.0/PKG-INFO
-drwxrwxr-x   0 equsjd    (1000) equsjd    (1000)        0 2024-04-11 00:07:29.838088 SecLoadSDK-1.0.0/SecLoad/
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)     1135 2024-04-10 23:55:04.000000 SecLoadSDK-1.0.0/SecLoad/__init__.py
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)     4740 2024-04-10 23:52:15.000000 SecLoadSDK-1.0.0/SecLoad/apihandlers.py
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      127 2024-04-10 22:20:59.000000 SecLoadSDK-1.0.0/SecLoad/enums.py
-drwxrwxr-x   0 equsjd    (1000) equsjd    (1000)        0 2024-04-11 00:07:29.838088 SecLoadSDK-1.0.0/SecLoadSDK.egg-info/
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      303 2024-04-11 00:07:29.000000 SecLoadSDK-1.0.0/SecLoadSDK.egg-info/PKG-INFO
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      204 2024-04-11 00:07:29.000000 SecLoadSDK-1.0.0/SecLoadSDK.egg-info/SOURCES.txt
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)        1 2024-04-11 00:07:29.000000 SecLoadSDK-1.0.0/SecLoadSDK.egg-info/dependency_links.txt
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)        8 2024-04-11 00:07:29.000000 SecLoadSDK-1.0.0/SecLoadSDK.egg-info/top_level.txt
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)       38 2024-04-11 00:07:29.838088 SecLoadSDK-1.0.0/setup.cfg
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      497 2024-04-11 00:06:09.000000 SecLoadSDK-1.0.0/setup.py
+drwxrwxr-x   0 equsjd    (1000) equsjd    (1000)        0 2024-04-11 03:29:16.326858 SecLoadSDK-1.0.1/
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      303 2024-04-11 03:29:16.326858 SecLoadSDK-1.0.1/PKG-INFO
+drwxrwxr-x   0 equsjd    (1000) equsjd    (1000)        0 2024-04-11 03:29:16.326858 SecLoadSDK-1.0.1/SecLoad/
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)     1137 2024-04-11 03:23:37.000000 SecLoadSDK-1.0.1/SecLoad/__init__.py
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)     4740 2024-04-11 03:26:50.000000 SecLoadSDK-1.0.1/SecLoad/apihandlers.py
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      127 2024-04-10 22:20:59.000000 SecLoadSDK-1.0.1/SecLoad/enums.py
+drwxrwxr-x   0 equsjd    (1000) equsjd    (1000)        0 2024-04-11 03:29:16.326858 SecLoadSDK-1.0.1/SecLoadSDK.egg-info/
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      303 2024-04-11 03:29:16.000000 SecLoadSDK-1.0.1/SecLoadSDK.egg-info/PKG-INFO
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      204 2024-04-11 03:29:16.000000 SecLoadSDK-1.0.1/SecLoadSDK.egg-info/SOURCES.txt
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)        1 2024-04-11 03:29:16.000000 SecLoadSDK-1.0.1/SecLoadSDK.egg-info/dependency_links.txt
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)        8 2024-04-11 03:29:16.000000 SecLoadSDK-1.0.1/SecLoadSDK.egg-info/top_level.txt
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)       38 2024-04-11 03:29:16.326858 SecLoadSDK-1.0.1/setup.cfg
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      497 2024-04-11 03:28:18.000000 SecLoadSDK-1.0.1/setup.py
```

### Comparing `SecLoadSDK-1.0.0/SecLoad/__init__.py` & `SecLoadSDK-1.0.1/SecLoad/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,9 +18,9 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
-from apihandlers import *
-from enums import *
+from .apihandlers import *
+from .enums import *
```

### Comparing `SecLoadSDK-1.0.0/SecLoad/apihandlers.py` & `SecLoadSDK-1.0.1/SecLoad/apihandlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from enums import *
-
+from .enums import *
 import requests, os
 
 class SecLoad:
     def __init__(self, APIKey: str):
         self.APIKey = APIKey
         self.URL = "https://secload.scriptlang.com"
```

