# Comparing `tmp/conformal_tights-0.2.4.tar.gz` & `tmp/conformal_tights-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conformal_tights-0.2.4.tar", max compression
+gzip compressed data, was "conformal_tights-0.3.0.tar", max compression
```

## Comparing `conformal_tights-0.2.4.tar` & `conformal_tights-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1062 2024-04-01 13:48:23.132477 conformal_tights-0.2.4/LICENSE
--rw-r--r--   0        0        0    10483 2024-04-01 13:48:23.132477 conformal_tights-0.2.4/README.md
--rw-r--r--   0        0        0     4656 2024-04-01 13:48:23.132477 conformal_tights-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      195 2024-04-01 13:48:23.132477 conformal_tights-0.2.4/src/conformal_tights/__init__.py
--rw-r--r--   0        0        0    11839 2024-04-01 13:48:23.132477 conformal_tights-0.2.4/src/conformal_tights/_coherent_linear_quantile_regressor.py
--rw-r--r--   0        0        0    17568 2024-04-01 13:48:23.132477 conformal_tights-0.2.4/src/conformal_tights/_conformal_coherent_quantile_regressor.py
--rw-r--r--   0        0        0      239 2024-04-01 13:48:23.132477 conformal_tights-0.2.4/src/conformal_tights/_typing.py
--rw-r--r--   0        0        0        0 2024-04-01 13:48:23.132477 conformal_tights-0.2.4/src/conformal_tights/py.typed
--rw-r--r--   0        0        0    11210 1970-01-01 00:00:00.000000 conformal_tights-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-04-14 17:50:51.436605 conformal_tights-0.3.0/LICENSE
+-rw-r--r--   0        0        0    17724 2024-04-14 17:50:51.436605 conformal_tights-0.3.0/README.md
+-rw-r--r--   0        0        0     5204 2024-04-14 17:50:51.440605 conformal_tights-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      277 2024-04-14 17:50:51.440605 conformal_tights-0.3.0/src/conformal_tights/__init__.py
+-rw-r--r--   0        0        0    11839 2024-04-14 17:50:51.440605 conformal_tights-0.3.0/src/conformal_tights/_coherent_linear_quantile_regressor.py
+-rw-r--r--   0        0        0    17568 2024-04-14 17:50:51.440605 conformal_tights-0.3.0/src/conformal_tights/_conformal_coherent_quantile_regressor.py
+-rw-r--r--   0        0        0     8782 2024-04-14 17:50:51.440605 conformal_tights-0.3.0/src/conformal_tights/_darts_forecaster.py
+-rw-r--r--   0        0        0      279 2024-04-14 17:50:51.440605 conformal_tights-0.3.0/src/conformal_tights/_typing.py
+-rw-r--r--   0        0        0        0 2024-04-14 17:50:51.440605 conformal_tights-0.3.0/src/conformal_tights/py.typed
+-rw-r--r--   0        0        0    18524 1970-01-01 00:00:00.000000 conformal_tights-0.3.0/PKG-INFO
```

### Comparing `conformal_tights-0.2.4/LICENSE` & `conformal_tights-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `conformal_tights-0.2.4/pyproject.toml` & `conformal_tights-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]  # https://python-poetry.org/docs/pyproject/#poetry-and-pep-517
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]  # https://python-poetry.org/docs/pyproject/
 name = "conformal-tights"
-version = "0.2.4"
+version = "0.3.0"
 description = "A scikit-learn meta-estimator for computing tight conformal predictions"
 authors = ["Laurent Sorber <laurent@radix.ai>"]
 readme = "README.md"
 repository = "https://github.com/radix-ai/conformal-tights"
 
 [tool.commitizen]  # https://commitizen-tools.github.io/commitizen/config/
 bump_message = "bump(release): v$current_version → v$new_version"
@@ -18,14 +18,18 @@
 
 [tool.poetry.dependencies]  # https://python-poetry.org/docs/dependency-specification/
 python = ">=3.10,<4.0"
 numpy = ">=1.22.0"
 scikit-learn = ">=1.0.0"
 scipy = ">=1.5.0"
 xgboost = ">=2.0.0"
+darts = { version = ">=0.25.0", optional = true }
+
+[tool.poetry.extras]  # https://python-poetry.org/docs/pyproject/#extras
+darts = ["darts"]
 
 [tool.poetry.group.test.dependencies]  # https://python-poetry.org/docs/master/managing-dependencies/
 commitizen = ">=3.2.1"
 coverage = { extras = ["toml"], version = ">=7.2.5" }
 lightgbm = ">=4.3.0"
 mypy = ">=1.2.0"
 pandas = ">=2.2.1"
@@ -39,14 +43,15 @@
 safety = ">=2.3.4,!=2.3.5"
 shellcheck-py = ">=0.9.0"
 
 [tool.poetry.group.dev.dependencies]  # https://python-poetry.org/docs/master/managing-dependencies/
 cruft = ">=2.14.0"
 ipykernel = ">=6.29.2"
 matplotlib = ">=3.8.3"
+nbconvert = ">=7.16.3"
 pdoc = ">=13.1.1"
 tabulate = ">=0.9.0"
 
 [tool.coverage.report]  # https://coverage.readthedocs.io/en/latest/config.html#report
 fail_under = 50
 precision = 1
 show_missing = true
@@ -98,14 +103,25 @@
 max-doc-length = 100
 
 [tool.ruff.lint.pydocstyle]
 convention = "numpy"
 
 [tool.poe.tasks]  # https://github.com/nat-n/poethepoet
 
+  [tool.poe.tasks.readme]
+  help = "Generate this package's README"
+  cmd = """
+    jupyter nbconvert notebooks/README.ipynb
+      --to markdown
+      --TagRemovePreprocessor.enabled=True
+      --TagRemovePreprocessor.remove_cell_tags remove_cell
+      --TagRemovePreprocessor.remove_all_outputs_tags remove_output
+      --TagRemovePreprocessor.remove_input_tags remove_input
+  """
+
   [tool.poe.tasks.docs]
   help = "Generate this package's docs"
   cmd = """
     pdoc
       --docformat $docformat
       --output-directory $outputdirectory
       conformal_tights
```

### Comparing `conformal_tights-0.2.4/src/conformal_tights/_coherent_linear_quantile_regressor.py` & `conformal_tights-0.3.0/src/conformal_tights/_coherent_linear_quantile_regressor.py`

 * *Files identical despite different names*

### Comparing `conformal_tights-0.2.4/src/conformal_tights/_conformal_coherent_quantile_regressor.py` & `conformal_tights-0.3.0/src/conformal_tights/_conformal_coherent_quantile_regressor.py`

 * *Files identical despite different names*

