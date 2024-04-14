# Comparing `tmp/aedev_git_repo_manager-0.3.72.tar.gz` & `tmp/aedev_git_repo_manager-0.3.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aedev_git_repo_manager-0.3.72.tar", last modified: Tue Mar 19 20:02:15 2024, max compression
+gzip compressed data, was "aedev_git_repo_manager-0.3.75.tar", last modified: Sun Apr 14 19:38:23 2024, max compression
```

## Comparing `aedev_git_repo_manager-0.3.72.tar` & `aedev_git_repo_manager-0.3.75.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:02:15.612947 aedev_git_repo_manager-0.3.72/
--rw-rw-rw-   0 root         (0) root         (0)    35002 2024-03-19 20:02:03.000000 aedev_git_repo_manager-0.3.72/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     6521 2024-03-19 20:02:15.612947 aedev_git_repo_manager-0.3.72/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3543 2024-03-19 20:02:03.000000 aedev_git_repo_manager-0.3.72/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:02:15.604947 aedev_git_repo_manager-0.3.72/aedev/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:02:15.606947 aedev_git_repo_manager-0.3.72/aedev/git_repo_manager/
--rw-rw-rw-   0 root         (0) root         (0)     1879 2024-03-19 20:02:03.000000 aedev_git_repo_manager-0.3.72/aedev/git_repo_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   186740 2024-03-19 20:02:03.000000 aedev_git_repo_manager-0.3.72/aedev/git_repo_manager/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:02:15.609947 aedev_git_repo_manager-0.3.72/aedev_git_repo_manager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6521 2024-03-19 20:02:15.000000 aedev_git_repo_manager-0.3.72/aedev_git_repo_manager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      449 2024-03-19 20:02:15.000000 aedev_git_repo_manager-0.3.72/aedev_git_repo_manager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-19 20:02:15.000000 aedev_git_repo_manager-0.3.72/aedev_git_repo_manager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      117 2024-03-19 20:02:15.000000 aedev_git_repo_manager-0.3.72/aedev_git_repo_manager.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      530 2024-03-19 20:02:15.000000 aedev_git_repo_manager-0.3.72/aedev_git_repo_manager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-03-19 20:02:15.000000 aedev_git_repo_manager-0.3.72/aedev_git_repo_manager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-19 20:02:15.000000 aedev_git_repo_manager-0.3.72/aedev_git_repo_manager.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-19 20:02:15.612947 aedev_git_repo_manager-0.3.72/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      704 2024-03-19 20:02:03.000000 aedev_git_repo_manager-0.3.72/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:02:15.608947 aedev_git_repo_manager-0.3.72/tests/
--rw-rw-rw-   0 root         (0) root         (0)   157929 2024-03-19 20:02:03.000000 aedev_git_repo_manager-0.3.72/tests/test_git_repo_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 19:38:23.711288 aedev_git_repo_manager-0.3.75/
+-rw-rw-rw-   0 root         (0) root         (0)    35002 2024-04-14 19:38:12.000000 aedev_git_repo_manager-0.3.75/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     6549 2024-04-14 19:38:23.711288 aedev_git_repo_manager-0.3.75/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3543 2024-04-14 19:38:12.000000 aedev_git_repo_manager-0.3.75/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 19:38:23.703964 aedev_git_repo_manager-0.3.75/aedev/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 19:38:23.705795 aedev_git_repo_manager-0.3.75/aedev/git_repo_manager/
+-rw-rw-rw-   0 root         (0) root         (0)     1879 2024-04-14 19:38:12.000000 aedev_git_repo_manager-0.3.75/aedev/git_repo_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   186882 2024-04-14 19:38:12.000000 aedev_git_repo_manager-0.3.75/aedev/git_repo_manager/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 19:38:23.707626 aedev_git_repo_manager-0.3.75/aedev_git_repo_manager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6549 2024-04-14 19:38:23.000000 aedev_git_repo_manager-0.3.75/aedev_git_repo_manager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      449 2024-04-14 19:38:23.000000 aedev_git_repo_manager-0.3.75/aedev_git_repo_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-14 19:38:23.000000 aedev_git_repo_manager-0.3.75/aedev_git_repo_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      117 2024-04-14 19:38:23.000000 aedev_git_repo_manager-0.3.75/aedev_git_repo_manager.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      543 2024-04-14 19:38:23.000000 aedev_git_repo_manager-0.3.75/aedev_git_repo_manager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-14 19:38:23.000000 aedev_git_repo_manager-0.3.75/aedev_git_repo_manager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-14 19:38:23.000000 aedev_git_repo_manager-0.3.75/aedev_git_repo_manager.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-14 19:38:23.711288 aedev_git_repo_manager-0.3.75/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      704 2024-04-14 19:38:12.000000 aedev_git_repo_manager-0.3.75/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 19:38:23.707626 aedev_git_repo_manager-0.3.75/tests/
+-rw-rw-rw-   0 root         (0) root         (0)   157998 2024-04-14 19:38:12.000000 aedev_git_repo_manager-0.3.75/tests/test_git_repo_manager.py
```

### Comparing `aedev_git_repo_manager-0.3.72/LICENSE.md` & `aedev_git_repo_manager-0.3.75/LICENSE.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.tpl_project V0.3.29 -->
+<!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.tpl_project V0.3.30 -->
 ### GNU GENERAL PUBLIC LICENSE
 
 Version 3, 29 June 2007
 
 Copyright (C) 2007 Free Software Foundation, Inc.
 <https://fsf.org/>
