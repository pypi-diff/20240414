# Comparing `tmp/argcomplete-3.2.2.tar.gz` & `tmp/argcomplete-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argcomplete-3.2.2.tar", last modified: Tue Jan 23 20:48:10 2024, max compression
+gzip compressed data, was "argcomplete-3.2.3.tar", last modified: Fri Mar  8 01:30:04 2024, max compression
```

## Comparing `argcomplete-3.2.2.tar` & `argcomplete-3.2.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-01-23 20:48:10.472690 argcomplete-3.2.2/
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-01-23 20:48:10.454050 argcomplete-3.2.2/.github/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       18 2023-10-23 21:31:17.000000 argcomplete-3.2.2/.github/FUNDING.yml
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-01-23 20:48:10.454430 argcomplete-3.2.2/.github/workflows/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1253 2023-12-29 01:33:45.000000 argcomplete-3.2.2/.github/workflows/ci.yml
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      474 2023-10-23 21:31:17.000000 argcomplete-3.2.2/.gitignore
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       35 2023-10-23 21:31:18.000000 argcomplete-3.2.2/Authors.rst
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    14367 2024-01-23 20:47:52.000000 argcomplete-3.2.2/Changes.rst
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    10174 2023-10-23 21:31:17.000000 argcomplete-3.2.2/LICENSE.rst
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       79 2023-10-23 21:31:16.000000 argcomplete-3.2.2/MANIFEST.in
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      766 2023-10-23 21:31:16.000000 argcomplete-3.2.2/Makefile
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      387 2023-10-23 21:31:16.000000 argcomplete-3.2.2/NOTICE
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    16580 2024-01-23 20:48:10.472192 argcomplete-3.2.2/PKG-INFO
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    14692 2023-11-01 15:21:48.000000 argcomplete-3.2.2/README.rst
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      705 2023-10-23 21:31:54.000000 argcomplete-3.2.2/SECURITY.md
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-01-23 20:48:10.459047 argcomplete-3.2.2/argcomplete/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      693 2023-10-23 21:31:16.000000 argcomplete-3.2.2/argcomplete/__init__.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2412 2023-11-19 21:17:53.000000 argcomplete-3.2.2/argcomplete/_check_console_script.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2615 2023-11-01 15:11:23.000000 argcomplete-3.2.2/argcomplete/_check_module.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-01-23 20:48:10.461634 argcomplete-3.2.2/argcomplete/bash_completion.d/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     9852 2024-01-23 20:39:07.000000 argcomplete-3.2.2/argcomplete/bash_completion.d/_python-argcomplete
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3980 2023-10-23 21:31:16.000000 argcomplete-3.2.2/argcomplete/completers.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      112 2023-10-23 21:31:16.000000 argcomplete-3.2.2/argcomplete/exceptions.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    27793 2024-01-23 20:47:39.000000 argcomplete-3.2.2/argcomplete/finders.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      866 2023-10-23 21:31:16.000000 argcomplete-3.2.2/argcomplete/io.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2131 2023-10-23 21:31:16.000000 argcomplete-3.2.2/argcomplete/lexers.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-01-23 20:48:10.463157 argcomplete-3.2.2/argcomplete/packages/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2023-10-23 21:31:16.000000 argcomplete-3.2.2/argcomplete/packages/__init__.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    15846 2024-01-23 20:47:39.000000 argcomplete-3.2.2/argcomplete/packages/_argparse.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    12766 2024-01-23 20:47:39.000000 argcomplete-3.2.2/argcomplete/packages/_shlex.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2023-10-23 21:31:16.000000 argcomplete-3.2.2/argcomplete/py.typed
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     7377 2023-12-03 01:57:10.000000 argcomplete-3.2.2/argcomplete/shell_integration.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-01-23 20:48:10.471365 argcomplete-3.2.2/argcomplete.egg-info/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    16580 2024-01-23 20:48:10.000000 argcomplete-3.2.2/argcomplete.egg-info/PKG-INFO
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1291 2024-01-23 20:48:10.000000 argcomplete-3.2.2/argcomplete.egg-info/SOURCES.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2024-01-23 20:48:10.000000 argcomplete-3.2.2/argcomplete.egg-info/dependency_links.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2024-01-23 20:47:58.000000 argcomplete-3.2.2/argcomplete.egg-info/not-zip-safe
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       41 2024-01-23 20:48:10.000000 argcomplete-3.2.2/argcomplete.egg-info/requires.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       12 2024-01-23 20:48:10.000000 argcomplete-3.2.2/argcomplete.egg-info/top_level.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2200 2023-11-06 11:52:13.000000 argcomplete-3.2.2/common.mk
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-01-23 20:48:10.463798 argcomplete-3.2.2/contrib/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2888 2023-10-23 21:31:16.000000 argcomplete-3.2.2/contrib/README.rst
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-01-23 20:48:10.466108 argcomplete-3.2.2/docs/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       56 2023-10-23 21:31:16.000000 argcomplete-3.2.2/docs/changelog.rst
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1162 2023-10-23 21:31:16.000000 argcomplete-3.2.2/docs/conf.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-01-23 20:48:10.466503 argcomplete-3.2.2/docs/examples/
--rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)      721 2023-10-23 21:31:16.000000 argcomplete-3.2.2/docs/examples/describe_github_user.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    14171 2023-10-23 21:31:16.000000 argcomplete-3.2.2/docs/fish_help_string.png
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      293 2023-10-23 21:31:16.000000 argcomplete-3.2.2/docs/index.rst
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        8 2023-10-23 21:31:16.000000 argcomplete-3.2.2/docs/toc.html
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2043 2023-11-01 15:11:23.000000 argcomplete-3.2.2/pyproject.toml
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-01-23 20:48:10.467879 argcomplete-3.2.2/scripts/
--rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     5350 2023-12-03 01:13:18.000000 argcomplete-3.2.2/scripts/activate-global-python-argcomplete
--rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     2608 2023-10-23 21:31:17.000000 argcomplete-3.2.2/scripts/python-argcomplete-check-easy-install-script
--rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     1997 2023-10-23 21:31:17.000000 argcomplete-3.2.2/scripts/register-python-argcomplete
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      143 2024-01-23 20:48:10.472979 argcomplete-3.2.2/setup.cfg
--rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)      408 2023-10-23 21:31:16.000000 argcomplete-3.2.2/setup.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-01-23 20:48:10.469681 argcomplete-3.2.2/test/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2023-10-23 21:31:16.000000 argcomplete-3.2.2/test/__init__.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       31 2023-10-23 21:31:16.000000 argcomplete-3.2.2/test/inputrc
--rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     1764 2023-10-23 21:31:16.000000 argcomplete-3.2.2/test/prog
--rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)    59850 2023-12-10 15:15:17.000000 argcomplete-3.2.2/test/test.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3183 2023-10-23 21:31:16.000000 argcomplete-3.2.2/test/test_contrib_shells.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-01-23 20:48:10.470568 argcomplete-3.2.2/test/test_package/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2023-10-23 21:31:16.000000 argcomplete-3.2.2/test/test_package/__init__.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      299 2023-10-23 21:31:16.000000 argcomplete-3.2.2/test/test_package/setup.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       94 2023-10-23 21:31:16.000000 argcomplete-3.2.2/test/test_package/test_module.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-01-23 20:48:10.470898 argcomplete-3.2.2/test/test_package/test_package/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      289 2023-10-23 21:31:16.000000 argcomplete-3.2.2/test/test_package/test_package/__init__.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-03-08 01:30:04.593095 argcomplete-3.2.3/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-03-08 01:30:04.572384 argcomplete-3.2.3/.github/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       18 2023-10-23 21:31:17.000000 argcomplete-3.2.3/.github/FUNDING.yml
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-03-08 01:30:04.572930 argcomplete-3.2.3/.github/workflows/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1253 2023-12-29 01:33:45.000000 argcomplete-3.2.3/.github/workflows/ci.yml
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      474 2023-10-23 21:31:17.000000 argcomplete-3.2.3/.gitignore
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       35 2023-10-23 21:31:18.000000 argcomplete-3.2.3/Authors.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    14653 2024-03-08 01:29:41.000000 argcomplete-3.2.3/Changes.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    10174 2023-10-23 21:31:17.000000 argcomplete-3.2.3/LICENSE.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       79 2023-10-23 21:31:16.000000 argcomplete-3.2.3/MANIFEST.in
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      766 2023-10-23 21:31:16.000000 argcomplete-3.2.3/Makefile
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      387 2023-10-23 21:31:16.000000 argcomplete-3.2.3/NOTICE
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    16580 2024-03-08 01:30:04.592744 argcomplete-3.2.3/PKG-INFO
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    14692 2023-11-01 15:21:48.000000 argcomplete-3.2.3/README.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      705 2023-10-23 21:31:54.000000 argcomplete-3.2.3/SECURITY.md
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-03-08 01:30:04.578174 argcomplete-3.2.3/argcomplete/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      693 2023-10-23 21:31:16.000000 argcomplete-3.2.3/argcomplete/__init__.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2413 2024-01-29 17:15:56.000000 argcomplete-3.2.3/argcomplete/_check_console_script.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2616 2024-01-29 17:16:05.000000 argcomplete-3.2.3/argcomplete/_check_module.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-03-08 01:30:04.581451 argcomplete-3.2.3/argcomplete/bash_completion.d/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     9852 2024-01-23 20:39:07.000000 argcomplete-3.2.3/argcomplete/bash_completion.d/_python-argcomplete
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3980 2023-10-23 21:31:16.000000 argcomplete-3.2.3/argcomplete/completers.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      112 2023-10-23 21:31:16.000000 argcomplete-3.2.3/argcomplete/exceptions.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    28143 2024-01-29 17:14:15.000000 argcomplete-3.2.3/argcomplete/finders.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      866 2023-10-23 21:31:16.000000 argcomplete-3.2.3/argcomplete/io.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2131 2023-10-23 21:31:16.000000 argcomplete-3.2.3/argcomplete/lexers.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-03-08 01:30:04.582984 argcomplete-3.2.3/argcomplete/packages/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2023-10-23 21:31:16.000000 argcomplete-3.2.3/argcomplete/packages/__init__.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    15846 2024-01-23 20:47:39.000000 argcomplete-3.2.3/argcomplete/packages/_argparse.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    12766 2024-01-23 20:47:39.000000 argcomplete-3.2.3/argcomplete/packages/_shlex.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2023-10-23 21:31:16.000000 argcomplete-3.2.3/argcomplete/py.typed
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     7763 2024-03-08 01:27:42.000000 argcomplete-3.2.3/argcomplete/shell_integration.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-03-08 01:30:04.591945 argcomplete-3.2.3/argcomplete.egg-info/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    16580 2024-03-08 01:30:04.000000 argcomplete-3.2.3/argcomplete.egg-info/PKG-INFO
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1291 2024-03-08 01:30:04.000000 argcomplete-3.2.3/argcomplete.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2024-03-08 01:30:04.000000 argcomplete-3.2.3/argcomplete.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2024-03-08 01:29:47.000000 argcomplete-3.2.3/argcomplete.egg-info/not-zip-safe
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       41 2024-03-08 01:30:04.000000 argcomplete-3.2.3/argcomplete.egg-info/requires.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       12 2024-03-08 01:30:04.000000 argcomplete-3.2.3/argcomplete.egg-info/top_level.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2200 2023-11-06 11:52:13.000000 argcomplete-3.2.3/common.mk
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-03-08 01:30:04.583553 argcomplete-3.2.3/contrib/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2888 2023-10-23 21:31:16.000000 argcomplete-3.2.3/contrib/README.rst
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-03-08 01:30:04.585971 argcomplete-3.2.3/docs/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       56 2023-10-23 21:31:16.000000 argcomplete-3.2.3/docs/changelog.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1162 2023-10-23 21:31:16.000000 argcomplete-3.2.3/docs/conf.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-03-08 01:30:04.586338 argcomplete-3.2.3/docs/examples/
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)      721 2023-10-23 21:31:16.000000 argcomplete-3.2.3/docs/examples/describe_github_user.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    14171 2023-10-23 21:31:16.000000 argcomplete-3.2.3/docs/fish_help_string.png
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      293 2023-10-23 21:31:16.000000 argcomplete-3.2.3/docs/index.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        8 2023-10-23 21:31:16.000000 argcomplete-3.2.3/docs/toc.html
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2043 2023-11-01 15:11:23.000000 argcomplete-3.2.3/pyproject.toml
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-03-08 01:30:04.587934 argcomplete-3.2.3/scripts/
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     5350 2023-12-03 01:13:18.000000 argcomplete-3.2.3/scripts/activate-global-python-argcomplete
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     2608 2023-10-23 21:31:17.000000 argcomplete-3.2.3/scripts/python-argcomplete-check-easy-install-script
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     1997 2023-10-23 21:31:17.000000 argcomplete-3.2.3/scripts/register-python-argcomplete
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      143 2024-03-08 01:30:04.593461 argcomplete-3.2.3/setup.cfg
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)      408 2023-10-23 21:31:16.000000 argcomplete-3.2.3/setup.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-03-08 01:30:04.590208 argcomplete-3.2.3/test/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2023-10-23 21:31:16.000000 argcomplete-3.2.3/test/__init__.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       31 2023-10-23 21:31:16.000000 argcomplete-3.2.3/test/inputrc
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     1764 2023-10-23 21:31:16.000000 argcomplete-3.2.3/test/prog
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)    59850 2023-12-10 15:15:17.000000 argcomplete-3.2.3/test/test.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3183 2023-10-23 21:31:16.000000 argcomplete-3.2.3/test/test_contrib_shells.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-03-08 01:30:04.591114 argcomplete-3.2.3/test/test_package/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2023-10-23 21:31:16.000000 argcomplete-3.2.3/test/test_package/__init__.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      299 2023-10-23 21:31:16.000000 argcomplete-3.2.3/test/test_package/setup.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       94 2023-10-23 21:31:16.000000 argcomplete-3.2.3/test/test_package/test_module.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-03-08 01:30:04.591488 argcomplete-3.2.3/test/test_package/test_package/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      289 2023-10-23 21:31:16.000000 argcomplete-3.2.3/test/test_package/test_package/__init__.py
```

### Comparing `argcomplete-3.2.2/.github/workflows/ci.yml` & `argcomplete-3.2.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `argcomplete-3.2.2/Changes.rst` & `argcomplete-3.2.3/Changes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Changes for v3.2.3 (2024-03-07)
+===============================
+
+-  Allow register-python-argcomplete output to be used as lazy-loaded
+   zsh completion module (#475)
+
+-  Move debug_stream initialization to helper method to allow fd 9
+   behavior to be overridden in subclasses (#471)
+
 Changes for v3.2.2 (2024-01-23)
 ===============================
 
 Expand tilde in zsh
 
 Changes for v3.2.1 (2023-12-10)
 ===============================
```

