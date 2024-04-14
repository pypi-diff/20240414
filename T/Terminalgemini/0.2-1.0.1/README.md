# Comparing `tmp/Terminalgemini-0.2.tar.gz` & `tmp/terminalgemini-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Terminalgemini-0.2.tar", last modified: Sun Apr 14 04:20:50 2024, max compression
+gzip compressed data, was "terminalgemini-1.0.1.tar", last modified: Sun Apr 14 16:17:54 2024, max compression
```

## Comparing `Terminalgemini-0.2.tar` & `terminalgemini-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 04:20:50.601116 Terminalgemini-0.2/
--rw-rw-rw-   0        0        0     1070 2024-04-13 01:32:20.000000 Terminalgemini-0.2/LICENSE
--rw-rw-rw-   0        0        0     5194 2024-04-14 04:20:50.600022 Terminalgemini-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4382 2024-04-13 01:32:20.000000 Terminalgemini-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 04:20:50.585882 Terminalgemini-0.2/Terminalgemini.egg-info/
--rw-rw-rw-   0        0        0     5194 2024-04-14 04:20:50.000000 Terminalgemini-0.2/Terminalgemini.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      453 2024-04-14 04:20:50.000000 Terminalgemini-0.2/Terminalgemini.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 04:20:50.000000 Terminalgemini-0.2/Terminalgemini.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-14 04:20:50.000000 Terminalgemini-0.2/Terminalgemini.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      104 2024-04-14 04:20:50.000000 Terminalgemini-0.2/Terminalgemini.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-14 04:20:50.000000 Terminalgemini-0.2/Terminalgemini.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1012 2024-04-13 01:32:20.000000 Terminalgemini-0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-14 04:20:50.601116 Terminalgemini-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1869 2024-04-14 03:27:34.000000 Terminalgemini-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-14 04:20:50.596959 Terminalgemini-0.2/terminalgpt/
--rw-rw-rw-   0        0        0        0 2024-04-13 01:32:20.000000 Terminalgemini-0.2/terminalgpt/__init__.py
--rw-rw-rw-   0        0        0     8077 2024-04-14 00:01:34.000000 Terminalgemini-0.2/terminalgpt/chat.py
--rw-rw-rw-   0        0        0     3108 2024-04-13 23:53:04.000000 Terminalgemini-0.2/terminalgpt/config.py
--rw-rw-rw-   0        0        0     2477 2024-04-14 00:01:34.000000 Terminalgemini-0.2/terminalgpt/conversations.py
--rw-rw-rw-   0        0        0     2678 2024-04-14 00:02:48.000000 Terminalgemini-0.2/terminalgpt/encryption.py
--rw-rw-rw-   0        0        0    15188 2024-04-14 00:11:50.000000 Terminalgemini-0.2/terminalgpt/main.py
--rw-rw-rw-   0        0        0     6289 2024-04-13 01:32:20.000000 Terminalgemini-0.2/terminalgpt/printer.py
-drwxrwxrwx   0        0        0        0 2024-04-14 04:20:50.599002 Terminalgemini-0.2/tests/
--rw-rw-rw-   0        0        0        0 2024-04-13 01:32:20.000000 Terminalgemini-0.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 16:17:54.509726 terminalgemini-1.0.1/
+-rw-rw-rw-   0        0        0     1070 2024-04-13 01:32:20.000000 terminalgemini-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     5435 2024-04-14 16:17:54.508123 terminalgemini-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4382 2024-04-13 01:32:20.000000 terminalgemini-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 16:17:54.507573 terminalgemini-1.0.1/Terminalgemini.egg-info/
+-rw-rw-rw-   0        0        0     5435 2024-04-14 16:17:54.000000 terminalgemini-1.0.1/Terminalgemini.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2024-04-14 16:17:54.000000 terminalgemini-1.0.1/Terminalgemini.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 16:17:54.000000 terminalgemini-1.0.1/Terminalgemini.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-14 16:17:54.000000 terminalgemini-1.0.1/Terminalgemini.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      104 2024-04-14 16:17:54.000000 terminalgemini-1.0.1/Terminalgemini.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-14 16:17:54.000000 terminalgemini-1.0.1/Terminalgemini.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1012 2024-04-13 01:32:20.000000 terminalgemini-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-14 16:17:54.509726 terminalgemini-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1871 2024-04-14 16:17:03.000000 terminalgemini-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 16:17:54.505502 terminalgemini-1.0.1/terminalgpt/
+-rw-rw-rw-   0        0        0        0 2024-04-13 01:32:20.000000 terminalgemini-1.0.1/terminalgpt/__init__.py
+-rw-rw-rw-   0        0        0     8077 2024-04-14 00:01:34.000000 terminalgemini-1.0.1/terminalgpt/chat.py
+-rw-rw-rw-   0        0        0     3108 2024-04-13 23:53:04.000000 terminalgemini-1.0.1/terminalgpt/config.py
+-rw-rw-rw-   0        0        0     2477 2024-04-14 00:01:34.000000 terminalgemini-1.0.1/terminalgpt/conversations.py
+-rw-rw-rw-   0        0        0     2368 2024-04-14 04:51:24.000000 terminalgemini-1.0.1/terminalgpt/encryption.py
+-rw-rw-rw-   0        0        0    15360 2024-04-14 16:07:39.000000 terminalgemini-1.0.1/terminalgpt/main.py
+-rw-rw-rw-   0        0        0     6289 2024-04-13 01:32:20.000000 terminalgemini-1.0.1/terminalgpt/printer.py
+drwxrwxrwx   0        0        0        0 2024-04-14 16:17:54.505502 terminalgemini-1.0.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-13 01:32:20.000000 terminalgemini-1.0.1/tests/__init__.py
```

### Comparing `Terminalgemini-0.2/LICENSE` & `terminalgemini-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Terminalgemini-0.2/PKG-INFO` & `terminalgemini-1.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 Metadata-Version: 2.1
 Name: Terminalgemini
