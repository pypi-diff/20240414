# Comparing `tmp/matchmeta-2023.5.30.tar.gz` & `tmp/matchmeta-2024.4.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matchmeta-2023.5.30.tar", last modified: Wed May 31 00:29:35 2023, max compression
+gzip compressed data, was "matchmeta-2024.4.14.tar", last modified: Sun Apr 14 13:24:27 2024, max compression
```

## Comparing `matchmeta-2023.5.30.tar` & `matchmeta-2024.4.14.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:29:35.569254 matchmeta-2023.5.30/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 00:29:24.000000 matchmeta-2023.5.30/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-31 00:29:35.569254 matchmeta-2023.5.30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-31 00:29:24.000000 matchmeta-2023.5.30/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:29:35.565253 matchmeta-2023.5.30/matchmeta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-31 00:29:35.000000 matchmeta-2023.5.30/matchmeta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-31 00:29:35.000000 matchmeta-2023.5.30/matchmeta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 00:29:35.000000 matchmeta-2023.5.30/matchmeta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-31 00:29:35.000000 matchmeta-2023.5.30/matchmeta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-31 00:29:35.000000 matchmeta-2023.5.30/matchmeta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-31 00:29:35.000000 matchmeta-2023.5.30/matchmeta.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:29:35.565253 matchmeta-2023.5.30/mmi/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-31 00:29:24.000000 matchmeta-2023.5.30/mmi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-31 00:29:24.000000 matchmeta-2023.5.30/mmi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10432 2023-05-31 00:29:24.000000 matchmeta-2023.5.30/mmi/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 00:29:35.569254 matchmeta-2023.5.30/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-31 00:29:24.000000 matchmeta-2023.5.30/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:24:27.478940 matchmeta-2024.4.14/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-14 13:24:23.000000 matchmeta-2024.4.14/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-14 13:24:27.478940 matchmeta-2024.4.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-04-14 13:24:23.000000 matchmeta-2024.4.14/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:24:27.478940 matchmeta-2024.4.14/matchmeta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-14 13:24:27.000000 matchmeta-2024.4.14/matchmeta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-14 13:24:27.000000 matchmeta-2024.4.14/matchmeta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 13:24:27.000000 matchmeta-2024.4.14/matchmeta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-14 13:24:27.000000 matchmeta-2024.4.14/matchmeta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-14 13:24:27.000000 matchmeta-2024.4.14/matchmeta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-14 13:24:27.000000 matchmeta-2024.4.14/matchmeta.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:24:27.478940 matchmeta-2024.4.14/mmi/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-14 13:24:23.000000 matchmeta-2024.4.14/mmi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-14 13:24:23.000000 matchmeta-2024.4.14/mmi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10540 2024-04-14 13:24:23.000000 matchmeta-2024.4.14/mmi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 13:24:27.478940 matchmeta-2024.4.14/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-14 13:24:23.000000 matchmeta-2024.4.14/setup.py
```

### Comparing `matchmeta-2023.5.30/LICENSE` & `matchmeta-2024.4.14/LICENSE`

 * *Files identical despite different names*

### Comparing `matchmeta-2023.5.30/PKG-INFO` & `matchmeta-2024.4.14/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: matchmeta
-Version: 2023.5.30
+Version: 2024.4.14
 Summary: OS Triage for Anyone and Everyone
 Home-page: https://github.com/jblukach/mmi
 Author: John Lukach
 Author-email: hello@lukach.io
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pybloomfiltermmap3
+Requires-Dist: requests
 
 # mmi
 
 Metadata is the lowest-value indicator as easy to circumvent. Still, with the exponential volume of directories and files standard on default operating system installations, finding things hiding in plain sight has become an important analysis technique.
 
 ```
 MMI - OS Triage for Anyone and Everyone
@@ -27,53 +29,57 @@
 
 ### DATASET
 
 GetBlocks generates the dataset using the SHA256 format for directories, files, hashes, and paths.
 
 https://github.com/4n6ir/getblocks
 
-A pipeline runs every hour to determine if AWS has released any new verified Amazon Machine Image (AMI) to harvest artifacts with the current coverage available.
-
-https://static.matchmeta.info/amazonami.json
+A pipeline runs every hour to determine if AWS has released any new verified Amazon Machine Image (AMI) to harvest artifacts.
 
 ### DISTRIBUTION
 
 A download option in the command line interface (CLI) stores the bloom filters in the user's home directory.
 
 ```
 mmi -d
 ```
 
 Please use these links to download the bloom filters for offline analysis.
 
-https://static.matchmeta.info/gtfo.bloom
+https://dl.4n6ir.com/match-meta-info/gtfo.bloom
 
-https://static.matchmeta.info/mmi.bloom
+https://dl.4n6ir.com/match-meta-info/mmi.bloom
 
 You can verify the integrity of the bloom filters by using the provided SHA256 hash values.
 
-https://static.matchmeta.info/gtfo.sha256
+https://dl.4n6ir.com/match-meta-info/gtfo.sha256
 
-https://static.matchmeta.info/mmi.sha256
+https://dl.4n6ir.com/match-meta-info/mmi.sha256
 
-It is available for download if you're interested in the raw data using API keys available through self-registration.
+Raw data is available for download if you want to use the artifacts elsewhere.
 
-https://store.lukach.io/l/sha256
+https://dl.4n6ir.com/?p=amazon-linux-pipeline/
 
 ### LAST UPDATED
 
 Check when the bloom filters were last updated using the command line interface (CLI).
 
 ```
 mmi -u
 ```
 
 Or by hitting the provided website for the last updated timestamp.
 
-https://static.matchmeta.info/mmi.updated
+https://dl.4n6ir.com/match-meta-info/last.updated
+
+### COUNTS
+
+https://dl.4n6ir.com/match-meta-info/gtfo.count
+
+https://dl.4n6ir.com/match-meta-info/mmi.count
 
 ### DETECTIONS
 
 :purple_square: Empty File (purple) 
 
 A zero byte size determines empty files or the following hash value for this detection.
 
@@ -128,7 +134,9 @@
 ```
 
 ### DEVELOPMENT
 
 ```
 python setup.py install --user
 ```
