# Comparing `tmp/dyff-client-0.2.2.tar.gz` & `tmp/dyff_client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff-client-0.2.2.tar", last modified: Tue Apr  9 21:04:03 2024, max compression
+gzip compressed data, was "dyff_client-0.3.0.tar", last modified: Sun Apr 14 19:26:09 2024, max compression
```

## Comparing `dyff-client-0.2.2.tar` & `dyff_client-0.3.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:04:03.014518 dyff-client-0.2.2/
--rw-rw-rw-   0 root         (0) root         (0)      467 2024-04-09 21:03:56.000000 dyff-client-0.2.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1777 2024-04-09 21:03:56.000000 dyff-client-0.2.2/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      512 2024-04-09 21:03:56.000000 dyff-client-0.2.2/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1674 2024-04-09 21:03:56.000000 dyff-client-0.2.2/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      182 2024-04-09 21:03:56.000000 dyff-client-0.2.2/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     3478 2024-04-09 21:03:56.000000 dyff-client-0.2.2/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-09 21:03:56.000000 dyff-client-0.2.2/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-09 21:03:56.000000 dyff-client-0.2.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-04-09 21:03:56.000000 dyff-client-0.2.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4008 2024-04-09 21:04:03.014518 dyff-client-0.2.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2781 2024-04-09 21:03:56.000000 dyff-client-0.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:04:02.998519 dyff-client-0.2.2/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:04:03.005518 dyff-client-0.2.2/dyff/client/
--rw-rw-rw-   0 root         (0) root         (0)      221 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:04:03.007518 dyff-client-0.2.2/dyff/client/_generated/
--rw-rw-rw-   0 root         (0) root         (0)      704 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6220 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1942 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      752 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/_patch.py
--rw-rw-rw-   0 root         (0) root         (0)    80932 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/_serialization.py
--rw-rw-rw-   0 root         (0) root         (0)      861 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/_vendor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:04:03.008518 dyff-client-0.2.2/dyff/client/_generated/aio/
--rw-rw-rw-   0 root         (0) root         (0)      704 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/aio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6360 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/aio/_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1974 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/aio/_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/aio/_patch.py
--rw-rw-rw-   0 root         (0) root         (0)      861 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/aio/_vendor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:04:03.009518 dyff-client-0.2.2/dyff/client/_generated/aio/operations/
--rw-rw-rw-   0 root         (0) root         (0)     1128 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/aio/operations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   542099 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/aio/operations/_operations.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/aio/operations/_patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:04:03.010518 dyff-client-0.2.2/dyff/client/_generated/operations/
--rw-rw-rw-   0 root         (0) root         (0)     1128 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/operations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   581216 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/operations/_operations.py
--rw-rw-rw-   0 root         (0) root         (0)      994 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/operations/_patch.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    62743 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:04:03.014518 dyff-client-0.2.2/dyff_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4008 2024-04-09 21:04:02.000000 dyff-client-0.2.2/dyff_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1464 2024-04-09 21:04:02.000000 dyff-client-0.2.2/dyff_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 21:04:02.000000 dyff-client-0.2.2/dyff_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       83 2024-04-09 21:04:02.000000 dyff-client-0.2.2/dyff_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-09 21:04:02.000000 dyff-client-0.2.2/dyff_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1084 2024-04-09 21:03:56.000000 dyff-client-0.2.2/makefile
--rw-rw-rw-   0 root         (0) root         (0)      317 2024-04-09 21:03:56.000000 dyff-client-0.2.2/package-lock.json
--rw-rw-rw-   0 root         (0) root         (0)       53 2024-04-09 21:03:56.000000 dyff-client-0.2.2/package.json
--rw-rw-rw-   0 root         (0) root         (0)     1589 2024-04-09 21:03:56.000000 dyff-client-0.2.2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:04:03.000518 dyff-client-0.2.2/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:04:03.012518 dyff-client-0.2.2/scripts/inferenceservices/
--rw-rw-rw-   0 root         (0) root         (0)     2529 2024-04-09 21:03:56.000000 dyff-client-0.2.2/scripts/inferenceservices/databricks--dolly-v2-3b--default.py
--rw-rw-rw-   0 root         (0) root         (0)     2537 2024-04-09 21:03:56.000000 dyff-client-0.2.2/scripts/inferenceservices/tiiuae--falcon-7b--default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:04:03.013518 dyff-client-0.2.2/scripts/models/
--rw-rw-rw-   0 root         (0) root         (0)      420 2024-04-09 21:03:56.000000 dyff-client-0.2.2/scripts/models/databricks--dolly-v2-3b--rox.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1374 2024-04-09 21:03:56.000000 dyff-client-0.2.2/scripts/models/databricks--dolly-v2-3b.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2024-04-09 21:03:56.000000 dyff-client-0.2.2/scripts/models/tiiuae--falcon-7b--rox.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1356 2024-04-09 21:03:56.000000 dyff-client-0.2.2/scripts/models/tiiuae--falcon-7b.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 21:04:03.014518 dyff-client-0.2.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:04:03.013518 dyff-client-0.2.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1123 2024-04-09 21:03:56.000000 dyff-client-0.2.2/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 19:26:09.727008 dyff_client-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)      467 2024-04-14 19:26:03.000000 dyff_client-0.3.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1777 2024-04-14 19:26:03.000000 dyff_client-0.3.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      512 2024-04-14 19:26:03.000000 dyff_client-0.3.0/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2024-04-14 19:26:03.000000 dyff_client-0.3.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      182 2024-04-14 19:26:03.000000 dyff_client-0.3.0/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     3478 2024-04-14 19:26:03.000000 dyff_client-0.3.0/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-14 19:26:03.000000 dyff_client-0.3.0/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-14 19:26:03.000000 dyff_client-0.3.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-04-14 19:26:03.000000 dyff_client-0.3.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4008 2024-04-14 19:26:09.727008 dyff_client-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2781 2024-04-14 19:26:03.000000 dyff_client-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 19:26:09.712025 dyff_client-0.3.0/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 19:26:09.718018 dyff_client-0.3.0/dyff/client/
+-rw-rw-rw-   0 root         (0) root         (0)      221 2024-04-14 19:26:03.000000 dyff_client-0.3.0/dyff/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 19:26:09.720016 dyff_client-0.3.0/dyff/client/_generated/
+-rw-rw-rw-   0 root         (0) root         (0)      709 2024-04-14 19:26:03.000000 dyff_client-0.3.0/dyff/client/_generated/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7058 2024-04-14 19:26:03.000000 dyff_client-0.3.0/dyff/client/_generated/_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-14 19:26:03.000000 dyff_client-0.3.0/dyff/client/_generated/_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      752 2024-04-14 19:26:03.000000 dyff_client-0.3.0/dyff/client/_generated/_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)    80932 2024-04-14 19:26:03.000000 dyff_client-0.3.0/dyff/client/_generated/_serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-04-14 19:26:03.000000 dyff_client-0.3.0/dyff/client/_generated/_vendor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 19:26:09.721015 dyff_client-0.3.0/dyff/client/_generated/aio/
+-rw-rw-rw-   0 root         (0) root         (0)      709 2024-04-14 19:26:03.000000 dyff_client-0.3.0/dyff/client/_generated/aio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7226 2024-04-14 19:26:03.000000 dyff_client-0.3.0/dyff/client/_generated/aio/_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1981 2024-04-14 19:26:03.000000 dyff_client-0.3.0/dyff/client/_generated/aio/_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-04-14 19:26:03.000000 dyff_client-0.3.0/dyff/client/_generated/aio/_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-04-14 19:26:03.000000 dyff_client-0.3.0/dyff/client/_generated/aio/_vendor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 19:26:09.722014 dyff_client-0.3.0/dyff/client/_generated/aio/operations/
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2024-04-14 19:26:03.000000 dyff_client-0.3.0/dyff/client/_generated/aio/operations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   770253 2024-04-14 19:26:03.000000 dyff_client-0.3.0/dyff/client/_generated/aio/operations/_operations.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-04-14 19:26:03.000000 dyff_client-0.3.0/dyff/client/_generated/aio/operations/_patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 19:26:09.723013 dyff_client-0.3.0/dyff/client/_generated/operations/
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2024-04-14 19:26:03.000000 dyff_client-0.3.0/dyff/client/_generated/operations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   821959 2024-04-14 19:26:03.000000 dyff_client-0.3.0/dyff/client/_generated/operations/_operations.py
+-rw-rw-rw-   0 root         (0) root         (0)      994 2024-04-14 19:26:03.000000 dyff_client-0.3.0/dyff/client/_generated/operations/_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-04-14 19:26:03.000000 dyff_client-0.3.0/dyff/client/_generated/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    81214 2024-04-14 19:26:03.000000 dyff_client-0.3.0/dyff/client/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 19:26:09.726009 dyff_client-0.3.0/dyff_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4008 2024-04-14 19:26:09.000000 dyff_client-0.3.0/dyff_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1464 2024-04-14 19:26:09.000000 dyff_client-0.3.0/dyff_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-14 19:26:09.000000 dyff_client-0.3.0/dyff_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2024-04-14 19:26:09.000000 dyff_client-0.3.0/dyff_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-14 19:26:09.000000 dyff_client-0.3.0/dyff_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2024-04-14 19:26:03.000000 dyff_client-0.3.0/makefile
+-rw-rw-rw-   0 root         (0) root         (0)      317 2024-04-14 19:26:03.000000 dyff_client-0.3.0/package-lock.json
+-rw-rw-rw-   0 root         (0) root         (0)       53 2024-04-14 19:26:03.000000 dyff_client-0.3.0/package.json
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2024-04-14 19:26:03.000000 dyff_client-0.3.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 19:26:09.714023 dyff_client-0.3.0/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 19:26:09.725011 dyff_client-0.3.0/scripts/inferenceservices/
+-rw-rw-rw-   0 root         (0) root         (0)     2529 2024-04-14 19:26:03.000000 dyff_client-0.3.0/scripts/inferenceservices/databricks--dolly-v2-3b--default.py
+-rw-rw-rw-   0 root         (0) root         (0)     2537 2024-04-14 19:26:03.000000 dyff_client-0.3.0/scripts/inferenceservices/tiiuae--falcon-7b--default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 19:26:09.726009 dyff_client-0.3.0/scripts/models/
+-rw-rw-rw-   0 root         (0) root         (0)      420 2024-04-14 19:26:03.000000 dyff_client-0.3.0/scripts/models/databricks--dolly-v2-3b--rox.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1374 2024-04-14 19:26:03.000000 dyff_client-0.3.0/scripts/models/databricks--dolly-v2-3b.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2024-04-14 19:26:03.000000 dyff_client-0.3.0/scripts/models/tiiuae--falcon-7b--rox.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1356 2024-04-14 19:26:03.000000 dyff_client-0.3.0/scripts/models/tiiuae--falcon-7b.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-14 19:26:09.727008 dyff_client-0.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 19:26:09.726009 dyff_client-0.3.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1123 2024-04-14 19:26:03.000000 dyff_client-0.3.0/tests/test_import.py
```

### Comparing `dyff-client-0.2.2/.gitlab-ci.yml` & `dyff_client-0.3.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.2/.licenserc.yaml` & `dyff_client-0.3.0/.licenserc.yaml`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.2/.pre-commit-config.yaml` & `dyff_client-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.2/.secrets.baseline` & `dyff_client-0.3.0/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.2/CODE_OF_CONDUCT.md` & `dyff_client-0.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.2/LICENSE` & `dyff_client-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.2/PKG-INFO` & `dyff_client-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-client
-Version: 0.2.2
+Version: 0.3.0
 Summary: Python client for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-client
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-client/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff-client-0.2.2/README.md` & `dyff_client-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.2/dyff/client/_generated/__init__.py` & `dyff_client-0.3.0/dyff/client/_generated/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.2)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.12)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from ._client import DyffAPI
+from ._client import DyffV0API
 
 try:
     from ._patch import *  # pylint: disable=unused-wildcard-import
     from ._patch import __all__ as _patch_all
 except ImportError:
     _patch_all = []
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
-    "DyffAPI",
+    "DyffV0API",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 
 _patch_sdk()
```

### Comparing `dyff-client-0.2.2/dyff/client/_generated/_client.py` & `dyff_client-0.3.0/dyff/client/_generated/aio/_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,64 +1,73 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.2)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.12)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
-from typing import Any
+from typing import Any, Awaitable
 
-from azure.core import PipelineClient
+from azure.core import AsyncPipelineClient
 from azure.core.pipeline import policies
-from azure.core.rest import HttpRequest, HttpResponse
+from azure.core.rest import AsyncHttpResponse, HttpRequest
 
-from ._configuration import DyffAPIConfiguration
-from ._serialization import Deserializer, Serializer
+from .._serialization import Deserializer, Serializer
+from ._configuration import DyffV0APIConfiguration
 from .operations import (
     AuditproceduresOperations,
     AuditsOperations,
     DatasetsOperations,
     EvaluationsOperations,
     InferenceservicesOperations,
     InferencesessionsOperations,
+    MeasurementsOperations,
+    MethodsOperations,
     ModelsOperations,
     ModulesOperations,
     ReportsOperations,
+    SafetycasesOperations,
 )
 
 
-class DyffAPI:  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
-    """DyffAPI.
+class DyffV0API:  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
+    """DyffV0API.
 
     :ivar audits: AuditsOperations operations
-    :vartype audits: _generated.operations.AuditsOperations
+    :vartype audits: _generated.aio.operations.AuditsOperations
     :ivar auditprocedures: AuditproceduresOperations operations
-    :vartype auditprocedures: _generated.operations.AuditproceduresOperations
+    :vartype auditprocedures: _generated.aio.operations.AuditproceduresOperations
     :ivar datasets: DatasetsOperations operations
-    :vartype datasets: _generated.operations.DatasetsOperations
+    :vartype datasets: _generated.aio.operations.DatasetsOperations
     :ivar evaluations: EvaluationsOperations operations
-    :vartype evaluations: _generated.operations.EvaluationsOperations
+    :vartype evaluations: _generated.aio.operations.EvaluationsOperations
     :ivar inferenceservices: InferenceservicesOperations operations
-    :vartype inferenceservices: _generated.operations.InferenceservicesOperations
+    :vartype inferenceservices: _generated.aio.operations.InferenceservicesOperations
     :ivar inferencesessions: InferencesessionsOperations operations
-    :vartype inferencesessions: _generated.operations.InferencesessionsOperations
+    :vartype inferencesessions: _generated.aio.operations.InferencesessionsOperations
+    :ivar measurements: MeasurementsOperations operations
+    :vartype measurements: _generated.aio.operations.MeasurementsOperations
+    :ivar methods: MethodsOperations operations
+    :vartype methods: _generated.aio.operations.MethodsOperations
     :ivar models: ModelsOperations operations
-    :vartype models: _generated.operations.ModelsOperations
+    :vartype models: _generated.aio.operations.ModelsOperations
     :ivar modules: ModulesOperations operations
-    :vartype modules: _generated.operations.ModulesOperations
+    :vartype modules: _generated.aio.operations.ModulesOperations
     :ivar reports: ReportsOperations operations
-    :vartype reports: _generated.operations.ReportsOperations
+    :vartype reports: _generated.aio.operations.ReportsOperations
+    :ivar safetycases: SafetycasesOperations operations
+    :vartype safetycases: _generated.aio.operations.SafetycasesOperations
     :keyword endpoint: Service URL. Required. Default value is "".
     :paramtype endpoint: str
     """
 
     def __init__(  # pylint: disable=missing-client-constructor-parameter-credential
         self, *, endpoint: str = "", **kwargs: Any
     ) -> None:
-        self._config = DyffAPIConfiguration(**kwargs)
+        self._config = DyffV0APIConfiguration(**kwargs)
         _policies = kwargs.pop("policies", None)
         if _policies is None:
             _policies = [
                 policies.RequestIdPolicy(**kwargs),
                 self._config.headers_policy,
                 self._config.user_agent_policy,
                 self._config.proxy_policy,
@@ -72,15 +81,15 @@
                 (
                     policies.SensitiveHeaderCleanupPolicy(**kwargs)
                     if self._config.redirect_policy
                     else None
                 ),
                 self._config.http_logging_policy,
             ]
-        self._client: PipelineClient = PipelineClient(
+        self._client: AsyncPipelineClient = AsyncPipelineClient(
             base_url=endpoint, policies=_policies, **kwargs
         )
 
         self._serialize = Serializer()
         self._deserialize = Deserializer()
         self._serialize.client_side_validation = False
         self.audits = AuditsOperations(
@@ -97,50 +106,59 @@
         )
         self.inferenceservices = InferenceservicesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.inferencesessions = InferencesessionsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
+        self.measurements = MeasurementsOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
+        self.methods = MethodsOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
         self.models = ModelsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.modules = ModulesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.reports = ReportsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
+        self.safetycases = SafetycasesOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
 
     def send_request(
         self, request: HttpRequest, *, stream: bool = False, **kwargs: Any
-    ) -> HttpResponse:
+    ) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
-        >>> response = client.send_request(request)
-        <HttpResponse: 200 OK>
+        >>> response = await client.send_request(request)
+        <AsyncHttpResponse: 200 OK>
 
         For more information on this code flow, see https://aka.ms/azsdk/dpcodegen/python/send_request
 
         :param request: The network request you want to make. Required.
         :type request: ~azure.core.rest.HttpRequest
         :keyword bool stream: Whether the response payload will be streamed. Defaults to False.
         :return: The response of your network call. Does not do error handling on your response.
-        :rtype: ~azure.core.rest.HttpResponse
+        :rtype: ~azure.core.rest.AsyncHttpResponse
         """
 
         request_copy = deepcopy(request)
         request_copy.url = self._client.format_url(request_copy.url)
         return self._client.send_request(request_copy, stream=stream, **kwargs)  # type: ignore
 
-    def close(self) -> None:
-        self._client.close()
+    async def close(self) -> None:
+        await self._client.close()
 
-    def __enter__(self) -> "DyffAPI":
-        self._client.__enter__()
+    async def __aenter__(self) -> "DyffV0API":
+        await self._client.__aenter__()
         return self
 
-    def __exit__(self, *exc_details: Any) -> None:
-        self._client.__exit__(*exc_details)
+    async def __aexit__(self, *exc_details: Any) -> None:
+        await self._client.__aexit__(*exc_details)
```

### Comparing `dyff-client-0.2.2/dyff/client/_generated/_configuration.py` & `dyff_client-0.3.0/dyff/client/_generated/_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.2)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.12)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any
 
 from azure.core.pipeline import policies
 
 VERSION = "unknown"
 
 
-class DyffAPIConfiguration:  # pylint: disable=too-many-instance-attributes
-    """Configuration for DyffAPI.
+class DyffV0APIConfiguration:  # pylint: disable=too-many-instance-attributes
+    """Configuration for DyffV0API.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
     """
 
     def __init__(self, **kwargs: Any) -> None:
 
-        kwargs.setdefault("sdk_moniker", "dyffapi/{}".format(VERSION))
+        kwargs.setdefault("sdk_moniker", "dyffv0api/{}".format(VERSION))
         self.polling_interval = kwargs.get("polling_interval", 30)
         self._configure(**kwargs)
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get(
             "user_agent_policy"
         ) or policies.UserAgentPolicy(**kwargs)
```

### Comparing `dyff-client-0.2.2/dyff/client/_generated/_patch.py` & `dyff_client-0.3.0/dyff/client/_generated/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.2/dyff/client/_generated/_serialization.py` & `dyff_client-0.3.0/dyff/client/_generated/_serialization.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.2/dyff/client/_generated/_vendor.py` & `dyff_client-0.3.0/dyff/client/_generated/_vendor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.2)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.12)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 
 def raise_if_not_implemented(cls, abstract_methods):
     not_implemented = [
         f for f in abstract_methods if not callable(getattr(cls, f, None))
```

### Comparing `dyff-client-0.2.2/dyff/client/_generated/aio/__init__.py` & `dyff_client-0.3.0/dyff/client/_generated/aio/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.2)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.12)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from ._client import DyffAPI
+from ._client import DyffV0API
 
 try:
     from ._patch import *  # pylint: disable=unused-wildcard-import
     from ._patch import __all__ as _patch_all
 except ImportError:
     _patch_all = []
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
-    "DyffAPI",
+    "DyffV0API",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 
 _patch_sdk()
```

### Comparing `dyff-client-0.2.2/dyff/client/_generated/aio/_client.py` & `dyff_client-0.3.0/dyff/client/_generated/_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,64 +1,69 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.2)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.12)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
-from typing import Any, Awaitable
+from typing import Any
 
-from azure.core import AsyncPipelineClient
+from azure.core import PipelineClient
 from azure.core.pipeline import policies
-from azure.core.rest import AsyncHttpResponse, HttpRequest
+from azure.core.rest import HttpRequest, HttpResponse
 
-from .._serialization import Deserializer, Serializer
-from ._configuration import DyffAPIConfiguration
+from ._configuration import DyffV0APIConfiguration
+from ._serialization import Deserializer, Serializer
 from .operations import (
     AuditproceduresOperations,
     AuditsOperations,
     DatasetsOperations,
     EvaluationsOperations,
     InferenceservicesOperations,
     InferencesessionsOperations,
+    MeasurementsOperations,
+    MethodsOperations,
     ModelsOperations,
     ModulesOperations,
     ReportsOperations,
+    SafetycasesOperations,
 )
 
 
-class DyffAPI:  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
-    """DyffAPI.
+class DyffV0API:  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
+    """DyffV0API.
 
-    :ivar audits: AuditsOperations operations
-    :vartype audits: _generated.aio.operations.AuditsOperations
-    :ivar auditprocedures: AuditproceduresOperations operations
-    :vartype auditprocedures: _generated.aio.operations.AuditproceduresOperations
-    :ivar datasets: DatasetsOperations operations
-    :vartype datasets: _generated.aio.operations.DatasetsOperations
-    :ivar evaluations: EvaluationsOperations operations
-    :vartype evaluations: _generated.aio.operations.EvaluationsOperations
-    :ivar inferenceservices: InferenceservicesOperations operations
-    :vartype inferenceservices: _generated.aio.operations.InferenceservicesOperations
-    :ivar inferencesessions: InferencesessionsOperations operations
-    :vartype inferencesessions: _generated.aio.operations.InferencesessionsOperations
-    :ivar models: ModelsOperations operations
-    :vartype models: _generated.aio.operations.ModelsOperations
-    :ivar modules: ModulesOperations operations
-    :vartype modules: _generated.aio.operations.ModulesOperations
-    :ivar reports: ReportsOperations operations
-    :vartype reports: _generated.aio.operations.ReportsOperations
-    :keyword endpoint: Service URL. Required. Default value is "".
+    :ivar audits: AuditsOperations operations :vartype audits:
+    _generated.operations.AuditsOperations :ivar auditprocedures:
+    AuditproceduresOperations operations :vartype auditprocedures:
+    _generated.operations.AuditproceduresOperations :ivar datasets: DatasetsOperations
+    operations :vartype datasets: _generated.operations.DatasetsOperations :ivar
+    evaluations: EvaluationsOperations operations :vartype evaluations:
+    _generated.operations.EvaluationsOperations :ivar inferenceservices:
+    InferenceservicesOperations operations :vartype inferenceservices:
+    _generated.operations.InferenceservicesOperations :ivar inferencesessions:
+    InferencesessionsOperations operations :vartype inferencesessions:
+    _generated.operations.InferencesessionsOperations :ivar measurements:
+    MeasurementsOperations operations :vartype measurements:
+    _generated.operations.MeasurementsOperations :ivar methods: MethodsOperations
+    operations :vartype methods: _generated.operations.MethodsOperations :ivar models:
+    ModelsOperations operations :vartype models: _generated.operations.ModelsOperations
+    :ivar modules: ModulesOperations operations :vartype modules:
+    _generated.operations.ModulesOperations :ivar reports: ReportsOperations operations
+    :vartype reports: _generated.operations.ReportsOperations :ivar safetycases:
+    SafetycasesOperations operations :vartype safetycases:
+    _generated.operations.SafetycasesOperations :keyword endpoint: Service URL.
+    Required. Default value is "".
     :paramtype endpoint: str
     """
 
     def __init__(  # pylint: disable=missing-client-constructor-parameter-credential
         self, *, endpoint: str = "", **kwargs: Any
     ) -> None:
-        self._config = DyffAPIConfiguration(**kwargs)
+        self._config = DyffV0APIConfiguration(**kwargs)
         _policies = kwargs.pop("policies", None)
         if _policies is None:
             _policies = [
                 policies.RequestIdPolicy(**kwargs),
                 self._config.headers_policy,
                 self._config.user_agent_policy,
                 self._config.proxy_policy,
@@ -72,15 +77,15 @@
                 (
                     policies.SensitiveHeaderCleanupPolicy(**kwargs)
                     if self._config.redirect_policy
                     else None
                 ),
                 self._config.http_logging_policy,
             ]
-        self._client: AsyncPipelineClient = AsyncPipelineClient(
+        self._client: PipelineClient = PipelineClient(
             base_url=endpoint, policies=_policies, **kwargs
         )
 
         self._serialize = Serializer()
         self._deserialize = Deserializer()
         self._serialize.client_side_validation = False
         self.audits = AuditsOperations(
@@ -97,50 +102,59 @@
         )
         self.inferenceservices = InferenceservicesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.inferencesessions = InferencesessionsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
+        self.measurements = MeasurementsOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
+        self.methods = MethodsOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
         self.models = ModelsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.modules = ModulesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.reports = ReportsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
+        self.safetycases = SafetycasesOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
 
     def send_request(
         self, request: HttpRequest, *, stream: bool = False, **kwargs: Any
-    ) -> Awaitable[AsyncHttpResponse]:
+    ) -> HttpResponse:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
-        >>> response = await client.send_request(request)
-        <AsyncHttpResponse: 200 OK>
+        >>> response = client.send_request(request)
+        <HttpResponse: 200 OK>
 
         For more information on this code flow, see https://aka.ms/azsdk/dpcodegen/python/send_request
 
         :param request: The network request you want to make. Required.
         :type request: ~azure.core.rest.HttpRequest
         :keyword bool stream: Whether the response payload will be streamed. Defaults to False.
         :return: The response of your network call. Does not do error handling on your response.
-        :rtype: ~azure.core.rest.AsyncHttpResponse
+        :rtype: ~azure.core.rest.HttpResponse
         """
 
         request_copy = deepcopy(request)
         request_copy.url = self._client.format_url(request_copy.url)
         return self._client.send_request(request_copy, stream=stream, **kwargs)  # type: ignore
 
-    async def close(self) -> None:
-        await self._client.close()
+    def close(self) -> None:
+        self._client.close()
 
-    async def __aenter__(self) -> "DyffAPI":
-        await self._client.__aenter__()
+    def __enter__(self) -> "DyffV0API":
+        self._client.__enter__()
         return self
 
-    async def __aexit__(self, *exc_details: Any) -> None:
-        await self._client.__aexit__(*exc_details)
+    def __exit__(self, *exc_details: Any) -> None:
+        self._client.__exit__(*exc_details)
```

### Comparing `dyff-client-0.2.2/dyff/client/_generated/aio/_configuration.py` & `dyff_client-0.3.0/dyff/client/_generated/aio/_configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.2)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.12)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any
 
 from azure.core.pipeline import policies
 
 VERSION = "unknown"
 
 
-class DyffAPIConfiguration:  # pylint: disable=too-many-instance-attributes
-    """Configuration for DyffAPI.
+class DyffV0APIConfiguration:  # pylint: disable=too-many-instance-attributes
+    """Configuration for DyffV0API.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
     """
 
     def __init__(self, **kwargs: Any) -> None:
 
-        kwargs.setdefault("sdk_moniker", "dyffapi/{}".format(VERSION))
+        kwargs.setdefault("sdk_moniker", "dyffv0api/{}".format(VERSION))
         self.polling_interval = kwargs.get("polling_interval", 30)
         self._configure(**kwargs)
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get(
             "user_agent_policy"
         ) or policies.UserAgentPolicy(**kwargs)
```

### Comparing `dyff-client-0.2.2/dyff/client/_generated/aio/_patch.py` & `dyff_client-0.3.0/dyff/client/_generated/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.2/dyff/client/_generated/aio/_vendor.py` & `dyff_client-0.3.0/dyff/client/_generated/aio/_vendor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.2)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.12)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 
 def raise_if_not_implemented(cls, abstract_methods):
     not_implemented = [
         f for f in abstract_methods if not callable(getattr(cls, f, None))
```

### Comparing `dyff-client-0.2.2/dyff/client/_generated/aio/operations/__init__.py` & `dyff_client-0.3.0/dyff/client/_generated/aio/operations/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.2)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.12)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._operations import (
     AuditproceduresOperations,
     AuditsOperations,
     DatasetsOperations,
     EvaluationsOperations,
     InferenceservicesOperations,
     InferencesessionsOperations,
+    MeasurementsOperations,
+    MethodsOperations,
     ModelsOperations,
     ModulesOperations,
     ReportsOperations,
+    SafetycasesOperations,
 )
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import __all__ as _patch_all
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "AuditsOperations",
     "AuditproceduresOperations",
     "DatasetsOperations",
     "EvaluationsOperations",
     "InferenceservicesOperations",
     "InferencesessionsOperations",
+    "MeasurementsOperations",
+    "MethodsOperations",
     "ModelsOperations",
     "ModulesOperations",
     "ReportsOperations",
+    "SafetycasesOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

