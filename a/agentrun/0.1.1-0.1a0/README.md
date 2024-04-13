# Comparing `tmp/agentrun-0.1.1.tar.gz` & `tmp/agentrun-0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentrun-0.1.1.tar", last modified: Sat Apr 13 22:20:41 2024, max compression
+gzip compressed data, was "agentrun-0.1a0.tar", last modified: Fri Apr 12 01:30:58 2024, max compression
```

## Comparing `agentrun-0.1.1.tar` & `agentrun-0.1a0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:20:41.762290 agentrun-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-04-13 22:20:34.000000 agentrun-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-04-13 22:20:41.762290 agentrun-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13170 2024-04-13 22:20:34.000000 agentrun-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:20:41.762290 agentrun-0.1.1/agentrun/
--rw-r--r--   0 runner    (1001) docker     (127)    14320 2024-04-13 22:20:34.000000 agentrun-0.1.1/agentrun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:20:41.762290 agentrun-0.1.1/agentrun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-04-13 22:20:41.000000 agentrun-0.1.1/agentrun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-13 22:20:41.000000 agentrun-0.1.1/agentrun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 22:20:41.000000 agentrun-0.1.1/agentrun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-13 22:20:41.000000 agentrun-0.1.1/agentrun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 22:20:41.000000 agentrun-0.1.1/agentrun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-13 22:20:34.000000 agentrun-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 22:20:41.762290 agentrun-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:20:41.762290 agentrun-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-13 22:20:34.000000 agentrun-0.1.1/tests/test_agentrun.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:30:58.671492 agentrun-0.1a0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 01:30:51.000000 agentrun-0.1a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-12 01:30:58.671492 agentrun-0.1a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-12 01:30:51.000000 agentrun-0.1a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:30:58.671492 agentrun-0.1a0/agentrun/
+-rw-r--r--   0 runner    (1001) docker     (127)    14134 2024-04-12 01:30:51.000000 agentrun-0.1a0/agentrun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:30:58.671492 agentrun-0.1a0/agentrun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-12 01:30:58.000000 agentrun-0.1a0/agentrun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-12 01:30:58.000000 agentrun-0.1a0/agentrun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 01:30:58.000000 agentrun-0.1a0/agentrun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-12 01:30:58.000000 agentrun-0.1a0/agentrun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 01:30:58.000000 agentrun-0.1a0/agentrun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-12 01:30:51.000000 agentrun-0.1a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 01:30:58.671492 agentrun-0.1a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:30:58.671492 agentrun-0.1a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7499 2024-04-12 01:30:51.000000 agentrun-0.1a0/tests/test_agentrun.py
```

### Comparing `agentrun-0.1.1/LICENSE` & `agentrun-0.1a0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2024 Jonathan Adly
+   Copyright [yyyy] [name of copyright owner]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `agentrun-0.1.1/agentrun/__init__.py` & `agentrun-0.1a0/agentrun/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -360,14 +360,10 @@
                 return "Execution timed out."
 
         except Exception as e:
             return str(e)
 
         finally:
             if container:
-                # run clean up in a seperate thread to avoid blocking the main thread
-                thread = Thread(
-                    target=self.clean_up, args=(container, script_name, dependencies)
-                )
-                thread.start()
+                self.clean_up(container, script_name, dependencies)
 
         return output
```

### Comparing `agentrun-0.1.1/pyproject.toml` & `agentrun-0.1a0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,28 @@
 [project]
 name = "agentrun"
-version = "v0.1.1"
+version = "v0.1-alpha"
 description = "The easiest way to run AI or user generated python code safely in a docker container"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [{name = "Jonathan Adly", email = "gadly0123@gmail.com"}]
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
 ]
 dependencies = [
  "docker", "RestrictedPython", 
 ]
 
 [build-system]
-requires = ["setuptools", "wheel"]
+requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
-[tool.setuptools]
-include-package-data = false
-
-[tool.setuptools.packages.find]
-include = ["agentrun*"]
-exclude = ["agentrun-api*", "docs*", "examples*", "tests*", ".github*"]
-
 [project.urls]
 Homepage = "https://github.com/jonathan-adly/agentrun"
 Changelog = "https://github.com/jonathan-adly/agentrun/releases"
 Issues = "https://github.com/jonathan-adly/agentrun/issues"
 CI = "https://github.com/jonathan-adly/agentrun/actions"
 
 
 [project.optional-dependencies]
-test = ["pytest", "pytest-cov", "pytest-benchmark", "mypy"]
+test = ["pytest"]
```

### Comparing `agentrun-0.1.1/tests/test_agentrun.py` & `agentrun-0.1a0/tests/test_agentrun.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,23 +228,7 @@
 # test with wrong container name
 def test_execute_code_in_container_with_wrong_container_name():
     runner = AgentRun(
         container_name="wrong-container-name",
     )
     output = runner.execute_code_in_container("print('Hello, World!')")
     assert output == "Container with name wrong-container-name not found."
-
-
-def execute_code_in_container_benchmark(docker_container):
-    runner = AgentRun(
-        container_name=docker_container.name,
-    )
-    code = "import numpy as np\nprint(np.array([1, 2, 3]))"
-    output = runner.execute_code_in_container(code)
-    return output
-
-
-def test_dependency_benchmark(benchmark, docker_container):
-    result = benchmark(
-        execute_code_in_container_benchmark, docker_container=docker_container
-    )
-    assert result == "[1 2 3]\n"
```

