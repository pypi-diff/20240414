# Comparing `tmp/lektor-netlify-lfs-resize-url-1.0.2.tar.gz` & `tmp/lektor_netlify_lfs_resize_url-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lektor-netlify-lfs-resize-url-1.0.2.tar", last modified: Tue Mar 21 01:06:57 2023, max compression
+gzip compressed data, was "lektor_netlify_lfs_resize_url-1.0.3.tar", last modified: Sun Apr 14 19:29:48 2024, max compression
```

## Comparing `lektor-netlify-lfs-resize-url-1.0.2.tar` & `lektor_netlify_lfs_resize_url-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-03-21 01:06:57.897282 lektor-netlify-lfs-resize-url-1.0.2/
--rw-r--r--   0 jm        (1000) jm        (1000)     1071 2023-03-21 00:39:16.000000 lektor-netlify-lfs-resize-url-1.0.2/LICENSE
--rw-r--r--   0 jm        (1000) jm        (1000)     2469 2023-03-21 01:06:57.897282 lektor-netlify-lfs-resize-url-1.0.2/PKG-INFO
--rw-r--r--   0 jm        (1000) jm        (1000)     2083 2023-03-21 00:39:16.000000 lektor-netlify-lfs-resize-url-1.0.2/README.md
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-03-21 01:06:57.897282 lektor-netlify-lfs-resize-url-1.0.2/lektor_netlify_lfs_resize_url.egg-info/
--rw-r--r--   0 jm        (1000) jm        (1000)     2469 2023-03-21 01:06:57.000000 lektor-netlify-lfs-resize-url-1.0.2/lektor_netlify_lfs_resize_url.egg-info/PKG-INFO
--rw-r--r--   0 jm        (1000) jm        (1000)      327 2023-03-21 01:06:57.000000 lektor-netlify-lfs-resize-url-1.0.2/lektor_netlify_lfs_resize_url.egg-info/SOURCES.txt
--rw-r--r--   0 jm        (1000) jm        (1000)        1 2023-03-21 01:06:57.000000 lektor-netlify-lfs-resize-url-1.0.2/lektor_netlify_lfs_resize_url.egg-info/dependency_links.txt
--rw-r--r--   0 jm        (1000) jm        (1000)       98 2023-03-21 01:06:57.000000 lektor-netlify-lfs-resize-url-1.0.2/lektor_netlify_lfs_resize_url.egg-info/entry_points.txt
--rw-r--r--   0 jm        (1000) jm        (1000)       30 2023-03-21 01:06:57.000000 lektor-netlify-lfs-resize-url-1.0.2/lektor_netlify_lfs_resize_url.egg-info/top_level.txt
--rw-r--r--   0 jm        (1000) jm        (1000)     1002 2023-03-21 00:39:16.000000 lektor-netlify-lfs-resize-url-1.0.2/lektor_netlify_lfs_resize_url.py
--rw-r--r--   0 jm        (1000) jm        (1000)       38 2023-03-21 01:06:57.897282 lektor-netlify-lfs-resize-url-1.0.2/setup.cfg
--rw-r--r--   0 jm        (1000) jm        (1000)     1067 2023-03-21 01:04:17.000000 lektor-netlify-lfs-resize-url-1.0.2/setup.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2024-04-14 19:29:48.441980 lektor_netlify_lfs_resize_url-1.0.3/
+-rw-r--r--   0 jm        (1000) jm        (1000)     1071 2024-04-14 19:27:57.000000 lektor_netlify_lfs_resize_url-1.0.3/LICENSE
+-rw-r--r--   0 jm        (1000) jm        (1000)     2808 2024-04-14 19:29:48.441980 lektor_netlify_lfs_resize_url-1.0.3/PKG-INFO
+-rw-r--r--   0 jm        (1000) jm        (1000)     2422 2024-04-14 19:27:06.000000 lektor_netlify_lfs_resize_url-1.0.3/README.md
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2024-04-14 19:29:48.441980 lektor_netlify_lfs_resize_url-1.0.3/lektor_netlify_lfs_resize_url.egg-info/
+-rw-r--r--   0 jm        (1000) jm        (1000)     2808 2024-04-14 19:29:48.000000 lektor_netlify_lfs_resize_url-1.0.3/lektor_netlify_lfs_resize_url.egg-info/PKG-INFO
+-rw-r--r--   0 jm        (1000) jm        (1000)      327 2024-04-14 19:29:48.000000 lektor_netlify_lfs_resize_url-1.0.3/lektor_netlify_lfs_resize_url.egg-info/SOURCES.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)        1 2024-04-14 19:29:48.000000 lektor_netlify_lfs_resize_url-1.0.3/lektor_netlify_lfs_resize_url.egg-info/dependency_links.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)       98 2024-04-14 19:29:48.000000 lektor_netlify_lfs_resize_url-1.0.3/lektor_netlify_lfs_resize_url.egg-info/entry_points.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)       30 2024-04-14 19:29:48.000000 lektor_netlify_lfs_resize_url-1.0.3/lektor_netlify_lfs_resize_url.egg-info/top_level.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)     1002 2023-03-21 00:39:16.000000 lektor_netlify_lfs_resize_url-1.0.3/lektor_netlify_lfs_resize_url.py
+-rw-r--r--   0 jm        (1000) jm        (1000)       38 2024-04-14 19:29:48.441980 lektor_netlify_lfs_resize_url-1.0.3/setup.cfg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1067 2024-04-14 19:27:37.000000 lektor_netlify_lfs_resize_url-1.0.3/setup.py
```

### Comparing `lektor-netlify-lfs-resize-url-1.0.2/LICENSE` & `lektor_netlify_lfs_resize_url-1.0.3/LICENSE`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Jonathan Mason
+Copyright (c) 2024 Jonathan Mason
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `lektor-netlify-lfs-resize-url-1.0.2/PKG-INFO` & `lektor_netlify_lfs_resize_url-1.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: lektor-netlify-lfs-resize-url
-Version: 1.0.2
+Version: 1.0.3
 Summary: Convert image URLs to Netlify LFS resize URLs.
 Home-page: https://gitlab.com/JM0804/lektor-netlify-lfs-resize-url
 Author: Jonathan Mason
 License: MIT
 Keywords: Lektor plugin
 Classifier: Framework :: Lektor
 Classifier: Environment :: Plugins
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # netlify-lfs-resize-url
 
 ![PyPI - License](https://img.shields.io/pypi/l/lektor-netlify-lfs-resize-url) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) ![PyPI - Downloads](https://img.shields.io/pypi/dw/lektor-netlify-lfs-resize-url)
 
+## Please note!
+
+Netlify Large Media has now [been deprecated](https://answers.netlify.com/t/large-media-feature-deprecated-but-not-removed/100804). This plugin will no longer be maintained. I would like to take this opportunity to thank everyone who's used it - I hope you've been happy with the service it has provided.
+
+## Description
+
 This plugin provides a filter that allows the user to generate [Netlify Image Transformation](https://www.netlify.com/docs/image-transformation/) resize URL parameters when working with [Netlify Large Media](https://www.netlify.com/docs/large-media/).
 
 ## Installation
 
 You can install this plugin by running the following command in your project's directory:
 
 ```sh
```

### Comparing `lektor-netlify-lfs-resize-url-1.0.2/README.md` & `lektor_netlify_lfs_resize_url-1.0.3/lektor_netlify_lfs_resize_url.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,30 @@
+Metadata-Version: 2.1
+Name: lektor-netlify-lfs-resize-url
+Version: 1.0.3
+Summary: Convert image URLs to Netlify LFS resize URLs.
+Home-page: https://gitlab.com/JM0804/lektor-netlify-lfs-resize-url
+Author: Jonathan Mason
+License: MIT
+Keywords: Lektor plugin
+Classifier: Framework :: Lektor
+Classifier: Environment :: Plugins
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # netlify-lfs-resize-url
 
 ![PyPI - License](https://img.shields.io/pypi/l/lektor-netlify-lfs-resize-url) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) ![PyPI - Downloads](https://img.shields.io/pypi/dw/lektor-netlify-lfs-resize-url)
 
+## Please note!
+
+Netlify Large Media has now [been deprecated](https://answers.netlify.com/t/large-media-feature-deprecated-but-not-removed/100804). This plugin will no longer be maintained. I would like to take this opportunity to thank everyone who's used it - I hope you've been happy with the service it has provided.
+
+## Description
+
 This plugin provides a filter that allows the user to generate [Netlify Image Transformation](https://www.netlify.com/docs/image-transformation/) resize URL parameters when working with [Netlify Large Media](https://www.netlify.com/docs/large-media/).
 
 ## Installation
 
 You can install this plugin by running the following command in your project's directory:
 
 ```sh
```

### Comparing `lektor-netlify-lfs-resize-url-1.0.2/lektor_netlify_lfs_resize_url.egg-info/PKG-INFO` & `lektor_netlify_lfs_resize_url-1.0.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,17 @@
-Metadata-Version: 2.1
-Name: lektor-netlify-lfs-resize-url
-Version: 1.0.2
-Summary: Convert image URLs to Netlify LFS resize URLs.
-Home-page: https://gitlab.com/JM0804/lektor-netlify-lfs-resize-url
-Author: Jonathan Mason
-License: MIT
-Keywords: Lektor plugin
-Classifier: Framework :: Lektor
-Classifier: Environment :: Plugins
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # netlify-lfs-resize-url
 
 ![PyPI - License](https://img.shields.io/pypi/l/lektor-netlify-lfs-resize-url) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) ![PyPI - Downloads](https://img.shields.io/pypi/dw/lektor-netlify-lfs-resize-url)
 
+## Please note!
+
+Netlify Large Media has now [been deprecated](https://answers.netlify.com/t/large-media-feature-deprecated-but-not-removed/100804). This plugin will no longer be maintained. I would like to take this opportunity to thank everyone who's used it - I hope you've been happy with the service it has provided.
+
+## Description
+
 This plugin provides a filter that allows the user to generate [Netlify Image Transformation](https://www.netlify.com/docs/image-transformation/) resize URL parameters when working with [Netlify Large Media](https://www.netlify.com/docs/large-media/).
 
 ## Installation
 
 You can install this plugin by running the following command in your project's directory:
 
 ```sh
```

### Comparing `lektor-netlify-lfs-resize-url-1.0.2/lektor_netlify_lfs_resize_url.py` & `lektor_netlify_lfs_resize_url-1.0.3/lektor_netlify_lfs_resize_url.py`

 * *Files identical despite different names*

### Comparing `lektor-netlify-lfs-resize-url-1.0.2/setup.py` & `lektor_netlify_lfs_resize_url-1.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     license='MIT',
     long_description=readme,
     long_description_content_type='text/markdown',
     name='lektor-netlify-lfs-resize-url',
     packages=find_packages(),
     py_modules=['lektor_netlify_lfs_resize_url'],
     url='https://gitlab.com/JM0804/lektor-netlify-lfs-resize-url',
-    version='1.0.2',
+    version='1.0.3',
     classifiers=[
         'Framework :: Lektor',
         'Environment :: Plugins',
     ],
     entry_points={
         'lektor.plugins': [
             'netlify-lfs-resize-url = \
```

