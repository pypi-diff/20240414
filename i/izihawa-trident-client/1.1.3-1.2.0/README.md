# Comparing `tmp/izihawa_trident_client-1.1.3.tar.gz` & `tmp/izihawa_trident_client-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "izihawa_trident_client-1.1.3.tar", max compression
+gzip compressed data, was "izihawa_trident_client-1.2.0.tar", max compression
```

## Comparing `izihawa_trident_client-1.1.3.tar` & `izihawa_trident_client-1.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       64 2023-12-10 19:54:01.661696 izihawa_trident_client-1.1.3/README.md
--rw-r--r--   0        0        0      348 2024-03-09 19:35:39.344298 izihawa_trident_client-1.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-19 06:00:51.101322 izihawa_trident_client-1.1.3/trident/__init__.py
--rw-r--r--   0        0        0     4483 2024-03-09 19:35:34.102106 izihawa_trident_client-1.1.3/trident/client.py
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 izihawa_trident_client-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0       64 2023-12-10 19:54:01.661696 izihawa_trident_client-1.2.0/README.md
+-rw-r--r--   0        0        0      348 2024-04-14 17:14:42.598735 izihawa_trident_client-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-19 06:00:51.101322 izihawa_trident_client-1.2.0/trident/__init__.py
+-rw-r--r--   0        0        0     4381 2024-04-14 17:13:23.892915 izihawa_trident_client-1.2.0/trident/client.py
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 izihawa_trident_client-1.2.0/PKG-INFO
```

### Comparing `izihawa_trident_client-1.1.3/trident/client.py` & `izihawa_trident_client-1.2.0/trident/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,22 +13,14 @@
             data = await response.read()
             if hasattr(response, "request"):
                 raise ExternalServiceError(response.request.url, response.status, data)
             else:
                 raise ExternalServiceError(None, response.status, data)
         return response
 
-    async def sinks_ls(self) -> dict:
-        response = await self.get(f"/sinks/")
-        return await response.json()
-
-    async def sinks_create(self, sink: str, config: dict) -> dict:
-        response = await self.post(f"/sinks/{sink}/", json=config)
-        return await response.read()
-
     async def tables_ls(self) -> dict:
         response = await self.get(f"/tables/")
         return await response.json()
 
     async def tables_create(self, table: str, storage: str) -> bytes:
         url = f"/tables/{table}/"
         response = await self.post(url, params={'storage': storage})
@@ -44,26 +36,22 @@
 
     async def tables_import(
         self,
         table: str,
         ticket: str,
         storage: str,
         download_policy: dict | None = None,
-        sinks: tuple | list = tuple(),
-        keep_blob: bool = True,
     ) -> bytes:
         url = f"/tables/{table}/import/"
         response = await self.post(
             url,
             json={
                 'ticket': ticket,
                 'storage': storage,
                 'download_policy': download_policy,
-                'sinks': sinks,
-                'keep_blob': keep_blob,
             },
         )
         return await response.read()
 
     async def tables_sync(
         self,
         table: str,
@@ -103,29 +91,38 @@
             'from_table': from_table,
             'from_key': from_key,
             'to_table': to_table,
             'to_key': to_key,
         })
         return await response.read()
 
-    async def table_get(self, table: str, key: str, timeout: float = None) -> bytes | None:
+    async def table_get(self, table: str, key: str, timeout: float = None) -> dict | None:
         url = f"/tables/{table}/{key}"
         response = await self.get(url, timeout=timeout)
         if response is None:
             return None
-        return await response.read()
+        content = await response.read()
+        return {
+            'iroh_hash': response.headers['X-Iroh-Hash'],
+            'size': response.headers['Content-Length'],
+            'content': content
+        }
 
     async def table_get_chunks(self, table: str, key: str, timeout: float = None) -> AsyncGenerator[bytes, None]:
         url = f"/tables/{table}/{key}"
         response = await self.get(url, timeout=timeout)
         async for data, _ in response.content.iter_chunks():
             yield data
 
     async def table_ls(self, table) -> typing.AsyncGenerator[str, None]:
         response = await self.get(f"/tables/{table}/")
         async for line in response.content:
             yield line.decode()[:-1]
 
-    async def table_exists(self, table: str, key: str) -> bool:
+    async def table_exists(self, table: str, key: str) -> dict | None:
         url = f"/tables/{table}/{key}"
         response = await self.head(url)
-        return response is not None
+        if response is not None:
+            return {
+                'iroh_hash': response.headers['X-Iroh-Hash'],
+                'size': response.headers['Content-Length'],
+            }
```

### Comparing `izihawa_trident_client-1.1.3/PKG-INFO` & `izihawa_trident_client-1.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: izihawa-trident-client
-Version: 1.1.3
+Version: 1.2.0
 Summary: 
 Author: Pasha Podolsky
 Author-email: ppodolsky@me.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

