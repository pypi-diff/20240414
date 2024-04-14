# Comparing `tmp/nacl_middleware-0.0.2.tar.gz` & `tmp/nacl_middleware-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nacl_middleware-0.0.2.tar", last modified: Mon Apr  8 15:50:01 2024, max compression
+gzip compressed data, was "nacl_middleware-0.0.3.tar", last modified: Sun Apr 14 02:21:03 2024, max compression
```

## Comparing `nacl_middleware-0.0.2.tar` & `nacl_middleware-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-08 15:50:01.080959 nacl_middleware-0.0.2/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3243 2024-04-08 15:50:01.080959 nacl_middleware-0.0.2/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1959 2024-04-08 11:47:04.000000 nacl_middleware-0.0.2/README.md
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-08 15:50:01.070959 nacl_middleware-0.0.2/nacl_middleware/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      113 2024-04-08 14:48:22.000000 nacl_middleware-0.0.2/nacl_middleware/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3681 2024-04-08 14:48:22.000000 nacl_middleware-0.0.2/nacl_middleware/nacl_middleware.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1351 2024-04-08 14:48:22.000000 nacl_middleware-0.0.2/nacl_middleware/nacl_utils.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      257 2024-04-08 14:48:22.000000 nacl_middleware-0.0.2/nacl_middleware/utils.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-08 15:50:01.070959 nacl_middleware-0.0.2/nacl_middleware.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3243 2024-04-08 15:50:01.000000 nacl_middleware-0.0.2/nacl_middleware.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      357 2024-04-08 15:50:01.000000 nacl_middleware-0.0.2/nacl_middleware.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2024-04-08 15:50:01.000000 nacl_middleware-0.0.2/nacl_middleware.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)      110 2024-04-08 15:50:01.000000 nacl_middleware-0.0.2/nacl_middleware.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       16 2024-04-08 15:50:01.000000 nacl_middleware-0.0.2/nacl_middleware.egg-info/top_level.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1207 2024-04-08 15:48:52.000000 nacl_middleware-0.0.2/pyproject.toml
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2024-04-08 15:50:01.080959 nacl_middleware-0.0.2/setup.cfg
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-08 15:50:01.070959 nacl_middleware-0.0.2/tests/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1103 2024-04-08 14:48:22.000000 nacl_middleware-0.0.2/tests/test_server.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-14 02:21:03.915906 nacl_middleware-0.0.3/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8625 2024-04-14 02:21:03.915906 nacl_middleware-0.0.3/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7008 2024-04-14 01:42:39.000000 nacl_middleware-0.0.3/README.rst
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-14 02:21:03.905906 nacl_middleware-0.0.3/nacl_middleware/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      113 2024-04-13 19:29:25.000000 nacl_middleware-0.0.3/nacl_middleware/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5014 2024-04-14 00:46:30.000000 nacl_middleware-0.0.3/nacl_middleware/nacl_middleware.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2999 2024-04-14 00:46:30.000000 nacl_middleware-0.0.3/nacl_middleware/nacl_utils.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      570 2024-04-14 00:46:30.000000 nacl_middleware-0.0.3/nacl_middleware/utils.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-14 02:21:03.915906 nacl_middleware-0.0.3/nacl_middleware.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8625 2024-04-14 02:21:03.000000 nacl_middleware-0.0.3/nacl_middleware.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      358 2024-04-14 02:21:03.000000 nacl_middleware-0.0.3/nacl_middleware.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2024-04-14 02:21:03.000000 nacl_middleware-0.0.3/nacl_middleware.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      211 2024-04-14 02:21:03.000000 nacl_middleware-0.0.3/nacl_middleware.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       16 2024-04-14 02:21:03.000000 nacl_middleware-0.0.3/nacl_middleware.egg-info/top_level.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1361 2024-04-14 02:20:08.000000 nacl_middleware-0.0.3/pyproject.toml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2024-04-14 02:21:03.915906 nacl_middleware-0.0.3/setup.cfg
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-14 02:21:03.905906 nacl_middleware-0.0.3/tests/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1698 2024-04-14 00:46:30.000000 nacl_middleware-0.0.3/tests/test_server.py
```

### Comparing `nacl_middleware-0.0.2/nacl_middleware/nacl_middleware.py` & `nacl_middleware-0.0.3/nacl_middleware/nacl_middleware.py`

 * *Files 26% similar despite different names*

```diff
@@ -25,29 +25,67 @@
 
 def nacl_middleware(
     private_key: PrivateKey,
     exclude_routes: Tuple = tuple(),
     exclude_methods: Tuple = tuple(),
     log=getLogger(),
 ) -> Middleware:
