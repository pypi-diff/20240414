# Comparing `tmp/panthon-0.2.0.tar.gz` & `tmp/panthon-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panthon-0.2.0.tar", last modified: Sun Apr 14 20:18:32 2024, max compression
+gzip compressed data, was "panthon-0.2.1.tar", last modified: Sun Apr 14 20:25:18 2024, max compression
```

## Comparing `panthon-0.2.0.tar` & `panthon-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:18:32.258679 panthon-0.2.0/
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1072 2023-07-23 10:41:07.000000 panthon-0.2.0/LICENSE
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1696 2024-04-14 20:18:32.258414 panthon-0.2.0/PKG-INFO
--rw-r--r--   0 nripeshniketan   (501) staff       (20)      951 2023-08-09 17:19:06.000000 panthon-0.2.0/README.md
-drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:18:32.255765 panthon-0.2.0/panthon/
--rw-r--r--   0 nripeshniketan   (501) staff       (20)      349 2024-04-14 20:04:34.000000 panthon-0.2.0/panthon/__init__.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1444 2024-04-14 19:34:55.000000 panthon-0.2.0/panthon/arp_spoofing.py
-drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:18:32.256595 panthon-0.2.0/panthon/data/
--rw-r--r--   0 nripeshniketan   (501) staff       (20)   110530 2023-09-16 19:07:13.000000 panthon-0.2.0/panthon/data/useragents.txt
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1899 2024-04-14 19:15:41.000000 panthon-0.2.0/panthon/ddos_attack.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1576 2024-04-13 09:37:29.000000 panthon-0.2.0/panthon/dns_spoofer.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     5269 2024-04-14 19:34:55.000000 panthon-0.2.0/panthon/dos_attack.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     2670 2024-04-14 19:15:41.000000 panthon-0.2.0/panthon/mitm_attack.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1644 2024-04-14 19:46:37.000000 panthon-0.2.0/panthon/network_spoofer.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     2499 2024-04-14 19:34:55.000000 panthon-0.2.0/panthon/sql_injection.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     2573 2024-04-14 20:03:26.000000 panthon-0.2.0/panthon/website_extractor.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     2689 2024-04-14 19:34:55.000000 panthon-0.2.0/panthon/xss_attack.py
-drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:18:32.258085 panthon-0.2.0/panthon.egg-info/
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1696 2024-04-14 20:18:32.000000 panthon-0.2.0/panthon.egg-info/PKG-INFO
--rw-r--r--   0 nripeshniketan   (501) staff       (20)      510 2024-04-14 20:18:32.000000 panthon-0.2.0/panthon.egg-info/SOURCES.txt
--rw-r--r--   0 nripeshniketan   (501) staff       (20)        1 2024-04-14 20:18:32.000000 panthon-0.2.0/panthon.egg-info/dependency_links.txt
--rw-r--r--   0 nripeshniketan   (501) staff       (20)       52 2024-04-14 20:18:32.000000 panthon-0.2.0/panthon.egg-info/requires.txt
--rw-r--r--   0 nripeshniketan   (501) staff       (20)        8 2024-04-14 20:18:32.000000 panthon-0.2.0/panthon.egg-info/top_level.txt
--rw-r--r--   0 nripeshniketan   (501) staff       (20)      103 2023-10-19 15:01:46.000000 panthon-0.2.0/pyproject.toml
--rw-r--r--   0 nripeshniketan   (501) staff       (20)       38 2024-04-14 20:18:32.258726 panthon-0.2.0/setup.cfg
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1189 2024-04-14 20:18:27.000000 panthon-0.2.0/setup.py
-drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:18:32.257723 panthon-0.2.0/test/
--rw-r--r--   0 nripeshniketan   (501) staff       (20)      448 2023-08-20 08:38:11.000000 panthon-0.2.0/test/test_ddos_attack.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1789 2023-08-20 08:38:11.000000 panthon-0.2.0/test/test_dos_attack.py
+drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:25:18.246863 panthon-0.2.1/
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1072 2023-07-23 10:41:07.000000 panthon-0.2.1/LICENSE
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1696 2024-04-14 20:25:18.246634 panthon-0.2.1/PKG-INFO
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)      951 2023-08-09 17:19:06.000000 panthon-0.2.1/README.md
+drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:25:18.243982 panthon-0.2.1/panthon/
+drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:25:18.244816 panthon-0.2.1/panthon/SQL/
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:24:59.000000 panthon-0.2.1/panthon/SQL/__init__.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)    11634 2024-04-13 09:37:29.000000 panthon-0.2.1/panthon/SQL/dsss.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)      349 2024-04-14 20:04:34.000000 panthon-0.2.1/panthon/__init__.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1444 2024-04-14 19:34:55.000000 panthon-0.2.1/panthon/arp_spoofing.py
+drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:25:18.244944 panthon-0.2.1/panthon/data/
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)   110530 2023-09-16 19:07:13.000000 panthon-0.2.1/panthon/data/useragents.txt
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1899 2024-04-14 19:15:41.000000 panthon-0.2.1/panthon/ddos_attack.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1576 2024-04-13 09:37:29.000000 panthon-0.2.1/panthon/dns_spoofer.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     5269 2024-04-14 19:34:55.000000 panthon-0.2.1/panthon/dos_attack.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     2670 2024-04-14 19:15:41.000000 panthon-0.2.1/panthon/mitm_attack.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1644 2024-04-14 19:46:37.000000 panthon-0.2.1/panthon/network_spoofer.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     2499 2024-04-14 19:34:55.000000 panthon-0.2.1/panthon/sql_injection.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     2573 2024-04-14 20:03:26.000000 panthon-0.2.1/panthon/website_extractor.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     2689 2024-04-14 19:34:55.000000 panthon-0.2.1/panthon/xss_attack.py
+drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:25:18.246358 panthon-0.2.1/panthon.egg-info/
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1696 2024-04-14 20:25:18.000000 panthon-0.2.1/panthon.egg-info/PKG-INFO
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)      554 2024-04-14 20:25:18.000000 panthon-0.2.1/panthon.egg-info/SOURCES.txt
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)        1 2024-04-14 20:25:18.000000 panthon-0.2.1/panthon.egg-info/dependency_links.txt
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)       52 2024-04-14 20:25:18.000000 panthon-0.2.1/panthon.egg-info/requires.txt
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)        8 2024-04-14 20:25:18.000000 panthon-0.2.1/panthon.egg-info/top_level.txt
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)      103 2023-10-19 15:01:46.000000 panthon-0.2.1/pyproject.toml
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)       38 2024-04-14 20:25:18.246907 panthon-0.2.1/setup.cfg
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1189 2024-04-14 20:25:13.000000 panthon-0.2.1/setup.py
+drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:25:18.246049 panthon-0.2.1/test/
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)      448 2023-08-20 08:38:11.000000 panthon-0.2.1/test/test_ddos_attack.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1789 2023-08-20 08:38:11.000000 panthon-0.2.1/test/test_dos_attack.py
```

### Comparing `panthon-0.2.0/LICENSE` & `panthon-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `panthon-0.2.0/PKG-INFO` & `panthon-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panthon
-Version: 0.2.0
+Version: 0.2.1
 Summary: Panthon employs sophisticated methods to replicate different cyber threats, offering a dynamic solution to proactively address the constantly shifting realm of cybersecurity risks. Our goal is to help build more resilient and secure systems through a deeper understanding and anticipation of potential vulnerabilities.
 Author: Nripesh
 Author-email: Nripesh14@gmail.com
 License: Apache Software License
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `panthon-0.2.0/README.md` & `panthon-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `panthon-0.2.0/panthon/arp_spoofing.py` & `panthon-0.2.1/panthon/arp_spoofing.py`

 * *Files identical despite different names*

