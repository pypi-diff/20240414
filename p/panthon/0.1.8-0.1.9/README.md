# Comparing `tmp/panthon-0.1.8.tar.gz` & `tmp/panthon-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panthon-0.1.8.tar", last modified: Thu Aug 10 09:02:17 2023, max compression
+gzip compressed data, was "panthon-0.1.9.tar", last modified: Thu Aug 10 09:10:25 2023, max compression
```

## Comparing `panthon-0.1.8.tar` & `panthon-0.1.9.tar`

### file list

```diff
@@ -1,28 +1,23 @@
-drwxr-xr-x   0 anni      (1000) anni      (1000)        0 2023-08-10 09:02:17.339138 panthon-0.1.8/
--rw-r--r--   0 anni      (1000) anni      (1000)     1072 2023-08-08 10:32:56.000000 panthon-0.1.8/LICENSE
--rw-r--r--   0 anni      (1000) anni      (1000)      700 2023-08-10 09:02:17.339138 panthon-0.1.8/PKG-INFO
--rw-r--r--   0 anni      (1000) anni      (1000)      951 2023-08-09 09:04:19.000000 panthon-0.1.8/README.md
-drwxr-xr-x   0 anni      (1000) anni      (1000)        0 2023-08-10 09:02:17.339138 panthon-0.1.8/panthon.egg-info/
--rw-r--r--   0 anni      (1000) anni      (1000)      700 2023-08-10 09:02:17.000000 panthon-0.1.8/panthon.egg-info/PKG-INFO
--rw-r--r--   0 anni      (1000) anni      (1000)      458 2023-08-10 09:02:17.000000 panthon-0.1.8/panthon.egg-info/SOURCES.txt
--rw-r--r--   0 anni      (1000) anni      (1000)        1 2023-08-10 09:02:17.000000 panthon-0.1.8/panthon.egg-info/dependency_links.txt
--rw-r--r--   0 anni      (1000) anni      (1000)       50 2023-08-10 09:02:17.000000 panthon-0.1.8/panthon.egg-info/requires.txt
--rw-r--r--   0 anni      (1000) anni      (1000)        4 2023-08-10 09:02:17.000000 panthon-0.1.8/panthon.egg-info/top_level.txt
--rw-r--r--   0 anni      (1000) anni      (1000)      103 2023-08-08 10:32:56.000000 panthon-0.1.8/pyproject.toml
--rw-r--r--   0 anni      (1000) anni      (1000)       79 2023-08-10 09:02:17.339138 panthon-0.1.8/setup.cfg
--rw-r--r--   0 anni      (1000) anni      (1000)     1169 2023-08-10 09:01:17.000000 panthon-0.1.8/setup.py
-drwxr-xr-x   0 anni      (1000) anni      (1000)        0 2023-08-10 09:02:17.339138 panthon-0.1.8/src/
--rw-r--r--   0 anni      (1000) anni      (1000)      277 2023-08-10 09:01:02.000000 panthon-0.1.8/src/__init__.py
--rw-r--r--   0 anni      (1000) anni      (1000)     1412 2023-08-08 10:32:56.000000 panthon-0.1.8/src/arp_spoofing.py
--rw-r--r--   0 anni      (1000) anni      (1000)     2276 2023-08-08 10:32:56.000000 panthon-0.1.8/src/ddos_attack.py
--rw-r--r--   0 anni      (1000) anni      (1000)     1926 2023-08-08 10:32:56.000000 panthon-0.1.8/src/dns_spoofer.py
-drwxr-xr-x   0 anni      (1000) anni      (1000)        0 2023-08-10 09:02:17.339138 panthon-0.1.8/src/dos/
--rw-r--r--   0 anni      (1000) anni      (1000)       33 2023-08-10 08:49:14.000000 panthon-0.1.8/src/dos/__init__.py
--rw-r--r--   0 anni      (1000) anni      (1000)     5190 2023-08-09 18:38:40.000000 panthon-0.1.8/src/dos/dos_attack.py
--rw-r--r--   0 anni      (1000) anni      (1000)    19740 2023-08-08 10:32:56.000000 panthon-0.1.8/src/dos/goldeneye.py
--rw-r--r--   0 anni      (1000) anni      (1000)    10515 2023-08-09 18:38:40.000000 panthon-0.1.8/src/dsss.py
--rw-r--r--   0 anni      (1000) anni      (1000)     2217 2023-08-08 10:32:56.000000 panthon-0.1.8/src/mitm_attack.py
--rw-r--r--   0 anni      (1000) anni      (1000)      380 2023-08-09 09:33:15.000000 panthon-0.1.8/src/random_string_generator.py
--rw-r--r--   0 anni      (1000) anni      (1000)   273202 2023-08-08 10:32:56.000000 panthon-0.1.8/src/saphyra.py
--rw-r--r--   0 anni      (1000) anni      (1000)     2392 2023-08-09 18:38:40.000000 panthon-0.1.8/src/sql_injection.py
--rw-r--r--   0 anni      (1000) anni      (1000)     1966 2023-08-08 10:32:56.000000 panthon-0.1.8/src/xss_attack.py
+drwxr-xr-x   0 anni      (1000) anni      (1000)        0 2023-08-10 09:10:25.965719 panthon-0.1.9/
+-rw-r--r--   0 anni      (1000) anni      (1000)     1072 2023-08-08 10:32:56.000000 panthon-0.1.9/LICENSE
+-rw-r--r--   0 anni      (1000) anni      (1000)      700 2023-08-10 09:10:25.965719 panthon-0.1.9/PKG-INFO
+-rw-r--r--   0 anni      (1000) anni      (1000)      951 2023-08-09 09:04:19.000000 panthon-0.1.9/README.md
+drwxr-xr-x   0 anni      (1000) anni      (1000)        0 2023-08-10 09:10:25.965719 panthon-0.1.9/panthon.egg-info/
+-rw-r--r--   0 anni      (1000) anni      (1000)      700 2023-08-10 09:10:25.000000 panthon-0.1.9/panthon.egg-info/PKG-INFO
+-rw-r--r--   0 anni      (1000) anni      (1000)      379 2023-08-10 09:10:25.000000 panthon-0.1.9/panthon.egg-info/SOURCES.txt
+-rw-r--r--   0 anni      (1000) anni      (1000)        1 2023-08-10 09:10:25.000000 panthon-0.1.9/panthon.egg-info/dependency_links.txt
+-rw-r--r--   0 anni      (1000) anni      (1000)       50 2023-08-10 09:10:25.000000 panthon-0.1.9/panthon.egg-info/requires.txt
+-rw-r--r--   0 anni      (1000) anni      (1000)        1 2023-08-10 09:10:25.000000 panthon-0.1.9/panthon.egg-info/top_level.txt
+-rw-r--r--   0 anni      (1000) anni      (1000)      103 2023-08-08 10:32:56.000000 panthon-0.1.9/pyproject.toml
+-rw-r--r--   0 anni      (1000) anni      (1000)       79 2023-08-10 09:10:25.965719 panthon-0.1.9/setup.cfg
+-rw-r--r--   0 anni      (1000) anni      (1000)     1169 2023-08-10 09:10:20.000000 panthon-0.1.9/setup.py
+drwxr-xr-x   0 anni      (1000) anni      (1000)        0 2023-08-10 09:10:25.965719 panthon-0.1.9/src/
+-rw-r--r--   0 anni      (1000) anni      (1000)     1412 2023-08-08 10:32:56.000000 panthon-0.1.9/src/arp_spoofing.py
+-rw-r--r--   0 anni      (1000) anni      (1000)     2276 2023-08-08 10:32:56.000000 panthon-0.1.9/src/ddos_attack.py
+-rw-r--r--   0 anni      (1000) anni      (1000)     1926 2023-08-08 10:32:56.000000 panthon-0.1.9/src/dns_spoofer.py
+-rw-r--r--   0 anni      (1000) anni      (1000)    10515 2023-08-09 18:38:40.000000 panthon-0.1.9/src/dsss.py
+-rw-r--r--   0 anni      (1000) anni      (1000)     2217 2023-08-08 10:32:56.000000 panthon-0.1.9/src/mitm_attack.py
+-rw-r--r--   0 anni      (1000) anni      (1000)      380 2023-08-09 09:33:15.000000 panthon-0.1.9/src/random_string_generator.py
+-rw-r--r--   0 anni      (1000) anni      (1000)   273202 2023-08-08 10:32:56.000000 panthon-0.1.9/src/saphyra.py
+-rw-r--r--   0 anni      (1000) anni      (1000)     2392 2023-08-09 18:38:40.000000 panthon-0.1.9/src/sql_injection.py
+-rw-r--r--   0 anni      (1000) anni      (1000)     1966 2023-08-08 10:32:56.000000 panthon-0.1.9/src/xss_attack.py
```

### Comparing `panthon-0.1.8/LICENSE` & `panthon-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `panthon-0.1.8/PKG-INFO` & `panthon-0.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panthon
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Machine Learning-powered Cybersecurity Attack Simulation Library
 Home-page: https://github.com/nripeshn/panthon
 Author: Nripesh Niketan
 Author-email: nripesh14@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `panthon-0.1.8/README.md` & `panthon-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `panthon-0.1.8/panthon.egg-info/PKG-INFO` & `panthon-0.1.9/panthon.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panthon
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Machine Learning-powered Cybersecurity Attack Simulation Library
 Home-page: https://github.com/nripeshn/panthon
 Author: Nripesh Niketan
 Author-email: nripesh14@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `panthon-0.1.8/setup.py` & `panthon-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # with open("~/panthon/requirements.txt", "r", encoding="utf-8") as f:
 #     requirements = f.read().splitlines()
 
 requirements = ["torch", "scapy", "netifaces", "bs4", "tld", "fuzzywuzzy", "requests"]
 
 setup(
     name="panthon",
-    version="0.1.8",
+    version="0.1.9",
     url="https://github.com/nripeshn/panthon",
     author="Nripesh Niketan",
     author_email="nripesh14@gmail.com",
     description="A Machine Learning-powered Cybersecurity Attack Simulation Library",
     packages=find_packages(),
     install_requires=requirements,
     classifiers=[
```

### Comparing `panthon-0.1.8/src/arp_spoofing.py` & `panthon-0.1.9/src/arp_spoofing.py`

 * *Files identical despite different names*

### Comparing `panthon-0.1.8/src/ddos_attack.py` & `panthon-0.1.9/src/ddos_attack.py`

 * *Files identical despite different names*

### Comparing `panthon-0.1.8/src/dns_spoofer.py` & `panthon-0.1.9/src/dns_spoofer.py`

 * *Files identical despite different names*

### Comparing `panthon-0.1.8/src/dsss.py` & `panthon-0.1.9/src/dsss.py`

 * *Files identical despite different names*

### Comparing `panthon-0.1.8/src/mitm_attack.py` & `panthon-0.1.9/src/mitm_attack.py`

 * *Files identical despite different names*

### Comparing `panthon-0.1.8/src/saphyra.py` & `panthon-0.1.9/src/saphyra.py`

 * *Files identical despite different names*

### Comparing `panthon-0.1.8/src/sql_injection.py` & `panthon-0.1.9/src/sql_injection.py`

 * *Files identical despite different names*

### Comparing `panthon-0.1.8/src/xss_attack.py` & `panthon-0.1.9/src/xss_attack.py`

 * *Files identical despite different names*

