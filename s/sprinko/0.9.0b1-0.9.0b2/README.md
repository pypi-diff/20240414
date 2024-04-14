# Comparing `tmp/sprinko-0.9.0b1.tar.gz` & `tmp/sprinko-0.9.0b2.tar.gz`

## Comparing `sprinko-0.9.0b1.tar` & `sprinko-0.9.0b2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/.gitattributes
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/.python-version
--rw-r--r--   0        0        0    35802 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/LICENSE
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/requirements-dev.lock
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/requirements.lock
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/.vscode/launch.json
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/.vscode/tasks.json
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/src/sprinko/__init__.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/src/sprinko/__main__.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/src/sprinko/cmds/_query.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/src/sprinko/cmds/generate.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/src/sprinko/cmds/info.py
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/src/sprinko/cmds/run.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/src/sprinko/cmds/setup.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/src/sprinko/core/__init__.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/src/sprinko/core/ctx.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/src/sprinko/core/mselect.py
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/src/sprinko/utils/__init__.py
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/src/sprinko/utils/selection.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/src/sprinko/utils/std.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/.gitignore
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/README.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/pyproject.toml
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/.gitattributes
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/.python-version
+-rw-r--r--   0        0        0    35802 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/LICENSE
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/requirements-dev.lock
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/requirements.lock
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/.vscode/launch.json
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/.vscode/tasks.json
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/src/sprinko/__init__.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/src/sprinko/__main__.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/src/sprinko/cmds/_query.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/src/sprinko/cmds/generate.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/src/sprinko/cmds/info.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/src/sprinko/cmds/run.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/src/sprinko/cmds/setup.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/src/sprinko/core/__init__.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/src/sprinko/core/ctx.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/src/sprinko/core/mselect.py
+-rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/src/sprinko/utils/__init__.py
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/src/sprinko/utils/selection.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/src/sprinko/utils/std.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/.gitignore
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/README.md
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/pyproject.toml
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/PKG-INFO
```

### Comparing `sprinko-0.9.0b1/LICENSE` & `sprinko-0.9.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `sprinko-0.9.0b1/requirements-dev.lock` & `sprinko-0.9.0b2/requirements-dev.lock`

 * *Files 4% similar despite different names*

```diff
@@ -34,18 +34,18 @@
 keyrings-cryptfile==1.3.9
     # via sprinko
 more-itertools==10.2.0
     # via jaraco-classes
     # via jaraco-functools
 parso==0.8.4
     # via jedi
-pip==24.0
 prompt-toolkit==3.0.43
     # via ptpython
 psutil==5.9.8
+    # via sprinko
 ptpython==3.0.26
     # via sprinko
 pycparser==2.22
     # via cffi
 pycryptodome==3.20.0
     # via keyrings-cryptfile
 pygments==2.17.2
```

### Comparing `sprinko-0.9.0b1/requirements.lock` & `sprinko-0.9.0b2/requirements.lock`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 more-itertools==10.2.0
     # via jaraco-classes
     # via jaraco-functools
 parso==0.8.4
     # via jedi
 prompt-toolkit==3.0.43
     # via ptpython
+psutil==5.9.8
+    # via sprinko
 ptpython==3.0.26
     # via sprinko
 pycparser==2.22
     # via cffi
 pycryptodome==3.20.0
     # via keyrings-cryptfile
 pygments==2.17.2
```

### Comparing `sprinko-0.9.0b1/.vscode/launch.json` & `sprinko-0.9.0b2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `sprinko-0.9.0b1/src/sprinko/__main__.py` & `sprinko-0.9.0b2/src/sprinko/__main__.py`

 * *Files identical despite different names*

### Comparing `sprinko-0.9.0b1/src/sprinko/cmds/_query.py` & `sprinko-0.9.0b2/src/sprinko/cmds/_query.py`

 * *Files identical despite different names*

### Comparing `sprinko-0.9.0b1/src/sprinko/cmds/generate.py` & `sprinko-0.9.0b2/src/sprinko/cmds/generate.py`

 * *Files identical despite different names*

### Comparing `sprinko-0.9.0b1/src/sprinko/cmds/run.py` & `sprinko-0.9.0b2/src/sprinko/cmds/run.py`

 * *Files identical despite different names*

### Comparing `sprinko-0.9.0b1/src/sprinko/cmds/setup.py` & `sprinko-0.9.0b2/src/sprinko/cmds/setup.py`

 * *Files identical despite different names*

### Comparing `sprinko-0.9.0b1/src/sprinko/core/__init__.py` & `sprinko-0.9.0b2/src/sprinko/core/__init__.py`

 * *Files identical despite different names*

### Comparing `sprinko-0.9.0b1/src/sprinko/core/ctx.py` & `sprinko-0.9.0b2/src/sprinko/core/ctx.py`

 * *Files identical despite different names*

### Comparing `sprinko-0.9.0b1/src/sprinko/core/mselect.py` & `sprinko-0.9.0b2/src/sprinko/core/mselect.py`

 * *Files identical despite different names*

### Comparing `sprinko-0.9.0b1/src/sprinko/utils/__init__.py` & `sprinko-0.9.0b2/src/sprinko/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sprinko-0.9.0b1/src/sprinko/utils/selection.py` & `sprinko-0.9.0b2/src/sprinko/utils/selection.py`

 * *Files identical despite different names*

### Comparing `sprinko-0.9.0b1/.gitignore` & `sprinko-0.9.0b2/.gitignore`

 * *Files identical despite different names*

### Comparing `sprinko-0.9.0b1/pyproject.toml` & `sprinko-0.9.0b2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [project]
 name = "sprinko"
-version = "0.9.0b1"
+version = "0.9.0b2"
 description = "sprinkles on scoop"
 authors = [
     { name = "ZackaryW", email = "36378555+ZackaryW@users.noreply.github.com" }
 ]
 dependencies = [
     "keyrings-cryptfile>=1.3.9",
     "pymasscode>=1.0.0b3",
     "click>=8.1.7",
     "readchar>=4.0.6",
     "ptpython>=3.0.26",
+    "psutil>=5.9.8",
 ]
 readme = "README.md"
 requires-python = ">= 3.8"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
 dev-dependencies = [
-    "pip>=24.0",
-    "psutil>=5.9.8",
+
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/sprinko"]
```

### Comparing `sprinko-0.9.0b1/PKG-INFO` & `sprinko-0.9.0b2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.3
 Name: sprinko
-Version: 0.9.0b1
+Version: 0.9.0b2
 Summary: sprinkles on scoop
 Author-email: ZackaryW <36378555+ZackaryW@users.noreply.github.com>
 Requires-Python: >=3.8
 Requires-Dist: click>=8.1.7
 Requires-Dist: keyrings-cryptfile>=1.3.9
+Requires-Dist: psutil>=5.9.8
 Requires-Dist: ptpython>=3.0.26
 Requires-Dist: pymasscode>=1.0.0b3
 Requires-Dist: readchar>=4.0.6
 Description-Content-Type: text/markdown
 
 # sprinko
 sprinkles on scoop
```

