# Comparing `tmp/supabase-2.4.1.tar.gz` & `tmp/supabase-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supabase-2.4.1.tar", max compression
+gzip compressed data, was "supabase-2.4.2.tar", max compression
```

## Comparing `supabase-2.4.1.tar` & `supabase-2.4.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1067 2024-03-26 22:13:04.558255 supabase-2.4.1/LICENSE
--rw-r--r--   0        0        0     8244 2024-03-26 22:13:04.558255 supabase-2.4.1/README.md
--rw-r--r--   0        0        0     1918 2024-03-26 22:13:10.246214 supabase-2.4.1/pyproject.toml
--rw-r--r--   0        0        0      751 2024-03-26 22:13:04.558255 supabase-2.4.1/supabase/__init__.py
--rw-r--r--   0        0        0       22 2024-03-26 22:13:10.246214 supabase-2.4.1/supabase/__version__.py
--rw-r--r--   0        0        0       35 2024-03-26 22:13:04.558255 supabase-2.4.1/supabase/_async/__init__.py
--rw-r--r--   0        0        0     1130 2024-03-26 22:13:04.558255 supabase-2.4.1/supabase/_async/auth_client.py
--rw-r--r--   0        0        0    10668 2024-03-26 22:13:04.558255 supabase-2.4.1/supabase/_async/client.py
--rw-r--r--   0        0        0       35 2024-03-26 22:13:04.558255 supabase-2.4.1/supabase/_sync/__init__.py
--rw-r--r--   0        0        0     1120 2024-03-26 22:13:04.558255 supabase-2.4.1/supabase/_sync/auth_client.py
--rw-r--r--   0        0        0    10610 2024-03-26 22:13:04.558255 supabase-2.4.1/supabase/_sync/client.py
--rw-r--r--   0        0        0      772 2024-03-26 22:13:04.558255 supabase-2.4.1/supabase/client.py
--rw-r--r--   0        0        0      127 2024-03-26 22:13:04.558255 supabase-2.4.1/supabase/lib/__init__.py
--rw-r--r--   0        0        0     3133 2024-03-26 22:13:04.558255 supabase-2.4.1/supabase/lib/client_options.py
--rw-r--r--   0        0        0     1892 2024-03-26 22:13:04.558255 supabase-2.4.1/supabase/lib/realtime_client.py
--rw-r--r--   0        0        0        0 2024-03-26 22:13:04.558255 supabase-2.4.1/supabase/py.typed
--rw-r--r--   0        0        0     9315 1970-01-01 00:00:00.000000 supabase-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-14 00:32:56.096397 supabase-2.4.2/LICENSE
+-rw-r--r--   0        0        0     8244 2024-04-14 00:32:56.096397 supabase-2.4.2/README.md
+-rw-r--r--   0        0        0     1892 2024-04-14 00:33:01.912412 supabase-2.4.2/pyproject.toml
+-rw-r--r--   0        0        0      751 2024-04-14 00:32:56.096397 supabase-2.4.2/supabase/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-14 00:33:01.912412 supabase-2.4.2/supabase/__version__.py
+-rw-r--r--   0        0        0       35 2024-04-14 00:32:56.096397 supabase-2.4.2/supabase/_async/__init__.py
+-rw-r--r--   0        0        0     1130 2024-04-14 00:32:56.096397 supabase-2.4.2/supabase/_async/auth_client.py
+-rw-r--r--   0        0        0    10713 2024-04-14 00:32:56.096397 supabase-2.4.2/supabase/_async/client.py
+-rw-r--r--   0        0        0       35 2024-04-14 00:32:56.096397 supabase-2.4.2/supabase/_sync/__init__.py
+-rw-r--r--   0        0        0     1120 2024-04-14 00:32:56.096397 supabase-2.4.2/supabase/_sync/auth_client.py
+-rw-r--r--   0        0        0    10656 2024-04-14 00:32:56.096397 supabase-2.4.2/supabase/_sync/client.py
+-rw-r--r--   0        0        0      772 2024-04-14 00:32:56.096397 supabase-2.4.2/supabase/client.py
+-rw-r--r--   0        0        0      127 2024-04-14 00:32:56.096397 supabase-2.4.2/supabase/lib/__init__.py
+-rw-r--r--   0        0        0     3133 2024-04-14 00:32:56.096397 supabase-2.4.2/supabase/lib/client_options.py
+-rw-r--r--   0        0        0     1892 2024-04-14 00:32:56.096397 supabase-2.4.2/supabase/lib/realtime_client.py
+-rw-r--r--   0        0        0        0 2024-04-14 00:32:56.096397 supabase-2.4.2/supabase/py.typed
+-rw-r--r--   0        0        0     9313 1970-01-01 00:00:00.000000 supabase-2.4.2/PKG-INFO
```

### Comparing `supabase-2.4.1/LICENSE` & `supabase-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `supabase-2.4.1/README.md` & `supabase-2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `supabase-2.4.1/pyproject.toml` & `supabase-2.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "supabase"
-version = "2.4.1"
+version = "2.4.2"
 description = "Supabase client for Python."
 authors = ["Joel Lee <joel@joellee.org>", "Leon Fedden <leonfedden@gmail.com>", "Daniel Reinón García <danielreinon@outlook.com>", "Leynier Gutiérrez González <leynier41@gmail.com>", "Anand", "Andrew Smith <a.smith@silentworks.co.uk>"]
 homepage = "https://github.com/supabase-community/supabase-py"
 repository = "https://github.com/supabase-community/supabase-py"
 documentation = "https://github.com/supabase-community/supabase-py"
 readme = "README.md"
 license = "MIT"