+
+![Match Meta Inforamtion (MMI)](images/mmi.png)
```

### Comparing `matchmeta-2023.5.30/README.md` & `matchmeta-2024.4.14/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -15,53 +15,57 @@
 
 ### DATASET
 
 GetBlocks generates the dataset using the SHA256 format for directories, files, hashes, and paths.
 
 https://github.com/4n6ir/getblocks
 
-A pipeline runs every hour to determine if AWS has released any new verified Amazon Machine Image (AMI) to harvest artifacts with the current coverage available.
-
-https://static.matchmeta.info/amazonami.json
+A pipeline runs every hour to determine if AWS has released any new verified Amazon Machine Image (AMI) to harvest artifacts.
 
 ### DISTRIBUTION
 
 A download option in the command line interface (CLI) stores the bloom filters in the user's home directory.
 
 ```
 mmi -d
 ```
 
 Please use these links to download the bloom filters for offline analysis.
 
-https://static.matchmeta.info/gtfo.bloom
+https://dl.4n6ir.com/match-meta-info/gtfo.bloom
 
-https://static.matchmeta.info/mmi.bloom
+https://dl.4n6ir.com/match-meta-info/mmi.bloom
 
 You can verify the integrity of the bloom filters by using the provided SHA256 hash values.
 
-https://static.matchmeta.info/gtfo.sha256
+https://dl.4n6ir.com/match-meta-info/gtfo.sha256
 
-https://static.matchmeta.info/mmi.sha256
+https://dl.4n6ir.com/match-meta-info/mmi.sha256
 
-It is available for download if you're interested in the raw data using API keys available through self-registration.
+Raw data is available for download if you want to use the artifacts elsewhere.
 
-https://store.lukach.io/l/sha256
+https://dl.4n6ir.com/?p=amazon-linux-pipeline/
 
 ### LAST UPDATED
 
 Check when the bloom filters were last updated using the command line interface (CLI).
 
 ```
 mmi -u
 ```
 
 Or by hitting the provided website for the last updated timestamp.
 
-https://static.matchmeta.info/mmi.updated
+https://dl.4n6ir.com/match-meta-info/last.updated
+
+### COUNTS
+
+https://dl.4n6ir.com/match-meta-info/gtfo.count
+
+https://dl.4n6ir.com/match-meta-info/mmi.count
 
 ### DETECTIONS
 
 :purple_square: Empty File (purple) 
 
 A zero byte size determines empty files or the following hash value for this detection.
 
@@ -115,8 +119,10 @@
 pip install matchmeta
 ```
 
 ### DEVELOPMENT
 
 ```
 python setup.py install --user