-Version: 0.2
+Version: 1.0.1
 Summary: AI chat assistant in your terminal powered by Gemini models.
 Home-page: https://github.com/yourusername/TerminalGPT-main
 Author: ticklecatisback
 Author-email: alesaholder@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: google-generativeai
+Requires-Dist: tiktoken
+Requires-Dist: colorama
+Requires-Dist: cryptography
+Requires-Dist: click
+Requires-Dist: prompt-toolkit
+Requires-Dist: yaspin
+Requires-Dist: rich
+Requires-Dist: isort
+Requires-Dist: pytest
+Requires-Dist: pylint
 
 # ![TerminalGPT](logo.png)
 
 [![Continuous Integration](https://github.com/adamyodinsky/TerminalGPT/actions/workflows/MainCI.yml/badge.svg?branch=main)](https://github.com/adamyodinsky/TerminalGPT/actions/workflows/main.yml) ![PyPI](https://img.shields.io/pypi/v/terminalgpt) ![PyPI - Downloads](https://img.shields.io/pypi/dm/terminalgpt) ![commits-since](https://img.shields.io/github/commits-since/adamyodinsky/TerminalGPT/latest) ![GitHub last commit](https://img.shields.io/github/last-commit/adamyodinsky/terminalgpt)
 
 Welcome to terminalGPT, the terminal-based ChatGPT personal assistant app!
 With terminalGPT, you can easily interact with the OpenAI GPT-3.5 and GPT-4 language models.
@@ -141,9 +150,7 @@
 ```
 
 ---
 
 [![Star History Chart](https://api.star-history.com/svg?repos=adamyodinsky/TerminalGPT&type=Date)](https://star-history.com/#bytebase/star-history&Date)
 
 ---
-
-
```

### Comparing `Terminalgemini-0.2/README.md` & `terminalgemini-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `Terminalgemini-0.2/Terminalgemini.egg-info/PKG-INFO` & `terminalgemini-1.0.1/Terminalgemini.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 Metadata-Version: 2.1
 Name: Terminalgemini
-Version: 0.2
+Version: 1.0.1
 Summary: AI chat assistant in your terminal powered by Gemini models.
 Home-page: https://github.com/yourusername/TerminalGPT-main
 Author: ticklecatisback
 Author-email: alesaholder@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: google-generativeai
+Requires-Dist: tiktoken
+Requires-Dist: colorama
+Requires-Dist: cryptography
+Requires-Dist: click
+Requires-Dist: prompt-toolkit
+Requires-Dist: yaspin
+Requires-Dist: rich
+Requires-Dist: isort
+Requires-Dist: pytest
+Requires-Dist: pylint
 
 # ![TerminalGPT](logo.png)
 
 [![Continuous Integration](https://github.com/adamyodinsky/TerminalGPT/actions/workflows/MainCI.yml/badge.svg?branch=main)](https://github.com/adamyodinsky/TerminalGPT/actions/workflows/main.yml) ![PyPI](https://img.shields.io/pypi/v/terminalgpt) ![PyPI - Downloads](https://img.shields.io/pypi/dm/terminalgpt) ![commits-since](https://img.shields.io/github/commits-since/adamyodinsky/TerminalGPT/latest) ![GitHub last commit](https://img.shields.io/github/last-commit/adamyodinsky/terminalgpt)
 
 Welcome to terminalGPT, the terminal-based ChatGPT personal assistant app!
 With terminalGPT, you can easily interact with the OpenAI GPT-3.5 and GPT-4 language models.
@@ -141,9 +150,7 @@
 ```
 
 ---
 
 [![Star History Chart](https://api.star-history.com/svg?repos=adamyodinsky/TerminalGPT&type=Date)](https://star-history.com/#bytebase/star-history&Date)
 
 ---
-
-
```

### Comparing `Terminalgemini-0.2/pyproject.toml` & `terminalgemini-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Terminalgemini-0.2/setup.py` & `terminalgemini-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Terminalgemini',  # Name of your package
-    version='0.2',  # Version of your package
+    version='1.0.1',  # Version of your package
     author='ticklecatisback',  # Your name or your organization's name
     author_email='alesaholder@gmail.com',  # Your email or your organization's contact email
     description='AI chat assistant in your terminal powered by Gemini models.',  # Short description of your package
     long_description=open('README.md').read(),  # Long description read from the README.md file
     long_description_content_type='text/markdown',  # Type of the long description, here markdown
     url='https://github.com/yourusername/TerminalGPT-main',  # Link to your project's GitHub repo
     packages=find_packages(),  # Automatically find all packages and subpackages
```

### Comparing `Terminalgemini-0.2/terminalgpt/chat.py` & `terminalgemini-1.0.1/terminalgpt/chat.py`

 * *Files identical despite different names*

### Comparing `Terminalgemini-0.2/terminalgpt/config.py` & `terminalgemini-1.0.1/terminalgpt/config.py`

 * *Files identical despite different names*

### Comparing `Terminalgemini-0.2/terminalgpt/conversations.py` & `terminalgemini-1.0.1/terminalgpt/conversations.py`

 * *Files identical despite different names*

### Comparing `Terminalgemini-0.2/terminalgpt/encryption.py` & `terminalgemini-1.0.1/terminalgpt/encryption.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 
 class EncryptionManager:
     """Manages encryption and decryption of secrets."""
 
     def __init__(self):
         self.__key_path = config.KEY_PATH
 
+
     def generate_and_store_key(self):
         """Generates and stores the encryption key."""
         key = Fernet.generate_key()
         try:
             os.makedirs(os.path.dirname(self.__key_path), exist_ok=True)
-            with open(self.__key_path, "wb") as file:
-                file.write(key)
+            with open(self.__key_path, "wb") as key_file:
+                key_file.write(key)
         except OSError as e:
             print(Style.BRIGHT + Fore.RED + f"Failed to store key at {self.__key_path}: {e}" + Style.RESET_ALL)
             sys.exit(1)
         return key
 
     def load_key(self):
         """Loads the encryption key from a file."""
@@ -32,35 +33,29 @@
         except FileNotFoundError:
             print(Style.BRIGHT + Fore.RED + f"Encryption key file not found at {self.__key_path}." + Style.RESET_ALL)
             sys.exit(1)
 
     def encrypt(self, data: str, key: bytes) -> bytes:
         """Encrypts a string using Fernet encryption."""
         cipher = Fernet(key)
-        # Ensure data is in bytes
-        data_bytes = data.encode('utf-8')
-        return cipher.encrypt(data_bytes)
+        return cipher.encrypt(data.encode('utf-8'))
 
     def decrypt(self, data: bytes, key: bytes) -> str:
         """Decrypts data using Fernet encryption and returns a string."""
         cipher = Fernet(key)
-        decrypted_data = cipher.decrypt(data)
-        # Convert bytes back to string
-        return decrypted_data.decode('utf-8')
+        return cipher.decrypt(data).decode('utf-8')
 
     def check_api_key_presence(self):
         """Checks if the Gemini API key is properly set up."""
         if not os.path.exists(config.SECRET_PATH) and "GEMINI_API_KEY" not in os.environ:
             message = f"Gemini API key is missing! Please install the API key first with '{config.APP_NAME} install' command."
             print(Style.BRIGHT + Fore.RED + message + Style.RESET_ALL)
             sys.exit(1)
 
     def get_api_key(self) -> str:
-        """Retrieves the Gemini API key securely and ensures it is in the correct type."""
-        self.check_api_key_presence()
+        """Retrieves the API key, preferring environment variable if set."""
         if "GEMINI_API_KEY" in os.environ:
-            # Convert environment variable from string to bytes, then back to string if necessary
-            return os.environ["GEMINI_API_KEY"].encode('utf-8').decode('utf-8')
+            return os.environ["GEMINI_API_KEY"]
         encryption_key = self.load_key()
-        api_key_bytes = self.decrypt(os.path.join(config.SECRET_PATH, 'api_key.enc'), encryption_key)
-        return api_key_bytes
+        api_key_encrypted = os.path.join(config.SECRET_PATH, 'api_key.enc')
+        return self.decrypt(api_key_encrypted, encryption_key)
```

### Comparing `Terminalgemini-0.2/terminalgpt/main.py` & `terminalgemini-1.0.1/terminalgpt/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 @click.group()
 @click.version_option(prog_name="TerminalGPT", message="%(prog)s %(version)s")
 @click.option(
     "--model",
     "-m",
     type=click.Choice(list(config.MODELS.keys())),
-    default=config.get_default_config().get("model", "gpt-3.5-turbo"),
+    default=config.get_default_config().get("model", "gemini-1.0-pro'"),
     show_default=True,
     help="Choose a model to use.",
 )
 # option to choose rich text output
 @click.option(
     "--style",
     "-s",
@@ -45,15 +45,14 @@
     type=int,
     default=0,
     help="Set the token limit. this will override the default token limit for the chosen model.",
 )
 @click.pass_context
 def cli(ctx, model, style: str, token_limit: int = 0):
     """*~ TerminalGPT - Your Personal Terminal Assistant ~*"""
-
     max_token_limit = (
         config.get_default_config().get("models", config.MODELS).get(model)
     )
     printer: Printer = PrinterFactory.get_printer("plain")
 
     if token_limit == 0:
         token_limit = max_token_limit
@@ -111,18 +110,24 @@
         token_limit=int(token_limit - safety_buffer),
         session=ctx.obj["SESSION"],
         messages=[],
         model=ctx.obj["MODEL"],
         printer=ctx.obj["PRINTER"],
     )
 
+    if ctx.obj is None:
+        ctx.obj = {}
+    ctx.obj['MODEL'] = model
+
 
 @click.command(help="Installing the OpenAI API key and setup some default settings.")
-def install():
+def install(ctx):
     """Install the terminalgpt openai api key and create app directories."""
+    model = ctx.obj['MODEL']
+    click.echo(f"Installing with the model: {model}")
 
     printer: Printer = PrinterFactory.get_printer(style="plain")
     enc_manager: EncryptionManager = EncryptionManager()
 
     # Get API key from user
     printer.printt(PrintUtils.INSTALL_WELCOME_MESSAGE)
     api_key = getpass.getpass(
@@ -162,15 +167,15 @@
     printing_style = prompt(
         "\n Choose a printing style ('markdown' is recommended):\n",
         completer=WordCompleter(printing_styles, ignore_case=True),
         style=PromptStyle.from_dict({"prompt": "bold lightblue"}),
         default=printing_styles[0],
     )
 
-    encryption_key = enc_manager.set_encryption_key()
+    encryption_key = enc_manager.generate_and_store_key()
     encrypted_secret = enc_manager.encrypt(api_key.encode(), encryption_key)
 
     if not os.path.exists(os.path.dirname(config.SECRET_PATH)):
         os.makedirs(os.path.dirname(config.SECRET_PATH))
 
     if not os.path.exists(config.CONVERSATIONS_PATH):
         os.mkdir(config.CONVERSATIONS_PATH)
@@ -461,8 +466,8 @@
 cli.add_command(install)
 cli.add_command(new)
 cli.add_command(load)
 cli.add_command(delete)
 
 # pylint: disable=no-value-for-parameter
 if __name__ == "__main__":
-    cli()
+    cli(obj={})
```

### Comparing `Terminalgemini-0.2/terminalgpt/printer.py` & `terminalgemini-1.0.1/terminalgpt/printer.py`

 * *Files identical despite different names*

