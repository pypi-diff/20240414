# Comparing `tmp/audiconnectpy-1.5.3.tar.gz` & `tmp/audiconnectpy-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-1.5.3.tar", last modified: Fri Jan  5 18:18:02 2024, max compression
+gzip compressed data, was "audiconnectpy-1.5.4.tar", last modified: Sat Apr 13 17:47:15 2024, max compression
```

## Comparing `audiconnectpy-1.5.3.tar` & `audiconnectpy-1.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 18:18:02.376633 audiconnectpy-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-05 18:17:47.000000 audiconnectpy-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-01-05 18:17:47.000000 audiconnectpy-1.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-01-05 18:18:02.376633 audiconnectpy-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-01-05 18:17:47.000000 audiconnectpy-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 18:18:02.376633 audiconnectpy-1.5.3/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-01-05 18:17:47.000000 audiconnectpy-1.5.3/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19480 2024-01-05 18:17:47.000000 audiconnectpy-1.5.3/audiconnectpy/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-01-05 18:17:47.000000 audiconnectpy-1.5.3/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23012 2024-01-05 18:17:47.000000 audiconnectpy-1.5.3/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-01-05 18:17:47.000000 audiconnectpy-1.5.3/audiconnectpy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-01-05 18:17:47.000000 audiconnectpy-1.5.3/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-01-05 18:17:47.000000 audiconnectpy-1.5.3/audiconnectpy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20136 2024-01-05 18:17:47.000000 audiconnectpy-1.5.3/audiconnectpy/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    10617 2024-01-05 18:17:47.000000 audiconnectpy-1.5.3/audiconnectpy/services.py
--rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-01-05 18:17:47.000000 audiconnectpy-1.5.3/audiconnectpy/vehicle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 18:18:02.376633 audiconnectpy-1.5.3/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-01-05 18:18:02.000000 audiconnectpy-1.5.3/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-01-05 18:18:02.000000 audiconnectpy-1.5.3/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-05 18:18:02.000000 audiconnectpy-1.5.3/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-05 18:18:02.000000 audiconnectpy-1.5.3/audiconnectpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-05 18:18:02.000000 audiconnectpy-1.5.3/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-05 18:18:02.000000 audiconnectpy-1.5.3/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-01-05 18:17:55.000000 audiconnectpy-1.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-05 18:18:02.376633 audiconnectpy-1.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:47:15.431876 audiconnectpy-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-13 17:47:00.000000 audiconnectpy-1.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-13 17:47:00.000000 audiconnectpy-1.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-13 17:47:15.431876 audiconnectpy-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-13 17:47:00.000000 audiconnectpy-1.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:47:15.431876 audiconnectpy-1.5.4/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-13 17:47:00.000000 audiconnectpy-1.5.4/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19481 2024-04-13 17:47:00.000000 audiconnectpy-1.5.4/audiconnectpy/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-13 17:47:00.000000 audiconnectpy-1.5.4/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22828 2024-04-13 17:47:00.000000 audiconnectpy-1.5.4/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-13 17:47:00.000000 audiconnectpy-1.5.4/audiconnectpy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-13 17:47:00.000000 audiconnectpy-1.5.4/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-04-13 17:47:00.000000 audiconnectpy-1.5.4/audiconnectpy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20137 2024-04-13 17:47:00.000000 audiconnectpy-1.5.4/audiconnectpy/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10618 2024-04-13 17:47:00.000000 audiconnectpy-1.5.4/audiconnectpy/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12474 2024-04-13 17:47:00.000000 audiconnectpy-1.5.4/audiconnectpy/vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:47:15.431876 audiconnectpy-1.5.4/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-13 17:47:15.000000 audiconnectpy-1.5.4/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-13 17:47:15.000000 audiconnectpy-1.5.4/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 17:47:15.000000 audiconnectpy-1.5.4/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 17:47:15.000000 audiconnectpy-1.5.4/audiconnectpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-13 17:47:15.000000 audiconnectpy-1.5.4/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-13 17:47:15.000000 audiconnectpy-1.5.4/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-13 17:47:12.000000 audiconnectpy-1.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 17:47:15.431876 audiconnectpy-1.5.4/setup.cfg
```

### Comparing `audiconnectpy-1.5.3/LICENSE` & `audiconnectpy-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.5.3/PKG-INFO` & `audiconnectpy-1.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.5.3
+Version: 1.5.4
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,14 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.8.1
+Requires-Dist: bs4>=0.0.2
 
 # audiconnectpy
 
 [![GitHub sourcecode](https://img.shields.io/badge/Source-GitHub-green)](https://github.com/cyr-ius/audiconnectpy/)
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/cyr-ius/audiconnectpy)](https://github.com/cyr-ius/audiconnectpy/releases/latest)
 ![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/audiconnectpy?label=PyPI%20Downloads)](https://pypi.org/project/audiconnectpy/)
```

### Comparing `audiconnectpy-1.5.3/README.md` & `audiconnectpy-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.5.3/audiconnectpy/actions.py` & `audiconnectpy-1.5.4/audiconnectpy/actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Audi actions."""
+
 from __future__ import annotations
 
 import asyncio
 from dataclasses import dataclass
 from typing import Any, Literal
 
 from .auth import Auth
```

### Comparing `audiconnectpy-1.5.3/audiconnectpy/api.py` & `audiconnectpy-1.5.4/audiconnectpy/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Audi connect."""
+
 from __future__ import annotations
 
 import logging
 from typing import Any, Tuple
 
 from aiohttp import ClientSession
```

### Comparing `audiconnectpy-1.5.3/audiconnectpy/auth.py` & `audiconnectpy-1.5.4/audiconnectpy/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """Audi connect."""
+
 from __future__ import annotations
 
 import asyncio
 import base64
+from datetime import datetime, timedelta
+from hashlib import sha256
 import json
 import logging
 import os
 import re
 import socket
-import uuid
-from datetime import datetime, timedelta
-from hashlib import sha256
 from typing import Any, Literal
 from urllib.parse import parse_qs, urlencode, urlparse
+import uuid
 
 import aiohttp
-import async_timeout
 from aiohttp.hdrs import METH_GET, METH_POST, METH_PUT
+import async_timeout
 from bs4 import BeautifulSoup
 
 from .exceptions import (
     AudiException,
     HttpRequestError,
     ServiceNotFoundError,
     TimeoutExceededError,
@@ -42,24 +43,17 @@
     """Authentication."""
 
     def __init__(
         self, session: aiohttp.ClientSession, proxy: str | None = None
     ) -> None:
         """Initialize."""
         self._session = session
-        if proxy:
-            self.__proxy: dict[
-                str, str
-            ] | None = {  # pylint: disable=unused-private-member
-                "http": proxy,
-                "https": proxy,
-            }
-        else:
-            self.__proxy = None  # pylint: disable=unused-private-member
-
+        self.__proxy: dict[str, str] | None = (
+            {"http": proxy, "https": proxy} if proxy else None
+        )
         self._audi_baseurl = ""
         self._mbb_baseurl = MBB_URL
         self._token_endpoint_url = ""
         self._authorization_endpoint_url = ""
         self._revocation_endpoint_url = ""
         self.profil_url = ""
```

### Comparing `audiconnectpy-1.5.3/audiconnectpy/helpers.py` & `audiconnectpy-1.5.4/audiconnectpy/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Helper functions."""
+
 from __future__ import annotations
 
 import functools
 import json
 import logging
 import random
 import time
```

### Comparing `audiconnectpy-1.5.3/audiconnectpy/models.py` & `audiconnectpy-1.5.4/audiconnectpy/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Definition class."""
+
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass
 from datetime import datetime as dt
 
 from .helpers import ExtendedDict
```

### Comparing `audiconnectpy-1.5.3/audiconnectpy/services.py` & `audiconnectpy-1.5.4/audiconnectpy/services.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Call url service."""
+
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from typing import Any, Literal
```

### Comparing `audiconnectpy-1.5.3/audiconnectpy/vehicle.py` & `audiconnectpy-1.5.4/audiconnectpy/vehicle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Vehicle class."""
+
 from __future__ import annotations
 
 import logging
 from typing import Literal
 
 from .actions import AudiActions
 from .auth import Auth
```

### Comparing `audiconnectpy-1.5.3/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-1.5.4/audiconnectpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.5.3
+Version: 1.5.4
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,14 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.8.1
+Requires-Dist: bs4>=0.0.2
 
 # audiconnectpy
 
 [![GitHub sourcecode](https://img.shields.io/badge/Source-GitHub-green)](https://github.com/cyr-ius/audiconnectpy/)
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/cyr-ius/audiconnectpy)](https://github.com/cyr-ius/audiconnectpy/releases/latest)
 ![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/audiconnectpy?label=PyPI%20Downloads)](https://pypi.org/project/audiconnectpy/)
```

