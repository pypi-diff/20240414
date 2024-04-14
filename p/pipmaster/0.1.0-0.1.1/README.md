# Comparing `tmp/pipmaster-0.1.0.tar.gz` & `tmp/pipmaster-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipmaster-0.1.0.tar", last modified: Sun Apr 14 20:30:38 2024, max compression
+gzip compressed data, was "pipmaster-0.1.1.tar", last modified: Sun Apr 14 20:31:31 2024, max compression
```

## Comparing `pipmaster-0.1.0.tar` & `pipmaster-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 20:30:38.438933 pipmaster-0.1.0/
--rw-rw-rw-   0        0        0    11558 2024-04-14 11:47:19.000000 pipmaster-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2443 2024-04-14 20:30:38.437340 pipmaster-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1581 2024-04-14 12:14:51.000000 pipmaster-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 20:30:38.412724 pipmaster-0.1.0/pipmaster/
--rw-rw-rw-   0        0        0     1941 2024-04-14 12:02:07.000000 pipmaster-0.1.0/pipmaster/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 20:30:38.436297 pipmaster-0.1.0/pipmaster.egg-info/
--rw-rw-rw-   0        0        0     2443 2024-04-14 20:30:38.000000 pipmaster-0.1.0/pipmaster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2024-04-14 20:30:38.000000 pipmaster-0.1.0/pipmaster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 20:30:38.000000 pipmaster-0.1.0/pipmaster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-14 20:30:38.000000 pipmaster-0.1.0/pipmaster.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-14 20:30:38.000000 pipmaster-0.1.0/pipmaster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 20:30:38.438933 pipmaster-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1201 2024-04-14 20:30:27.000000 pipmaster-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 20:31:31.391986 pipmaster-0.1.1/
+-rw-rw-rw-   0        0        0    11558 2024-04-14 11:47:19.000000 pipmaster-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2452 2024-04-14 20:31:31.390988 pipmaster-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1590 2024-04-14 20:31:10.000000 pipmaster-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 20:31:31.373975 pipmaster-0.1.1/pipmaster/
+-rw-rw-rw-   0        0        0     1941 2024-04-14 12:02:07.000000 pipmaster-0.1.1/pipmaster/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 20:31:31.390988 pipmaster-0.1.1/pipmaster.egg-info/
+-rw-rw-rw-   0        0        0     2452 2024-04-14 20:31:31.000000 pipmaster-0.1.1/pipmaster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2024-04-14 20:31:31.000000 pipmaster-0.1.1/pipmaster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 20:31:31.000000 pipmaster-0.1.1/pipmaster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-14 20:31:31.000000 pipmaster-0.1.1/pipmaster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-14 20:31:31.000000 pipmaster-0.1.1/pipmaster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 20:31:31.392986 pipmaster-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1201 2024-04-14 20:31:25.000000 pipmaster-0.1.1/setup.py
```

### Comparing `pipmaster-0.1.0/LICENSE` & `pipmaster-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pipmaster-0.1.0/PKG-INFO` & `pipmaster-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipmaster
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple and versatile Python package manager for automating installation and verification across platforms.
 Home-page: https://github.com/ParisNeo/pymanage
 Author: ParisNeo
 Author-email: parisneoai@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,32 +15,32 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ascii-colors
 
-# pymanage
+# pipmaster
 
