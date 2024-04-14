# Comparing `tmp/zkyhaxpy-0.3.0.2.0.tar.gz` & `tmp/zkyhaxpy-0.3.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zkyhaxpy-0.3.0.2.0.tar", last modified: Tue Feb 21 04:12:54 2023, max compression
+gzip compressed data, was "zkyhaxpy-0.3.1.0.1.tar", last modified: Sun Apr 14 16:07:11 2024, max compression
```

## Comparing `zkyhaxpy-0.3.0.2.0.tar` & `zkyhaxpy-0.3.1.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-02-21 04:12:54.485171 zkyhaxpy-0.3.0.2.0/
--rw-rw-rw-   0        0        0     1067 2022-12-13 12:57:29.000000 zkyhaxpy-0.3.0.2.0/LICENSE
--rw-rw-rw-   0        0        0      655 2023-02-21 04:12:54.484171 zkyhaxpy-0.3.0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      141 2022-12-13 12:57:29.000000 zkyhaxpy-0.3.0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-02-21 04:12:54.485171 zkyhaxpy-0.3.0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      736 2023-02-21 03:45:04.000000 zkyhaxpy-0.3.0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-21 04:12:54.446171 zkyhaxpy-0.3.0.2.0/zkyhaxpy/
--rw-rw-rw-   0        0        0        0 2022-12-13 12:57:29.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy/__init__.py
--rw-rw-rw-   0        0        0     1598 2022-12-13 12:57:29.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy/aws_tools.py
--rw-rw-rw-   0        0        0     2929 2022-12-13 12:57:29.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy/colab_tools.py
--rw-rw-rw-   0        0        0      875 2022-12-13 12:57:29.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy/console_tools.py
--rw-rw-rw-   0        0        0      623 2022-12-13 12:57:29.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy/dict_tools.py
--rw-rw-rw-   0        0        0     5115 2022-12-13 12:57:29.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy/dttm_tools.py
--rw-rw-rw-   0        0        0     3411 2022-12-13 12:57:29.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy/ftp_tools.py
--rw-rw-rw-   0        0        0      600 2022-12-13 12:57:29.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy/gcp_tools.py
--rw-rw-rw-   0        0        0    36016 2023-02-09 07:58:34.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy/gis_tools.py
--rw-rw-rw-   0        0        0      348 2022-12-13 12:57:29.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy/hash_tools.py
--rw-rw-rw-   0        0        0      644 2022-12-13 12:57:29.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy/http_tools.py
--rw-rw-rw-   0        0        0     1280 2022-12-13 12:57:29.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy/img_tools.py
--rw-rw-rw-   0        0        0    13142 2023-02-21 04:03:15.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy/io_tools.py
--rw-rw-rw-   0        0        0     3515 2022-12-13 12:57:29.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy/json_tools.py
--rw-rw-rw-   0        0        0      179 2023-02-10 08:41:26.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy/jupyter_tools.py
--rw-rw-rw-   0        0        0     2002 2022-12-13 12:57:29.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy/log_tools.py
--rw-rw-rw-   0        0        0     6180 2022-12-13 12:57:29.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy/ml_tools.py
--rw-rw-rw-   0        0        0      271 2022-12-13 12:57:29.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy/mpl_tools.py
--rw-rw-rw-   0        0        0      652 2022-12-13 12:57:29.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy/multitask_tools.py
--rw-rw-rw-   0        0        0     2396 2022-12-13 12:57:29.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy/np_tools.py
--rw-rw-rw-   0        0        0     6709 2023-02-21 04:10:03.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy/pd_tools.py
--rw-rw-rw-   0        0        0     1768 2022-12-13 12:57:29.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy/skopt_tools.py
--rw-rw-rw-   0        0        0     1208 2022-12-13 12:57:29.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy/snippet_tools.py
--rw-rw-rw-   0        0        0      449 2022-12-13 12:57:29.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy/str_tools.py
--rw-rw-rw-   0        0        0     1786 2022-12-13 12:57:29.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy/timer_tools.py
--rw-rw-rw-   0        0        0      645 2022-12-13 12:57:29.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy/util_tools.py
-drwxrwxrwx   0        0        0        0 2023-02-21 04:12:54.481179 zkyhaxpy-0.3.0.2.0/zkyhaxpy.egg-info/
--rw-rw-rw-   0        0        0      655 2023-02-21 04:12:52.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      751 2023-02-21 04:12:53.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-21 04:12:52.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-02-21 04:12:53.000000 zkyhaxpy-0.3.0.2.0/zkyhaxpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-14 16:07:11.873611 zkyhaxpy-0.3.1.0.1/
+-rw-rw-rw-   0        0        0     1088 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      616 2024-04-14 16:07:11.873611 zkyhaxpy-0.3.1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      141 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-14 16:07:11.874611 zkyhaxpy-0.3.1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      703 2024-04-14 14:46:44.000000 zkyhaxpy-0.3.1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 16:07:11.861611 zkyhaxpy-0.3.1.0.1/zkyhaxpy/
+-rw-rw-rw-   0        0        0        0 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/__init__.py
+-rw-rw-rw-   0        0        0     1651 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/aws_tools.py
+-rw-rw-rw-   0        0        0     2929 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/colab_tools.py
+-rw-rw-rw-   0        0        0      875 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/console_tools.py
+-rw-rw-rw-   0        0        0      623 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/dict_tools.py
+-rw-rw-rw-   0        0        0     5115 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/dttm_tools.py
+-rw-rw-rw-   0        0        0     3411 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/ftp_tools.py
+-rw-rw-rw-   0        0        0      614 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/gcp_tools.py
+-rw-rw-rw-   0        0        0    41927 2024-04-14 14:46:31.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/gis_tools.py
+-rw-rw-rw-   0        0        0      348 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/hash_tools.py
+-rw-rw-rw-   0        0        0      664 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/http_tools.py
+-rw-rw-rw-   0        0        0     1280 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/img_tools.py
+-rw-rw-rw-   0        0        0    13142 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/io_tools.py
+-rw-rw-rw-   0        0        0     3515 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/json_tools.py
+-rw-rw-rw-   0        0        0      179 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/jupyter_tools.py
+-rw-rw-rw-   0        0        0     2002 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/log_tools.py
+-rw-rw-rw-   0        0        0     6360 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/ml_tools.py
+-rw-rw-rw-   0        0        0      281 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/mpl_tools.py
+-rw-rw-rw-   0        0        0      652 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/multitask_tools.py
+-rw-rw-rw-   0        0        0     2396 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/np_tools.py
+-rw-rw-rw-   0        0        0     6709 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/pd_tools.py
+-rw-rw-rw-   0        0        0     1822 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/skopt_tools.py
+-rw-rw-rw-   0        0        0     1130 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/snippet_tools.py
+-rw-rw-rw-   0        0        0      463 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/str_tools.py
+-rw-rw-rw-   0        0        0     1838 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/timer_tools.py
+-rw-rw-rw-   0        0        0      663 2024-04-13 04:50:52.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy/util_tools.py
+drwxrwxrwx   0        0        0        0 2024-04-14 16:07:11.872611 zkyhaxpy-0.3.1.0.1/zkyhaxpy.egg-info/
+-rw-rw-rw-   0        0        0      616 2024-04-14 16:07:11.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      751 2024-04-14 16:07:11.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 16:07:11.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-14 16:07:11.000000 zkyhaxpy-0.3.1.0.1/zkyhaxpy.egg-info/top_level.txt
```

### Comparing `zkyhaxpy-0.3.0.2.0/LICENSE` & `zkyhaxpy-0.3.1.0.1/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2019 surasakcho
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2019 surasakcho
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `zkyhaxpy-0.3.0.2.0/PKG-INFO` & `zkyhaxpy-0.3.1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 Metadata-Version: 2.1
 Name: zkyhaxpy
-Version: 0.3.0.2.0
+Version: 0.3.1.0.1
 Summary: A swiss-knife Data Science package for python
 Home-page: https://github.com/surasakcho/zkyhaxpy
 Author: Surasak Choedpasuporn
 Author-email: surasak.cho@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is zkyhaxpy package.
 zkyhaxpy is a python package for personal usage.
 It provides a lot of useful tools for working as data scientist.
-
```