### Comparing `panthon-0.2.0/panthon/data/useragents.txt` & `panthon-0.2.1/panthon/data/useragents.txt`

 * *Files identical despite different names*

### Comparing `panthon-0.2.0/panthon/ddos_attack.py` & `panthon-0.2.1/panthon/ddos_attack.py`

 * *Files identical despite different names*

### Comparing `panthon-0.2.0/panthon/dns_spoofer.py` & `panthon-0.2.1/panthon/dns_spoofer.py`

 * *Files identical despite different names*

### Comparing `panthon-0.2.0/panthon/dos_attack.py` & `panthon-0.2.1/panthon/dos_attack.py`

 * *Files identical despite different names*

### Comparing `panthon-0.2.0/panthon/mitm_attack.py` & `panthon-0.2.1/panthon/mitm_attack.py`

 * *Files identical despite different names*

### Comparing `panthon-0.2.0/panthon/network_spoofer.py` & `panthon-0.2.1/panthon/network_spoofer.py`

 * *Files identical despite different names*

### Comparing `panthon-0.2.0/panthon/sql_injection.py` & `panthon-0.2.1/panthon/sql_injection.py`

 * *Files identical despite different names*

### Comparing `panthon-0.2.0/panthon/website_extractor.py` & `panthon-0.2.1/panthon/website_extractor.py`

 * *Files identical despite different names*

### Comparing `panthon-0.2.0/panthon/xss_attack.py` & `panthon-0.2.1/panthon/xss_attack.py`

 * *Files identical despite different names*

### Comparing `panthon-0.2.0/panthon.egg-info/PKG-INFO` & `panthon-0.2.1/panthon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panthon
-Version: 0.2.0
+Version: 0.2.1
 Summary: Panthon employs sophisticated methods to replicate different cyber threats, offering a dynamic solution to proactively address the constantly shifting realm of cybersecurity risks. Our goal is to help build more resilient and secure systems through a deeper understanding and anticipation of potential vulnerabilities.
 Author: Nripesh
 Author-email: Nripesh14@gmail.com
 License: Apache Software License
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `panthon-0.2.0/setup.py` & `panthon-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 def _strip(line):
     return line.split(" ")[0].split("#")[0].split(",")[0]
 
 setup(
     name="panthon",
-    version="0.2.0",
+    version="0.2.1",
     author="Nripesh",
     author_email="Nripesh14@gmail.com",
     description=(
         "Panthon employs sophisticated methods to replicate different cyber threats,"
         " offering a dynamic solution to proactively address the constantly shifting"
         " realm of cybersecurity risks. Our goal is to help build more resilient and"
         " secure systems through a deeper understanding and anticipation of potential"
```

### Comparing `panthon-0.2.0/test/test_dos_attack.py` & `panthon-0.2.1/test/test_dos_attack.py`

 * *Files identical despite different names*