### Comparing `argcomplete-3.2.2/LICENSE.rst` & `argcomplete-3.2.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `argcomplete-3.2.2/Makefile` & `argcomplete-3.2.3/Makefile`

 * *Files identical despite different names*

### Comparing `argcomplete-3.2.2/PKG-INFO` & `argcomplete-3.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argcomplete
-Version: 3.2.2
+Version: 3.2.3
 Summary: Bash tab completion for argparse
 Home-page: https://github.com/kislyuk/argcomplete
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Project-URL: Documentation, https://kislyuk.github.io/argcomplete
 Project-URL: Source Code, https://github.com/kislyuk/argcomplete
```

### Comparing `argcomplete-3.2.2/README.rst` & `argcomplete-3.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `argcomplete-3.2.2/SECURITY.md` & `argcomplete-3.2.3/SECURITY.md`

 * *Files identical despite different names*

### Comparing `argcomplete-3.2.2/argcomplete/__init__.py` & `argcomplete-3.2.3/argcomplete/__init__.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.2.2/argcomplete/_check_console_script.py` & `argcomplete-3.2.3/argcomplete/_check_console_script.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 the marker themselves, so we defer to the containing module or package.
 
 For more information on setuptools console_scripts, see
 https://setuptools.readthedocs.io/en/latest/setuptools.html#automatic-script-creation
 
 Intended to be invoked by argcomplete's global completion function.
 """
+
 import os
 import sys
 from importlib.metadata import EntryPoint
 from importlib.metadata import entry_points as importlib_entry_points
 from typing import Iterable
 
 from ._check_module import ArgcompleteMarkerNotFound, find
```

### Comparing `argcomplete-3.2.2/argcomplete/_check_module.py` & `argcomplete-3.2.3/argcomplete/_check_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Utility for locating a module (or package's __main__.py) with a given name
 and verifying it contains the PYTHON_ARGCOMPLETE_OK marker.
 
 The module name should be specified in a form usable with `python -m`.
 
 Intended to be invoked by argcomplete's global completion function.
 """