### Comparing `zkyhaxpy-0.3.0.2.0/setup.py` & `zkyhaxpy-0.3.1.0.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name="zkyhaxpy", # Replace with your own username
-    version="0.3.0.2.0",
+    name="zkyhaxpy",
+    version="0.3.1.0.1",
     author="Surasak Choedpasuporn",
     author_email="surasak.cho@gmail.com",
     description="A swiss-knife Data Science package for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/surasakcho/zkyhaxpy",
     packages=setuptools.find_packages(),
```

### Comparing `zkyhaxpy-0.3.0.2.0/zkyhaxpy/aws_tools.py` & `zkyhaxpy-0.3.1.0.1/zkyhaxpy/aws_tools.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-import logging
-import boto3
-from botocore.exceptions import ClientError
-import os
-import re
-
-def upload_file(file_name, bucket, object_name=None):
-    """
-    
-    Upload a file to an S3 bucket    
-
-    :param file_name: File to upload
-    :param bucket: Bucket to upload to
-    :param object_name: S3 object name. If not specified then file_name is used
-    :return: True if file was uploaded, else False
-    
-    (This code is from https://boto3.amazonaws.com/v1/documentation/api/latest/guide/s3-examples.html)
-    """
-
-    # If S3 object_name was not specified, use file_name
-    if object_name is None:
-        object_name = os.path.basename(file_name)
-
-    # Upload the file
-    s3_client = boto3.client('s3')
-    try:
-        response = s3_client.upload_file(file_name, bucket, object_name)
-    except ClientError as e:
-        logging.error(e)
-        return False
-    return True
-
-
-
-def download_file(bucket_name, object_name, path_dest, replace=False):
-    if (os.path.exists(path_dest) == True) & (replace==False):
-        print(f'{path_dest} already exists. Skipping.')
-        return
-    s3 = boto3.client('s3')
-    s3.download_file(bucket_name, object_name, path_dest)
-    
-
-def get_list_of_objects(bucket_name, object_regex='.*'):
-
-    s3 = boto3.client('s3')
-    s3_resource = boto3.resource('s3')
-    my_bucket = s3_resource.Bucket(bucket_name)
-
-    list_objects = []
-    for my_bucket_object in my_bucket.objects.all():
-        object_key = my_bucket_object.key
-        result = re.match(object_regex, object_key)
-        if result:
+import logging
+import boto3
+from botocore.exceptions import ClientError
+import os
+import re
+
+def upload_file(file_name, bucket, object_name=None):
+    """
+    
+    Upload a file to an S3 bucket    
+
+    :param file_name: File to upload
+    :param bucket: Bucket to upload to
+    :param object_name: S3 object name. If not specified then file_name is used
+    :return: True if file was uploaded, else False
+    
+    (This code is from https://boto3.amazonaws.com/v1/documentation/api/latest/guide/s3-examples.html)
+    """
+
+    # If S3 object_name was not specified, use file_name
+    if object_name is None:
+        object_name = os.path.basename(file_name)
+
+    # Upload the file
+    s3_client = boto3.client('s3')
+    try:
+        response = s3_client.upload_file(file_name, bucket, object_name)
+    except ClientError as e:
+        logging.error(e)
+        return False
+    return True
+
+
+
+def download_file(bucket_name, object_name, path_dest, replace=False):
+    if (os.path.exists(path_dest) == True) & (replace==False):
+        print(f'{path_dest} already exists. Skipping.')
+        return
+    s3 = boto3.client('s3')
+    s3.download_file(bucket_name, object_name, path_dest)
+    
+
+def get_list_of_objects(bucket_name, object_regex='.*'):
+
+    s3 = boto3.client('s3')
+    s3_resource = boto3.resource('s3')
+    my_bucket = s3_resource.Bucket(bucket_name)
+
+    list_objects = []
+    for my_bucket_object in my_bucket.objects.all():
+        object_key = my_bucket_object.key
+        result = re.match(object_regex, object_key)
+        if result:
             list_objects.append(object_key)
