# Comparing `tmp/impactpy-0.0.4.tar.gz` & `tmp/impactpy-0.0.5.tar.gz`

## Comparing `impactpy-0.0.4.tar` & `impactpy-0.0.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 impactpy-0.0.4/ImpactPy.egg-info/PKG-INFO
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 impactpy-0.0.4/ImpactPy.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 impactpy-0.0.4/ImpactPy.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 impactpy-0.0.4/ImpactPy.egg-info/requires.txt
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 impactpy-0.0.4/ImpactPy.egg-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactpy-0.0.4/build/lib/src/__init__.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 impactpy-0.0.4/build/lib/src/alpha/__init__.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 impactpy-0.0.4/build/lib/src/alpha/base_alpha.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactpy-0.0.4/build/lib/src/alpha/intraday_alpha.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactpy-0.0.4/build/lib/src/alpha/overnight_alpha.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 impactpy-0.0.4/build/lib/src/alpha/trading_alpha.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 impactpy-0.0.4/build/lib/src/models/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 impactpy-0.0.4/build/lib/src/models/afs_model.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 impactpy-0.0.4/build/lib/src/models/impact_model.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 impactpy-0.0.4/build/lib/src/models/ow_model.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 impactpy-0.0.4/build/lib/src/schedule/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 impactpy-0.0.4/build/lib/src/schedule/schedule.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 impactpy-0.0.4/build/lib/src/tca/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 impactpy-0.0.4/build/lib/src/tca/tca_report.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactpy-0.0.4/build/lib/testing/__init__.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 impactpy-0.0.4/build/lib/testing/test_cfg.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactpy-0.0.4/impactpy/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 impactpy-0.0.4/impactpy/alpha/__init__.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 impactpy-0.0.4/impactpy/alpha/base_alpha.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactpy-0.0.4/impactpy/alpha/intraday_alpha.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactpy-0.0.4/impactpy/alpha/overnight_alpha.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 impactpy-0.0.4/impactpy/alpha/trading_alpha.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 impactpy-0.0.4/impactpy/models/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 impactpy-0.0.4/impactpy/models/afs_model.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 impactpy-0.0.4/impactpy/models/impact_model.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 impactpy-0.0.4/impactpy/models/ow_model.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 impactpy-0.0.4/impactpy/schedule/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 impactpy-0.0.4/impactpy/schedule/schedule.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 impactpy-0.0.4/impactpy/tca/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 impactpy-0.0.4/impactpy/tca/tca_report.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 impactpy-0.0.4/impactpy_lachlanbaxter.egg-info/PKG-INFO
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 impactpy-0.0.4/impactpy_lachlanbaxter.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 impactpy-0.0.4/impactpy_lachlanbaxter.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 impactpy-0.0.4/impactpy_lachlanbaxter.egg-info/requires.txt
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 impactpy-0.0.4/impactpy_lachlanbaxter.egg-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactpy-0.0.4/README.md
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 impactpy-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 impactpy-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 impactpy-0.0.5/ImpactPy.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 impactpy-0.0.5/ImpactPy.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 impactpy-0.0.5/ImpactPy.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 impactpy-0.0.5/ImpactPy.egg-info/requires.txt
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 impactpy-0.0.5/ImpactPy.egg-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactpy-0.0.5/build/lib/src/__init__.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 impactpy-0.0.5/build/lib/src/alpha/__init__.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 impactpy-0.0.5/build/lib/src/alpha/base_alpha.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactpy-0.0.5/build/lib/src/alpha/intraday_alpha.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactpy-0.0.5/build/lib/src/alpha/overnight_alpha.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 impactpy-0.0.5/build/lib/src/alpha/trading_alpha.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 impactpy-0.0.5/build/lib/src/models/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 impactpy-0.0.5/build/lib/src/models/afs_model.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 impactpy-0.0.5/build/lib/src/models/impact_model.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 impactpy-0.0.5/build/lib/src/models/ow_model.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 impactpy-0.0.5/build/lib/src/schedule/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 impactpy-0.0.5/build/lib/src/schedule/schedule.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 impactpy-0.0.5/build/lib/src/tca/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 impactpy-0.0.5/build/lib/src/tca/tca_report.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactpy-0.0.5/build/lib/testing/__init__.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 impactpy-0.0.5/build/lib/testing/test_cfg.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactpy-0.0.5/impactpy/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 impactpy-0.0.5/impactpy/alpha/__init__.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 impactpy-0.0.5/impactpy/alpha/base_alpha.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 impactpy-0.0.5/impactpy/alpha/intraday_alpha.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactpy-0.0.5/impactpy/alpha/overnight_alpha.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 impactpy-0.0.5/impactpy/alpha/trading_alpha.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 impactpy-0.0.5/impactpy/models/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 impactpy-0.0.5/impactpy/models/afs_model.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 impactpy-0.0.5/impactpy/models/impact_model.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 impactpy-0.0.5/impactpy/models/ow_model.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 impactpy-0.0.5/impactpy/schedule/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 impactpy-0.0.5/impactpy/schedule/schedule.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 impactpy-0.0.5/impactpy/tca/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 impactpy-0.0.5/impactpy/tca/tca_report.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 impactpy-0.0.5/impactpy_lachlanbaxter.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 impactpy-0.0.5/impactpy_lachlanbaxter.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 impactpy-0.0.5/impactpy_lachlanbaxter.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 impactpy-0.0.5/impactpy_lachlanbaxter.egg-info/requires.txt
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 impactpy-0.0.5/impactpy_lachlanbaxter.egg-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactpy-0.0.5/README.md
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 impactpy-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 impactpy-0.0.5/PKG-INFO
```

### Comparing `impactpy-0.0.4/ImpactPy.egg-info/SOURCES.txt` & `impactpy-0.0.5/ImpactPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `impactpy-0.0.4/build/lib/src/models/impact_model.py` & `impactpy-0.0.5/build/lib/src/models/impact_model.py`

 * *Files identical despite different names*

### Comparing `impactpy-0.0.4/build/lib/testing/test_cfg.py` & `impactpy-0.0.5/build/lib/testing/test_cfg.py`

 * *Files identical despite different names*

### Comparing `impactpy-0.0.4/impactpy/models/impact_model.py` & `impactpy-0.0.5/impactpy/models/impact_model.py`

 * *Files identical despite different names*

### Comparing `impactpy-0.0.4/impactpy_lachlanbaxter.egg-info/PKG-INFO` & `impactpy-0.0.5/impactpy_lachlanbaxter.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `impactpy-0.0.4/impactpy_lachlanbaxter.egg-info/SOURCES.txt` & `impactpy-0.0.5/impactpy_lachlanbaxter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `impactpy-0.0.4/pyproject.toml` & `impactpy-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["impactpy"]
 
 [project]
 name = "impactpy"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Lachlan Baxter", email="lachlan.baxter@outlook.com" },
 ]
 description = "Toolset for calibrating price impact models to LOB data"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers= [
```

