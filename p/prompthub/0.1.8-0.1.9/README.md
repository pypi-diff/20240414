# Comparing `tmp/prompthub-0.1.8-py3-none-any.whl.zip` & `tmp/prompthub-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4194 bytes, number of entries: 7
+Zip file size: 4218 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       69 b- defN 24-Feb-21 07:06 prompthub/__init__.py
--rw-r--r--  2.0 unx      678 b- defN 24-Feb-19 11:06 prompthub/errors.py
--rw-r--r--  2.0 unx     5961 b- defN 24-Feb-21 07:09 prompthub/hub.py
--rw-r--r--  2.0 unx     1575 b- defN 24-Feb-21 07:09 prompthub-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-21 07:09 prompthub-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 24-Feb-21 07:09 prompthub-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      530 b- defN 24-Feb-21 07:09 prompthub-0.1.8.dist-info/RECORD
-7 files, 8915 bytes uncompressed, 3256 bytes compressed:  63.5%
+-rw-r--r--  2.0 unx      729 b- defN 24-Feb-21 14:43 prompthub/errors.py
+-rw-r--r--  2.0 unx     6056 b- defN 24-Feb-21 14:43 prompthub/hub.py
+-rw-r--r--  2.0 unx     1575 b- defN 24-Feb-21 14:43 prompthub-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Feb-21 14:43 prompthub-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-Feb-21 14:43 prompthub-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      530 b- defN 24-Feb-21 14:43 prompthub-0.1.9.dist-info/RECORD
+7 files, 9061 bytes uncompressed, 3280 bytes compressed:  63.8%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: prompthub/errors.py
 Comment: 
 
 Filename: prompthub/hub.py
 Comment: 
 
-Filename: prompthub-0.1.8.dist-info/METADATA
+Filename: prompthub-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: prompthub-0.1.8.dist-info/WHEEL
+Filename: prompthub-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: prompthub-0.1.8.dist-info/top_level.txt
+Filename: prompthub-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: prompthub-0.1.8.dist-info/RECORD
+Filename: prompthub-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## prompthub/errors.py

```diff
@@ -3,14 +3,16 @@
 
 class CategoryNotFoundError(PromptsHubError):
     pass
 
 class ConnectionError(PromptsHubError):
     pass
 
+class UnauthorizedError(PromptsHubError):
+    pass
 
 class NotFoundError(PromptsHubError):
     pass
 
 class CategoryNotFoundError(PromptsHubError):
     pass
```

## prompthub/hub.py

```diff
@@ -30,14 +30,16 @@
             response.raise_for_status()
             return response.json()
         except requests.exceptions.ConnectionError:
             raise errors.ConnectionError
         except requests.exceptions.HTTPError as e:
             if e.response.status_code == 404:
                 raise errors.NotFoundError
+            elif e.response.status_code == 401:
+                raise errors.UnauthorizedError
             else:
                 raise errors.PromptsHubError(e)
 
 
 class Prompt:
     def __init__(self, content: str, output_format: str, model: Optional[str] = None):
         self.content = content
```

## Comparing `prompthub-0.1.8.dist-info/METADATA` & `prompthub-0.1.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompthub
-Version: 0.1.8
+Version: 0.1.9
 Summary: Prompt Hub SDK.
 Home-page: https://github.com/DataMini/prompt-hub
 Author: lele
 Description-Content-Type: text/markdown
 Requires-Dist: jinja2
 
 ```python
```

## Comparing `prompthub-0.1.8.dist-info/RECORD` & `prompthub-0.1.9.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 prompthub/__init__.py,sha256=gpKajy_LkNlz6R8ka0EP7tXpWqSi3yaSuiHlNcVUOUQ,69
-prompthub/errors.py,sha256=texhGCgdgoqnfx5vH7pHDNjcjePYK904idQUJOHZvZk,678
-prompthub/hub.py,sha256=pmNN8gPY8yWNTFyaf_ihGoF7MwgY4hm1qFyZcon_4RQ,5961
-prompthub-0.1.8.dist-info/METADATA,sha256=lcjVEQ_r1TmO3Vq2gL6nNM3ISGoQxf-WqVejkp4unjk,1575
-prompthub-0.1.8.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-prompthub-0.1.8.dist-info/top_level.txt,sha256=V04Ws6mofRYrFoBHLPJ2sgDqzWbD-bEMPQ9WgXLV9is,10
-prompthub-0.1.8.dist-info/RECORD,,
+prompthub/errors.py,sha256=u66WvIIHhRDMSBBIMe-ZkIMsEqDqXVSWg_Qv52xZP-E,729
+prompthub/hub.py,sha256=CVEGdOY78MwsAwa67rYK9YgWqF3GSxR5y-EP5CXXs6I,6056
+prompthub-0.1.9.dist-info/METADATA,sha256=PGg_ZjYg2uRg_XFmnDWVbr_DK_5qbHP4ehxbn0AV_9o,1575
+prompthub-0.1.9.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+prompthub-0.1.9.dist-info/top_level.txt,sha256=V04Ws6mofRYrFoBHLPJ2sgDqzWbD-bEMPQ9WgXLV9is,10
+prompthub-0.1.9.dist-info/RECORD,,
```