```

### Comparing `zkyhaxpy-0.3.0.2.0/zkyhaxpy/colab_tools.py` & `zkyhaxpy-0.3.1.0.1/zkyhaxpy/colab_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.0.2.0/zkyhaxpy/console_tools.py` & `zkyhaxpy-0.3.1.0.1/zkyhaxpy/console_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.0.2.0/zkyhaxpy/dict_tools.py` & `zkyhaxpy-0.3.1.0.1/zkyhaxpy/dict_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.0.2.0/zkyhaxpy/dttm_tools.py` & `zkyhaxpy-0.3.1.0.1/zkyhaxpy/dttm_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.0.2.0/zkyhaxpy/ftp_tools.py` & `zkyhaxpy-0.3.1.0.1/zkyhaxpy/ftp_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.0.2.0/zkyhaxpy/gcp_tools.py` & `zkyhaxpy-0.3.1.0.1/zkyhaxpy/gcp_tools.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from google.cloud import storage
-
-def get_bucket_and_file_name_from_uri(file_uri):
-    assert(file_uri.startswith('gs://'))
-    file_uri = file_uri.replace('gs://', '')
-    bucket_name = file_uri.split('/')[0]
-    file_name = '/'.join(file_uri.split('/')[1:])
-    return (bucket_name, file_name)
-
-def check_file_exists_gcs(file_uri):        
-    bucket_name, file_name = get_bucket_and_file_name_from_uri(file_uri)
-    storage_client = storage.Client()    
-    bucket = storage_client.bucket(bucket_name)
-    stats = storage.Blob(bucket=bucket, name=file_name).exists(storage_client)
+from google.cloud import storage
+
+def get_bucket_and_file_name_from_uri(file_uri):
+    assert(file_uri.startswith('gs://'))
+    file_uri = file_uri.replace('gs://', '')
+    bucket_name = file_uri.split('/')[0]
+    file_name = '/'.join(file_uri.split('/')[1:])
+    return (bucket_name, file_name)
+
+def check_file_exists_gcs(file_uri):        
+    bucket_name, file_name = get_bucket_and_file_name_from_uri(file_uri)
+    storage_client = storage.Client()    
+    bucket = storage_client.bucket(bucket_name)
+    stats = storage.Blob(bucket=bucket, name=file_name).exists(storage_client)
     return stats