@@ -12,38 +12,37 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-postgrest = ">=0.10.8,<0.17.0"
+postgrest = ">=0.14,<0.17.0"
 realtime = "^1.0.0"
 gotrue = ">=1.3,<3.0"
 httpx = ">=0.24,<0.28"
 storage3 = ">=0.5.3,<0.8.0"
 supafunc = ">=0.3.1,<0.5.0"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^3.5.0"
-black = "^24.3"
+black = "^24.4"
 pytest = "^8.1.1"
 flake8 = "^5.0.4"
 isort = "^5.10.1"
 pytest-cov = "^5.0.0"
-commitizen = "^3.20.0"
-python-semantic-release = "^9.3.1"
+commitizen = "^3.22.0"
+python-semantic-release = "^9.4.1"
 python-dotenv = "^1.0.1"
 
 [tool.poetry.scripts]
 tests = 'poetry_scripts:run_tests'
 
 [tool.poetry.group.dev.dependencies]
 unasync-cli = "^0.0.9"
-mdformat-gfm = "^0.3.6"
 
 [tool.semantic_release]
 version_variables = ["supabase/__version__.py:__version__"]
 version_toml = ["pyproject.toml:tool.poetry.version"]
 major_on_zero = false
 commit_message = "chore(release): bump version to v{version}"
 build_command = "curl -sSL https://install.python-poetry.org | python - --preview && export PATH=\"/github/home/.local/bin:$PATH\" && poetry install && poetry build"
```

### Comparing `supabase-2.4.1/supabase/__init__.py` & `supabase-2.4.2/supabase/__init__.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.1/supabase/_async/auth_client.py` & `supabase-2.4.2/supabase/_async/auth_client.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.1/supabase/_async/client.py` & `supabase-2.4.2/supabase/_async/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 class AsyncClient:
     """Supabase client class."""
 
     def __init__(
         self,
         supabase_url: str,
         supabase_key: str,
-        options: ClientOptions = ClientOptions(storage=AsyncMemoryStorage()),
+        options: Union[ClientOptions, None] = None,
     ):
         """Instantiate the client.
 
         Parameters
         ----------
         supabase_url: str
             The URL to the Supabase instance that should be connected to.
@@ -58,14 +58,17 @@
 
         # Check if the key is a valid JWT
         if not re.match(
             r"^[A-Za-z0-9-_=]+\.[A-Za-z0-9-_=]+\.?[A-Za-z0-9-_.+/=]*$", supabase_key
         ):
             raise SupabaseException("Invalid API key")
 
+        if options is None:
+            options = ClientOptions(storage=AsyncMemoryStorage())
+
         self.supabase_url = supabase_url
         self.supabase_key = supabase_key
         self._auth_token = {
             "Authorization": f"Bearer {supabase_key}",
         }
         options.headers.update(self._get_auth_headers())
         self.options = options
@@ -93,15 +96,15 @@
         self.auth.on_auth_state_change(self._listen_to_auth_events)
 
     @classmethod
     async def create(
         cls,
         supabase_url: str,
         supabase_key: str,
-        options: ClientOptions = ClientOptions(),
+        options: Union[ClientOptions, None] = None,
     ):
         client = cls(supabase_url, supabase_key, options)
         client._auth_token = await client._get_token_header()
         return client
 
     def table(self, table_name: str) -> AsyncRequestBuilder:
         """Perform a table operation.
