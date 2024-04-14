# Comparing `tmp/apidays24pj-0.0.8.tar.gz` & `tmp/apidays24pj-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apidays24pj-0.0.8.tar", last modified: Thu Apr 11 14:45:16 2024, max compression
+gzip compressed data, was "apidays24pj-0.0.9.tar", last modified: Thu Apr 11 15:46:54 2024, max compression
```

## Comparing `apidays24pj-0.0.8.tar` & `apidays24pj-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:45:16.439412 apidays24pj-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-11 14:45:01.000000 apidays24pj-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-11 14:45:01.000000 apidays24pj-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-11 14:45:16.439412 apidays24pj-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 14:45:01.000000 apidays24pj-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-11 14:45:01.000000 apidays24pj-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 14:45:16.439412 apidays24pj-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-11 14:45:01.000000 apidays24pj-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:45:16.435412 apidays24pj-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:45:16.439412 apidays24pj-0.0.8/src/apidays24pj/
--rw-r--r--   0 runner    (1001) docker     (127)   741362 2024-04-11 14:45:01.000000 apidays24pj-0.0.8/src/apidays24pj/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:45:16.439412 apidays24pj-0.0.8/src/apidays24pj/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-11 14:45:01.000000 apidays24pj-0.0.8/src/apidays24pj/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   100909 2024-04-11 14:45:01.000000 apidays24pj-0.0.8/src/apidays24pj/_jsii/apidays24pj@0.0.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:45:01.000000 apidays24pj-0.0.8/src/apidays24pj/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:45:16.439412 apidays24pj-0.0.8/src/apidays24pj.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-11 14:45:16.000000 apidays24pj-0.0.8/src/apidays24pj.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-11 14:45:16.000000 apidays24pj-0.0.8/src/apidays24pj.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:45:16.000000 apidays24pj-0.0.8/src/apidays24pj.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-11 14:45:16.000000 apidays24pj-0.0.8/src/apidays24pj.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 14:45:16.000000 apidays24pj-0.0.8/src/apidays24pj.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:46:54.193481 apidays24pj-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-11 15:46:43.000000 apidays24pj-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-11 15:46:43.000000 apidays24pj-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-11 15:46:54.193481 apidays24pj-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 15:46:43.000000 apidays24pj-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-11 15:46:43.000000 apidays24pj-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 15:46:54.193481 apidays24pj-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-11 15:46:43.000000 apidays24pj-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:46:54.189481 apidays24pj-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:46:54.193481 apidays24pj-0.0.9/src/apidays24pj/
+-rw-r--r--   0 runner    (1001) docker     (127)   741610 2024-04-11 15:46:43.000000 apidays24pj-0.0.9/src/apidays24pj/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:46:54.193481 apidays24pj-0.0.9/src/apidays24pj/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-11 15:46:43.000000 apidays24pj-0.0.9/src/apidays24pj/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101941 2024-04-11 15:46:43.000000 apidays24pj-0.0.9/src/apidays24pj/_jsii/apidays24pj@0.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:46:43.000000 apidays24pj-0.0.9/src/apidays24pj/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:46:54.193481 apidays24pj-0.0.9/src/apidays24pj.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-11 15:46:54.000000 apidays24pj-0.0.9/src/apidays24pj.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-11 15:46:54.000000 apidays24pj-0.0.9/src/apidays24pj.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:46:54.000000 apidays24pj-0.0.9/src/apidays24pj.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-11 15:46:54.000000 apidays24pj-0.0.9/src/apidays24pj.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 15:46:54.000000 apidays24pj-0.0.9/src/apidays24pj.egg-info/top_level.txt
```

### Comparing `apidays24pj-0.0.8/LICENSE` & `apidays24pj-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `apidays24pj-0.0.8/PKG-INFO` & `apidays24pj-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: apidays24pj
-Version: 0.0.8
-Summary: apidays24pj
+Version: 0.0.9
+Summary: @vianho/apidays24pj
 Home-page: https://github.com/vianho/projen-projects
 Author: Silviana<email@example.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/vianho/projen-projects
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
```

### Comparing `apidays24pj-0.0.8/setup.py` & `apidays24pj-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "apidays24pj",
-    "version": "0.0.8",
-    "description": "apidays24pj",
+    "version": "0.0.9",
+    "description": "@vianho/apidays24pj",
     "license": "Apache-2.0",
     "url": "https://github.com/vianho/projen-projects",
     "long_description_content_type": "text/markdown",
     "author": "Silviana<email@example.com>",
     "bdist_wheel": {
         "universal": true
     },
