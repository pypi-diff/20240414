# Comparing `tmp/keymouse-0.0.5.tar.gz` & `tmp/keymouse-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keymouse-0.0.5.tar", last modified: Fri Aug 26 20:20:39 2022, max compression
+gzip compressed data, was "keymouse-0.0.6.tar", last modified: Sun Apr 14 13:46:04 2024, max compression
```

## Comparing `keymouse-0.0.5.tar` & `keymouse-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-08-26 20:20:39.221152 keymouse-0.0.5/
--rw-rw-rw-   0        0        0      570 2022-08-26 20:20:39.221152 keymouse-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      261 2022-08-02 04:31:19.000000 keymouse-0.0.5/README.md
--rw-rw-rw-   0        0        0      198 2022-08-26 20:20:39.221969 keymouse-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      500 2022-08-26 20:20:08.000000 keymouse-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-26 20:20:39.208350 keymouse-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2022-08-26 20:20:39.214355 keymouse-0.0.5/src/keymouse/
--rw-rw-rw-   0        0        0       31 2022-07-31 22:34:48.000000 keymouse-0.0.5/src/keymouse/__init__.py
--rw-rw-rw-   0        0        0     6886 2022-08-26 20:19:44.000000 keymouse-0.0.5/src/keymouse/keymouse.py
-drwxrwxrwx   0        0        0        0 2022-08-26 20:20:39.219324 keymouse-0.0.5/src/keymouse.egg-info/
--rw-rw-rw-   0        0        0      570 2022-08-26 20:20:39.000000 keymouse-0.0.5/src/keymouse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2022-08-26 20:20:39.000000 keymouse-0.0.5/src/keymouse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-26 20:20:39.000000 keymouse-0.0.5/src/keymouse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2022-08-26 20:20:39.000000 keymouse-0.0.5/src/keymouse.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-08-26 20:20:39.000000 keymouse-0.0.5/src/keymouse.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-14 13:46:04.104267 keymouse-0.0.6/
+-rw-rw-rw-   0        0        0     1074 2022-07-31 18:41:58.000000 keymouse-0.0.6/LICENCE.txt
+-rw-rw-rw-   0        0        0      851 2024-04-14 13:46:04.094077 keymouse-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2022-08-02 04:31:19.000000 keymouse-0.0.6/README.md
+-rw-rw-rw-   0        0        0      718 2024-04-14 13:43:15.000000 keymouse-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-14 13:46:04.105278 keymouse-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-14 13:46:04.060992 keymouse-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-14 13:46:04.078449 keymouse-0.0.6/src/keymouse/
+-rw-rw-rw-   0        0        0       31 2022-07-31 22:34:48.000000 keymouse-0.0.6/src/keymouse/__init__.py
+-rw-rw-rw-   0        0        0     6901 2024-04-14 13:29:07.000000 keymouse-0.0.6/src/keymouse/keymouse.py
+drwxrwxrwx   0        0        0        0 2024-04-14 13:46:04.094077 keymouse-0.0.6/src/keymouse.egg-info/
+-rw-rw-rw-   0        0        0      851 2024-04-14 13:46:04.000000 keymouse-0.0.6/src/keymouse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2024-04-14 13:46:04.000000 keymouse-0.0.6/src/keymouse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 13:46:04.000000 keymouse-0.0.6/src/keymouse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-14 13:46:04.000000 keymouse-0.0.6/src/keymouse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-14 13:46:04.000000 keymouse-0.0.6/src/keymouse.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-14 13:46:04.094077 keymouse-0.0.6/tests/
+-rw-rw-rw-   0        0        0     1330 2023-08-13 17:43:42.000000 keymouse-0.0.6/tests/test.py
```

### Comparing `keymouse-0.0.5/src/keymouse/keymouse.py` & `keymouse-0.0.6/src/keymouse/keymouse.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 }
 
 
 class KeyMouse:
     def __init__(self) -> None:
         self._keyboard = pynput.keyboard.Controller()
         self._mouse = pynput.mouse.Controller()
-        self.layout = Layout()
+        self.layout = Layout(use_cache=False)
         # It is important to get layout as we need to change 0 thread language to 'us'
         cur_layout = self.layout.get()
         logger.debug(f"Layout: '{cur_layout}'")
 
     def press(self, key, interval=0.0, delay=0.0):
         logger.debug(f"Press: '{key}'")
         key = KEYS.get(key, key)
```