```

### Comparing `zkyhaxpy-0.3.0.2.0/zkyhaxpy/gis_tools.py` & `zkyhaxpy-0.3.1.0.1/zkyhaxpy/gis_tools.py`

 * *Files 18% similar despite different names*

```diff
@@ -229,15 +229,15 @@
     geometry : str specifies column name of geometry in df
     
     OUTPUT
     return :GeoPandas's DataFrame (gdf)
     '''
     df = df.copy()
     df['geometry'] = df[geometry].apply(wkt.loads)
-    gdf = gpd.GeoDataFrame(df, geometry='geometry', crs={'init' : 'epsg:4326'})
+    gdf = gpd.GeoDataFrame(df, geometry='geometry', crs='epsg:4326')
     del(df)
     if drop_old_geom_col==True:
         gdf = gdf.drop(columns=[geometry]).copy()
         
     if drop_z==True:
         if gdf['geometry'].has_z.sum() > 0:
             gdf_has_z = gdf[gdf['geometry'].has_z]
@@ -883,15 +883,21 @@
     path_ds_mapping = create_row_col_mapping_raster(in_raster_path, out_mem=False)
     
 
     #getting row-col from on-memory row-col raster
     list_arr_row_col = []    
     list_polygon_id = []    
     
-    for polygon_id, tmp_polygon in tqdm(in_s_polygon.iteritems(), 'Getting row&col of pixels...', total=len(in_s_polygon)):
+    try:
+        zip_tup_polygon =  in_s_polygon.items()
+    except AttributeError:
+        #Support pandas version >= 1.5.0
+        zip_tup_polygon =  in_s_polygon.iteritems()        
+        
+    for polygon_id, tmp_polygon in tqdm(zip_tup_polygon, 'Getting row&col of pixels...', total=len(in_s_polygon)):
         is_polygon_overlap, nbr_pixels, arr_row_col = get_pix_row_col(tmp_polygon, path_ds_mapping)
         if is_polygon_overlap:
             list_polygon_id.append(polygon_id)
             list_arr_row_col.append(arr_row_col)
         
     shutil.rmtree(os.path.dirname(path_ds_mapping))
     arr_polygon_id, arr_row, arr_col = __reformat_list_row_col_for_df(list_polygon_id, list_arr_row_col)
@@ -1094,8 +1100,185 @@
 
 #         arr_pixel_row_col = arr_mapping[((arr_mapping[:, 2] >= lat ) & (arr_mapping[:, 3] < lat) & (arr_mapping[:, 4] >= lon ) & (arr_mapping[:, 5] < lon))]
 #         if(len(arr_pixel_row_col)==1):
 #             row, col = arr_pixel_row_col[0, 0:2]
 #             row = int(row)
 #             col = int(col)
 #         return row, col
-        return __get_pixel_rowcol_from_latlon_numba(lat, lon, arr_mapping)
+        return __get_pixel_rowcol_from_latlon_numba(lat, lon, arr_mapping)
+    
+    
+
+def convert_hdf_to_geotiff(
+    path_in, path_out, subds,
+    ):
+    '''
+    Convert one band of one subdataset from a HDF4 (ex. MODIS) into GeoTiff file.
+        
+    params
+    ----------
+    path_in: str or path-like
+        A path of input HDF file
+    path_out: str or path-like
+        A path of input GeoTiff file
+    subds: str
+        Target subdataset to extract (ex. "grid1km:Optical_Depth_055")
+
+        
+    returns
+    ---------
+    result: int
+        0 = ok, otherwise failed
+    '''
+    
+    srcfile = f'HDF4_EOS:EOS_GRID:"{path_in}":{subds}' 
+    gdal_cmd = f"gdal_translate -of GTiff {srcfile} {path_out}"    
+    return os.system(gdal_cmd)    
+
+
+
+def get_qa_val_cloud_clear_flag(qa_val, tup_cloud_bits_idx, str_cloud_clear, qa_total_bits, nodata, ):
+    '''
+    Get cloud clear flag of given QA value.
+    
+    params
+    ---------
+    qa_val: numeric
+        Pixel value of QA
+    tup_cloud_bits_idx: tuple()
+        A tuple to idx to extract bits from binary str. This identifier will work backward. Meaning getting first 3 digits will actually last 3 digits of binary string. For example, if binary string = '0b000100' and tup_cloud_bits_idx = (0, 3), it will get bit from backward and result will be '001'.        
+    str_cloud_clear: str
+        A string of bits that mean no cloud. This value can be get from Satellite data provider's document of the product. Do not reverse this value.
+    qa_total_bits: int
+        No. of bits for qa
+    nodata: numeric
+        A value specify pixel value is N/A
+    
+    For more information, see https://atmosphere-imager.gsfc.nasa.gov/sites/default/files/ModAtmo/QA_Plan_C61_Master_2017_03_15.pdf
+    
+    Return
+    ---------       
+        - 1 if it is cloud clear.
+        - 0 if it is not cloud clear.
+        - -9 if N/A
+    '''    
+    if qa_val==nodata:
+        return -9
+
+    str_bin = bin(qa_val)[2:].zfill(qa_total_bits)
+    
+    if tup_cloud_bits_idx[0] > 0:
+        
+        str_nbits = str_bin[-tup_cloud_bits_idx[1]:-tup_cloud_bits_idx[0]]
+    else:    
+        str_nbits = str_bin[-tup_cloud_bits_idx[1]:]
+        
+    return int(str_nbits==str_cloud_clear)
+    
+    
+def get_arr_cloud_clear_f(
+    path_in_qa,
+    band_id_qa,
+    tup_cloud_bits_idx, 
+    str_cloud_clear,
+    qa_total_bits,
+    nodata_qa=0
+):
+    '''
+    Get an array of cloud clear flag from given qa raster.
+    
+    params
+    ----------
+    paht_in_qa - str or path
+        A path of QA raster
+    tup_cloud_bits_idx - tuple
+        A tuple of bits identifier index for QA band that can identify cloud. If first 3 digits, tup_cloud_bits_idx should be (0, 3). Get this value from product manual.
+    str_cloud_clear - str
+        A string of cloud bits that means cloud clear. Get this value from product manual.        
+    nodata_qa - numeric
+        A value that means QA pixel is N/A. Default is 0.
+        
+    returns
+    ----------
+    arr_cloud_clear_f - numpy array (m, n)
+        An array of cloud clear flag. 1 = cloud clear pixel, 0 = cloudy pixel, NaN = N/A
+    '''
+    with rasterio.open(path_in_qa) as ds:    
+        arr_qa = ds.read(band_id_qa)
+            
+    #Array of cloud clear flag
+    dict_qa_cloud_clear = {qa_val:get_qa_val_cloud_clear_flag(qa_val, tup_cloud_bits_idx, str_cloud_clear, qa_total_bits, nodata_qa) for qa_val in np.unique(arr_qa)}
+    
+    
+    return np.vectorize(dict_qa_cloud_clear.get)(arr_qa)
+
+
+
+def extract_cloudless_band(
+    path_in_target, 
+    path_in_qa,     
+    band_id_target, 
+    band_id_qa,     
+    tup_cloud_bits_idx, 
+    str_cloud_clear,
+    qa_total_bits,
+    nodata_target=None,
+    nodata_qa=0,    
+    path_out=None,     
+    ):
+    '''
+    Extract cloudless band of a value raster given a qa raster.
+    
+    params
+    ---------
+    path_in_target - str or path
+        A path of target raster
+    paht_in_qa - str or path
+        A path of QA raster
+    path_out - str or path
+        path for output raster
+    band_id_target - int
+        target's band id (start at 1)
+    band_id_qa - int
+        QA's band id        
+    tup_cloud_bits_idx - tuple
+        A tuple of bits identifier index for QA band that can identify cloud. If first 3 digits, tup_cloud_bits_idx should be (0, 3). Get this value from product manual.
+    str_cloud_clear - str
+        A string of cloud bits that means cloud clear. Get this value from product manual.        
+    qa_total_bits - int
+        No. of total bits of QA
+    nodata_target - numeric
+        A value that means target pixel is N/A. 
+    nodata_qa - numeric
+        A value that means QA pixel is N/A. Default is 0.
+    '''
+    #Read band data
+    with rasterio.open(path_in_target) as ds:    
+        profile = ds.profile
+        arr_target = ds.read(band_id_target)
+        if nodata_target is None:
+            #Get nodata value from dataset
+            nodata_target = ds.nodatavals[band_id_target-1]
+        # arr_target = np.where(arr_target==nodata_target, np.nan, arr_target)
+
+    #Get array of cloud clear flag        
+    arr_cloud_clear_f = get_arr_cloud_clear_f(
+        path_in_qa,
+        band_id_qa,
+        tup_cloud_bits_idx,
+        str_cloud_clear,
+        qa_total_bits,
+        nodata_qa
+    )
+    
+    arr_out = np.where(arr_cloud_clear_f==1, arr_target, nodata_target)
+    if path_out is not None:  
+        profile.update(
+            count=1,
+            compress='lzw'
+        )
+
+        with rasterio.open(path_out, 'w', **profile) as ds_out:
+            ds_out.write(arr_out, 1)
+        print(f'{path_out} has been saved')
+    return arr_out
+
```

### Comparing `zkyhaxpy-0.3.0.2.0/zkyhaxpy/img_tools.py` & `zkyhaxpy-0.3.1.0.1/zkyhaxpy/img_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.0.2.0/zkyhaxpy/io_tools.py` & `zkyhaxpy-0.3.1.0.1/zkyhaxpy/io_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.0.2.0/zkyhaxpy/json_tools.py` & `zkyhaxpy-0.3.1.0.1/zkyhaxpy/json_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.0.2.0/zkyhaxpy/log_tools.py` & `zkyhaxpy-0.3.1.0.1/zkyhaxpy/log_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.0.2.0/zkyhaxpy/multitask_tools.py` & `zkyhaxpy-0.3.1.0.1/zkyhaxpy/multitask_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.0.2.0/zkyhaxpy/np_tools.py` & `zkyhaxpy-0.3.1.0.1/zkyhaxpy/np_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.0.2.0/zkyhaxpy/pd_tools.py` & `zkyhaxpy-0.3.1.0.1/zkyhaxpy/pd_tools.py`

 * *Files identical despite different names*

### Comparing `zkyhaxpy-0.3.0.2.0/zkyhaxpy/skopt_tools.py` & `zkyhaxpy-0.3.1.0.1/zkyhaxpy/skopt_tools.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-from skopt.space import Real, Integer, Categorical
-
-def get_skopt_search_space(in_dict_search_space):
-    '''
-    Transform dict of search space into skopt search space formatted.
-    
-    Input dict must be formatted as follow
-    
-    in_dict_search_space = {
-        "param_1":{
-            "type":"int",
-            "min":0,
-            "max":10,
-            "scale":"auto"
-        },
-        "param_2":{
-            "type":"real",
-            "min":0.1,
-            "max":100,
-            "scale":"log"
-        },
-        "param_3":{
-            "type":"categorical",
-            "values":["a", "b", "c"]
-        }
-    }
-    
-    '''
-    
-    out_dict_skopt_search_space = {}
-    for parm_nm in in_dict_search_space.keys():
-        if in_dict_search_space[parm_nm].get('scale')=='auto':
-            scale = 'uniform'
-        elif in_dict_search_space[parm_nm].get('scale')=='log':
-            scale = 'log-uniform'
-        else:
-            scale = 'auto'
-            
-        if in_dict_search_space[parm_nm]['type']=='real':
-            out_dict_skopt_search_space[parm_nm] = Real(
-                low=in_dict_search_space[parm_nm]['min'],
-                high=in_dict_search_space[parm_nm]['max'],
-                prior=scale
-            )
-        elif in_dict_search_space[parm_nm]['type']=='int':
-            out_dict_skopt_search_space[parm_nm] = Integer(
-                low=in_dict_search_space[parm_nm]['min'],
-                high=in_dict_search_space[parm_nm]['max'],
-                prior=scale
-            )
-        elif in_dict_search_space[parm_nm]['type']=='categorical':
-            out_dict_skopt_search_space[parm_nm] = Categorical(categories=in_dict_search_space[parm_nm]['values'], prior=None)
-        
-    return out_dict_skopt_search_space
+from skopt.space import Real, Integer, Categorical
+
+def get_skopt_search_space(in_dict_search_space):
+    '''
+    Transform dict of search space into skopt search space formatted.
+    
+    Input dict must be formatted as follow
+    
+    in_dict_search_space = {
+        "param_1":{
+            "type":"int",
+            "min":0,
+            "max":10,
+            "scale":"auto"
+        },
+        "param_2":{
+            "type":"real",
+            "min":0.1,
+            "max":100,
+            "scale":"log"
+        },
+        "param_3":{
+            "type":"categorical",
+            "values":["a", "b", "c"]
+        }
+    }
+    
+    '''
+    
+    out_dict_skopt_search_space = {}
+    for parm_nm in in_dict_search_space.keys():
+        if in_dict_search_space[parm_nm].get('scale')=='auto':
+            scale = 'uniform'
+        elif in_dict_search_space[parm_nm].get('scale')=='log':
+            scale = 'log-uniform'
+        else:
+            scale = 'auto'
+            
+        if in_dict_search_space[parm_nm]['type']=='real':
+            out_dict_skopt_search_space[parm_nm] = Real(
+                low=in_dict_search_space[parm_nm]['min'],
+                high=in_dict_search_space[parm_nm]['max'],
+                prior=scale
+            )
+        elif in_dict_search_space[parm_nm]['type']=='int':
+            out_dict_skopt_search_space[parm_nm] = Integer(
+                low=in_dict_search_space[parm_nm]['min'],
+                high=in_dict_search_space[parm_nm]['max'],
+                prior=scale
+            )
+        elif in_dict_search_space[parm_nm]['type']=='categorical':
+            out_dict_skopt_search_space[parm_nm] = Categorical(categories=in_dict_search_space[parm_nm]['values'], prior=None)
+        
+    return out_dict_skopt_search_space
```

### Comparing `zkyhaxpy-0.3.0.2.0/zkyhaxpy/timer_tools.py` & `zkyhaxpy-0.3.1.0.1/zkyhaxpy/timer_tools.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import datetime
-
-class timer:
-  
-    def __init__(self, name):
-        self.name = name
-        self.start_time = None
-        self.end_time = None
-        self.lap_times = []
-        self.elapsed_time = None
-
-    def start(self):
-        self.start_time = datetime.datetime.now()
-        print(f'Start at: {self.start_time}')
-
-    def end(self):
-        self.end_time = datetime.datetime.now()        
-        print(f'End at: {self.end_time}')
-        self.elapsed_time = self.end_time - self.start_time
-        print()
-        self.show()
-
-    def lap(self):
-        curr_lap_time = datetime.datetime.now()
-        if len(self.lap_times) > 0:
-            prev_lap_time = self.lap_times[-1]
-        else:
-            prev_lap_time = self.start_time
-        latest_lap_elapsed_time = curr_lap_time - prev_lap_time
-        self.lap_times.append(curr_lap_time)
-        
-        print(f'Lap {len(self.lap_times)} time at: {curr_lap_time}')
-        print(f'Lap {len(self.lap_times)} time: {latest_lap_elapsed_time}')
-
-    def show(self):
-        print('###############################')
-        print(f'Timer: {self.name}')          
-        if len(self.lap_times) > 0:
-            for i, lap_time in enumerate(self.lap_times):
-                
-                if i == 0:
-                    curr_lap_elapsed_time = lap_time - self.start_time
-                else:
-                    curr_lap_elapsed_time = lap_time - prev_lap_time
-                prev_lap_time = lap_time                
-                [print(f'Lap {i+1} elapsed time: {curr_lap_elapsed_time}')]
-            print(f'Lap {i+2} elapsed time: {self.end_time - prev_lap_time}')
-            
-        print(f'Total elapsed time: {self.elapsed_time}')
-        print('###############################')
-
-timer_1 = timer('Test')
+import datetime
+
+class timer:
+  
+    def __init__(self, name):
+        self.name = name
+        self.start_time = None
+        self.end_time = None
+        self.lap_times = []
+        self.elapsed_time = None
+
+    def start(self):
+        self.start_time = datetime.datetime.now()
+        print(f'Start at: {self.start_time}')
+
+    def end(self):
+        self.end_time = datetime.datetime.now()        
+        print(f'End at: {self.end_time}')
+        self.elapsed_time = self.end_time - self.start_time
+        print()
+        self.show()
+
+    def lap(self):
+        curr_lap_time = datetime.datetime.now()
+        if len(self.lap_times) > 0:
+            prev_lap_time = self.lap_times[-1]
+        else:
+            prev_lap_time = self.start_time
+        latest_lap_elapsed_time = curr_lap_time - prev_lap_time
+        self.lap_times.append(curr_lap_time)
+        
+        print(f'Lap {len(self.lap_times)} time at: {curr_lap_time}')
+        print(f'Lap {len(self.lap_times)} time: {latest_lap_elapsed_time}')
+
+    def show(self):
+        print('###############################')
+        print(f'Timer: {self.name}')          
+        if len(self.lap_times) > 0:
+            for i, lap_time in enumerate(self.lap_times):
+                
+                if i == 0:
+                    curr_lap_elapsed_time = lap_time - self.start_time
+                else:
+                    curr_lap_elapsed_time = lap_time - prev_lap_time
+                prev_lap_time = lap_time                
+                [print(f'Lap {i+1} elapsed time: {curr_lap_elapsed_time}')]
+            print(f'Lap {i+2} elapsed time: {self.end_time - prev_lap_time}')
+            
+        print(f'Total elapsed time: {self.elapsed_time}')
+        print('###############################')
+
+timer_1 = timer('Test')
```

### Comparing `zkyhaxpy-0.3.0.2.0/zkyhaxpy/util_tools.py` & `zkyhaxpy-0.3.1.0.1/zkyhaxpy/util_tools.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-import os
-import psutil
-import time
-
-def wait_mem(max_mem_pct_used=60, refresh_mins=5, timeout_mins=180):
-
-    mem_pct_used = psutil.virtual_memory()[2]
-    waiting_mins = 0
-    #print(f'current memory usage : {mem_pct_used}%')
-    while mem_pct_used > max_mem_pct_used:     
-        print(f'Current memory usage : {mem_pct_used}%... wait for {refresh_mins} mins...')   
-        time.sleep(60*refresh_mins)
-        waiting_mins = waiting_mins + (refresh_mins)
-        mem_pct_used = psutil.virtual_memory()[2]
-            
-        if mem_pct_used <= max_mem_pct_used:
-            print('Continue...')
-        assert(waiting_mins < timeout_mins)
+import os
+import psutil
+import time
+
+def wait_mem(max_mem_pct_used=60, refresh_mins=5, timeout_mins=180):
+
+    mem_pct_used = psutil.virtual_memory()[2]
+    waiting_mins = 0
+    #print(f'current memory usage : {mem_pct_used}%')
+    while mem_pct_used > max_mem_pct_used:     
+        print(f'Current memory usage : {mem_pct_used}%... wait for {refresh_mins} mins...')   
+        time.sleep(60*refresh_mins)
+        waiting_mins = waiting_mins + (refresh_mins)
+        mem_pct_used = psutil.virtual_memory()[2]
+            
+        if mem_pct_used <= max_mem_pct_used:
+            print('Continue...')
+        assert(waiting_mins < timeout_mins)
```

### Comparing `zkyhaxpy-0.3.0.2.0/zkyhaxpy.egg-info/PKG-INFO` & `zkyhaxpy-0.3.1.0.1/zkyhaxpy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 Metadata-Version: 2.1
 Name: zkyhaxpy
-Version: 0.3.0.2.0
+Version: 0.3.1.0.1
 Summary: A swiss-knife Data Science package for python
 Home-page: https://github.com/surasakcho/zkyhaxpy
 Author: Surasak Choedpasuporn
 Author-email: surasak.cho@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is zkyhaxpy package.
 zkyhaxpy is a python package for personal usage.
 It provides a lot of useful tools for working as data scientist.
-
```

### Comparing `zkyhaxpy-0.3.0.2.0/zkyhaxpy.egg-info/SOURCES.txt` & `zkyhaxpy-0.3.1.0.1/zkyhaxpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

