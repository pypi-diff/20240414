# Comparing `tmp/sprinko-0.9.0b2.tar.gz` & `tmp/sprinko-0.9.0b3.tar.gz`

## Comparing `sprinko-0.9.0b2.tar` & `sprinko-0.9.0b3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/.gitattributes
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/.python-version
--rw-r--r--   0        0        0    35802 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/LICENSE
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/requirements-dev.lock
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/requirements.lock
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/.vscode/launch.json
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/.vscode/tasks.json
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/src/sprinko/__init__.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/src/sprinko/__main__.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/src/sprinko/cmds/_query.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/src/sprinko/cmds/generate.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/src/sprinko/cmds/info.py
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/src/sprinko/cmds/run.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/src/sprinko/cmds/setup.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/src/sprinko/core/__init__.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/src/sprinko/core/ctx.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/src/sprinko/core/mselect.py
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/src/sprinko/utils/__init__.py
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/src/sprinko/utils/selection.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/src/sprinko/utils/std.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/.gitignore
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/README.md
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/pyproject.toml
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 sprinko-0.9.0b2/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 sprinko-0.9.0b3/.gitattributes
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 sprinko-0.9.0b3/.python-version
+-rw-r--r--   0        0        0    35802 2020-02-02 00:00:00.000000 sprinko-0.9.0b3/LICENSE
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 sprinko-0.9.0b3/requirements-dev.lock
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 sprinko-0.9.0b3/requirements.lock
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 sprinko-0.9.0b3/.vscode/launch.json
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 sprinko-0.9.0b3/.vscode/tasks.json
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 sprinko-0.9.0b3/src/sprinko/__init__.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 sprinko-0.9.0b3/src/sprinko/__main__.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 sprinko-0.9.0b3/src/sprinko/cmds/_query.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 sprinko-0.9.0b3/src/sprinko/cmds/generate.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 sprinko-0.9.0b3/src/sprinko/cmds/info.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 sprinko-0.9.0b3/src/sprinko/cmds/run.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 sprinko-0.9.0b3/src/sprinko/cmds/setup.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 sprinko-0.9.0b3/src/sprinko/core/__init__.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 sprinko-0.9.0b3/src/sprinko/core/ctx.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 sprinko-0.9.0b3/src/sprinko/core/mselect.py
+-rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 sprinko-0.9.0b3/src/sprinko/utils/__init__.py
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 sprinko-0.9.0b3/src/sprinko/utils/selection.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 sprinko-0.9.0b3/src/sprinko/utils/std.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 sprinko-0.9.0b3/.gitignore
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 sprinko-0.9.0b3/README.md
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 sprinko-0.9.0b3/pyproject.toml
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 sprinko-0.9.0b3/PKG-INFO
```

### Comparing `sprinko-0.9.0b2/LICENSE` & `sprinko-0.9.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `sprinko-0.9.0b2/requirements-dev.lock` & `sprinko-0.9.0b3/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `sprinko-0.9.0b2/requirements.lock` & `sprinko-0.9.0b3/requirements.lock`

 * *Files identical despite different names*

### Comparing `sprinko-0.9.0b2/.vscode/launch.json` & `sprinko-0.9.0b3/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `sprinko-0.9.0b2/src/sprinko/__main__.py` & `sprinko-0.9.0b3/src/sprinko/__main__.py`

 * *Files identical despite different names*

### Comparing `sprinko-0.9.0b2/src/sprinko/cmds/_query.py` & `sprinko-0.9.0b3/src/sprinko/cmds/_query.py`

 * *Files identical despite different names*

### Comparing `sprinko-0.9.0b2/src/sprinko/cmds/generate.py` & `sprinko-0.9.0b3/src/sprinko/cmds/generate.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 @click.group("generate", invoke_without_command=True, chain=True, short_help="Generate output")
 @click.option("--id", "-i", help="Run by ID")
 @click.option("--name", "-n", help="Run by exact name")
 @click.option("--frag", "-f", help="Run fragment index", type=click.INT, default=0)
 @click.option("--out", "-o", type=click.STRING, help="Output file", default="output")
 # custom
 @click.pass_context
-def sprinko_generate(ctx : click.Context, id : str = None, name : str = None, frag : int = 0 , save : str = None, live_eval : bool = False):
+def sprinko_generate(ctx : click.Context, id : str = None, name : str = None, frag : int = 0 , 
+    out : str = None,
+):
     tsnippet = resolve_snippet(ctx, id, name)
     if tsnippet:
         ctx.obj.gathered.append((frag, tsnippet))
 
 @sprinko_generate.result_callback()
 @click.pass_obj
 def sprinko_run_result(obj : Ctx, *args, **kwargs):
```

### Comparing `sprinko-0.9.0b2/src/sprinko/cmds/run.py` & `sprinko-0.9.0b3/src/sprinko/cmds/run.py`

 * *Files identical despite different names*

### Comparing `sprinko-0.9.0b2/src/sprinko/cmds/setup.py` & `sprinko-0.9.0b3/src/sprinko/cmds/setup.py`

 * *Files identical despite different names*

### Comparing `sprinko-0.9.0b2/src/sprinko/core/__init__.py` & `sprinko-0.9.0b3/src/sprinko/core/__init__.py`

 * *Files identical despite different names*

### Comparing `sprinko-0.9.0b2/src/sprinko/core/ctx.py` & `sprinko-0.9.0b3/src/sprinko/core/ctx.py`

 * *Files identical despite different names*

### Comparing `sprinko-0.9.0b2/src/sprinko/core/mselect.py` & `sprinko-0.9.0b3/src/sprinko/core/mselect.py`

 * *Files identical despite different names*

### Comparing `sprinko-0.9.0b2/src/sprinko/utils/__init__.py` & `sprinko-0.9.0b3/src/sprinko/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sprinko-0.9.0b2/src/sprinko/utils/selection.py` & `sprinko-0.9.0b3/src/sprinko/utils/selection.py`

 * *Files identical despite different names*

### Comparing `sprinko-0.9.0b2/.gitignore` & `sprinko-0.9.0b3/.gitignore`

 * *Files identical despite different names*

### Comparing `sprinko-0.9.0b2/pyproject.toml` & `sprinko-0.9.0b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sprinko"
-version = "0.9.0b2"
+version = "0.9.0b3"
 description = "sprinkles on scoop"
 authors = [
     { name = "ZackaryW", email = "36378555+ZackaryW@users.noreply.github.com" }
 ]
 dependencies = [
     "keyrings-cryptfile>=1.3.9",
     "pymasscode>=1.0.0b3",
```

### Comparing `sprinko-0.9.0b2/PKG-INFO` & `sprinko-0.9.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sprinko
-Version: 0.9.0b2
+Version: 0.9.0b3
 Summary: sprinkles on scoop
 Author-email: ZackaryW <36378555+ZackaryW@users.noreply.github.com>
 Requires-Python: >=3.8
 Requires-Dist: click>=8.1.7
 Requires-Dist: keyrings-cryptfile>=1.3.9
 Requires-Dist: psutil>=5.9.8
 Requires-Dist: ptpython>=3.0.26
```

