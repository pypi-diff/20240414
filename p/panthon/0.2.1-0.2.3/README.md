# Comparing `tmp/panthon-0.2.1.tar.gz` & `tmp/panthon-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panthon-0.2.1.tar", last modified: Sun Apr 14 20:25:18 2024, max compression
+gzip compressed data, was "panthon-0.2.3.tar", last modified: Sun Apr 14 20:27:29 2024, max compression
```

## Comparing `panthon-0.2.1.tar` & `panthon-0.2.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:25:18.246863 panthon-0.2.1/
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1072 2023-07-23 10:41:07.000000 panthon-0.2.1/LICENSE
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1696 2024-04-14 20:25:18.246634 panthon-0.2.1/PKG-INFO
--rw-r--r--   0 nripeshniketan   (501) staff       (20)      951 2023-08-09 17:19:06.000000 panthon-0.2.1/README.md
-drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:25:18.243982 panthon-0.2.1/panthon/
-drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:25:18.244816 panthon-0.2.1/panthon/SQL/
--rw-r--r--   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:24:59.000000 panthon-0.2.1/panthon/SQL/__init__.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)    11634 2024-04-13 09:37:29.000000 panthon-0.2.1/panthon/SQL/dsss.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)      349 2024-04-14 20:04:34.000000 panthon-0.2.1/panthon/__init__.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1444 2024-04-14 19:34:55.000000 panthon-0.2.1/panthon/arp_spoofing.py
-drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:25:18.244944 panthon-0.2.1/panthon/data/
--rw-r--r--   0 nripeshniketan   (501) staff       (20)   110530 2023-09-16 19:07:13.000000 panthon-0.2.1/panthon/data/useragents.txt
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1899 2024-04-14 19:15:41.000000 panthon-0.2.1/panthon/ddos_attack.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1576 2024-04-13 09:37:29.000000 panthon-0.2.1/panthon/dns_spoofer.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     5269 2024-04-14 19:34:55.000000 panthon-0.2.1/panthon/dos_attack.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     2670 2024-04-14 19:15:41.000000 panthon-0.2.1/panthon/mitm_attack.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1644 2024-04-14 19:46:37.000000 panthon-0.2.1/panthon/network_spoofer.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     2499 2024-04-14 19:34:55.000000 panthon-0.2.1/panthon/sql_injection.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     2573 2024-04-14 20:03:26.000000 panthon-0.2.1/panthon/website_extractor.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     2689 2024-04-14 19:34:55.000000 panthon-0.2.1/panthon/xss_attack.py
-drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:25:18.246358 panthon-0.2.1/panthon.egg-info/
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1696 2024-04-14 20:25:18.000000 panthon-0.2.1/panthon.egg-info/PKG-INFO
--rw-r--r--   0 nripeshniketan   (501) staff       (20)      554 2024-04-14 20:25:18.000000 panthon-0.2.1/panthon.egg-info/SOURCES.txt
--rw-r--r--   0 nripeshniketan   (501) staff       (20)        1 2024-04-14 20:25:18.000000 panthon-0.2.1/panthon.egg-info/dependency_links.txt
--rw-r--r--   0 nripeshniketan   (501) staff       (20)       52 2024-04-14 20:25:18.000000 panthon-0.2.1/panthon.egg-info/requires.txt
--rw-r--r--   0 nripeshniketan   (501) staff       (20)        8 2024-04-14 20:25:18.000000 panthon-0.2.1/panthon.egg-info/top_level.txt
--rw-r--r--   0 nripeshniketan   (501) staff       (20)      103 2023-10-19 15:01:46.000000 panthon-0.2.1/pyproject.toml
--rw-r--r--   0 nripeshniketan   (501) staff       (20)       38 2024-04-14 20:25:18.246907 panthon-0.2.1/setup.cfg
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1189 2024-04-14 20:25:13.000000 panthon-0.2.1/setup.py
-drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:25:18.246049 panthon-0.2.1/test/
--rw-r--r--   0 nripeshniketan   (501) staff       (20)      448 2023-08-20 08:38:11.000000 panthon-0.2.1/test/test_ddos_attack.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1789 2023-08-20 08:38:11.000000 panthon-0.2.1/test/test_dos_attack.py
+drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:27:29.069492 panthon-0.2.3/
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1072 2023-07-23 10:41:07.000000 panthon-0.2.3/LICENSE
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1696 2024-04-14 20:27:29.069292 panthon-0.2.3/PKG-INFO
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)      951 2023-08-09 17:19:06.000000 panthon-0.2.3/README.md
+drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:27:29.066916 panthon-0.2.3/panthon/
+drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:27:29.067673 panthon-0.2.3/panthon/SQL/
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:24:59.000000 panthon-0.2.3/panthon/SQL/__init__.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     8635 2024-04-14 20:26:15.000000 panthon-0.2.3/panthon/SQL/dsss.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)      349 2024-04-14 20:27:07.000000 panthon-0.2.3/panthon/__init__.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1444 2024-04-14 19:34:55.000000 panthon-0.2.3/panthon/arp_spoofing.py
+drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:27:29.067832 panthon-0.2.3/panthon/data/
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)   110530 2023-09-16 19:07:13.000000 panthon-0.2.3/panthon/data/useragents.txt
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1899 2024-04-14 19:15:41.000000 panthon-0.2.3/panthon/ddos_attack.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1576 2024-04-13 09:37:29.000000 panthon-0.2.3/panthon/dns_spoofer.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     5269 2024-04-14 19:34:55.000000 panthon-0.2.3/panthon/dos_attack.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     2670 2024-04-14 19:15:41.000000 panthon-0.2.3/panthon/mitm_attack.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1644 2024-04-14 19:46:37.000000 panthon-0.2.3/panthon/network_spoofer.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     2986 2024-04-14 20:26:15.000000 panthon-0.2.3/panthon/sql_injection.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     2573 2024-04-14 20:03:26.000000 panthon-0.2.3/panthon/website_extractor.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     2689 2024-04-14 19:34:55.000000 panthon-0.2.3/panthon/xss_attack.py
+drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:27:29.069072 panthon-0.2.3/panthon.egg-info/
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1696 2024-04-14 20:27:29.000000 panthon-0.2.3/panthon.egg-info/PKG-INFO
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)      554 2024-04-14 20:27:29.000000 panthon-0.2.3/panthon.egg-info/SOURCES.txt
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)        1 2024-04-14 20:27:29.000000 panthon-0.2.3/panthon.egg-info/dependency_links.txt
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)       52 2024-04-14 20:27:29.000000 panthon-0.2.3/panthon.egg-info/requires.txt
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)        8 2024-04-14 20:27:29.000000 panthon-0.2.3/panthon.egg-info/top_level.txt
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)      103 2023-10-19 15:01:46.000000 panthon-0.2.3/pyproject.toml
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)       38 2024-04-14 20:27:29.069529 panthon-0.2.3/setup.cfg
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1189 2024-04-14 20:27:21.000000 panthon-0.2.3/setup.py
+drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2024-04-14 20:27:29.068870 panthon-0.2.3/test/
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)      448 2023-08-20 08:38:11.000000 panthon-0.2.3/test/test_ddos_attack.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1789 2023-08-20 08:38:11.000000 panthon-0.2.3/test/test_dos_attack.py
```

### Comparing `panthon-0.2.1/LICENSE` & `panthon-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `panthon-0.2.1/PKG-INFO` & `panthon-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panthon
-Version: 0.2.1
+Version: 0.2.3
 Summary: Panthon employs sophisticated methods to replicate different cyber threats, offering a dynamic solution to proactively address the constantly shifting realm of cybersecurity risks. Our goal is to help build more resilient and secure systems through a deeper understanding and anticipation of potential vulnerabilities.
 Author: Nripesh
 Author-email: Nripesh14@gmail.com
 License: Apache Software License
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `panthon-0.2.1/README.md` & `panthon-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `panthon-0.2.1/panthon/arp_spoofing.py` & `panthon-0.2.3/panthon/arp_spoofing.py`

 * *Files identical despite different names*

