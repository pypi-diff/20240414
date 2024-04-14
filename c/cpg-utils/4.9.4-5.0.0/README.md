# Comparing `tmp/cpg-utils-4.9.4.tar.gz` & `tmp/cpg-utils-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpg-utils-4.9.4.tar", last modified: Wed Oct 26 05:43:42 2022, max compression
+gzip compressed data, was "cpg-utils-5.0.0.tar", last modified: Sun Apr 14 09:33:50 2024, max compression
```

## Comparing `cpg-utils-4.9.4.tar` & `cpg-utils-5.0.0.tar`

### file list

```diff
@@ -1,38 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 05:43:42.506573 cpg-utils-4.9.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1590 2022-10-26 05:43:42.506573 cpg-utils-4.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      818 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 05:43:42.506573 cpg-utils-4.9.4/cpg_utils/
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10435 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/cloud.py
--rw-r--r--   0 runner    (1001) docker     (121)     3477 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/cloudpath_hail_az.py
--rw-r--r--   0 runner    (1001) docker     (121)     9480 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/config-template.toml
--rw-r--r--   0 runner    (1001) docker     (121)     4094 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     8110 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/git.py
--rw-r--r--   0 runner    (1001) docker     (121)    20487 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/hail_batch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 05:43:42.506573 cpg-utils-4.9.4/cpg_utils/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6897 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/workflows/batch.py
--rw-r--r--   0 runner    (1001) docker     (121)     6618 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/workflows/filetypes.py
--rw-r--r--   0 runner    (1001) docker     (121)     8758 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/workflows/inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    24422 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/workflows/metamist.py
--rw-r--r--   0 runner    (1001) docker     (121)    10250 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/workflows/resources.py
--rw-r--r--   0 runner    (1001) docker     (121)     2306 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/workflows/slack.py
--rw-r--r--   0 runner    (1001) docker     (121)     5552 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/workflows/status.py
--rw-r--r--   0 runner    (1001) docker     (121)    19302 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/workflows/targets.py
--rw-r--r--   0 runner    (1001) docker     (121)     4092 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/workflows/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    39375 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/workflows/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 05:43:42.506573 cpg-utils-4.9.4/cpg_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1590 2022-10-26 05:43:42.000000 cpg-utils-4.9.4/cpg_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      790 2022-10-26 05:43:42.000000 cpg-utils-4.9.4/cpg_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 05:43:42.000000 cpg-utils-4.9.4/cpg_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-10-26 05:43:42.000000 cpg-utils-4.9.4/cpg_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-26 05:43:42.000000 cpg-utils-4.9.4/cpg_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-26 05:43:42.506573 cpg-utils-4.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1698 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 05:43:42.506573 cpg-utils-4.9.4/test/
--rw-r--r--   0 runner    (1001) docker     (121)     2777 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/test/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (121)     8393 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/test/test_cohort.py
--rw-r--r--   0 runner    (1001) docker     (121)     3322 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/test/test_status.py
--rw-r--r--   0 runner    (1001) docker     (121)     3815 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/test/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:33:50.945660 cpg-utils-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-14 09:33:47.000000 cpg-utils-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-14 09:33:50.945660 cpg-utils-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-14 09:33:47.000000 cpg-utils-5.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:33:50.941660 cpg-utils-5.0.0/cpg_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-14 09:33:47.000000 cpg-utils-5.0.0/cpg_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14297 2024-04-14 09:33:47.000000 cpg-utils-5.0.0/cpg_utils/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-14 09:33:47.000000 cpg-utils-5.0.0/cpg_utils/cloudpath_hail_az.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16312 2024-04-14 09:33:47.000000 cpg-utils-5.0.0/cpg_utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-14 09:33:47.000000 cpg-utils-5.0.0/cpg_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26173 2024-04-14 09:33:47.000000 cpg-utils-5.0.0/cpg_utils/cromwell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13237 2024-04-14 09:33:47.000000 cpg-utils-5.0.0/cpg_utils/cromwell_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-04-14 09:33:47.000000 cpg-utils-5.0.0/cpg_utils/dataproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-04-14 09:33:47.000000 cpg-utils-5.0.0/cpg_utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-04-14 09:33:47.000000 cpg-utils-5.0.0/cpg_utils/hail_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-14 09:33:47.000000 cpg-utils-5.0.0/cpg_utils/membership.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 09:33:47.000000 cpg-utils-5.0.0/cpg_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-14 09:33:47.000000 cpg-utils-5.0.0/cpg_utils/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:33:50.941660 cpg-utils-5.0.0/cpg_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-14 09:33:50.000000 cpg-utils-5.0.0/cpg_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-14 09:33:50.000000 cpg-utils-5.0.0/cpg_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 09:33:50.000000 cpg-utils-5.0.0/cpg_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-14 09:33:50.000000 cpg-utils-5.0.0/cpg_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-14 09:33:50.000000 cpg-utils-5.0.0/cpg_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-14 09:33:47.000000 cpg-utils-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 09:33:50.945660 cpg-utils-5.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1177 2024-04-14 09:33:47.000000 cpg-utils-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:33:50.945660 cpg-utils-5.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 09:33:47.000000 cpg-utils-5.0.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-04-14 09:33:47.000000 cpg-utils-5.0.0/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-14 09:33:47.000000 cpg-utils-5.0.0/test/test_cromwell.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-14 09:33:47.000000 cpg-utils-5.0.0/test/test_doctests.py
```

### Comparing `cpg-utils-4.9.4/LICENSE` & `cpg-utils-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cpg-utils-4.9.4/PKG-INFO` & `cpg-utils-5.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpg-utils
-Version: 4.9.4
+Version: 5.0.0
 Summary: Library of convenience functions specific to the CPG
 Home-page: https://github.com/populationgenomics/cpg-utils
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -12,16 +12,14 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: workflows
 License-File: LICENSE
 
 # cpg-utils
 
 This is a Python library containing convenience functions that are specific to the CPG.
 
 In order to install the library in a conda environment, run:
