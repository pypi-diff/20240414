# Comparing `tmp/chaturbate_poller-0.3.8.tar.gz` & `tmp/chaturbate_poller-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaturbate_poller-0.3.8.tar", max compression
+gzip compressed data, was "chaturbate_poller-0.3.9.tar", max compression
```

## Comparing `chaturbate_poller-0.3.8.tar` & `chaturbate_poller-0.3.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0     1071 2024-04-11 16:04:32.008994 chaturbate_poller-0.3.8/LICENSE
--rw-r--r--   0        0        0     2692 2024-04-11 16:04:32.008994 chaturbate_poller-0.3.8/README.md
--rw-r--r--   0        0        0     3129 2024-04-11 16:04:42.441065 chaturbate_poller-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      573 2024-04-11 16:04:32.012994 chaturbate_poller-0.3.8/src/chaturbate_poller/__init__.py
--rw-r--r--   0        0        0     4286 2024-04-11 16:04:32.012994 chaturbate_poller-0.3.8/src/chaturbate_poller/chaturbate_poller.py
--rw-r--r--   0        0        0     1762 2024-04-11 16:04:32.012994 chaturbate_poller-0.3.8/src/chaturbate_poller/constants.py
--rw-r--r--   0        0        0     4017 2024-04-11 16:04:32.012994 chaturbate_poller-0.3.8/src/chaturbate_poller/format_messages.py
--rw-r--r--   0        0        0     1564 2024-04-11 16:04:32.012994 chaturbate_poller-0.3.8/src/chaturbate_poller/logging_config.py
--rw-r--r--   0        0        0     4877 2024-04-11 16:04:32.012994 chaturbate_poller-0.3.8/src/chaturbate_poller/models.py
--rw-r--r--   0        0        0     3585 1970-01-01 00:00:00.000000 chaturbate_poller-0.3.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1071 2024-04-11 18:03:50.913418 chaturbate_poller-0.3.9/LICENSE
+-rw-r--r--   0        0        0     2692 2024-04-11 18:03:50.913418 chaturbate_poller-0.3.9/README.md
+-rw-r--r--   0        0        0     3129 2024-04-11 18:04:01.681475 chaturbate_poller-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0      573 2024-04-11 18:03:50.917418 chaturbate_poller-0.3.9/src/chaturbate_poller/__init__.py
+-rw-r--r--   0        0        0     4623 2024-04-11 18:03:50.917418 chaturbate_poller-0.3.9/src/chaturbate_poller/chaturbate_poller.py
+-rw-r--r--   0        0        0     1762 2024-04-11 18:03:50.917418 chaturbate_poller-0.3.9/src/chaturbate_poller/constants.py
+-rw-r--r--   0        0        0     4017 2024-04-11 18:03:50.917418 chaturbate_poller-0.3.9/src/chaturbate_poller/format_messages.py
+-rw-r--r--   0        0        0     1564 2024-04-11 18:03:50.917418 chaturbate_poller-0.3.9/src/chaturbate_poller/logging_config.py
+-rw-r--r--   0        0        0     4877 2024-04-11 18:03:50.917418 chaturbate_poller-0.3.9/src/chaturbate_poller/models.py
+-rw-r--r--   0        0        0     3585 1970-01-01 00:00:00.000000 chaturbate_poller-0.3.9/PKG-INFO
```

### Comparing `chaturbate_poller-0.3.8/LICENSE` & `chaturbate_poller-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.8/README.md` & `chaturbate_poller-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.8/pyproject.toml` & `chaturbate_poller-0.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chaturbate-poller"
-version = "0.3.8"
+version = "0.3.9"
 description = "Poller for the Chaturbate events API."
 authors = ["MountainGod2"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/MountainGod2/chaturbate_poller"
 documentation = "https://mountaingod2.github.io/chaturbate_poller/"
```

### Comparing `chaturbate_poller-0.3.8/src/chaturbate_poller/__init__.py` & `chaturbate_poller-0.3.9/src/chaturbate_poller/__init__.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.8/src/chaturbate_poller/chaturbate_poller.py` & `chaturbate_poller-0.3.9/src/chaturbate_poller/chaturbate_poller.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,15 +101,22 @@
 
         Returns:
             EventsAPIResponse: The events API response.
         """
         if url is None:
             url = self._construct_url()
         response = await self.client.get(url, timeout=self.timeout)
-        response.raise_for_status()
+        try:
+            response.raise_for_status()
+        except httpx.HTTPStatusError as e:
+            if e.response.status_code == HttpStatusCode.UNAUTHORIZED:
+                error_message = "Unauthorized access. Verify the username and token."
+                logger.exception(error_message)
+                raise ValueError(error_message) from e
+            raise
         return EventsAPIResponse.model_validate(response.json())
 
     def _construct_url(self) -> str:
         """Construct URL with username, token, and timeout.
 
         Returns:
             str: The constructed URL.
```

### Comparing `chaturbate_poller-0.3.8/src/chaturbate_poller/constants.py` & `chaturbate_poller-0.3.9/src/chaturbate_poller/constants.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.8/src/chaturbate_poller/format_messages.py` & `chaturbate_poller-0.3.9/src/chaturbate_poller/format_messages.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.8/src/chaturbate_poller/logging_config.py` & `chaturbate_poller-0.3.9/src/chaturbate_poller/logging_config.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.8/src/chaturbate_poller/models.py` & `chaturbate_poller-0.3.9/src/chaturbate_poller/models.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.8/PKG-INFO` & `chaturbate_poller-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaturbate-poller
-Version: 0.3.8
+Version: 0.3.9
 Summary: Poller for the Chaturbate events API.
 Home-page: https://github.com/MountainGod2/chaturbate_poller
 License: MIT
 Author: MountainGod2
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