### Comparing `panthon-0.2.1/panthon/data/useragents.txt` & `panthon-0.2.3/panthon/data/useragents.txt`

 * *Files identical despite different names*

### Comparing `panthon-0.2.1/panthon/ddos_attack.py` & `panthon-0.2.3/panthon/ddos_attack.py`

 * *Files identical despite different names*

### Comparing `panthon-0.2.1/panthon/dns_spoofer.py` & `panthon-0.2.3/panthon/dns_spoofer.py`

 * *Files identical despite different names*

### Comparing `panthon-0.2.1/panthon/dos_attack.py` & `panthon-0.2.3/panthon/dos_attack.py`

 * *Files identical despite different names*

### Comparing `panthon-0.2.1/panthon/mitm_attack.py` & `panthon-0.2.3/panthon/mitm_attack.py`

 * *Files identical despite different names*

### Comparing `panthon-0.2.1/panthon/network_spoofer.py` & `panthon-0.2.3/panthon/network_spoofer.py`

 * *Files identical despite different names*

### Comparing `panthon-0.2.1/panthon/sql_injection.py` & `panthon-0.2.3/panthon/sql_injection.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 import subprocess
 import os
-from .SQL.dsss import dsss
 
 
 class SQLInjectionAttack:
     def sqlmap_attack(
         self,
         target_url,
         level=None,
@@ -46,15 +45,15 @@
             "--cookie" if cookies else "",
             str(cookies) if cookies else "",
             "--crawl=2" if crawl else "",
         ]
         print("sqlmap")
         subprocess.run(command)
 