-```
+```
+
+![Match Meta Inforamtion (MMI)](images/mmi.png)
```

### Comparing `matchmeta-2023.5.30/matchmeta.egg-info/PKG-INFO` & `matchmeta-2024.4.14/matchmeta.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: matchmeta
-Version: 2023.5.30
+Version: 2024.4.14
 Summary: OS Triage for Anyone and Everyone
 Home-page: https://github.com/jblukach/mmi
 Author: John Lukach
 Author-email: hello@lukach.io
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pybloomfiltermmap3
+Requires-Dist: requests
 
 # mmi
 
 Metadata is the lowest-value indicator as easy to circumvent. Still, with the exponential volume of directories and files standard on default operating system installations, finding things hiding in plain sight has become an important analysis technique.
 
 ```
 MMI - OS Triage for Anyone and Everyone
@@ -27,53 +29,57 @@
 
 ### DATASET
 
 GetBlocks generates the dataset using the SHA256 format for directories, files, hashes, and paths.
 
 https://github.com/4n6ir/getblocks
 
-A pipeline runs every hour to determine if AWS has released any new verified Amazon Machine Image (AMI) to harvest artifacts with the current coverage available.
-
-https://static.matchmeta.info/amazonami.json
+A pipeline runs every hour to determine if AWS has released any new verified Amazon Machine Image (AMI) to harvest artifacts.
 
 ### DISTRIBUTION
 
 A download option in the command line interface (CLI) stores the bloom filters in the user's home directory.
 
 ```
 mmi -d
 ```
 
 Please use these links to download the bloom filters for offline analysis.
 
-https://static.matchmeta.info/gtfo.bloom
+https://dl.4n6ir.com/match-meta-info/gtfo.bloom
 
-https://static.matchmeta.info/mmi.bloom
+https://dl.4n6ir.com/match-meta-info/mmi.bloom
 
 You can verify the integrity of the bloom filters by using the provided SHA256 hash values.
 
-https://static.matchmeta.info/gtfo.sha256
+https://dl.4n6ir.com/match-meta-info/gtfo.sha256
 
-https://static.matchmeta.info/mmi.sha256
+https://dl.4n6ir.com/match-meta-info/mmi.sha256
 
-It is available for download if you're interested in the raw data using API keys available through self-registration.
+Raw data is available for download if you want to use the artifacts elsewhere.
 
-https://store.lukach.io/l/sha256
+https://dl.4n6ir.com/?p=amazon-linux-pipeline/
 
 ### LAST UPDATED
 
 Check when the bloom filters were last updated using the command line interface (CLI).
 
 ```
 mmi -u
 ```
 
 Or by hitting the provided website for the last updated timestamp.
 
-https://static.matchmeta.info/mmi.updated
+https://dl.4n6ir.com/match-meta-info/last.updated
+
+### COUNTS
+
+https://dl.4n6ir.com/match-meta-info/gtfo.count
+
+https://dl.4n6ir.com/match-meta-info/mmi.count
 
 ### DETECTIONS
 
 :purple_square: Empty File (purple) 
 
 A zero byte size determines empty files or the following hash value for this detection.
 
@@ -128,7 +134,9 @@
 ```
 
 ### DEVELOPMENT
 
 ```
 python setup.py install --user
 ```
+
+![Match Meta Inforamtion (MMI)](images/mmi.png)
```

### Comparing `matchmeta-2023.5.30/mmi/__init__.py` & `matchmeta-2024.4.14/mmi/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 __largefile__ = LARGEFILE = '\033[91m{}\033[00m'        ### RED ###
 __nofilehash__ = NOFILEHASH = '\033[93m{}\033[00m'      ### YELLOW ###
 __partialmeta__ = PARTIALMETA = '\033[97m{}\033[00m'    ### GREY ###
 
 __gtfo__ = GTFO = pathlib.Path.joinpath(pathlib.Path.home(), 'gtfo.bloom')
 __mmi__ = MMI = pathlib.Path.joinpath(pathlib.Path.home(), 'mmi.bloom')
 
-__version__ = VERSION = '2023.5.30'
+__version__ = VERSION = '2024.4.14'
```

### Comparing `matchmeta-2023.5.30/mmi/cli.py` & `matchmeta-2024.4.14/mmi/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -91,31 +91,31 @@
             else:
                 print('VERIFIED: '+str(__mmi__))
         else:
             print('CURRENT: '+str(__mmi__))
 
 def gtfobloom():
 