+
 import os
 import sys
 import tokenize
 
 try:
     from importlib.util import find_spec  # type:ignore
 except ImportError:
```

### Comparing `argcomplete-3.2.2/argcomplete/bash_completion.d/_python-argcomplete` & `argcomplete-3.2.3/argcomplete/bash_completion.d/_python-argcomplete`

 * *Files identical despite different names*

### Comparing `argcomplete-3.2.2/argcomplete/completers.py` & `argcomplete-3.2.3/argcomplete/completers.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.2.2/argcomplete/finders.py` & `argcomplete-3.2.3/argcomplete/finders.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,19 +113,15 @@
             default_completer=default_completer,
         )
 
         if "_ARGCOMPLETE" not in os.environ:
             # not an argument completion invocation
             return
 
-        try:
-            _io.debug_stream = os.fdopen(9, "w")
-        except Exception:
-            _io.debug_stream = sys.stderr
-        debug()
+        self._init_debug_stream()
 
         if output_stream is None:
             filename = os.environ.get("_ARGCOMPLETE_STDOUT_FILENAME")
             if filename is not None:
                 debug("Using output file {}".format(filename))
                 output_stream = open(filename, "w")
 
@@ -186,14 +182,27 @@
 
         debug("\nReturning completions:", completions)
         output_stream.write(ifs.join(completions))
         output_stream.flush()
         _io.debug_stream.flush()
         exit_method(0)
 