-[![GitHub stars](https://img.shields.io/github/stars/ParisNeo/pymanage.svg?style=social&label=Stars)](https://github.com/ParisNeo/pymanage)
-[![PyPI version](https://badge.fury.io/py/pymanage.svg)](https://badge.fury.io/py/pymanage)
-[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/ParisNeo/pymanage/blob/main/LICENSE)
+[![GitHub stars](https://img.shields.io/github/stars/ParisNeo/pipmaster.svg?style=social&label=Stars)](https://github.com/ParisNeo/pipmaster)
+[![PyPI version](https://badge.fury.io/py/pipmaster.svg)](https://badge.fury.io/py/pipmaster)
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/ParisNeo/pipmaster/blob/main/LICENSE)
 
 A simple and versatile Python package manager for automating installation and verification across platforms.
 
 ## Installation
 
 ```
-pip install pymanage
+pip install pipmaster
 ```
 
 ## Usage
 
 ```python
-from pymanage import PackageManager
+from pipmaster import PackageManager
 
 # Create a PackageManager instance
 pm = PackageManager()
 
 # Install a package
 pm.install("requests")
 
@@ -51,15 +51,15 @@
 # Get information about an installed package
 package_info = pm.get_package_info("pandas")
 print(package_info)
 ```
 
 ## Contributing
 
-Contributions are welcome! Please open an issue or submit a pull request on the [GitHub repository](https://github.com/ParisNeo/pymanage).
+Contributions are welcome! Please open an issue or submit a pull request on the [GitHub repository](https://github.com/ParisNeo/pipmaster).
 
 ## Author
 
 - ParisNeo ([@ParisNeo_AI](https://twitter.com/ParisNeo_AI))
 
 ## Social
```

### Comparing `pipmaster-0.1.0/README.md` & `pipmaster-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# pymanage
+# pipmaster
 
-[![GitHub stars](https://img.shields.io/github/stars/ParisNeo/pymanage.svg?style=social&label=Stars)](https://github.com/ParisNeo/pymanage)
-[![PyPI version](https://badge.fury.io/py/pymanage.svg)](https://badge.fury.io/py/pymanage)
-[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/ParisNeo/pymanage/blob/main/LICENSE)
+[![GitHub stars](https://img.shields.io/github/stars/ParisNeo/pipmaster.svg?style=social&label=Stars)](https://github.com/ParisNeo/pipmaster)
+[![PyPI version](https://badge.fury.io/py/pipmaster.svg)](https://badge.fury.io/py/pipmaster)
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/ParisNeo/pipmaster/blob/main/LICENSE)
 
 A simple and versatile Python package manager for automating installation and verification across platforms.
 
 ## Installation
 
 ```
-pip install pymanage
+pip install pipmaster
 ```
 
 ## Usage
 
 ```python
-from pymanage import PackageManager
+from pipmaster import PackageManager
 
 # Create a PackageManager instance
 pm = PackageManager()
 
 # Install a package
 pm.install("requests")
 
@@ -30,15 +30,15 @@
 # Get information about an installed package
 package_info = pm.get_package_info("pandas")
 print(package_info)
 ```
 
 ## Contributing
 
-Contributions are welcome! Please open an issue or submit a pull request on the [GitHub repository](https://github.com/ParisNeo/pymanage).
+Contributions are welcome! Please open an issue or submit a pull request on the [GitHub repository](https://github.com/ParisNeo/pipmaster).
 
 ## Author
 
 - ParisNeo ([@ParisNeo_AI](https://twitter.com/ParisNeo_AI))
 
 ## Social
```

### Comparing `pipmaster-0.1.0/pipmaster/__init__.py` & `pipmaster-0.1.1/pipmaster/__init__.py`

 * *Files identical despite different names*

### Comparing `pipmaster-0.1.0/pipmaster.egg-info/PKG-INFO` & `pipmaster-0.1.1/pipmaster.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipmaster
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple and versatile Python package manager for automating installation and verification across platforms.
 Home-page: https://github.com/ParisNeo/pymanage
 Author: ParisNeo
 Author-email: parisneoai@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,32 +15,32 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ascii-colors
 
-# pymanage
+# pipmaster
 
-[![GitHub stars](https://img.shields.io/github/stars/ParisNeo/pymanage.svg?style=social&label=Stars)](https://github.com/ParisNeo/pymanage)
-[![PyPI version](https://badge.fury.io/py/pymanage.svg)](https://badge.fury.io/py/pymanage)
-[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/ParisNeo/pymanage/blob/main/LICENSE)
+[![GitHub stars](https://img.shields.io/github/stars/ParisNeo/pipmaster.svg?style=social&label=Stars)](https://github.com/ParisNeo/pipmaster)
+[![PyPI version](https://badge.fury.io/py/pipmaster.svg)](https://badge.fury.io/py/pipmaster)
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/ParisNeo/pipmaster/blob/main/LICENSE)
 
 A simple and versatile Python package manager for automating installation and verification across platforms.
 
 ## Installation
 
 ```
-pip install pymanage
+pip install pipmaster
 ```
 
 ## Usage
 
 ```python
-from pymanage import PackageManager
+from pipmaster import PackageManager
 
 # Create a PackageManager instance
 pm = PackageManager()
 
 # Install a package
 pm.install("requests")
 
@@ -51,15 +51,15 @@
 # Get information about an installed package
 package_info = pm.get_package_info("pandas")
 print(package_info)
 ```
 
 ## Contributing
 
-Contributions are welcome! Please open an issue or submit a pull request on the [GitHub repository](https://github.com/ParisNeo/pymanage).
+Contributions are welcome! Please open an issue or submit a pull request on the [GitHub repository](https://github.com/ParisNeo/pipmaster).
 
 ## Author
 
 - ParisNeo ([@ParisNeo_AI](https://twitter.com/ParisNeo_AI))
 
 ## Social
```

### Comparing `pipmaster-0.1.0/setup.py` & `pipmaster-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt', 'r') as f:
     install_requires = f.read().splitlines()
 
 setup(
     name="pipmaster",
-    version="0.1.0",
+    version="0.1.1",
     author="ParisNeo",
     author_email="parisneoai@gmail.com",
     description="A simple and versatile Python package manager for automating installation and verification across platforms.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/pymanage",
     packages=find_packages(),
```