-    r = requests.get('https://static.matchmeta.info/gtfo.bloom')
+    r = requests.get('https://dl.4n6ir.com/match-meta-info/gtfo.bloom')
     if r.status_code == 200:
         with open(__gtfo__, 'wb') as f:
-            print('SUCCESS: https://static.matchmeta.info/gtfo.bloom')
+            print('SUCCESS: https://dl.4n6ir.com/match-meta-info/gtfo.bloom')
             f.write(r.content)
     else:
-        print('FAILED: https://static.matchmeta.info/gtfo.bloom')
+        print('FAILED: https://dl.4n6ir.com/match-meta-info/gtfo.bloom')
         sys.exit(1)
 
 def gtfoverify():
 
-    r = requests.get('https://static.matchmeta.info/gtfo.sha256')
+    r = requests.get('https://dl.4n6ir.com/match-meta-info/gtfo.sha256')
     if r.status_code == 200:
-        print('SUCCESS: https://static.matchmeta.info/gtfo.sha256')
+        print('SUCCESS: https://dl.4n6ir.com/match-meta-info/gtfo.sha256')
         return r.text
     else:
-        print('FAILED: https://static.matchmeta.info/gtfo.sha256')
+        print('FAILED: https://dl.4n6ir.com/match-meta-info/gtfo.sha256')
         sys.exit(1)
 
 def hasher(fullpath, mmi, gtfo):
 
     try:
         BLOCKSIZE = 65536
         sha256_hasher = hashlib.sha256()
@@ -148,31 +148,31 @@
     sha256_meta.update(fullpath.encode())
     sha256_hash = sha256_meta.hexdigest().upper()
     status = check(sha256_hash, mmi, gtfo)
     return status
 
 def mmibloom():
 
-    r = requests.get('https://static.matchmeta.info/mmi.bloom')
+    r = requests.get('https://dl.4n6ir.com/match-meta-info/mmi.bloom')
     if r.status_code == 200:
         with open(__mmi__, 'wb') as f:
-            print('SUCCESS: https://static.matchmeta.info/mmi.bloom')
+            print('SUCCESS: https://dl.4n6ir.com/match-meta-info/mmi.bloom')
             f.write(r.content)
     else:
-        print('FAILED: https://static.matchmeta.info/mmi.bloom')
+        print('FAILED: https://dl.4n6ir.com/match-meta-info/mmi.bloom')
         sys.exit(1)
 
 def mmiverify():
 
-    r = requests.get('https://static.matchmeta.info/mmi.sha256')
+    r = requests.get('https://dl.4n6ir.com/match-meta-info/mmi.sha256')
     if r.status_code == 200:
-        print('SUCCESS: https://static.matchmeta.info/mmi.sha256')
+        print('SUCCESS: https://dl.4n6ir.com/match-meta-info/mmi.sha256')
         return r.text
     else:
-        print('FAILED: https://static.matchmeta.info/mmi.sha256')
+        print('FAILED: https://dl.4n6ir.com/match-meta-info/mmi.sha256')
         sys.exit(1)
 
 def normalize(path):
 
     if path[:1] == '/':
         out = path.split('/')
         try:
@@ -279,20 +279,20 @@
             if str(p.parent) == '/':
                 print(denied+' '+sha256+' '+dir+file)
             else:
                 print(denied+' '+sha256+' '+dir+slash+file)
 
 def updated():
 
-    r = requests.get('https://static.matchmeta.info/mmi.updated')
+    r = requests.get('https://dl.4n6ir.com/match-meta-info/last.updated')
     if r.status_code == 200:
-        print('SUCCESS: https://static.matchmeta.info/mmi.updated')
+        print('SUCCESS: https://dl.4n6ir.com/match-meta-info/last.updated')
         print('LAST UPDATED: '+r.text)
     else:
-        print('FAILED: https://static.matchmeta.info/mmi.updated')
+        print('FAILED: https://dl.4n6ir.com/match-meta-info/last.updated')
         sys.exit(1)
 
 def main():
 
     parser = argparse.ArgumentParser(description='MMI - OS Triage for Anyone and Everyone')
     parser.add_argument('-d', '--download', help='Download Bloom Filters', action='store_true')
     parser.add_argument('-s', '--skip', help='Skip File Hashing', action='store_true')
```

### Comparing `matchmeta-2023.5.30/setup.py` & `matchmeta-2024.4.14/setup.py`

 * *Files identical despite different names*