+    def _init_debug_stream(self):
+        """Initialize debug output stream
+
+        By default, writes to file descriptor 9, or stderr if that fails.
+        This can be overridden by derived classes, for example to avoid
+        clashes with file descriptors being used elsewhere (such as in pytest).
+        """
+        try:
+            _io.debug_stream = os.fdopen(9, "w")
+        except Exception:
+            _io.debug_stream = sys.stderr
+        debug()
+
     def _get_completions(self, comp_words, cword_prefix, cword_prequote, last_wordbreak_pos):
         active_parsers = self._patch_argument_parser()
 
         parsed_args = argparse.Namespace()
         self.completing = True
 
         try:
```

### Comparing `argcomplete-3.2.2/argcomplete/io.py` & `argcomplete-3.2.3/argcomplete/io.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.2.2/argcomplete/lexers.py` & `argcomplete-3.2.3/argcomplete/lexers.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.2.2/argcomplete/packages/_argparse.py` & `argcomplete-3.2.3/argcomplete/packages/_argparse.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.2.2/argcomplete/packages/_shlex.py` & `argcomplete-3.2.3/argcomplete/packages/_shlex.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.2.2/argcomplete/shell_integration.py` & `argcomplete-3.2.3/argcomplete/shell_integration.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2012-2023, Andrey Kislyuk and argcomplete contributors. Licensed under the terms of the
 # `Apache License, Version 2.0 <http://www.apache.org/licenses/LICENSE-2.0>`_. Distribution of the LICENSE and NOTICE
 # files with source copies of this package and derivative works is **REQUIRED** as specified by the Apache License.
 # See https://github.com/kislyuk/argcomplete for more info.
 
 from shlex import quote
 
