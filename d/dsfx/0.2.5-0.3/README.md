# Comparing `tmp/dsfx-0.2.5.tar.gz` & `tmp/dsfx-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsfx-0.2.5.tar", last modified: Mon Apr  8 12:02:13 2024, max compression
+gzip compressed data, was "dsfx-0.3.tar", last modified: Sun Apr 14 09:40:46 2024, max compression
```

## Comparing `dsfx-0.2.5.tar` & `dsfx-0.3.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-08 12:02:13.103269 dsfx-0.2.5/
--rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-03-28 18:30:28.000000 dsfx-0.2.5/LICENSE
--rw-r--r--   0 d33pster   (501) staff       (20)     7546 2024-04-08 12:02:13.102733 dsfx-0.2.5/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)     5245 2024-03-30 16:34:05.000000 dsfx-0.2.5/README.md
--rw-r--r--   0 d33pster   (501) staff       (20)     1233 2024-04-08 11:59:15.000000 dsfx-0.2.5/pyproject.toml
--rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-08 12:02:13.103332 dsfx-0.2.5/setup.cfg
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-08 12:02:13.094426 dsfx-0.2.5/src/
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-08 12:02:13.097113 dsfx-0.2.5/src/dsfx/
--rw-r--r--   0 d33pster   (501) staff       (20)       22 2024-03-30 16:08:42.000000 dsfx-0.2.5/src/dsfx/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)    23641 2024-03-30 16:30:22.000000 dsfx-0.2.5/src/dsfx/dsfx.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-08 12:02:13.102047 dsfx-0.2.5/src/dsfx.egg-info/
--rw-r--r--   0 d33pster   (501) staff       (20)     7546 2024-04-08 12:02:13.000000 dsfx-0.2.5/src/dsfx.egg-info/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      264 2024-04-08 12:02:13.000000 dsfx-0.2.5/src/dsfx.egg-info/SOURCES.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-08 12:02:13.000000 dsfx-0.2.5/src/dsfx.egg-info/dependency_links.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       39 2024-04-08 12:02:13.000000 dsfx-0.2.5/src/dsfx.egg-info/entry_points.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       34 2024-04-08 12:02:13.000000 dsfx-0.2.5/src/dsfx.egg-info/requires.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        5 2024-04-08 12:02:13.000000 dsfx-0.2.5/src/dsfx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:40:46.079064 dsfx-0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-14 09:40:42.000000 dsfx-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8028 2024-04-14 09:40:46.079064 dsfx-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-04-14 09:40:42.000000 dsfx-0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-14 09:40:42.000000 dsfx-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 09:40:46.079064 dsfx-0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:40:46.075063 dsfx-0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:40:46.079064 dsfx-0.3/src/dsfx/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-14 09:40:42.000000 dsfx-0.3/src/dsfx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29643 2024-04-14 09:40:42.000000 dsfx-0.3/src/dsfx/dsfx.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-14 09:40:42.000000 dsfx-0.3/src/dsfx/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:40:46.079064 dsfx-0.3/src/dsfx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8028 2024-04-14 09:40:46.000000 dsfx-0.3/src/dsfx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-14 09:40:46.000000 dsfx-0.3/src/dsfx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 09:40:46.000000 dsfx-0.3/src/dsfx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-14 09:40:46.000000 dsfx-0.3/src/dsfx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-14 09:40:46.000000 dsfx-0.3/src/dsfx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-14 09:40:46.000000 dsfx-0.3/src/dsfx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:40:46.079064 dsfx-0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-14 09:40:42.000000 dsfx-0.3/test/test_archives.py
```

### Comparing `dsfx-0.2.5/LICENSE` & `dsfx-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dsfx-0.2.5/PKG-INFO` & `dsfx-0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsfx
-Version: 0.2.5
+Version: 0.3
 Summary: create installer packages
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -35,28 +35,32 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.1
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: optioner>=1.4.1
+Requires-Dist: optioner>=1.5.2
 Requires-Dist: colorama
 Requires-Dist: argparse
+Requires-Dist: cryptography
+Requires-Dist: pyinstaller
 
 # dsfx