```

### Comparing `aedev_git_repo_manager-0.3.72/PKG-INFO` & `aedev_git_repo_manager-0.3.75/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aedev_git_repo_manager
-Version: 0.3.72
+Version: 0.3.75
 Summary: aedev namespace package portion git_repo_manager: create and maintain local/remote git repositories of Python projects
 Home-page: https://gitlab.com/aedev-group/aedev_git_repo_manager
 Author: AndiEcker
 Author-email: aecker2@gmail.com
 License: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Documentation, https://aedev.readthedocs.io/en/latest/_autosummary/aedev.git_repo_manager.html
 Project-URL: Repository, https://gitlab.com/aedev-group/aedev_git_repo_manager
@@ -39,14 +39,15 @@
 Requires-Dist: ae_core
 Requires-Dist: ae_console
 Requires-Dist: ae_dynamicod
 Requires-Dist: ae_literal
 Requires-Dist: aedev_pythonanywhere
 Requires-Dist: aedev_setup_project
 Requires-Dist: Pillow
+Requires-Dist: types-Pillow
 Provides-Extra: dev
 Requires-Dist: aedev_tpl_project; extra == "dev"
 Requires-Dist: aedev_aedev; extra == "dev"
 Requires-Dist: anybadge; extra == "dev"
 Requires-Dist: coverage-badge; extra == "dev"
 Requires-Dist: aedev_git_repo_manager; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
@@ -69,27 +70,27 @@
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: typing; extra == "tests"
 Requires-Dist: types-setuptools; extra == "tests"
 Requires-Dist: wheel; extra == "tests"
 Requires-Dist: twine; extra == "tests"
 