@@ -278,15 +281,15 @@
 
         self._auth_token = self._create_auth_header(access_token)
 
 
 async def create_client(
     supabase_url: str,
     supabase_key: str,
-    options: ClientOptions = ClientOptions(storage=AsyncMemoryStorage()),
+    options: Union[ClientOptions, None] = None,
 ) -> AsyncClient:
     """Create client function to instantiate supabase client like JS runtime.
 
     Parameters
     ----------
     supabase_url: str
         The URL to the Supabase instance that should be connected to.
```

### Comparing `supabase-2.4.1/supabase/_sync/auth_client.py` & `supabase-2.4.2/supabase/_sync/auth_client.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.1/supabase/_sync/client.py` & `supabase-2.4.2/supabase/_sync/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 class SyncClient:
     """Supabase client class."""
 
     def __init__(
         self,
         supabase_url: str,
         supabase_key: str,
-        options: ClientOptions = ClientOptions(storage=SyncMemoryStorage()),
+        options: Union[ClientOptions, None] = None,
     ):
         """Instantiate the client.
 
         Parameters
         ----------
         supabase_url: str
             The URL to the Supabase instance that should be connected to.
@@ -58,14 +58,17 @@
 
         # Check if the key is a valid JWT
         if not re.match(
             r"^[A-Za-z0-9-_=]+\.[A-Za-z0-9-_=]+\.?[A-Za-z0-9-_.+/=]*$", supabase_key
         ):
             raise SupabaseException("Invalid API key")
 
+        if options is None:
+            options = ClientOptions(storage=SyncMemoryStorage())
+
         self.supabase_url = supabase_url
         self.supabase_key = supabase_key
         self._auth_token = {
             "Authorization": f"Bearer {supabase_key}",
         }
         options.headers.update(self._get_auth_headers())
         self.options = options
@@ -93,15 +96,15 @@
         self.auth.on_auth_state_change(self._listen_to_auth_events)
 
     @classmethod
     def create(
         cls,
         supabase_url: str,
         supabase_key: str,
-        options: ClientOptions = ClientOptions(),
+        options: Union[ClientOptions, None] = None,
     ):
         client = cls(supabase_url, supabase_key, options)
         client._auth_token = client._get_token_header()
         return client
 
     def table(self, table_name: str) -> SyncRequestBuilder:
         """Perform a table operation.
@@ -278,15 +281,15 @@
 
         self._auth_token = self._create_auth_header(access_token)
 
 
 def create_client(
     supabase_url: str,
     supabase_key: str,
-    options: ClientOptions = ClientOptions(storage=SyncMemoryStorage()),
+    options: Union[ClientOptions, None] = None,
 ) -> SyncClient:
     """Create client function to instantiate supabase client like JS runtime.
 
     Parameters
     ----------
     supabase_url: str
         The URL to the Supabase instance that should be connected to.
```

### Comparing `supabase-2.4.1/supabase/client.py` & `supabase-2.4.2/supabase/client.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.1/supabase/lib/client_options.py` & `supabase-2.4.2/supabase/lib/client_options.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.1/supabase/lib/realtime_client.py` & `supabase-2.4.2/supabase/lib/realtime_client.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.1/PKG-INFO` & `supabase-2.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supabase
-Version: 2.4.1
+Version: 2.4.2
 Summary: Supabase client for Python.
 Home-page: https://github.com/supabase-community/supabase-py
 License: MIT
 Author: Joel Lee
 Author-email: joel@joellee.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: gotrue (>=1.3,<3.0)
 Requires-Dist: httpx (>=0.24,<0.28)
-Requires-Dist: postgrest (>=0.10.8,<0.17.0)
+Requires-Dist: postgrest (>=0.14,<0.17.0)
 Requires-Dist: realtime (>=1.0.0,<2.0.0)
 Requires-Dist: storage3 (>=0.5.3,<0.8.0)
 Requires-Dist: supafunc (>=0.3.1,<0.5.0)
 Project-URL: Documentation, https://github.com/supabase-community/supabase-py
 Project-URL: Repository, https://github.com/supabase-community/supabase-py
 Description-Content-Type: text/markdown
```

