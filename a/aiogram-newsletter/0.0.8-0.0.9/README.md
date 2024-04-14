# Comparing `tmp/aiogram-newsletter-0.0.8.tar.gz` & `tmp/aiogram-newsletter-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram-newsletter-0.0.8.tar", last modified: Fri Apr  5 21:56:36 2024, max compression
+gzip compressed data, was "aiogram-newsletter-0.0.9.tar", last modified: Sat Apr 13 20:33:39 2024, max compression
```

## Comparing `aiogram-newsletter-0.0.8.tar` & `aiogram-newsletter-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-05 21:56:36.879755 aiogram-newsletter-0.0.8/
--rw-rw-r--   0 ness      (1000) ness      (1000)     1066 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.8/LICENSE
--rw-r--r--   0 ness      (1000) ness      (1000)     2643 2024-04-05 21:56:36.879755 aiogram-newsletter-0.0.8/PKG-INFO
--rw-rw-r--   0 ness      (1000) ness      (1000)     1985 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.8/README.md
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-05 21:56:36.875754 aiogram-newsletter-0.0.8/aiogram_newsletter/
--rw-rw-r--   0 ness      (1000) ness      (1000)        0 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.8/aiogram_newsletter/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)    10748 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.8/aiogram_newsletter/handlers.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     8129 2024-04-05 21:55:03.000000 aiogram-newsletter-0.0.8/aiogram_newsletter/manager.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1504 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.8/aiogram_newsletter/middleware.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-05 21:56:36.879755 aiogram-newsletter-0.0.8/aiogram_newsletter/utils/
--rw-rw-r--   0 ness      (1000) ness      (1000)        0 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.8/aiogram_newsletter/utils/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      409 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.8/aiogram_newsletter/utils/exceptions.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     7165 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.8/aiogram_newsletter/utils/keyboards.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2868 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.8/aiogram_newsletter/utils/misc.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      367 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.8/aiogram_newsletter/utils/states.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     9124 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.8/aiogram_newsletter/utils/texts.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-05 21:56:36.879755 aiogram-newsletter-0.0.8/aiogram_newsletter.egg-info/
--rw-r--r--   0 ness      (1000) ness      (1000)     2643 2024-04-05 21:56:36.000000 aiogram-newsletter-0.0.8/aiogram_newsletter.egg-info/PKG-INFO
--rw-rw-r--   0 ness      (1000) ness      (1000)      576 2024-04-05 21:56:36.000000 aiogram-newsletter-0.0.8/aiogram_newsletter.egg-info/SOURCES.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)        1 2024-04-05 21:56:36.000000 aiogram-newsletter-0.0.8/aiogram_newsletter.egg-info/dependency_links.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)       29 2024-04-05 21:56:36.000000 aiogram-newsletter-0.0.8/aiogram_newsletter.egg-info/requires.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)       19 2024-04-05 21:56:36.000000 aiogram-newsletter-0.0.8/aiogram_newsletter.egg-info/top_level.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)       38 2024-04-05 21:56:36.879755 aiogram-newsletter-0.0.8/setup.cfg
--rw-rw-r--   0 ness      (1000) ness      (1000)      898 2024-04-05 21:56:11.000000 aiogram-newsletter-0.0.8/setup.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-13 20:33:39.420539 aiogram-newsletter-0.0.9/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1066 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.9/LICENSE
+-rw-r--r--   0 ness      (1000) ness      (1000)     2643 2024-04-13 20:33:39.420539 aiogram-newsletter-0.0.9/PKG-INFO
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1985 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.9/README.md
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-13 20:33:39.420539 aiogram-newsletter-0.0.9/aiogram_newsletter/
+-rw-rw-r--   0 ness      (1000) ness      (1000)        0 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.9/aiogram_newsletter/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)    10748 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.9/aiogram_newsletter/handlers.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     8940 2024-04-13 20:17:39.000000 aiogram-newsletter-0.0.9/aiogram_newsletter/manager.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1763 2024-04-13 20:20:10.000000 aiogram-newsletter-0.0.9/aiogram_newsletter/middleware.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-13 20:33:39.420539 aiogram-newsletter-0.0.9/aiogram_newsletter/utils/
+-rw-rw-r--   0 ness      (1000) ness      (1000)        0 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.9/aiogram_newsletter/utils/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      409 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.9/aiogram_newsletter/utils/exceptions.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     7165 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.9/aiogram_newsletter/utils/keyboards.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2868 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.9/aiogram_newsletter/utils/misc.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      367 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.9/aiogram_newsletter/utils/states.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     9124 2024-04-05 21:52:20.000000 aiogram-newsletter-0.0.9/aiogram_newsletter/utils/texts.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-04-13 20:33:39.420539 aiogram-newsletter-0.0.9/aiogram_newsletter.egg-info/
+-rw-r--r--   0 ness      (1000) ness      (1000)     2643 2024-04-13 20:33:39.000000 aiogram-newsletter-0.0.9/aiogram_newsletter.egg-info/PKG-INFO
+-rw-rw-r--   0 ness      (1000) ness      (1000)      576 2024-04-13 20:33:39.000000 aiogram-newsletter-0.0.9/aiogram_newsletter.egg-info/SOURCES.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)        1 2024-04-13 20:33:39.000000 aiogram-newsletter-0.0.9/aiogram_newsletter.egg-info/dependency_links.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)       29 2024-04-13 20:33:39.000000 aiogram-newsletter-0.0.9/aiogram_newsletter.egg-info/requires.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)       19 2024-04-13 20:33:39.000000 aiogram-newsletter-0.0.9/aiogram_newsletter.egg-info/top_level.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)       38 2024-04-13 20:33:39.420539 aiogram-newsletter-0.0.9/setup.cfg
+-rw-rw-r--   0 ness      (1000) ness      (1000)      898 2024-04-13 20:21:06.000000 aiogram-newsletter-0.0.9/setup.py
```

### Comparing `aiogram-newsletter-0.0.8/LICENSE` & `aiogram-newsletter-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogram-newsletter-0.0.8/PKG-INFO` & `aiogram-newsletter-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram-newsletter
-Version: 0.0.8
+Version: 0.0.9
 Summary: Newsletter handler for aiogram bots.
 Home-page: https://github.com/nessshon/aiogram-newsletter/
 Author: nessshon
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `aiogram-newsletter-0.0.8/README.md` & `aiogram-newsletter-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `aiogram-newsletter-0.0.8/aiogram_newsletter/handlers.py` & `aiogram-newsletter-0.0.9/aiogram_newsletter/handlers.py`

 * *Files identical despite different names*

### Comparing `aiogram-newsletter-0.0.8/aiogram_newsletter/manager.py` & `aiogram-newsletter-0.0.9/aiogram_newsletter/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,34 @@
     def middleware_data(self) -> Dict[str, Any]:
         return self._data
 
     async def return_callback(self) -> None:
         return_callback = await self.data_storage.get_data("return_callback")
         await return_callback(**self.middleware_data)
 
