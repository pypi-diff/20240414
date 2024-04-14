# Comparing `tmp/docker_autotag-2.0.3.tar.gz` & `tmp/docker_autotag-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_autotag-2.0.3.tar", max compression
+gzip compressed data, was "docker_autotag-2.0.4.tar", max compression
```

## Comparing `docker_autotag-2.0.3.tar` & `docker_autotag-2.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1123 2024-03-02 13:54:39.635066 docker_autotag-2.0.3/LICENSE
--rw-r--r--   0        0        0     3559 2024-03-02 13:54:39.635066 docker_autotag-2.0.3/README.md
--rw-r--r--   0        0        0       46 2024-03-02 13:54:59.723100 docker_autotag-2.0.3/dockerautotag/__init__.py
--rw-r--r--   0        0        0     3859 2024-03-02 13:54:39.635066 docker_autotag-2.0.3/dockerautotag/cli.py
--rw-r--r--   0        0        0     5694 2024-03-02 13:54:39.635066 docker_autotag-2.0.3/dockerautotag/logging.py
--rw-r--r--   0        0        0     1190 2024-03-02 13:54:39.635066 docker_autotag-2.0.3/dockerautotag/utils.py
--rw-r--r--   0        0        0     2923 2024-03-02 13:54:59.719100 docker_autotag-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     4942 1970-01-01 00:00:00.000000 docker_autotag-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1123 2024-04-14 09:47:20.423408 docker_autotag-2.0.4/LICENSE
+-rw-r--r--   0        0        0     3559 2024-04-14 09:47:20.423408 docker_autotag-2.0.4/README.md
+-rw-r--r--   0        0        0       46 2024-04-14 09:47:32.551702 docker_autotag-2.0.4/dockerautotag/__init__.py
+-rw-r--r--   0        0        0     3807 2024-04-14 09:47:20.423408 docker_autotag-2.0.4/dockerautotag/cli.py
+-rw-r--r--   0        0        0     5694 2024-04-14 09:47:20.423408 docker_autotag-2.0.4/dockerautotag/logging.py
+-rw-r--r--   0        0        0     1190 2024-04-14 09:47:20.423408 docker_autotag-2.0.4/dockerautotag/utils.py
+-rw-r--r--   0        0        0     2923 2024-04-14 09:47:32.551702 docker_autotag-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4942 1970-01-01 00:00:00.000000 docker_autotag-2.0.4/PKG-INFO
```

### Comparing `docker_autotag-2.0.3/LICENSE` & `docker_autotag-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `docker_autotag-2.0.3/README.md` & `docker_autotag-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `docker_autotag-2.0.3/dockerautotag/cli.py` & `docker_autotag-2.0.4/dockerautotag/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -93,17 +93,15 @@
             except Exception:  # noqa: BLE001
                 return default
         except Exception:  # noqa: BLE001
             return default
 
         if version.prerelease:
             tags.append(
-                "{}.{}.{}-{}".format(
-                    version.major, version.minor, version.patch, to_prerelease(version.prerelease)
-                )
+                f"{version.major}.{version.minor}.{version.patch}-{to_prerelease(version.prerelease)}"
             )
             if not ignore_pre:
                 return tags
 
         tags.append(f"{version.major}.{version.minor}")
         tags.append(f"{version.major}.{version.minor}.{version.patch}")
```

### Comparing `docker_autotag-2.0.3/dockerautotag/logging.py` & `docker_autotag-2.0.4/dockerautotag/logging.py`

 * *Files identical despite different names*

### Comparing `docker_autotag-2.0.3/dockerautotag/utils.py` & `docker_autotag-2.0.4/dockerautotag/utils.py`

 * *Files identical despite different names*

### Comparing `docker_autotag-2.0.3/pyproject.toml` & `docker_autotag-2.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,30 +24,30 @@
 include = ["LICENSE"]
 keywords = ["docker", "versioning", "automation", "ci"]
 license = "MIT"
 name = "docker-autotag"
 packages = [{ include = "dockerautotag" }]
 readme = "README.md"
 repository = "https://github.com/thegeeklab/docker-autotag/"
-version = "2.0.3"
+version = "2.0.4"
 
 [tool.poetry.dependencies]
 colorama = "0.4.6"
 python = "^3.8.0"
 python-json-logger = "2.0.7"
 semantic-version = "2.10.0"
 
 [tool.poetry.scripts]
 docker-autotag = "dockerautotag.cli:main"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "0.2.2"
-pytest = "8.0.2"
-pytest-mock = "3.12.0"
-pytest-cov = "4.1.0"
+ruff = "0.3.5"
+pytest = "8.1.1"
+pytest-mock = "3.14.0"
+pytest-cov = "5.0.0"
 toml = "0.10.2"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 style = "semver"
 vcs = "git"
```

### Comparing `docker_autotag-2.0.3/PKG-INFO` & `docker_autotag-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-autotag
-Version: 2.0.3
+Version: 2.0.4
 Summary: Creates a list of docker tags from a given version string.
 Home-page: https://github.com/thegeeklab/docker-autotag/
 License: MIT
 Keywords: docker,versioning,automation,ci
 Author: Robert Kaussow
 Author-email: mail@thegeeklab.de
 Requires-Python: >=3.8.0,<4.0.0
```

