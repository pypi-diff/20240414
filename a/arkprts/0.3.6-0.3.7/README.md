# Comparing `tmp/arkprts-0.3.6.tar.gz` & `tmp/arkprts-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkprts-0.3.6.tar", last modified: Sun Mar  3 13:29:08 2024, max compression
+gzip compressed data, was "arkprts-0.3.7.tar", last modified: Sun Apr 14 13:30:24 2024, max compression
```

## Comparing `arkprts-0.3.6.tar` & `arkprts-0.3.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 13:29:08.499975 arkprts-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-03 13:29:04.000000 arkprts-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-03-03 13:29:08.499975 arkprts-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-03-03 13:29:04.000000 arkprts-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 13:29:08.495975 arkprts-0.3.6/arkprts/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-03 13:29:04.000000 arkprts-0.3.6/arkprts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-03-03 13:29:04.000000 arkprts-0.3.6/arkprts/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 13:29:08.495975 arkprts-0.3.6/arkprts/assets/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-03 13:29:04.000000 arkprts-0.3.6/arkprts/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-03-03 13:29:04.000000 arkprts-0.3.6/arkprts/assets/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5838 2024-03-03 13:29:04.000000 arkprts-0.3.6/arkprts/assets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    18024 2024-03-03 13:29:04.000000 arkprts-0.3.6/arkprts/assets/bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-03-03 13:29:04.000000 arkprts-0.3.6/arkprts/assets/git.py
--rw-r--r--   0 runner    (1001) docker     (127)    30547 2024-03-03 13:29:04.000000 arkprts-0.3.6/arkprts/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    20326 2024-03-03 13:29:04.000000 arkprts-0.3.6/arkprts/automation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9539 2024-03-03 13:29:04.000000 arkprts-0.3.6/arkprts/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-03-03 13:29:04.000000 arkprts-0.3.6/arkprts/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 13:29:08.499975 arkprts-0.3.6/arkprts/models/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-03 13:29:04.000000 arkprts-0.3.6/arkprts/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-03-03 13:29:04.000000 arkprts-0.3.6/arkprts/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-03-03 13:29:04.000000 arkprts-0.3.6/arkprts/models/battle.py
--rw-r--r--   0 runner    (1001) docker     (127)    12664 2024-03-03 13:29:04.000000 arkprts-0.3.6/arkprts/models/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6817 2024-03-03 13:29:04.000000 arkprts-0.3.6/arkprts/models/social.py
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-03-03 13:29:04.000000 arkprts-0.3.6/arkprts/network.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 13:29:04.000000 arkprts-0.3.6/arkprts/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 13:29:08.499975 arkprts-0.3.6/arkprts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-03-03 13:29:08.000000 arkprts-0.3.6/arkprts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-03 13:29:08.000000 arkprts-0.3.6/arkprts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 13:29:08.000000 arkprts-0.3.6/arkprts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-03 13:29:08.000000 arkprts-0.3.6/arkprts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-03 13:29:08.000000 arkprts-0.3.6/arkprts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-03-03 13:29:04.000000 arkprts-0.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-03 13:29:08.499975 arkprts-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-03-03 13:29:04.000000 arkprts-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 13:29:08.499975 arkprts-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-03 13:29:04.000000 arkprts-0.3.6/tests/test_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-03-03 13:29:04.000000 arkprts-0.3.6/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-03 13:29:04.000000 arkprts-0.3.6/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:30:24.310088 arkprts-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-14 13:30:21.000000 arkprts-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-14 13:30:24.310088 arkprts-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-14 13:30:21.000000 arkprts-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:30:24.306088 arkprts-0.3.7/arkprts/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-14 13:30:21.000000 arkprts-0.3.7/arkprts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-14 13:30:21.000000 arkprts-0.3.7/arkprts/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:30:24.306088 arkprts-0.3.7/arkprts/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-14 13:30:21.000000 arkprts-0.3.7/arkprts/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-14 13:30:21.000000 arkprts-0.3.7/arkprts/assets/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5838 2024-04-14 13:30:21.000000 arkprts-0.3.7/arkprts/assets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18024 2024-04-14 13:30:21.000000 arkprts-0.3.7/arkprts/assets/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-04-14 13:30:21.000000 arkprts-0.3.7/arkprts/assets/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30547 2024-04-14 13:30:21.000000 arkprts-0.3.7/arkprts/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20326 2024-04-14 13:30:21.000000 arkprts-0.3.7/arkprts/automation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9539 2024-04-14 13:30:21.000000 arkprts-0.3.7/arkprts/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-14 13:30:21.000000 arkprts-0.3.7/arkprts/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:30:24.306088 arkprts-0.3.7/arkprts/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-14 13:30:21.000000 arkprts-0.3.7/arkprts/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-14 13:30:21.000000 arkprts-0.3.7/arkprts/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-04-14 13:30:21.000000 arkprts-0.3.7/arkprts/models/battle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12678 2024-04-14 13:30:21.000000 arkprts-0.3.7/arkprts/models/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6817 2024-04-14 13:30:21.000000 arkprts-0.3.7/arkprts/models/social.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-14 13:30:21.000000 arkprts-0.3.7/arkprts/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:30:21.000000 arkprts-0.3.7/arkprts/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:30:24.310088 arkprts-0.3.7/arkprts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-14 13:30:24.000000 arkprts-0.3.7/arkprts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-14 13:30:24.000000 arkprts-0.3.7/arkprts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 13:30:24.000000 arkprts-0.3.7/arkprts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-14 13:30:24.000000 arkprts-0.3.7/arkprts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-14 13:30:24.000000 arkprts-0.3.7/arkprts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-14 13:30:21.000000 arkprts-0.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 13:30:24.310088 arkprts-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-14 13:30:21.000000 arkprts-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:30:24.310088 arkprts-0.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-14 13:30:21.000000 arkprts-0.3.7/tests/test_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-04-14 13:30:21.000000 arkprts-0.3.7/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-14 13:30:21.000000 arkprts-0.3.7/tests/test_client.py
```

### Comparing `arkprts-0.3.6/LICENSE` & `arkprts-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `arkprts-0.3.6/PKG-INFO` & `arkprts-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkprts
-Version: 0.3.6
+Version: 0.3.7
 Summary: Arknights python wrapper.
 Home-page: https://github.com/thesadru/arkprts
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
```