@@ -22,15 +22,15 @@
     },
     "packages": [
         "apidays24pj",
         "apidays24pj._jsii"
     ],
     "package_data": {
         "apidays24pj._jsii": [
-            "apidays24pj@0.0.8.jsii.tgz"
+            "apidays24pj@0.0.9.jsii.tgz"
         ],
         "apidays24pj": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `apidays24pj-0.0.8/src/apidays24pj/__init__.py` & `apidays24pj-0.0.9/src/apidays24pj/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import projen.javascript as _projen_javascript_04054675
 import projen.python as _projen_python_04054675
 import projen.release as _projen_release_04054675
 import projen.typescript as _projen_typescript_04054675
 
 
 @jsii.data_type(
-    jsii_type="apidays24pj.AuthenticateSnykOptions",
+    jsii_type="@vianho/apidays24pj.AuthenticateSnykOptions",
     jsii_struct_bases=[_projen_github_workflows_04054675.JobStepConfiguration],
     name_mapping={
         "env": "env",
         "id": "id",
         "if_": "if",
         "name": "name",
         "working_directory": "workingDirectory",
@@ -66,15 +66,15 @@
         :param working_directory: (experimental) Specifies a working directory for a step. Overrides a job's working directory.
         :param continue_on_error: (experimental) Prevents a job from failing when a step fails. Set to true to allow a job to pass when this step fails.
         :param timeout_minutes: (experimental) The maximum number of minutes to run the step before killing the process.
         :param snyk_org_id: 
         :param snyk_token: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7499bcac71e42b3d0bd6be83ad116500914c3fa1d57c699cd857047452b8b7b5)
+            type_hints = typing.get_type_hints(_typecheckingstub__9d8425126db24c75dc31a21c4b9944e8e2c263e278f1ca0615968eb602d8dd73)
             check_type(argname="argument env", value=env, expected_type=type_hints["env"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument if_", value=if_, expected_type=type_hints["if_"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument working_directory", value=working_directory, expected_type=type_hints["working_directory"])
             check_type(argname="argument continue_on_error", value=continue_on_error, expected_type=type_hints["continue_on_error"])
             check_type(argname="argument timeout_minutes", value=timeout_minutes, expected_type=type_hints["timeout_minutes"])
@@ -196,15 +196,15 @@
     def __repr__(self) -> str:
         return "AuthenticateSnykOptions(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
-    jsii_type="apidays24pj.CreateCacheOptions",
+    jsii_type="@vianho/apidays24pj.CreateCacheOptions",
     jsii_struct_bases=[_projen_github_workflows_04054675.JobStepConfiguration],
     name_mapping={
         "env": "env",
         "id": "id",
         "if_": "if",
         "name": "name",
         "working_directory": "workingDirectory",
@@ -235,15 +235,15 @@
         :param continue_on_error: (experimental) Prevents a job from failing when a step fails. Set to true to allow a job to pass when this step fails.
         :param timeout_minutes: (experimental) The maximum number of minutes to run the step before killing the process.
         :param with_: 
         '''
         if isinstance(with_, dict):
             with_ = CreateCacheWithOptions(**with_)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__6a13eaadc693af6419d337a0a037c1fefe0a413b3f3a3ba6e27ed07f8f93d349)
+            type_hints = typing.get_type_hints(_typecheckingstub__a392f47fe3aac33d0549380cc9fdbfc579a13a3c6d4313275def6f23a9a7ce0d)
             check_type(argname="argument env", value=env, expected_type=type_hints["env"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument if_", value=if_, expected_type=type_hints["if_"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument working_directory", value=working_directory, expected_type=type_hints["working_directory"])
             check_type(argname="argument continue_on_error", value=continue_on_error, expected_type=type_hints["continue_on_error"])
             check_type(argname="argument timeout_minutes", value=timeout_minutes, expected_type=type_hints["timeout_minutes"])
@@ -357,15 +357,15 @@
     def __repr__(self) -> str:
         return "CreateCacheOptions(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
-    jsii_type="apidays24pj.CreateCacheWithOptions",
+    jsii_type="@vianho/apidays24pj.CreateCacheWithOptions",
     jsii_struct_bases=[],
     name_mapping={
         "key": "key",
         "path": "path",
         "enable_cross_os_archive": "enableCrossOsArchive",
         "fail_on_cache_miss": "failOnCacheMiss",
         "lookup_only": "lookupOnly",
@@ -394,15 +394,15 @@
         :param fail_on_cache_miss: 
         :param lookup_only: 
         :param restore_keys: 
         :param save_always: 
         :param upload_chunk_size: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ea833d15382a60a8a18d31af670573cb61eaa1a9f5b7c096627d6c11cc8ef345)
+            type_hints = typing.get_type_hints(_typecheckingstub__fc49593c630f79bd92b523141ad72926301b0c4ad5cb531f79d3e6f83fc041ff)
             check_type(argname="argument key", value=key, expected_type=type_hints["key"])
             check_type(argname="argument path", value=path, expected_type=type_hints["path"])
             check_type(argname="argument enable_cross_os_archive", value=enable_cross_os_archive, expected_type=type_hints["enable_cross_os_archive"])
             check_type(argname="argument fail_on_cache_miss", value=fail_on_cache_miss, expected_type=type_hints["fail_on_cache_miss"])
             check_type(argname="argument lookup_only", value=lookup_only, expected_type=type_hints["lookup_only"])
             check_type(argname="argument restore_keys", value=restore_keys, expected_type=type_hints["restore_keys"])
             check_type(argname="argument save_always", value=save_always, expected_type=type_hints["save_always"])
@@ -477,15 +477,15 @@
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 class Envrc(
     _projen_04054675.FileBase,
     metaclass=jsii.JSIIMeta,
-    jsii_type="apidays24pj.Envrc",
+    jsii_type="@vianho/apidays24pj.Envrc",
 ):
     def __init__(
         self,
         project: _projen_04054675.Project,
         file_path: builtins.str,
         *,
         committed: typing.Optional[builtins.bool] = None,
@@ -500,15 +500,15 @@
         :param committed: (experimental) Indicates whether this file should be committed to git or ignored. By default, all generated files are committed and anti-tamper is used to protect against manual modifications. Default: true
         :param edit_gitignore: (experimental) Update the project's .gitignore file. Default: true
         :param executable: (experimental) Whether the generated file should be marked as executable. Default: false
         :param marker: (experimental) Adds the projen marker to the file. Default: - marker will be included as long as the project is not ejected
         :param readonly: (experimental) Whether the generated file should be readonly. Default: true
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ab43d75f13ad56674e2faec69ea8d19b8f29118c1aeb82b494a76763ab56ebed)
+            type_hints = typing.get_type_hints(_typecheckingstub__2122c06ad20ce5bd6dc82942fed07f8e4747805fcaee09ebd4ff1819404f9b8d)
             check_type(argname="argument project", value=project, expected_type=type_hints["project"])
             check_type(argname="argument file_path", value=file_path, expected_type=type_hints["file_path"])
         options = EnvrcOptions(
             committed=committed,
             edit_gitignore=edit_gitignore,
             executable=executable,
             marker=marker,
@@ -523,21 +523,21 @@
         resolver: _projen_04054675.IResolver,
     ) -> typing.Optional[builtins.str]:
         '''Implemented by derived classes and returns the contents of the file to emit.
 
         :param resolver: -
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__f01c9c292e1b1442fefef01d629b2113fb285d746f6e3bafbc5a9bc8cfb92df3)
+            type_hints = typing.get_type_hints(_typecheckingstub__683b82d7360fc75db810de449d3d4565e455d5e0255f8820ff67019f35661e6e)
             check_type(argname="argument resolver", value=resolver, expected_type=type_hints["resolver"])
         return typing.cast(typing.Optional[builtins.str], jsii.invoke(self, "synthesizeContent", [resolver]))
 
 
 @jsii.data_type(
-    jsii_type="apidays24pj.EnvrcOptions",
+    jsii_type="@vianho/apidays24pj.EnvrcOptions",
     jsii_struct_bases=[_projen_04054675.FileBaseOptions],
     name_mapping={
         "committed": "committed",
         "edit_gitignore": "editGitignore",
         "executable": "executable",
         "marker": "marker",
         "readonly": "readonly",
@@ -557,15 +557,15 @@
         :param committed: (experimental) Indicates whether this file should be committed to git or ignored. By default, all generated files are committed and anti-tamper is used to protect against manual modifications. Default: true
         :param edit_gitignore: (experimental) Update the project's .gitignore file. Default: true
         :param executable: (experimental) Whether the generated file should be marked as executable. Default: false
         :param marker: (experimental) Adds the projen marker to the file. Default: - marker will be included as long as the project is not ejected
         :param readonly: (experimental) Whether the generated file should be readonly. Default: true
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__f20332f9af214ba472ea1e1e5734d15d4a70e549387fbdbced7d8536598f4832)
+            type_hints = typing.get_type_hints(_typecheckingstub__7beb6ebe0c1d59f5dbbab8be19d6e18939c51219feb13da759cb619b8aca716f)
             check_type(argname="argument committed", value=committed, expected_type=type_hints["committed"])
             check_type(argname="argument edit_gitignore", value=edit_gitignore, expected_type=type_hints["edit_gitignore"])
             check_type(argname="argument executable", value=executable, expected_type=type_hints["executable"])
             check_type(argname="argument marker", value=marker, expected_type=type_hints["marker"])
             check_type(argname="argument readonly", value=readonly, expected_type=type_hints["readonly"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if committed is not None:
@@ -647,15 +647,15 @@
     def __repr__(self) -> str:
         return "EnvrcOptions(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
-    jsii_type="apidays24pj.InstallSnykOptions",
+    jsii_type="@vianho/apidays24pj.InstallSnykOptions",
     jsii_struct_bases=[_projen_github_workflows_04054675.JobStepConfiguration],
     name_mapping={
         "env": "env",
         "id": "id",
         "if_": "if",
         "name": "name",
         "working_directory": "workingDirectory",
@@ -695,15 +695,15 @@
         :param create_cache_options: 
         :param snyk_delta_version: 
         :param snyk_version: 
         '''
         if isinstance(create_cache_options, dict):
             create_cache_options = CreateCacheOptions(**create_cache_options)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__c914ee45f7c0eb47e0d9cc31d3686e4310074487655fb96e610c7ef15b35a82c)
+            type_hints = typing.get_type_hints(_typecheckingstub__af3a8e60d04fdfe1def4992e68fe353d0bf2a9ee372438a7959d989c5b8b7911)
             check_type(argname="argument env", value=env, expected_type=type_hints["env"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument if_", value=if_, expected_type=type_hints["if_"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument working_directory", value=working_directory, expected_type=type_hints["working_directory"])
             check_type(argname="argument continue_on_error", value=continue_on_error, expected_type=type_hints["continue_on_error"])
             check_type(argname="argument timeout_minutes", value=timeout_minutes, expected_type=type_hints["timeout_minutes"])
@@ -840,15 +840,15 @@
     def __repr__(self) -> str:
         return "InstallSnykOptions(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
-    jsii_type="apidays24pj.InstallSnykPrDiffOptions",
+    jsii_type="@vianho/apidays24pj.InstallSnykPrDiffOptions",
     jsii_struct_bases=[_projen_github_workflows_04054675.JobStepConfiguration],
     name_mapping={
         "env": "env",
         "id": "id",
         "if_": "if",
         "name": "name",
         "working_directory": "workingDirectory",
@@ -885,15 +885,15 @@
         :param cache: 
         :param create_cache_options: 
         :param version: 
         '''
         if isinstance(create_cache_options, dict):
             create_cache_options = CreateCacheOptions(**create_cache_options)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__f6c6a9712fc3dce9ccf17efe4fa4a84a14ef2a11e7adaa9fba911b2705c621b0)
+            type_hints = typing.get_type_hints(_typecheckingstub__8c703b1b8ea3b49f58bdb97a4a351acc0f376081db036a62df5a1c3c832961f2)
             check_type(argname="argument env", value=env, expected_type=type_hints["env"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument if_", value=if_, expected_type=type_hints["if_"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument working_directory", value=working_directory, expected_type=type_hints["working_directory"])
             check_type(argname="argument continue_on_error", value=continue_on_error, expected_type=type_hints["continue_on_error"])
             check_type(argname="argument timeout_minutes", value=timeout_minutes, expected_type=type_hints["timeout_minutes"])
@@ -1024,15 +1024,15 @@
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 class JSIIProject(
     _projen_cdk_04054675.JsiiProject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="apidays24pj.JSIIProject",
+    jsii_type="@vianho/apidays24pj.JSIIProject",
 ):
     '''JSII project.
 
     :pjid: jsii
     '''
 
     def __init__(
@@ -1527,15 +1527,15 @@
             renovatebot_options=renovatebot_options,
         )
 
         jsii.create(self.__class__, self, [options])
 
 
 @jsii.data_type(
-    jsii_type="apidays24pj.JSIIProjectOptions",
+    jsii_type="@vianho/apidays24pj.JSIIProjectOptions",
     jsii_struct_bases=[_projen_cdk_04054675.JsiiProjectOptions],
     name_mapping={
         "name": "name",
         "commit_generated": "commitGenerated",
         "git_ignore_options": "gitIgnoreOptions",
         "git_options": "gitOptions",
         "logging": "logging",
@@ -2097,15 +2097,15 @@
         if isinstance(publish_to_pypi, dict):
             publish_to_pypi = _projen_cdk_04054675.JsiiPythonTarget(**publish_to_pypi)
         if isinstance(python, dict):
             python = _projen_cdk_04054675.JsiiPythonTarget(**python)
         if isinstance(snyk_options, dict):
             snyk_options = SnykComponentOptions(**snyk_options)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__99f139571fd89965ef29bcec365b3acac0d2bf8f80bc6f75c7dbb8935c651ca9)
+            type_hints = typing.get_type_hints(_typecheckingstub__4140b37e76a6e68a146824bfb84673ecf5cbe5081a0931bd2d04361925ab497e)
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument commit_generated", value=commit_generated, expected_type=type_hints["commit_generated"])
             check_type(argname="argument git_ignore_options", value=git_ignore_options, expected_type=type_hints["git_ignore_options"])
             check_type(argname="argument git_options", value=git_options, expected_type=type_hints["git_options"])
             check_type(argname="argument logging", value=logging, expected_type=type_hints["logging"])
             check_type(argname="argument outdir", value=outdir, expected_type=type_hints["outdir"])
             check_type(argname="argument parent", value=parent, expected_type=type_hints["parent"])
@@ -4591,15 +4591,15 @@
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 class JavaProject(
     _projen_java_04054675.JavaProject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="apidays24pj.JavaProject",
+    jsii_type="@vianho/apidays24pj.JavaProject",
 ):
     '''Java project.
 
     :pjid: java
     '''
 
     def __init__(
@@ -4755,15 +4755,15 @@
             renovatebot_options=renovatebot_options,
         )
 
         jsii.create(self.__class__, self, [options])
 
 
 @jsii.data_type(
-    jsii_type="apidays24pj.JavaProjectOptions",
+    jsii_type="@vianho/apidays24pj.JavaProjectOptions",
     jsii_struct_bases=[_projen_java_04054675.JavaProjectOptions],
     name_mapping={
         "name": "name",
         "commit_generated": "commitGenerated",
         "git_ignore_options": "gitIgnoreOptions",
         "git_options": "gitOptions",
         "logging": "logging",
@@ -4946,15 +4946,15 @@
         if isinstance(packaging_options, dict):
             packaging_options = _projen_java_04054675.MavenPackagingOptions(**packaging_options)
         if isinstance(projenrc_java_options, dict):
             projenrc_java_options = _projen_java_04054675.ProjenrcOptions(**projenrc_java_options)
         if isinstance(snyk_options, dict):
             snyk_options = SnykComponentOptions(**snyk_options)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__1742f76ee2ee1687558699b1f671449ff1d742df6aa5019c85cc6f8fa9e4fea8)
+            type_hints = typing.get_type_hints(_typecheckingstub__12c379aa135bc0e1a1b53c8b5e3594a5a52062eee38868a1a87333f59f2d8074)
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument commit_generated", value=commit_generated, expected_type=type_hints["commit_generated"])
             check_type(argname="argument git_ignore_options", value=git_ignore_options, expected_type=type_hints["git_ignore_options"])
             check_type(argname="argument git_options", value=git_options, expected_type=type_hints["git_options"])
             check_type(argname="argument logging", value=logging, expected_type=type_hints["logging"])
             check_type(argname="argument outdir", value=outdir, expected_type=type_hints["outdir"])
             check_type(argname="argument parent", value=parent, expected_type=type_hints["parent"])
@@ -5738,15 +5738,15 @@
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 class PythonProject(
     _projen_python_04054675.PythonProject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="apidays24pj.PythonProject",
+    jsii_type="@vianho/apidays24pj.PythonProject",
 ):
     '''Python project.
 
     :pjid: py
     '''
 
     def __init__(
@@ -5932,15 +5932,15 @@
             renovatebot_options=renovatebot_options,
         )
 
         jsii.create(self.__class__, self, [options])
 
 
 @jsii.data_type(
-    jsii_type="apidays24pj.PythonProjectOptions",
+    jsii_type="@vianho/apidays24pj.PythonProjectOptions",
     jsii_struct_bases=[_projen_python_04054675.PythonProjectOptions],
     name_mapping={
         "name": "name",
         "commit_generated": "commitGenerated",
         "git_ignore_options": "gitIgnoreOptions",
         "git_options": "gitOptions",
         "logging": "logging",
@@ -6155,15 +6155,15 @@
         if isinstance(pytest_options, dict):
             pytest_options = _projen_python_04054675.PytestOptions(**pytest_options)
         if isinstance(venv_options, dict):
             venv_options = _projen_python_04054675.VenvOptions(**venv_options)
         if isinstance(snyk_options, dict):
             snyk_options = SnykComponentOptions(**snyk_options)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__957fb874ddb064650932935177b2ea1e011812edad4af8c5a506fc74107ed151)
+            type_hints = typing.get_type_hints(_typecheckingstub__891da87c367c14eb9024685586cafe6a3f10bc82d0da0c9c8a2290953b15ff66)
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument commit_generated", value=commit_generated, expected_type=type_hints["commit_generated"])
             check_type(argname="argument git_ignore_options", value=git_ignore_options, expected_type=type_hints["git_ignore_options"])
             check_type(argname="argument git_options", value=git_options, expected_type=type_hints["git_options"])
             check_type(argname="argument logging", value=logging, expected_type=type_hints["logging"])
             check_type(argname="argument outdir", value=outdir, expected_type=type_hints["outdir"])
             check_type(argname="argument parent", value=parent, expected_type=type_hints["parent"])
@@ -7048,15 +7048,15 @@
     def __repr__(self) -> str:
         return "PythonProjectOptions(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
-    jsii_type="apidays24pj.RunScaOptions",
+    jsii_type="@vianho/apidays24pj.RunScaOptions",
     jsii_struct_bases=[_projen_github_workflows_04054675.JobStepConfiguration],
     name_mapping={
         "env": "env",
         "id": "id",
         "if_": "if",
         "name": "name",
         "working_directory": "workingDirectory",
@@ -7091,15 +7091,15 @@
         :param continue_on_error: (experimental) Prevents a job from failing when a step fails. Set to true to allow a job to pass when this step fails.
         :param timeout_minutes: (experimental) The maximum number of minutes to run the step before killing the process.
         :param args: 
         :param result_path_output_id: 
         :param severity_threshold: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__11b9e25a6f753d83c33e159908b8f7823d99aa6927b697579dedbe900bcd6533)
+            type_hints = typing.get_type_hints(_typecheckingstub__0e002e7132017789d5df99e1716a07debfb5a4e13cbe3068c32c46073c26d346)
             check_type(argname="argument env", value=env, expected_type=type_hints["env"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument if_", value=if_, expected_type=type_hints["if_"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument working_directory", value=working_directory, expected_type=type_hints["working_directory"])
             check_type(argname="argument continue_on_error", value=continue_on_error, expected_type=type_hints["continue_on_error"])
             check_type(argname="argument timeout_minutes", value=timeout_minutes, expected_type=type_hints["timeout_minutes"])
@@ -7228,15 +7228,15 @@
     def __repr__(self) -> str:
         return "RunScaOptions(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
-    jsii_type="apidays24pj.RunSnykPrDiffOptions",
+    jsii_type="@vianho/apidays24pj.RunSnykPrDiffOptions",
     jsii_struct_bases=[_projen_github_workflows_04054675.JobStepConfiguration],
     name_mapping={
         "env": "env",
         "id": "id",
         "if_": "if",
         "name": "name",
         "working_directory": "workingDirectory",
@@ -7268,15 +7268,15 @@
         :param working_directory: (experimental) Specifies a working directory for a step. Overrides a job's working directory.
         :param continue_on_error: (experimental) Prevents a job from failing when a step fails. Set to true to allow a job to pass when this step fails.
         :param timeout_minutes: (experimental) The maximum number of minutes to run the step before killing the process.
         :param snyk_code_baseline_path: 
         :param snyk_code_current_path: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__9a689218f851a9f5b77288348c6dd48f1baa343882a0c678222c8a6636ca6642)
+            type_hints = typing.get_type_hints(_typecheckingstub__575d1d4a3c76341c42bfb993207158ebe8c83c6d7388f32b24a709d8668ae251)
             check_type(argname="argument env", value=env, expected_type=type_hints["env"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument if_", value=if_, expected_type=type_hints["if_"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument working_directory", value=working_directory, expected_type=type_hints["working_directory"])
             check_type(argname="argument continue_on_error", value=continue_on_error, expected_type=type_hints["continue_on_error"])
             check_type(argname="argument timeout_minutes", value=timeout_minutes, expected_type=type_hints["timeout_minutes"])
@@ -7398,15 +7398,15 @@
     def __repr__(self) -> str:
         return "RunSnykPrDiffOptions(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
-    jsii_type="apidays24pj.RunSnykSastOptions",
+    jsii_type="@vianho/apidays24pj.RunSnykSastOptions",
     jsii_struct_bases=[_projen_github_workflows_04054675.JobStepConfiguration],
     name_mapping={
         "env": "env",
         "id": "id",
         "if_": "if",
         "name": "name",
         "working_directory": "workingDirectory",
@@ -7440,15 +7440,15 @@
         :param timeout_minutes: (experimental) The maximum number of minutes to run the step before killing the process.
         :param authenticate_snyk_options: 
         :param severity_threshold: 
         '''
         if isinstance(authenticate_snyk_options, dict):
             authenticate_snyk_options = AuthenticateSnykOptions(**authenticate_snyk_options)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__917bbfab2f121ac66af4e22af7100b50aaaa08801c6843a48840d1286346a4d7)
+            type_hints = typing.get_type_hints(_typecheckingstub__3a20e44fb24557adba3d97dbfde5a79154b8a9ab953f810991a89123e22c3543)
             check_type(argname="argument env", value=env, expected_type=type_hints["env"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument if_", value=if_, expected_type=type_hints["if_"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument working_directory", value=working_directory, expected_type=type_hints["working_directory"])
             check_type(argname="argument continue_on_error", value=continue_on_error, expected_type=type_hints["continue_on_error"])
             check_type(argname="argument timeout_minutes", value=timeout_minutes, expected_type=type_hints["timeout_minutes"])
@@ -7570,15 +7570,15 @@
     def __repr__(self) -> str:
         return "RunSnykSastOptions(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
-    jsii_type="apidays24pj.RunSnykScaWithDeltaOptions",
+    jsii_type="@vianho/apidays24pj.RunSnykScaWithDeltaOptions",
     jsii_struct_bases=[_projen_github_workflows_04054675.JobStepConfiguration],
     name_mapping={
         "env": "env",
         "id": "id",
         "if_": "if",
         "name": "name",
         "working_directory": "workingDirectory",
@@ -7628,15 +7628,15 @@
         :param severity_threshold: 
         '''
         if isinstance(authenticate_snyk_options, dict):
             authenticate_snyk_options = AuthenticateSnykOptions(**authenticate_snyk_options)
         if isinstance(run_sca_options, dict):
             run_sca_options = RunScaOptions(**run_sca_options)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a0e8186f614b238d0b08b946ae63cd32cb9914849433387a41d2e306d36c67a2)
+            type_hints = typing.get_type_hints(_typecheckingstub__2878c4b2368eb6494231041317e9ed6bf275d47abadbe16f1a77b49d6ec85db1)
             check_type(argname="argument env", value=env, expected_type=type_hints["env"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument if_", value=if_, expected_type=type_hints["if_"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument working_directory", value=working_directory, expected_type=type_hints["working_directory"])
             check_type(argname="argument continue_on_error", value=continue_on_error, expected_type=type_hints["continue_on_error"])
             check_type(argname="argument timeout_minutes", value=timeout_minutes, expected_type=type_hints["timeout_minutes"])
@@ -7792,15 +7792,15 @@
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 class SecurityScanWorkflow(
     _projen_04054675.Component,
     metaclass=jsii.JSIIMeta,
-    jsii_type="apidays24pj.SecurityScanWorkflow",
+    jsii_type="@vianho/apidays24pj.SecurityScanWorkflow",
 ):
     def __init__(
         self,
         project: typing.Union[_projen_java_04054675.JavaProject, _projen_python_04054675.PythonProject, _projen_javascript_04054675.NodeProject, _projen_cdk_04054675.JsiiProject],
         name: builtins.str,
         *,
         triggers_options: typing.Optional[typing.Union[_projen_github_workflows_04054675.Triggers, typing.Dict[builtins.str, typing.Any]]] = None,
@@ -7809,15 +7809,15 @@
         '''
         :param project: -
         :param name: -
         :param triggers_options: 
         :param workflow_options: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__14ab5340a54ed05a3cb521aeea6091c331fce3b554cd4e4c909171f54789320f)
+            type_hints = typing.get_type_hints(_typecheckingstub__9ae80cfd938bfb79f63f4a9a860a04c3006dc3ccd21d42cf92f8198523654977)
             check_type(argname="argument project", value=project, expected_type=type_hints["project"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
         options = SecurityScanWorkflowOptions(
             triggers_options=triggers_options, workflow_options=workflow_options
         )
 
         jsii.create(self.__class__, self, [project, name, options])
@@ -7856,15 +7856,15 @@
         :param pages: 
         :param pull_requests: 
         :param repository_projects: 
         :param security_events: 
         :param statuses: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__82feaffcc0c7354797b7c8f3bf82188f862a51d27e911f2c5483eb544f1fb8c0)
+            type_hints = typing.get_type_hints(_typecheckingstub__418456736145bcec36319c90fb181c090b70c624edbcae96557ca2dd9f391ffb)
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument path", value=path, expected_type=type_hints["path"])
         permissions = _projen_github_workflows_04054675.JobPermissions(
             actions=actions,
             checks=checks,
             contents=contents,
             deployments=deployments,
@@ -7884,15 +7884,15 @@
     @builtins.property
     @jsii.member(jsii_name="workflow")
     def workflow(self) -> typing.Optional[_projen_github_04054675.GithubWorkflow]:
         return typing.cast(typing.Optional[_projen_github_04054675.GithubWorkflow], jsii.get(self, "workflow"))
 
 
 @jsii.data_type(
-    jsii_type="apidays24pj.SecurityScanWorkflowOptions",
+    jsii_type="@vianho/apidays24pj.SecurityScanWorkflowOptions",
     jsii_struct_bases=[],
     name_mapping={
         "triggers_options": "triggersOptions",
         "workflow_options": "workflowOptions",
     },
 )
 class SecurityScanWorkflowOptions:
@@ -7907,15 +7907,15 @@
         :param workflow_options: 
         '''
         if isinstance(triggers_options, dict):
             triggers_options = _projen_github_workflows_04054675.Triggers(**triggers_options)
         if isinstance(workflow_options, dict):
             workflow_options = _projen_github_04054675.GithubWorkflowOptions(**workflow_options)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__79146a50fc97b2474e8fa5d43d64887475e1b3e9e55efe88b25958358bcff36a)
+            type_hints = typing.get_type_hints(_typecheckingstub__affb2f3a02329f30fc70b12e8e5900f22b8648704b40143dd25429bec544044a)
             check_type(argname="argument triggers_options", value=triggers_options, expected_type=type_hints["triggers_options"])
             check_type(argname="argument workflow_options", value=workflow_options, expected_type=type_hints["workflow_options"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if triggers_options is not None:
             self._values["triggers_options"] = triggers_options
         if workflow_options is not None:
             self._values["workflow_options"] = workflow_options
@@ -7943,15 +7943,15 @@
     def __repr__(self) -> str:
         return "SecurityScanWorkflowOptions(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
-    jsii_type="apidays24pj.SetupNodeOptions",
+    jsii_type="@vianho/apidays24pj.SetupNodeOptions",
     jsii_struct_bases=[_projen_github_workflows_04054675.JobStepConfiguration],
     name_mapping={
         "env": "env",
         "id": "id",
         "if_": "if",
         "name": "name",
         "working_directory": "workingDirectory",
@@ -7980,15 +7980,15 @@
         :param name: (experimental) A name for your step to display on GitHub.
         :param working_directory: (experimental) Specifies a working directory for a step. Overrides a job's working directory.
         :param continue_on_error: (experimental) Prevents a job from failing when a step fails. Set to true to allow a job to pass when this step fails.
         :param timeout_minutes: (experimental) The maximum number of minutes to run the step before killing the process.
         :param node_version: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__68437243d81c9e0bb8cc2233867ed1a1270df2657cc2c32243091d7a780f36cb)
+            type_hints = typing.get_type_hints(_typecheckingstub__fc17ca199138f9ea8093446b733610b42f8c339c77c56ceb1b626a53b8e26562)
             check_type(argname="argument env", value=env, expected_type=type_hints["env"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument if_", value=if_, expected_type=type_hints["if_"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument working_directory", value=working_directory, expected_type=type_hints["working_directory"])
             check_type(argname="argument continue_on_error", value=continue_on_error, expected_type=type_hints["continue_on_error"])
             check_type(argname="argument timeout_minutes", value=timeout_minutes, expected_type=type_hints["timeout_minutes"])
@@ -8100,26 +8100,26 @@
 
     def __repr__(self) -> str:
         return "SetupNodeOptions(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-@jsii.enum(jsii_type="apidays24pj.SeverityThreshold")
+@jsii.enum(jsii_type="@vianho/apidays24pj.SeverityThreshold")
 class SeverityThreshold(enum.Enum):
     LOW = "LOW"
     MEDIUM = "MEDIUM"
     HIGH = "HIGH"
     CRITICAL = "CRITICAL"
 
 
 class SnykComponent(
     _projen_04054675.Component,
     metaclass=jsii.JSIIMeta,
-    jsii_type="apidays24pj.SnykComponent",
+    jsii_type="@vianho/apidays24pj.SnykComponent",
 ):
     def __init__(
         self,
         project: typing.Union[_projen_java_04054675.JavaProject, _projen_python_04054675.PythonProject, _projen_javascript_04054675.NodeProject, _projen_cdk_04054675.JsiiProject],
         *,
         enable_sast: typing.Optional[builtins.bool] = None,
         enable_sca: typing.Optional[builtins.bool] = None,
@@ -8138,15 +8138,15 @@
         :param snyk_monitored_project_id: 
         :param snyk_org_id: 
         :param snyk_sast_workflow_options: 
         :param snyk_sca_workflow_options: 
         :param workflow_name: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__059eec1cd4997b382e2a9b22feecdc034c8dfdd4dfe116062f6e386b6a9ac532)
+            type_hints = typing.get_type_hints(_typecheckingstub__cb405cdef6274681176612f421e28f571baaff0cd9d30c2f1ede9822b654f1ef)
             check_type(argname="argument project", value=project, expected_type=type_hints["project"])
         options = SnykComponentOptions(
             enable_sast=enable_sast,
             enable_sca=enable_sca,
             security_scan_workflow_options=security_scan_workflow_options,
             snyk_monitored_project_id=snyk_monitored_project_id,
             snyk_org_id=snyk_org_id,
@@ -8170,15 +8170,15 @@
     @builtins.property
     @jsii.member(jsii_name="snykWorkflowName")
     def snyk_workflow_name(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "snykWorkflowName"))
 
 
 @jsii.data_type(
-    jsii_type="apidays24pj.SnykComponentOptions",
+    jsii_type="@vianho/apidays24pj.SnykComponentOptions",
     jsii_struct_bases=[],
     name_mapping={
         "enable_sast": "enableSast",
         "enable_sca": "enableSca",
         "security_scan_workflow_options": "securityScanWorkflowOptions",
         "snyk_monitored_project_id": "snykMonitoredProjectId",
         "snyk_org_id": "snykOrgId",
@@ -8213,15 +8213,15 @@
         if isinstance(security_scan_workflow_options, dict):
             security_scan_workflow_options = SecurityScanWorkflowOptions(**security_scan_workflow_options)
         if isinstance(snyk_sast_workflow_options, dict):
             snyk_sast_workflow_options = SnykSastWorkflowOptions(**snyk_sast_workflow_options)
         if isinstance(snyk_sca_workflow_options, dict):
             snyk_sca_workflow_options = SnykScaWorkflowOptions(**snyk_sca_workflow_options)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__bd92fc73698543f9e46a0f483f66bb3f257d5458e779fd8ec087394cd49b8447)
+            type_hints = typing.get_type_hints(_typecheckingstub__dfd8814387fc6585660859797326036165cb9d67939e2e0e13f90d855e01e9ab)
             check_type(argname="argument enable_sast", value=enable_sast, expected_type=type_hints["enable_sast"])
             check_type(argname="argument enable_sca", value=enable_sca, expected_type=type_hints["enable_sca"])
             check_type(argname="argument security_scan_workflow_options", value=security_scan_workflow_options, expected_type=type_hints["security_scan_workflow_options"])
             check_type(argname="argument snyk_monitored_project_id", value=snyk_monitored_project_id, expected_type=type_hints["snyk_monitored_project_id"])
             check_type(argname="argument snyk_org_id", value=snyk_org_id, expected_type=type_hints["snyk_org_id"])
             check_type(argname="argument snyk_sast_workflow_options", value=snyk_sast_workflow_options, expected_type=type_hints["snyk_sast_workflow_options"])
             check_type(argname="argument snyk_sca_workflow_options", value=snyk_sca_workflow_options, expected_type=type_hints["snyk_sca_workflow_options"])
@@ -8295,15 +8295,15 @@
     def __repr__(self) -> str:
         return "SnykComponentOptions(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
-    jsii_type="apidays24pj.SnykReusableWorkflowOptions",
+    jsii_type="@vianho/apidays24pj.SnykReusableWorkflowOptions",
     jsii_struct_bases=[],
     name_mapping={
         "install_snyk_options": "installSnykOptions",
         "job_id": "jobId",
         "job_options": "jobOptions",
         "setup_node_options": "setupNodeOptions",
         "workflow_name": "workflowName",
@@ -8334,15 +8334,15 @@
         if isinstance(job_options, dict):
             job_options = _projen_github_workflows_04054675.Job(**job_options)
         if isinstance(setup_node_options, dict):
             setup_node_options = SetupNodeOptions(**setup_node_options)
         if isinstance(workflow_options, dict):
             workflow_options = _projen_github_04054675.GithubWorkflowOptions(**workflow_options)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b50419a73c6742644b189527cac822f77473cd6b0675087d8b1d801310fb9039)
+            type_hints = typing.get_type_hints(_typecheckingstub__7b881678ff7dd868659f80d530f797e51f8f508403b2f9318fc66e11b3954817)
             check_type(argname="argument install_snyk_options", value=install_snyk_options, expected_type=type_hints["install_snyk_options"])
             check_type(argname="argument job_id", value=job_id, expected_type=type_hints["job_id"])
             check_type(argname="argument job_options", value=job_options, expected_type=type_hints["job_options"])
             check_type(argname="argument setup_node_options", value=setup_node_options, expected_type=type_hints["setup_node_options"])
             check_type(argname="argument workflow_name", value=workflow_name, expected_type=type_hints["workflow_name"])
             check_type(argname="argument workflow_options", value=workflow_options, expected_type=type_hints["workflow_options"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
@@ -8402,15 +8402,15 @@
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 class SnykSastWorkflow(
     _projen_04054675.Component,
     metaclass=jsii.JSIIMeta,
-    jsii_type="apidays24pj.SnykSastWorkflow",
+    jsii_type="@vianho/apidays24pj.SnykSastWorkflow",
 ):
     def __init__(
         self,
         project: typing.Union[_projen_java_04054675.JavaProject, _projen_python_04054675.PythonProject, _projen_javascript_04054675.NodeProject, _projen_cdk_04054675.JsiiProject],
         *,
         authenticate_snyk_options: typing.Union[AuthenticateSnykOptions, typing.Dict[builtins.str, typing.Any]],
         checkout_baseline_options: typing.Optional[typing.Union[_projen_github_04054675.CheckoutOptions, typing.Dict[builtins.str, typing.Any]]] = None,
@@ -8443,15 +8443,15 @@
         :param job_id: 
         :param job_options: 
         :param setup_node_options: 
         :param workflow_name: 
         :param workflow_options: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0421a1e8469318296b8cc8e91d45895ca74a274f088ac3bdc6d19d2281e6b36b)
+            type_hints = typing.get_type_hints(_typecheckingstub__ee34abce9cb44b5c5b5b29fb7aa65f997c1c2b7ec3f23a82ee4c54838ac3daf8)
             check_type(argname="argument project", value=project, expected_type=type_hints["project"])
         options = SnykSastWorkflowOptions(
             authenticate_snyk_options=authenticate_snyk_options,
             checkout_baseline_options=checkout_baseline_options,
             checkout_current_options=checkout_current_options,
             delta=delta,
             download_artifact_options=download_artifact_options,
@@ -8472,15 +8472,15 @@
     @builtins.property
     @jsii.member(jsii_name="workflow")
     def workflow(self) -> typing.Optional[_projen_github_04054675.GithubWorkflow]:
         return typing.cast(typing.Optional[_projen_github_04054675.GithubWorkflow], jsii.get(self, "workflow"))
 
 
 @jsii.data_type(
-    jsii_type="apidays24pj.SnykSastWorkflowOptions",
+    jsii_type="@vianho/apidays24pj.SnykSastWorkflowOptions",
     jsii_struct_bases=[SnykReusableWorkflowOptions],
     name_mapping={
         "install_snyk_options": "installSnykOptions",
         "job_id": "jobId",
         "job_options": "jobOptions",
         "setup_node_options": "setupNodeOptions",
         "workflow_name": "workflowName",
@@ -8554,15 +8554,15 @@
         if isinstance(run_snyk_sast_baseline_options, dict):
             run_snyk_sast_baseline_options = RunSnykSastOptions(**run_snyk_sast_baseline_options)
         if isinstance(run_snyk_sast_current_options, dict):
             run_snyk_sast_current_options = RunSnykSastOptions(**run_snyk_sast_current_options)
         if isinstance(upload_artifact_options, dict):
             upload_artifact_options = _projen_github_04054675.UploadArtifactOptions(**upload_artifact_options)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e1b27431bdc247ac8f74dec999d67a7ae3c97832ce49550a65941fe558640f78)
+            type_hints = typing.get_type_hints(_typecheckingstub__fad9c203a45cfe324b94f121d928c27f1be1e11663352b77d79f7874b5e22510)
             check_type(argname="argument install_snyk_options", value=install_snyk_options, expected_type=type_hints["install_snyk_options"])
             check_type(argname="argument job_id", value=job_id, expected_type=type_hints["job_id"])
             check_type(argname="argument job_options", value=job_options, expected_type=type_hints["job_options"])
             check_type(argname="argument setup_node_options", value=setup_node_options, expected_type=type_hints["setup_node_options"])
             check_type(argname="argument workflow_name", value=workflow_name, expected_type=type_hints["workflow_name"])
             check_type(argname="argument workflow_options", value=workflow_options, expected_type=type_hints["workflow_options"])
             check_type(argname="argument authenticate_snyk_options", value=authenticate_snyk_options, expected_type=type_hints["authenticate_snyk_options"])
@@ -8703,15 +8703,15 @@
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 class SnykScaWorkflow(
     _projen_04054675.Component,
     metaclass=jsii.JSIIMeta,
-    jsii_type="apidays24pj.SnykScaWorkflow",
+    jsii_type="@vianho/apidays24pj.SnykScaWorkflow",
 ):
     def __init__(
         self,
         project: typing.Union[_projen_java_04054675.JavaProject, _projen_python_04054675.PythonProject, _projen_javascript_04054675.NodeProject, _projen_cdk_04054675.JsiiProject],
         *,
         run_snyk_sca_with_delta_options: typing.Union[RunSnykScaWithDeltaOptions, typing.Dict[builtins.str, typing.Any]],
         install_snyk_options: typing.Optional[typing.Union[InstallSnykOptions, typing.Dict[builtins.str, typing.Any]]] = None,
@@ -8728,15 +8728,15 @@
         :param job_id: 
         :param job_options: 
         :param setup_node_options: 
         :param workflow_name: 
         :param workflow_options: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__681d02162783f2f4359671e9b7f1069d8e16ef884a73dc8636c35bcddef14d7c)
+            type_hints = typing.get_type_hints(_typecheckingstub__3d8a4ececb4d8d1903a494c604219dc078f6d286fc74546d6a33ee74a851e757)
             check_type(argname="argument project", value=project, expected_type=type_hints["project"])
         options = SnykScaWorkflowOptions(
             run_snyk_sca_with_delta_options=run_snyk_sca_with_delta_options,
             install_snyk_options=install_snyk_options,
             job_id=job_id,
             job_options=job_options,
             setup_node_options=setup_node_options,
@@ -8749,15 +8749,15 @@
     @builtins.property
     @jsii.member(jsii_name="workflow")
     def workflow(self) -> typing.Optional[_projen_github_04054675.GithubWorkflow]:
         return typing.cast(typing.Optional[_projen_github_04054675.GithubWorkflow], jsii.get(self, "workflow"))
 
 
 @jsii.data_type(
-    jsii_type="apidays24pj.SnykScaWorkflowOptions",
+    jsii_type="@vianho/apidays24pj.SnykScaWorkflowOptions",
     jsii_struct_bases=[SnykReusableWorkflowOptions],
     name_mapping={
         "install_snyk_options": "installSnykOptions",
         "job_id": "jobId",
         "job_options": "jobOptions",
         "setup_node_options": "setupNodeOptions",
         "workflow_name": "workflowName",
@@ -8793,15 +8793,15 @@
         if isinstance(setup_node_options, dict):
             setup_node_options = SetupNodeOptions(**setup_node_options)
         if isinstance(workflow_options, dict):
             workflow_options = _projen_github_04054675.GithubWorkflowOptions(**workflow_options)
         if isinstance(run_snyk_sca_with_delta_options, dict):
             run_snyk_sca_with_delta_options = RunSnykScaWithDeltaOptions(**run_snyk_sca_with_delta_options)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__2bc23e034505ef53c3ec0d15e65f59f3f7494b2b45f81ad332c0b53e5078c284)
+            type_hints = typing.get_type_hints(_typecheckingstub__d484df1abf5b6a307ccf3a84cb4d33b4249d80c9af4457c6038c42e004ba7474)
             check_type(argname="argument install_snyk_options", value=install_snyk_options, expected_type=type_hints["install_snyk_options"])
             check_type(argname="argument job_id", value=job_id, expected_type=type_hints["job_id"])
             check_type(argname="argument job_options", value=job_options, expected_type=type_hints["job_options"])
             check_type(argname="argument setup_node_options", value=setup_node_options, expected_type=type_hints["setup_node_options"])
             check_type(argname="argument workflow_name", value=workflow_name, expected_type=type_hints["workflow_name"])
             check_type(argname="argument workflow_options", value=workflow_options, expected_type=type_hints["workflow_options"])
             check_type(argname="argument run_snyk_sca_with_delta_options", value=run_snyk_sca_with_delta_options, expected_type=type_hints["run_snyk_sca_with_delta_options"])
@@ -8870,15 +8870,15 @@
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 class SnykWorkflowSteps(
     _projen_github_04054675.WorkflowSteps,
     metaclass=jsii.JSIIMeta,
-    jsii_type="apidays24pj.SnykWorkflowSteps",
+    jsii_type="@vianho/apidays24pj.SnykWorkflowSteps",
 ):
     def __init__(self) -> None:
         '''
         :stability: experimental
         '''
         jsii.create(self.__class__, self, [])
 
@@ -9294,15 +9294,15 @@
 
         return typing.cast(typing.List[_projen_github_workflows_04054675.JobStep], jsii.sinvoke(cls, "setupNode", [options]))
 
 
 class TypescriptProject(
     _projen_typescript_04054675.TypeScriptProject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="apidays24pj.TypescriptProject",
+    jsii_type="@vianho/apidays24pj.TypescriptProject",
 ):
     '''TypeScript project.
 
     :pjid: ts
     '''
 
     def __init__(
@@ -9749,15 +9749,15 @@
             renovatebot_options=renovatebot_options,
         )
 
         jsii.create(self.__class__, self, [options])
 
 
 @jsii.data_type(
-    jsii_type="apidays24pj.TypescriptProjectOptions",
+    jsii_type="@vianho/apidays24pj.TypescriptProjectOptions",
     jsii_struct_bases=[_projen_typescript_04054675.TypeScriptProjectOptions],
     name_mapping={
         "name": "name",
         "commit_generated": "commitGenerated",
         "git_ignore_options": "gitIgnoreOptions",
         "git_options": "gitOptions",
         "logging": "logging",
@@ -10259,15 +10259,15 @@
         if isinstance(tsconfig_dev, dict):
             tsconfig_dev = _projen_javascript_04054675.TypescriptConfigOptions(**tsconfig_dev)
         if isinstance(ts_jest_options, dict):
             ts_jest_options = _projen_typescript_04054675.TsJestOptions(**ts_jest_options)
         if isinstance(snyk_options, dict):
             snyk_options = SnykComponentOptions(**snyk_options)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__6adc172565d72dfb6861a105f8786e402fbc637fa08a5a372bd5b0cdd8a650da)
+            type_hints = typing.get_type_hints(_typecheckingstub__8160d003d5ae6604cf1b9b6ed14b6a721bfbb191b9833c5238df611177ffccf6)
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument commit_generated", value=commit_generated, expected_type=type_hints["commit_generated"])
             check_type(argname="argument git_ignore_options", value=git_ignore_options, expected_type=type_hints["git_ignore_options"])
             check_type(argname="argument git_options", value=git_options, expected_type=type_hints["git_options"])
             check_type(argname="argument logging", value=logging, expected_type=type_hints["logging"])
             check_type(argname="argument outdir", value=outdir, expected_type=type_hints["outdir"])
             check_type(argname="argument parent", value=parent, expected_type=type_hints["parent"])
@@ -12548,88 +12548,88 @@
     "SnykWorkflowSteps",
     "TypescriptProject",
     "TypescriptProjectOptions",
 ]
 
 publication.publish()
 
-def _typecheckingstub__7499bcac71e42b3d0bd6be83ad116500914c3fa1d57c699cd857047452b8b7b5(
+def _typecheckingstub__9d8425126db24c75dc31a21c4b9944e8e2c263e278f1ca0615968eb602d8dd73(
     *,
     env: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     id: typing.Optional[builtins.str] = None,
     if_: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     working_directory: typing.Optional[builtins.str] = None,
     continue_on_error: typing.Optional[builtins.bool] = None,
     timeout_minutes: typing.Optional[jsii.Number] = None,
     snyk_org_id: builtins.str,
     snyk_token: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__6a13eaadc693af6419d337a0a037c1fefe0a413b3f3a3ba6e27ed07f8f93d349(
+def _typecheckingstub__a392f47fe3aac33d0549380cc9fdbfc579a13a3c6d4313275def6f23a9a7ce0d(
     *,
     env: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     id: typing.Optional[builtins.str] = None,
     if_: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     working_directory: typing.Optional[builtins.str] = None,
     continue_on_error: typing.Optional[builtins.bool] = None,
     timeout_minutes: typing.Optional[jsii.Number] = None,
     with_: typing.Union[CreateCacheWithOptions, typing.Dict[builtins.str, typing.Any]],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__ea833d15382a60a8a18d31af670573cb61eaa1a9f5b7c096627d6c11cc8ef345(
+def _typecheckingstub__fc49593c630f79bd92b523141ad72926301b0c4ad5cb531f79d3e6f83fc041ff(
     *,
     key: builtins.str,
     path: builtins.str,
     enable_cross_os_archive: typing.Optional[builtins.bool] = None,
     fail_on_cache_miss: typing.Optional[builtins.bool] = None,
     lookup_only: typing.Optional[builtins.bool] = None,
     restore_keys: typing.Optional[builtins.str] = None,
     save_always: typing.Optional[builtins.bool] = None,
     upload_chunk_size: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__ab43d75f13ad56674e2faec69ea8d19b8f29118c1aeb82b494a76763ab56ebed(
+def _typecheckingstub__2122c06ad20ce5bd6dc82942fed07f8e4747805fcaee09ebd4ff1819404f9b8d(
     project: _projen_04054675.Project,
     file_path: builtins.str,
     *,
     committed: typing.Optional[builtins.bool] = None,
     edit_gitignore: typing.Optional[builtins.bool] = None,
     executable: typing.Optional[builtins.bool] = None,
     marker: typing.Optional[builtins.bool] = None,
     readonly: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__f01c9c292e1b1442fefef01d629b2113fb285d746f6e3bafbc5a9bc8cfb92df3(
+def _typecheckingstub__683b82d7360fc75db810de449d3d4565e455d5e0255f8820ff67019f35661e6e(
     resolver: _projen_04054675.IResolver,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__f20332f9af214ba472ea1e1e5734d15d4a70e549387fbdbced7d8536598f4832(
+def _typecheckingstub__7beb6ebe0c1d59f5dbbab8be19d6e18939c51219feb13da759cb619b8aca716f(
     *,
     committed: typing.Optional[builtins.bool] = None,
     edit_gitignore: typing.Optional[builtins.bool] = None,
     executable: typing.Optional[builtins.bool] = None,
     marker: typing.Optional[builtins.bool] = None,
     readonly: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__c914ee45f7c0eb47e0d9cc31d3686e4310074487655fb96e610c7ef15b35a82c(
+def _typecheckingstub__af3a8e60d04fdfe1def4992e68fe353d0bf2a9ee372438a7959d989c5b8b7911(
     *,
     env: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     id: typing.Optional[builtins.str] = None,
     if_: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     working_directory: typing.Optional[builtins.str] = None,
     continue_on_error: typing.Optional[builtins.bool] = None,
@@ -12638,15 +12638,15 @@
     create_cache_options: typing.Optional[typing.Union[CreateCacheOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     snyk_delta_version: typing.Optional[builtins.str] = None,
     snyk_version: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__f6c6a9712fc3dce9ccf17efe4fa4a84a14ef2a11e7adaa9fba911b2705c621b0(
+def _typecheckingstub__8c703b1b8ea3b49f58bdb97a4a351acc0f376081db036a62df5a1c3c832961f2(
     *,
     env: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     id: typing.Optional[builtins.str] = None,
     if_: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     working_directory: typing.Optional[builtins.str] = None,
     continue_on_error: typing.Optional[builtins.bool] = None,
@@ -12654,15 +12654,15 @@
     cache: typing.Optional[builtins.bool] = None,
     create_cache_options: typing.Optional[typing.Union[CreateCacheOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     version: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__99f139571fd89965ef29bcec365b3acac0d2bf8f80bc6f75c7dbb8935c651ca9(
+def _typecheckingstub__4140b37e76a6e68a146824bfb84673ecf5cbe5081a0931bd2d04361925ab497e(
     *,
     name: builtins.str,
     commit_generated: typing.Optional[builtins.bool] = None,
     git_ignore_options: typing.Optional[typing.Union[_projen_04054675.IgnoreFileOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     git_options: typing.Optional[typing.Union[_projen_04054675.GitOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     logging: typing.Optional[typing.Union[_projen_04054675.LoggerOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     outdir: typing.Optional[builtins.str] = None,
@@ -12821,15 +12821,15 @@
     python: typing.Optional[typing.Union[_projen_cdk_04054675.JsiiPythonTarget, typing.Dict[builtins.str, typing.Any]]] = None,
     rootdir: typing.Optional[builtins.str] = None,
     snyk_options: typing.Optional[typing.Union[SnykComponentOptions, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__1742f76ee2ee1687558699b1f671449ff1d742df6aa5019c85cc6f8fa9e4fea8(
+def _typecheckingstub__12c379aa135bc0e1a1b53c8b5e3594a5a52062eee38868a1a87333f59f2d8074(
     *,
     name: builtins.str,
     commit_generated: typing.Optional[builtins.bool] = None,
     git_ignore_options: typing.Optional[typing.Union[_projen_04054675.IgnoreFileOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     git_options: typing.Optional[typing.Union[_projen_04054675.GitOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     logging: typing.Optional[typing.Union[_projen_04054675.LoggerOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     outdir: typing.Optional[builtins.str] = None,
@@ -12875,15 +12875,15 @@
     sample: typing.Optional[builtins.bool] = None,
     sample_java_package: typing.Optional[builtins.str] = None,
     snyk_options: typing.Optional[typing.Union[SnykComponentOptions, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__957fb874ddb064650932935177b2ea1e011812edad4af8c5a506fc74107ed151(
+def _typecheckingstub__891da87c367c14eb9024685586cafe6a3f10bc82d0da0c9c8a2290953b15ff66(
     *,
     name: builtins.str,
     commit_generated: typing.Optional[builtins.bool] = None,
     git_ignore_options: typing.Optional[typing.Union[_projen_04054675.IgnoreFileOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     git_options: typing.Optional[typing.Union[_projen_04054675.GitOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     logging: typing.Optional[typing.Union[_projen_04054675.LoggerOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     outdir: typing.Optional[builtins.str] = None,
@@ -12939,15 +12939,15 @@
     venv: typing.Optional[builtins.bool] = None,
     venv_options: typing.Optional[typing.Union[_projen_python_04054675.VenvOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     snyk_options: typing.Optional[typing.Union[SnykComponentOptions, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__11b9e25a6f753d83c33e159908b8f7823d99aa6927b697579dedbe900bcd6533(
+def _typecheckingstub__0e002e7132017789d5df99e1716a07debfb5a4e13cbe3068c32c46073c26d346(
     *,
     env: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     id: typing.Optional[builtins.str] = None,
     if_: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     working_directory: typing.Optional[builtins.str] = None,
     continue_on_error: typing.Optional[builtins.bool] = None,
@@ -12955,45 +12955,45 @@
     args: typing.Optional[builtins.str] = None,
     result_path_output_id: typing.Optional[builtins.str] = None,
     severity_threshold: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__9a689218f851a9f5b77288348c6dd48f1baa343882a0c678222c8a6636ca6642(
+def _typecheckingstub__575d1d4a3c76341c42bfb993207158ebe8c83c6d7388f32b24a709d8668ae251(
     *,
     env: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     id: typing.Optional[builtins.str] = None,
     if_: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     working_directory: typing.Optional[builtins.str] = None,
     continue_on_error: typing.Optional[builtins.bool] = None,
     timeout_minutes: typing.Optional[jsii.Number] = None,
     snyk_code_baseline_path: builtins.str,
     snyk_code_current_path: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__917bbfab2f121ac66af4e22af7100b50aaaa08801c6843a48840d1286346a4d7(
+def _typecheckingstub__3a20e44fb24557adba3d97dbfde5a79154b8a9ab953f810991a89123e22c3543(
     *,
     env: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     id: typing.Optional[builtins.str] = None,
     if_: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     working_directory: typing.Optional[builtins.str] = None,
     continue_on_error: typing.Optional[builtins.bool] = None,
     timeout_minutes: typing.Optional[jsii.Number] = None,
     authenticate_snyk_options: typing.Union[AuthenticateSnykOptions, typing.Dict[builtins.str, typing.Any]],
     severity_threshold: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__a0e8186f614b238d0b08b946ae63cd32cb9914849433387a41d2e306d36c67a2(
+def _typecheckingstub__2878c4b2368eb6494231041317e9ed6bf275d47abadbe16f1a77b49d6ec85db1(
     *,
     env: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     id: typing.Optional[builtins.str] = None,
     if_: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     working_directory: typing.Optional[builtins.str] = None,
     continue_on_error: typing.Optional[builtins.bool] = None,
@@ -13004,25 +13004,25 @@
     delta: typing.Optional[builtins.bool] = None,
     run_sca_options: typing.Optional[typing.Union[RunScaOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     severity_threshold: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__14ab5340a54ed05a3cb521aeea6091c331fce3b554cd4e4c909171f54789320f(
+def _typecheckingstub__9ae80cfd938bfb79f63f4a9a860a04c3006dc3ccd21d42cf92f8198523654977(
     project: typing.Union[_projen_java_04054675.JavaProject, _projen_python_04054675.PythonProject, _projen_javascript_04054675.NodeProject, _projen_cdk_04054675.JsiiProject],
     name: builtins.str,
     *,
     triggers_options: typing.Optional[typing.Union[_projen_github_workflows_04054675.Triggers, typing.Dict[builtins.str, typing.Any]]] = None,
     workflow_options: typing.Optional[typing.Union[_projen_github_04054675.GithubWorkflowOptions, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__82feaffcc0c7354797b7c8f3bf82188f862a51d27e911f2c5483eb544f1fb8c0(
+def _typecheckingstub__418456736145bcec36319c90fb181c090b70c624edbcae96557ca2dd9f391ffb(
     id: builtins.str,
     path: builtins.str,
     *,
     actions: typing.Optional[_projen_github_workflows_04054675.JobPermission] = None,
     checks: typing.Optional[_projen_github_workflows_04054675.JobPermission] = None,
     contents: typing.Optional[_projen_github_workflows_04054675.JobPermission] = None,
     deployments: typing.Optional[_projen_github_workflows_04054675.JobPermission] = None,
@@ -13035,78 +13035,78 @@
     repository_projects: typing.Optional[_projen_github_workflows_04054675.JobPermission] = None,
     security_events: typing.Optional[_projen_github_workflows_04054675.JobPermission] = None,
     statuses: typing.Optional[_projen_github_workflows_04054675.JobPermission] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__79146a50fc97b2474e8fa5d43d64887475e1b3e9e55efe88b25958358bcff36a(
+def _typecheckingstub__affb2f3a02329f30fc70b12e8e5900f22b8648704b40143dd25429bec544044a(
     *,
     triggers_options: typing.Optional[typing.Union[_projen_github_workflows_04054675.Triggers, typing.Dict[builtins.str, typing.Any]]] = None,
     workflow_options: typing.Optional[typing.Union[_projen_github_04054675.GithubWorkflowOptions, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__68437243d81c9e0bb8cc2233867ed1a1270df2657cc2c32243091d7a780f36cb(
+def _typecheckingstub__fc17ca199138f9ea8093446b733610b42f8c339c77c56ceb1b626a53b8e26562(
     *,
     env: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     id: typing.Optional[builtins.str] = None,
     if_: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     working_directory: typing.Optional[builtins.str] = None,
     continue_on_error: typing.Optional[builtins.bool] = None,
     timeout_minutes: typing.Optional[jsii.Number] = None,
     node_version: typing.Optional[jsii.Number] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__059eec1cd4997b382e2a9b22feecdc034c8dfdd4dfe116062f6e386b6a9ac532(
+def _typecheckingstub__cb405cdef6274681176612f421e28f571baaff0cd9d30c2f1ede9822b654f1ef(
     project: typing.Union[_projen_java_04054675.JavaProject, _projen_python_04054675.PythonProject, _projen_javascript_04054675.NodeProject, _projen_cdk_04054675.JsiiProject],
     *,
     enable_sast: typing.Optional[builtins.bool] = None,
     enable_sca: typing.Optional[builtins.bool] = None,
     security_scan_workflow_options: typing.Optional[typing.Union[SecurityScanWorkflowOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     snyk_monitored_project_id: typing.Optional[builtins.str] = None,
     snyk_org_id: typing.Optional[builtins.str] = None,
     snyk_sast_workflow_options: typing.Optional[typing.Union[SnykSastWorkflowOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     snyk_sca_workflow_options: typing.Optional[typing.Union[SnykScaWorkflowOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     workflow_name: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__bd92fc73698543f9e46a0f483f66bb3f257d5458e779fd8ec087394cd49b8447(
+def _typecheckingstub__dfd8814387fc6585660859797326036165cb9d67939e2e0e13f90d855e01e9ab(
     *,
     enable_sast: typing.Optional[builtins.bool] = None,
     enable_sca: typing.Optional[builtins.bool] = None,
     security_scan_workflow_options: typing.Optional[typing.Union[SecurityScanWorkflowOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     snyk_monitored_project_id: typing.Optional[builtins.str] = None,
     snyk_org_id: typing.Optional[builtins.str] = None,
     snyk_sast_workflow_options: typing.Optional[typing.Union[SnykSastWorkflowOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     snyk_sca_workflow_options: typing.Optional[typing.Union[SnykScaWorkflowOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     workflow_name: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__b50419a73c6742644b189527cac822f77473cd6b0675087d8b1d801310fb9039(
+def _typecheckingstub__7b881678ff7dd868659f80d530f797e51f8f508403b2f9318fc66e11b3954817(
     *,
     install_snyk_options: typing.Optional[typing.Union[InstallSnykOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     job_id: typing.Optional[builtins.str] = None,
     job_options: typing.Optional[typing.Union[_projen_github_workflows_04054675.Job, typing.Dict[builtins.str, typing.Any]]] = None,
     setup_node_options: typing.Optional[typing.Union[SetupNodeOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     workflow_name: typing.Optional[builtins.str] = None,
     workflow_options: typing.Optional[typing.Union[_projen_github_04054675.GithubWorkflowOptions, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__0421a1e8469318296b8cc8e91d45895ca74a274f088ac3bdc6d19d2281e6b36b(
+def _typecheckingstub__ee34abce9cb44b5c5b5b29fb7aa65f997c1c2b7ec3f23a82ee4c54838ac3daf8(
     project: typing.Union[_projen_java_04054675.JavaProject, _projen_python_04054675.PythonProject, _projen_javascript_04054675.NodeProject, _projen_cdk_04054675.JsiiProject],
     *,
     authenticate_snyk_options: typing.Union[AuthenticateSnykOptions, typing.Dict[builtins.str, typing.Any]],
     checkout_baseline_options: typing.Optional[typing.Union[_projen_github_04054675.CheckoutOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     checkout_current_options: typing.Optional[typing.Union[_projen_github_04054675.CheckoutOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     delta: typing.Optional[builtins.bool] = None,
     download_artifact_options: typing.Optional[typing.Union[_projen_github_04054675.DownloadArtifactOptions, typing.Dict[builtins.str, typing.Any]]] = None,
@@ -13120,15 +13120,15 @@
     setup_node_options: typing.Optional[typing.Union[SetupNodeOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     workflow_name: typing.Optional[builtins.str] = None,
     workflow_options: typing.Optional[typing.Union[_projen_github_04054675.GithubWorkflowOptions, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__e1b27431bdc247ac8f74dec999d67a7ae3c97832ce49550a65941fe558640f78(
+def _typecheckingstub__fad9c203a45cfe324b94f121d928c27f1be1e11663352b77d79f7874b5e22510(
     *,
     install_snyk_options: typing.Optional[typing.Union[InstallSnykOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     job_id: typing.Optional[builtins.str] = None,
     job_options: typing.Optional[typing.Union[_projen_github_workflows_04054675.Job, typing.Dict[builtins.str, typing.Any]]] = None,
     setup_node_options: typing.Optional[typing.Union[SetupNodeOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     workflow_name: typing.Optional[builtins.str] = None,
     workflow_options: typing.Optional[typing.Union[_projen_github_04054675.GithubWorkflowOptions, typing.Dict[builtins.str, typing.Any]]] = None,
@@ -13141,42 +13141,42 @@
     run_snyk_sast_baseline_options: typing.Optional[typing.Union[RunSnykSastOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     run_snyk_sast_current_options: typing.Optional[typing.Union[RunSnykSastOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     upload_artifact_options: typing.Optional[typing.Union[_projen_github_04054675.UploadArtifactOptions, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__681d02162783f2f4359671e9b7f1069d8e16ef884a73dc8636c35bcddef14d7c(
+def _typecheckingstub__3d8a4ececb4d8d1903a494c604219dc078f6d286fc74546d6a33ee74a851e757(
     project: typing.Union[_projen_java_04054675.JavaProject, _projen_python_04054675.PythonProject, _projen_javascript_04054675.NodeProject, _projen_cdk_04054675.JsiiProject],
     *,
     run_snyk_sca_with_delta_options: typing.Union[RunSnykScaWithDeltaOptions, typing.Dict[builtins.str, typing.Any]],
     install_snyk_options: typing.Optional[typing.Union[InstallSnykOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     job_id: typing.Optional[builtins.str] = None,
     job_options: typing.Optional[typing.Union[_projen_github_workflows_04054675.Job, typing.Dict[builtins.str, typing.Any]]] = None,
     setup_node_options: typing.Optional[typing.Union[SetupNodeOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     workflow_name: typing.Optional[builtins.str] = None,
     workflow_options: typing.Optional[typing.Union[_projen_github_04054675.GithubWorkflowOptions, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__2bc23e034505ef53c3ec0d15e65f59f3f7494b2b45f81ad332c0b53e5078c284(
+def _typecheckingstub__d484df1abf5b6a307ccf3a84cb4d33b4249d80c9af4457c6038c42e004ba7474(
     *,
     install_snyk_options: typing.Optional[typing.Union[InstallSnykOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     job_id: typing.Optional[builtins.str] = None,
     job_options: typing.Optional[typing.Union[_projen_github_workflows_04054675.Job, typing.Dict[builtins.str, typing.Any]]] = None,
     setup_node_options: typing.Optional[typing.Union[SetupNodeOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     workflow_name: typing.Optional[builtins.str] = None,
     workflow_options: typing.Optional[typing.Union[_projen_github_04054675.GithubWorkflowOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     run_snyk_sca_with_delta_options: typing.Union[RunSnykScaWithDeltaOptions, typing.Dict[builtins.str, typing.Any]],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__6adc172565d72dfb6861a105f8786e402fbc637fa08a5a372bd5b0cdd8a650da(
+def _typecheckingstub__8160d003d5ae6604cf1b9b6ed14b6a721bfbb191b9833c5238df611177ffccf6(
     *,
     name: builtins.str,
     commit_generated: typing.Optional[builtins.bool] = None,
     git_ignore_options: typing.Optional[typing.Union[_projen_04054675.IgnoreFileOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     git_options: typing.Optional[typing.Union[_projen_04054675.GitOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     logging: typing.Optional[typing.Union[_projen_04054675.LoggerOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     outdir: typing.Optional[builtins.str] = None,
```

### Comparing `apidays24pj-0.0.8/src/apidays24pj.egg-info/PKG-INFO` & `apidays24pj-0.0.9/src/apidays24pj.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: apidays24pj
-Version: 0.0.8
-Summary: apidays24pj
+Version: 0.0.9
+Summary: @vianho/apidays24pj
 Home-page: https://github.com/vianho/projen-projects
 Author: Silviana<email@example.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/vianho/projen-projects
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
```

