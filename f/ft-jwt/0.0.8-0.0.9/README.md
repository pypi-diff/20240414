# Comparing `tmp/ft_jwt-0.0.8.tar.gz` & `tmp/ft_jwt-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ft_jwt-0.0.8.tar", last modified: Thu Apr  4 15:38:36 2024, max compression
+gzip compressed data, was "ft_jwt-0.0.9.tar", last modified: Thu Apr  4 15:40:23 2024, max compression
```

## Comparing `ft_jwt-0.0.8.tar` & `ft_jwt-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 15:38:36.000000 ft_jwt-0.0.8/
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1063 2024-04-04 14:17:44.000000 ft_jwt-0.0.8/LICENSE
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1852 2024-04-04 15:38:36.000000 ft_jwt-0.0.8/PKG-INFO
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1286 2024-04-04 15:37:53.000000 ft_jwt-0.0.8/README.md
-drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 15:38:36.000000 ft_jwt-0.0.8/ft_jwt/
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 14:17:44.000000 ft_jwt-0.0.8/ft_jwt/__init__.py
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     3148 2024-04-04 14:17:44.000000 ft_jwt-0.0.8/ft_jwt/ft_jwt.py
-drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 15:38:36.000000 ft_jwt-0.0.8/ft_jwt.egg-info/
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1852 2024-04-04 15:38:35.000000 ft_jwt-0.0.8/ft_jwt.egg-info/PKG-INFO
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)      182 2024-04-04 15:38:35.000000 ft_jwt-0.0.8/ft_jwt.egg-info/SOURCES.txt
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        1 2024-04-04 15:38:35.000000 ft_jwt-0.0.8/ft_jwt.egg-info/dependency_links.txt
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        7 2024-04-04 15:38:35.000000 ft_jwt-0.0.8/ft_jwt.egg-info/top_level.txt
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)       38 2024-04-04 15:38:36.000000 ft_jwt-0.0.8/setup.cfg
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)      723 2024-04-04 15:38:05.000000 ft_jwt-0.0.8/setup.py
+drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 15:40:22.000000 ft_jwt-0.0.9/
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1063 2024-04-04 14:17:44.000000 ft_jwt-0.0.9/LICENSE
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1853 2024-04-04 15:40:22.000000 ft_jwt-0.0.9/PKG-INFO
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1286 2024-04-04 15:37:53.000000 ft_jwt-0.0.9/README.md
+drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 15:40:22.000000 ft_jwt-0.0.9/ft_jwt/
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 14:17:44.000000 ft_jwt-0.0.9/ft_jwt/__init__.py
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     3148 2024-04-04 14:17:44.000000 ft_jwt-0.0.9/ft_jwt/ft_jwt.py
+drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 15:40:22.000000 ft_jwt-0.0.9/ft_jwt.egg-info/
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1853 2024-04-04 15:40:22.000000 ft_jwt-0.0.9/ft_jwt.egg-info/PKG-INFO
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)      182 2024-04-04 15:40:22.000000 ft_jwt-0.0.9/ft_jwt.egg-info/SOURCES.txt
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        1 2024-04-04 15:40:22.000000 ft_jwt-0.0.9/ft_jwt.egg-info/dependency_links.txt
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        7 2024-04-04 15:40:22.000000 ft_jwt-0.0.9/ft_jwt.egg-info/top_level.txt
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)       38 2024-04-04 15:40:22.000000 ft_jwt-0.0.9/setup.cfg
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)      724 2024-04-04 15:40:17.000000 ft_jwt-0.0.9/setup.py
```

### Comparing `ft_jwt-0.0.8/LICENSE` & `ft_jwt-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ft_jwt-0.0.8/PKG-INFO` & `ft_jwt-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ft_jwt
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.
-Home-page: https://github.com/minthe/ft_transcendence/blob/jwt/auth/ft_jwt/ft_jwt/ft_jwt.py
+Home-page: https://github.com/minthe/ft_transcendence/blob/main/auth/ft_jwt/ft_jwt/ft_jwt.py
 Author: vfuhlenb
 Author-email: minh.tee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `ft_jwt-0.0.8/README.md` & `ft_jwt-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ft_jwt-0.0.8/ft_jwt/ft_jwt.py` & `ft_jwt-0.0.9/ft_jwt/ft_jwt.py`

 * *Files identical despite different names*

### Comparing `ft_jwt-0.0.8/ft_jwt.egg-info/PKG-INFO` & `ft_jwt-0.0.9/ft_jwt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ft-jwt
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.
-Home-page: https://github.com/minthe/ft_transcendence/blob/jwt/auth/ft_jwt/ft_jwt/ft_jwt.py
+Home-page: https://github.com/minthe/ft_transcendence/blob/main/auth/ft_jwt/ft_jwt/ft_jwt.py
 Author: vfuhlenb
 Author-email: minh.tee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `ft_jwt-0.0.8/setup.py` & `ft_jwt-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="ft_jwt",
-	version="0.0.8",
+	version="0.0.9",
 	author="vfuhlenb",
 	author_email="minh.tee@gmail.com",
 	description="A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
-	url="https://github.com/minthe/ft_transcendence/blob/jwt/auth/ft_jwt/ft_jwt/ft_jwt.py",
+	url="https://github.com/minthe/ft_transcendence/blob/main/auth/ft_jwt/ft_jwt/ft_jwt.py",
 	packages=setuptools.find_packages(),
 	classifiers=[
 		"Programming Language :: Python :: 3",
 		"License :: OSI Approved :: MIT License",
 		"Operating System :: OS Independent",
 	],
 	python_requires='>=3.6',
```