### Comparing `arkprts-0.3.6/README.md` & `arkprts-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `arkprts-0.3.6/arkprts/__main__.py` & `arkprts-0.3.7/arkprts/__main__.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.3.6/arkprts/assets/__main__.py` & `arkprts-0.3.7/arkprts/assets/__main__.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.3.6/arkprts/assets/base.py` & `arkprts-0.3.7/arkprts/assets/base.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.3.6/arkprts/assets/bundle.py` & `arkprts-0.3.7/arkprts/assets/bundle.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.3.6/arkprts/assets/git.py` & `arkprts-0.3.7/arkprts/assets/git.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.3.6/arkprts/auth.py` & `arkprts-0.3.7/arkprts/auth.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.3.6/arkprts/automation.py` & `arkprts-0.3.7/arkprts/automation.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.3.6/arkprts/client.py` & `arkprts-0.3.7/arkprts/client.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.3.6/arkprts/errors.py` & `arkprts-0.3.7/arkprts/errors.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.3.6/arkprts/models/base.py` & `arkprts-0.3.7/arkprts/models/base.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.3.6/arkprts/models/battle.py` & `arkprts-0.3.7/arkprts/models/battle.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.3.6/arkprts/models/data.py` & `arkprts-0.3.7/arkprts/models/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,15 +279,15 @@
 class AssistChar(base.BaseModel):
     """Assist operator data."""
 
     char_inst_id: int = pydantic.Field(alias="charInstId")
     """Index of the operator."""
     skill_index: int = pydantic.Field(alias="skillIndex")
     """Index of the selected skill."""
-    current_equip: typing.Optional[str] = pydantic.Field(alias="currentEquip")
+    current_equip: typing.Optional[str] = pydantic.Field(default=None, alias="currentEquip")
     """Currently equipped module."""
     tmpl: typing.Mapping[str, base.DDict] = pydantic.Field(default_factory=base.DDict, repr=False)
     """Alternative operator class data. Only for Amiya."""
 
 
 class Social(base.BaseModel):
     """Social data."""
```

### Comparing `arkprts-0.3.6/arkprts/models/social.py` & `arkprts-0.3.7/arkprts/models/social.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.3.6/arkprts/network.py` & `arkprts-0.3.7/arkprts/network.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.3.6/arkprts.egg-info/PKG-INFO` & `arkprts-0.3.7/arkprts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkprts
-Version: 0.3.6
+Version: 0.3.7
 Summary: Arknights python wrapper.
 Home-page: https://github.com/thesadru/arkprts
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
```

### Comparing `arkprts-0.3.6/arkprts.egg-info/SOURCES.txt` & `arkprts-0.3.7/arkprts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arkprts-0.3.6/pyproject.toml` & `arkprts-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "arkprts"
 requires-python = ">=3.9"
-version = "0.3.6"
+version = "0.3.7"
 dynamic = [
     "dependencies",
     "description",
     "license",
     "optional-dependencies",
     "readme",
 ]
```

### Comparing `arkprts-0.3.6/setup.py` & `arkprts-0.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Run setuptools."""
 import pathlib
 
 from setuptools import find_packages, setup
 
 setup(
     name="arkprts",
-    version="0.3.6",
+    version="0.3.7",
     description="Arknights python wrapper.",
     url="https://github.com/thesadru/arkprts",
     packages=find_packages(exclude=["tests", "tests.*"]),
     include_package_data=True,
     package_data={"arkprts": ["py.typed"]},
     install_requires=["aiohttp", "pydantic==2.*"],
     extras_require={
```

### Comparing `arkprts-0.3.6/tests/test_assets.py` & `arkprts-0.3.7/tests/test_assets.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.3.6/tests/test_auth.py` & `arkprts-0.3.7/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.3.6/tests/test_client.py` & `arkprts-0.3.7/tests/test_client.py`

 * *Files identical despite different names*