@@ -31,15 +29,15 @@
 ```
 
 To use the library, import functions like this:
 
 ```python
 from cpg_utils.cloud import email_from_id_token
 
-_email_string = email_from_id_token(id_token='TOKEN_STRING')
+_email_string = email_from_id_token(id_token_jwt='TOKEN_STRING')
 ```
 
 We use `bumpversion` for incrementing the library's semantic version. A new conda package gets published automatically in the `cpg` conda channel whenever a version bump commit is merged with the `main` branch.
 
 
 ## Contents
```

### Comparing `cpg-utils-4.9.4/README.md` & `cpg-utils-5.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ```
 
 To use the library, import functions like this:
 
 ```python
 from cpg_utils.cloud import email_from_id_token
 
-_email_string = email_from_id_token(id_token='TOKEN_STRING')
+_email_string = email_from_id_token(id_token_jwt='TOKEN_STRING')
 ```
 
 We use `bumpversion` for incrementing the library's semantic version. A new conda package gets published automatically in the `cpg` conda channel whenever a version bump commit is merged with the `main` branch.
 
 
 ## Contents
```

### Comparing `cpg-utils-4.9.4/cpg_utils/__init__.py` & `cpg-utils-5.0.0/cpg_utils/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
 CPG utils
 """
+
 import pathlib
-from typing import Union
 
 from cloudpathlib import CloudPath
 from cloudpathlib.anypath import to_anypath
 
-
 # The AnyPath class https://cloudpathlib.drivendata.org/stable/anypath-polymorphism/
 # is very handy to parse a string that can be either a cloud URL or a local posix path.
 # However, AnyPath can't be used for type hinting, because neither CloudPath nor
 # pathlib.Path derive from it. The AnyPath's constructor method doesn't actually return
 # an instance of AnyPath class, but rather Union[CloudPath, pathlib.Path], and it's
 # designed to dynamically pick a specific CloudPath or pathlib.Path subclass.
 # Here we create an alias for such union to allow using simple "Path" in type hints:
-Path = Union[CloudPath, pathlib.Path]
+Path = CloudPath | pathlib.Path
 
 # We would still need to call AnyPath() to parse a string, which might be confusing.
 # Something like to_path() would look better, so we are aliasing a handy method
 # to_anypath to to_path, which returns exactly the Union type we are looking for:
 to_path = to_anypath
```

### Comparing `cpg-utils-4.9.4/cpg_utils/cloudpath_hail_az.py` & `cpg-utils-5.0.0/cpg_utils/cloudpath_hail_az.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """
 Extend cloudpathlib Azure implementation to support hail-az:// scheme.
 Inspired by https://github.com/drivendataorg/cloudpathlib/issues/157
 """
 
 import re
-from typing import Union, Optional
 from urllib.parse import urlparse
 
 from cloudpathlib import AzureBlobClient, AzureBlobPath
 from cloudpathlib.client import register_client_class
-from cloudpathlib.cloudpath import register_path_class, CloudPath
+from cloudpathlib.cloudpath import CloudPath, register_path_class
 from cloudpathlib.exceptions import InvalidPrefixError
 
 
 @register_client_class('hail-az')
 class HailAzureBlobClient(AzureBlobClient):
     """
     Client is identical to the base Azure implementation.