-bashcode = r"""
+bashcode = r"""#compdef %(executables)s
 # Run something, muting output or redirecting it to the debug stream
 # depending on the value of _ARC_DEBUG.
 # If ARGCOMPLETE_USE_TEMPFILES is set, use tempfiles for IPC.
 __python_argcomplete_run() {
     if [[ -z "${ARGCOMPLETE_USE_TEMPFILES-}" ]]; then
         __python_argcomplete_run_inner "$@"
         return
@@ -71,16 +71,24 @@
             compopt -o nospace
         fi
     fi
 }
 if [[ -z "${ZSH_VERSION-}" ]]; then
     complete %(complete_opts)s -F _python_argcomplete%(function_suffix)s %(executables)s
 else
+    # When called by the Zsh completion system, this will end with
+    # "loadautofunc" when initially autoloaded and "shfunc" later on, otherwise,
+    # the script was "eval"-ed so use "compdef" to register it with the
+    # completion system
     autoload is-at-least
-    compdef _python_argcomplete%(function_suffix)s %(executables)s
+    if [[ $zsh_eval_context == *func ]]; then
+        _python_argcomplete%(function_suffix)s "$@"
+    else
+        compdef _python_argcomplete%(function_suffix)s %(executables)s
+    fi
 fi
 """
 
 tcshcode = """\
 complete "%(executable)s" 'p@*@`python-argcomplete-tcsh "%(argcomplete_script)s"`@' ;
 """
```

### Comparing `argcomplete-3.2.2/argcomplete.egg-info/PKG-INFO` & `argcomplete-3.2.3/argcomplete.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argcomplete
-Version: 3.2.2
+Version: 3.2.3
 Summary: Bash tab completion for argparse
 Home-page: https://github.com/kislyuk/argcomplete
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Project-URL: Documentation, https://kislyuk.github.io/argcomplete
 Project-URL: Source Code, https://github.com/kislyuk/argcomplete
```

### Comparing `argcomplete-3.2.2/argcomplete.egg-info/SOURCES.txt` & `argcomplete-3.2.3/argcomplete.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `argcomplete-3.2.2/common.mk` & `argcomplete-3.2.3/common.mk`

 * *Files identical despite different names*

### Comparing `argcomplete-3.2.2/contrib/README.rst` & `argcomplete-3.2.3/contrib/README.rst`

 * *Files identical despite different names*

### Comparing `argcomplete-3.2.2/docs/conf.py` & `argcomplete-3.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.2.2/docs/examples/describe_github_user.py` & `argcomplete-3.2.3/docs/examples/describe_github_user.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.2.2/docs/fish_help_string.png` & `argcomplete-3.2.3/docs/fish_help_string.png`

 * *Files identical despite different names*

### Comparing `argcomplete-3.2.2/pyproject.toml` & `argcomplete-3.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `argcomplete-3.2.2/scripts/activate-global-python-argcomplete` & `argcomplete-3.2.3/scripts/activate-global-python-argcomplete`

 * *Files identical despite different names*

### Comparing `argcomplete-3.2.2/scripts/python-argcomplete-check-easy-install-script` & `argcomplete-3.2.3/scripts/python-argcomplete-check-easy-install-script`

 * *Files identical despite different names*

### Comparing `argcomplete-3.2.2/scripts/register-python-argcomplete` & `argcomplete-3.2.3/scripts/register-python-argcomplete`

 * *Files identical despite different names*

### Comparing `argcomplete-3.2.2/test/prog` & `argcomplete-3.2.3/test/prog`

 * *Files identical despite different names*

### Comparing `argcomplete-3.2.2/test/test.py` & `argcomplete-3.2.3/test/test.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.2.2/test/test_contrib_shells.py` & `argcomplete-3.2.3/test/test_contrib_shells.py`

 * *Files identical despite different names*