-
-![GitHub last commit](https://img.shields.io/github/last-commit/d33pster/dsfx)
+[![Build status](https://ci.appveyor.com/api/projects/status/nd0u2o25ad9myfib?svg=true)](https://ci.appveyor.com/project/d33pster/dsfx)
+[![codecov](https://codecov.io/gh/d33pster/dsfx/graph/badge.svg?token=OHSJBMP7QO)](https://codecov.io/gh/d33pster/dsfx)
+[![Features Test CI](https://github.com/d33pster/dsfx/actions/workflows/FeaturesTestCI.yml/badge.svg)](https://github.com/d33pster/dsfx/actions/workflows/FeaturesTestCI.yml)
 ![PyPI - Status](https://img.shields.io/pypi/status/dsfx)
+![PyPI - Version](https://img.shields.io/pypi/v/dsfx)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/dsfx)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dsfx)
-![PyPI - Version](https://img.shields.io/pypi/v/dsfx)
+![GitHub last commit](https://img.shields.io/github/last-commit/d33pster/dsfx)
 ![GitHub License](https://img.shields.io/github/license/d33pster/dsfx)
 
 <p align='center'>
     <a href='#Installation'>Installation</a>
     &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
     <a href='#Usage'>Usage</a>
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dsfx Version: 0.2.5 Summary: create installer
+Metadata-Version: 2.1 Name: dsfx Version: 0.3 Summary: create installer
 packages Author-email: Soumyo Deep Gupta
 gmail.com> Maintainer-email: Soumyo Deep Gupta
 gmail.com> License: MIT License Copyright (c) 2024 Soumyo Deep Gupta Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -20,23 +20,29 @@
 Documentation, https://d33pster.github.io/dsfx/ Keywords:
 d33pster,pymakeself,makeself,makesfx,dsfx,pythonsfx Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Topic :: Software Development :: Build Tools Classifier: Programming Language
 :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Requires-Python: >=3.1 Description-Content-
-Type: text/markdown License-File: LICENSE Requires-Dist: optioner>=1.4.1
-Requires-Dist: colorama Requires-Dist: argparse # dsfx ![GitHub last commit]
-(https://img.shields.io/github/last-commit/d33pster/dsfx) ![PyPI - Status]
-(https://img.shields.io/pypi/status/dsfx) ![PyPI - Implementation](https://
-img.shields.io/pypi/implementation/dsfx) ![PyPI - Python Version](https://
-img.shields.io/pypi/pyversions/dsfx) ![PyPI - Version](https://img.shields.io/
-pypi/v/dsfx) ![GitHub License](https://img.shields.io/github/license/d33pster/
-dsfx)
+Operating System :: OS Independent Requires-Python: >=3.9 Description-Content-
+Type: text/markdown License-File: LICENSE Requires-Dist: optioner>=1.5.2
+Requires-Dist: colorama Requires-Dist: argparse Requires-Dist: cryptography
+Requires-Dist: pyinstaller # dsfx [![Build status](https://ci.appveyor.com/api/
+projects/status/nd0u2o25ad9myfib?svg=true)](https://ci.appveyor.com/project/
+d33pster/dsfx) [![codecov](https://codecov.io/gh/d33pster/dsfx/graph/
+badge.svg?token=OHSJBMP7QO)](https://codecov.io/gh/d33pster/dsfx) [![Features
+Test CI](https://github.com/d33pster/dsfx/actions/workflows/FeaturesTestCI.yml/
+badge.svg)](https://github.com/d33pster/dsfx/actions/workflows/
+FeaturesTestCI.yml) ![PyPI - Status](https://img.shields.io/pypi/status/dsfx) !
+[PyPI - Version](https://img.shields.io/pypi/v/dsfx) ![PyPI - Implementation]
+(https://img.shields.io/pypi/implementation/dsfx) ![PyPI - Python Version]
+(https://img.shields.io/pypi/pyversions/dsfx) ![GitHub last commit](https://
+img.shields.io/github/last-commit/d33pster/dsfx) ![GitHub License](https://
+img.shields.io/github/license/d33pster/dsfx)
                           _I_n_s_t_a_l_l_a_t_i_o_n    |    _U_s_a_g_e
 ## NOTE: Backing up your files before using dsfx is best practice dsfx is an
 upgraded version of pymakeself by Andrew Gillis, well, kind of.
 
 Changes: - python >= 3.9 support - choice of output file (OS specific
 executable file(with custom extension) or a .py file) - removed encryption
 support. - some features are made optional ## About dsfx is a part of warlock
```

### Comparing `dsfx-0.2.5/README.md` & `dsfx-0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # dsfx
-
-![GitHub last commit](https://img.shields.io/github/last-commit/d33pster/dsfx)
+[![Build status](https://ci.appveyor.com/api/projects/status/nd0u2o25ad9myfib?svg=true)](https://ci.appveyor.com/project/d33pster/dsfx)
+[![codecov](https://codecov.io/gh/d33pster/dsfx/graph/badge.svg?token=OHSJBMP7QO)](https://codecov.io/gh/d33pster/dsfx)
+[![Features Test CI](https://github.com/d33pster/dsfx/actions/workflows/FeaturesTestCI.yml/badge.svg)](https://github.com/d33pster/dsfx/actions/workflows/FeaturesTestCI.yml)
 ![PyPI - Status](https://img.shields.io/pypi/status/dsfx)
+![PyPI - Version](https://img.shields.io/pypi/v/dsfx)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/dsfx)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dsfx)
-![PyPI - Version](https://img.shields.io/pypi/v/dsfx)
+![GitHub last commit](https://img.shields.io/github/last-commit/d33pster/dsfx)
 ![GitHub License](https://img.shields.io/github/license/d33pster/dsfx)
 
 <p align='center'>
     <a href='#Installation'>Installation</a>
     &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
     <a href='#Usage'>Usage</a>
 </p>
```

#### html2text {}

```diff
@@ -1,13 +1,19 @@
-# dsfx ![GitHub last commit](https://img.shields.io/github/last-commit/
-d33pster/dsfx) ![PyPI - Status](https://img.shields.io/pypi/status/dsfx) ![PyPI
-- Implementation](https://img.shields.io/pypi/implementation/dsfx) ![PyPI -
-Python Version](https://img.shields.io/pypi/pyversions/dsfx) ![PyPI - Version]
-(https://img.shields.io/pypi/v/dsfx) ![GitHub License](https://img.shields.io/
-github/license/d33pster/dsfx)
+# dsfx [![Build status](https://ci.appveyor.com/api/projects/status/
+nd0u2o25ad9myfib?svg=true)](https://ci.appveyor.com/project/d33pster/dsfx) [!
+[codecov](https://codecov.io/gh/d33pster/dsfx/graph/
+badge.svg?token=OHSJBMP7QO)](https://codecov.io/gh/d33pster/dsfx) [![Features
+Test CI](https://github.com/d33pster/dsfx/actions/workflows/FeaturesTestCI.yml/
+badge.svg)](https://github.com/d33pster/dsfx/actions/workflows/
+FeaturesTestCI.yml) ![PyPI - Status](https://img.shields.io/pypi/status/dsfx) !
+[PyPI - Version](https://img.shields.io/pypi/v/dsfx) ![PyPI - Implementation]
+(https://img.shields.io/pypi/implementation/dsfx) ![PyPI - Python Version]
+(https://img.shields.io/pypi/pyversions/dsfx) ![GitHub last commit](https://
+img.shields.io/github/last-commit/d33pster/dsfx) ![GitHub License](https://
+img.shields.io/github/license/d33pster/dsfx)
                           _I_n_s_t_a_l_l_a_t_i_o_n    |    _U_s_a_g_e
 ## NOTE: Backing up your files before using dsfx is best practice dsfx is an
 upgraded version of pymakeself by Andrew Gillis, well, kind of.
 
 Changes: - python >= 3.9 support - choice of output file (OS specific
 executable file(with custom extension) or a .py file) - removed encryption
 support. - some features are made optional ## About dsfx is a part of warlock
```

### Comparing `dsfx-0.2.5/pyproject.toml` & `dsfx-0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dsfx"
-version = "0.2.5"
+version = "0.3"
 description = "create installer packages"
-requires-python = ">=3.1"
+requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    'optioner>=1.4.1',
+    'optioner>=1.5.2',
     'colorama',
-    'argparse'
+    'argparse',
+    'cryptography',
+    'pyinstaller'
 ]
 keywords = ['d33pster', 'pymakeself', 'makeself', 'makesfx', 'dsfx', 'pythonsfx']
 readme = {file = "README.md", content-type = "text/markdown"}
 license = { file = "LICENSE" }
 authors = [
     {name = "Soumyo Deep Gupta", email = "deep.main.ac@gmail.com"}
 ]
```

### Comparing `dsfx-0.2.5/src/dsfx/dsfx.py` & `dsfx-0.3/src/dsfx/dsfx.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,19 +4,24 @@
 from __future__ import absolute_import
 
 __version__ = '0.2.4'
 
 from os import system as mkdir, getcwd as pwd, chdir, unlink, chmod, makedirs
 from os.path import isdir, isfile, abspath, dirname, basename, join, exists as there, relpath
 from shutil import rmtree, ignore_patterns as shutil_ignp, copytree, copyfile, copymode
+from cryptography.fernet import Fernet
+from cryptography.hazmat.primitives.hashes import SHA256
+from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
+from dsfx.exceptions import ParameterNotSet
+from re import match
 from tarfile import open as topen
 from platform import system as getos
 from sys import stderr, argv
 from optioner import options
-from base64 import encode as bencode
+from base64 import encode as bencode, urlsafe_b64encode
 from colorama import init as color, Fore as _
 import subprocess
 import stat
 import curses
 try:
     import lzma
 except ImportError:
@@ -26,43 +31,70 @@
     def __init__(self):
         self._os = getos()
         self._exe_format_ = \
             b"""
 from __future__ import print_function
 from os import unlink, getcwd as pwd, chdir, chmod
 from os.path import join, basename, dirname, abspath
-from base64 import decodebytes as db
+from base64 import decodebytes as db, urlsafe_b64encode
 from sys import argv, stderr
-import sys
+from cryptography.fernet import Fernet, InvalidToken
+from cryptography.exceptions import InvalidSignature
+from cryptography.hazmat.primitives.hashes import SHA256
+from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
 from shutil import rmtree
 from tarfile import open as topen
 import argparse
 import datetime
 import subprocess
 import stat
+import sys
 from colorama import init as color, Fore as _
 
 def main():
+    global _tarname, sha256_sum, label, _pkgname, _setup, in_content, _setupargs, encryption, salt, DATA
     color()
     arguments = argparse.ArgumentParser(description='dsfx sfx')
     arguments.add_argument('--check', action='store_true', help='check sfx integrity')
     arguments.add_argument('--list', action='store_true', help='List the files inside the sfx')
     arguments.add_argument('--extract', action='store_true', help='Extract and exit')
     arguments.add_argument('args', nargs=argparse.REMAINDER, help='setup arguments')
     args = arguments.parse_args()
     
     _tempd = pwd()
     _originald = None
     
     try:
+        
+        if encryption:
+            password0 = input('password: ')
+            kdf = PBKDF2HMAC(
+                algorithm=SHA256(),
+                length=32,
+                iterations=480000,
+                salt=salt.encode('ascii'),
+            )
+            password = urlsafe_b64encode(kdf.derive(password0.encode('ascii')))
+            fernet = Fernet(password)
+            try:
+                try:
+                    DATA = fernet.decrypt(DATA)
+                except:
+                    print('password ERROR')
+                    sys.exit(1)
+            except:
+                sys.exit(1)
     
-        # put the tar file in temp dir
+        # put the tar file in current dir
         _tar = join(_tempd, _tarname)
         with open(_tar, 'wb') as f:
-            f.write(db(DATA))
+            if not encryption:
+                f.write(db(DATA))
+            else:
+                f.write(DATA)
         
         def check_integrity(default = False):
             if default:
                 if sha256_sum:
                     import hashlib
                     BLOCKSIZE = 65536
                     sha256 = hashlib.sha256()
@@ -177,15 +209,15 @@
     except RuntimeError as e:
         print(e, file=stderr)
         return 1
     
     return 0
 """
         
-    def _make(self, content: str, outfile: str, _setup: str, _setupargs=(), executable=True, sha256=False, compress='gz', quiet=False, label=None, extension='.dsfx'):
+    def _make(self, content: str, outfile: str, _setup: str, _setupargs:tuple=(), executable:bool=True, sha256:bool=False, compress:str='gz', quiet:bool=False, label:str=None, extension: str='.dsfx', encryption: bool = False, password:str='', salt:str=''):
         """Create SFX
 
         Args:
             content (str): input directory
             outfile (str): output executable name
             _setup (str): setup file which will be executed from the extracted content dir
             _setupargs (tuple, optional): setup file arguments if any. Defaults to ().
@@ -232,41 +264,64 @@
         if not isfile(_setup):
             raise RuntimeError(f'setup is not valid: {_setup}')
         
         # remove .py extension from outfile name if it is there, any other can be allowed
         if outfile.endswith('.py'):
             outfile = outfile.rsplit('.py', 1)[0]
         
+        # encryption setup
+        if encryption:
+            if password=='':
+                raise ParameterNotSet('Password parameter is empty.')
+            if salt=='':
+                raise ParameterNotSet('Salt parameter is empty.')
+            
+            self.usersalt = salt
+            
+            self.userkdf = PBKDF2HMAC(
+                algorithm=SHA256(),
+                length=32,
+                iterations=480000,
+                salt=self.usersalt.encode('ascii'),
+            )
+            
+            self.userpassword0 = password
+            self.userpassword = urlsafe_b64encode(self.userkdf.derive(self.userpassword0.encode('ascii')))
+            self.userfernet = Fernet(self.userpassword)
+        
         # create a temp dir to work on
         _tempd =  pwd() # mkt('_makesfx')
         # set _pkg dir
         _pkg = join(_tempd, basename(outfile))
         
         # copy files
 
         _copy_package_files(_pkg, content, _setup, in_content, quiet)
         _tar, sha256_sum = _archive_package(_pkg, compress, sha256, quiet)
-        self._midfile = self._pkg_to_exe(_tar, outfile, _setup, _setupargs, in_content, sha256_sum, label, quiet)
+        if encryption:
+            _enctar, sha256_sum = self.encrypt(_tar, quiet, sha256)
+        else:
+            _enctar = _tar
+        self._midfile = self._pkg_to_exe(_enctar, outfile, _setup, _setupargs, in_content, sha256_sum, label, quiet, encryption)
         
         # set exe name
         _exe_name = basename(self._midfile).split('.')[0] ## remove py extension
         
         # directory at this point is the directory where the script has started
         
         # change to current directory ==> dont
         # chdir(dirname(abspath(__file__)))
         
         _current = pwd()
         
-        if not quiet:
-            print(f'\n{_.RED}Running Pyinstaller{_.RESET}\n')
-        
         # use pyinstaller to make executable of the final file
         if executable:
             if not quiet:
+                print(f'\n{_.RED}Running Pyinstaller{_.RESET}\n')
+            if not quiet:
                 subprocess.Popen(['pyinstaller', '--onefile', f'{self._midfile}']).wait()
             else:
                 subprocess.Popen(['pyinstaller', '--onefile', f'{self._midfile}'], stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL).wait()
             
             if not quiet:
                 print(f'\n{_.BLUE}Deleting{_.RESET} build')
             # delete build
@@ -312,15 +367,52 @@
             chmod(self._midfile,
                 stat.S_IRUSR | stat.S_IWUSR | stat.S_IXUSR |  # rwx user
                 stat.S_IRGRP | stat.S_IXGRP |                 # rx group
                 stat.S_IROTH | stat.S_IXOTH)                  # rx other
             
             return self._midfile
     
-    def _pkg_to_exe(self, _tar: str, outfile: str, _setup: str, _setupargs: tuple, in_content: bool, sha256_sum: str, label: str, quiet:bool = False):
+    def encrypt(self, _tar:str, quiet:bool, sha256:bool = False):
+        if not quiet:
+            print(f'{_.BLUE}Encrypting{_.RESET} {_tar} {_.BLUE}with{_.RESET} key->\'{self.userpassword0}\'', end='\r')
+        
+        with open(_tar, 'rb') as tarfile:
+            content = tarfile.read()
+        
+        content = self.userfernet.encrypt(content)
+        
+        with open(_tar, 'wb') as tarfile:
+            tarfile.write(content)
+        
+        if not quiet:
+            print('                                                                                          ', end='\r')
+            print(f'{_.GREEN}Encrypted{_.RESET} {_tar} {_.BLUE}with{_.RESET} key->\'{self.userpassword0}\'')
+        
+        sha256_sum = None
+        if sha256:
+            # import hashlib here and not on the top of the code
+            # incase user cannot use checksum and needs to omit
+            import hashlib
+            BLOCKSIZE = 65536
+            sha256_ = hashlib.sha256()
+            with open(_tar, 'rb') as tarf:
+                buf = tarf.read(BLOCKSIZE)
+                while buf:
+                    sha256_.update(buf)
+                    buf = tarf.read(BLOCKSIZE)
+            sha256_sum = sha256_.hexdigest()
+            if not quiet:
+                print(f'{_.BLUE}SHA256 - ENC{_.RESET} {basename(_tar)} = {sha256_sum}')
+        else:
+            if not quiet:
+                print(f'{_.RED}Skipped SHA256 Again{_.RESET}')
+        
+        return _tar, sha256_sum
+    
+    def _pkg_to_exe(self, _tar: str, outfile: str, _setup: str, _setupargs: tuple, in_content: bool, sha256_sum: str, label: str, quiet:bool = False, encryption:bool = False):
         _tarname = basename(_tar)
         _exe_mid = abspath(outfile) + '.py'
         
         if there(_exe_mid):
             if not quiet:
                 print(f'{_.BLUE}Removing existing midfile{_.RESET} {relpath(_exe_mid)}', file=stderr)
             unlink(_exe_mid)
@@ -358,32 +450,44 @@
                 else:
                     exemid.write(b"in_content = False\n")
                 
                 exemid.write(f"_setupargs = {repr(tuple(_setupargs))}\n".encode())
             else:
                 exemid.write(b"_setup = None\n")
             
+            if encryption:
+                exemid.write(b"encryption = True\n")
+                exemid.write(f"salt = \'{self.usersalt}\'\n".encode())
+            else:
+                exemid.write(b"encryption = False\n")
+            
             ## write base64 encoded tar file into executable script.
             exemid.write(b'\nDATA = b"""\n')
             with open(_tar, 'rb') as pkgf:
-                bencode(pkgf, exemid)
+                if not encryption:
+                    bencode(pkgf, exemid)
+                else:
+                    exemid.write(pkgf.read())
             exemid.write(b'"""\n\n')
             
             exemid.write(b'if __name__ == "__main__":\n')
             exemid.write(b'    sys.exit(main())\n')
     
         # remove the tar file that was written into the executable script.
         unlink(_tar)
         
         # set the permissions on the executable installer script that was created ====> no need
         return _exe_mid
         
         
 def _copy_package_files(_pkg: str, _install_src: str, _setup: str, in_content: bool, quiet:bool = False):
-    makedirs(_pkg,)
+    try:
+        makedirs(_pkg)
+    except FileExistsError:
+        raise RuntimeError(f'target dir already exits.')
     # set install destination
     install_dst = join(_pkg, 'infs')
     
     if not quiet:
         print(f'{_.BLUE}Packaging{_.RESET} from {_install_src}')
     # copy the files
     ignores = shutil_ignp('*~', '.#*', '.ssh')
@@ -489,14 +593,17 @@
         stdscr.addstr('    |    NORMAL ARGUMENTS\n    |\n')
         stdscr.scrollok(1)
         stdscr.addstr('    |    -c or --compress-method  -      set compression method. Possible values: [\'gz\', \'bz2\', \'xz\']\n')
         # stdscr.scrollok(1)
         stdscr.addstr('    |    -l or --label            -      set label text. Default: None\n')
         stdscr.scrollok(1)
         stdscr.addstr('    |    -e or --extension        -      specify output file extension. Default: \'*.dsfx\'\n')
+        stdscr.addstr('    |    -en or --encrypted       -      this sets encryption option to True, specify password and salt.\n')
+        stdscr.addstr('    |                                    if salt is not given, it will be default.(Not Recommended)\n')
+        stdscr.addstr('    |                                    Format: --encrypted <password> <salt>\n')
         # stdscr.scrollok(1)
         stdscr.addstr('    |    -cs or --checksum        -      set checksum true or false. if not specified, it is off. (switch)\n')
         # stdscr.scrollok(1)
         stdscr.addstr('    |    -q or --quiet            -      set quiet mode on. Default: off. (switch)\n')
         # stdscr.scrollok(1)
         stdscr.addstr('    |    -ne or --no-executable   -      Output .py file. Default: make executable file. (switch)')
         stdscr.addstr('\n\nEND')
@@ -512,29 +619,32 @@
         curses.endwin()
     
     exit(0)
 
 def cli():
     color()
     # define shortargs
-    shortargs = ['i', 'o', 's', 'c', 'l', 'e', 'cs', 'q', 'v', 'h', 'ne']
+    shortargs = ['i', 'o', 's', 'c', 'l', 'e', 'cs', 'q', 'v', 'h', 'ne', 'en']
     # define longargs
-    longargs = ['infile', 'outfile', 'setup', 'compress-method', 'label', 'extension', 'checksum', 'quiet', 'version', 'help', 'no-executable']
+    longargs = ['infile', 'outfile', 'setup', 'compress-method', 'label', 'extension', 'checksum', 'quiet', 'version', 'help', 'no-executable', 'encrypted']
     # get option control
     optionCTRL = options(shortargs, longargs, argv[1:], ['i','o','s'], ['infile', 'outfile', 'setup'], ['-h', '--help', '-v', '--version'])
     # get argument values
     actualargs, argcheck, argerror, falseargs = optionCTRL._argparse()
     
     # define checks and defaults
     extension = '.dsfx'
     label = ''
     compress_method = 'gz'
     checksum = False
     quiet = False
     executable = True
+    encryption = False
+    password = ''
+    salt = ''
     
     # if errors:
     if not argcheck:
         print(f'{_.RED}dsfx>{_.RESET} {argerror}')
         exit(1)
     else:
         # if version:
@@ -580,14 +690,50 @@
         if '-q' in actualargs:
             quiet = True
         elif '--quiet' in actualargs:
             quiet = True
         else:
             pass
         
+        if '-en' in actualargs or '--encrypted' in actualargs:
+            encryption = True
+            try:
+                index = argv.index('-en')
+            except ValueError:
+                index = argv.index('--encrypted')
+            
+            nextcommandindex = None
+            try:
+                for i in range(index+1, len(argv)):
+                    if match(r'^-', argv[i]) or match(r'^--', argv[i]):
+                        nextcommandindex = i
+                        break
+            except IndexError:
+                print('-en or --encrypted requires values')
+                exit(1)
+            
+            values:list[str] = []
+            
+            if nextcommandindex!=None:
+                for i in range(index+1, nextcommandindex):
+                    values.append(argv[i])
+            elif nextcommandindex==None:
+                for i in range(index+1, len(argv)):
+                    values.append(argv[i])
+            
+            if len(values)>2:
+                print('-en or --encrypted accepts only two values.')
+                exit(1)
+            elif len(values)<2:
+                print('-en or --encrypted requires two values.')
+                exit(1)
+            elif len(values)==2:
+                password = values[0]
+                salt = values[1]
+        
         ## get infile, outfile, setup and setupargs
         try:
             if '-i' in actualargs:
                 infile = optionCTRL._what_is_('i')
             elif '--infile' in actualargs:
                 infile = optionCTRL._what_is_('infile')
             else:
@@ -625,11 +771,11 @@
         setupargs = ()
         if len(optionCTRL._args[index:])>0:
             setupargs = tuple(optionCTRL._args[index:])
         
     # get class object
     sfxCTRL = _makesfx()
     # call class method
-    sfxCTRL._make(infile, outfile, setup, setupargs, executable, checksum, compress_method, quiet, label, extension)
+    sfxCTRL._make(infile, outfile, setup, setupargs, executable, checksum, compress_method, quiet, label, extension, encryption, password, salt)
 
 if __name__=="__main__":
     cli()
```

### Comparing `dsfx-0.2.5/src/dsfx.egg-info/PKG-INFO` & `dsfx-0.3/src/dsfx.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsfx
-Version: 0.2.5
+Version: 0.3
 Summary: create installer packages
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -35,28 +35,32 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.1
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: optioner>=1.4.1
+Requires-Dist: optioner>=1.5.2
 Requires-Dist: colorama
 Requires-Dist: argparse
+Requires-Dist: cryptography
+Requires-Dist: pyinstaller
 
 # dsfx
-
-![GitHub last commit](https://img.shields.io/github/last-commit/d33pster/dsfx)
+[![Build status](https://ci.appveyor.com/api/projects/status/nd0u2o25ad9myfib?svg=true)](https://ci.appveyor.com/project/d33pster/dsfx)
+[![codecov](https://codecov.io/gh/d33pster/dsfx/graph/badge.svg?token=OHSJBMP7QO)](https://codecov.io/gh/d33pster/dsfx)
+[![Features Test CI](https://github.com/d33pster/dsfx/actions/workflows/FeaturesTestCI.yml/badge.svg)](https://github.com/d33pster/dsfx/actions/workflows/FeaturesTestCI.yml)
 ![PyPI - Status](https://img.shields.io/pypi/status/dsfx)
+![PyPI - Version](https://img.shields.io/pypi/v/dsfx)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/dsfx)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dsfx)
-![PyPI - Version](https://img.shields.io/pypi/v/dsfx)
+![GitHub last commit](https://img.shields.io/github/last-commit/d33pster/dsfx)
 ![GitHub License](https://img.shields.io/github/license/d33pster/dsfx)
 
 <p align='center'>
     <a href='#Installation'>Installation</a>
     &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
     <a href='#Usage'>Usage</a>
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dsfx Version: 0.2.5 Summary: create installer
+Metadata-Version: 2.1 Name: dsfx Version: 0.3 Summary: create installer
 packages Author-email: Soumyo Deep Gupta
 gmail.com> Maintainer-email: Soumyo Deep Gupta
 gmail.com> License: MIT License Copyright (c) 2024 Soumyo Deep Gupta Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -20,23 +20,29 @@
 Documentation, https://d33pster.github.io/dsfx/ Keywords:
 d33pster,pymakeself,makeself,makesfx,dsfx,pythonsfx Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Topic :: Software Development :: Build Tools Classifier: Programming Language
 :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Requires-Python: >=3.1 Description-Content-
-Type: text/markdown License-File: LICENSE Requires-Dist: optioner>=1.4.1
-Requires-Dist: colorama Requires-Dist: argparse # dsfx ![GitHub last commit]
-(https://img.shields.io/github/last-commit/d33pster/dsfx) ![PyPI - Status]
-(https://img.shields.io/pypi/status/dsfx) ![PyPI - Implementation](https://
-img.shields.io/pypi/implementation/dsfx) ![PyPI - Python Version](https://
-img.shields.io/pypi/pyversions/dsfx) ![PyPI - Version](https://img.shields.io/
-pypi/v/dsfx) ![GitHub License](https://img.shields.io/github/license/d33pster/
-dsfx)
+Operating System :: OS Independent Requires-Python: >=3.9 Description-Content-
+Type: text/markdown License-File: LICENSE Requires-Dist: optioner>=1.5.2
+Requires-Dist: colorama Requires-Dist: argparse Requires-Dist: cryptography
+Requires-Dist: pyinstaller # dsfx [![Build status](https://ci.appveyor.com/api/
+projects/status/nd0u2o25ad9myfib?svg=true)](https://ci.appveyor.com/project/
+d33pster/dsfx) [![codecov](https://codecov.io/gh/d33pster/dsfx/graph/
+badge.svg?token=OHSJBMP7QO)](https://codecov.io/gh/d33pster/dsfx) [![Features
+Test CI](https://github.com/d33pster/dsfx/actions/workflows/FeaturesTestCI.yml/
+badge.svg)](https://github.com/d33pster/dsfx/actions/workflows/
+FeaturesTestCI.yml) ![PyPI - Status](https://img.shields.io/pypi/status/dsfx) !
+[PyPI - Version](https://img.shields.io/pypi/v/dsfx) ![PyPI - Implementation]
+(https://img.shields.io/pypi/implementation/dsfx) ![PyPI - Python Version]
+(https://img.shields.io/pypi/pyversions/dsfx) ![GitHub last commit](https://
+img.shields.io/github/last-commit/d33pster/dsfx) ![GitHub License](https://
+img.shields.io/github/license/d33pster/dsfx)
                           _I_n_s_t_a_l_l_a_t_i_o_n    |    _U_s_a_g_e
 ## NOTE: Backing up your files before using dsfx is best practice dsfx is an
 upgraded version of pymakeself by Andrew Gillis, well, kind of.
 
 Changes: - python >= 3.9 support - choice of output file (OS specific
 executable file(with custom extension) or a .py file) - removed encryption
 support. - some features are made optional ## About dsfx is a part of warlock
```