-<!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.aedev V0.3.20 -->
+<!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.aedev V0.3.22 -->
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.tpl_namespace_root V0.3.14 -->
-# git_repo_manager 0.3.72
+# git_repo_manager 0.3.75
 
 [![GitLab develop](https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/develop?logo=python)](
     https://gitlab.com/aedev-group/aedev_git_repo_manager)
 [![LatestPyPIrelease](
-    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.71?logo=python)](
-    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.71)
+    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.72?logo=python)](
+    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.72)
 [![PyPIVersions](https://img.shields.io/pypi/v/aedev_git_repo_manager)](
     https://pypi.org/project/aedev-git-repo-manager/#history)
 
->aedev_git_repo_manager package 0.3.72.
+>aedev_git_repo_manager package 0.3.75.
 
 [![Coverage](https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage/index.html)
 [![MyPyPrecision](https://aedev-group.gitlab.io/aedev_git_repo_manager/mypy.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/lineprecision.txt)
 [![PyLintScore](https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.log)
```

### Comparing `aedev_git_repo_manager-0.3.72/README.md` & `aedev_git_repo_manager-0.3.75/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-<!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.aedev V0.3.20 -->
+<!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.aedev V0.3.22 -->
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.tpl_namespace_root V0.3.14 -->
-# git_repo_manager 0.3.72
+# git_repo_manager 0.3.75
 
 [![GitLab develop](https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/develop?logo=python)](
     https://gitlab.com/aedev-group/aedev_git_repo_manager)
 [![LatestPyPIrelease](
-    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.71?logo=python)](
-    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.71)
+    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.72?logo=python)](
+    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.72)
 [![PyPIVersions](https://img.shields.io/pypi/v/aedev_git_repo_manager)](
     https://pypi.org/project/aedev-git-repo-manager/#history)
 
->aedev_git_repo_manager package 0.3.72.
+>aedev_git_repo_manager package 0.3.75.
 
 [![Coverage](https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage/index.html)
 [![MyPyPrecision](https://aedev-group.gitlab.io/aedev_git_repo_manager/mypy.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/lineprecision.txt)
 [![PyLintScore](https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.log)
```

### Comparing `aedev_git_repo_manager-0.3.72/aedev/git_repo_manager/__init__.py` & `aedev_git_repo_manager-0.3.75/aedev/git_repo_manager/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,21 +22,21 @@
 file patching helper functions
 ------------------------------
 
 this portion is also providing some helper functions to patch code and documentation files.
 
 the functions :func:`~aedev.git_repo_manager.__main__.bump_file_version`,
 :func:`~aedev.git_repo_manager.__main__.increment_version`,
-:func:`~aedev.git_repo_manager.__main__.next_project_version` and
+:func:`~aedev.git_repo_manager.__main__._git_project_version` and
 :func:`~aedev.git_repo_manager.__main__.replace_file_version`
 are incrementing any part of a version number of a module, portion, app or package.
 
 templates are patched with the help of the functions :func:`~aedev.git_repo_manager.__main__.deploy_template`,
 :func:`~aedev.git_repo_manager.__main__.patch_string` and :func:`~aedev.git_repo_manager.__main__.refresh_templates`.
 
 in conjunction with the template projects of the `aedev` namespace (like e.g. :mod:`aedev.tpl_project`) any common
 portions file (even the ``setup.py`` file) can be created/maintained as a template in a single place, and then
 requested and updated individually for each portion project.
 """
 
 
-__version__ = '0.3.72'
+__version__ = '0.3.75'
```

### Comparing `aedev_git_repo_manager-0.3.72/aedev/git_repo_manager/__main__.py` & `aedev_git_repo_manager-0.3.75/aedev/git_repo_manager/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 from difflib import context_diff, diff_bytes, ndiff, unified_diff
 from functools import wraps
 from traceback import format_exc
 from typing import (
     Any, Callable, Collection, Dict, Iterable, Iterator, List, Optional, OrderedDict as OrderedDictType,
     Sequence, Set, Tuple, Union, cast)
 
-from dotenv import load_dotenv
+from dotenv import find_dotenv, load_dotenv
 
 from github import Github
 from gitlab import Gitlab, GitlabCreateError, GitlabError, GitlabHttpError
 from gitlab.const import MAINTAINER_ACCESS
 from gitlab.v4.objects import Group, Project
 
 from packaging.version import Version
-from PIL import Image                                                                   # type: ignore
+from PIL import Image
 
 import ae.base                                                                          # type: ignore # for patching
 from ae.base import (
     PY_EXT, PY_INIT, TEMPLATES_FOLDER, UNSET, UnsetType,
     camel_to_snake, duplicates, in_wd, module_attr, norm_name, norm_path,
     project_main_file, read_file, stack_var, write_file)
 from ae.files import FileObject                                                         # type: ignore
@@ -561,34 +561,14 @@
         main_name = 'main' + PY_EXT
     else:
         main_name = main_stem + PY_EXT
 
     return os.path.join(main_path, main_name)
 
 
-def next_project_version(pdv: PdvType, increment_part: int = 3) -> str:
-    """ determine latest or the next free package repository version or the project specified via the pdv argument.
-
-    :param pdv:                 project dev vars to identify the package.
-    :param increment_part:      part of the version number to be incremented (1=mayor, 2=minor/namespace, 3=patch).
-                                pass zero/0 to return the latest published package version.
-    :return:                    latest published repository package version as string
-                                or "0.0.1" if project never published a version tag to remotes/origin
-                                or empty string on error.
-    """
-    if _git_fetch(pdv):
-        return ""
-
-    version_tags = _git_tag_list(pdv)
-    if not version_tags[-1]:
-        return "0.0.1"
-
-    return increment_version(version_tags[-1][1:], increment_part=increment_part)
-
-
 def on_ci_host() -> bool:
     """ check and return True if this tool is running on the GitLab/GitHub CI host/server.
 
     :return:                    True if running on CI host, else False
     """
     return 'CI' in os.environ or 'CI_PROJECT_ID' in os.environ
 
@@ -683,16 +663,16 @@
 
     :param project_path:        optional rel/abs path of the package/app/project root directory of a new and existing
                                 project (defaults to the current working directory if empty or not passed).
     :return:                    dict/mapping with the determined project development variable values.
     """
     abs_prj_path = os.path.abspath(project_path)
     if os.path.exists(abs_prj_path):
-        with in_wd(abs_prj_path):
-            load_dotenv()   # load .env file from project path folder (or above from projects folder)
+        with in_wd(abs_prj_path):   # load .env file from project path folder (or above from projects folder)
+            load_dotenv(dotenv_path=find_dotenv(usecwd=True))
 
     pdv = cast(PdvType, project_env_vars(project_path=project_path))
     project_path = pdv_str(pdv, 'project_path')     # re-read as absolute path
     project_type = pdv_str(pdv, 'project_type')
     sep = os.linesep
     ins = sep + " " * 4
 
@@ -1457,15 +1437,15 @@
     """ determine host domain, group, user and credential values.
 
     :param host_domain:         domain name of the host. pass empty string to skip search for host-specific variable.
     :param option_name:         host option name and config variable name part ('domain', 'group', 'user', 'token'),
                                 resulting in e.g. user, repo_user, repo_user_at_xxx, web_user, web_user_at...
     :param host_user:           username at the host. if not passed or :paramref:`~_get_host_config_val.host_domain` is
                                 empty then skip the search for a user-specific variable value.
-    :param name_prefix          config variable name prefix. pass 'web' to get web server host config values.
+    :param name_prefix:         config variable name prefix. pass 'web' to get web server host config values.
     :return:                    config variable value or None if not found.
     """
     val = cae.get_option(option_name)
     if val is None:
         var_name = f'{name_prefix}_{option_name}'
         if host_domain:
             if host_user:
@@ -1476,15 +1456,15 @@
             val = cae.get_variable(var_name)
     return val
 
 
 def _get_host_domain(pdv: PdvType, name_prefix: str = 'repo') -> str:
     """ determine domain name of repository|web host from --domain option, repo_domain or web_domain config variable.
 
-    :param name_prefix          config variable name prefix. pass 'web' to get web server host config values.
+    :param name_prefix:         config variable name prefix. pass 'web' to get web server host config values.
     :return:                    domain name of repository|web host.
     """
     host_domain = _get_host_config_val("", 'domain', name_prefix=name_prefix)
     if host_domain is None:
         host_domain = pdv_str(pdv, f'{name_prefix}_domain') or pdv_str(pdv, 'REPO_CODE_DOMAIN')     # repo_|web_domain
 
     if not _get_host_class_name(host_domain):
@@ -1505,29 +1485,31 @@
     return user_group
 
 
 def _get_host_user_name(pdv: PdvType, host_domain: str, name_prefix: str = 'repo') -> str:
     """ determine username from --user option, repo_user or web_user config variable.
 
     :param host_domain:         domain to get user token for.
-    :param name_prefix          config variable name prefix. pass 'web' to get web server host config values.
+    :param name_prefix:         config variable name prefix. pass 'web' to get web server host config values.
     :return:                    username or if not found the user group name.
     """
     user_name = _get_host_config_val(host_domain, 'user', name_prefix=name_prefix)
     if user_name is None:
-        user_name = _get_host_group(pdv, host_domain)
+        user_name = pdv_str(pdv, f'{name_prefix}_user')     # if specified in pev.defaults config file
+        if not user_name:
+            user_name = _get_host_group(pdv, host_domain)
     return user_name
 
 
 def _get_host_user_token(host_domain: str, host_user: str = "", name_prefix: str = 'repo') -> str:
     """ determine token or password of user from --token option, repo_token or web_token config variable.
 
     :param host_domain:         domain to get user token for.
     :param host_user:           host user to get token for.
-    :param name_prefix          config variable name prefix. pass 'web' to get web server host config values.
+    :param name_prefix:         config variable name prefix. pass 'web' to get web server host config values.
     :return:                    token string for domain and user on repository|web host.
     """
     return _get_host_config_val(host_domain, 'token', host_user=host_user, name_prefix=name_prefix) or ""
 
 
 def _get_namespace(pdv: PdvType, project_type: str) -> str:
     namespace_name = cae.get_option('namespace') or pdv_str(pdv, 'namespace_name')
@@ -1789,14 +1771,34 @@
     output: List[str] = []
     with _in_prj_dir_venv(pdv_str(pdv, 'project_path')):
         _cl(75, "git merge", extra_args=args, lines_output=output)
 
     return "=======" not in "".join(output)
 
 
+def _git_project_version(pdv: PdvType, increment_part: int = 3) -> str:
+    """ determine latest or the next free package git repository version or the project specified via the pdv argument.
+
+    :param pdv:                 project dev vars to identify the package.
+    :param increment_part:      part of the version number to be incremented (1=mayor, 2=minor/namespace, 3=patch).
+                                pass zero/0 to return the latest published package version.
+    :return:                    latest published repository package version as string
+                                or "0.0.1" if project never published a version tag to remotes/origin
+                                or empty string on error.
+    """
+    if _git_fetch(pdv):
+        return ""
+
+    version_tags = _git_tag_list(pdv)
+    if not version_tags[-1]:
+        return "0.0.1"
+
+    return increment_version(version_tags[-1][1:], increment_part=increment_part)
+
+
 def _git_push(pdv: PdvType, *branches_and_tags: str, exit_on_error: bool = True, extra_args: Iterable[str] = ()) -> int:
     """ push portion in the current working directory to the specified branch. """
     protocol = pdv_str(pdv, 'REPO_HOST_PROTOCOL')
     domain = _get_host_domain(pdv)
     project_name = _get_prj_name(pdv)
     usr = _get_host_user_name(pdv, domain)
     group_or_user_name = usr if 'upstream' in _git_remotes(pdv) else _get_host_group(pdv, domain)
@@ -2644,15 +2646,15 @@
 
             push_refs.append(MAIN_BRANCH)
 
         branch_name = branch_name or _get_branch(ini_pdv)
         if branch_name and branch_name not in push_refs:
             push_refs.append(branch_name)
 
-        pkg_version = next_project_version(ini_pdv, increment_part=cae.get_option('versionIncrementPart'))
+        pkg_version = _git_project_version(ini_pdv, increment_part=cae.get_option('versionIncrementPart'))
         file_version = pdv_str(ini_pdv, 'project_version')
         _chk_if(77, pkg_version == file_version, f"version mismatch: local={file_version} remote={pkg_version}")
         if Version(pkg_version) > Version(file_version):     # and cae.get_option('force')
             replace_file_version(pdv_str(ini_pdv, 'version_file'), new_version=pkg_version)
             _write_commit_message(ini_pdv, pkg_version=pkg_version,
                                   title=f"late commit of forced push version correction {file_version}->{pkg_version}")
             _git_add(ini_pdv)
@@ -2674,52 +2676,52 @@
         for chi_pdv in children_pdv:
             cae.po(f" ---  {pdv_str(chi_pdv, 'project_name')}  ---  {pdv_str(chi_pdv, 'project_desc')}")
             self.release_project(chi_pdv, 'LATEST')
             if chi_pdv != children_pdv[-1]:
                 _wait()
         cae.po(f"===== released {_children_desc(ini_pdv, children_pdv)}")
 
-    @_action(arg_names=(("push-tag", ), ('LATEST', )), shortcut='release')
-    def release_project(self, ini_pdv: PdvType, push_tag: str):
+    @_action(arg_names=(("version-tag", ), ('LATEST', )), shortcut='release')
+    def release_project(self, ini_pdv: PdvType, version_tag: str):
         """ update local MAIN_BRANCH from origin and if pip_name is set then also release the latest/specified version.
 
         :param ini_pdv:         project dev vars.
-        :param push_tag:        push version tag in the format ``v<version-number>`` to release or ``LATEST`` to use
-                                the version tag of the latest repository version.
+        :param version_tag:     push version tag in the format ``v<version-number>`` to release or ``LATEST`` to use
+                                the version tag of the latest git repository version.
         """
         errors = _git_fetch(ini_pdv)
         _chk_if(84, not bool(errors), f"git fetch errors:{_pp(errors)}" + _hint(
             self.release_project, " later to retry if server is currently unavailable, or check remote configuration"))
 
         # switch back to local MAIN_BRANCH and then merge-in the release-branch&-tag from remotes/origin/MAIN_BRANCH
         _git_checkout(ini_pdv, branch=MAIN_BRANCH)
         _git_merge(ini_pdv, f"origin/{MAIN_BRANCH}")
 
-        if push_tag == 'LATEST':
-            pkg_version = next_project_version(ini_pdv, increment_part=0)
-            push_tag = f"v{pkg_version}"
+        if version_tag == 'LATEST':
+            pkg_version = _git_project_version(ini_pdv, increment_part=0)
+            version_tag = f"v{pkg_version}"
         else:
-            _chk_if(85, push_tag[0] == "v" and push_tag.count(".") == 2, f"push-tag/version format error {push_tag}")
-            pkg_version = push_tag[1:]
-        _chk_if(85, _git_tag_in_branch(ini_pdv, push_tag),
-                f"push version tag {push_tag} has first to be merged into origin/{MAIN_BRANCH}" + _hint(
+            _chk_if(85, version_tag[0] == "v" and version_tag.count(".") == 2, f"version '{version_tag}' format error")
+            pkg_version = version_tag[1:]
+        _chk_if(85, _git_tag_in_branch(ini_pdv, version_tag),
+                f"push version tag {version_tag} has first to be merged into origin/{MAIN_BRANCH}" + _hint(
                     self.request_merge, " to request to merge your branch."))
 
         msg = f"updated local {MAIN_BRANCH} branch"
         if pdv_str(ini_pdv, 'pip_name'):    # create release*ver branch only for projects available in PyPi via pip
             release_branch = f"release{pkg_version}"
             _chk_if(85, not _git_tag_in_branch(ini_pdv, release_branch),
                     f"release branch {release_branch} already exists in origin/{MAIN_BRANCH}")
 
             prj = self.project_from_name(95, "project {name} not found", pdv_str(ini_pdv, 'project_name'))
-            cae.dpo(f"   -- creating branch '{release_branch}' for tag '{push_tag}' at remotes/origin")
+            cae.dpo(f"   -- creating branch '{release_branch}' for tag '{version_tag}' at remotes/origin")
             try:
-                prj.branches.create({'branch': release_branch, 'ref': push_tag})
+                prj.branches.create({'branch': release_branch, 'ref': version_tag})
             except (GitlabHttpError, GitlabCreateError, GitlabError, Exception):
-                _exit_error(86, f"error '{format_exc()}' creating branch '{release_branch}' for tag '{push_tag}'")
+                _exit_error(86, f"error '{format_exc()}' creating branch '{release_branch}' for tag '{version_tag}'")
             msg += f" and released {pkg_version}"
 
         cae.po(f" ==== {msg} of {pdv_str(ini_pdv, 'project_desc')}")
 
     @_action(PARENT_PRJ, ROOT_PRJ, shortcut='request')
     def request_children_merge(self, ini_pdv: PdvType, *children_pdv: PdvType):
         """ request the merge of the specified children of a parent/namespace on remote/upstream. """
@@ -2845,35 +2847,34 @@
         :param optional_flags:  optional command line arguments, documented in detail in the declaration of
                                 the action method parameter :paramref:`check_deploy.optional_flags`.
         :return:                tuple of string and 2 sets. both sets containing file paths, relative to the
                                 local/temporary project root folder, which gets returned as the first item of the tuple.
                                 the first set contains the deployable files, and the 2nd one the files that got removed
                                 from the repository or that could be cleaned-up on the server.
         """
+        func = self.check_deploy if action == 'check' else self.deploy_project
         lean_msg = ' lean' if optional_flags['LEAN'] else ''
         verbose = _debug_or_verbose()
-
         deployed_ver = self.connection.deployed_version()
-        _chk_if(85, not deployed_ver or version_tag[1:] in (deployed_ver, increment_version(deployed_ver)),
-                f"too big version increment between old|deployed ({deployed_ver}) and new version ({version_tag[1:]})"
-                + _hint(self.check_deploy if action == 'check' else self.deploy_project,
-                        " with the current/next version or with the --force/-f option to skip this version check"))
 
         if version_tag == 'WORKTREE':
             include_untracked = True
             branch_or_tag = f"v{deployed_ver}" if deployed_ver else MAIN_BRANCH     # from this to HEAD
             prj_root_path = pdv_str(ini_pdv, 'project_path')
-            version_tag = f"v{next_project_version(ini_pdv, increment_part=0)}w"    # w suffix only visible in logs
+            version_tag = f"v{_git_project_version(ini_pdv, increment_part=0)}w"    # w suffix only visible in logs
         else:
             include_untracked = False
             if version_tag == 'LATEST':
-                version_tag = f"v{next_project_version(ini_pdv, increment_part=0)}"
+                version_tag = f"v{_git_project_version(ini_pdv, increment_part=0)}"
             else:
                 _chk_if(85, version_tag[0] == "v" and version_tag.count(".") == 2,
                         f"expected 'LATEST', 'WORKTREE' or a project version tag (e.g. 'v0.1.2'), got '{version_tag}'")
+                _chk_if(85, not deployed_ver or version_tag[1:] in (deployed_ver, increment_version(deployed_ver)),
+                        f"too big increment between old|deployed ({deployed_ver}) and new version ({version_tag[1:]})"
+                        + _hint(func, " with the current/next version or the --force option to skip the version check"))
             prj_root_path = _git_clone(pdv_str(ini_pdv, 'repo_root'), pdv_str(ini_pdv, 'project_name'),
                                        branch_or_tag=version_tag, extra_args=("--filter=blob:none", ))
             _chk_if(85, bool(prj_root_path), "git clone tmp cleanup error, to check run again with the -D 1 option")
             branch_or_tag = f"v{deployed_ver}...{version_tag}"
 
         path_masks = optional_flags['MASKS'] + ['manage.py'] + root_packages_masks(ini_pdv)
         cae.vpo(f"  --- {len(path_masks)} deploy file path masks found: {_pp(sorted(path_masks))}")
@@ -2883,30 +2884,25 @@
         def _track_skipped(file_path: str) -> bool:
             if skip_func(file_path):
                 if skip_py_cache_files(file_path):
                     return True
                 skipped.add(file_path)
             return False
         deployable = find_project_files(prj_root_path, path_masks, skip_file_path=_track_skipped)
-        cae.vpo(f"  --- {len(deployable)} deployable project package files found: {_pp(sorted(deployable))}")
-        cae.vpo(f"  --- {len(skipped)}{lean_msg} files got skipped: {_pp(sorted(skipped))}")
+        cae.vpo(f"  --- {len(deployable)} deployable project files found: {_pp(sorted(deployable))}")
+        cae.vpo(f"  --- {len(skipped)}{lean_msg} project files got skipped: {_pp(sorted(skipped))}")
 
-        which_files = "deployable"
-
-        to_delete = set()
         to_deploy = deployable - skipped
-
+        to_delete = set()
+        which_files = "deployable"
         if deployed_ver and not optional_flags['ALL']:
             which_files = "new|changed|deleted"
             changed = find_git_branch_files(prj_root_path, branch_or_tag=branch_or_tag, untracked=include_untracked,
                                             skip_file_path=skip_func)
-            if verbose:
-                cae.po(f"  --- {len(changed)} {which_files} files found in specified {version_tag} repository")
-            _chk_if(85, bool(changed), f"no {which_files} files found in repository v{deployed_ver}" + _hint(
-                self.deploy_project, f" specifying ALL as extra argument to {action} all deployable project files"))
+            cae.vpo(f"  --- {len(changed)} changed project files found in {branch_or_tag}: {_pp(sorted(changed))}")
             to_deploy &= changed
             to_delete = set(paths_match(changed, path_masks)) - deployable
 
         for pkg_file_path in sorted(to_deploy):
             src_path = os.path.join(prj_root_path, pkg_file_path)
             src_content = read_file(src_path, extra_mode='b') if os.path.isfile(src_path) else None
             dst_content = self.connection.deployed_file_content(pkg_file_path)
@@ -2937,14 +2933,17 @@
             to_cleanup -= (deployable - skipped)
             if not to_cleanup:
                 cae.po("  --- no extra files to clean up found on server")
             elif verbose:
                 cae.po(f"  --- {len(to_cleanup)} deletable{lean_msg} files: {_pp(sorted(to_cleanup))}" +
                        (_hint(self.deploy_project, " to remove them from the server") if action == 'check' else ""))
 
+        _chk_if(85, bool(to_deploy | to_delete | to_cleanup), f"no {which_files}|cleanup files found in {version_tag}"
+                + _hint(func, f" specifying ALL as extra argument to {action} all deployable project files"))
+
         verbose = action == 'check' or verbose
         cae.po(f" ===  {len(to_deploy)} {which_files} files found to migrate server to {version_tag} version"
                f"{'; from v' + deployed_ver if deployed_ver else ''}{':' + _pp(sorted(to_deploy)) if verbose else ''}")
         cae.po(f" ===  {len(to_delete) + len(to_cleanup)} deletable (repo={len(to_delete)} cleanup={len(to_cleanup)})"
                f" files found{':' + _pp(sorted(to_delete | to_cleanup)) if verbose else ''}")
 
         return prj_root_path, to_deploy, to_delete | to_cleanup
@@ -2952,32 +2951,36 @@
     # ----------- remote action methods ----------------------------------------------------------------------------
 
     @_action(APP_PRJ, DJANGO_PRJ, arg_names=(("version-tag", ), ('LATEST', ), ('WORKTREE', ), ), flags=deploy_flags)
     def check_deploy(self, ini_pdv: PdvType, version_tag: str, **optional_flags):
         """ check all project package files at the app/web server against the specified package version.
 
         :param ini_pdv:         project dev vars.
+
         :param version_tag:     version tag in the format ``v<version-number>`` to check or ``LATEST`` to check against
                                 the latest repository version or ``WORKTREE`` to check directly against
                                 the local work tree (with the locally added, unstaged and changed files).
+
         :param optional_flags:  additional/optionally supported command line arguments:
-                                * `ALL` is including all deployable package files, instead of only the new, changed or
-                                   deleted files in the specified repository.
-                                * 'CLEANUP' is checking for deletable files on the web server/host, e.g. after
-                                   they got removed from the specified repository or work tree.
-                                * `LEAN` is reducing the deployable files sets to the minimum (using e.g. the method
-                                  :func:`skip_files_lean_web`), like e.g. the gettext '.po' files,
-                                  the 'media_ini' root folder, and the 'static' sub-folder with the initial static
+
+                                * ``ALL`` is including all deployable package files, instead of only the new, changed or
+                                  deleted files in the specified repository.
+                                * ``CLEANUP`` is checking for deletable files on the web server/host, e.g. after
+                                  they got removed from the specified repository or work tree.
+                                * ``LEAN`` is reducing the deployable files sets to the minimum (using e.g. the function
+                                  :func:`skip_files_lean_web`), like e.g. the gettext ``.po`` files,
+                                  the ``media_ini`` root folder, and the ``static`` sub-folder with the initial static
                                   files of the web project.
-                                * 'MASKS' specifies a list of file paths masks/pattern to be included in the
+                                * ``MASKS`` specifies a list of file paths masks/pattern to be included in the
                                   repository files to check/deploy. to include e.g. the files of the static root folder
                                   specify this argument as ``MASKS="['static/**/*']"``. single files can be included
                                   too, by adding their possible file names to the list - only the found ones will be
                                   included. for example to include the django database you could add some possible DB
                                   file names to the list like in ``"MASKS=['static/**/*', 'db.sqlite', 'project.db']"``
+
         """
         root, to_deploy, to_delete = self.deploy_differences(ini_pdv, 'check', version_tag, **optional_flags)
 
         cae.po(f" ==== {len(to_deploy)} files outdated and {len(to_delete)} could be deleted on server"
                f" {pdv_str(ini_pdv, 'web_user')}@{pdv_str(ini_pdv, 'web_domain')} / {pdv_str(ini_pdv, 'project_desc')}")
 
     @_action(APP_PRJ, DJANGO_PRJ, arg_names=(("version-tag", ), ('LATEST', ), ('WORKTREE', ), ), flags=deploy_flags,
@@ -3080,15 +3083,15 @@
     inc_part = cae.get_option('versionIncrementPart')
     if inc_part not in range(1, 4):
         cae.dpo(f"    = skipped bump of version (because versionIncrementPart=={inc_part})")
         return
 
     old_version = pdv_str(ini_pdv, 'project_version')
     new_version = increment_version(old_version, increment_part=inc_part)
-    nxt_version = next_project_version(ini_pdv, increment_part=inc_part)
+    nxt_version = _git_project_version(ini_pdv, increment_part=inc_part)
     _chk_if(59, new_version == nxt_version,
             f"next/incremented package versions out of sync: new-local={new_version} next-remote={nxt_version}")
 
     bump_file_version(pdv_str(ini_pdv, 'version_file'), increment_part=inc_part)
 
     ini_pdv.update(project_dev_vars(pdv_str(ini_pdv, 'project_path')))
```

### Comparing `aedev_git_repo_manager-0.3.72/aedev_git_repo_manager.egg-info/PKG-INFO` & `aedev_git_repo_manager-0.3.75/aedev_git_repo_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aedev_git_repo_manager
-Version: 0.3.72
+Version: 0.3.75
 Summary: aedev namespace package portion git_repo_manager: create and maintain local/remote git repositories of Python projects
 Home-page: https://gitlab.com/aedev-group/aedev_git_repo_manager
 Author: AndiEcker
 Author-email: aecker2@gmail.com
 License: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Documentation, https://aedev.readthedocs.io/en/latest/_autosummary/aedev.git_repo_manager.html
 Project-URL: Repository, https://gitlab.com/aedev-group/aedev_git_repo_manager
@@ -39,14 +39,15 @@
 Requires-Dist: ae_core
 Requires-Dist: ae_console
 Requires-Dist: ae_dynamicod
 Requires-Dist: ae_literal
 Requires-Dist: aedev_pythonanywhere
 Requires-Dist: aedev_setup_project
 Requires-Dist: Pillow
+Requires-Dist: types-Pillow
 Provides-Extra: dev
 Requires-Dist: aedev_tpl_project; extra == "dev"
 Requires-Dist: aedev_aedev; extra == "dev"
 Requires-Dist: anybadge; extra == "dev"
 Requires-Dist: coverage-badge; extra == "dev"
 Requires-Dist: aedev_git_repo_manager; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
@@ -69,27 +70,27 @@
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: typing; extra == "tests"
 Requires-Dist: types-setuptools; extra == "tests"
 Requires-Dist: wheel; extra == "tests"
 Requires-Dist: twine; extra == "tests"
 
-<!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.aedev V0.3.20 -->
+<!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.aedev V0.3.22 -->
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.tpl_namespace_root V0.3.14 -->
-# git_repo_manager 0.3.72
+# git_repo_manager 0.3.75
 
 [![GitLab develop](https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/develop?logo=python)](
     https://gitlab.com/aedev-group/aedev_git_repo_manager)
 [![LatestPyPIrelease](
-    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.71?logo=python)](
-    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.71)
+    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.72?logo=python)](
+    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.72)
 [![PyPIVersions](https://img.shields.io/pypi/v/aedev_git_repo_manager)](
     https://pypi.org/project/aedev-git-repo-manager/#history)
 
->aedev_git_repo_manager package 0.3.72.
+>aedev_git_repo_manager package 0.3.75.
 
 [![Coverage](https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage/index.html)
 [![MyPyPrecision](https://aedev-group.gitlab.io/aedev_git_repo_manager/mypy.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/lineprecision.txt)
 [![PyLintScore](https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.log)
```

### Comparing `aedev_git_repo_manager-0.3.72/aedev_git_repo_manager.egg-info/requires.txt` & `aedev_git_repo_manager-0.3.75/aedev_git_repo_manager.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 ae_core
 ae_console
 ae_dynamicod
 ae_literal
 aedev_pythonanywhere
 aedev_setup_project
 Pillow
+types-Pillow
 
 [dev]
 aedev_tpl_project
 aedev_aedev
 anybadge
 coverage-badge
 aedev_git_repo_manager
```

### Comparing `aedev_git_repo_manager-0.3.72/setup.py` & `aedev_git_repo_manager-0.3.75/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.tpl_project V0.3.29
+# THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.tpl_project V0.3.30
 """ setup this project with setuptools and aedev.setup_project. """
 import pprint
 import sys
 
 import setuptools
 
 from aedev.setup_project import project_env_vars    # type: ignore
```

### Comparing `aedev_git_repo_manager-0.3.72/tests/test_git_repo_manager.py` & `aedev_git_repo_manager-0.3.75/tests/test_git_repo_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,23 +27,23 @@
     REGISTERED_TPL_PROJECTS, REGISTERED_HOSTS_CLASS_NAMES, SKIP_PRJ_TYPE_FILE_NAME_PREFIX,
     TEMPLATE_INCLUDE_FILE_PLACEHOLDER_ID, TEMPLATE_PLACEHOLDER_ARGS_SUFFIX, TEMPLATE_PLACEHOLDER_ID_PREFIX,
     TEMPLATE_PLACEHOLDER_ID_SUFFIX,
     TPL_FILE_NAME_PREFIX, TPL_IMPORT_NAME_PREFIX, TPL_PACKAGES, TPL_STOP_CNV_PREFIX,
     GitlabCom, PdvType, cae,
     _act_callable, _action, _available_actions, _cl, _debug_or_verbose, _exit_error, _expected_args,
     _get_branch, _get_host_user_name, _get_host_user_token,
-    _git_add, _git_checkout, _git_clone, _git_commit, _git_current_branch, _git_diff, _git_init_if_needed, _git_status,
-    _git_uncommitted, _in_prj_dir_venv,
+    _git_add, _git_checkout, _git_clone, _git_commit, _git_current_branch, _git_diff, _git_init_if_needed,
+    _git_project_version, _git_status, _git_uncommitted, _in_prj_dir_venv,
     _init_act_args_check, _init_act_exec_args, _init_children_pdv_args, _init_children_presets,
     _patch_outsourced, _print_pdv, _renew_prj_dir, _renew_project,
     _template_projects, _register_template, _template_version_option,
     _wait,
     activate_venv, active_venv, bump_file_version, deploy_template, editable_project_path,
     find_extra_modules, find_project_files, find_git_branch_files, increment_version,
-    in_venv, main_file_path, next_project_version, project_version, patch_string, pdv_str, project_dev_vars,
+    in_venv, main_file_path, project_version, patch_string, pdv_str, project_dev_vars,
     pypi_versions, refresh_templates, replace_file_version, replace_with_file_content_or_default,
     root_packages_masks, skip_files_lean_web, skip_files_migrations, venv_bin_path,
     add_children_file, bump_version, check_children_integrity, check_integrity, clone_children, clone_project,
     commit_children, commit_project, delete_children_file, install_children_editable, install_editable,
     new_app, new_children, new_django, new_module, new_namespace_root, new_package, new_project, on_ci_host,
     prepare_children_commit, prepare_commit, refresh_children_outsourced, rename_children_file, run_children_command,
     show_actions, show_children_status, show_children_versions, show_status,
@@ -108,16 +108,17 @@
 @pytest.fixture
 def gitlab_remote(mocked_app_options):
     """ provide a connected Gitlab remote repository api. """
     repo_domain = "gitlab.com"
     mocked_app_options['group'] = "aedev-group"
     mocked_app_options['namespace'] = ""
     mocked_app_options['project'] = "aedev_git_repo_manager"
-    from dotenv import load_dotenv
-    load_dotenv()   # pytest resets os.environ in each test run, reverting values set by load_dotenv in __main__.py
+    from dotenv import find_dotenv, load_dotenv
+    # load_dotenv()   # pytest resets os.environ in each test run, reverting values set by load_dotenv in __main__.py
+    load_dotenv(dotenv_path=find_dotenv(usecwd=True))
     mocked_app_options['token'] = repo_token = cae.get_variable(f'repo_token_at_{norm_name(repo_domain)}')
 
     remote_project = GitlabCom()
     #remote_project.connect(project_dev_vars(), cae.get_variable('repo_token'))
     remote_project.connect({'REPO_HOST_PROTOCOL': "https://",
                             'repo_domain': repo_domain,
                             'repo_token': repo_token})
@@ -1627,23 +1628,14 @@
 
     def test_in_venv(self):
         cur_venv = active_venv()
         with in_venv(LOCAL_VENV):
             assert active_venv() == '' if 'CI_PROJECT_ID' in os.environ else LOCAL_VENV
         assert active_venv() == cur_venv
 
-    def test_next_project_version(self, empty_repo_path, mocked_app_options):
-        mocked_app_options['namespace'] = ""
-        assert next_project_version({'project_path': TESTS_FOLDER}) == ""
-        assert next_project_version({'project_path': empty_repo_path}) == "0.0.1"
-
-    def test_next_project_version_local(self, empty_repo_path, mocked_app_options):
-        mocked_app_options['namespace'] = ""
-        assert next_project_version(project_dev_vars()) > "0.0.1"
-
     @skip_gitlab_ci
     def test_on_ci_host_local(self):
         assert not on_ci_host()
 
     def test_on_ci_host_on_gitlab(self):
         assert on_ci_host() == ('CI_PROJECT_ID' in os.environ)
 
@@ -2611,14 +2603,23 @@
         with _in_prj_dir_venv(changed_repo_path):
             _cl(0, "git ls-files -m", lines_output=ls_uncommitted)
         st_uncommitted = [_[3:] for _ in _git_status(pev)]
 
         assert len(ls_uncommitted) >= 2 and 'added.cfg' not in ls_uncommitted
         assert all(lsi in st_uncommitted for lsi in ls_uncommitted)
 
+    def test__git_project_version(self, empty_repo_path, mocked_app_options):
+        mocked_app_options['namespace'] = ""
+        assert _git_project_version({'project_path': TESTS_FOLDER}) == ""
+        assert _git_project_version({'project_path': empty_repo_path}) == "0.0.1"
+
+    def test__git_project_version_local(self, empty_repo_path, mocked_app_options):
+        mocked_app_options['namespace'] = ""
+        assert _git_project_version(project_dev_vars()) > "0.0.1"
+
     def test_git_status_on_changed_repo(self, changed_repo_path, mocked_app_options):
         mocked_app_options['force'] = False
         mocked_app_options['verbose'] = False
         files = set(path_items(os.path.join(changed_repo_path, "**")))
         pev = {'project_path': changed_repo_path}
 
         output = _git_status(pev)
```