+    """
+    Middleware function that handles NaCl encryption and decryption.
+
+    Args:
+        private_key (PrivateKey): The private key used for decryption.
+        exclude_routes (Tuple, optional): Tuple of routes to exclude from encryption/decryption. Defaults to an empty tuple.
+        exclude_methods (Tuple, optional): Tuple of HTTP methods to exclude from encryption/decryption. Defaults to an empty tuple.
+        log (Logger, optional): Logger object for logging debug messages. Defaults to getLogger().
+
+    Returns:
+        Middleware: The middleware function.
+
+    """
 
     def nacl_decryptor(public_key, encrypted_message) -> Tuple[any, MailBox]:
+        """
+        Decrypts the encrypted message using the public key.
+
+        Args:
+            public_key: The public key used for encryption.
+            encrypted_message: The encrypted message to decrypt.
+
+        Returns:
+            Tuple[any, MailBox]: A tuple containing the decrypted message and the MailBox object.
+
+        """
         if public_key in mailBoxes:
             my_mail_box = mailBoxes[public_key]
         else:
             my_mail_box = MailBox(private_key, public_key)
             mailBoxes[public_key] = my_mail_box
 
         log.debug("Decrypting message...")
         message = my_mail_box.unbox(encrypted_message)
         log.debug(f"Message {message} decrypted!")
         return message, my_mail_box
 
     @middleware
     async def returned_middleware(request: Request, handler: Handler) -> StreamResponse:
+        """
+        Middleware function that processes the incoming request and handles exceptions.
+
+        Args:
+            request (Request): The incoming request object.
+            handler (Handler): The handler function to be called.
+
+        Returns:
+            StreamResponse: The response object.
+
+        Raises:
+            HTTPUnauthorized: If a valid message cannot be retrieved.
+
+        """
         if not (
             is_exclude(request, exclude_routes) or request.method in exclude_methods
         ):
 
             try:
                 log.debug("Retrieving publicKey and encryptedMessage from message...")
                 publicKey, encryptedMessage = itemgetter(
```

### Comparing `nacl_middleware-0.0.2/pyproject.toml` & `nacl_middleware-0.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Declare the build backend (required)
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools"]
 
 [project]
 name = "nacl_middleware"
-version = "0.0.2"
+version = "0.0.3"
 description = "aiohttp compatible pynacl middleware"
 license = { text = "GNU General Public License v3 or later (GPLv3+)" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Plugins",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
@@ -24,25 +24,35 @@
 ]
 keywords = ["pynacle", "middleware", "aiohttp"]
 dependencies = [
     "aiohttp",
     "aiohttp_middlewares",
     "pynacl"
 ]
-readme = "README.md"
+readme = "README.rst"
 
 
 [project.optional-dependencies]
 test = ["pytest"]
 
 dev = [
+    "docstring-gen",
     "build",
     "black",
     "flake8",
     "isort",
     "pip-tools",
     "bumpversion",
     "twine"
 ]
 
+docs = [
+    "sphinx",
+    "sphinx_copybutton",
+    "sphinx_favicon",
+    "sphinx_reredirects",
+    "sphinx_toolbox",
+    "furo"
+]
+
 [tool.black]
 line-length = 89
```