@@ -31,17 +30,17 @@
     """
 
     cloud_prefix: str = 'hail-az://'
     client: 'HailAzureBlobClient'
 
     def __init__(
         self,
-        cloud_path: Union[str, CloudPath],
-        client: Optional[AzureBlobClient] = None,
-        token: Optional[str] = None,
+        cloud_path: str | CloudPath,
+        client: AzureBlobClient | None = None,
+        token: str | None = None,
     ):
         if isinstance(cloud_path, str):
             parsed = urlparse(cloud_path)
             m = re.match(
                 r'(?P<account>[a-z0-9]+)(\.(?P<type>blob|dfs)(\.core\.windows\.net)?)?',
                 parsed.netloc,
                 flags=re.IGNORECASE,
@@ -68,30 +67,32 @@
                     token = '?' + parsed.query
                 client = HailAzureBlobClient(account_url, token)
 
         super().__init__(cloud_path, client=client)
 
     @classmethod
     def is_valid_cloudpath(
-        cls, path: Union[str, CloudPath], raise_on_error=False
+        cls,
+        path: str | CloudPath,
+        raise_on_error: bool = False,
     ) -> bool:
         """
         Also allowing HTTP.
         """
         valid = bool(
             re.match(
                 fr'({HailAzureBlobPath.cloud_prefix}|https://[a-z0-9]+\.(blob|dfs)\.core\.windows\.net)',
                 str(path).lower(),
-            )
+            ),
         )
 
         if raise_on_error and not valid:
             raise InvalidPrefixError(
                 f'{path} is not a valid path since it does not start with {cls.cloud_prefix} '
-                f'or valid Azure https blob or dfs location.'
+                f'or valid Azure https blob or dfs location.',
             )
 
         return valid
 
     @property
     def container(self) -> str:
         """
```

### Comparing `cpg-utils-4.9.4/cpg_utils/git.py` & `cpg-utils-5.0.0/cpg_utils/git.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 """
 Helper functions for working with Git repositories
 """
 
-
-from typing import List
-
 import os
 import re
 import subprocess
-from shlex import quote
 
+from cpg_utils.constants import DEFAULT_GITHUB_ORGANISATION
 
-def get_output_of_command(command: List[str], description: str) -> str:
+
+def get_output_of_command(command: list[str], description: str) -> str:
     """
     subprocess.check_output wrapper that returns string output and raises detailed
     exceptions on error.
 
     Parameters
     ----------
     command:     list of strings creating a full command
@@ -23,26 +21,26 @@
 
     Returns
     -------
     stripped output string if command was successful
 
     """
     try:
-        return subprocess.check_output(command).decode().strip()
+        return subprocess.check_output(command).decode().strip()  # noqa: S603
     # Handle and rethrow KeyboardInterrupt error to stop global exception catch
-    # pylint: disable=try-except-raise
+
     except KeyboardInterrupt:
         raise
     except subprocess.CalledProcessError as e:
-        raise Exception(
-            f"Couldn't call {description} by calling '{' '.join(command)}', {e}"
+        raise OSError(
+            f"Couldn't call {description} by calling '{' '.join(command)}', {e}",
         ) from e
-    except Exception as e:
-        raise Exception(
-            f"Couldn't process {description} through calling '{' '.join(command)}', {e}"
+    except Exception as e:  # noqa: BLE001
+        raise type(e)(
+            f"Couldn't process {description} through calling '{' '.join(command)}', {e}",
         ) from e
 
 
 def get_relative_script_path_from_git_root(script_name: str) -> str:
     """
     If we're in a subdirectory, get the relative path from the git root
     to the current directory, and append the script path.
@@ -89,30 +87,42 @@
     e.g. /Users/foo/repos/cpg-utils
 
     Returns
     -------
 
     """
     command = ['git', 'rev-parse', '--show-toplevel']
-    repo_root = get_output_of_command(command, 'get Git repo directory')
-    return repo_root
+    return get_output_of_command(command, 'get Git repo directory')
 
 
 def get_git_commit_ref_of_current_repository() -> str:
     """
     Returns the commit SHA at the current HEAD
 
     Returns
     -------
 
     """
     command = ['git', 'rev-parse', 'HEAD']
     return get_output_of_command(command, 'get latest Git commit')
 
 
+def get_git_branch_name() -> str | None:
+    """Returns the current branch name."""
+    command = ['git', 'rev-parse', '--abbrev-ref', 'HEAD']
+    try:
+        value = subprocess.check_output(command).decode().strip()  # noqa: S603
+        if value:
+            return value
+    except Exception:  # noqa: BLE001
+        return None
+
+    return None
+
+
 def get_repo_name_from_current_directory() -> str:
     """
     Gets the repo name from the default remote
 
     Returns
     -------
 
@@ -130,19 +140,20 @@
     return get_organisation_name_from_remote(get_git_default_remote())
 
 
 def get_organisation_name_from_remote(remote_name: str) -> str:
     """
     Takes the GitHub repo path and obtains the source organisation
     based on its remote URL e.g.:
-    >>> get_repo_name_from_remote(\
+    >>> get_organisation_name_from_remote(\
         'git@github.com:populationgenomics/cpg-utils.git'\
     )
     'populationgenomics'
-    >>> get_repo_name_from_remote(\
+
+    >>> get_organisation_name_from_remote(\
         'https://github.com/populationgenomics/cpg-utils.git'\
     )
     'populationgenomics'
 
     Parameters
     ----------
     remote_name
@@ -153,35 +164,36 @@
     """
 
     organisation = None
 
     try:
         if remote_name.startswith('http'):
             match = re.match(
-                r'http[s]?:\/\/[A-z0-9\.]+?\/(?P<org>.+?)\/.+$', remote_name
+                r'http[s]?:\/\/[A-Za-z0-9._-]+?\/(?P<org>.+?)\/.+$',
+                remote_name,
             )
             if match:
                 organisation = match.group('org')
 
         elif remote_name.startswith('git@'):
-            match = re.match(r'git@[A-z0-9\.]+?:(?P<org>.+?)\/.+$', remote_name)
+            match = re.match(r'git@[A-Aa-z0-9.+-]+?:(?P<org>.+?)\/.+$', remote_name)
             if match:
                 organisation = match.group('org')
     except AttributeError as ae:
-        raise Exception(f'Unsupported remote format: "{remote_name}"') from ae
+        raise ValueError(f'Unsupported remote format: "{remote_name}"') from ae
 
     if organisation is None:
-        raise Exception(f'Unsupported remote format: "{remote_name}"')
+        raise ValueError(f'Unsupported remote format: "{remote_name}"')
 
     return organisation
 
 
 def get_repo_name_from_remote(remote_name: str) -> str:
     """
-    Get the name of a GitHub repo from a supported organization
+    Get the name of a GitHub repo from a supported organisation
     based on its remote URL e.g.:
     >>> get_repo_name_from_remote(\
         'git@github.com:populationgenomics/cpg-utils.git'\
     )
     'cpg-utils'
     >>> get_repo_name_from_remote(\
         'https://github.com/populationgenomics/cpg-utils.git'\
@@ -193,28 +205,29 @@
     potentially harmful code
     """
 
     repo = None
     try:
         if remote_name.startswith('http'):
             match = re.match(
-                r'http[s]?:\/\/[A-z0-9\.]+?\/.+?\/(?P<repo>.+)$', remote_name
+                r'http[s]?:\/\/[A-Za-z0-9_.-]+?\/.+?\/(?P<repo>.+)$',
+                remote_name,
             )
             if match:
                 repo = match.group('repo')
 
         elif remote_name.startswith('git@'):
-            match = re.match(r'git@[A-z0-9\.]+?:.+?\/(?P<repo>.+)$', remote_name)
+            match = re.match(r'git@[A-Za-z0-9_.-]+?:.+?/(?P<repo>.+)$', remote_name)
             if match:
                 repo = match.group('repo')
     except AttributeError as ae:
-        raise Exception(f'Unsupported remote format: "{remote_name}"') from ae
+        raise ValueError(f'Unsupported remote format: "{remote_name}"') from ae
 
     if repo is None:
-        raise Exception(f'Unsupported remote format: "{remote_name}"')
+        raise ValueError(f'Unsupported remote format: "{remote_name}"')
 
     if repo.endswith('.git'):
         repo = repo[:-4]
 
     return repo
 
 
@@ -230,63 +243,70 @@
 
     Returns
     -------
 
     """
     command = ['git', 'branch', '-r', '--contains', commit]
     try:
-        ret = subprocess.check_output(command)
+        ret = subprocess.check_output(command)  # noqa: S603
         return bool(ret)
     except subprocess.CalledProcessError:
         return False
 
 
-def prepare_git_job(
-    job,
-    organisation: str,
-    repo_name: str,
-    commit: str,
-    is_test: bool = True,
-    print_all_statements: bool = True,
-):
-    """
-    Takes a hail batch job, and:
-        * Clones the repository
-            * if access_level != "test": check the desired commit is on 'main'
-        * Check out the specific commit
+def guess_script_name_from_script_argument(script: list[str]) -> str | None:
+    """
+    Guess the script name from the first argument of the script.
+    If the first argument is an executable, try the second param
 
-    Parameters
-    ----------
-    job                     - A hail BashJob
-    organisation            - The GitHub individual or organisation
-    repo_name               - The repository name to check out
-    commit                  - The commit hash to check out
-    is_test                 - CPG specific: only Main commits can run on Main data
-    print_all_statements    - logging toggle
+    >>> guess_script_name_from_script_argument(['python', 'main.py'])
+    'main.py'
+
+    >>> guess_script_name_from_script_argument(['./main.sh'])
+    'main.sh'
+
+    >>> guess_script_name_from_script_argument(['main.sh'])
+    'main.sh'
+
+    >>> guess_script_name_from_script_argument(['./test/path/main.sh', 'arg1', 'arg2'])
+    'test/path/main.sh'
+
+    >>> guess_script_name_from_script_argument(['gcloud', 'cp' 'test']) is None
+    True
 
-    Returns
-    -------
-    No return required
     """
+    executables = {'python', 'python3', 'bash', 'sh', 'rscript'}
+    _script = script[0]
+    if _script.lower() in executables:
+        _script = script[1]
 
-    # Use "set -x" to print the commands for easier debugging.
-    if print_all_statements:
-        job.command('set -x')
-
-    # Note: for private GitHub repos we'd need to use a token to clone.
-    # Any job commands here are evaluated in a bash shell, so user arguments should
-    # be escaped to avoid command injection.
-    job.command(
-        f'git clone --recurse-submodules https://github.com/{quote(organisation)}/{quote(repo_name)}.git'
-    )
-    job.command(f'cd {quote(repo_name)}')
+    if _script.startswith('./'):
+        return _script[2:]
+
+    # a very bad check if it follows format "file.ext"
+    if '.' in _script:
+        return _script
+
+    return None
+
+
+def guess_script_github_url_from(
+    *,
+    repo: str | None,
+    commit: str | None,
+    cwd: str | None,
+    script: list[str],
+    organisation: str = DEFAULT_GITHUB_ORGANISATION,
+) -> str | None:
+    """
+    Guess the GitHub URL of the script from the given arguments.
+    """
+    guessed_script_name = guess_script_name_from_script_argument(script)
+    if not guessed_script_name:
+        return None
+
+    url = f'https://github.com/{organisation}/{repo}/tree/{commit}'
+
+    if cwd == '.' or cwd is None:
+        return f'{url}/{guessed_script_name}'
 
-    # Except for the "test" access level, we check whether commits have been
-    # reviewed by verifying that the given commit is in the main branch.
-    if not is_test:
-        job.command('git checkout main')
-        job.command(
-            f'git merge-base --is-ancestor {quote(commit)} HEAD || '
-            '{ echo "error: commit not merged into main branch"; exit 1; }'
-        )
-    job.command(f'git checkout {quote(commit)}')
-    job.command(f'git submodule update')
+    return os.path.join(url, cwd, guessed_script_name)
```

### Comparing `cpg-utils-4.9.4/cpg_utils/workflows/slack.py` & `cpg-utils-5.0.0/cpg_utils/slack.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,83 +1,79 @@
 """
-Sending notifications to Slack. To enable, create a channel, add "Seqr Loader" app
-into a channel with:
+Sending notifications to Slack. To enable, create a channel, then add a
+corresponding Slack app (e.g. Seqr Loader) to the channel:
 
 /invite @Seqr Loader
 
 Make sure `slack/channel`, `slack/token_secret_id`, and `slack/token_project_id`
 configuration values are set.
 """
 
-from textwrap import dedent
+import logging
+
+try:
+    import slack_sdk
+except ImportError:
+    slack_sdk = None
 
 from cpg_utils.cloud import read_secret
-from cpg_utils.config import get_config
+from cpg_utils.config import config_retrieve
+
+
+def _get_slack_sdk():  # noqa: ANN202
+    if slack_sdk:
+        return slack_sdk
+
+    raise ImportError("slack_sdk is not installed")
+
 
-from hailtop.batch.job import Job
+def _get_channel() -> str:
+    """Returns the Slack channel from the config."""
+    slack_channel = config_retrieve(['slack', 'channel'], default=None)
+    if not slack_channel:
+        raise ValueError('`slack.channel` must be set in config')
+    return slack_channel
 
 
-def get_token() -> str:
-    """
-    Returns Slack token.
-    """
-    token_secret_id = get_config()['slack'].get('token_secret_id')
-    token_project_id = get_config()['slack'].get('token_project_id')
+def _get_token() -> str:
+    """Returns the Slack token from the config."""
+    token_secret_id = config_retrieve(['slack', 'token_secret_id'], default=None)
+    token_project_id = config_retrieve(['slack', 'token_project_id'], default=None)
+
     if not token_secret_id or not token_project_id:
         raise ValueError(
             '`slack.token_secret_id` and `slack.token_project_id` '
-            'must be set in config to retrieve Slack token'
+            'must be set in config to retrieve Slack token',
         )
-    token = read_secret(
+    slack_token = read_secret(
         project_id=token_project_id,
         secret_name=token_secret_id,
         fail_gracefully=False,
     )
-    assert token
-    return token
+    if slack_token is None:
+        raise ValueError('Failed to retrieve Slack token')
+    return slack_token
 
 
-def slack_env(j: Job):
-    """
-    Add environment variables that configure Slack reporter.
-    """
-    if not (channel := get_config().get('slack', {}).get('channel')):
-        return None
-    j.env('SLACK_CHANNEL', channel)
-    j.env('SLACK_TOKEN', get_token())
-
-
-def slack_message_cmd(
-    j: Job,
-    text: str | None = None,
-    data: dict[str, str] | None = None,
-):
-    """
-    Make a bash command that prepares and sends a Slack message.
-    Message can be constructed from a dict `data`, or can be passed directly
-    as text (`text`). In either case, strings can use Slack `mrkdwn`
-    for formatting: https://api.slack.com/reference/surfaces/formatting
-
-    Assumes `slack/channel` configuration parameter is set, as well as
-    SLACK_TOKEN environment variable.
-    """
-    if not (channel := get_config()['slack'].get('channel')):
-        return ''
-    msg = ''
-    if data:
-        msg += '\\n'.join(f'{k}: {v}' for k, v in data.items())
-    if text:
-        msg += f'\\n{text}'
-    if not msg:
-        return ''
-    slack_env(j)
-    j.command(
-        dedent(
-            f"""
-    curl -X POST \
-    -H "Authorization: Bearer {get_token()}" \
-    -H "Content-type: application/json" \
-    -d '{{"channel": "'{channel}'", "text": "{msg}"}}' \
-    https://slack.com/api/chat.postMessage
-    """
+def send_message(text: str) -> None:
+    """Sends `text` as a Slack message, reading credentials from the config."""
+    slack_client = _get_slack_sdk().WebClient(token=_get_token())
+    try:
+        slack_client.chat_postMessage(
+            channel=_get_channel(),
+            text=text,
         )
-    )
+    except _get_slack_sdk().errors.SlackApiError as err:
+        logging.error(f'Error posting to Slack: {err}')
+
+
+def upload_file(content: bytes, comment: str) -> None:
+    """Uploads `content` to Slack with the given text `comment`, reading credentials from the config."""
+    slack_client = _get_slack_sdk().WebClient(token=_get_token())
+    try:
+        slack_client.files_upload(
+            channels=_get_channel(),
+            content=content,
+            initial_comment=comment,
+        )
+    except _get_slack_sdk().errors.SlackApiError as err:
+        logging.error(f'Error posting to Slack: {err}')
```

### Comparing `cpg-utils-4.9.4/cpg_utils.egg-info/PKG-INFO` & `cpg-utils-5.0.0/cpg_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpg-utils
-Version: 4.9.4
+Version: 5.0.0
 Summary: Library of convenience functions specific to the CPG
 Home-page: https://github.com/populationgenomics/cpg-utils
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -12,16 +12,14 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: workflows
 License-File: LICENSE
 
 # cpg-utils
 
 This is a Python library containing convenience functions that are specific to the CPG.
 
 In order to install the library in a conda environment, run:
@@ -31,15 +29,15 @@
 ```
 
 To use the library, import functions like this:
 
 ```python
 from cpg_utils.cloud import email_from_id_token
 
-_email_string = email_from_id_token(id_token='TOKEN_STRING')
+_email_string = email_from_id_token(id_token_jwt='TOKEN_STRING')
 ```
 
 We use `bumpversion` for incrementing the library's semantic version. A new conda package gets published automatically in the `cpg` conda channel whenever a version bump commit is merged with the `main` branch.
 
 
 ## Contents
```

### Comparing `cpg-utils-4.9.4/cpg_utils.egg-info/SOURCES.txt` & `cpg-utils-5.0.0/cpg_utils.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 cpg_utils/__init__.py
 cpg_utils/cloud.py
 cpg_utils/cloudpath_hail_az.py
-cpg_utils/config-template.toml
 cpg_utils/config.py
+cpg_utils/constants.py
+cpg_utils/cromwell.py
+cpg_utils/cromwell_model.py
+cpg_utils/dataproc.py
 cpg_utils/git.py
 cpg_utils/hail_batch.py
+cpg_utils/membership.py
+cpg_utils/py.typed
+cpg_utils/slack.py
 cpg_utils.egg-info/PKG-INFO
 cpg_utils.egg-info/SOURCES.txt
 cpg_utils.egg-info/dependency_links.txt
 cpg_utils.egg-info/requires.txt
 cpg_utils.egg-info/top_level.txt
-cpg_utils/workflows/__init__.py
-cpg_utils/workflows/batch.py
-cpg_utils/workflows/filetypes.py
-cpg_utils/workflows/inputs.py
-cpg_utils/workflows/metamist.py
-cpg_utils/workflows/resources.py
-cpg_utils/workflows/slack.py
-cpg_utils/workflows/status.py
-cpg_utils/workflows/targets.py
-cpg_utils/workflows/utils.py
-cpg_utils/workflows/workflow.py
-test/test_batch.py
-test/test_cohort.py
-test/test_status.py
-test/test_workflow.py
+test/__init__.py
+test/test_config.py
+test/test_cromwell.py
+test/test_doctests.py
```