+    async def update_interfaces_language(self, language_code: str) -> None:
+        """
+        Update interfaces language.
+
+        :param language_code: The language code to update to.
+        :raise LanguageCodeNotSupported: If the provided language code is not supported.
+        """
+        if (
+                language_code in self.text_message.text_messages and
+                language_code in self.inline_keyboard.text_buttons
+        ):
+            await self.state.update_data(language_code=language_code)
+            self.user.language_code = language_code
+            self.text_message.language_code = self.inline_keyboard.language_code = language_code
+            return None
+
+        raise ValueError(
+            f"Language code '{language_code}' not in text message or button text"
+        )
+
     async def newsletter_menu(
             self,
             users_ids: List[int],
             return_callback: Callable[..., Awaitable],
     ) -> Message:
         await self.data_storage.set_data(return_callback, "return_callback")
         await self.state.update_data(users_ids=users_ids, page=1)
```

### Comparing `aiogram-newsletter-0.0.8/aiogram_newsletter/middleware.py` & `aiogram-newsletter-0.0.9/aiogram_newsletter/middleware.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 from typing import Callable, Dict, Any, Awaitable, Optional
 
+from aiogram.fsm.context import FSMContext
 from apscheduler.schedulers.asyncio import AsyncIOScheduler
 
 from aiogram import BaseMiddleware
 from aiogram.types import TelegramObject, User
 
 from .manager import ANManager
 from .utils.keyboards import InlineKeyboard
@@ -26,17 +27,22 @@
     async def __call__(
             self,
             handler: Callable[[TelegramObject, Dict[str, Any]], Awaitable[Any]],
             event: TelegramObject,
             data: Dict[str, Any],
     ) -> Any:
         user: User = data.get("event_from_user")
+        state: FSMContext = data.get("state")
 
-        text_message = self.text_message or TextMessage(user.language_code)
-        inline_keyboard = self.inline_keyboard or InlineKeyboard(user.language_code)
+        state_data = await state.get_data()
+        language_code = state_data.get("language_code")
+
+        language_code = language_code if language_code else user.language_code
+        text_message = self.text_message or TextMessage(language_code)
+        inline_keyboard = self.inline_keyboard or InlineKeyboard(language_code)
 
         an_manager = ANManager(
             apscheduler=self.apscheduler,
             text_message=text_message,
             inline_keyboard=inline_keyboard,
             data=data,
         )
```

### Comparing `aiogram-newsletter-0.0.8/aiogram_newsletter/utils/keyboards.py` & `aiogram-newsletter-0.0.9/aiogram_newsletter/utils/keyboards.py`

 * *Files identical despite different names*

### Comparing `aiogram-newsletter-0.0.8/aiogram_newsletter/utils/misc.py` & `aiogram-newsletter-0.0.9/aiogram_newsletter/utils/misc.py`

 * *Files identical despite different names*

### Comparing `aiogram-newsletter-0.0.8/aiogram_newsletter/utils/texts.py` & `aiogram-newsletter-0.0.9/aiogram_newsletter/utils/texts.py`

 * *Files identical despite different names*

### Comparing `aiogram-newsletter-0.0.8/aiogram_newsletter.egg-info/PKG-INFO` & `aiogram-newsletter-0.0.9/aiogram_newsletter.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram-newsletter
-Version: 0.0.8
+Version: 0.0.9
 Summary: Newsletter handler for aiogram bots.
 Home-page: https://github.com/nessshon/aiogram-newsletter/
 Author: nessshon
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `aiogram-newsletter-0.0.8/aiogram_newsletter.egg-info/SOURCES.txt` & `aiogram-newsletter-0.0.9/aiogram_newsletter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiogram-newsletter-0.0.8/setup.py` & `aiogram-newsletter-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aiogram-newsletter",
-    version="0.0.8",
+    version="0.0.9",
     author="nessshon",
     description="Newsletter handler for aiogram bots.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=["example"]),
     install_requires=[
         "aiogram>=3",
```