-    def sqli_scanner(
+    def dsss_attack(
         self, target_url, data=None, cookie=None, ua=None, referer=None, proxy=None
     ):
         """Scans the target_url for potential SQL injection vulnerabilities.
 
         Args:
         - target_url (str): The target URL to scan.
         - data (str, optional): POST data to send with the request.
@@ -64,19 +63,35 @@
         - proxy (str, optional): HTTP proxy address.
 
         Returns:
         - bool: True if potential vulnerabilities are found, False otherwise.
         """
 
         # Initialize options for the scanner
-        attack = dsss(proxy=proxy, cookie=cookie, ua=ua, referer=referer)
+     #   attack = dsss(proxy=proxy, cookie=cookie, ua=ua, referer=referer)
 
         # Scan the target URL
-        result = attack.scan_page(target_url, data)
+        #result = attack.scan_page(target_url, data)
+
+        command = [
+            "python3",
+            os.path.join(os.path.dirname(__file__), "SQL/dsss.py"),
+            "-u",
+            target_url,
+            "--cookie" if cookie else "",
+            cookie if cookie else "",
+            "--user-agent" if ua else "",
+            ua if ua else "",
+            "--referer" if referer else "",
+            referer if referer else "",
+            "--proxy" if proxy else "",
+            proxy if proxy else ""
+        ]
+        subprocess.run(command)
 
         # Print the result
-        logging.info(
-            "\nscan results: %s vulnerabilities found"
-            % ("possible" if result else "no")
-        )
-        print("sqli")
-        return result
+#        logging.info(
+ #           "\nscan results: %s vulnerabilities found"
+  #          % ("possible" if result else "no")
+    #    )
+   #     print("sqli")
+     #   return result
```

### Comparing `panthon-0.2.1/panthon/website_extractor.py` & `panthon-0.2.3/panthon/website_extractor.py`

 * *Files identical despite different names*

### Comparing `panthon-0.2.1/panthon/xss_attack.py` & `panthon-0.2.3/panthon/xss_attack.py`

 * *Files identical despite different names*

### Comparing `panthon-0.2.1/panthon.egg-info/PKG-INFO` & `panthon-0.2.3/panthon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panthon
-Version: 0.2.1
+Version: 0.2.3
 Summary: Panthon employs sophisticated methods to replicate different cyber threats, offering a dynamic solution to proactively address the constantly shifting realm of cybersecurity risks. Our goal is to help build more resilient and secure systems through a deeper understanding and anticipation of potential vulnerabilities.
 Author: Nripesh
 Author-email: Nripesh14@gmail.com
 License: Apache Software License
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `panthon-0.2.1/panthon.egg-info/SOURCES.txt` & `panthon-0.2.3/panthon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panthon-0.2.1/setup.py` & `panthon-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 def _strip(line):
     return line.split(" ")[0].split("#")[0].split(",")[0]
 
 setup(
     name="panthon",
-    version="0.2.1",
+    version="0.2.3",
     author="Nripesh",
     author_email="Nripesh14@gmail.com",
     description=(
         "Panthon employs sophisticated methods to replicate different cyber threats,"
         " offering a dynamic solution to proactively address the constantly shifting"
         " realm of cybersecurity risks. Our goal is to help build more resilient and"
         " secure systems through a deeper understanding and anticipation of potential"
```

### Comparing `panthon-0.2.1/test/test_dos_attack.py` & `panthon-0.2.3/test/test_dos_attack.py`

 * *Files identical despite different names*