### Comparing `dyff-client-0.2.2/dyff/client/_generated/aio/operations/_operations.py` & `dyff_client-0.3.0/dyff/client/_generated/aio/operations/_operations.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.2)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.12)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 import sys
 from io import IOBase
 from typing import (
     IO,
     Any,
     AsyncIterator,
     Callable,
     Dict,
     List,
     Optional,
+    Type,
     TypeVar,
     Union,
     cast,
     overload,
 )
 
 from azure.core.exceptions import (
@@ -63,14 +64,24 @@
     build_inferencesessions_get_request,
     build_inferencesessions_infer_request,
     build_inferencesessions_label_request,
     build_inferencesessions_query_request,
     build_inferencesessions_ready_request,
     build_inferencesessions_terminate_request,
     build_inferencesessions_token_request,
+    build_measurements_create_request,
+    build_measurements_delete_request,
+    build_measurements_get_request,
+    build_measurements_label_request,
+    build_measurements_query_request,
+    build_methods_create_request,
+    build_methods_delete_request,
+    build_methods_get_request,
+    build_methods_label_request,
+    build_methods_query_request,
     build_models_create_request,
     build_models_delete_request,
     build_models_get_request,
     build_models_label_request,
     build_models_query_request,
     build_modules_create_request,
     build_modules_delete_request,
@@ -81,14 +92,19 @@
     build_modules_upload_request,
     build_reports_create_request,
     build_reports_data_request,
     build_reports_delete_request,
     build_reports_get_request,
     build_reports_label_request,
     build_reports_query_request,
+    build_safetycases_create_request,
+    build_safetycases_delete_request,
+    build_safetycases_get_request,
+    build_safetycases_label_request,
+    build_safetycases_query_request,
 )
 from .._vendor import raise_if_not_implemented
 
 if sys.version_info >= (3, 9):
     from collections.abc import MutableMapping
 else:
     from typing import (
@@ -103,15 +119,15 @@
 
 class AuditsOperations:  # pylint: disable=abstract-class-instantiated
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~_generated.aio.DyffAPI`'s
+        :class:`~_generated.aio.DyffV0API`'s
         :attr:`audits` attribute.
     """
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
@@ -267,15 +283,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -427,15 +443,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -551,15 +567,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -638,15 +654,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -699,15 +715,15 @@
 
 class AuditproceduresOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~_generated.aio.DyffAPI`'s
+        :class:`~_generated.aio.DyffV0API`'s
         :attr:`auditprocedures` attribute.
     """
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
@@ -722,15 +738,15 @@
     ) -> Union[AsyncIterator[bytes], JSON]:
         """Download the source code of an AuditProcedure.
 
         Download the source code of an AuditProcedure.
 
         :param path: Required.
         :type path: str
-        :return: Async iterator of the response bytes or JSON object or None
+        :return: AsyncIterator[bytes] or JSON object or None
         :rtype: AsyncIterator[bytes] or JSON or None
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 422
@@ -742,15 +758,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -798,15 +814,15 @@
 
 class DatasetsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~_generated.aio.DyffAPI`'s
+        :class:`~_generated.aio.DyffV0API`'s
         :attr:`datasets` attribute.
     """
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
@@ -955,15 +971,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1172,15 +1188,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1726,15 +1742,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1912,15 +1928,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1977,15 +1993,15 @@
         """Get the strata corresponding to a Dataset.
 
         Get the strata corresponding to a Dataset. The data is returned as a
         Parquet file suitable for reading with libraries like Pandas.
 
         :param dataset_id: Required.
         :type dataset_id: str
-        :return: Async iterator of the response bytes or JSON object or None
+        :return: AsyncIterator[bytes] or JSON object or None
         :rtype: AsyncIterator[bytes] or JSON or None
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 422
@@ -1997,15 +2013,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -2057,15 +2073,15 @@
         """Get the raw data for the Dataset.
 
         Get the raw data for the Dataset. The data is streamed in pyarrow.ipc
         format.
 
         :param dataset_id: Required.
         :type dataset_id: str
-        :return: Async iterator of the response bytes or JSON object or None
+        :return: AsyncIterator[bytes] or JSON object or None
         :rtype: AsyncIterator[bytes] or JSON or None
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 422
@@ -2077,15 +2093,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -2159,15 +2175,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -2252,15 +2268,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -2335,15 +2351,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -2396,15 +2412,15 @@
 
 class EvaluationsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~_generated.aio.DyffAPI`'s
+        :class:`~_generated.aio.DyffV0API`'s
         :attr:`evaluations` attribute.
     """
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
@@ -2553,15 +2569,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -2896,15 +2912,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -3724,15 +3740,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -4018,15 +4034,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -4105,15 +4121,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -4166,15 +4182,15 @@
 
 class InferenceservicesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~_generated.aio.DyffAPI`'s
+        :class:`~_generated.aio.DyffV0API`'s
         :attr:`inferenceservices` attribute.
     """
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
@@ -4323,15 +4339,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -4609,15 +4625,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -5449,15 +5465,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -5699,15 +5715,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -5786,15 +5802,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -5847,15 +5863,15 @@
 
 class InferencesessionsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~_generated.aio.DyffAPI`'s
+        :class:`~_generated.aio.DyffV0API`'s
         :attr:`inferencesessions` attribute.
     """
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
@@ -6004,15 +6020,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -6330,15 +6346,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7135,15 +7151,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7410,15 +7426,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7497,15 +7513,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7584,15 +7600,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7670,15 +7686,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7753,15 +7769,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7841,15 +7857,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7896,21 +7912,3015 @@
 
         if cls:
             return cls(pipeline_response, cast(Union[Any, JSON], deserialized), {})  # type: ignore
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
 
+class MeasurementsOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~_generated.aio.DyffV0API`'s
+        :attr:`measurements` attribute.
+    """
+
+    def __init__(self, *args, **kwargs) -> None:
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = (
+            input_args.pop(0) if input_args else kwargs.pop("deserializer")
+        )
+
+    @overload
+    async def label(
+        self,
+        measurement_id: str,
+        body: JSON,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> Union[Any, JSON]:
+        # pylint: disable=line-too-long
+        """Update labels for an existing Measurement.
+
+        Update labels for an existing Measurement.
+
+        :param measurement_id: Required.
+        :type measurement_id: str
+        :param body: Required.
+        :type body: JSON
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: any or JSON object
+        :rtype: any or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    }
+                }
+
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @overload
+    async def label(
+        self,
+        measurement_id: str,
+        body: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> Union[Any, JSON]:
+        """Update labels for an existing Measurement.
+
+        Update labels for an existing Measurement.
+
+        :param measurement_id: Required.
+        :type measurement_id: str
+        :param body: Required.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: any or JSON object
+        :rtype: any or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @distributed_trace_async
+    async def label(
+        self, measurement_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any
+    ) -> Union[Any, JSON]:
+        # pylint: disable=line-too-long
+        """Update labels for an existing Measurement.
+
+        Update labels for an existing Measurement.
+
+        :param measurement_id: Required.
+        :type measurement_id: str
+        :param body: Is either a JSON type or a IO[bytes] type. Required.
+        :type body: JSON or IO[bytes]
+        :return: any or JSON object
+        :rtype: any or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    }
+                }
+
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop(
+            "content_type", _headers.pop("Content-Type", None)
+        )
+        cls: ClsType[Union[Any, JSON]] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        _request = build_measurements_label_request(
+            measurement_id=measurement_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(Union[Any, JSON], deserialized), {})  # type: ignore
+
+        return cast(Union[Any, JSON], deserialized)  # type: ignore
+
+    @distributed_trace_async
+    async def query(
+        self,
+        *,
+        id: Optional[str] = None,
+        account: Optional[str] = None,
+        status: Optional[str] = None,
+        reason: Optional[str] = None,
+        labels: Optional[str] = None,
+        analysis: Optional[str] = None,
+        method: Optional[str] = None,
+        method_name: Optional[str] = None,
+        inputs_any_of: Optional[str] = None,
+        **kwargs: Any,
+    ) -> Union[List[JSON], JSON]:
+        # pylint: disable=line-too-long
+        """Get all Measurements matching a query.
+
+        Get all Measurements matching a query. The query is a set of equality
+        constraints specified as key-value pairs.
+
+        :keyword id: Default value is None.
+        :paramtype id: str
+        :keyword account: Default value is None.
+        :paramtype account: str
+        :keyword status: Default value is None.
+        :paramtype status: str
+        :keyword reason: Default value is None.
+        :paramtype reason: str
+        :keyword labels: Default value is None.
+        :paramtype labels: str
+        :keyword analysis: Default value is None.
+        :paramtype analysis: str
+        :keyword method: Default value is None.
+        :paramtype method: str
+        :keyword method_name: Default value is None.
+        :paramtype method_name: str
+        :keyword inputs_any_of: Default value is None.
+        :paramtype inputs_any_of: str
+        :return: list of JSON object or JSON object
+        :rtype: list[JSON] or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == [
+                    {
+                        "account": "str",  # Account that owns the entity. Required.
+                        "id": "str",  # Unique identifier of the entity. Required.
+                        "level": "str",  # Measurement level. Required. Known values are:
+                          "Dataset" and "Instance".
+                        "method": {
+                            "account": "str",  # Account that owns the entity. Required.
+                            "id": "str",  # Unique identifier of the entity. Required.
+                            "implementation": {
+                                "kind": "str",  # The kind of implementation.
+                                  Required.
+                                "jupyterNotebook": {
+                                    "notebookModule": "str",  # ID of the Module
+                                      that contains the notebook file. This does *not* add the Module
+                                      as a dependency; you must do that separately. Required.
+                                    "notebookPath": "str"  # Path to the notebook
+                                      file relative to the Module root directory. Required.
+                                },
+                                "pythonFunction": {
+                                    "fullyQualifiedName": "str"  # The
+                                      fully-qualified name of the Python function to call. Required.
+                                },
+                                "pythonRubric": {
+                                    "fullyQualifiedName": "str"  # The
+                                      fully-qualified name of the Python Rubric to run. Required.
+                                }
+                            },
+                            "name": "str",  # Descriptive name of the Method. Required.
+                            "output": {
+                                "kind": "str",  # The kind of output artifact.
+                                  Required. Known values are: "Measurement" and "SafetyCase".
+                                "measurement": {
+                                    "level": "str",  # Measurement level.
+                                      Required. Known values are: "Dataset" and "Instance".
+                                    "name": "str",  # Descriptive name of the
+                                      Measurement. Required.
+                                    "schema": {
+                                        "arrowSchema": "str",  # The schema
+                                          in Arrow format, encoded with
+                                          dyff.schema.arrow.encode_schema(). This is required, but can
+                                          be populated from a DyffDataSchema. Required.
+                                        "dyffSchema": {
+                                            "components": [
+                                                "str"  # A list of
+                                                  named dyff data schemas. The final schema is the
+                                                  composition of these component schemas. Required.
+                                            ],
+                                            "schemaVersion": "0.1"  #
+                                              Optional. Default value is "0.1". The dyff schema
+                                              version. "0.1"
+                                        },
+                                        "jsonSchema": {}  # Optional. The
+                                          schema in JSON Schema format.
+                                    },
+                                    "description": "str"  # Optional. Long-form
+                                      description, interpreted as Markdown.
+                                },
+                                "safetyCase": {
+                                    "name": "str",  # Descriptive name of the
+                                      SafetyCase. Required.
+                                    "description": "str"  # Optional. Long-form
+                                      description, interpreted as Markdown.
+                                }
+                            },
+                            "scope": "str",  # The scope of the Method. The Method
+                              produces outputs that are specific to one entity of the type specified in
+                              the .scope field. Required. Known values are: "InferenceService" and
+                              "Evaluation".
+                            "description": "str",  # Optional. Long-form description,
+                              interpreted as Markdown.
+                            "inputs": [
+                                {
+                                    "keyword": "str",  # The input is referred to
+                                      by 'keyword' in the context of the method implementation.
+                                      Required.
+                                    "kind": "str",  # The kind of input artifact.
+                                      Required. Known values are: "Dataset", "Evaluation",
+                                      "Measurement", and "Report".
+                                    "description": "str"  # Optional. Long-form
+                                      description, interpreted as Markdown.
+                                }
+                            ],
+                            "modules": [
+                                "str"  # Optional. Modules to load into the analysis
+                                  environment.
+                            ],
+                            "parameters": [
+                                {
+                                    "keyword": "str",  # The parameter is
+                                      referred to by 'keyword' in the context of the method
+                                      implementation. Required.
+                                    "description": "str"  # Optional. Long-form
+                                      description, interpreted as Markdown.
+                                }
+                            ]
+                        },
+                        "name": "str",  # Descriptive name of the Measurement. Required.
+                        "schema": {
+                            "arrowSchema": "str",  # The schema in Arrow format, encoded
+                              with dyff.schema.arrow.encode_schema(). This is required, but can be
+                              populated from a DyffDataSchema. Required.
+                            "dyffSchema": {
+                                "components": [
+                                    "str"  # A list of named dyff data schemas.
+                                      The final schema is the composition of these component schemas.
+                                      Required.
+                                ],
+                                "schemaVersion": "0.1"  # Optional. Default value is
+                                  "0.1". The dyff schema version. "0.1"
+                            },
+                            "jsonSchema": {}  # Optional. The schema in JSON Schema
+                              format.
+                        },
+                        "scope": {
+                            "dataset": "str",  # Optional. Dataset.
+                            "evaluation": "str",  # Optional. Evaluation.
+                            "inferenceService": "str",  # Optional. Inferenceservice.
+                            "model": "str"  # Optional. Model.
+                        },
+                        "annotations": [
+                            {
+                                "key": "str",  # The annotation key. A DNS label with
+                                  an optional DNS domain prefix. For example: 'my-key',
+                                  'your.com/key_0'. Names prefixed with 'dyff.io/',
+                                  'subdomain.dyff.io/', etc. are reserved.  See
+                                  https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                                  for detailed naming rules. Required.
+                                "value": "str"  # The annotation value. An arbitrary
+                                  string. Required.
+                            }
+                        ],
+                        "arguments": [
+                            {
+                                "keyword": "str",  # The 'keyword' of the
+                                  corresponding ModelParameter. Required.
+                                "value": "str"  # The value of of the argument.
+                                  Always a string; implementations are responsible for parsing.
+                                  Required.
+                            }
+                        ],
+                        "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation
+                          time (assigned by system).
+                        "description": "str",  # Optional. Long-form description, interpreted
+                          as Markdown.
+                        "inputs": [
+                            {
+                                "entity": "str",  # The ID of the entity whose data
+                                  should be made available as 'keyword'. Required.
+                                "keyword": "str"  # The 'keyword' specified for this
+                                  input in the MethodSpec. Required.
+                            }
+                        ],
+                        "kind": "Measurement",  # Optional. Default value is "Measurement".
+                          Kind. "Measurement"
+                        "labels": {
+                            "str": "str"  # Optional. A set of key-value labels for the
+                              resource. Used to specify identifying attributes of resources that are
+                              meaningful to users but do not imply semantics in the dyff system.  The
+                              keys are DNS labels with an optional DNS domain prefix. For example:
+                              'my-key', 'your.com/key_0'. Keys prefixed with 'dyff.io/',
+                              'subdomain.dyff.io/', etc. are reserved.  The label values are
+                              alphanumeric characters separated by '.', '-', or '_'.  We follow the
+                              kubernetes label conventions closely. See:
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                        },
+                        "reason": "str",  # Optional. Reason for current status (assigned by
+                          system).
+                        "schemaVersion": "0.1",  # Optional. Default value is "0.1". The
+                          schema version. "0.1"
+                        "status": "str"  # Optional. Top-level resource status (assigned by
+                          system).
+                    }
+                ]
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
+
+        _request = build_measurements_query_request(
+            id=id,
+            account=account,
+            status=status,
+            reason=reason,
+            labels=labels,
+            analysis=analysis,
+            method=method,
+            method_name=method_name,
+            inputs_any_of=inputs_any_of,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(Union[List[JSON], JSON], deserialized), {})  # type: ignore
+
+        return cast(Union[List[JSON], JSON], deserialized)  # type: ignore
+
+    @overload
+    async def create(
+        self, body: JSON, *, content_type: str = "application/json", **kwargs: Any
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Create a Measurement.
+
+        Create a Measurement.
+
+        :param body: Required.
+        :type body: JSON
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "method": "str",  # Method ID. Required.
+                    "scope": {
+                        "dataset": "str",  # Optional. Dataset.
+                        "evaluation": "str",  # Optional. Evaluation.
+                        "inferenceService": "str",  # Optional. Inferenceservice.
+                        "model": "str"  # Optional. Model.
+                    },
+                    "arguments": [
+                        {
+                            "keyword": "str",  # The 'keyword' of the corresponding
+                              ModelParameter. Required.
+                            "value": "str"  # The value of of the argument. Always a
+                              string; implementations are responsible for parsing. Required.
+                        }
+                    ],
+                    "inputs": [
+                        {
+                            "entity": "str",  # The ID of the entity whose data should be
+                              made available as 'keyword'. Required.
+                            "keyword": "str"  # The 'keyword' specified for this input in
+                              the MethodSpec. Required.
+                        }
+                    ],
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "id": "str",  # Unique identifier of the entity. Required.
+                    "level": "str",  # Measurement level. Required. Known values are: "Dataset"
+                      and "Instance".
+                    "method": {
+                        "account": "str",  # Account that owns the entity. Required.
+                        "id": "str",  # Unique identifier of the entity. Required.
+                        "implementation": {
+                            "kind": "str",  # The kind of implementation. Required.
+                            "jupyterNotebook": {
+                                "notebookModule": "str",  # ID of the Module that
+                                  contains the notebook file. This does *not* add the Module as a
+                                  dependency; you must do that separately. Required.
+                                "notebookPath": "str"  # Path to the notebook file
+                                  relative to the Module root directory. Required.
+                            },
+                            "pythonFunction": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python function to call. Required.
+                            },
+                            "pythonRubric": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python Rubric to run. Required.
+                            }
+                        },
+                        "name": "str",  # Descriptive name of the Method. Required.
+                        "output": {
+                            "kind": "str",  # The kind of output artifact. Required.
+                              Known values are: "Measurement" and "SafetyCase".
+                            "measurement": {
+                                "level": "str",  # Measurement level. Required. Known
+                                  values are: "Dataset" and "Instance".
+                                "name": "str",  # Descriptive name of the
+                                  Measurement. Required.
+                                "schema": {
+                                    "arrowSchema": "str",  # The schema in Arrow
+                                      format, encoded with dyff.schema.arrow.encode_schema(). This is
+                                      required, but can be populated from a DyffDataSchema. Required.
+                                    "dyffSchema": {
+                                        "components": [
+                                            "str"  # A list of named dyff
+                                              data schemas. The final schema is the composition of
+                                              these component schemas. Required.
+                                        ],
+                                        "schemaVersion": "0.1"  # Optional.
+                                          Default value is "0.1". The dyff schema version. "0.1"
+                                    },
+                                    "jsonSchema": {}  # Optional. The schema in
+                                      JSON Schema format.
+                                },
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            },
+                            "safetyCase": {
+                                "name": "str",  # Descriptive name of the SafetyCase.
+                                  Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        },
+                        "scope": "str",  # The scope of the Method. The Method produces
+                          outputs that are specific to one entity of the type specified in the .scope
+                          field. Required. Known values are: "InferenceService" and "Evaluation".
+                        "description": "str",  # Optional. Long-form description, interpreted
+                          as Markdown.
+                        "inputs": [
+                            {
+                                "keyword": "str",  # The input is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "kind": "str",  # The kind of input artifact.
+                                  Required. Known values are: "Dataset", "Evaluation", "Measurement",
+                                  and "Report".
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ],
+                        "modules": [
+                            "str"  # Optional. Modules to load into the analysis
+                              environment.
+                        ],
+                        "parameters": [
+                            {
+                                "keyword": "str",  # The parameter is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ]
+                    },
+                    "name": "str",  # Descriptive name of the Measurement. Required.
+                    "schema": {
+                        "arrowSchema": "str",  # The schema in Arrow format, encoded with
+                          dyff.schema.arrow.encode_schema(). This is required, but can be populated
+                          from a DyffDataSchema. Required.
+                        "dyffSchema": {
+                            "components": [
+                                "str"  # A list of named dyff data schemas. The final
+                                  schema is the composition of these component schemas. Required.
+                            ],
+                            "schemaVersion": "0.1"  # Optional. Default value is "0.1".
+                              The dyff schema version. "0.1"
+                        },
+                        "jsonSchema": {}  # Optional. The schema in JSON Schema format.
+                    },
+                    "scope": {
+                        "dataset": "str",  # Optional. Dataset.
+                        "evaluation": "str",  # Optional. Evaluation.
+                        "inferenceService": "str",  # Optional. Inferenceservice.
+                        "model": "str"  # Optional. Model.
+                    },
+                    "annotations": [
+                        {
+                            "key": "str",  # The annotation key. A DNS label with an
+                              optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                              Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
+                              See
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                              for detailed naming rules. Required.
+                            "value": "str"  # The annotation value. An arbitrary string.
+                              Required.
+                        }
+                    ],
+                    "arguments": [
+                        {
+                            "keyword": "str",  # The 'keyword' of the corresponding
+                              ModelParameter. Required.
+                            "value": "str"  # The value of of the argument. Always a
+                              string; implementations are responsible for parsing. Required.
+                        }
+                    ],
+                    "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
+                      (assigned by system).
+                    "description": "str",  # Optional. Long-form description, interpreted as
+                      Markdown.
+                    "inputs": [
+                        {
+                            "entity": "str",  # The ID of the entity whose data should be
+                              made available as 'keyword'. Required.
+                            "keyword": "str"  # The 'keyword' specified for this input in
+                              the MethodSpec. Required.
+                        }
+                    ],
+                    "kind": "Measurement",  # Optional. Default value is "Measurement". Kind.
+                      "Measurement"
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    },
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @overload
+    async def create(
+        self, body: IO[bytes], *, content_type: str = "application/json", **kwargs: Any
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Create a Measurement.
+
+        Create a Measurement.
+
+        :param body: Required.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "id": "str",  # Unique identifier of the entity. Required.
+                    "level": "str",  # Measurement level. Required. Known values are: "Dataset"
+                      and "Instance".
+                    "method": {
+                        "account": "str",  # Account that owns the entity. Required.
+                        "id": "str",  # Unique identifier of the entity. Required.
+                        "implementation": {
+                            "kind": "str",  # The kind of implementation. Required.
+                            "jupyterNotebook": {
+                                "notebookModule": "str",  # ID of the Module that
+                                  contains the notebook file. This does *not* add the Module as a
+                                  dependency; you must do that separately. Required.
+                                "notebookPath": "str"  # Path to the notebook file
+                                  relative to the Module root directory. Required.
+                            },
+                            "pythonFunction": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python function to call. Required.
+                            },
+                            "pythonRubric": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python Rubric to run. Required.
+                            }
+                        },
+                        "name": "str",  # Descriptive name of the Method. Required.
+                        "output": {
+                            "kind": "str",  # The kind of output artifact. Required.
+                              Known values are: "Measurement" and "SafetyCase".
+                            "measurement": {
+                                "level": "str",  # Measurement level. Required. Known
+                                  values are: "Dataset" and "Instance".
+                                "name": "str",  # Descriptive name of the
+                                  Measurement. Required.
+                                "schema": {
+                                    "arrowSchema": "str",  # The schema in Arrow
+                                      format, encoded with dyff.schema.arrow.encode_schema(). This is
+                                      required, but can be populated from a DyffDataSchema. Required.
+                                    "dyffSchema": {
+                                        "components": [
+                                            "str"  # A list of named dyff
+                                              data schemas. The final schema is the composition of
+                                              these component schemas. Required.
+                                        ],
+                                        "schemaVersion": "0.1"  # Optional.
+                                          Default value is "0.1". The dyff schema version. "0.1"
+                                    },
+                                    "jsonSchema": {}  # Optional. The schema in
+                                      JSON Schema format.
+                                },
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            },
+                            "safetyCase": {
+                                "name": "str",  # Descriptive name of the SafetyCase.
+                                  Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        },
+                        "scope": "str",  # The scope of the Method. The Method produces
+                          outputs that are specific to one entity of the type specified in the .scope
+                          field. Required. Known values are: "InferenceService" and "Evaluation".
+                        "description": "str",  # Optional. Long-form description, interpreted
+                          as Markdown.
+                        "inputs": [
+                            {
+                                "keyword": "str",  # The input is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "kind": "str",  # The kind of input artifact.
+                                  Required. Known values are: "Dataset", "Evaluation", "Measurement",
+                                  and "Report".
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ],
+                        "modules": [
+                            "str"  # Optional. Modules to load into the analysis
+                              environment.
+                        ],
+                        "parameters": [
+                            {
+                                "keyword": "str",  # The parameter is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ]
+                    },
+                    "name": "str",  # Descriptive name of the Measurement. Required.
+                    "schema": {
+                        "arrowSchema": "str",  # The schema in Arrow format, encoded with
+                          dyff.schema.arrow.encode_schema(). This is required, but can be populated
+                          from a DyffDataSchema. Required.
+                        "dyffSchema": {
+                            "components": [
+                                "str"  # A list of named dyff data schemas. The final
+                                  schema is the composition of these component schemas. Required.
+                            ],
+                            "schemaVersion": "0.1"  # Optional. Default value is "0.1".
+                              The dyff schema version. "0.1"
+                        },
+                        "jsonSchema": {}  # Optional. The schema in JSON Schema format.
+                    },
+                    "scope": {
+                        "dataset": "str",  # Optional. Dataset.
+                        "evaluation": "str",  # Optional. Evaluation.
+                        "inferenceService": "str",  # Optional. Inferenceservice.
+                        "model": "str"  # Optional. Model.
+                    },
+                    "annotations": [
+                        {
+                            "key": "str",  # The annotation key. A DNS label with an
+                              optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                              Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
+                              See
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                              for detailed naming rules. Required.
+                            "value": "str"  # The annotation value. An arbitrary string.
+                              Required.
+                        }
+                    ],
+                    "arguments": [
+                        {
+                            "keyword": "str",  # The 'keyword' of the corresponding
+                              ModelParameter. Required.
+                            "value": "str"  # The value of of the argument. Always a
+                              string; implementations are responsible for parsing. Required.
+                        }
+                    ],
+                    "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
+                      (assigned by system).
+                    "description": "str",  # Optional. Long-form description, interpreted as
+                      Markdown.
+                    "inputs": [
+                        {
+                            "entity": "str",  # The ID of the entity whose data should be
+                              made available as 'keyword'. Required.
+                            "keyword": "str"  # The 'keyword' specified for this input in
+                              the MethodSpec. Required.
+                        }
+                    ],
+                    "kind": "Measurement",  # Optional. Default value is "Measurement". Kind.
+                      "Measurement"
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    },
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @distributed_trace_async
+    async def create(self, body: Union[JSON, IO[bytes]], **kwargs: Any) -> JSON:
+        # pylint: disable=line-too-long
+        """Create a Measurement.
+
+        Create a Measurement.
+
+        :param body: Is either a JSON type or a IO[bytes] type. Required.
+        :type body: JSON or IO[bytes]
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "method": "str",  # Method ID. Required.
+                    "scope": {
+                        "dataset": "str",  # Optional. Dataset.
+                        "evaluation": "str",  # Optional. Evaluation.
+                        "inferenceService": "str",  # Optional. Inferenceservice.
+                        "model": "str"  # Optional. Model.
+                    },
+                    "arguments": [
+                        {
+                            "keyword": "str",  # The 'keyword' of the corresponding
+                              ModelParameter. Required.
+                            "value": "str"  # The value of of the argument. Always a
+                              string; implementations are responsible for parsing. Required.
+                        }
+                    ],
+                    "inputs": [
+                        {
+                            "entity": "str",  # The ID of the entity whose data should be
+                              made available as 'keyword'. Required.
+                            "keyword": "str"  # The 'keyword' specified for this input in
+                              the MethodSpec. Required.
+                        }
+                    ],
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "id": "str",  # Unique identifier of the entity. Required.
+                    "level": "str",  # Measurement level. Required. Known values are: "Dataset"
+                      and "Instance".
+                    "method": {
+                        "account": "str",  # Account that owns the entity. Required.
+                        "id": "str",  # Unique identifier of the entity. Required.
+                        "implementation": {
+                            "kind": "str",  # The kind of implementation. Required.
+                            "jupyterNotebook": {
+                                "notebookModule": "str",  # ID of the Module that
+                                  contains the notebook file. This does *not* add the Module as a
+                                  dependency; you must do that separately. Required.
+                                "notebookPath": "str"  # Path to the notebook file
+                                  relative to the Module root directory. Required.
+                            },
+                            "pythonFunction": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python function to call. Required.
+                            },
+                            "pythonRubric": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python Rubric to run. Required.
+                            }
+                        },
+                        "name": "str",  # Descriptive name of the Method. Required.
+                        "output": {
+                            "kind": "str",  # The kind of output artifact. Required.
+                              Known values are: "Measurement" and "SafetyCase".
+                            "measurement": {
+                                "level": "str",  # Measurement level. Required. Known
+                                  values are: "Dataset" and "Instance".
+                                "name": "str",  # Descriptive name of the
+                                  Measurement. Required.
+                                "schema": {
+                                    "arrowSchema": "str",  # The schema in Arrow
+                                      format, encoded with dyff.schema.arrow.encode_schema(). This is
+                                      required, but can be populated from a DyffDataSchema. Required.
+                                    "dyffSchema": {
+                                        "components": [
+                                            "str"  # A list of named dyff
+                                              data schemas. The final schema is the composition of
+                                              these component schemas. Required.
+                                        ],
+                                        "schemaVersion": "0.1"  # Optional.
+                                          Default value is "0.1". The dyff schema version. "0.1"
+                                    },
+                                    "jsonSchema": {}  # Optional. The schema in
+                                      JSON Schema format.
+                                },
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            },
+                            "safetyCase": {
+                                "name": "str",  # Descriptive name of the SafetyCase.
+                                  Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        },
+                        "scope": "str",  # The scope of the Method. The Method produces
+                          outputs that are specific to one entity of the type specified in the .scope
+                          field. Required. Known values are: "InferenceService" and "Evaluation".
+                        "description": "str",  # Optional. Long-form description, interpreted
+                          as Markdown.
+                        "inputs": [
+                            {
+                                "keyword": "str",  # The input is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "kind": "str",  # The kind of input artifact.
+                                  Required. Known values are: "Dataset", "Evaluation", "Measurement",
+                                  and "Report".
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ],
+                        "modules": [
+                            "str"  # Optional. Modules to load into the analysis
+                              environment.
+                        ],
+                        "parameters": [
+                            {
+                                "keyword": "str",  # The parameter is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ]
+                    },
+                    "name": "str",  # Descriptive name of the Measurement. Required.
+                    "schema": {
+                        "arrowSchema": "str",  # The schema in Arrow format, encoded with
+                          dyff.schema.arrow.encode_schema(). This is required, but can be populated
+                          from a DyffDataSchema. Required.
+                        "dyffSchema": {
+                            "components": [
+                                "str"  # A list of named dyff data schemas. The final
+                                  schema is the composition of these component schemas. Required.
+                            ],
+                            "schemaVersion": "0.1"  # Optional. Default value is "0.1".
+                              The dyff schema version. "0.1"
+                        },
+                        "jsonSchema": {}  # Optional. The schema in JSON Schema format.
+                    },
+                    "scope": {
+                        "dataset": "str",  # Optional. Dataset.
+                        "evaluation": "str",  # Optional. Evaluation.
+                        "inferenceService": "str",  # Optional. Inferenceservice.
+                        "model": "str"  # Optional. Model.
+                    },
+                    "annotations": [
+                        {
+                            "key": "str",  # The annotation key. A DNS label with an
+                              optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                              Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
+                              See
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                              for detailed naming rules. Required.
+                            "value": "str"  # The annotation value. An arbitrary string.
+                              Required.
+                        }
+                    ],
+                    "arguments": [
+                        {
+                            "keyword": "str",  # The 'keyword' of the corresponding
+                              ModelParameter. Required.
+                            "value": "str"  # The value of of the argument. Always a
+                              string; implementations are responsible for parsing. Required.
+                        }
+                    ],
+                    "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
+                      (assigned by system).
+                    "description": "str",  # Optional. Long-form description, interpreted as
+                      Markdown.
+                    "inputs": [
+                        {
+                            "entity": "str",  # The ID of the entity whose data should be
+                              made available as 'keyword'. Required.
+                            "keyword": "str"  # The 'keyword' specified for this input in
+                              the MethodSpec. Required.
+                        }
+                    ],
+                    "kind": "Measurement",  # Optional. Default value is "Measurement". Kind.
+                      "Measurement"
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    },
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop(
+            "content_type", _headers.pop("Content-Type", None)
+        )
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        _request = build_measurements_create_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @distributed_trace_async
+    async def get(self, measurement_id: str, **kwargs: Any) -> JSON:
+        # pylint: disable=line-too-long
+        """Get a Measurement by its key.
+
+        Get a Measurement by its key. Raises a 404 error if no entity exists with that key.
+
+        :param measurement_id: Required.
+        :type measurement_id: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "id": "str",  # Unique identifier of the entity. Required.
+                    "level": "str",  # Measurement level. Required. Known values are: "Dataset"
+                      and "Instance".
+                    "method": {
+                        "account": "str",  # Account that owns the entity. Required.
+                        "id": "str",  # Unique identifier of the entity. Required.
+                        "implementation": {
+                            "kind": "str",  # The kind of implementation. Required.
+                            "jupyterNotebook": {
+                                "notebookModule": "str",  # ID of the Module that
+                                  contains the notebook file. This does *not* add the Module as a
+                                  dependency; you must do that separately. Required.
+                                "notebookPath": "str"  # Path to the notebook file
+                                  relative to the Module root directory. Required.
+                            },
+                            "pythonFunction": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python function to call. Required.
+                            },
+                            "pythonRubric": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python Rubric to run. Required.
+                            }
+                        },
+                        "name": "str",  # Descriptive name of the Method. Required.
+                        "output": {
+                            "kind": "str",  # The kind of output artifact. Required.
+                              Known values are: "Measurement" and "SafetyCase".
+                            "measurement": {
+                                "level": "str",  # Measurement level. Required. Known
+                                  values are: "Dataset" and "Instance".
+                                "name": "str",  # Descriptive name of the
+                                  Measurement. Required.
+                                "schema": {
+                                    "arrowSchema": "str",  # The schema in Arrow
+                                      format, encoded with dyff.schema.arrow.encode_schema(). This is
+                                      required, but can be populated from a DyffDataSchema. Required.
+                                    "dyffSchema": {
+                                        "components": [
+                                            "str"  # A list of named dyff
+                                              data schemas. The final schema is the composition of
+                                              these component schemas. Required.
+                                        ],
+                                        "schemaVersion": "0.1"  # Optional.
+                                          Default value is "0.1". The dyff schema version. "0.1"
+                                    },
+                                    "jsonSchema": {}  # Optional. The schema in
+                                      JSON Schema format.
+                                },
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            },
+                            "safetyCase": {
+                                "name": "str",  # Descriptive name of the SafetyCase.
+                                  Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        },
+                        "scope": "str",  # The scope of the Method. The Method produces
+                          outputs that are specific to one entity of the type specified in the .scope
+                          field. Required. Known values are: "InferenceService" and "Evaluation".
+                        "description": "str",  # Optional. Long-form description, interpreted
+                          as Markdown.
+                        "inputs": [
+                            {
+                                "keyword": "str",  # The input is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "kind": "str",  # The kind of input artifact.
+                                  Required. Known values are: "Dataset", "Evaluation", "Measurement",
+                                  and "Report".
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ],
+                        "modules": [
+                            "str"  # Optional. Modules to load into the analysis
+                              environment.
+                        ],
+                        "parameters": [
+                            {
+                                "keyword": "str",  # The parameter is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ]
+                    },
+                    "name": "str",  # Descriptive name of the Measurement. Required.
+                    "schema": {
+                        "arrowSchema": "str",  # The schema in Arrow format, encoded with
+                          dyff.schema.arrow.encode_schema(). This is required, but can be populated
+                          from a DyffDataSchema. Required.
+                        "dyffSchema": {
+                            "components": [
+                                "str"  # A list of named dyff data schemas. The final
+                                  schema is the composition of these component schemas. Required.
+                            ],
+                            "schemaVersion": "0.1"  # Optional. Default value is "0.1".
+                              The dyff schema version. "0.1"
+                        },
+                        "jsonSchema": {}  # Optional. The schema in JSON Schema format.
+                    },
+                    "scope": {
+                        "dataset": "str",  # Optional. Dataset.
+                        "evaluation": "str",  # Optional. Evaluation.
+                        "inferenceService": "str",  # Optional. Inferenceservice.
+                        "model": "str"  # Optional. Model.
+                    },
+                    "annotations": [
+                        {
+                            "key": "str",  # The annotation key. A DNS label with an
+                              optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                              Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
+                              See
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                              for detailed naming rules. Required.
+                            "value": "str"  # The annotation value. An arbitrary string.
+                              Required.
+                        }
+                    ],
+                    "arguments": [
+                        {
+                            "keyword": "str",  # The 'keyword' of the corresponding
+                              ModelParameter. Required.
+                            "value": "str"  # The value of of the argument. Always a
+                              string; implementations are responsible for parsing. Required.
+                        }
+                    ],
+                    "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
+                      (assigned by system).
+                    "description": "str",  # Optional. Long-form description, interpreted as
+                      Markdown.
+                    "inputs": [
+                        {
+                            "entity": "str",  # The ID of the entity whose data should be
+                              made available as 'keyword'. Required.
+                            "keyword": "str"  # The 'keyword' specified for this input in
+                              the MethodSpec. Required.
+                        }
+                    ],
+                    "kind": "Measurement",  # Optional. Default value is "Measurement". Kind.
+                      "Measurement"
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    },
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        _request = build_measurements_get_request(
+            measurement_id=measurement_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @distributed_trace_async
+    async def delete(self, measurement_id: str, **kwargs: Any) -> JSON:
+        """Mark a Measurement for deletion.
+
+        Mark a Measurement for deletion.
+
+        :param measurement_id: Required.
+        :type measurement_id: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        _request = build_measurements_delete_request(
+            measurement_id=measurement_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+
+class MethodsOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~_generated.aio.DyffV0API`'s
+        :attr:`methods` attribute.
+    """
+
+    def __init__(self, *args, **kwargs) -> None:
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = (
+            input_args.pop(0) if input_args else kwargs.pop("deserializer")
+        )
+
+    @overload
+    async def label(
+        self,
+        method_id: str,
+        body: JSON,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> Union[Any, JSON]:
+        # pylint: disable=line-too-long
+        """Update labels for an existing Method.
+
+        Update labels for an existing Method.
+
+        :param method_id: Required.
+        :type method_id: str
+        :param body: Required.
+        :type body: JSON
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: any or JSON object
+        :rtype: any or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    }
+                }
+
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @overload
+    async def label(
+        self,
+        method_id: str,
+        body: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> Union[Any, JSON]:
+        """Update labels for an existing Method.
+
+        Update labels for an existing Method.
+
+        :param method_id: Required.
+        :type method_id: str
+        :param body: Required.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: any or JSON object
+        :rtype: any or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @distributed_trace_async
+    async def label(
+        self, method_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any
+    ) -> Union[Any, JSON]:
+        # pylint: disable=line-too-long
+        """Update labels for an existing Method.
+
+        Update labels for an existing Method.
+
+        :param method_id: Required.
+        :type method_id: str
+        :param body: Is either a JSON type or a IO[bytes] type. Required.
+        :type body: JSON or IO[bytes]
+        :return: any or JSON object
+        :rtype: any or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    }
+                }
+
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop(
+            "content_type", _headers.pop("Content-Type", None)
+        )
+        cls: ClsType[Union[Any, JSON]] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        _request = build_methods_label_request(
+            method_id=method_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(Union[Any, JSON], deserialized), {})  # type: ignore
+
+        return cast(Union[Any, JSON], deserialized)  # type: ignore
+
+    @distributed_trace_async
+    async def query(
+        self,
+        *,
+        id: Optional[str] = None,
+        account: Optional[str] = None,
+        status: Optional[str] = None,
+        reason: Optional[str] = None,
+        labels: Optional[str] = None,
+        name: Optional[str] = None,
+        output_kind: Optional[str] = None,
+        **kwargs: Any,
+    ) -> Union[List[JSON], JSON]:
+        # pylint: disable=line-too-long
+        """Get all Methods matching a query.
+
+        Get all Methods matching a query. The query is a set of equality
+        constraints specified as key-value pairs.
+
+        :keyword id: Default value is None.
+        :paramtype id: str
+        :keyword account: Default value is None.
+        :paramtype account: str
+        :keyword status: Default value is None.
+        :paramtype status: str
+        :keyword reason: Default value is None.
+        :paramtype reason: str
+        :keyword labels: Default value is None.
+        :paramtype labels: str
+        :keyword name: Default value is None.
+        :paramtype name: str
+        :keyword output_kind: Default value is None.
+        :paramtype output_kind: str
+        :return: list of JSON object or JSON object
+        :rtype: list[JSON] or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == [
+                    {
+                        "account": "str",  # Account that owns the entity. Required.
+                        "id": "str",  # Unique identifier of the entity. Required.
+                        "implementation": {
+                            "kind": "str",  # The kind of implementation. Required.
+                            "jupyterNotebook": {
+                                "notebookModule": "str",  # ID of the Module that
+                                  contains the notebook file. This does *not* add the Module as a
+                                  dependency; you must do that separately. Required.
+                                "notebookPath": "str"  # Path to the notebook file
+                                  relative to the Module root directory. Required.
+                            },
+                            "pythonFunction": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python function to call. Required.
+                            },
+                            "pythonRubric": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python Rubric to run. Required.
+                            }
+                        },
+                        "name": "str",  # Descriptive name of the Method. Required.
+                        "output": {
+                            "kind": "str",  # The kind of output artifact. Required.
+                              Known values are: "Measurement" and "SafetyCase".
+                            "measurement": {
+                                "level": "str",  # Measurement level. Required. Known
+                                  values are: "Dataset" and "Instance".
+                                "name": "str",  # Descriptive name of the
+                                  Measurement. Required.
+                                "schema": {
+                                    "arrowSchema": "str",  # The schema in Arrow
+                                      format, encoded with dyff.schema.arrow.encode_schema(). This is
+                                      required, but can be populated from a DyffDataSchema. Required.
+                                    "dyffSchema": {
+                                        "components": [
+                                            "str"  # A list of named dyff
+                                              data schemas. The final schema is the composition of
+                                              these component schemas. Required.
+                                        ],
+                                        "schemaVersion": "0.1"  # Optional.
+                                          Default value is "0.1". The dyff schema version. "0.1"
+                                    },
+                                    "jsonSchema": {}  # Optional. The schema in
+                                      JSON Schema format.
+                                },
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            },
+                            "safetyCase": {
+                                "name": "str",  # Descriptive name of the SafetyCase.
+                                  Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        },
+                        "scope": "str",  # The scope of the Method. The Method produces
+                          outputs that are specific to one entity of the type specified in the .scope
+                          field. Required. Known values are: "InferenceService" and "Evaluation".
+                        "annotations": [
+                            {
+                                "key": "str",  # The annotation key. A DNS label with
+                                  an optional DNS domain prefix. For example: 'my-key',
+                                  'your.com/key_0'. Names prefixed with 'dyff.io/',
+                                  'subdomain.dyff.io/', etc. are reserved.  See
+                                  https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                                  for detailed naming rules. Required.
+                                "value": "str"  # The annotation value. An arbitrary
+                                  string. Required.
+                            }
+                        ],
+                        "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation
+                          time (assigned by system).
+                        "description": "str",  # Optional. Long-form description, interpreted
+                          as Markdown.
+                        "inputs": [
+                            {
+                                "keyword": "str",  # The input is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "kind": "str",  # The kind of input artifact.
+                                  Required. Known values are: "Dataset", "Evaluation", "Measurement",
+                                  and "Report".
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ],
+                        "kind": "Method",  # Optional. Default value is "Method". Kind.
+                          "Method"
+                        "labels": {
+                            "str": "str"  # Optional. A set of key-value labels for the
+                              resource. Used to specify identifying attributes of resources that are
+                              meaningful to users but do not imply semantics in the dyff system.  The
+                              keys are DNS labels with an optional DNS domain prefix. For example:
+                              'my-key', 'your.com/key_0'. Keys prefixed with 'dyff.io/',
+                              'subdomain.dyff.io/', etc. are reserved.  The label values are
+                              alphanumeric characters separated by '.', '-', or '_'.  We follow the
+                              kubernetes label conventions closely. See:
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                        },
+                        "modules": [
+                            "str"  # Optional. Modules to load into the analysis
+                              environment.
+                        ],
+                        "parameters": [
+                            {
+                                "keyword": "str",  # The parameter is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ],
+                        "reason": "str",  # Optional. Reason for current status (assigned by
+                          system).
+                        "schemaVersion": "0.1",  # Optional. Default value is "0.1". The
+                          schema version. "0.1"
+                        "status": "str"  # Optional. Top-level resource status (assigned by
+                          system).
+                    }
+                ]
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
+
+        _request = build_methods_query_request(
+            id=id,
+            account=account,
+            status=status,
+            reason=reason,
+            labels=labels,
+            name=name,
+            output_kind=output_kind,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(Union[List[JSON], JSON], deserialized), {})  # type: ignore
+
+        return cast(Union[List[JSON], JSON], deserialized)  # type: ignore
+
+    @overload
+    async def create(
+        self, body: JSON, *, content_type: str = "application/json", **kwargs: Any
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Create a Method.
+
+        Create a Method.
+
+        :param body: Required.
+        :type body: JSON
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "implementation": {
+                        "kind": "str",  # The kind of implementation. Required.
+                        "jupyterNotebook": {
+                            "notebookModule": "str",  # ID of the Module that contains
+                              the notebook file. This does *not* add the Module as a dependency; you
+                              must do that separately. Required.
+                            "notebookPath": "str"  # Path to the notebook file relative
+                              to the Module root directory. Required.
+                        },
+                        "pythonFunction": {
+                            "fullyQualifiedName": "str"  # The fully-qualified name of
+                              the Python function to call. Required.
+                        },
+                        "pythonRubric": {
+                            "fullyQualifiedName": "str"  # The fully-qualified name of
+                              the Python Rubric to run. Required.
+                        }
+                    },
+                    "name": "str",  # Descriptive name of the Method. Required.
+                    "output": {
+                        "kind": "str",  # The kind of output artifact. Required. Known values
+                          are: "Measurement" and "SafetyCase".
+                        "measurement": {
+                            "level": "str",  # Measurement level. Required. Known values
+                              are: "Dataset" and "Instance".
+                            "name": "str",  # Descriptive name of the Measurement.
+                              Required.
+                            "schema": {
+                                "arrowSchema": "str",  # The schema in Arrow format,
+                                  encoded with dyff.schema.arrow.encode_schema(). This is required, but
+                                  can be populated from a DyffDataSchema. Required.
+                                "dyffSchema": {
+                                    "components": [
+                                        "str"  # A list of named dyff data
+                                          schemas. The final schema is the composition of these
+                                          component schemas. Required.
+                                    ],
+                                    "schemaVersion": "0.1"  # Optional. Default
+                                      value is "0.1". The dyff schema version. "0.1"
+                                },
+                                "jsonSchema": {}  # Optional. The schema in JSON
+                                  Schema format.
+                            },
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        },
+                        "safetyCase": {
+                            "name": "str",  # Descriptive name of the SafetyCase.
+                              Required.
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    },
+                    "scope": "str",  # The scope of the Method. The Method produces outputs that
+                      are specific to one entity of the type specified in the .scope field. Required.
+                      Known values are: "InferenceService" and "Evaluation".
+                    "description": "str",  # Optional. Long-form description, interpreted as
+                      Markdown.
+                    "inputs": [
+                        {
+                            "keyword": "str",  # The input is referred to by 'keyword' in
+                              the context of the method implementation. Required.
+                            "kind": "str",  # The kind of input artifact. Required. Known
+                              values are: "Dataset", "Evaluation", "Measurement", and "Report".
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    ],
+                    "modules": [
+                        "str"  # Optional. Modules to load into the analysis environment.
+                    ],
+                    "parameters": [
+                        {
+                            "keyword": "str",  # The parameter is referred to by
+                              'keyword' in the context of the method implementation. Required.
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    ],
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "id": "str",  # Unique identifier of the entity. Required.
+                    "implementation": {
+                        "kind": "str",  # The kind of implementation. Required.
+                        "jupyterNotebook": {
+                            "notebookModule": "str",  # ID of the Module that contains
+                              the notebook file. This does *not* add the Module as a dependency; you
+                              must do that separately. Required.
+                            "notebookPath": "str"  # Path to the notebook file relative
+                              to the Module root directory. Required.
+                        },
+                        "pythonFunction": {
+                            "fullyQualifiedName": "str"  # The fully-qualified name of
+                              the Python function to call. Required.
+                        },
+                        "pythonRubric": {
+                            "fullyQualifiedName": "str"  # The fully-qualified name of
+                              the Python Rubric to run. Required.
+                        }
+                    },
+                    "name": "str",  # Descriptive name of the Method. Required.
+                    "output": {
+                        "kind": "str",  # The kind of output artifact. Required. Known values
+                          are: "Measurement" and "SafetyCase".
+                        "measurement": {
+                            "level": "str",  # Measurement level. Required. Known values
+                              are: "Dataset" and "Instance".
+                            "name": "str",  # Descriptive name of the Measurement.
+                              Required.
+                            "schema": {
+                                "arrowSchema": "str",  # The schema in Arrow format,
+                                  encoded with dyff.schema.arrow.encode_schema(). This is required, but
+                                  can be populated from a DyffDataSchema. Required.
+                                "dyffSchema": {
+                                    "components": [
+                                        "str"  # A list of named dyff data
+                                          schemas. The final schema is the composition of these
+                                          component schemas. Required.
+                                    ],
+                                    "schemaVersion": "0.1"  # Optional. Default
+                                      value is "0.1". The dyff schema version. "0.1"
+                                },
+                                "jsonSchema": {}  # Optional. The schema in JSON
+                                  Schema format.
+                            },
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        },
+                        "safetyCase": {
+                            "name": "str",  # Descriptive name of the SafetyCase.
+                              Required.
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    },
+                    "scope": "str",  # The scope of the Method. The Method produces outputs that
+                      are specific to one entity of the type specified in the .scope field. Required.
+                      Known values are: "InferenceService" and "Evaluation".
+                    "annotations": [
+                        {
+                            "key": "str",  # The annotation key. A DNS label with an
+                              optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                              Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
+                              See
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                              for detailed naming rules. Required.
+                            "value": "str"  # The annotation value. An arbitrary string.
+                              Required.
+                        }
+                    ],
+                    "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
+                      (assigned by system).
+                    "description": "str",  # Optional. Long-form description, interpreted as
+                      Markdown.
+                    "inputs": [
+                        {
+                            "keyword": "str",  # The input is referred to by 'keyword' in
+                              the context of the method implementation. Required.
+                            "kind": "str",  # The kind of input artifact. Required. Known
+                              values are: "Dataset", "Evaluation", "Measurement", and "Report".
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    ],
+                    "kind": "Method",  # Optional. Default value is "Method". Kind. "Method"
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    },
+                    "modules": [
+                        "str"  # Optional. Modules to load into the analysis environment.
+                    ],
+                    "parameters": [
+                        {
+                            "keyword": "str",  # The parameter is referred to by
+                              'keyword' in the context of the method implementation. Required.
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    ],
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @overload
+    async def create(
+        self, body: IO[bytes], *, content_type: str = "application/json", **kwargs: Any
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Create a Method.
+
+        Create a Method.
+
+        :param body: Required.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "id": "str",  # Unique identifier of the entity. Required.
+                    "implementation": {
+                        "kind": "str",  # The kind of implementation. Required.
+                        "jupyterNotebook": {
+                            "notebookModule": "str",  # ID of the Module that contains
+                              the notebook file. This does *not* add the Module as a dependency; you
+                              must do that separately. Required.
+                            "notebookPath": "str"  # Path to the notebook file relative
+                              to the Module root directory. Required.
+                        },
+                        "pythonFunction": {
+                            "fullyQualifiedName": "str"  # The fully-qualified name of
+                              the Python function to call. Required.
+                        },
+                        "pythonRubric": {
+                            "fullyQualifiedName": "str"  # The fully-qualified name of
+                              the Python Rubric to run. Required.
+                        }
+                    },
+                    "name": "str",  # Descriptive name of the Method. Required.
+                    "output": {
+                        "kind": "str",  # The kind of output artifact. Required. Known values
+                          are: "Measurement" and "SafetyCase".
+                        "measurement": {
+                            "level": "str",  # Measurement level. Required. Known values
+                              are: "Dataset" and "Instance".
+                            "name": "str",  # Descriptive name of the Measurement.
+                              Required.
+                            "schema": {
+                                "arrowSchema": "str",  # The schema in Arrow format,
+                                  encoded with dyff.schema.arrow.encode_schema(). This is required, but
+                                  can be populated from a DyffDataSchema. Required.
+                                "dyffSchema": {
+                                    "components": [
+                                        "str"  # A list of named dyff data
+                                          schemas. The final schema is the composition of these
+                                          component schemas. Required.
+                                    ],
+                                    "schemaVersion": "0.1"  # Optional. Default
+                                      value is "0.1". The dyff schema version. "0.1"
+                                },
+                                "jsonSchema": {}  # Optional. The schema in JSON
+                                  Schema format.
+                            },
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        },
+                        "safetyCase": {
+                            "name": "str",  # Descriptive name of the SafetyCase.
+                              Required.
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    },
+                    "scope": "str",  # The scope of the Method. The Method produces outputs that
+                      are specific to one entity of the type specified in the .scope field. Required.
+                      Known values are: "InferenceService" and "Evaluation".
+                    "annotations": [
+                        {
+                            "key": "str",  # The annotation key. A DNS label with an
+                              optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                              Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
+                              See
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                              for detailed naming rules. Required.
+                            "value": "str"  # The annotation value. An arbitrary string.
+                              Required.
+                        }
+                    ],
+                    "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
+                      (assigned by system).
+                    "description": "str",  # Optional. Long-form description, interpreted as
+                      Markdown.
+                    "inputs": [
+                        {
+                            "keyword": "str",  # The input is referred to by 'keyword' in
+                              the context of the method implementation. Required.
+                            "kind": "str",  # The kind of input artifact. Required. Known
+                              values are: "Dataset", "Evaluation", "Measurement", and "Report".
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    ],
+                    "kind": "Method",  # Optional. Default value is "Method". Kind. "Method"
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    },
+                    "modules": [
+                        "str"  # Optional. Modules to load into the analysis environment.
+                    ],
+                    "parameters": [
+                        {
+                            "keyword": "str",  # The parameter is referred to by
+                              'keyword' in the context of the method implementation. Required.
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    ],
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @distributed_trace_async
+    async def create(self, body: Union[JSON, IO[bytes]], **kwargs: Any) -> JSON:
+        # pylint: disable=line-too-long
+        """Create a Method.
+
+        Create a Method.
+
+        :param body: Is either a JSON type or a IO[bytes] type. Required.
+        :type body: JSON or IO[bytes]
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "implementation": {
+                        "kind": "str",  # The kind of implementation. Required.
+                        "jupyterNotebook": {
+                            "notebookModule": "str",  # ID of the Module that contains
+                              the notebook file. This does *not* add the Module as a dependency; you
+                              must do that separately. Required.
+                            "notebookPath": "str"  # Path to the notebook file relative
+                              to the Module root directory. Required.
+                        },
+                        "pythonFunction": {
+                            "fullyQualifiedName": "str"  # The fully-qualified name of
+                              the Python function to call. Required.
+                        },
+                        "pythonRubric": {
+                            "fullyQualifiedName": "str"  # The fully-qualified name of
+                              the Python Rubric to run. Required.
+                        }
+                    },
+                    "name": "str",  # Descriptive name of the Method. Required.
+                    "output": {
+                        "kind": "str",  # The kind of output artifact. Required. Known values
+                          are: "Measurement" and "SafetyCase".
+                        "measurement": {
+                            "level": "str",  # Measurement level. Required. Known values
+                              are: "Dataset" and "Instance".
+                            "name": "str",  # Descriptive name of the Measurement.
+                              Required.
+                            "schema": {
+                                "arrowSchema": "str",  # The schema in Arrow format,
+                                  encoded with dyff.schema.arrow.encode_schema(). This is required, but
+                                  can be populated from a DyffDataSchema. Required.
+                                "dyffSchema": {
+                                    "components": [
+                                        "str"  # A list of named dyff data
+                                          schemas. The final schema is the composition of these
+                                          component schemas. Required.
+                                    ],
+                                    "schemaVersion": "0.1"  # Optional. Default
+                                      value is "0.1". The dyff schema version. "0.1"
+                                },
+                                "jsonSchema": {}  # Optional. The schema in JSON
+                                  Schema format.
+                            },
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        },
+                        "safetyCase": {
+                            "name": "str",  # Descriptive name of the SafetyCase.
+                              Required.
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    },
+                    "scope": "str",  # The scope of the Method. The Method produces outputs that
+                      are specific to one entity of the type specified in the .scope field. Required.
+                      Known values are: "InferenceService" and "Evaluation".
+                    "description": "str",  # Optional. Long-form description, interpreted as
+                      Markdown.
+                    "inputs": [
+                        {
+                            "keyword": "str",  # The input is referred to by 'keyword' in
+                              the context of the method implementation. Required.
+                            "kind": "str",  # The kind of input artifact. Required. Known
+                              values are: "Dataset", "Evaluation", "Measurement", and "Report".
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    ],
+                    "modules": [
+                        "str"  # Optional. Modules to load into the analysis environment.
+                    ],
+                    "parameters": [
+                        {
+                            "keyword": "str",  # The parameter is referred to by
+                              'keyword' in the context of the method implementation. Required.
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    ],
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "id": "str",  # Unique identifier of the entity. Required.
+                    "implementation": {
+                        "kind": "str",  # The kind of implementation. Required.
+                        "jupyterNotebook": {
+                            "notebookModule": "str",  # ID of the Module that contains
+                              the notebook file. This does *not* add the Module as a dependency; you
+                              must do that separately. Required.
+                            "notebookPath": "str"  # Path to the notebook file relative
+                              to the Module root directory. Required.
+                        },
+                        "pythonFunction": {
+                            "fullyQualifiedName": "str"  # The fully-qualified name of
+                              the Python function to call. Required.
+                        },
+                        "pythonRubric": {
+                            "fullyQualifiedName": "str"  # The fully-qualified name of
+                              the Python Rubric to run. Required.
+                        }
+                    },
+                    "name": "str",  # Descriptive name of the Method. Required.
+                    "output": {
+                        "kind": "str",  # The kind of output artifact. Required. Known values
+                          are: "Measurement" and "SafetyCase".
+                        "measurement": {
+                            "level": "str",  # Measurement level. Required. Known values
+                              are: "Dataset" and "Instance".
+                            "name": "str",  # Descriptive name of the Measurement.
+                              Required.
+                            "schema": {
+                                "arrowSchema": "str",  # The schema in Arrow format,
+                                  encoded with dyff.schema.arrow.encode_schema(). This is required, but
+                                  can be populated from a DyffDataSchema. Required.
+                                "dyffSchema": {
+                                    "components": [
+                                        "str"  # A list of named dyff data
+                                          schemas. The final schema is the composition of these
+                                          component schemas. Required.
+                                    ],
+                                    "schemaVersion": "0.1"  # Optional. Default
+                                      value is "0.1". The dyff schema version. "0.1"
+                                },
+                                "jsonSchema": {}  # Optional. The schema in JSON
+                                  Schema format.
+                            },
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        },
+                        "safetyCase": {
+                            "name": "str",  # Descriptive name of the SafetyCase.
+                              Required.
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    },
+                    "scope": "str",  # The scope of the Method. The Method produces outputs that
+                      are specific to one entity of the type specified in the .scope field. Required.
+                      Known values are: "InferenceService" and "Evaluation".
+                    "annotations": [
+                        {
+                            "key": "str",  # The annotation key. A DNS label with an
+                              optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                              Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
+                              See
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                              for detailed naming rules. Required.
+                            "value": "str"  # The annotation value. An arbitrary string.
+                              Required.
+                        }
+                    ],
+                    "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
+                      (assigned by system).
+                    "description": "str",  # Optional. Long-form description, interpreted as
+                      Markdown.
+                    "inputs": [
+                        {
+                            "keyword": "str",  # The input is referred to by 'keyword' in
+                              the context of the method implementation. Required.
+                            "kind": "str",  # The kind of input artifact. Required. Known
+                              values are: "Dataset", "Evaluation", "Measurement", and "Report".
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    ],
+                    "kind": "Method",  # Optional. Default value is "Method". Kind. "Method"
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    },
+                    "modules": [
+                        "str"  # Optional. Modules to load into the analysis environment.
+                    ],
+                    "parameters": [
+                        {
+                            "keyword": "str",  # The parameter is referred to by
+                              'keyword' in the context of the method implementation. Required.
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    ],
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop(
+            "content_type", _headers.pop("Content-Type", None)
+        )
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        _request = build_methods_create_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @distributed_trace_async
+    async def get(self, method_id: str, **kwargs: Any) -> JSON:
+        # pylint: disable=line-too-long
+        """Get a Method by its key.
+
+        Get a Method by its key. Raises a 404 error if no entity exists with that key.
+
+        :param method_id: Required.
+        :type method_id: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "id": "str",  # Unique identifier of the entity. Required.
+                    "implementation": {
+                        "kind": "str",  # The kind of implementation. Required.
+                        "jupyterNotebook": {
+                            "notebookModule": "str",  # ID of the Module that contains
+                              the notebook file. This does *not* add the Module as a dependency; you
+                              must do that separately. Required.
+                            "notebookPath": "str"  # Path to the notebook file relative
+                              to the Module root directory. Required.
+                        },
+                        "pythonFunction": {
+                            "fullyQualifiedName": "str"  # The fully-qualified name of
+                              the Python function to call. Required.
+                        },
+                        "pythonRubric": {
+                            "fullyQualifiedName": "str"  # The fully-qualified name of
+                              the Python Rubric to run. Required.
+                        }
+                    },
+                    "name": "str",  # Descriptive name of the Method. Required.
+                    "output": {
+                        "kind": "str",  # The kind of output artifact. Required. Known values
+                          are: "Measurement" and "SafetyCase".
+                        "measurement": {
+                            "level": "str",  # Measurement level. Required. Known values
+                              are: "Dataset" and "Instance".
+                            "name": "str",  # Descriptive name of the Measurement.
+                              Required.
+                            "schema": {
+                                "arrowSchema": "str",  # The schema in Arrow format,
+                                  encoded with dyff.schema.arrow.encode_schema(). This is required, but
+                                  can be populated from a DyffDataSchema. Required.
+                                "dyffSchema": {
+                                    "components": [
+                                        "str"  # A list of named dyff data
+                                          schemas. The final schema is the composition of these
+                                          component schemas. Required.
+                                    ],
+                                    "schemaVersion": "0.1"  # Optional. Default
+                                      value is "0.1". The dyff schema version. "0.1"
+                                },
+                                "jsonSchema": {}  # Optional. The schema in JSON
+                                  Schema format.
+                            },
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        },
+                        "safetyCase": {
+                            "name": "str",  # Descriptive name of the SafetyCase.
+                              Required.
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    },
+                    "scope": "str",  # The scope of the Method. The Method produces outputs that
+                      are specific to one entity of the type specified in the .scope field. Required.
+                      Known values are: "InferenceService" and "Evaluation".
+                    "annotations": [
+                        {
+                            "key": "str",  # The annotation key. A DNS label with an
+                              optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                              Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
+                              See
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                              for detailed naming rules. Required.
+                            "value": "str"  # The annotation value. An arbitrary string.
+                              Required.
+                        }
+                    ],
+                    "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
+                      (assigned by system).
+                    "description": "str",  # Optional. Long-form description, interpreted as
+                      Markdown.
+                    "inputs": [
+                        {
+                            "keyword": "str",  # The input is referred to by 'keyword' in
+                              the context of the method implementation. Required.
+                            "kind": "str",  # The kind of input artifact. Required. Known
+                              values are: "Dataset", "Evaluation", "Measurement", and "Report".
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    ],
+                    "kind": "Method",  # Optional. Default value is "Method". Kind. "Method"
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    },
+                    "modules": [
+                        "str"  # Optional. Modules to load into the analysis environment.
+                    ],
+                    "parameters": [
+                        {
+                            "keyword": "str",  # The parameter is referred to by
+                              'keyword' in the context of the method implementation. Required.
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    ],
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        _request = build_methods_get_request(
+            method_id=method_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @distributed_trace_async
+    async def delete(self, method_id: str, **kwargs: Any) -> JSON:
+        """Mark a Method for deletion.
+
+        Mark a Method for deletion.
+
+        :param method_id: Required.
+        :type method_id: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        _request = build_methods_delete_request(
+            method_id=method_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+
 class ModelsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~_generated.aio.DyffAPI`'s
+        :class:`~_generated.aio.DyffV0API`'s
         :attr:`models` attribute.
     """
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
@@ -8059,15 +11069,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8278,15 +11288,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8857,15 +11867,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9048,15 +12058,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9135,15 +12145,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9196,15 +12206,15 @@
 
 class ModulesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~_generated.aio.DyffAPI`'s
+        :class:`~_generated.aio.DyffV0API`'s
         :attr:`modules` attribute.
     """
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
@@ -9353,15 +12363,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9522,15 +12532,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9851,15 +12861,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9992,15 +13002,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10079,15 +13089,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10172,15 +13182,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10255,15 +13265,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10316,15 +13326,15 @@
 
 class ReportsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~_generated.aio.DyffAPI`'s
+        :class:`~_generated.aio.DyffV0API`'s
         :attr:`reports` attribute.
     """
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
@@ -10473,15 +13483,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10689,14 +13699,18 @@
                               'subdomain.dyff.io/', etc. are reserved.  The label values are
                               alphanumeric characters separated by '.', '-', or '_'.  We follow the
                               kubernetes label conventions closely. See:
                               https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                         },
                         "model": "str",  # Optional. The model backing the inference service,
                           if applicable.
+                        "modules": [
+                            "str"  # Optional. Additional modules to load into the report
+                              environment.
+                        ],
                         "reason": "str",  # Optional. Reason for current status (assigned by
                           system).
                         "schemaVersion": "0.1",  # Optional. Default value is "0.1". The
                           schema version. "0.1"
                         "status": "str"  # Optional. Top-level resource status (assigned by
                           system).
                     }
@@ -10710,15 +13724,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10803,14 +13817,18 @@
                     "account": "str",  # Account that owns the entity. Required.
                     "evaluation": "str",  # The evaluation (and corresponding output data) to run
                       the report on. Required.
                     "rubric": "str",  # The scoring rubric to apply (e.g.,
                       'classification.TopKAccuracy'). Required.
                     "datasetView": {},
                     "evaluationView": {},
+                    "modules": [
+                        "str"  # Optional. Additional modules to load into the report
+                          environment.
+                    ],
                     "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
                       version. "0.1"
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "account": "str",  # Account that owns the entity. Required.
@@ -10903,14 +13921,18 @@
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                     },
                     "model": "str",  # Optional. The model backing the inference service, if
                       applicable.
+                    "modules": [
+                        "str"  # Optional. Additional modules to load into the report
+                          environment.
+                    ],
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
                     "status": "str"  # Optional. Top-level resource status (assigned by system).
                 }
                 # response body for status code(s): 422
                 response == {
@@ -11039,14 +14061,18 @@
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                     },
                     "model": "str",  # Optional. The model backing the inference service, if
                       applicable.
+                    "modules": [
+                        "str"  # Optional. Additional modules to load into the report
+                          environment.
+                    ],
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
                     "status": "str"  # Optional. Top-level resource status (assigned by system).
                 }
                 # response body for status code(s): 422
                 response == {
@@ -11083,14 +14109,18 @@
                     "account": "str",  # Account that owns the entity. Required.
                     "evaluation": "str",  # The evaluation (and corresponding output data) to run
                       the report on. Required.
                     "rubric": "str",  # The scoring rubric to apply (e.g.,
                       'classification.TopKAccuracy'). Required.
                     "datasetView": {},
                     "evaluationView": {},
+                    "modules": [
+                        "str"  # Optional. Additional modules to load into the report
+                          environment.
+                    ],
                     "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
                       version. "0.1"
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "account": "str",  # Account that owns the entity. Required.
@@ -11183,14 +14213,18 @@
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                     },
                     "model": "str",  # Optional. The model backing the inference service, if
                       applicable.
+                    "modules": [
+                        "str"  # Optional. Additional modules to load into the report
+                          environment.
+                    ],
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
                     "status": "str"  # Optional. Top-level resource status (assigned by system).
                 }
                 # response body for status code(s): 422
                 response == {
@@ -11201,15 +14235,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11380,14 +14414,18 @@
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                     },
                     "model": "str",  # Optional. The model backing the inference service, if
                       applicable.
+                    "modules": [
+                        "str"  # Optional. Additional modules to load into the report
+                          environment.
+                    ],
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
                     "status": "str"  # Optional. Top-level resource status (assigned by system).
                 }
                 # response body for status code(s): 422
                 response == {
@@ -11398,15 +14436,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11485,15 +14523,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11549,15 +14587,15 @@
     ) -> Union[AsyncIterator[bytes], JSON]:
         """Get the raw data for the Report.
 
         Get the raw data for the Report.
 
         :param report_id: Required.
         :type report_id: str
-        :return: Async iterator of the response bytes or JSON object or None
+        :return: AsyncIterator[bytes] or JSON object or None
         :rtype: AsyncIterator[bytes] or JSON or None
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 422
@@ -11569,15 +14607,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11617,7 +14655,1493 @@
         if response.status_code == 422:
             deserialized = response.iter_bytes()
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
+
+
+class SafetycasesOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~_generated.aio.DyffV0API`'s
+        :attr:`safetycases` attribute.
+    """
+
+    def __init__(self, *args, **kwargs) -> None:
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = (
+            input_args.pop(0) if input_args else kwargs.pop("deserializer")
+        )
+
+    @overload
+    async def label(
+        self,
+        safetycase_id: str,
+        body: JSON,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> Union[Any, JSON]:
+        # pylint: disable=line-too-long
+        """Update labels for an existing SafetyCase.
+
+        Update labels for an existing SafetyCase.
+
+        :param safetycase_id: Required.
+        :type safetycase_id: str
+        :param body: Required.
+        :type body: JSON
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: any or JSON object
+        :rtype: any or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    }
+                }
+
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @overload
+    async def label(
+        self,
+        safetycase_id: str,
+        body: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> Union[Any, JSON]:
+        """Update labels for an existing SafetyCase.
+
+        Update labels for an existing SafetyCase.
+
+        :param safetycase_id: Required.
+        :type safetycase_id: str
+        :param body: Required.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: any or JSON object
+        :rtype: any or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @distributed_trace_async
+    async def label(
+        self, safetycase_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any
+    ) -> Union[Any, JSON]:
+        # pylint: disable=line-too-long
+        """Update labels for an existing SafetyCase.
+
+        Update labels for an existing SafetyCase.
+
+        :param safetycase_id: Required.
+        :type safetycase_id: str
+        :param body: Is either a JSON type or a IO[bytes] type. Required.
+        :type body: JSON or IO[bytes]
+        :return: any or JSON object
+        :rtype: any or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    }
+                }
+
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop(
+            "content_type", _headers.pop("Content-Type", None)
+        )
+        cls: ClsType[Union[Any, JSON]] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        _request = build_safetycases_label_request(
+            safetycase_id=safetycase_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(Union[Any, JSON], deserialized), {})  # type: ignore
+
+        return cast(Union[Any, JSON], deserialized)  # type: ignore
+
+    @distributed_trace_async
+    async def query(
+        self,
+        *,
+        id: Optional[str] = None,
+        account: Optional[str] = None,
+        status: Optional[str] = None,
+        reason: Optional[str] = None,
+        labels: Optional[str] = None,
+        analysis: Optional[str] = None,
+        method: Optional[str] = None,
+        method_name: Optional[str] = None,
+        inputs_any_of: Optional[str] = None,
+        **kwargs: Any,
+    ) -> Union[List[JSON], JSON]:
+        # pylint: disable=line-too-long
+        """Get all SafetyCase entities matching a query.
+
+        Get all SafetyCase entities matching a query. The query is a set of equality
+        constraints specified as key-value pairs.
+
+        :keyword id: Default value is None.
+        :paramtype id: str
+        :keyword account: Default value is None.
+        :paramtype account: str
+        :keyword status: Default value is None.
+        :paramtype status: str
+        :keyword reason: Default value is None.
+        :paramtype reason: str
+        :keyword labels: Default value is None.
+        :paramtype labels: str
+        :keyword analysis: Default value is None.
+        :paramtype analysis: str
+        :keyword method: Default value is None.
+        :paramtype method: str
+        :keyword method_name: Default value is None.
+        :paramtype method_name: str
+        :keyword inputs_any_of: Default value is None.
+        :paramtype inputs_any_of: str
+        :return: list of JSON object or JSON object
+        :rtype: list[JSON] or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == [
+                    {
+                        "account": "str",  # Account that owns the entity. Required.
+                        "id": "str",  # Unique identifier of the entity. Required.
+                        "method": {
+                            "account": "str",  # Account that owns the entity. Required.
+                            "id": "str",  # Unique identifier of the entity. Required.
+                            "implementation": {
+                                "kind": "str",  # The kind of implementation.
+                                  Required.
+                                "jupyterNotebook": {
+                                    "notebookModule": "str",  # ID of the Module
+                                      that contains the notebook file. This does *not* add the Module
+                                      as a dependency; you must do that separately. Required.
+                                    "notebookPath": "str"  # Path to the notebook
+                                      file relative to the Module root directory. Required.
+                                },
+                                "pythonFunction": {
+                                    "fullyQualifiedName": "str"  # The
+                                      fully-qualified name of the Python function to call. Required.
+                                },
+                                "pythonRubric": {
+                                    "fullyQualifiedName": "str"  # The
+                                      fully-qualified name of the Python Rubric to run. Required.
+                                }
+                            },
+                            "name": "str",  # Descriptive name of the Method. Required.
+                            "output": {
+                                "kind": "str",  # The kind of output artifact.
+                                  Required. Known values are: "Measurement" and "SafetyCase".
+                                "measurement": {
+                                    "level": "str",  # Measurement level.
+                                      Required. Known values are: "Dataset" and "Instance".
+                                    "name": "str",  # Descriptive name of the
+                                      Measurement. Required.
+                                    "schema": {
+                                        "arrowSchema": "str",  # The schema
+                                          in Arrow format, encoded with
+                                          dyff.schema.arrow.encode_schema(). This is required, but can
+                                          be populated from a DyffDataSchema. Required.
+                                        "dyffSchema": {
+                                            "components": [
+                                                "str"  # A list of
+                                                  named dyff data schemas. The final schema is the
+                                                  composition of these component schemas. Required.
+                                            ],
+                                            "schemaVersion": "0.1"  #
+                                              Optional. Default value is "0.1". The dyff schema
+                                              version. "0.1"
+                                        },
+                                        "jsonSchema": {}  # Optional. The
+                                          schema in JSON Schema format.
+                                    },
+                                    "description": "str"  # Optional. Long-form
+                                      description, interpreted as Markdown.
+                                },
+                                "safetyCase": {
+                                    "name": "str",  # Descriptive name of the
+                                      SafetyCase. Required.
+                                    "description": "str"  # Optional. Long-form
+                                      description, interpreted as Markdown.
+                                }
+                            },
+                            "scope": "str",  # The scope of the Method. The Method
+                              produces outputs that are specific to one entity of the type specified in
+                              the .scope field. Required. Known values are: "InferenceService" and
+                              "Evaluation".
+                            "description": "str",  # Optional. Long-form description,
+                              interpreted as Markdown.
+                            "inputs": [
+                                {
+                                    "keyword": "str",  # The input is referred to
+                                      by 'keyword' in the context of the method implementation.
+                                      Required.
+                                    "kind": "str",  # The kind of input artifact.
+                                      Required. Known values are: "Dataset", "Evaluation",
+                                      "Measurement", and "Report".
+                                    "description": "str"  # Optional. Long-form
+                                      description, interpreted as Markdown.
+                                }
+                            ],
+                            "modules": [
+                                "str"  # Optional. Modules to load into the analysis
+                                  environment.
+                            ],
+                            "parameters": [
+                                {
+                                    "keyword": "str",  # The parameter is
+                                      referred to by 'keyword' in the context of the method
+                                      implementation. Required.
+                                    "description": "str"  # Optional. Long-form
+                                      description, interpreted as Markdown.
+                                }
+                            ]
+                        },
+                        "name": "str",  # Descriptive name of the SafetyCase. Required.
+                        "scope": {
+                            "dataset": "str",  # Optional. Dataset.
+                            "evaluation": "str",  # Optional. Evaluation.
+                            "inferenceService": "str",  # Optional. Inferenceservice.
+                            "model": "str"  # Optional. Model.
+                        },
+                        "annotations": [
+                            {
+                                "key": "str",  # The annotation key. A DNS label with
+                                  an optional DNS domain prefix. For example: 'my-key',
+                                  'your.com/key_0'. Names prefixed with 'dyff.io/',
+                                  'subdomain.dyff.io/', etc. are reserved.  See
+                                  https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                                  for detailed naming rules. Required.
+                                "value": "str"  # The annotation value. An arbitrary
+                                  string. Required.
+                            }
+                        ],
+                        "arguments": [
+                            {
+                                "keyword": "str",  # The 'keyword' of the
+                                  corresponding ModelParameter. Required.
+                                "value": "str"  # The value of of the argument.
+                                  Always a string; implementations are responsible for parsing.
+                                  Required.
+                            }
+                        ],
+                        "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation
+                          time (assigned by system).
+                        "description": "str",  # Optional. Long-form description, interpreted
+                          as Markdown.
+                        "inputs": [
+                            {
+                                "entity": "str",  # The ID of the entity whose data
+                                  should be made available as 'keyword'. Required.
+                                "keyword": "str"  # The 'keyword' specified for this
+                                  input in the MethodSpec. Required.
+                            }
+                        ],
+                        "kind": "SafetyCase",  # Optional. Default value is "SafetyCase".
+                          Kind. "SafetyCase"
+                        "labels": {
+                            "str": "str"  # Optional. A set of key-value labels for the
+                              resource. Used to specify identifying attributes of resources that are
+                              meaningful to users but do not imply semantics in the dyff system.  The
+                              keys are DNS labels with an optional DNS domain prefix. For example:
+                              'my-key', 'your.com/key_0'. Keys prefixed with 'dyff.io/',
+                              'subdomain.dyff.io/', etc. are reserved.  The label values are
+                              alphanumeric characters separated by '.', '-', or '_'.  We follow the
+                              kubernetes label conventions closely. See:
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                        },
+                        "reason": "str",  # Optional. Reason for current status (assigned by
+                          system).
+                        "schemaVersion": "0.1",  # Optional. Default value is "0.1". The
+                          schema version. "0.1"
+                        "status": "str"  # Optional. Top-level resource status (assigned by
+                          system).
+                    }
+                ]
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
+
+        _request = build_safetycases_query_request(
+            id=id,
+            account=account,
+            status=status,
+            reason=reason,
+            labels=labels,
+            analysis=analysis,
+            method=method,
+            method_name=method_name,
+            inputs_any_of=inputs_any_of,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(Union[List[JSON], JSON], deserialized), {})  # type: ignore
+
+        return cast(Union[List[JSON], JSON], deserialized)  # type: ignore
+
+    @overload
+    async def create(
+        self, body: JSON, *, content_type: str = "application/json", **kwargs: Any
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Create a SafetyCase.
+
+        Create a SafetyCase.
+
+        :param body: Required.
+        :type body: JSON
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "method": "str",  # Method ID. Required.
+                    "scope": {
+                        "dataset": "str",  # Optional. Dataset.
+                        "evaluation": "str",  # Optional. Evaluation.
+                        "inferenceService": "str",  # Optional. Inferenceservice.
+                        "model": "str"  # Optional. Model.
+                    },
+                    "arguments": [
+                        {
+                            "keyword": "str",  # The 'keyword' of the corresponding
+                              ModelParameter. Required.
+                            "value": "str"  # The value of of the argument. Always a
+                              string; implementations are responsible for parsing. Required.
+                        }
+                    ],
+                    "inputs": [
+                        {
+                            "entity": "str",  # The ID of the entity whose data should be
+                              made available as 'keyword'. Required.
+                            "keyword": "str"  # The 'keyword' specified for this input in
+                              the MethodSpec. Required.
+                        }
+                    ],
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "id": "str",  # Unique identifier of the entity. Required.
+                    "method": {
+                        "account": "str",  # Account that owns the entity. Required.
+                        "id": "str",  # Unique identifier of the entity. Required.
+                        "implementation": {
+                            "kind": "str",  # The kind of implementation. Required.
+                            "jupyterNotebook": {
+                                "notebookModule": "str",  # ID of the Module that
+                                  contains the notebook file. This does *not* add the Module as a
+                                  dependency; you must do that separately. Required.
+                                "notebookPath": "str"  # Path to the notebook file
+                                  relative to the Module root directory. Required.
+                            },
+                            "pythonFunction": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python function to call. Required.
+                            },
+                            "pythonRubric": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python Rubric to run. Required.
+                            }
+                        },
+                        "name": "str",  # Descriptive name of the Method. Required.
+                        "output": {
+                            "kind": "str",  # The kind of output artifact. Required.
+                              Known values are: "Measurement" and "SafetyCase".
+                            "measurement": {
+                                "level": "str",  # Measurement level. Required. Known
+                                  values are: "Dataset" and "Instance".
+                                "name": "str",  # Descriptive name of the
+                                  Measurement. Required.
+                                "schema": {
+                                    "arrowSchema": "str",  # The schema in Arrow
+                                      format, encoded with dyff.schema.arrow.encode_schema(). This is
+                                      required, but can be populated from a DyffDataSchema. Required.
+                                    "dyffSchema": {
+                                        "components": [
+                                            "str"  # A list of named dyff
+                                              data schemas. The final schema is the composition of
+                                              these component schemas. Required.
+                                        ],
+                                        "schemaVersion": "0.1"  # Optional.
+                                          Default value is "0.1". The dyff schema version. "0.1"
+                                    },
+                                    "jsonSchema": {}  # Optional. The schema in
+                                      JSON Schema format.
+                                },
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            },
+                            "safetyCase": {
+                                "name": "str",  # Descriptive name of the SafetyCase.
+                                  Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        },
+                        "scope": "str",  # The scope of the Method. The Method produces
+                          outputs that are specific to one entity of the type specified in the .scope
+                          field. Required. Known values are: "InferenceService" and "Evaluation".
+                        "description": "str",  # Optional. Long-form description, interpreted
+                          as Markdown.
+                        "inputs": [
+                            {
+                                "keyword": "str",  # The input is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "kind": "str",  # The kind of input artifact.
+                                  Required. Known values are: "Dataset", "Evaluation", "Measurement",
+                                  and "Report".
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ],
+                        "modules": [
+                            "str"  # Optional. Modules to load into the analysis
+                              environment.
+                        ],
+                        "parameters": [
+                            {
+                                "keyword": "str",  # The parameter is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ]
+                    },
+                    "name": "str",  # Descriptive name of the SafetyCase. Required.
+                    "scope": {
+                        "dataset": "str",  # Optional. Dataset.
+                        "evaluation": "str",  # Optional. Evaluation.
+                        "inferenceService": "str",  # Optional. Inferenceservice.
+                        "model": "str"  # Optional. Model.
+                    },
+                    "annotations": [
+                        {
+                            "key": "str",  # The annotation key. A DNS label with an
+                              optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                              Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
+                              See
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                              for detailed naming rules. Required.
+                            "value": "str"  # The annotation value. An arbitrary string.
+                              Required.
+                        }
+                    ],
+                    "arguments": [
+                        {
+                            "keyword": "str",  # The 'keyword' of the corresponding
+                              ModelParameter. Required.
+                            "value": "str"  # The value of of the argument. Always a
+                              string; implementations are responsible for parsing. Required.
+                        }
+                    ],
+                    "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
+                      (assigned by system).
+                    "description": "str",  # Optional. Long-form description, interpreted as
+                      Markdown.
+                    "inputs": [
+                        {
+                            "entity": "str",  # The ID of the entity whose data should be
+                              made available as 'keyword'. Required.
+                            "keyword": "str"  # The 'keyword' specified for this input in
+                              the MethodSpec. Required.
+                        }
+                    ],
+                    "kind": "SafetyCase",  # Optional. Default value is "SafetyCase". Kind.
+                      "SafetyCase"
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    },
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @overload
+    async def create(
+        self, body: IO[bytes], *, content_type: str = "application/json", **kwargs: Any
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Create a SafetyCase.
+
+        Create a SafetyCase.
+
+        :param body: Required.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "id": "str",  # Unique identifier of the entity. Required.
+                    "method": {
+                        "account": "str",  # Account that owns the entity. Required.
+                        "id": "str",  # Unique identifier of the entity. Required.
+                        "implementation": {
+                            "kind": "str",  # The kind of implementation. Required.
+                            "jupyterNotebook": {
+                                "notebookModule": "str",  # ID of the Module that
+                                  contains the notebook file. This does *not* add the Module as a
+                                  dependency; you must do that separately. Required.
+                                "notebookPath": "str"  # Path to the notebook file
+                                  relative to the Module root directory. Required.
+                            },
+                            "pythonFunction": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python function to call. Required.
+                            },
+                            "pythonRubric": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python Rubric to run. Required.
+                            }
+                        },
+                        "name": "str",  # Descriptive name of the Method. Required.
+                        "output": {
+                            "kind": "str",  # The kind of output artifact. Required.
+                              Known values are: "Measurement" and "SafetyCase".
+                            "measurement": {
+                                "level": "str",  # Measurement level. Required. Known
+                                  values are: "Dataset" and "Instance".
+                                "name": "str",  # Descriptive name of the
+                                  Measurement. Required.
+                                "schema": {
+                                    "arrowSchema": "str",  # The schema in Arrow
+                                      format, encoded with dyff.schema.arrow.encode_schema(). This is
+                                      required, but can be populated from a DyffDataSchema. Required.
+                                    "dyffSchema": {
+                                        "components": [
+                                            "str"  # A list of named dyff
+                                              data schemas. The final schema is the composition of
+                                              these component schemas. Required.
+                                        ],
+                                        "schemaVersion": "0.1"  # Optional.
+                                          Default value is "0.1". The dyff schema version. "0.1"
+                                    },
+                                    "jsonSchema": {}  # Optional. The schema in
+                                      JSON Schema format.
+                                },
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            },
+                            "safetyCase": {
+                                "name": "str",  # Descriptive name of the SafetyCase.
+                                  Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        },
+                        "scope": "str",  # The scope of the Method. The Method produces
+                          outputs that are specific to one entity of the type specified in the .scope
+                          field. Required. Known values are: "InferenceService" and "Evaluation".
+                        "description": "str",  # Optional. Long-form description, interpreted
+                          as Markdown.
+                        "inputs": [
+                            {
+                                "keyword": "str",  # The input is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "kind": "str",  # The kind of input artifact.
+                                  Required. Known values are: "Dataset", "Evaluation", "Measurement",
+                                  and "Report".
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ],
+                        "modules": [
+                            "str"  # Optional. Modules to load into the analysis
+                              environment.
+                        ],
+                        "parameters": [
+                            {
+                                "keyword": "str",  # The parameter is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ]
+                    },
+                    "name": "str",  # Descriptive name of the SafetyCase. Required.
+                    "scope": {
+                        "dataset": "str",  # Optional. Dataset.
+                        "evaluation": "str",  # Optional. Evaluation.
+                        "inferenceService": "str",  # Optional. Inferenceservice.
+                        "model": "str"  # Optional. Model.
+                    },
+                    "annotations": [
+                        {
+                            "key": "str",  # The annotation key. A DNS label with an
+                              optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                              Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
+                              See
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                              for detailed naming rules. Required.
+                            "value": "str"  # The annotation value. An arbitrary string.
+                              Required.
+                        }
+                    ],
+                    "arguments": [
+                        {
+                            "keyword": "str",  # The 'keyword' of the corresponding
+                              ModelParameter. Required.
+                            "value": "str"  # The value of of the argument. Always a
+                              string; implementations are responsible for parsing. Required.
+                        }
+                    ],
+                    "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
+                      (assigned by system).
+                    "description": "str",  # Optional. Long-form description, interpreted as
+                      Markdown.
+                    "inputs": [
+                        {
+                            "entity": "str",  # The ID of the entity whose data should be
+                              made available as 'keyword'. Required.
+                            "keyword": "str"  # The 'keyword' specified for this input in
+                              the MethodSpec. Required.
+                        }
+                    ],
+                    "kind": "SafetyCase",  # Optional. Default value is "SafetyCase". Kind.
+                      "SafetyCase"
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    },
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @distributed_trace_async
+    async def create(self, body: Union[JSON, IO[bytes]], **kwargs: Any) -> JSON:
+        # pylint: disable=line-too-long
+        """Create a SafetyCase.
+
+        Create a SafetyCase.
+
+        :param body: Is either a JSON type or a IO[bytes] type. Required.
+        :type body: JSON or IO[bytes]
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "method": "str",  # Method ID. Required.
+                    "scope": {
+                        "dataset": "str",  # Optional. Dataset.
+                        "evaluation": "str",  # Optional. Evaluation.
+                        "inferenceService": "str",  # Optional. Inferenceservice.
+                        "model": "str"  # Optional. Model.
+                    },
+                    "arguments": [
+                        {
+                            "keyword": "str",  # The 'keyword' of the corresponding
+                              ModelParameter. Required.
+                            "value": "str"  # The value of of the argument. Always a
+                              string; implementations are responsible for parsing. Required.
+                        }
+                    ],
+                    "inputs": [
+                        {
+                            "entity": "str",  # The ID of the entity whose data should be
+                              made available as 'keyword'. Required.
+                            "keyword": "str"  # The 'keyword' specified for this input in
+                              the MethodSpec. Required.
+                        }
+                    ],
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "id": "str",  # Unique identifier of the entity. Required.
+                    "method": {
+                        "account": "str",  # Account that owns the entity. Required.
+                        "id": "str",  # Unique identifier of the entity. Required.
+                        "implementation": {
+                            "kind": "str",  # The kind of implementation. Required.
+                            "jupyterNotebook": {
+                                "notebookModule": "str",  # ID of the Module that
+                                  contains the notebook file. This does *not* add the Module as a
+                                  dependency; you must do that separately. Required.
+                                "notebookPath": "str"  # Path to the notebook file
+                                  relative to the Module root directory. Required.
+                            },
+                            "pythonFunction": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python function to call. Required.
+                            },
+                            "pythonRubric": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python Rubric to run. Required.
+                            }
+                        },
+                        "name": "str",  # Descriptive name of the Method. Required.
+                        "output": {
+                            "kind": "str",  # The kind of output artifact. Required.
+                              Known values are: "Measurement" and "SafetyCase".
+                            "measurement": {
+                                "level": "str",  # Measurement level. Required. Known
+                                  values are: "Dataset" and "Instance".
+                                "name": "str",  # Descriptive name of the
+                                  Measurement. Required.
+                                "schema": {
+                                    "arrowSchema": "str",  # The schema in Arrow
+                                      format, encoded with dyff.schema.arrow.encode_schema(). This is
+                                      required, but can be populated from a DyffDataSchema. Required.
+                                    "dyffSchema": {
+                                        "components": [
+                                            "str"  # A list of named dyff
+                                              data schemas. The final schema is the composition of
+                                              these component schemas. Required.
+                                        ],
+                                        "schemaVersion": "0.1"  # Optional.
+                                          Default value is "0.1". The dyff schema version. "0.1"
+                                    },
+                                    "jsonSchema": {}  # Optional. The schema in
+                                      JSON Schema format.
+                                },
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            },
+                            "safetyCase": {
+                                "name": "str",  # Descriptive name of the SafetyCase.
+                                  Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        },
+                        "scope": "str",  # The scope of the Method. The Method produces
+                          outputs that are specific to one entity of the type specified in the .scope
+                          field. Required. Known values are: "InferenceService" and "Evaluation".
+                        "description": "str",  # Optional. Long-form description, interpreted
+                          as Markdown.
+                        "inputs": [
+                            {
+                                "keyword": "str",  # The input is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "kind": "str",  # The kind of input artifact.
+                                  Required. Known values are: "Dataset", "Evaluation", "Measurement",
+                                  and "Report".
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ],
+                        "modules": [
+                            "str"  # Optional. Modules to load into the analysis
+                              environment.
+                        ],
+                        "parameters": [
+                            {
+                                "keyword": "str",  # The parameter is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ]
+                    },
+                    "name": "str",  # Descriptive name of the SafetyCase. Required.
+                    "scope": {
+                        "dataset": "str",  # Optional. Dataset.
+                        "evaluation": "str",  # Optional. Evaluation.
+                        "inferenceService": "str",  # Optional. Inferenceservice.
+                        "model": "str"  # Optional. Model.
+                    },
+                    "annotations": [
+                        {
+                            "key": "str",  # The annotation key. A DNS label with an
+                              optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                              Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
+                              See
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                              for detailed naming rules. Required.
+                            "value": "str"  # The annotation value. An arbitrary string.
+                              Required.
+                        }
+                    ],
+                    "arguments": [
+                        {
+                            "keyword": "str",  # The 'keyword' of the corresponding
+                              ModelParameter. Required.
+                            "value": "str"  # The value of of the argument. Always a
+                              string; implementations are responsible for parsing. Required.
+                        }
+                    ],
+                    "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
+                      (assigned by system).
+                    "description": "str",  # Optional. Long-form description, interpreted as
+                      Markdown.
+                    "inputs": [
+                        {
+                            "entity": "str",  # The ID of the entity whose data should be
+                              made available as 'keyword'. Required.
+                            "keyword": "str"  # The 'keyword' specified for this input in
+                              the MethodSpec. Required.
+                        }
+                    ],
+                    "kind": "SafetyCase",  # Optional. Default value is "SafetyCase". Kind.
+                      "SafetyCase"
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    },
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop(
+            "content_type", _headers.pop("Content-Type", None)
+        )
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        _request = build_safetycases_create_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @distributed_trace_async
+    async def get(self, safetycase_id: str, **kwargs: Any) -> JSON:
+        # pylint: disable=line-too-long
+        """Get a SafetyCase by its key.
+
+        Get a SafetyCase by its key. Raises a 404 error if no entity exists with that key.
+
+        :param safetycase_id: Required.
+        :type safetycase_id: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "id": "str",  # Unique identifier of the entity. Required.
+                    "method": {
+                        "account": "str",  # Account that owns the entity. Required.
+                        "id": "str",  # Unique identifier of the entity. Required.
+                        "implementation": {
+                            "kind": "str",  # The kind of implementation. Required.
+                            "jupyterNotebook": {
+                                "notebookModule": "str",  # ID of the Module that
+                                  contains the notebook file. This does *not* add the Module as a
+                                  dependency; you must do that separately. Required.
+                                "notebookPath": "str"  # Path to the notebook file
+                                  relative to the Module root directory. Required.
+                            },
+                            "pythonFunction": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python function to call. Required.
+                            },
+                            "pythonRubric": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python Rubric to run. Required.
+                            }
+                        },
+                        "name": "str",  # Descriptive name of the Method. Required.
+                        "output": {
+                            "kind": "str",  # The kind of output artifact. Required.
+                              Known values are: "Measurement" and "SafetyCase".
+                            "measurement": {
+                                "level": "str",  # Measurement level. Required. Known
+                                  values are: "Dataset" and "Instance".
+                                "name": "str",  # Descriptive name of the
+                                  Measurement. Required.
+                                "schema": {
+                                    "arrowSchema": "str",  # The schema in Arrow
+                                      format, encoded with dyff.schema.arrow.encode_schema(). This is
+                                      required, but can be populated from a DyffDataSchema. Required.
+                                    "dyffSchema": {
+                                        "components": [
+                                            "str"  # A list of named dyff
+                                              data schemas. The final schema is the composition of
+                                              these component schemas. Required.
+                                        ],
+                                        "schemaVersion": "0.1"  # Optional.
+                                          Default value is "0.1". The dyff schema version. "0.1"
+                                    },
+                                    "jsonSchema": {}  # Optional. The schema in
+                                      JSON Schema format.
+                                },
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            },
+                            "safetyCase": {
+                                "name": "str",  # Descriptive name of the SafetyCase.
+                                  Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        },
+                        "scope": "str",  # The scope of the Method. The Method produces
+                          outputs that are specific to one entity of the type specified in the .scope
+                          field. Required. Known values are: "InferenceService" and "Evaluation".
+                        "description": "str",  # Optional. Long-form description, interpreted
+                          as Markdown.
+                        "inputs": [
+                            {
+                                "keyword": "str",  # The input is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "kind": "str",  # The kind of input artifact.
+                                  Required. Known values are: "Dataset", "Evaluation", "Measurement",
+                                  and "Report".
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ],
+                        "modules": [
+                            "str"  # Optional. Modules to load into the analysis
+                              environment.
+                        ],
+                        "parameters": [
+                            {
+                                "keyword": "str",  # The parameter is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ]
+                    },
+                    "name": "str",  # Descriptive name of the SafetyCase. Required.
+                    "scope": {
+                        "dataset": "str",  # Optional. Dataset.
+                        "evaluation": "str",  # Optional. Evaluation.
+                        "inferenceService": "str",  # Optional. Inferenceservice.
+                        "model": "str"  # Optional. Model.
+                    },
+                    "annotations": [
+                        {
+                            "key": "str",  # The annotation key. A DNS label with an
+                              optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                              Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
+                              See
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                              for detailed naming rules. Required.
+                            "value": "str"  # The annotation value. An arbitrary string.
+                              Required.
+                        }
+                    ],
+                    "arguments": [
+                        {
+                            "keyword": "str",  # The 'keyword' of the corresponding
+                              ModelParameter. Required.
+                            "value": "str"  # The value of of the argument. Always a
+                              string; implementations are responsible for parsing. Required.
+                        }
+                    ],
+                    "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
+                      (assigned by system).
+                    "description": "str",  # Optional. Long-form description, interpreted as
+                      Markdown.
+                    "inputs": [
+                        {
+                            "entity": "str",  # The ID of the entity whose data should be
+                              made available as 'keyword'. Required.
+                            "keyword": "str"  # The 'keyword' specified for this input in
+                              the MethodSpec. Required.
+                        }
+                    ],
+                    "kind": "SafetyCase",  # Optional. Default value is "SafetyCase". Kind.
+                      "SafetyCase"
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    },
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        _request = build_safetycases_get_request(
+            safetycase_id=safetycase_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @distributed_trace_async
+    async def delete(self, safetycase_id: str, **kwargs: Any) -> JSON:
+        """Mark a SafetyCase for deletion.
+
+        Mark a SafetyCase for deletion.
+
+        :param safetycase_id: Required.
+        :type safetycase_id: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        _request = build_safetycases_delete_request(
+            safetycase_id=safetycase_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
```

### Comparing `dyff-client-0.2.2/dyff/client/_generated/aio/operations/_patch.py` & `dyff_client-0.3.0/dyff/client/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.2/dyff/client/_generated/operations/__init__.py` & `dyff_client-0.3.0/dyff/client/_generated/operations/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.2)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.12)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._operations import (
     AuditproceduresOperations,
     AuditsOperations,
     DatasetsOperations,
     EvaluationsOperations,
     InferenceservicesOperations,
     InferencesessionsOperations,
+    MeasurementsOperations,
+    MethodsOperations,
     ModelsOperations,
     ModulesOperations,
     ReportsOperations,
+    SafetycasesOperations,
 )
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import __all__ as _patch_all
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "AuditsOperations",
     "AuditproceduresOperations",
     "DatasetsOperations",
     "EvaluationsOperations",
     "InferenceservicesOperations",
     "InferencesessionsOperations",
+    "MeasurementsOperations",
+    "MethodsOperations",
     "ModelsOperations",
     "ModulesOperations",
     "ReportsOperations",
+    "SafetycasesOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

### Comparing `dyff-client-0.2.2/dyff/client/_generated/operations/_operations.py` & `dyff_client-0.3.0/dyff/client/_generated/operations/_operations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.2)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.12)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 import sys
 from io import IOBase
 from typing import (
     IO,
     Any,
     Callable,
     Dict,
     Iterator,
     List,
     Optional,
+    Type,
     TypeVar,
     Union,
     cast,
     overload,
 )
 
 from azure.core.exceptions import (
@@ -883,14 +884,280 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
 
 
+def build_measurements_label_request(measurement_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop(
+        "content_type", _headers.pop("Content-Type", None)
+    )
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/measurements/{measurement_id}/labels"
+    path_format_arguments = {
+        "measurement_id": _SERIALIZER.url("measurement_id", measurement_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header(
+            "content_type", content_type, "str"
+        )
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="PATCH", url=_url, headers=_headers, **kwargs)
+
+
+def build_measurements_query_request(
+    *,
+    id: Optional[str] = None,
+    account: Optional[str] = None,
+    status: Optional[str] = None,
+    reason: Optional[str] = None,
+    labels: Optional[str] = None,
+    analysis: Optional[str] = None,
+    method: Optional[str] = None,
+    method_name: Optional[str] = None,
+    inputs_any_of: Optional[str] = None,
+    **kwargs: Any,
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/measurements"
+
+    # Construct parameters
+    if id is not None:
+        _params["id"] = _SERIALIZER.query("id", id, "str")
+    if account is not None:
+        _params["account"] = _SERIALIZER.query("account", account, "str")
+    if status is not None:
+        _params["status"] = _SERIALIZER.query("status", status, "str")
+    if reason is not None:
+        _params["reason"] = _SERIALIZER.query("reason", reason, "str")
+    if labels is not None:
+        _params["labels"] = _SERIALIZER.query("labels", labels, "str")
+    if analysis is not None:
+        _params["analysis"] = _SERIALIZER.query("analysis", analysis, "str")
+    if method is not None:
+        _params["method"] = _SERIALIZER.query("method", method, "str")
+    if method_name is not None:
+        _params["methodName"] = _SERIALIZER.query("method_name", method_name, "str")
+    if inputs_any_of is not None:
+        _params["inputsAnyOf"] = _SERIALIZER.query(
+            "inputs_any_of", inputs_any_of, "str"
+        )
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(
+        method="GET", url=_url, params=_params, headers=_headers, **kwargs
+    )
+
+
+def build_measurements_create_request(**kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop(
+        "content_type", _headers.pop("Content-Type", None)
+    )
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/measurements"
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header(
+            "content_type", content_type, "str"
+        )
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
+def build_measurements_get_request(measurement_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/measurements/{measurement_id}"
+    path_format_arguments = {
+        "measurement_id": _SERIALIZER.url("measurement_id", measurement_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
+
+
+def build_measurements_delete_request(
+    measurement_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/measurements/{measurement_id}/delete"
+    path_format_arguments = {
+        "measurement_id": _SERIALIZER.url("measurement_id", measurement_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="PUT", url=_url, headers=_headers, **kwargs)
+
+
+def build_methods_label_request(method_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop(
+        "content_type", _headers.pop("Content-Type", None)
+    )
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/methods/{method_id}/labels"
+    path_format_arguments = {
+        "method_id": _SERIALIZER.url("method_id", method_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header(
+            "content_type", content_type, "str"
+        )
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="PATCH", url=_url, headers=_headers, **kwargs)
+
+
+def build_methods_query_request(
+    *,
+    id: Optional[str] = None,
+    account: Optional[str] = None,
+    status: Optional[str] = None,
+    reason: Optional[str] = None,
+    labels: Optional[str] = None,
+    name: Optional[str] = None,
+    output_kind: Optional[str] = None,
+    **kwargs: Any,
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/methods"
+
+    # Construct parameters
+    if id is not None:
+        _params["id"] = _SERIALIZER.query("id", id, "str")
+    if account is not None:
+        _params["account"] = _SERIALIZER.query("account", account, "str")
+    if status is not None:
+        _params["status"] = _SERIALIZER.query("status", status, "str")
+    if reason is not None:
+        _params["reason"] = _SERIALIZER.query("reason", reason, "str")
+    if labels is not None:
+        _params["labels"] = _SERIALIZER.query("labels", labels, "str")
+    if name is not None:
+        _params["name"] = _SERIALIZER.query("name", name, "str")
+    if output_kind is not None:
+        _params["outputKind"] = _SERIALIZER.query("output_kind", output_kind, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(
+        method="GET", url=_url, params=_params, headers=_headers, **kwargs
+    )
+
+
+def build_methods_create_request(**kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop(
+        "content_type", _headers.pop("Content-Type", None)
+    )
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/methods"
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header(
+            "content_type", content_type, "str"
+        )
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
+def build_methods_get_request(method_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/methods/{method_id}"
+    path_format_arguments = {
+        "method_id": _SERIALIZER.url("method_id", method_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
+
+
+def build_methods_delete_request(method_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/methods/{method_id}/delete"
+    path_format_arguments = {
+        "method_id": _SERIALIZER.url("method_id", method_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="PUT", url=_url, headers=_headers, **kwargs)
+
+
 def build_models_label_request(model_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     content_type: Optional[str] = kwargs.pop(
         "content_type", _headers.pop("Content-Type", None)
     )
     accept = _headers.pop("Accept", "application/json")
@@ -1332,21 +1599,157 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
 
 
+def build_safetycases_label_request(safetycase_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop(
+        "content_type", _headers.pop("Content-Type", None)
+    )
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/safetycases/{safetycase_id}/labels"
+    path_format_arguments = {
+        "safetycase_id": _SERIALIZER.url("safetycase_id", safetycase_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header(
+            "content_type", content_type, "str"
+        )
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="PATCH", url=_url, headers=_headers, **kwargs)
+
+
+def build_safetycases_query_request(
+    *,
+    id: Optional[str] = None,
+    account: Optional[str] = None,
+    status: Optional[str] = None,
+    reason: Optional[str] = None,
+    labels: Optional[str] = None,
+    analysis: Optional[str] = None,
+    method: Optional[str] = None,
+    method_name: Optional[str] = None,
+    inputs_any_of: Optional[str] = None,
+    **kwargs: Any,
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/safetycases"
+
+    # Construct parameters
+    if id is not None:
+        _params["id"] = _SERIALIZER.query("id", id, "str")
+    if account is not None:
+        _params["account"] = _SERIALIZER.query("account", account, "str")
+    if status is not None:
+        _params["status"] = _SERIALIZER.query("status", status, "str")
+    if reason is not None:
+        _params["reason"] = _SERIALIZER.query("reason", reason, "str")
+    if labels is not None:
+        _params["labels"] = _SERIALIZER.query("labels", labels, "str")
+    if analysis is not None:
+        _params["analysis"] = _SERIALIZER.query("analysis", analysis, "str")
+    if method is not None:
+        _params["method"] = _SERIALIZER.query("method", method, "str")
+    if method_name is not None:
+        _params["methodName"] = _SERIALIZER.query("method_name", method_name, "str")
+    if inputs_any_of is not None:
+        _params["inputsAnyOf"] = _SERIALIZER.query(
+            "inputs_any_of", inputs_any_of, "str"
+        )
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(
+        method="GET", url=_url, params=_params, headers=_headers, **kwargs
+    )
+
+
+def build_safetycases_create_request(**kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop(
+        "content_type", _headers.pop("Content-Type", None)
+    )
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/safetycases"
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header(
+            "content_type", content_type, "str"
+        )
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
+def build_safetycases_get_request(safetycase_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/safetycases/{safetycase_id}"
+    path_format_arguments = {
+        "safetycase_id": _SERIALIZER.url("safetycase_id", safetycase_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
+
+
+def build_safetycases_delete_request(safetycase_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/safetycases/{safetycase_id}/delete"
+    path_format_arguments = {
+        "safetycase_id": _SERIALIZER.url("safetycase_id", safetycase_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="PUT", url=_url, headers=_headers, **kwargs)
+
+
 class AuditsOperations:  # pylint: disable=abstract-class-instantiated
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~_generated.DyffAPI`'s
+        :class:`~_generated.DyffV0API`'s
         :attr:`audits` attribute.
     """
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
@@ -1502,15 +1905,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1662,15 +2065,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1786,15 +2189,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1873,15 +2276,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -1934,15 +2337,15 @@
 
 class AuditproceduresOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~_generated.DyffAPI`'s
+        :class:`~_generated.DyffV0API`'s
         :attr:`auditprocedures` attribute.
     """
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
@@ -1955,15 +2358,15 @@
     def download(self, path: str, **kwargs: Any) -> Union[Iterator[bytes], JSON]:
         """Download the source code of an AuditProcedure.
 
         Download the source code of an AuditProcedure.
 
         :param path: Required.
         :type path: str
-        :return: Iterator of the response bytes or JSON object or None
+        :return: Iterator[bytes] or JSON object or None
         :rtype: Iterator[bytes] or JSON or None
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 422
@@ -1975,15 +2378,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -2031,15 +2434,15 @@
 
 class DatasetsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~_generated.DyffAPI`'s
+        :class:`~_generated.DyffV0API`'s
         :attr:`datasets` attribute.
     """
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
@@ -2188,15 +2591,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -2405,15 +2808,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -2959,15 +3362,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -3145,15 +3548,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -3208,15 +3611,15 @@
         """Get the strata corresponding to a Dataset.
 
         Get the strata corresponding to a Dataset. The data is returned as a
         Parquet file suitable for reading with libraries like Pandas.
 
         :param dataset_id: Required.
         :type dataset_id: str
-        :return: Iterator of the response bytes or JSON object or None
+        :return: Iterator[bytes] or JSON object or None
         :rtype: Iterator[bytes] or JSON or None
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 422
@@ -3228,15 +3631,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -3286,15 +3689,15 @@
         """Get the raw data for the Dataset.
 
         Get the raw data for the Dataset. The data is streamed in pyarrow.ipc
         format.
 
         :param dataset_id: Required.
         :type dataset_id: str
-        :return: Iterator of the response bytes or JSON object or None
+        :return: Iterator[bytes] or JSON object or None
         :rtype: Iterator[bytes] or JSON or None
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 422
@@ -3306,15 +3709,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -3388,15 +3791,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -3481,15 +3884,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -3564,15 +3967,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -3625,15 +4028,15 @@
 
 class EvaluationsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~_generated.DyffAPI`'s
+        :class:`~_generated.DyffV0API`'s
         :attr:`evaluations` attribute.
     """
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
@@ -3782,15 +4185,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -4125,15 +4528,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -4953,15 +5356,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -5247,15 +5650,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -5334,15 +5737,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -5395,15 +5798,15 @@
 
 class InferenceservicesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~_generated.DyffAPI`'s
+        :class:`~_generated.DyffV0API`'s
         :attr:`inferenceservices` attribute.
     """
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
@@ -5552,15 +5955,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -5838,15 +6241,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -6678,15 +7081,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -6928,15 +7331,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7015,15 +7418,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7076,15 +7479,15 @@
 
 class InferencesessionsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~_generated.DyffAPI`'s
+        :class:`~_generated.DyffV0API`'s
         :attr:`inferencesessions` attribute.
     """
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
@@ -7233,15 +7636,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7559,15 +7962,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8364,15 +8767,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8639,15 +9042,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8726,15 +9129,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8813,15 +9216,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8899,15 +9302,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8982,15 +9385,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9070,15 +9473,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9125,21 +9528,3015 @@
 
         if cls:
             return cls(pipeline_response, cast(Union[Any, JSON], deserialized), {})  # type: ignore
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
 
+class MeasurementsOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~_generated.DyffV0API`'s
+        :attr:`measurements` attribute.
+    """
+
+    def __init__(self, *args, **kwargs):
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = (
+            input_args.pop(0) if input_args else kwargs.pop("deserializer")
+        )
+
+    @overload
+    def label(
+        self,
+        measurement_id: str,
+        body: JSON,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> Union[Any, JSON]:
+        # pylint: disable=line-too-long
+        """Update labels for an existing Measurement.
+
+        Update labels for an existing Measurement.
+
+        :param measurement_id: Required.
+        :type measurement_id: str
+        :param body: Required.
+        :type body: JSON
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: any or JSON object
+        :rtype: any or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    }
+                }
+
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @overload
+    def label(
+        self,
+        measurement_id: str,
+        body: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> Union[Any, JSON]:
+        """Update labels for an existing Measurement.
+
+        Update labels for an existing Measurement.
+
+        :param measurement_id: Required.
+        :type measurement_id: str
+        :param body: Required.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: any or JSON object
+        :rtype: any or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @distributed_trace
+    def label(
+        self, measurement_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any
+    ) -> Union[Any, JSON]:
+        # pylint: disable=line-too-long
+        """Update labels for an existing Measurement.
+
+        Update labels for an existing Measurement.
+
+        :param measurement_id: Required.
+        :type measurement_id: str
+        :param body: Is either a JSON type or a IO[bytes] type. Required.
+        :type body: JSON or IO[bytes]
+        :return: any or JSON object
+        :rtype: any or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    }
+                }
+
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop(
+            "content_type", _headers.pop("Content-Type", None)
+        )
+        cls: ClsType[Union[Any, JSON]] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        _request = build_measurements_label_request(
+            measurement_id=measurement_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(Union[Any, JSON], deserialized), {})  # type: ignore
+
+        return cast(Union[Any, JSON], deserialized)  # type: ignore
+
+    @distributed_trace
+    def query(
+        self,
+        *,
+        id: Optional[str] = None,
+        account: Optional[str] = None,
+        status: Optional[str] = None,
+        reason: Optional[str] = None,
+        labels: Optional[str] = None,
+        analysis: Optional[str] = None,
+        method: Optional[str] = None,
+        method_name: Optional[str] = None,
+        inputs_any_of: Optional[str] = None,
+        **kwargs: Any,
+    ) -> Union[List[JSON], JSON]:
+        # pylint: disable=line-too-long
+        """Get all Measurements matching a query.
+
+        Get all Measurements matching a query. The query is a set of equality
+        constraints specified as key-value pairs.
+
+        :keyword id: Default value is None.
+        :paramtype id: str
+        :keyword account: Default value is None.
+        :paramtype account: str
+        :keyword status: Default value is None.
+        :paramtype status: str
+        :keyword reason: Default value is None.
+        :paramtype reason: str
+        :keyword labels: Default value is None.
+        :paramtype labels: str
+        :keyword analysis: Default value is None.
+        :paramtype analysis: str
+        :keyword method: Default value is None.
+        :paramtype method: str
+        :keyword method_name: Default value is None.
+        :paramtype method_name: str
+        :keyword inputs_any_of: Default value is None.
+        :paramtype inputs_any_of: str
+        :return: list of JSON object or JSON object
+        :rtype: list[JSON] or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == [
+                    {
+                        "account": "str",  # Account that owns the entity. Required.
+                        "id": "str",  # Unique identifier of the entity. Required.
+                        "level": "str",  # Measurement level. Required. Known values are:
+                          "Dataset" and "Instance".
+                        "method": {
+                            "account": "str",  # Account that owns the entity. Required.
+                            "id": "str",  # Unique identifier of the entity. Required.
+                            "implementation": {
+                                "kind": "str",  # The kind of implementation.
+                                  Required.
+                                "jupyterNotebook": {
+                                    "notebookModule": "str",  # ID of the Module
+                                      that contains the notebook file. This does *not* add the Module
+                                      as a dependency; you must do that separately. Required.
+                                    "notebookPath": "str"  # Path to the notebook
+                                      file relative to the Module root directory. Required.
+                                },
+                                "pythonFunction": {
+                                    "fullyQualifiedName": "str"  # The
+                                      fully-qualified name of the Python function to call. Required.
+                                },
+                                "pythonRubric": {
+                                    "fullyQualifiedName": "str"  # The
+                                      fully-qualified name of the Python Rubric to run. Required.
+                                }
+                            },
+                            "name": "str",  # Descriptive name of the Method. Required.
+                            "output": {
+                                "kind": "str",  # The kind of output artifact.
+                                  Required. Known values are: "Measurement" and "SafetyCase".
+                                "measurement": {
+                                    "level": "str",  # Measurement level.
+                                      Required. Known values are: "Dataset" and "Instance".
+                                    "name": "str",  # Descriptive name of the
+                                      Measurement. Required.
+                                    "schema": {
+                                        "arrowSchema": "str",  # The schema
+                                          in Arrow format, encoded with
+                                          dyff.schema.arrow.encode_schema(). This is required, but can
+                                          be populated from a DyffDataSchema. Required.
+                                        "dyffSchema": {
+                                            "components": [
+                                                "str"  # A list of
+                                                  named dyff data schemas. The final schema is the
+                                                  composition of these component schemas. Required.
+                                            ],
+                                            "schemaVersion": "0.1"  #
+                                              Optional. Default value is "0.1". The dyff schema
+                                              version. "0.1"
+                                        },
+                                        "jsonSchema": {}  # Optional. The
+                                          schema in JSON Schema format.
+                                    },
+                                    "description": "str"  # Optional. Long-form
+                                      description, interpreted as Markdown.
+                                },
+                                "safetyCase": {
+                                    "name": "str",  # Descriptive name of the
+                                      SafetyCase. Required.
+                                    "description": "str"  # Optional. Long-form
+                                      description, interpreted as Markdown.
+                                }
+                            },
+                            "scope": "str",  # The scope of the Method. The Method
+                              produces outputs that are specific to one entity of the type specified in
+                              the .scope field. Required. Known values are: "InferenceService" and
+                              "Evaluation".
+                            "description": "str",  # Optional. Long-form description,
+                              interpreted as Markdown.
+                            "inputs": [
+                                {
+                                    "keyword": "str",  # The input is referred to
+                                      by 'keyword' in the context of the method implementation.
+                                      Required.
+                                    "kind": "str",  # The kind of input artifact.
+                                      Required. Known values are: "Dataset", "Evaluation",
+                                      "Measurement", and "Report".
+                                    "description": "str"  # Optional. Long-form
+                                      description, interpreted as Markdown.
+                                }
+                            ],
+                            "modules": [
+                                "str"  # Optional. Modules to load into the analysis
+                                  environment.
+                            ],
+                            "parameters": [
+                                {
+                                    "keyword": "str",  # The parameter is
+                                      referred to by 'keyword' in the context of the method
+                                      implementation. Required.
+                                    "description": "str"  # Optional. Long-form
+                                      description, interpreted as Markdown.
+                                }
+                            ]
+                        },
+                        "name": "str",  # Descriptive name of the Measurement. Required.
+                        "schema": {
+                            "arrowSchema": "str",  # The schema in Arrow format, encoded
+                              with dyff.schema.arrow.encode_schema(). This is required, but can be
+                              populated from a DyffDataSchema. Required.
+                            "dyffSchema": {
+                                "components": [
+                                    "str"  # A list of named dyff data schemas.
+                                      The final schema is the composition of these component schemas.
+                                      Required.
+                                ],
+                                "schemaVersion": "0.1"  # Optional. Default value is
+                                  "0.1". The dyff schema version. "0.1"
+                            },
+                            "jsonSchema": {}  # Optional. The schema in JSON Schema
+                              format.
+                        },
+                        "scope": {
+                            "dataset": "str",  # Optional. Dataset.
+                            "evaluation": "str",  # Optional. Evaluation.
+                            "inferenceService": "str",  # Optional. Inferenceservice.
+                            "model": "str"  # Optional. Model.
+                        },
+                        "annotations": [
+                            {
+                                "key": "str",  # The annotation key. A DNS label with
+                                  an optional DNS domain prefix. For example: 'my-key',
+                                  'your.com/key_0'. Names prefixed with 'dyff.io/',
+                                  'subdomain.dyff.io/', etc. are reserved.  See
+                                  https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                                  for detailed naming rules. Required.
+                                "value": "str"  # The annotation value. An arbitrary
+                                  string. Required.
+                            }
+                        ],
+                        "arguments": [
+                            {
+                                "keyword": "str",  # The 'keyword' of the
+                                  corresponding ModelParameter. Required.
+                                "value": "str"  # The value of of the argument.
+                                  Always a string; implementations are responsible for parsing.
+                                  Required.
+                            }
+                        ],
+                        "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation
+                          time (assigned by system).
+                        "description": "str",  # Optional. Long-form description, interpreted
+                          as Markdown.
+                        "inputs": [
+                            {
+                                "entity": "str",  # The ID of the entity whose data
+                                  should be made available as 'keyword'. Required.
+                                "keyword": "str"  # The 'keyword' specified for this
+                                  input in the MethodSpec. Required.
+                            }
+                        ],
+                        "kind": "Measurement",  # Optional. Default value is "Measurement".
+                          Kind. "Measurement"
+                        "labels": {
+                            "str": "str"  # Optional. A set of key-value labels for the
+                              resource. Used to specify identifying attributes of resources that are
+                              meaningful to users but do not imply semantics in the dyff system.  The
+                              keys are DNS labels with an optional DNS domain prefix. For example:
+                              'my-key', 'your.com/key_0'. Keys prefixed with 'dyff.io/',
+                              'subdomain.dyff.io/', etc. are reserved.  The label values are
+                              alphanumeric characters separated by '.', '-', or '_'.  We follow the
+                              kubernetes label conventions closely. See:
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                        },
+                        "reason": "str",  # Optional. Reason for current status (assigned by
+                          system).
+                        "schemaVersion": "0.1",  # Optional. Default value is "0.1". The
+                          schema version. "0.1"
+                        "status": "str"  # Optional. Top-level resource status (assigned by
+                          system).
+                    }
+                ]
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
+
+        _request = build_measurements_query_request(
+            id=id,
+            account=account,
+            status=status,
+            reason=reason,
+            labels=labels,
+            analysis=analysis,
+            method=method,
+            method_name=method_name,
+            inputs_any_of=inputs_any_of,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(Union[List[JSON], JSON], deserialized), {})  # type: ignore
+
+        return cast(Union[List[JSON], JSON], deserialized)  # type: ignore
+
+    @overload
+    def create(
+        self, body: JSON, *, content_type: str = "application/json", **kwargs: Any
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Create a Measurement.
+
+        Create a Measurement.
+
+        :param body: Required.
+        :type body: JSON
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "method": "str",  # Method ID. Required.
+                    "scope": {
+                        "dataset": "str",  # Optional. Dataset.
+                        "evaluation": "str",  # Optional. Evaluation.
+                        "inferenceService": "str",  # Optional. Inferenceservice.
+                        "model": "str"  # Optional. Model.
+                    },
+                    "arguments": [
+                        {
+                            "keyword": "str",  # The 'keyword' of the corresponding
+                              ModelParameter. Required.
+                            "value": "str"  # The value of of the argument. Always a
+                              string; implementations are responsible for parsing. Required.
+                        }
+                    ],
+                    "inputs": [
+                        {
+                            "entity": "str",  # The ID of the entity whose data should be
+                              made available as 'keyword'. Required.
+                            "keyword": "str"  # The 'keyword' specified for this input in
+                              the MethodSpec. Required.
+                        }
+                    ],
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "id": "str",  # Unique identifier of the entity. Required.
+                    "level": "str",  # Measurement level. Required. Known values are: "Dataset"
+                      and "Instance".
+                    "method": {
+                        "account": "str",  # Account that owns the entity. Required.
+                        "id": "str",  # Unique identifier of the entity. Required.
+                        "implementation": {
+                            "kind": "str",  # The kind of implementation. Required.
+                            "jupyterNotebook": {
+                                "notebookModule": "str",  # ID of the Module that
+                                  contains the notebook file. This does *not* add the Module as a
+                                  dependency; you must do that separately. Required.
+                                "notebookPath": "str"  # Path to the notebook file
+                                  relative to the Module root directory. Required.
+                            },
+                            "pythonFunction": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python function to call. Required.
+                            },
+                            "pythonRubric": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python Rubric to run. Required.
+                            }
+                        },
+                        "name": "str",  # Descriptive name of the Method. Required.
+                        "output": {
+                            "kind": "str",  # The kind of output artifact. Required.
+                              Known values are: "Measurement" and "SafetyCase".
+                            "measurement": {
+                                "level": "str",  # Measurement level. Required. Known
+                                  values are: "Dataset" and "Instance".
+                                "name": "str",  # Descriptive name of the
+                                  Measurement. Required.
+                                "schema": {
+                                    "arrowSchema": "str",  # The schema in Arrow
+                                      format, encoded with dyff.schema.arrow.encode_schema(). This is
+                                      required, but can be populated from a DyffDataSchema. Required.
+                                    "dyffSchema": {
+                                        "components": [
+                                            "str"  # A list of named dyff
+                                              data schemas. The final schema is the composition of
+                                              these component schemas. Required.
+                                        ],
+                                        "schemaVersion": "0.1"  # Optional.
+                                          Default value is "0.1". The dyff schema version. "0.1"
+                                    },
+                                    "jsonSchema": {}  # Optional. The schema in
+                                      JSON Schema format.
+                                },
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            },
+                            "safetyCase": {
+                                "name": "str",  # Descriptive name of the SafetyCase.
+                                  Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        },
+                        "scope": "str",  # The scope of the Method. The Method produces
+                          outputs that are specific to one entity of the type specified in the .scope
+                          field. Required. Known values are: "InferenceService" and "Evaluation".
+                        "description": "str",  # Optional. Long-form description, interpreted
+                          as Markdown.
+                        "inputs": [
+                            {
+                                "keyword": "str",  # The input is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "kind": "str",  # The kind of input artifact.
+                                  Required. Known values are: "Dataset", "Evaluation", "Measurement",
+                                  and "Report".
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ],
+                        "modules": [
+                            "str"  # Optional. Modules to load into the analysis
+                              environment.
+                        ],
+                        "parameters": [
+                            {
+                                "keyword": "str",  # The parameter is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ]
+                    },
+                    "name": "str",  # Descriptive name of the Measurement. Required.
+                    "schema": {
+                        "arrowSchema": "str",  # The schema in Arrow format, encoded with
+                          dyff.schema.arrow.encode_schema(). This is required, but can be populated
+                          from a DyffDataSchema. Required.
+                        "dyffSchema": {
+                            "components": [
+                                "str"  # A list of named dyff data schemas. The final
+                                  schema is the composition of these component schemas. Required.
+                            ],
+                            "schemaVersion": "0.1"  # Optional. Default value is "0.1".
+                              The dyff schema version. "0.1"
+                        },
+                        "jsonSchema": {}  # Optional. The schema in JSON Schema format.
+                    },
+                    "scope": {
+                        "dataset": "str",  # Optional. Dataset.
+                        "evaluation": "str",  # Optional. Evaluation.
+                        "inferenceService": "str",  # Optional. Inferenceservice.
+                        "model": "str"  # Optional. Model.
+                    },
+                    "annotations": [
+                        {
+                            "key": "str",  # The annotation key. A DNS label with an
+                              optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                              Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
+                              See
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                              for detailed naming rules. Required.
+                            "value": "str"  # The annotation value. An arbitrary string.
+                              Required.
+                        }
+                    ],
+                    "arguments": [
+                        {
+                            "keyword": "str",  # The 'keyword' of the corresponding
+                              ModelParameter. Required.
+                            "value": "str"  # The value of of the argument. Always a
+                              string; implementations are responsible for parsing. Required.
+                        }
+                    ],
+                    "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
+                      (assigned by system).
+                    "description": "str",  # Optional. Long-form description, interpreted as
+                      Markdown.
+                    "inputs": [
+                        {
+                            "entity": "str",  # The ID of the entity whose data should be
+                              made available as 'keyword'. Required.
+                            "keyword": "str"  # The 'keyword' specified for this input in
+                              the MethodSpec. Required.
+                        }
+                    ],
+                    "kind": "Measurement",  # Optional. Default value is "Measurement". Kind.
+                      "Measurement"
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    },
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @overload
+    def create(
+        self, body: IO[bytes], *, content_type: str = "application/json", **kwargs: Any
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Create a Measurement.
+
+        Create a Measurement.
+
+        :param body: Required.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "id": "str",  # Unique identifier of the entity. Required.
+                    "level": "str",  # Measurement level. Required. Known values are: "Dataset"
+                      and "Instance".
+                    "method": {
+                        "account": "str",  # Account that owns the entity. Required.
+                        "id": "str",  # Unique identifier of the entity. Required.
+                        "implementation": {
+                            "kind": "str",  # The kind of implementation. Required.
+                            "jupyterNotebook": {
+                                "notebookModule": "str",  # ID of the Module that
+                                  contains the notebook file. This does *not* add the Module as a
+                                  dependency; you must do that separately. Required.
+                                "notebookPath": "str"  # Path to the notebook file
+                                  relative to the Module root directory. Required.
+                            },
+                            "pythonFunction": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python function to call. Required.
+                            },
+                            "pythonRubric": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python Rubric to run. Required.
+                            }
+                        },
+                        "name": "str",  # Descriptive name of the Method. Required.
+                        "output": {
+                            "kind": "str",  # The kind of output artifact. Required.
+                              Known values are: "Measurement" and "SafetyCase".
+                            "measurement": {
+                                "level": "str",  # Measurement level. Required. Known
+                                  values are: "Dataset" and "Instance".
+                                "name": "str",  # Descriptive name of the
+                                  Measurement. Required.
+                                "schema": {
+                                    "arrowSchema": "str",  # The schema in Arrow
+                                      format, encoded with dyff.schema.arrow.encode_schema(). This is
+                                      required, but can be populated from a DyffDataSchema. Required.
+                                    "dyffSchema": {
+                                        "components": [
+                                            "str"  # A list of named dyff
+                                              data schemas. The final schema is the composition of
+                                              these component schemas. Required.
+                                        ],
+                                        "schemaVersion": "0.1"  # Optional.
+                                          Default value is "0.1". The dyff schema version. "0.1"
+                                    },
+                                    "jsonSchema": {}  # Optional. The schema in
+                                      JSON Schema format.
+                                },
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            },
+                            "safetyCase": {
+                                "name": "str",  # Descriptive name of the SafetyCase.
+                                  Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        },
+                        "scope": "str",  # The scope of the Method. The Method produces
+                          outputs that are specific to one entity of the type specified in the .scope
+                          field. Required. Known values are: "InferenceService" and "Evaluation".
+                        "description": "str",  # Optional. Long-form description, interpreted
+                          as Markdown.
+                        "inputs": [
+                            {
+                                "keyword": "str",  # The input is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "kind": "str",  # The kind of input artifact.
+                                  Required. Known values are: "Dataset", "Evaluation", "Measurement",
+                                  and "Report".
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ],
+                        "modules": [
+                            "str"  # Optional. Modules to load into the analysis
+                              environment.
+                        ],
+                        "parameters": [
+                            {
+                                "keyword": "str",  # The parameter is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ]
+                    },
+                    "name": "str",  # Descriptive name of the Measurement. Required.
+                    "schema": {
+                        "arrowSchema": "str",  # The schema in Arrow format, encoded with
+                          dyff.schema.arrow.encode_schema(). This is required, but can be populated
+                          from a DyffDataSchema. Required.
+                        "dyffSchema": {
+                            "components": [
+                                "str"  # A list of named dyff data schemas. The final
+                                  schema is the composition of these component schemas. Required.
+                            ],
+                            "schemaVersion": "0.1"  # Optional. Default value is "0.1".
+                              The dyff schema version. "0.1"
+                        },
+                        "jsonSchema": {}  # Optional. The schema in JSON Schema format.
+                    },
+                    "scope": {
+                        "dataset": "str",  # Optional. Dataset.
+                        "evaluation": "str",  # Optional. Evaluation.
+                        "inferenceService": "str",  # Optional. Inferenceservice.
+                        "model": "str"  # Optional. Model.
+                    },
+                    "annotations": [
+                        {
+                            "key": "str",  # The annotation key. A DNS label with an
+                              optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                              Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
+                              See
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                              for detailed naming rules. Required.
+                            "value": "str"  # The annotation value. An arbitrary string.
+                              Required.
+                        }
+                    ],
+                    "arguments": [
+                        {
+                            "keyword": "str",  # The 'keyword' of the corresponding
+                              ModelParameter. Required.
+                            "value": "str"  # The value of of the argument. Always a
+                              string; implementations are responsible for parsing. Required.
+                        }
+                    ],
+                    "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
+                      (assigned by system).
+                    "description": "str",  # Optional. Long-form description, interpreted as
+                      Markdown.
+                    "inputs": [
+                        {
+                            "entity": "str",  # The ID of the entity whose data should be
+                              made available as 'keyword'. Required.
+                            "keyword": "str"  # The 'keyword' specified for this input in
+                              the MethodSpec. Required.
+                        }
+                    ],
+                    "kind": "Measurement",  # Optional. Default value is "Measurement". Kind.
+                      "Measurement"
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    },
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @distributed_trace
+    def create(self, body: Union[JSON, IO[bytes]], **kwargs: Any) -> JSON:
+        # pylint: disable=line-too-long
+        """Create a Measurement.
+
+        Create a Measurement.
+
+        :param body: Is either a JSON type or a IO[bytes] type. Required.
+        :type body: JSON or IO[bytes]
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "method": "str",  # Method ID. Required.
+                    "scope": {
+                        "dataset": "str",  # Optional. Dataset.
+                        "evaluation": "str",  # Optional. Evaluation.
+                        "inferenceService": "str",  # Optional. Inferenceservice.
+                        "model": "str"  # Optional. Model.
+                    },
+                    "arguments": [
+                        {
+                            "keyword": "str",  # The 'keyword' of the corresponding
+                              ModelParameter. Required.
+                            "value": "str"  # The value of of the argument. Always a
+                              string; implementations are responsible for parsing. Required.
+                        }
+                    ],
+                    "inputs": [
+                        {
+                            "entity": "str",  # The ID of the entity whose data should be
+                              made available as 'keyword'. Required.
+                            "keyword": "str"  # The 'keyword' specified for this input in
+                              the MethodSpec. Required.
+                        }
+                    ],
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "id": "str",  # Unique identifier of the entity. Required.
+                    "level": "str",  # Measurement level. Required. Known values are: "Dataset"
+                      and "Instance".
+                    "method": {
+                        "account": "str",  # Account that owns the entity. Required.
+                        "id": "str",  # Unique identifier of the entity. Required.
+                        "implementation": {
+                            "kind": "str",  # The kind of implementation. Required.
+                            "jupyterNotebook": {
+                                "notebookModule": "str",  # ID of the Module that
+                                  contains the notebook file. This does *not* add the Module as a
+                                  dependency; you must do that separately. Required.
+                                "notebookPath": "str"  # Path to the notebook file
+                                  relative to the Module root directory. Required.
+                            },
+                            "pythonFunction": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python function to call. Required.
+                            },
+                            "pythonRubric": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python Rubric to run. Required.
+                            }
+                        },
+                        "name": "str",  # Descriptive name of the Method. Required.
+                        "output": {
+                            "kind": "str",  # The kind of output artifact. Required.
+                              Known values are: "Measurement" and "SafetyCase".
+                            "measurement": {
+                                "level": "str",  # Measurement level. Required. Known
+                                  values are: "Dataset" and "Instance".
+                                "name": "str",  # Descriptive name of the
+                                  Measurement. Required.
+                                "schema": {
+                                    "arrowSchema": "str",  # The schema in Arrow
+                                      format, encoded with dyff.schema.arrow.encode_schema(). This is
+                                      required, but can be populated from a DyffDataSchema. Required.
+                                    "dyffSchema": {
+                                        "components": [
+                                            "str"  # A list of named dyff
+                                              data schemas. The final schema is the composition of
+                                              these component schemas. Required.
+                                        ],
+                                        "schemaVersion": "0.1"  # Optional.
+                                          Default value is "0.1". The dyff schema version. "0.1"
+                                    },
+                                    "jsonSchema": {}  # Optional. The schema in
+                                      JSON Schema format.
+                                },
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            },
+                            "safetyCase": {
+                                "name": "str",  # Descriptive name of the SafetyCase.
+                                  Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        },
+                        "scope": "str",  # The scope of the Method. The Method produces
+                          outputs that are specific to one entity of the type specified in the .scope
+                          field. Required. Known values are: "InferenceService" and "Evaluation".
+                        "description": "str",  # Optional. Long-form description, interpreted
+                          as Markdown.
+                        "inputs": [
+                            {
+                                "keyword": "str",  # The input is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "kind": "str",  # The kind of input artifact.
+                                  Required. Known values are: "Dataset", "Evaluation", "Measurement",
+                                  and "Report".
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ],
+                        "modules": [
+                            "str"  # Optional. Modules to load into the analysis
+                              environment.
+                        ],
+                        "parameters": [
+                            {
+                                "keyword": "str",  # The parameter is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ]
+                    },
+                    "name": "str",  # Descriptive name of the Measurement. Required.
+                    "schema": {
+                        "arrowSchema": "str",  # The schema in Arrow format, encoded with
+                          dyff.schema.arrow.encode_schema(). This is required, but can be populated
+                          from a DyffDataSchema. Required.
+                        "dyffSchema": {
+                            "components": [
+                                "str"  # A list of named dyff data schemas. The final
+                                  schema is the composition of these component schemas. Required.
+                            ],
+                            "schemaVersion": "0.1"  # Optional. Default value is "0.1".
+                              The dyff schema version. "0.1"
+                        },
+                        "jsonSchema": {}  # Optional. The schema in JSON Schema format.
+                    },
+                    "scope": {
+                        "dataset": "str",  # Optional. Dataset.
+                        "evaluation": "str",  # Optional. Evaluation.
+                        "inferenceService": "str",  # Optional. Inferenceservice.
+                        "model": "str"  # Optional. Model.
+                    },
+                    "annotations": [
+                        {
+                            "key": "str",  # The annotation key. A DNS label with an
+                              optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                              Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
+                              See
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                              for detailed naming rules. Required.
+                            "value": "str"  # The annotation value. An arbitrary string.
+                              Required.
+                        }
+                    ],
+                    "arguments": [
+                        {
+                            "keyword": "str",  # The 'keyword' of the corresponding
+                              ModelParameter. Required.
+                            "value": "str"  # The value of of the argument. Always a
+                              string; implementations are responsible for parsing. Required.
+                        }
+                    ],
+                    "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
+                      (assigned by system).
+                    "description": "str",  # Optional. Long-form description, interpreted as
+                      Markdown.
+                    "inputs": [
+                        {
+                            "entity": "str",  # The ID of the entity whose data should be
+                              made available as 'keyword'. Required.
+                            "keyword": "str"  # The 'keyword' specified for this input in
+                              the MethodSpec. Required.
+                        }
+                    ],
+                    "kind": "Measurement",  # Optional. Default value is "Measurement". Kind.
+                      "Measurement"
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    },
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop(
+            "content_type", _headers.pop("Content-Type", None)
+        )
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        _request = build_measurements_create_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @distributed_trace
+    def get(self, measurement_id: str, **kwargs: Any) -> JSON:
+        # pylint: disable=line-too-long
+        """Get a Measurement by its key.
+
+        Get a Measurement by its key. Raises a 404 error if no entity exists with that key.
+
+        :param measurement_id: Required.
+        :type measurement_id: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "id": "str",  # Unique identifier of the entity. Required.
+                    "level": "str",  # Measurement level. Required. Known values are: "Dataset"
+                      and "Instance".
+                    "method": {
+                        "account": "str",  # Account that owns the entity. Required.
+                        "id": "str",  # Unique identifier of the entity. Required.
+                        "implementation": {
+                            "kind": "str",  # The kind of implementation. Required.
+                            "jupyterNotebook": {
+                                "notebookModule": "str",  # ID of the Module that
+                                  contains the notebook file. This does *not* add the Module as a
+                                  dependency; you must do that separately. Required.
+                                "notebookPath": "str"  # Path to the notebook file
+                                  relative to the Module root directory. Required.
+                            },
+                            "pythonFunction": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python function to call. Required.
+                            },
+                            "pythonRubric": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python Rubric to run. Required.
+                            }
+                        },
+                        "name": "str",  # Descriptive name of the Method. Required.
+                        "output": {
+                            "kind": "str",  # The kind of output artifact. Required.
+                              Known values are: "Measurement" and "SafetyCase".
+                            "measurement": {
+                                "level": "str",  # Measurement level. Required. Known
+                                  values are: "Dataset" and "Instance".
+                                "name": "str",  # Descriptive name of the
+                                  Measurement. Required.
+                                "schema": {
+                                    "arrowSchema": "str",  # The schema in Arrow
+                                      format, encoded with dyff.schema.arrow.encode_schema(). This is
+                                      required, but can be populated from a DyffDataSchema. Required.
+                                    "dyffSchema": {
+                                        "components": [
+                                            "str"  # A list of named dyff
+                                              data schemas. The final schema is the composition of
+                                              these component schemas. Required.
+                                        ],
+                                        "schemaVersion": "0.1"  # Optional.
+                                          Default value is "0.1". The dyff schema version. "0.1"
+                                    },
+                                    "jsonSchema": {}  # Optional. The schema in
+                                      JSON Schema format.
+                                },
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            },
+                            "safetyCase": {
+                                "name": "str",  # Descriptive name of the SafetyCase.
+                                  Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        },
+                        "scope": "str",  # The scope of the Method. The Method produces
+                          outputs that are specific to one entity of the type specified in the .scope
+                          field. Required. Known values are: "InferenceService" and "Evaluation".
+                        "description": "str",  # Optional. Long-form description, interpreted
+                          as Markdown.
+                        "inputs": [
+                            {
+                                "keyword": "str",  # The input is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "kind": "str",  # The kind of input artifact.
+                                  Required. Known values are: "Dataset", "Evaluation", "Measurement",
+                                  and "Report".
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ],
+                        "modules": [
+                            "str"  # Optional. Modules to load into the analysis
+                              environment.
+                        ],
+                        "parameters": [
+                            {
+                                "keyword": "str",  # The parameter is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ]
+                    },
+                    "name": "str",  # Descriptive name of the Measurement. Required.
+                    "schema": {
+                        "arrowSchema": "str",  # The schema in Arrow format, encoded with
+                          dyff.schema.arrow.encode_schema(). This is required, but can be populated
+                          from a DyffDataSchema. Required.
+                        "dyffSchema": {
+                            "components": [
+                                "str"  # A list of named dyff data schemas. The final
+                                  schema is the composition of these component schemas. Required.
+                            ],
+                            "schemaVersion": "0.1"  # Optional. Default value is "0.1".
+                              The dyff schema version. "0.1"
+                        },
+                        "jsonSchema": {}  # Optional. The schema in JSON Schema format.
+                    },
+                    "scope": {
+                        "dataset": "str",  # Optional. Dataset.
+                        "evaluation": "str",  # Optional. Evaluation.
+                        "inferenceService": "str",  # Optional. Inferenceservice.
+                        "model": "str"  # Optional. Model.
+                    },
+                    "annotations": [
+                        {
+                            "key": "str",  # The annotation key. A DNS label with an
+                              optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                              Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
+                              See
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                              for detailed naming rules. Required.
+                            "value": "str"  # The annotation value. An arbitrary string.
+                              Required.
+                        }
+                    ],
+                    "arguments": [
+                        {
+                            "keyword": "str",  # The 'keyword' of the corresponding
+                              ModelParameter. Required.
+                            "value": "str"  # The value of of the argument. Always a
+                              string; implementations are responsible for parsing. Required.
+                        }
+                    ],
+                    "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
+                      (assigned by system).
+                    "description": "str",  # Optional. Long-form description, interpreted as
+                      Markdown.
+                    "inputs": [
+                        {
+                            "entity": "str",  # The ID of the entity whose data should be
+                              made available as 'keyword'. Required.
+                            "keyword": "str"  # The 'keyword' specified for this input in
+                              the MethodSpec. Required.
+                        }
+                    ],
+                    "kind": "Measurement",  # Optional. Default value is "Measurement". Kind.
+                      "Measurement"
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    },
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        _request = build_measurements_get_request(
+            measurement_id=measurement_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @distributed_trace
+    def delete(self, measurement_id: str, **kwargs: Any) -> JSON:
+        """Mark a Measurement for deletion.
+
+        Mark a Measurement for deletion.
+
+        :param measurement_id: Required.
+        :type measurement_id: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        _request = build_measurements_delete_request(
+            measurement_id=measurement_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+
+class MethodsOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~_generated.DyffV0API`'s
+        :attr:`methods` attribute.
+    """
+
+    def __init__(self, *args, **kwargs):
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = (
+            input_args.pop(0) if input_args else kwargs.pop("deserializer")
+        )
+
+    @overload
+    def label(
+        self,
+        method_id: str,
+        body: JSON,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> Union[Any, JSON]:
+        # pylint: disable=line-too-long
+        """Update labels for an existing Method.
+
+        Update labels for an existing Method.
+
+        :param method_id: Required.
+        :type method_id: str
+        :param body: Required.
+        :type body: JSON
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: any or JSON object
+        :rtype: any or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    }
+                }
+
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @overload
+    def label(
+        self,
+        method_id: str,
+        body: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> Union[Any, JSON]:
+        """Update labels for an existing Method.
+
+        Update labels for an existing Method.
+
+        :param method_id: Required.
+        :type method_id: str
+        :param body: Required.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: any or JSON object
+        :rtype: any or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @distributed_trace
+    def label(
+        self, method_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any
+    ) -> Union[Any, JSON]:
+        # pylint: disable=line-too-long
+        """Update labels for an existing Method.
+
+        Update labels for an existing Method.
+
+        :param method_id: Required.
+        :type method_id: str
+        :param body: Is either a JSON type or a IO[bytes] type. Required.
+        :type body: JSON or IO[bytes]
+        :return: any or JSON object
+        :rtype: any or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    }
+                }
+
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop(
+            "content_type", _headers.pop("Content-Type", None)
+        )
+        cls: ClsType[Union[Any, JSON]] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        _request = build_methods_label_request(
+            method_id=method_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(Union[Any, JSON], deserialized), {})  # type: ignore
+
+        return cast(Union[Any, JSON], deserialized)  # type: ignore
+
+    @distributed_trace
+    def query(
+        self,
+        *,
+        id: Optional[str] = None,
+        account: Optional[str] = None,
+        status: Optional[str] = None,
+        reason: Optional[str] = None,
+        labels: Optional[str] = None,
+        name: Optional[str] = None,
+        output_kind: Optional[str] = None,
+        **kwargs: Any,
+    ) -> Union[List[JSON], JSON]:
+        # pylint: disable=line-too-long
+        """Get all Methods matching a query.
+
+        Get all Methods matching a query. The query is a set of equality
+        constraints specified as key-value pairs.
+
+        :keyword id: Default value is None.
+        :paramtype id: str
+        :keyword account: Default value is None.
+        :paramtype account: str
+        :keyword status: Default value is None.
+        :paramtype status: str
+        :keyword reason: Default value is None.
+        :paramtype reason: str
+        :keyword labels: Default value is None.
+        :paramtype labels: str
+        :keyword name: Default value is None.
+        :paramtype name: str
+        :keyword output_kind: Default value is None.
+        :paramtype output_kind: str
+        :return: list of JSON object or JSON object
+        :rtype: list[JSON] or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == [
+                    {
+                        "account": "str",  # Account that owns the entity. Required.
+                        "id": "str",  # Unique identifier of the entity. Required.
+                        "implementation": {
+                            "kind": "str",  # The kind of implementation. Required.
+                            "jupyterNotebook": {
+                                "notebookModule": "str",  # ID of the Module that
+                                  contains the notebook file. This does *not* add the Module as a
+                                  dependency; you must do that separately. Required.
+                                "notebookPath": "str"  # Path to the notebook file
+                                  relative to the Module root directory. Required.
+                            },
+                            "pythonFunction": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python function to call. Required.
+                            },
+                            "pythonRubric": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python Rubric to run. Required.
+                            }
+                        },
+                        "name": "str",  # Descriptive name of the Method. Required.
+                        "output": {
+                            "kind": "str",  # The kind of output artifact. Required.
+                              Known values are: "Measurement" and "SafetyCase".
+                            "measurement": {
+                                "level": "str",  # Measurement level. Required. Known
+                                  values are: "Dataset" and "Instance".
+                                "name": "str",  # Descriptive name of the
+                                  Measurement. Required.
+                                "schema": {
+                                    "arrowSchema": "str",  # The schema in Arrow
+                                      format, encoded with dyff.schema.arrow.encode_schema(). This is
+                                      required, but can be populated from a DyffDataSchema. Required.
+                                    "dyffSchema": {
+                                        "components": [
+                                            "str"  # A list of named dyff
+                                              data schemas. The final schema is the composition of
+                                              these component schemas. Required.
+                                        ],
+                                        "schemaVersion": "0.1"  # Optional.
+                                          Default value is "0.1". The dyff schema version. "0.1"
+                                    },
+                                    "jsonSchema": {}  # Optional. The schema in
+                                      JSON Schema format.
+                                },
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            },
+                            "safetyCase": {
+                                "name": "str",  # Descriptive name of the SafetyCase.
+                                  Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        },
+                        "scope": "str",  # The scope of the Method. The Method produces
+                          outputs that are specific to one entity of the type specified in the .scope
+                          field. Required. Known values are: "InferenceService" and "Evaluation".
+                        "annotations": [
+                            {
+                                "key": "str",  # The annotation key. A DNS label with
+                                  an optional DNS domain prefix. For example: 'my-key',
+                                  'your.com/key_0'. Names prefixed with 'dyff.io/',
+                                  'subdomain.dyff.io/', etc. are reserved.  See
+                                  https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                                  for detailed naming rules. Required.
+                                "value": "str"  # The annotation value. An arbitrary
+                                  string. Required.
+                            }
+                        ],
+                        "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation
+                          time (assigned by system).
+                        "description": "str",  # Optional. Long-form description, interpreted
+                          as Markdown.
+                        "inputs": [
+                            {
+                                "keyword": "str",  # The input is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "kind": "str",  # The kind of input artifact.
+                                  Required. Known values are: "Dataset", "Evaluation", "Measurement",
+                                  and "Report".
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ],
+                        "kind": "Method",  # Optional. Default value is "Method". Kind.
+                          "Method"
+                        "labels": {
+                            "str": "str"  # Optional. A set of key-value labels for the
+                              resource. Used to specify identifying attributes of resources that are
+                              meaningful to users but do not imply semantics in the dyff system.  The
+                              keys are DNS labels with an optional DNS domain prefix. For example:
+                              'my-key', 'your.com/key_0'. Keys prefixed with 'dyff.io/',
+                              'subdomain.dyff.io/', etc. are reserved.  The label values are
+                              alphanumeric characters separated by '.', '-', or '_'.  We follow the
+                              kubernetes label conventions closely. See:
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                        },
+                        "modules": [
+                            "str"  # Optional. Modules to load into the analysis
+                              environment.
+                        ],
+                        "parameters": [
+                            {
+                                "keyword": "str",  # The parameter is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ],
+                        "reason": "str",  # Optional. Reason for current status (assigned by
+                          system).
+                        "schemaVersion": "0.1",  # Optional. Default value is "0.1". The
+                          schema version. "0.1"
+                        "status": "str"  # Optional. Top-level resource status (assigned by
+                          system).
+                    }
+                ]
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
+
+        _request = build_methods_query_request(
+            id=id,
+            account=account,
+            status=status,
+            reason=reason,
+            labels=labels,
+            name=name,
+            output_kind=output_kind,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(Union[List[JSON], JSON], deserialized), {})  # type: ignore
+
+        return cast(Union[List[JSON], JSON], deserialized)  # type: ignore
+
+    @overload
+    def create(
+        self, body: JSON, *, content_type: str = "application/json", **kwargs: Any
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Create a Method.
+
+        Create a Method.
+
+        :param body: Required.
+        :type body: JSON
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "implementation": {
+                        "kind": "str",  # The kind of implementation. Required.
+                        "jupyterNotebook": {
+                            "notebookModule": "str",  # ID of the Module that contains
+                              the notebook file. This does *not* add the Module as a dependency; you
+                              must do that separately. Required.
+                            "notebookPath": "str"  # Path to the notebook file relative
+                              to the Module root directory. Required.
+                        },
+                        "pythonFunction": {
+                            "fullyQualifiedName": "str"  # The fully-qualified name of
+                              the Python function to call. Required.
+                        },
+                        "pythonRubric": {
+                            "fullyQualifiedName": "str"  # The fully-qualified name of
+                              the Python Rubric to run. Required.
+                        }
+                    },
+                    "name": "str",  # Descriptive name of the Method. Required.
+                    "output": {
+                        "kind": "str",  # The kind of output artifact. Required. Known values
+                          are: "Measurement" and "SafetyCase".
+                        "measurement": {
+                            "level": "str",  # Measurement level. Required. Known values
+                              are: "Dataset" and "Instance".
+                            "name": "str",  # Descriptive name of the Measurement.
+                              Required.
+                            "schema": {
+                                "arrowSchema": "str",  # The schema in Arrow format,
+                                  encoded with dyff.schema.arrow.encode_schema(). This is required, but
+                                  can be populated from a DyffDataSchema. Required.
+                                "dyffSchema": {
+                                    "components": [
+                                        "str"  # A list of named dyff data
+                                          schemas. The final schema is the composition of these
+                                          component schemas. Required.
+                                    ],
+                                    "schemaVersion": "0.1"  # Optional. Default
+                                      value is "0.1". The dyff schema version. "0.1"
+                                },
+                                "jsonSchema": {}  # Optional. The schema in JSON
+                                  Schema format.
+                            },
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        },
+                        "safetyCase": {
+                            "name": "str",  # Descriptive name of the SafetyCase.
+                              Required.
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    },
+                    "scope": "str",  # The scope of the Method. The Method produces outputs that
+                      are specific to one entity of the type specified in the .scope field. Required.
+                      Known values are: "InferenceService" and "Evaluation".
+                    "description": "str",  # Optional. Long-form description, interpreted as
+                      Markdown.
+                    "inputs": [
+                        {
+                            "keyword": "str",  # The input is referred to by 'keyword' in
+                              the context of the method implementation. Required.
+                            "kind": "str",  # The kind of input artifact. Required. Known
+                              values are: "Dataset", "Evaluation", "Measurement", and "Report".
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    ],
+                    "modules": [
+                        "str"  # Optional. Modules to load into the analysis environment.
+                    ],
+                    "parameters": [
+                        {
+                            "keyword": "str",  # The parameter is referred to by
+                              'keyword' in the context of the method implementation. Required.
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    ],
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "id": "str",  # Unique identifier of the entity. Required.
+                    "implementation": {
+                        "kind": "str",  # The kind of implementation. Required.
+                        "jupyterNotebook": {
+                            "notebookModule": "str",  # ID of the Module that contains
+                              the notebook file. This does *not* add the Module as a dependency; you
+                              must do that separately. Required.
+                            "notebookPath": "str"  # Path to the notebook file relative
+                              to the Module root directory. Required.
+                        },
+                        "pythonFunction": {
+                            "fullyQualifiedName": "str"  # The fully-qualified name of
+                              the Python function to call. Required.
+                        },
+                        "pythonRubric": {
+                            "fullyQualifiedName": "str"  # The fully-qualified name of
+                              the Python Rubric to run. Required.
+                        }
+                    },
+                    "name": "str",  # Descriptive name of the Method. Required.
+                    "output": {
+                        "kind": "str",  # The kind of output artifact. Required. Known values
+                          are: "Measurement" and "SafetyCase".
+                        "measurement": {
+                            "level": "str",  # Measurement level. Required. Known values
+                              are: "Dataset" and "Instance".
+                            "name": "str",  # Descriptive name of the Measurement.
+                              Required.
+                            "schema": {
+                                "arrowSchema": "str",  # The schema in Arrow format,
+                                  encoded with dyff.schema.arrow.encode_schema(). This is required, but
+                                  can be populated from a DyffDataSchema. Required.
+                                "dyffSchema": {
+                                    "components": [
+                                        "str"  # A list of named dyff data
+                                          schemas. The final schema is the composition of these
+                                          component schemas. Required.
+                                    ],
+                                    "schemaVersion": "0.1"  # Optional. Default
+                                      value is "0.1". The dyff schema version. "0.1"
+                                },
+                                "jsonSchema": {}  # Optional. The schema in JSON
+                                  Schema format.
+                            },
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        },
+                        "safetyCase": {
+                            "name": "str",  # Descriptive name of the SafetyCase.
+                              Required.
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    },
+                    "scope": "str",  # The scope of the Method. The Method produces outputs that
+                      are specific to one entity of the type specified in the .scope field. Required.
+                      Known values are: "InferenceService" and "Evaluation".
+                    "annotations": [
+                        {
+                            "key": "str",  # The annotation key. A DNS label with an
+                              optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                              Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
+                              See
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                              for detailed naming rules. Required.
+                            "value": "str"  # The annotation value. An arbitrary string.
+                              Required.
+                        }
+                    ],
+                    "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
+                      (assigned by system).
+                    "description": "str",  # Optional. Long-form description, interpreted as
+                      Markdown.
+                    "inputs": [
+                        {
+                            "keyword": "str",  # The input is referred to by 'keyword' in
+                              the context of the method implementation. Required.
+                            "kind": "str",  # The kind of input artifact. Required. Known
+                              values are: "Dataset", "Evaluation", "Measurement", and "Report".
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    ],
+                    "kind": "Method",  # Optional. Default value is "Method". Kind. "Method"
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    },
+                    "modules": [
+                        "str"  # Optional. Modules to load into the analysis environment.
+                    ],
+                    "parameters": [
+                        {
+                            "keyword": "str",  # The parameter is referred to by
+                              'keyword' in the context of the method implementation. Required.
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    ],
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @overload
+    def create(
+        self, body: IO[bytes], *, content_type: str = "application/json", **kwargs: Any
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Create a Method.
+
+        Create a Method.
+
+        :param body: Required.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "id": "str",  # Unique identifier of the entity. Required.
+                    "implementation": {
+                        "kind": "str",  # The kind of implementation. Required.
+                        "jupyterNotebook": {
+                            "notebookModule": "str",  # ID of the Module that contains
+                              the notebook file. This does *not* add the Module as a dependency; you
+                              must do that separately. Required.
+                            "notebookPath": "str"  # Path to the notebook file relative
+                              to the Module root directory. Required.
+                        },
+                        "pythonFunction": {
+                            "fullyQualifiedName": "str"  # The fully-qualified name of
+                              the Python function to call. Required.
+                        },
+                        "pythonRubric": {
+                            "fullyQualifiedName": "str"  # The fully-qualified name of
+                              the Python Rubric to run. Required.
+                        }
+                    },
+                    "name": "str",  # Descriptive name of the Method. Required.
+                    "output": {
+                        "kind": "str",  # The kind of output artifact. Required. Known values
+                          are: "Measurement" and "SafetyCase".
+                        "measurement": {
+                            "level": "str",  # Measurement level. Required. Known values
+                              are: "Dataset" and "Instance".
+                            "name": "str",  # Descriptive name of the Measurement.
+                              Required.
+                            "schema": {
+                                "arrowSchema": "str",  # The schema in Arrow format,
+                                  encoded with dyff.schema.arrow.encode_schema(). This is required, but
+                                  can be populated from a DyffDataSchema. Required.
+                                "dyffSchema": {
+                                    "components": [
+                                        "str"  # A list of named dyff data
+                                          schemas. The final schema is the composition of these
+                                          component schemas. Required.
+                                    ],
+                                    "schemaVersion": "0.1"  # Optional. Default
+                                      value is "0.1". The dyff schema version. "0.1"
+                                },
+                                "jsonSchema": {}  # Optional. The schema in JSON
+                                  Schema format.
+                            },
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        },
+                        "safetyCase": {
+                            "name": "str",  # Descriptive name of the SafetyCase.
+                              Required.
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    },
+                    "scope": "str",  # The scope of the Method. The Method produces outputs that
+                      are specific to one entity of the type specified in the .scope field. Required.
+                      Known values are: "InferenceService" and "Evaluation".
+                    "annotations": [
+                        {
+                            "key": "str",  # The annotation key. A DNS label with an
+                              optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                              Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
+                              See
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                              for detailed naming rules. Required.
+                            "value": "str"  # The annotation value. An arbitrary string.
+                              Required.
+                        }
+                    ],
+                    "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
+                      (assigned by system).
+                    "description": "str",  # Optional. Long-form description, interpreted as
+                      Markdown.
+                    "inputs": [
+                        {
+                            "keyword": "str",  # The input is referred to by 'keyword' in
+                              the context of the method implementation. Required.
+                            "kind": "str",  # The kind of input artifact. Required. Known
+                              values are: "Dataset", "Evaluation", "Measurement", and "Report".
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    ],
+                    "kind": "Method",  # Optional. Default value is "Method". Kind. "Method"
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    },
+                    "modules": [
+                        "str"  # Optional. Modules to load into the analysis environment.
+                    ],
+                    "parameters": [
+                        {
+                            "keyword": "str",  # The parameter is referred to by
+                              'keyword' in the context of the method implementation. Required.
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    ],
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @distributed_trace
+    def create(self, body: Union[JSON, IO[bytes]], **kwargs: Any) -> JSON:
+        # pylint: disable=line-too-long
+        """Create a Method.
+
+        Create a Method.
+
+        :param body: Is either a JSON type or a IO[bytes] type. Required.
+        :type body: JSON or IO[bytes]
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "implementation": {
+                        "kind": "str",  # The kind of implementation. Required.
+                        "jupyterNotebook": {
+                            "notebookModule": "str",  # ID of the Module that contains
+                              the notebook file. This does *not* add the Module as a dependency; you
+                              must do that separately. Required.
+                            "notebookPath": "str"  # Path to the notebook file relative
+                              to the Module root directory. Required.
+                        },
+                        "pythonFunction": {
+                            "fullyQualifiedName": "str"  # The fully-qualified name of
+                              the Python function to call. Required.
+                        },
+                        "pythonRubric": {
+                            "fullyQualifiedName": "str"  # The fully-qualified name of
+                              the Python Rubric to run. Required.
+                        }
+                    },
+                    "name": "str",  # Descriptive name of the Method. Required.
+                    "output": {
+                        "kind": "str",  # The kind of output artifact. Required. Known values
+                          are: "Measurement" and "SafetyCase".
+                        "measurement": {
+                            "level": "str",  # Measurement level. Required. Known values
+                              are: "Dataset" and "Instance".
+                            "name": "str",  # Descriptive name of the Measurement.
+                              Required.
+                            "schema": {
+                                "arrowSchema": "str",  # The schema in Arrow format,
+                                  encoded with dyff.schema.arrow.encode_schema(). This is required, but
+                                  can be populated from a DyffDataSchema. Required.
+                                "dyffSchema": {
+                                    "components": [
+                                        "str"  # A list of named dyff data
+                                          schemas. The final schema is the composition of these
+                                          component schemas. Required.
+                                    ],
+                                    "schemaVersion": "0.1"  # Optional. Default
+                                      value is "0.1". The dyff schema version. "0.1"
+                                },
+                                "jsonSchema": {}  # Optional. The schema in JSON
+                                  Schema format.
+                            },
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        },
+                        "safetyCase": {
+                            "name": "str",  # Descriptive name of the SafetyCase.
+                              Required.
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    },
+                    "scope": "str",  # The scope of the Method. The Method produces outputs that
+                      are specific to one entity of the type specified in the .scope field. Required.
+                      Known values are: "InferenceService" and "Evaluation".
+                    "description": "str",  # Optional. Long-form description, interpreted as
+                      Markdown.
+                    "inputs": [
+                        {
+                            "keyword": "str",  # The input is referred to by 'keyword' in
+                              the context of the method implementation. Required.
+                            "kind": "str",  # The kind of input artifact. Required. Known
+                              values are: "Dataset", "Evaluation", "Measurement", and "Report".
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    ],
+                    "modules": [
+                        "str"  # Optional. Modules to load into the analysis environment.
+                    ],
+                    "parameters": [
+                        {
+                            "keyword": "str",  # The parameter is referred to by
+                              'keyword' in the context of the method implementation. Required.
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    ],
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "id": "str",  # Unique identifier of the entity. Required.
+                    "implementation": {
+                        "kind": "str",  # The kind of implementation. Required.
+                        "jupyterNotebook": {
+                            "notebookModule": "str",  # ID of the Module that contains
+                              the notebook file. This does *not* add the Module as a dependency; you
+                              must do that separately. Required.
+                            "notebookPath": "str"  # Path to the notebook file relative
+                              to the Module root directory. Required.
+                        },
+                        "pythonFunction": {
+                            "fullyQualifiedName": "str"  # The fully-qualified name of
+                              the Python function to call. Required.
+                        },
+                        "pythonRubric": {
+                            "fullyQualifiedName": "str"  # The fully-qualified name of
+                              the Python Rubric to run. Required.
+                        }
+                    },
+                    "name": "str",  # Descriptive name of the Method. Required.
+                    "output": {
+                        "kind": "str",  # The kind of output artifact. Required. Known values
+                          are: "Measurement" and "SafetyCase".
+                        "measurement": {
+                            "level": "str",  # Measurement level. Required. Known values
+                              are: "Dataset" and "Instance".
+                            "name": "str",  # Descriptive name of the Measurement.
+                              Required.
+                            "schema": {
+                                "arrowSchema": "str",  # The schema in Arrow format,
+                                  encoded with dyff.schema.arrow.encode_schema(). This is required, but
+                                  can be populated from a DyffDataSchema. Required.
+                                "dyffSchema": {
+                                    "components": [
+                                        "str"  # A list of named dyff data
+                                          schemas. The final schema is the composition of these
+                                          component schemas. Required.
+                                    ],
+                                    "schemaVersion": "0.1"  # Optional. Default
+                                      value is "0.1". The dyff schema version. "0.1"
+                                },
+                                "jsonSchema": {}  # Optional. The schema in JSON
+                                  Schema format.
+                            },
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        },
+                        "safetyCase": {
+                            "name": "str",  # Descriptive name of the SafetyCase.
+                              Required.
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    },
+                    "scope": "str",  # The scope of the Method. The Method produces outputs that
+                      are specific to one entity of the type specified in the .scope field. Required.
+                      Known values are: "InferenceService" and "Evaluation".
+                    "annotations": [
+                        {
+                            "key": "str",  # The annotation key. A DNS label with an
+                              optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                              Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
+                              See
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                              for detailed naming rules. Required.
+                            "value": "str"  # The annotation value. An arbitrary string.
+                              Required.
+                        }
+                    ],
+                    "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
+                      (assigned by system).
+                    "description": "str",  # Optional. Long-form description, interpreted as
+                      Markdown.
+                    "inputs": [
+                        {
+                            "keyword": "str",  # The input is referred to by 'keyword' in
+                              the context of the method implementation. Required.
+                            "kind": "str",  # The kind of input artifact. Required. Known
+                              values are: "Dataset", "Evaluation", "Measurement", and "Report".
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    ],
+                    "kind": "Method",  # Optional. Default value is "Method". Kind. "Method"
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    },
+                    "modules": [
+                        "str"  # Optional. Modules to load into the analysis environment.
+                    ],
+                    "parameters": [
+                        {
+                            "keyword": "str",  # The parameter is referred to by
+                              'keyword' in the context of the method implementation. Required.
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    ],
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop(
+            "content_type", _headers.pop("Content-Type", None)
+        )
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        _request = build_methods_create_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @distributed_trace
+    def get(self, method_id: str, **kwargs: Any) -> JSON:
+        # pylint: disable=line-too-long
+        """Get a Method by its key.
+
+        Get a Method by its key. Raises a 404 error if no entity exists with that key.
+
+        :param method_id: Required.
+        :type method_id: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "id": "str",  # Unique identifier of the entity. Required.
+                    "implementation": {
+                        "kind": "str",  # The kind of implementation. Required.
+                        "jupyterNotebook": {
+                            "notebookModule": "str",  # ID of the Module that contains
+                              the notebook file. This does *not* add the Module as a dependency; you
+                              must do that separately. Required.
+                            "notebookPath": "str"  # Path to the notebook file relative
+                              to the Module root directory. Required.
+                        },
+                        "pythonFunction": {
+                            "fullyQualifiedName": "str"  # The fully-qualified name of
+                              the Python function to call. Required.
+                        },
+                        "pythonRubric": {
+                            "fullyQualifiedName": "str"  # The fully-qualified name of
+                              the Python Rubric to run. Required.
+                        }
+                    },
+                    "name": "str",  # Descriptive name of the Method. Required.
+                    "output": {
+                        "kind": "str",  # The kind of output artifact. Required. Known values
+                          are: "Measurement" and "SafetyCase".
+                        "measurement": {
+                            "level": "str",  # Measurement level. Required. Known values
+                              are: "Dataset" and "Instance".
+                            "name": "str",  # Descriptive name of the Measurement.
+                              Required.
+                            "schema": {
+                                "arrowSchema": "str",  # The schema in Arrow format,
+                                  encoded with dyff.schema.arrow.encode_schema(). This is required, but
+                                  can be populated from a DyffDataSchema. Required.
+                                "dyffSchema": {
+                                    "components": [
+                                        "str"  # A list of named dyff data
+                                          schemas. The final schema is the composition of these
+                                          component schemas. Required.
+                                    ],
+                                    "schemaVersion": "0.1"  # Optional. Default
+                                      value is "0.1". The dyff schema version. "0.1"
+                                },
+                                "jsonSchema": {}  # Optional. The schema in JSON
+                                  Schema format.
+                            },
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        },
+                        "safetyCase": {
+                            "name": "str",  # Descriptive name of the SafetyCase.
+                              Required.
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    },
+                    "scope": "str",  # The scope of the Method. The Method produces outputs that
+                      are specific to one entity of the type specified in the .scope field. Required.
+                      Known values are: "InferenceService" and "Evaluation".
+                    "annotations": [
+                        {
+                            "key": "str",  # The annotation key. A DNS label with an
+                              optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                              Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
+                              See
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                              for detailed naming rules. Required.
+                            "value": "str"  # The annotation value. An arbitrary string.
+                              Required.
+                        }
+                    ],
+                    "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
+                      (assigned by system).
+                    "description": "str",  # Optional. Long-form description, interpreted as
+                      Markdown.
+                    "inputs": [
+                        {
+                            "keyword": "str",  # The input is referred to by 'keyword' in
+                              the context of the method implementation. Required.
+                            "kind": "str",  # The kind of input artifact. Required. Known
+                              values are: "Dataset", "Evaluation", "Measurement", and "Report".
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    ],
+                    "kind": "Method",  # Optional. Default value is "Method". Kind. "Method"
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    },
+                    "modules": [
+                        "str"  # Optional. Modules to load into the analysis environment.
+                    ],
+                    "parameters": [
+                        {
+                            "keyword": "str",  # The parameter is referred to by
+                              'keyword' in the context of the method implementation. Required.
+                            "description": "str"  # Optional. Long-form description,
+                              interpreted as Markdown.
+                        }
+                    ],
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        _request = build_methods_get_request(
+            method_id=method_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @distributed_trace
+    def delete(self, method_id: str, **kwargs: Any) -> JSON:
+        """Mark a Method for deletion.
+
+        Mark a Method for deletion.
+
+        :param method_id: Required.
+        :type method_id: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        _request = build_methods_delete_request(
+            method_id=method_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+
 class ModelsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~_generated.DyffAPI`'s
+        :class:`~_generated.DyffV0API`'s
         :attr:`models` attribute.
     """
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
@@ -9288,15 +12685,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9507,15 +12904,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10086,15 +13483,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10277,15 +13674,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10364,15 +13761,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10425,15 +13822,15 @@
 
 class ModulesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~_generated.DyffAPI`'s
+        :class:`~_generated.DyffV0API`'s
         :attr:`modules` attribute.
     """
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
@@ -10582,15 +13979,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10751,15 +14148,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11080,15 +14477,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11221,15 +14618,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11308,15 +14705,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11401,15 +14798,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11484,15 +14881,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11545,15 +14942,15 @@
 
 class ReportsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~_generated.DyffAPI`'s
+        :class:`~_generated.DyffV0API`'s
         :attr:`reports` attribute.
     """
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
@@ -11702,15 +15099,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -11918,14 +15315,18 @@
                               'subdomain.dyff.io/', etc. are reserved.  The label values are
                               alphanumeric characters separated by '.', '-', or '_'.  We follow the
                               kubernetes label conventions closely. See:
                               https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                         },
                         "model": "str",  # Optional. The model backing the inference service,
                           if applicable.
+                        "modules": [
+                            "str"  # Optional. Additional modules to load into the report
+                              environment.
+                        ],
                         "reason": "str",  # Optional. Reason for current status (assigned by
                           system).
                         "schemaVersion": "0.1",  # Optional. Default value is "0.1". The
                           schema version. "0.1"
                         "status": "str"  # Optional. Top-level resource status (assigned by
                           system).
                     }
@@ -11939,15 +15340,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12032,14 +15433,18 @@
                     "account": "str",  # Account that owns the entity. Required.
                     "evaluation": "str",  # The evaluation (and corresponding output data) to run
                       the report on. Required.
                     "rubric": "str",  # The scoring rubric to apply (e.g.,
                       'classification.TopKAccuracy'). Required.
                     "datasetView": {},
                     "evaluationView": {},
+                    "modules": [
+                        "str"  # Optional. Additional modules to load into the report
+                          environment.
+                    ],
                     "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
                       version. "0.1"
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "account": "str",  # Account that owns the entity. Required.
@@ -12132,14 +15537,18 @@
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                     },
                     "model": "str",  # Optional. The model backing the inference service, if
                       applicable.
+                    "modules": [
+                        "str"  # Optional. Additional modules to load into the report
+                          environment.
+                    ],
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
                     "status": "str"  # Optional. Top-level resource status (assigned by system).
                 }
                 # response body for status code(s): 422
                 response == {
@@ -12268,14 +15677,18 @@
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                     },
                     "model": "str",  # Optional. The model backing the inference service, if
                       applicable.
+                    "modules": [
+                        "str"  # Optional. Additional modules to load into the report
+                          environment.
+                    ],
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
                     "status": "str"  # Optional. Top-level resource status (assigned by system).
                 }
                 # response body for status code(s): 422
                 response == {
@@ -12312,14 +15725,18 @@
                     "account": "str",  # Account that owns the entity. Required.
                     "evaluation": "str",  # The evaluation (and corresponding output data) to run
                       the report on. Required.
                     "rubric": "str",  # The scoring rubric to apply (e.g.,
                       'classification.TopKAccuracy'). Required.
                     "datasetView": {},
                     "evaluationView": {},
+                    "modules": [
+                        "str"  # Optional. Additional modules to load into the report
+                          environment.
+                    ],
                     "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
                       version. "0.1"
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "account": "str",  # Account that owns the entity. Required.
@@ -12412,14 +15829,18 @@
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                     },
                     "model": "str",  # Optional. The model backing the inference service, if
                       applicable.
+                    "modules": [
+                        "str"  # Optional. Additional modules to load into the report
+                          environment.
+                    ],
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
                     "status": "str"  # Optional. Top-level resource status (assigned by system).
                 }
                 # response body for status code(s): 422
                 response == {
@@ -12430,15 +15851,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12609,14 +16030,18 @@
                           Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                     },
                     "model": "str",  # Optional. The model backing the inference service, if
                       applicable.
+                    "modules": [
+                        "str"  # Optional. Additional modules to load into the report
+                          environment.
+                    ],
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
                     "status": "str"  # Optional. Top-level resource status (assigned by system).
                 }
                 # response body for status code(s): 422
                 response == {
@@ -12627,15 +16052,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12714,15 +16139,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12776,15 +16201,15 @@
     def data(self, report_id: str, **kwargs: Any) -> Union[Iterator[bytes], JSON]:
         """Get the raw data for the Report.
 
         Get the raw data for the Report.
 
         :param report_id: Required.
         :type report_id: str
-        :return: Iterator of the response bytes or JSON object or None
+        :return: Iterator[bytes] or JSON object or None
         :rtype: Iterator[bytes] or JSON or None
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 422
@@ -12796,15 +16221,15 @@
                             ],
                             "msg": "str",  # Message. Required.
                             "type": "str"  # Error Type. Required.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -12844,7 +16269,1493 @@
         if response.status_code == 422:
             deserialized = response.iter_bytes()
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
+
+
+class SafetycasesOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~_generated.DyffV0API`'s
+        :attr:`safetycases` attribute.
+    """
+
+    def __init__(self, *args, **kwargs):
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = (
+            input_args.pop(0) if input_args else kwargs.pop("deserializer")
+        )
+
+    @overload
+    def label(
+        self,
+        safetycase_id: str,
+        body: JSON,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> Union[Any, JSON]:
+        # pylint: disable=line-too-long
+        """Update labels for an existing SafetyCase.
+
+        Update labels for an existing SafetyCase.
+
+        :param safetycase_id: Required.
+        :type safetycase_id: str
+        :param body: Required.
+        :type body: JSON
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: any or JSON object
+        :rtype: any or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    }
+                }
+
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @overload
+    def label(
+        self,
+        safetycase_id: str,
+        body: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> Union[Any, JSON]:
+        """Update labels for an existing SafetyCase.
+
+        Update labels for an existing SafetyCase.
+
+        :param safetycase_id: Required.
+        :type safetycase_id: str
+        :param body: Required.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: any or JSON object
+        :rtype: any or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @distributed_trace
+    def label(
+        self, safetycase_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any
+    ) -> Union[Any, JSON]:
+        # pylint: disable=line-too-long
+        """Update labels for an existing SafetyCase.
+
+        Update labels for an existing SafetyCase.
+
+        :param safetycase_id: Required.
+        :type safetycase_id: str
+        :param body: Is either a JSON type or a IO[bytes] type. Required.
+        :type body: JSON or IO[bytes]
+        :return: any or JSON object
+        :rtype: any or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    }
+                }
+
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop(
+            "content_type", _headers.pop("Content-Type", None)
+        )
+        cls: ClsType[Union[Any, JSON]] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        _request = build_safetycases_label_request(
+            safetycase_id=safetycase_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(Union[Any, JSON], deserialized), {})  # type: ignore
+
+        return cast(Union[Any, JSON], deserialized)  # type: ignore
+
+    @distributed_trace
+    def query(
+        self,
+        *,
+        id: Optional[str] = None,
+        account: Optional[str] = None,
+        status: Optional[str] = None,
+        reason: Optional[str] = None,
+        labels: Optional[str] = None,
+        analysis: Optional[str] = None,
+        method: Optional[str] = None,
+        method_name: Optional[str] = None,
+        inputs_any_of: Optional[str] = None,
+        **kwargs: Any,
+    ) -> Union[List[JSON], JSON]:
+        # pylint: disable=line-too-long
+        """Get all SafetyCase entities matching a query.
+
+        Get all SafetyCase entities matching a query. The query is a set of equality
+        constraints specified as key-value pairs.
+
+        :keyword id: Default value is None.
+        :paramtype id: str
+        :keyword account: Default value is None.
+        :paramtype account: str
+        :keyword status: Default value is None.
+        :paramtype status: str
+        :keyword reason: Default value is None.
+        :paramtype reason: str
+        :keyword labels: Default value is None.
+        :paramtype labels: str
+        :keyword analysis: Default value is None.
+        :paramtype analysis: str
+        :keyword method: Default value is None.
+        :paramtype method: str
+        :keyword method_name: Default value is None.
+        :paramtype method_name: str
+        :keyword inputs_any_of: Default value is None.
+        :paramtype inputs_any_of: str
+        :return: list of JSON object or JSON object
+        :rtype: list[JSON] or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == [
+                    {
+                        "account": "str",  # Account that owns the entity. Required.
+                        "id": "str",  # Unique identifier of the entity. Required.
+                        "method": {
+                            "account": "str",  # Account that owns the entity. Required.
+                            "id": "str",  # Unique identifier of the entity. Required.
+                            "implementation": {
+                                "kind": "str",  # The kind of implementation.
+                                  Required.
+                                "jupyterNotebook": {
+                                    "notebookModule": "str",  # ID of the Module
+                                      that contains the notebook file. This does *not* add the Module
+                                      as a dependency; you must do that separately. Required.
+                                    "notebookPath": "str"  # Path to the notebook
+                                      file relative to the Module root directory. Required.
+                                },
+                                "pythonFunction": {
+                                    "fullyQualifiedName": "str"  # The
+                                      fully-qualified name of the Python function to call. Required.
+                                },
+                                "pythonRubric": {
+                                    "fullyQualifiedName": "str"  # The
+                                      fully-qualified name of the Python Rubric to run. Required.
+                                }
+                            },
+                            "name": "str",  # Descriptive name of the Method. Required.
+                            "output": {
+                                "kind": "str",  # The kind of output artifact.
+                                  Required. Known values are: "Measurement" and "SafetyCase".
+                                "measurement": {
+                                    "level": "str",  # Measurement level.
+                                      Required. Known values are: "Dataset" and "Instance".
+                                    "name": "str",  # Descriptive name of the
+                                      Measurement. Required.
+                                    "schema": {
+                                        "arrowSchema": "str",  # The schema
+                                          in Arrow format, encoded with
+                                          dyff.schema.arrow.encode_schema(). This is required, but can
+                                          be populated from a DyffDataSchema. Required.
+                                        "dyffSchema": {
+                                            "components": [
+                                                "str"  # A list of
+                                                  named dyff data schemas. The final schema is the
+                                                  composition of these component schemas. Required.
+                                            ],
+                                            "schemaVersion": "0.1"  #
+                                              Optional. Default value is "0.1". The dyff schema
+                                              version. "0.1"
+                                        },
+                                        "jsonSchema": {}  # Optional. The
+                                          schema in JSON Schema format.
+                                    },
+                                    "description": "str"  # Optional. Long-form
+                                      description, interpreted as Markdown.
+                                },
+                                "safetyCase": {
+                                    "name": "str",  # Descriptive name of the
+                                      SafetyCase. Required.
+                                    "description": "str"  # Optional. Long-form
+                                      description, interpreted as Markdown.
+                                }
+                            },
+                            "scope": "str",  # The scope of the Method. The Method
+                              produces outputs that are specific to one entity of the type specified in
+                              the .scope field. Required. Known values are: "InferenceService" and
+                              "Evaluation".
+                            "description": "str",  # Optional. Long-form description,
+                              interpreted as Markdown.
+                            "inputs": [
+                                {
+                                    "keyword": "str",  # The input is referred to
+                                      by 'keyword' in the context of the method implementation.
+                                      Required.
+                                    "kind": "str",  # The kind of input artifact.
+                                      Required. Known values are: "Dataset", "Evaluation",
+                                      "Measurement", and "Report".
+                                    "description": "str"  # Optional. Long-form
+                                      description, interpreted as Markdown.
+                                }
+                            ],
+                            "modules": [
+                                "str"  # Optional. Modules to load into the analysis
+                                  environment.
+                            ],
+                            "parameters": [
+                                {
+                                    "keyword": "str",  # The parameter is
+                                      referred to by 'keyword' in the context of the method
+                                      implementation. Required.
+                                    "description": "str"  # Optional. Long-form
+                                      description, interpreted as Markdown.
+                                }
+                            ]
+                        },
+                        "name": "str",  # Descriptive name of the SafetyCase. Required.
+                        "scope": {
+                            "dataset": "str",  # Optional. Dataset.
+                            "evaluation": "str",  # Optional. Evaluation.
+                            "inferenceService": "str",  # Optional. Inferenceservice.
+                            "model": "str"  # Optional. Model.
+                        },
+                        "annotations": [
+                            {
+                                "key": "str",  # The annotation key. A DNS label with
+                                  an optional DNS domain prefix. For example: 'my-key',
+                                  'your.com/key_0'. Names prefixed with 'dyff.io/',
+                                  'subdomain.dyff.io/', etc. are reserved.  See
+                                  https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                                  for detailed naming rules. Required.
+                                "value": "str"  # The annotation value. An arbitrary
+                                  string. Required.
+                            }
+                        ],
+                        "arguments": [
+                            {
+                                "keyword": "str",  # The 'keyword' of the
+                                  corresponding ModelParameter. Required.
+                                "value": "str"  # The value of of the argument.
+                                  Always a string; implementations are responsible for parsing.
+                                  Required.
+                            }
+                        ],
+                        "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation
+                          time (assigned by system).
+                        "description": "str",  # Optional. Long-form description, interpreted
+                          as Markdown.
+                        "inputs": [
+                            {
+                                "entity": "str",  # The ID of the entity whose data
+                                  should be made available as 'keyword'. Required.
+                                "keyword": "str"  # The 'keyword' specified for this
+                                  input in the MethodSpec. Required.
+                            }
+                        ],
+                        "kind": "SafetyCase",  # Optional. Default value is "SafetyCase".
+                          Kind. "SafetyCase"
+                        "labels": {
+                            "str": "str"  # Optional. A set of key-value labels for the
+                              resource. Used to specify identifying attributes of resources that are
+                              meaningful to users but do not imply semantics in the dyff system.  The
+                              keys are DNS labels with an optional DNS domain prefix. For example:
+                              'my-key', 'your.com/key_0'. Keys prefixed with 'dyff.io/',
+                              'subdomain.dyff.io/', etc. are reserved.  The label values are
+                              alphanumeric characters separated by '.', '-', or '_'.  We follow the
+                              kubernetes label conventions closely. See:
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                        },
+                        "reason": "str",  # Optional. Reason for current status (assigned by
+                          system).
+                        "schemaVersion": "0.1",  # Optional. Default value is "0.1". The
+                          schema version. "0.1"
+                        "status": "str"  # Optional. Top-level resource status (assigned by
+                          system).
+                    }
+                ]
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
+
+        _request = build_safetycases_query_request(
+            id=id,
+            account=account,
+            status=status,
+            reason=reason,
+            labels=labels,
+            analysis=analysis,
+            method=method,
+            method_name=method_name,
+            inputs_any_of=inputs_any_of,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(Union[List[JSON], JSON], deserialized), {})  # type: ignore
+
+        return cast(Union[List[JSON], JSON], deserialized)  # type: ignore
+
+    @overload
+    def create(
+        self, body: JSON, *, content_type: str = "application/json", **kwargs: Any
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Create a SafetyCase.
+
+        Create a SafetyCase.
+
+        :param body: Required.
+        :type body: JSON
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "method": "str",  # Method ID. Required.
+                    "scope": {
+                        "dataset": "str",  # Optional. Dataset.
+                        "evaluation": "str",  # Optional. Evaluation.
+                        "inferenceService": "str",  # Optional. Inferenceservice.
+                        "model": "str"  # Optional. Model.
+                    },
+                    "arguments": [
+                        {
+                            "keyword": "str",  # The 'keyword' of the corresponding
+                              ModelParameter. Required.
+                            "value": "str"  # The value of of the argument. Always a
+                              string; implementations are responsible for parsing. Required.
+                        }
+                    ],
+                    "inputs": [
+                        {
+                            "entity": "str",  # The ID of the entity whose data should be
+                              made available as 'keyword'. Required.
+                            "keyword": "str"  # The 'keyword' specified for this input in
+                              the MethodSpec. Required.
+                        }
+                    ],
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "id": "str",  # Unique identifier of the entity. Required.
+                    "method": {
+                        "account": "str",  # Account that owns the entity. Required.
+                        "id": "str",  # Unique identifier of the entity. Required.
+                        "implementation": {
+                            "kind": "str",  # The kind of implementation. Required.
+                            "jupyterNotebook": {
+                                "notebookModule": "str",  # ID of the Module that
+                                  contains the notebook file. This does *not* add the Module as a
+                                  dependency; you must do that separately. Required.
+                                "notebookPath": "str"  # Path to the notebook file
+                                  relative to the Module root directory. Required.
+                            },
+                            "pythonFunction": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python function to call. Required.
+                            },
+                            "pythonRubric": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python Rubric to run. Required.
+                            }
+                        },
+                        "name": "str",  # Descriptive name of the Method. Required.
+                        "output": {
+                            "kind": "str",  # The kind of output artifact. Required.
+                              Known values are: "Measurement" and "SafetyCase".
+                            "measurement": {
+                                "level": "str",  # Measurement level. Required. Known
+                                  values are: "Dataset" and "Instance".
+                                "name": "str",  # Descriptive name of the
+                                  Measurement. Required.
+                                "schema": {
+                                    "arrowSchema": "str",  # The schema in Arrow
+                                      format, encoded with dyff.schema.arrow.encode_schema(). This is
+                                      required, but can be populated from a DyffDataSchema. Required.
+                                    "dyffSchema": {
+                                        "components": [
+                                            "str"  # A list of named dyff
+                                              data schemas. The final schema is the composition of
+                                              these component schemas. Required.
+                                        ],
+                                        "schemaVersion": "0.1"  # Optional.
+                                          Default value is "0.1". The dyff schema version. "0.1"
+                                    },
+                                    "jsonSchema": {}  # Optional. The schema in
+                                      JSON Schema format.
+                                },
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            },
+                            "safetyCase": {
+                                "name": "str",  # Descriptive name of the SafetyCase.
+                                  Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        },
+                        "scope": "str",  # The scope of the Method. The Method produces
+                          outputs that are specific to one entity of the type specified in the .scope
+                          field. Required. Known values are: "InferenceService" and "Evaluation".
+                        "description": "str",  # Optional. Long-form description, interpreted
+                          as Markdown.
+                        "inputs": [
+                            {
+                                "keyword": "str",  # The input is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "kind": "str",  # The kind of input artifact.
+                                  Required. Known values are: "Dataset", "Evaluation", "Measurement",
+                                  and "Report".
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ],
+                        "modules": [
+                            "str"  # Optional. Modules to load into the analysis
+                              environment.
+                        ],
+                        "parameters": [
+                            {
+                                "keyword": "str",  # The parameter is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ]
+                    },
+                    "name": "str",  # Descriptive name of the SafetyCase. Required.
+                    "scope": {
+                        "dataset": "str",  # Optional. Dataset.
+                        "evaluation": "str",  # Optional. Evaluation.
+                        "inferenceService": "str",  # Optional. Inferenceservice.
+                        "model": "str"  # Optional. Model.
+                    },
+                    "annotations": [
+                        {
+                            "key": "str",  # The annotation key. A DNS label with an
+                              optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                              Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
+                              See
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                              for detailed naming rules. Required.
+                            "value": "str"  # The annotation value. An arbitrary string.
+                              Required.
+                        }
+                    ],
+                    "arguments": [
+                        {
+                            "keyword": "str",  # The 'keyword' of the corresponding
+                              ModelParameter. Required.
+                            "value": "str"  # The value of of the argument. Always a
+                              string; implementations are responsible for parsing. Required.
+                        }
+                    ],
+                    "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
+                      (assigned by system).
+                    "description": "str",  # Optional. Long-form description, interpreted as
+                      Markdown.
+                    "inputs": [
+                        {
+                            "entity": "str",  # The ID of the entity whose data should be
+                              made available as 'keyword'. Required.
+                            "keyword": "str"  # The 'keyword' specified for this input in
+                              the MethodSpec. Required.
+                        }
+                    ],
+                    "kind": "SafetyCase",  # Optional. Default value is "SafetyCase". Kind.
+                      "SafetyCase"
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    },
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @overload
+    def create(
+        self, body: IO[bytes], *, content_type: str = "application/json", **kwargs: Any
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Create a SafetyCase.
+
+        Create a SafetyCase.
+
+        :param body: Required.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "id": "str",  # Unique identifier of the entity. Required.
+                    "method": {
+                        "account": "str",  # Account that owns the entity. Required.
+                        "id": "str",  # Unique identifier of the entity. Required.
+                        "implementation": {
+                            "kind": "str",  # The kind of implementation. Required.
+                            "jupyterNotebook": {
+                                "notebookModule": "str",  # ID of the Module that
+                                  contains the notebook file. This does *not* add the Module as a
+                                  dependency; you must do that separately. Required.
+                                "notebookPath": "str"  # Path to the notebook file
+                                  relative to the Module root directory. Required.
+                            },
+                            "pythonFunction": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python function to call. Required.
+                            },
+                            "pythonRubric": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python Rubric to run. Required.
+                            }
+                        },
+                        "name": "str",  # Descriptive name of the Method. Required.
+                        "output": {
+                            "kind": "str",  # The kind of output artifact. Required.
+                              Known values are: "Measurement" and "SafetyCase".
+                            "measurement": {
+                                "level": "str",  # Measurement level. Required. Known
+                                  values are: "Dataset" and "Instance".
+                                "name": "str",  # Descriptive name of the
+                                  Measurement. Required.
+                                "schema": {
+                                    "arrowSchema": "str",  # The schema in Arrow
+                                      format, encoded with dyff.schema.arrow.encode_schema(). This is
+                                      required, but can be populated from a DyffDataSchema. Required.
+                                    "dyffSchema": {
+                                        "components": [
+                                            "str"  # A list of named dyff
+                                              data schemas. The final schema is the composition of
+                                              these component schemas. Required.
+                                        ],
+                                        "schemaVersion": "0.1"  # Optional.
+                                          Default value is "0.1". The dyff schema version. "0.1"
+                                    },
+                                    "jsonSchema": {}  # Optional. The schema in
+                                      JSON Schema format.
+                                },
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            },
+                            "safetyCase": {
+                                "name": "str",  # Descriptive name of the SafetyCase.
+                                  Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        },
+                        "scope": "str",  # The scope of the Method. The Method produces
+                          outputs that are specific to one entity of the type specified in the .scope
+                          field. Required. Known values are: "InferenceService" and "Evaluation".
+                        "description": "str",  # Optional. Long-form description, interpreted
+                          as Markdown.
+                        "inputs": [
+                            {
+                                "keyword": "str",  # The input is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "kind": "str",  # The kind of input artifact.
+                                  Required. Known values are: "Dataset", "Evaluation", "Measurement",
+                                  and "Report".
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ],
+                        "modules": [
+                            "str"  # Optional. Modules to load into the analysis
+                              environment.
+                        ],
+                        "parameters": [
+                            {
+                                "keyword": "str",  # The parameter is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ]
+                    },
+                    "name": "str",  # Descriptive name of the SafetyCase. Required.
+                    "scope": {
+                        "dataset": "str",  # Optional. Dataset.
+                        "evaluation": "str",  # Optional. Evaluation.
+                        "inferenceService": "str",  # Optional. Inferenceservice.
+                        "model": "str"  # Optional. Model.
+                    },
+                    "annotations": [
+                        {
+                            "key": "str",  # The annotation key. A DNS label with an
+                              optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                              Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
+                              See
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                              for detailed naming rules. Required.
+                            "value": "str"  # The annotation value. An arbitrary string.
+                              Required.
+                        }
+                    ],
+                    "arguments": [
+                        {
+                            "keyword": "str",  # The 'keyword' of the corresponding
+                              ModelParameter. Required.
+                            "value": "str"  # The value of of the argument. Always a
+                              string; implementations are responsible for parsing. Required.
+                        }
+                    ],
+                    "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
+                      (assigned by system).
+                    "description": "str",  # Optional. Long-form description, interpreted as
+                      Markdown.
+                    "inputs": [
+                        {
+                            "entity": "str",  # The ID of the entity whose data should be
+                              made available as 'keyword'. Required.
+                            "keyword": "str"  # The 'keyword' specified for this input in
+                              the MethodSpec. Required.
+                        }
+                    ],
+                    "kind": "SafetyCase",  # Optional. Default value is "SafetyCase". Kind.
+                      "SafetyCase"
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    },
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @distributed_trace
+    def create(self, body: Union[JSON, IO[bytes]], **kwargs: Any) -> JSON:
+        # pylint: disable=line-too-long
+        """Create a SafetyCase.
+
+        Create a SafetyCase.
+
+        :param body: Is either a JSON type or a IO[bytes] type. Required.
+        :type body: JSON or IO[bytes]
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "method": "str",  # Method ID. Required.
+                    "scope": {
+                        "dataset": "str",  # Optional. Dataset.
+                        "evaluation": "str",  # Optional. Evaluation.
+                        "inferenceService": "str",  # Optional. Inferenceservice.
+                        "model": "str"  # Optional. Model.
+                    },
+                    "arguments": [
+                        {
+                            "keyword": "str",  # The 'keyword' of the corresponding
+                              ModelParameter. Required.
+                            "value": "str"  # The value of of the argument. Always a
+                              string; implementations are responsible for parsing. Required.
+                        }
+                    ],
+                    "inputs": [
+                        {
+                            "entity": "str",  # The ID of the entity whose data should be
+                              made available as 'keyword'. Required.
+                            "keyword": "str"  # The 'keyword' specified for this input in
+                              the MethodSpec. Required.
+                        }
+                    ],
+                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "id": "str",  # Unique identifier of the entity. Required.
+                    "method": {
+                        "account": "str",  # Account that owns the entity. Required.
+                        "id": "str",  # Unique identifier of the entity. Required.
+                        "implementation": {
+                            "kind": "str",  # The kind of implementation. Required.
+                            "jupyterNotebook": {
+                                "notebookModule": "str",  # ID of the Module that
+                                  contains the notebook file. This does *not* add the Module as a
+                                  dependency; you must do that separately. Required.
+                                "notebookPath": "str"  # Path to the notebook file
+                                  relative to the Module root directory. Required.
+                            },
+                            "pythonFunction": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python function to call. Required.
+                            },
+                            "pythonRubric": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python Rubric to run. Required.
+                            }
+                        },
+                        "name": "str",  # Descriptive name of the Method. Required.
+                        "output": {
+                            "kind": "str",  # The kind of output artifact. Required.
+                              Known values are: "Measurement" and "SafetyCase".
+                            "measurement": {
+                                "level": "str",  # Measurement level. Required. Known
+                                  values are: "Dataset" and "Instance".
+                                "name": "str",  # Descriptive name of the
+                                  Measurement. Required.
+                                "schema": {
+                                    "arrowSchema": "str",  # The schema in Arrow
+                                      format, encoded with dyff.schema.arrow.encode_schema(). This is
+                                      required, but can be populated from a DyffDataSchema. Required.
+                                    "dyffSchema": {
+                                        "components": [
+                                            "str"  # A list of named dyff
+                                              data schemas. The final schema is the composition of
+                                              these component schemas. Required.
+                                        ],
+                                        "schemaVersion": "0.1"  # Optional.
+                                          Default value is "0.1". The dyff schema version. "0.1"
+                                    },
+                                    "jsonSchema": {}  # Optional. The schema in
+                                      JSON Schema format.
+                                },
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            },
+                            "safetyCase": {
+                                "name": "str",  # Descriptive name of the SafetyCase.
+                                  Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        },
+                        "scope": "str",  # The scope of the Method. The Method produces
+                          outputs that are specific to one entity of the type specified in the .scope
+                          field. Required. Known values are: "InferenceService" and "Evaluation".
+                        "description": "str",  # Optional. Long-form description, interpreted
+                          as Markdown.
+                        "inputs": [
+                            {
+                                "keyword": "str",  # The input is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "kind": "str",  # The kind of input artifact.
+                                  Required. Known values are: "Dataset", "Evaluation", "Measurement",
+                                  and "Report".
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ],
+                        "modules": [
+                            "str"  # Optional. Modules to load into the analysis
+                              environment.
+                        ],
+                        "parameters": [
+                            {
+                                "keyword": "str",  # The parameter is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ]
+                    },
+                    "name": "str",  # Descriptive name of the SafetyCase. Required.
+                    "scope": {
+                        "dataset": "str",  # Optional. Dataset.
+                        "evaluation": "str",  # Optional. Evaluation.
+                        "inferenceService": "str",  # Optional. Inferenceservice.
+                        "model": "str"  # Optional. Model.
+                    },
+                    "annotations": [
+                        {
+                            "key": "str",  # The annotation key. A DNS label with an
+                              optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                              Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
+                              See
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                              for detailed naming rules. Required.
+                            "value": "str"  # The annotation value. An arbitrary string.
+                              Required.
+                        }
+                    ],
+                    "arguments": [
+                        {
+                            "keyword": "str",  # The 'keyword' of the corresponding
+                              ModelParameter. Required.
+                            "value": "str"  # The value of of the argument. Always a
+                              string; implementations are responsible for parsing. Required.
+                        }
+                    ],
+                    "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
+                      (assigned by system).
+                    "description": "str",  # Optional. Long-form description, interpreted as
+                      Markdown.
+                    "inputs": [
+                        {
+                            "entity": "str",  # The ID of the entity whose data should be
+                              made available as 'keyword'. Required.
+                            "keyword": "str"  # The 'keyword' specified for this input in
+                              the MethodSpec. Required.
+                        }
+                    ],
+                    "kind": "SafetyCase",  # Optional. Default value is "SafetyCase". Kind.
+                      "SafetyCase"
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    },
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop(
+            "content_type", _headers.pop("Content-Type", None)
+        )
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        _request = build_safetycases_create_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @distributed_trace
+    def get(self, safetycase_id: str, **kwargs: Any) -> JSON:
+        # pylint: disable=line-too-long
+        """Get a SafetyCase by its key.
+
+        Get a SafetyCase by its key. Raises a 404 error if no entity exists with that key.
+
+        :param safetycase_id: Required.
+        :type safetycase_id: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "account": "str",  # Account that owns the entity. Required.
+                    "id": "str",  # Unique identifier of the entity. Required.
+                    "method": {
+                        "account": "str",  # Account that owns the entity. Required.
+                        "id": "str",  # Unique identifier of the entity. Required.
+                        "implementation": {
+                            "kind": "str",  # The kind of implementation. Required.
+                            "jupyterNotebook": {
+                                "notebookModule": "str",  # ID of the Module that
+                                  contains the notebook file. This does *not* add the Module as a
+                                  dependency; you must do that separately. Required.
+                                "notebookPath": "str"  # Path to the notebook file
+                                  relative to the Module root directory. Required.
+                            },
+                            "pythonFunction": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python function to call. Required.
+                            },
+                            "pythonRubric": {
+                                "fullyQualifiedName": "str"  # The fully-qualified
+                                  name of the Python Rubric to run. Required.
+                            }
+                        },
+                        "name": "str",  # Descriptive name of the Method. Required.
+                        "output": {
+                            "kind": "str",  # The kind of output artifact. Required.
+                              Known values are: "Measurement" and "SafetyCase".
+                            "measurement": {
+                                "level": "str",  # Measurement level. Required. Known
+                                  values are: "Dataset" and "Instance".
+                                "name": "str",  # Descriptive name of the
+                                  Measurement. Required.
+                                "schema": {
+                                    "arrowSchema": "str",  # The schema in Arrow
+                                      format, encoded with dyff.schema.arrow.encode_schema(). This is
+                                      required, but can be populated from a DyffDataSchema. Required.
+                                    "dyffSchema": {
+                                        "components": [
+                                            "str"  # A list of named dyff
+                                              data schemas. The final schema is the composition of
+                                              these component schemas. Required.
+                                        ],
+                                        "schemaVersion": "0.1"  # Optional.
+                                          Default value is "0.1". The dyff schema version. "0.1"
+                                    },
+                                    "jsonSchema": {}  # Optional. The schema in
+                                      JSON Schema format.
+                                },
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            },
+                            "safetyCase": {
+                                "name": "str",  # Descriptive name of the SafetyCase.
+                                  Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        },
+                        "scope": "str",  # The scope of the Method. The Method produces
+                          outputs that are specific to one entity of the type specified in the .scope
+                          field. Required. Known values are: "InferenceService" and "Evaluation".
+                        "description": "str",  # Optional. Long-form description, interpreted
+                          as Markdown.
+                        "inputs": [
+                            {
+                                "keyword": "str",  # The input is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "kind": "str",  # The kind of input artifact.
+                                  Required. Known values are: "Dataset", "Evaluation", "Measurement",
+                                  and "Report".
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ],
+                        "modules": [
+                            "str"  # Optional. Modules to load into the analysis
+                              environment.
+                        ],
+                        "parameters": [
+                            {
+                                "keyword": "str",  # The parameter is referred to by
+                                  'keyword' in the context of the method implementation. Required.
+                                "description": "str"  # Optional. Long-form
+                                  description, interpreted as Markdown.
+                            }
+                        ]
+                    },
+                    "name": "str",  # Descriptive name of the SafetyCase. Required.
+                    "scope": {
+                        "dataset": "str",  # Optional. Dataset.
+                        "evaluation": "str",  # Optional. Evaluation.
+                        "inferenceService": "str",  # Optional. Inferenceservice.
+                        "model": "str"  # Optional. Model.
+                    },
+                    "annotations": [
+                        {
+                            "key": "str",  # The annotation key. A DNS label with an
+                              optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                              Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
+                              See
+                              https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+                              for detailed naming rules. Required.
+                            "value": "str"  # The annotation value. An arbitrary string.
+                              Required.
+                        }
+                    ],
+                    "arguments": [
+                        {
+                            "keyword": "str",  # The 'keyword' of the corresponding
+                              ModelParameter. Required.
+                            "value": "str"  # The value of of the argument. Always a
+                              string; implementations are responsible for parsing. Required.
+                        }
+                    ],
+                    "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
+                      (assigned by system).
+                    "description": "str",  # Optional. Long-form description, interpreted as
+                      Markdown.
+                    "inputs": [
+                        {
+                            "entity": "str",  # The ID of the entity whose data should be
+                              made available as 'keyword'. Required.
+                            "keyword": "str"  # The 'keyword' specified for this input in
+                              the MethodSpec. Required.
+                        }
+                    ],
+                    "kind": "SafetyCase",  # Optional. Default value is "SafetyCase". Kind.
+                      "SafetyCase"
+                    "labels": {
+                        "str": "str"  # Optional. A set of key-value labels for the resource.
+                          Used to specify identifying attributes of resources that are meaningful to
+                          users but do not imply semantics in the dyff system.  The keys are DNS labels
+                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
+                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
+                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
+                          follow the kubernetes label conventions closely. See:
+                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
+                    },
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
+                      version. "0.1"
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        _request = build_safetycases_get_request(
+            safetycase_id=safetycase_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @distributed_trace
+    def delete(self, safetycase_id: str, **kwargs: Any) -> JSON:
+        """Mark a SafetyCase for deletion.
+
+        Mark a SafetyCase for deletion.
+
+        :param safetycase_id: Required.
+        :type safetycase_id: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        _request = build_safetycases_delete_request(
+            safetycase_id=safetycase_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
```

### Comparing `dyff-client-0.2.2/dyff/client/_generated/operations/_patch.py` & `dyff_client-0.3.0/dyff/client/_generated/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.2/dyff/client/client.py` & `dyff_client-0.3.0/dyff/client/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,33 +43,42 @@
     DyffEntity,
     Evaluation,
     InferenceInterface,
     InferenceService,
     InferenceSession,
     InferenceSessionAndToken,
     Label,
+    Measurement,
+    Method,
     Model,
     Module,
     Report,
+    SafetyCase,
     Status,
     StorageSignedURL,
 )
 from dyff.schema.requests import (
+    AnalysisCreateRequest,
     DatasetCreateRequest,
     EvaluationCreateRequest,
     InferenceServiceCreateRequest,
     InferenceSessionCreateRequest,
     LabelUpdateRequest,
+    MethodCreateRequest,
     ModelCreateRequest,
     ModuleCreateRequest,
     ReportCreateRequest,
 )
 
-from ._generated import DyffAPI as RawClient
+from ._generated import DyffV0API as RawClient
 from ._generated._serialization import Serializer
+
+# from ._generated.operations._operations import (
+#     AnalysesOperations as AnalysesOperationsGenerated,
+# )
 from ._generated.operations._operations import (
     AuditproceduresOperations as AuditproceduresOperationsGenerated,
 )
 from ._generated.operations._operations import (
     AuditsOperations as AuditsOperationsGenerated,
 )
 from ._generated.operations._operations import (
@@ -81,22 +90,31 @@
 from ._generated.operations._operations import (
     InferenceservicesOperations as InferenceservicesOperationsGenerated,
 )
 from ._generated.operations._operations import (
     InferencesessionsOperations as InferencesessionsOperationsGenerated,
 )
 from ._generated.operations._operations import (
+    MeasurementsOperations as MeasurementsOperationsGenerated,
+)
+from ._generated.operations._operations import (
+    MethodsOperations as MethodsOperationsGenerated,
+)
+from ._generated.operations._operations import (
     ModelsOperations as ModelsOperationsGenerated,
 )
 from ._generated.operations._operations import (
     ModulesOperations as ModulesOperationsGenerated,
 )
 from ._generated.operations._operations import (
     ReportsOperations as ReportsOperationsGenerated,
 )
+from ._generated.operations._operations import (
+    SafetycasesOperations as SafetycasesOperationsGenerated,
+)
 
 if sys.version_info >= (3, 9):
     from collections.abc import MutableMapping
 else:
     from typing import (
         MutableMapping,  # type: ignore  # pylint: disable=ungrouped-imports
     )
@@ -260,14 +278,126 @@
             response.read()
             json_response = once(response.json())
             if self._output_adapter is not None:
                 json_response = self._output_adapter(json_response)
         return list(json_response)
 
 
+# class AnalysesOperations:
+#     """Operations on :class:`~dyff.schema.platform.Analysis` entities.
+
+#     .. note::
+
+#       Do not instantiate this class. Access it through the
+#       ``.analyses`` attribute of :class:`~dyff.client.Client`.
+#     """
+
+#     def __init__(self, _raw_ops: AnalysesOperationsGenerated):
+#         self._raw_ops = _raw_ops
+
+#     def get(self, analysis_id: str) -> Analysis:
+#         """Get an Analysis by its key.
+
+#         :param analysis_id: The analysis id
+#         :type analysis_id: str
+#         :return: The Analysis with the given ID.
+#         """
+#         return Analysis.parse_obj(self._raw_ops.get(analysis_id))
+
+#     def delete(self, analysis_id: str) -> Status:
+#         """Mark an Analysis for deletion.
+
+#         :param analysis_id: The analysis id
+#         :type analysis_id: str
+#         :return: The resulting status of the entity
+#         :rtype: dyff.schema.platform.Status
+#         """
+#         return Status.parse_obj(self._raw_ops.delete(analysis_id))
+
+#     def query(
+#         self,
+#         *,
+#         id: Optional[str] = None,
+#         account: Optional[str] = None,
+#         status: Optional[str] = None,
+#         reason: Optional[str] = None,
+#         labels: Optional[dict[str, str]] = None,
+#         method: Optional[str] = None,
+#         method_name: Optional[str] = None,
+#         method_output_kind: Optional[str] = None,
+#     ) -> list[Analysis]:
+#         """Get all Analysis entities matching a query. The query is a set of equality constraints
+#         specified as key-value pairs.
+
+#         :keyword id: Default value is None.
+#         :paramtype id: str
+#         :keyword account: Default value is None.
+#         :paramtype account: str
+#         :keyword status: Default value is None.
+#         :paramtype status: str
+#         :keyword reason: Default value is None.
+#         :paramtype reason: str
+#         :keyword labels: Default value is None.
+#         :paramtype labels: dict[str, str]
+#         :keyword method: Default value is None.
+#         :paramtype method: str
+#         :keyword method_name: Default value is None.
+#         :paramtype method_name: str
+#         :keyword method_output_kind: Default value is None.
+#         :paramtype method_output_kind: str
+#         :return: list of Analysis entities matching the query
+#         :rtype: list[Analysis]
+#         :raises ~azure.core.exceptions.HttpResponseError:
+#         """
+#         return [
+#             Analysis.parse_obj(obj)
+#             for obj in self._raw_ops.query(
+#                 id=id,
+#                 account=account,
+#                 status=status,
+#                 reason=reason,
+#                 labels=_encode_labels(labels),
+#                 method=method,
+#                 method_name=method_name,
+#                 method_output_kind=method_output_kind,
+#             )
+#         ]
+
+#     def label(self, analysis_id: str, labels: dict[str, Optional[str]]) -> None:
+#         """Label the specified Analysis with key-value pairs (stored in the ``.labels``
+#         field of the resource).
+
+#         Providing ``None`` for the value deletes the label.
+
+#         See :class:`~dyff.schema.platform.Label` for a description of the
+#         constraints on label keys and values.
+
+#         :param analysis_id: The ID of the Analysis to label.
+#         :type analysis_id: str
+#         :param labels: The label keys and values.
+#         :type labels: dict[str, Optional[str]]
+#         """
+#         if not labels:
+#             return
+#         labels = LabelUpdateRequest(labels=labels).dict()
+#         self._raw_ops.label(analysis_id, labels)
+
+#     def create(self, analysis_request: AnalysisCreateRequest) -> Analysis:
+#         """Create an Analysis.
+
+#         .. note::
+#             This operation will incur compute costs.
+
+#         :param analysis_request: The Analysis specification.
+#         :type analysis_request: AnalysisCreateRequest
+#         :return: A full Analysis entity with .id and other properties set.
+#         """
+#         return Analysis.parse_obj(self._raw_ops.create(analysis_request.dict()))
+
+
 class AuditsOperations:
     """Operations on :class:`~dyff.schema.platform.Audit` entities.
 
     .. note::
 
       Do not instantiate this class. Access it through the
       ``.audits`` attribute of :class:`~dyff.client.Client`.
@@ -1166,14 +1296,235 @@
 
         :param str session_id: The ID of the session.
         :raises HttpResponseError:
         """
         return str(self._raw_ops.token(session_id))
 
 
+class MeasurementsOperations:
+    """Operations on :class:`~dyff.schema.platform.Measurement` entities.
+
+    .. note::
+
+      Do not instantiate this class. Access it through the
+      ``.measurements`` attribute of :class:`~dyff.client.Client`.
+    """
+
+    def __init__(self, _raw_ops: MeasurementsOperationsGenerated):
+        self._raw_ops = _raw_ops
+
+    def get(self, measurement_id: str) -> Measurement:
+        """Get a Measurement by its key.
+
+        :param measurement_id: The Measurement ID
+        :type measurement_id: str
+        :return: The Measurement with the given ID.
+        """
+        return Measurement.parse_obj(self._raw_ops.get(measurement_id))
+
+    def query(
+        self,
+        *,
+        id: Optional[str] = None,
+        account: Optional[str] = None,
+        status: Optional[str] = None,
+        reason: Optional[str] = None,
+        labels: Optional[dict[str, str]] = None,
+        dataset: Optional[str] = None,
+        dataset_name: Optional[str] = None,
+        evaluation: Optional[str] = None,
+        inference_service: Optional[str] = None,
+        inference_service_name: Optional[str] = None,
+        method: Optional[str] = None,
+        method_name: Optional[str] = None,
+        model: Optional[str] = None,
+        model_name: Optional[str] = None,
+    ) -> list[Measurement]:
+        """Get all Measurement entities matching a query. The query is a set of equality
+        constraints specified as key-value pairs.
+
+        :keyword id: Default value is None.
+        :paramtype id: str
+        :keyword account: Default value is None.
+        :paramtype account: str
+        :keyword status: Default value is None.
+        :paramtype status: str
+        :keyword reason: Default value is None.
+        :paramtype reason: str
+        :keyword labels: Default value is None.
+        :paramtype labels: dict[str, str]
+        :keyword dataset: Default value is None.
+        :paramtype dataset: str
+        :keyword dataset_name: Default value is None.
+        :paramtype dataset_name: str
+        :keyword evaluation: Default value is None.
+        :paramtype evaluation: str
+        :keyword inference_service: Default value is None.
+        :paramtype inference_service: str
+        :keyword inference_service_name: Default value is None.
+        :paramtype inference_service_name: str
+        :keyword method: Default value is None.
+        :paramtype method: str
+        :keyword method_name: Default value is None.
+        :paramtype method_name: str
+        :keyword model: Default value is None.
+        :paramtype model: str
+        :keyword model_name: Default value is None.
+        :paramtype model_name: str
+        :return: Entities matching the query
+        :rtype: list[Measurement]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        return [
+            Measurement.parse_obj(obj)
+            for obj in self._raw_ops.query(
+                id=id,
+                account=account,
+                status=status,
+                reason=reason,
+                labels=_encode_labels(labels),
+                dataset=dataset,
+                dataset_name=dataset_name,
+                evaluation=evaluation,
+                inference_service=inference_service,
+                inference_service_name=inference_service_name,
+                method=method,
+                method_name=method_name,
+                model=model,
+                model_name=model_name,
+            )
+        ]
+
+    def label(self, measurement_id: str, labels: dict[str, Optional[str]]) -> None:
+        """Label the specified Measurement with key-value pairs (stored in the
+        ``.labels`` field of the resource).
+
+        Providing ``None`` for the value deletes the label.
+
+        See :class:`~dyff.schema.platform.Label` for a description of the
+        constraints on label keys and values.
+
+        :param measurement_id: The ID of the Measurement to label.
+        :type measurement_id: str
+        :param labels: The label keys and values.
+        :type labels: dict[str, Optional[str]]
+        """
+        if not labels:
+            return
+        labels = LabelUpdateRequest(labels=labels).dict()
+        self._raw_ops.label(measurement_id, labels)
+
+    def create(self, analysis_request: AnalysisCreateRequest) -> Measurement:
+        """Create a Measurement.
+
+        :param analysis_request: The Measurement specification.
+        :type analysis_request: AnalysisCreateRequest
+        :return: A full Meausrement entity with .id and other properties set.
+        """
+        return Measurement.parse_obj(self._raw_ops.create(analysis_request.dict()))
+
+
+class MethodsOperations:
+    """Operations on :class:`~dyff.schema.platform.Method` entities.
+
+    .. note::
+
+      Do not instantiate this class. Access it through the
+      ``.analyses`` attribute of :class:`~dyff.client.Client`.
+    """
+
+    def __init__(self, _raw_ops: MethodsOperationsGenerated):
+        self._raw_ops = _raw_ops
+
+    def get(self, analysis_id: str) -> Method:
+        """Get an Method by its key.
+
+        :param analysis_id: The Method id
+        :type analysis_id: str
+        :return: The Method with the given ID.
+        """
+        return Method.parse_obj(self._raw_ops.get(analysis_id))
+
+    def delete(self, analysis_id: str) -> Status:
+        """Mark an Method for deletion.
+
+        :param analysis_id: The analysis id
+        :type analysis_id: str
+        :return: The resulting status of the entity
+        :rtype: dyff.schema.platform.Status
+        """
+        return Status.parse_obj(self._raw_ops.delete(analysis_id))
+
+    def query(
+        self,
+        *,
+        id: Optional[str] = None,
+        account: Optional[str] = None,
+        status: Optional[str] = None,
+        reason: Optional[str] = None,
+        labels: Optional[dict[str, str]] = None,
+        name: Optional[str] = None,
+        output_kind: Optional[str] = None,
+    ) -> list[Method]:
+        """Get all Method entities matching a query. The query is a set of equality
+        constraints specified as key-value pairs.
+
+        :keyword id: Default value is None.
+        :paramtype id: str :keyword account: Default value is None.
+        :paramtype account: str :keyword status: Default value is None.
+        :paramtype status: str :keyword reason: Default value is None.
+        :paramtype reason: str :keyword labels: Default value is None.
+        :paramtype labels: dict[str, str] :keyword name: Default value is None.
+        :paramtype name: str :keyword output_kind: Default value is None.
+        :paramtype output_kind: str
+        :return: list of Method entities matching query
+        :rtype: list[Method] :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        return [
+            Method.parse_obj(obj)
+            for obj in self._raw_ops.query(
+                id=id,
+                account=account,
+                status=status,
+                reason=reason,
+                labels=_encode_labels(labels),
+                name=name,
+                output_kind=output_kind,
+            )
+        ]
+
+    def label(self, analysis_id: str, labels: dict[str, Optional[str]]) -> None:
+        """Label the specified Method with key-value pairs (stored in the ``.labels``
+        field of the resource).
+
+        Providing ``None`` for the value deletes the label.
+
+        See :class:`~dyff.schema.platform.Label` for a description of the
+        constraints on label keys and values.
+
+        :param analysis_id: The ID of the Method to label.
+        :type analysis_id: str
+        :param labels: The label keys and values.
+        :type labels: dict[str, Optional[str]]
+        """
+        if not labels:
+            return
+        labels = LabelUpdateRequest(labels=labels).dict()
+        self._raw_ops.label(analysis_id, labels)
+
+    def create(self, method_request: MethodCreateRequest) -> Method:
+        """Create an Method.
+
+        :param method_request: The Method specification.
+        :type method_request: MethodCreateRequest
+        :return: A full Method entity with .id and other properties set.
+        """
+        return Method.parse_obj(self._raw_ops.create(method_request.dict()))
+
+
 class ModelsOperations:
     """Operations on :class:`~dyff.schema.platform.Model` entities.
 
     .. note::
 
       Do not instantiate this class. Access it through the
       ``.models`` attribute of :class:`~dyff.client.Client`.
@@ -1614,14 +1965,137 @@
         blob = bytearray()
         for chunk in stream:
             blob.extend(chunk)  # type: ignore
         with BytesIO(blob) as fin:
             return pandas.read_parquet(fin)
 
 
+class SafetycasesOperations:
+    """Operations on :class:`~dyff.schema.platform.SafetyCase` entities.
+
+    .. note::
+
+      Do not instantiate this class. Access it through the
+      ``.safetycases`` attribute of :class:`~dyff.client.Client`.
+    """
+
+    def __init__(self, _raw_ops: SafetycasesOperationsGenerated):
+        self._raw_ops = _raw_ops
+
+    def get(self, safetycase_id: str) -> SafetyCase:
+        """Get a SafetyCase by its key.
+
+        :param safetycase_id: The SafetyCase ID
+        :type safetycase_id: str
+        :return: The SafetyCase with the given ID.
+        """
+        return SafetyCase.parse_obj(self._raw_ops.get(safetycase_id))
+
+    def query(
+        self,
+        *,
+        id: Optional[str] = None,
+        account: Optional[str] = None,
+        status: Optional[str] = None,
+        reason: Optional[str] = None,
+        labels: Optional[dict[str, str]] = None,
+        dataset: Optional[str] = None,
+        dataset_name: Optional[str] = None,
+        evaluation: Optional[str] = None,
+        inference_service: Optional[str] = None,
+        inference_service_name: Optional[str] = None,
+        method: Optional[str] = None,
+        method_name: Optional[str] = None,
+        model: Optional[str] = None,
+        model_name: Optional[str] = None,
+    ) -> list[SafetyCase]:
+        """Get all SafetyCase entities matching a query. The query is a set of equality
+        constraints specified as key-value pairs.
+
+        :keyword id: Default value is None.
+        :paramtype id: str
+        :keyword account: Default value is None.
+        :paramtype account: str
+        :keyword status: Default value is None.
+        :paramtype status: str
+        :keyword reason: Default value is None.
+        :paramtype reason: str
+        :keyword labels: Default value is None.
+        :paramtype labels: dict[str, str]
+        :keyword dataset: Default value is None.
+        :paramtype dataset: str
+        :keyword dataset_name: Default value is None.
+        :paramtype dataset_name: str
+        :keyword evaluation: Default value is None.
+        :paramtype evaluation: str
+        :keyword inference_service: Default value is None.
+        :paramtype inference_service: str
+        :keyword inference_service_name: Default value is None.
+        :paramtype inference_service_name: str
+        :keyword method: Default value is None.
+        :paramtype method: str
+        :keyword method_name: Default value is None.
+        :paramtype method_name: str
+        :keyword model: Default value is None.
+        :paramtype model: str
+        :keyword model_name: Default value is None.
+        :paramtype model_name: str
+        :return: Entities matching the query
+        :rtype: list[SafetyCase]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        return [
+            SafetyCase.parse_obj(obj)
+            for obj in self._raw_ops.query(
+                id=id,
+                account=account,
+                status=status,
+                reason=reason,
+                labels=_encode_labels(labels),
+                dataset=dataset,
+                dataset_name=dataset_name,
+                evaluation=evaluation,
+                inference_service=inference_service,
+                inference_service_name=inference_service_name,
+                method=method,
+                method_name=method_name,
+                model=model,
+                model_name=model_name,
+            )
+        ]
+
+    def label(self, safetycase_id: str, labels: dict[str, Optional[str]]) -> None:
+        """Label the specified SafetyCase with key-value pairs (stored in the
+        ``.labels`` field of the resource).
+
+        Providing ``None`` for the value deletes the label.
+
+        See :class:`~dyff.schema.platform.Label` for a description of the
+        constraints on label keys and values.
+
+        :param safetycase_id: The ID of the SafetyCase to label.
+        :type safetycase_id: str
+        :param labels: The label keys and values.
+        :type labels: dict[str, Optional[str]]
+        """
+        if not labels:
+            return
+        labels = LabelUpdateRequest(labels=labels).dict()
+        self._raw_ops.label(safetycase_id, labels)
+
+    def create(self, analysis_request: AnalysisCreateRequest) -> SafetyCase:
+        """Create a SafetyCase.
+
+        :param analysis_request: The SafetyCase specification.
+        :type analysis_request: AnalysisCreateRequest
+        :return: A full SafetyCase entity with .id and other properties set.
+        """
+        return SafetyCase.parse_obj(self._raw_ops.create(analysis_request.dict()))
+
+
 class _APIKeyCredential(TokenCredential):
     def __init__(self, *, api_key: str):
         self.api_key = api_key
 
     def get_token(
         self,
         *scopes: str,
@@ -1705,37 +2179,46 @@
         # False
         # >> print(self._pipeline._transport.connection_config.verify)
         # True
         self._raw._client._pipeline._transport.connection_config.verify = (  # type: ignore
             not insecure
         )
 
+        # self._analyses = AnalysesOperations(self._raw.analyses)
         self._audits = AuditsOperations(self._raw.audits)
         self._auditprocedures = AuditproceduresOperations(self._raw.auditprocedures)
         self._datasets = DatasetsOperations(self._raw.datasets, insecure=insecure)
         self._evaluations = EvaluationsOperations(self._raw.evaluations)
         self._inferenceservices = InferenceservicesOperations(
             self._raw.inferenceservices
         )
         self._inferencesessions = InferencesessionsOperations(
             self._raw.inferencesessions,
             insecure=insecure,
         )
+        self._measurements = MeasurementsOperations(self._raw.measurements)
+        self._methods = MethodsOperations(self._raw.methods)
         self._models = ModelsOperations(self._raw.models)
         self._modules = ModulesOperations(
             self._raw.modules,
             insecure=insecure,
         )
         self._reports = ReportsOperations(self._raw.reports)
+        self._safetycases = SafetycasesOperations(self._raw.safetycases)
 
     @property
     def raw(self) -> RawClient:
         """The "raw" API client, which can be used to send JSON requests directly."""
         return self._raw
 
+    # @property
+    # def analyses(self) -> AnalysesOperations:
+    #     """Operations on :class:`~dyff.schema.platform.Analysis` entities."""
+    #     return self._analyses
+
     @property
     def audits(self) -> AuditsOperations:
         """Operations on :class:`~dyff.schema.platform.Audit` entities."""
         return self._audits
 
     @property
     def auditprocedures(self) -> AuditproceduresOperations:
@@ -1759,28 +2242,43 @@
 
     @property
     def inferencesessions(self) -> InferencesessionsOperations:
         """Operations on :class:`~dyff.schema.platform.InferenceSession` entities."""
         return self._inferencesessions
 
     @property
+    def methods(self) -> MethodsOperations:
+        """Operations on :class:`~dyff.schema.platform.Method` entities."""
+        return self._methods
+
+    @property
+    def measurements(self) -> MeasurementsOperations:
+        """Operations on :class:`~dyff.schema.platform.Measurement` entities."""
+        return self._measurements
+
+    @property
     def models(self) -> ModelsOperations:
         """Operations on :class:`~dyff.schema.platform.Model` entities."""
         return self._models
 
     @property
     def modules(self) -> ModulesOperations:
         """Operations on :class:`~dyff.schema.platform.Module` entities."""
         return self._modules
 
     @property
     def reports(self) -> ReportsOperations:
         """Operations on :class:`~dyff.schema.platform.Report` entities."""
         return self._reports
 
+    @property
+    def safetycases(self) -> SafetycasesOperations:
+        """Operations on :class:`~dyff.schema.platform.SafetyCase` entities."""
+        return self._safetycases
+
 
 __all__ = [
     "Client",
     "InferenceSessionClient",
     "RawClient",
     "HttpResponseError",
 ]
```

### Comparing `dyff-client-0.2.2/dyff_client.egg-info/PKG-INFO` & `dyff_client-0.3.0/dyff_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-client
-Version: 0.2.2
+Version: 0.3.0
 Summary: Python client for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-client
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-client/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff-client-0.2.2/dyff_client.egg-info/SOURCES.txt` & `dyff_client-0.3.0/dyff_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.2/makefile` & `dyff_client-0.3.0/makefile`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.2/pyproject.toml` & `dyff_client-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.2/scripts/inferenceservices/databricks--dolly-v2-3b--default.py` & `dyff_client-0.3.0/scripts/inferenceservices/databricks--dolly-v2-3b--default.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.2/scripts/inferenceservices/tiiuae--falcon-7b--default.py` & `dyff_client-0.3.0/scripts/inferenceservices/tiiuae--falcon-7b--default.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.2/scripts/models/databricks--dolly-v2-3b.py` & `dyff_client-0.3.0/scripts/models/databricks--dolly-v2-3b.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.2/scripts/models/tiiuae--falcon-7b.py` & `dyff_client-0.3.0/scripts/models/tiiuae--falcon-7b.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.2/tests/test_import.py` & `dyff_client-0.3.0/tests/test_import.py`

 * *Files identical despite different names*

