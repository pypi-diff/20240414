# Comparing `tmp/pylayout-0.0.9.tar.gz` & `tmp/pylayout-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylayout-0.0.9.tar", last modified: Wed Aug 16 09:24:47 2023, max compression
+gzip compressed data, was "pylayout-0.1.0.tar", last modified: Sun Apr 14 13:38:18 2024, max compression
```

## Comparing `pylayout-0.0.9.tar` & `pylayout-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-x---   0 roman     (1001) roman     (1001)        0 2023-08-16 09:24:47.882139 pylayout-0.0.9/
--rw-r-----   0 roman     (1001) roman     (1001)      261 2023-08-16 09:24:47.882139 pylayout-0.0.9/PKG-INFO
--rw-r-----   0 roman     (1001) roman     (1001)       52 2023-08-16 09:16:54.000000 pylayout-0.0.9/README.md
--rw-r-----   0 roman     (1001) roman     (1001)      107 2023-08-16 09:24:47.882139 pylayout-0.0.9/setup.cfg
--rw-r-----   0 roman     (1001) roman     (1001)      470 2023-08-16 09:19:12.000000 pylayout-0.0.9/setup.py
-drwxr-x---   0 roman     (1001) roman     (1001)        0 2023-08-16 09:24:47.882139 pylayout-0.0.9/src/
-drwxr-x---   0 roman     (1001) roman     (1001)        0 2023-08-16 09:24:47.882139 pylayout-0.0.9/src/pylayout/
--rw-r-----   0 roman     (1001) roman     (1001)       29 2023-08-16 09:16:54.000000 pylayout-0.0.9/src/pylayout/__init__.py
--rw-r-----   0 roman     (1001) roman     (1001)      586 2023-08-16 09:16:54.000000 pylayout-0.0.9/src/pylayout/_lang_layouts.py
--rw-r-----   0 roman     (1001) roman     (1001)     8678 2023-08-16 09:18:57.000000 pylayout-0.0.9/src/pylayout/pylayout.py
-drwxr-x---   0 roman     (1001) roman     (1001)        0 2023-08-16 09:24:47.882139 pylayout-0.0.9/src/pylayout.egg-info/
--rw-r-----   0 roman     (1001) roman     (1001)      261 2023-08-16 09:24:47.000000 pylayout-0.0.9/src/pylayout.egg-info/PKG-INFO
--rw-r-----   0 roman     (1001) roman     (1001)      287 2023-08-16 09:24:47.000000 pylayout-0.0.9/src/pylayout.egg-info/SOURCES.txt
--rw-r-----   0 roman     (1001) roman     (1001)        1 2023-08-16 09:24:47.000000 pylayout-0.0.9/src/pylayout.egg-info/dependency_links.txt
--rw-r-----   0 roman     (1001) roman     (1001)       41 2023-08-16 09:24:47.000000 pylayout-0.0.9/src/pylayout.egg-info/requires.txt
--rw-r-----   0 roman     (1001) roman     (1001)        9 2023-08-16 09:24:47.000000 pylayout-0.0.9/src/pylayout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-14 13:38:18.521237 pylayout-0.1.0/
+-rw-rw-rw-   0        0        0     1074 2024-04-14 13:32:54.000000 pylayout-0.1.0/LICENCE.txt
+-rw-rw-rw-   0        0        0      600 2024-04-14 13:38:18.519240 pylayout-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       53 2024-04-14 13:32:44.000000 pylayout-0.1.0/README.md
+-rw-rw-rw-   0        0        0      691 2024-04-14 13:33:12.000000 pylayout-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-14 13:38:18.521237 pylayout-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-14 13:38:18.438496 pylayout-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-14 13:38:18.480846 pylayout-0.1.0/src/pylayout/
+-rw-rw-rw-   0        0        0       64 2024-04-14 07:56:50.000000 pylayout-0.1.0/src/pylayout/__init__.py
+-rw-rw-rw-   0        0        0      586 2023-08-13 17:05:02.000000 pylayout-0.1.0/src/pylayout/_lang_layouts.py
+-rw-rw-rw-   0        0        0    10819 2024-04-14 13:27:23.000000 pylayout-0.1.0/src/pylayout/pylayout.py
+drwxrwxrwx   0        0        0        0 2024-04-14 13:38:18.517277 pylayout-0.1.0/src/pylayout.egg-info/
+-rw-rw-rw-   0        0        0      600 2024-04-14 13:38:18.000000 pylayout-0.1.0/src/pylayout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2024-04-14 13:38:18.000000 pylayout-0.1.0/src/pylayout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 13:38:18.000000 pylayout-0.1.0/src/pylayout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-04-14 13:38:18.000000 pylayout-0.1.0/src/pylayout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-14 13:38:18.000000 pylayout-0.1.0/src/pylayout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-14 13:38:18.514236 pylayout-0.1.0/tests/
+-rw-rw-rw-   0        0        0      936 2024-04-14 08:04:29.000000 pylayout-0.1.0/tests/test.py
```

### Comparing `pylayout-0.0.9/src/pylayout/_lang_layouts.py` & `pylayout-0.1.0/src/pylayout/_lang_layouts.py`

 * *Files identical despite different names*

### Comparing `pylayout-0.0.9/src/pylayout/pylayout.py` & `pylayout-0.1.0/src/pylayout/pylayout.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,69 +15,91 @@
     import win32process
 
     # from ctypes import wintypes
 
 from ._lang_layouts import LAYOUTS
 
 
-def ban_ruscists(lang: str):
+def bun_ruscists(lang: str):
     if lang == "ru":
         print("Glory to Ukraine!!!")
         sys.exit()
 
 
+def adapt_lang_codes(key: str, invert=False):
+    codes = {"us": "en", "ua": "uk"}
+    if invert:
+        codes = {v: k for k, v in codes.items()}
+    code = codes.get(key)
+    return code if code else key
+
+
 class Layout:
     _ubuntu_call = "gdbus call --session --dest org.gnome.Shell --object-path /org/gnome/Shell --method org.gnome.Shell.Eval '{command}'"
     _windows_call = "chcp 65001 >NUL & powershell {command}"
 
-    def __init__(self) -> None:
+    def __init__(self, use_cache=True) -> None:
         if "Windows" not in platform.platform() and not "Linux" in platform.platform():
             raise TypeError("Invalid system")
 
-        self.cached_layouts = None
+        self.use_cache = use_cache
+        self.layouts = None
 
         try:
             sys.stdin.reconfigure(encoding="utf-8")
             sys.stdout.reconfigure(encoding="utf-8")
             sys.stderr.reconfigure(encoding="utf-8")
         except:
             pass
 
     def get(self) -> str:
         """Return current layout as 'uk', 'us' etc"""
         if "Windows" in platform.platform():
-            if not self.cached_layouts:
-                self.cached_layouts = self._get_available()
+            if self.use_cache == False or not self.layouts:
+                self.layouts = self._get_available_layouts()
+
+            hwnd = win32gui.GetForegroundWindow()
+            thread_id, process_id = win32process.GetWindowThreadProcessId(hwnd)
+            hkl = win32api.GetKeyboardLayout(thread_id)
+
+            # import pygetwindow
+
+            # for window in pygetwindow.getAllWindows():
+            #     if window._hWnd == hwnd:
+            #         break
+            # else:
+            #     raise Exception("No window assosiated with console")
 
-            # Using ctypes as it probably faster but I'm not sure
-            hwnd = ctypes.windll.user32.GetForegroundWindow()
-            tid = ctypes.windll.user32.GetWindowThreadProcessId(hwnd, 0)
-            result = ctypes.windll.user32.GetKeyboardLayout(tid)
+            layouts_reversed = {v: k for k, v in self.layouts.items()}
+            layout = layouts_reversed[hkl]
 
-            layouts = {v: k for k, v in self.cached_layouts.items()}
-            layout = layouts[result]
             # dictionary[new_key] = dictionary.pop(old_key)
         elif "Linux" in platform.platform():
             get_current_layout_command = "imports.ui.status.keyboard.getInputSourceManager().currentSource.id"
             command = self._ubuntu_call.format(command=get_current_layout_command)
             result = self._subprocess_execute(command)
-            layout = re.findall('"(.*)"', result)[0]
+            if "true" in result:
+                layout = re.findall('"(.*)"', result)[0]
+            else:
+                command = "gsettings get org.gnome.desktop.input-sources mru-sources"
+                result = self._subprocess_execute(command)
+                pre_result = re.findall(r"\(.*?\)", result)[0]
+                layout = re.findall(r"'(.*?)'", pre_result)[1]
 
-        # Convert lang names
-        layout = "en" if layout == "us" else layout
-        layout = "uk" if layout == "ua" else layout
+        layout = adapt_lang_codes(layout)
 
-        ban_ruscists(layout)
+        bun_ruscists(layout)
         return layout
 
     def set(self, dest_lang: str) -> bool:
         """dest_lang: 'uk', 'us' etc"""
-        ban_ruscists(dest_lang)
-        if not self.cached_layouts:
-            self.cached_layouts = self._get_available()
+        bun_ruscists(dest_lang)
+        if self.use_cache == False or not self.layouts:
+            self.layouts = self._get_available_layouts()
+
         if "Windows" in platform.platform():
             # Cache result to speed up
 
             # w = ctypes.windll.user32.GetForegroundWindow()
             # tid = ctypes.windll.user32.GetWindowThreadProcessId(w, 0)
             # result = ctypes.windll.user32.GetKeyboardLayout(tid)
             # z = self.available()
@@ -85,43 +107,56 @@
             # lid_hex = hex(lid)
             # Needs HKL
             # win32api.PostMessage(ctypes.windll.user32.GetForegroundWindow(), 0x0050, 2, self.cached_layouts[dest_lang])
             code = win32api.PostMessage(
                 win32gui.GetForegroundWindow(),
                 win32con.WM_INPUTLANGCHANGEREQUEST,
                 0,
-                self.cached_layouts[dest_lang],
+                self.layouts[dest_lang],
             )
             if not code:
                 return True
             else:
                 return False
 
             # ActivateKeyboardLayout = ctypes.windll.user32.ActivateKeyboardLayout
             # ActivateKeyboardLayout.argtypes = (wintypes.HKL, wintypes.UINT)
             # ActivateKeyboardLayout.restype = wintypes.HKL
             # ActivateKeyboardLayout(self.available()[dest_lang], 0)
         elif "Linux" in platform.platform():
-            set_layout_command = f"imports.ui.status.keyboard.getInputSourceManager().inputSources[{self.cached_layouts[dest_lang]}].activate()"
+            set_layout_command = (
+                f"imports.ui.status.keyboard.getInputSourceManager().inputSources[{self.layouts[dest_lang]}].activate()"
+            )
             command = self._ubuntu_call.format(command=set_layout_command)
             result = self._subprocess_execute(command)
-            # TODO Analyze result for success
-            return True
+            if "true" in result:
+                return True
+            else:
+                url = "https://askubuntu.com/questions/1412130/dbus-calls-to-gnome-shell-dont-work-under-ubuntu-22-04"
+                print("WARNING:", url)
+
+                if False:  # It changes layout to desired one but breaks default Ubuntu's functionality
+                    command = f"setxkbmap {adapt_lang_codes(dest_lang, invert=True)}"
+                    result = self._subprocess_execute(command)
+                    if "Error" in result:
+                        return False
+                    else:
+                        return True
 
     def toggle(self):
         """Cycle through available layouts"""
         if "Windows" in platform.platform():
             win32api.PostMessage(win32gui.GetForegroundWindow(), win32con.WM_INPUTLANGCHANGEREQUEST)
 
     def list(self) -> list:
         """Return list of available layouts"""
-        if not self.cached_layouts:
-            self.cached_layouts = self._get_available()
+        if self.use_cache == False or not self.layouts:
+            self.layouts = self._get_available_layouts()
         # tuple_ = win32api.GetKeyboardLayoutList()
-        return list(self.cached_layouts.keys())
+        return list(self.layouts.keys())
 
     @staticmethod
     def translate(text: str, source_lang: str, dest_lang: str) -> str:
         """Convert qwerty into йцукен or reverse"""
         converted = ""
         find = LAYOUTS[source_lang]
         take = LAYOUTS[dest_lang]
@@ -142,78 +177,94 @@
 
         language = (None, 0)
         for key, value in indexes.items():
             if value > language[1]:
                 language = (key, value)
         return language[0]
 
-    # def _available_mapped(self):
-    #     if "win32" not in sys.platform:
-    #         return
-    #     # Converts KLID into HKL
-    #     layouts = self._get_available()
-
-    def _get_available(self) -> dict:
+    def _get_available_layouts(self) -> dict:
         layouts = {}
         if "Windows" in platform.platform():
+            layouts_klid = {}
             # returns KLID
             command = self._windows_call.format(command="Get-WinUserLanguageList")
             result = self._subprocess_execute(command, shell=True)
             all_data = result.strip().split("\r\n\r")
             for data in all_data:
                 line = data.split("\r\n")
                 for l in line:
                     pair = l.split(" : ")
                     if "LanguageTag" in pair[0]:
                         key = pair[1].strip().lower()[-2:]
+                        key = adapt_lang_codes(key)
                     elif "InputMethodTips" in pair[0]:
-                        layouts[key] = pair[1].strip().replace("{", "").replace("}", "")
+                        layouts_klid[key] = pair[1].strip().replace("{", "").replace("}", "")
                         break
             # l = ctypes.windll.user32.GetKeyboardLayout(0)
             # z = gw.getActiveWindow()
             # titles = gw.getAllTitles()
             # win = gw.getWindowsWithTitle(titles[2])[0]
             # win.activate()
             # l2 = ctypes.windll.user32.GetKeyboardLayout(0)
             # z._hWnd
 
-            # Convert KLID into HKL
-            for i in range(len(layouts.items())):
+            # Get HKL layout values
+            layouts_hkl = {}
+            while True:
                 # win32api.LoadKeyboardLayout(v.split(":")[1], win32con.KLF_ACTIVATE)
                 # win32api.GetKeyboardLayout(0)
                 # thread_id = ctypes.windll.user32.GetWindowThreadProcessId(win32gui.GetForegroundWindow(), None)
-                thread_id, process_id = win32process.GetWindowThreadProcessId(win32gui.GetForegroundWindow())
+                hwnd = win32gui.GetForegroundWindow()
+                thread_id, process_id = win32process.GetWindowThreadProcessId(hwnd)
                 hkl = win32api.GetKeyboardLayout(thread_id)
                 klid = hex(hkl & 0xFFFFF)
                 # to_hex = hex(hkl)
                 # to_int = int(to_hex, 16)
-                for k, v in layouts.copy().items():
-                    if isinstance(v, str) and klid[-4:] == v.split(":")[0]:
-                        layouts[k] = hkl
-                        break
+                if hkl in list(layouts_hkl.keys()):
+                    break
+                else:
+                    layouts_hkl[hkl] = klid
                 self.toggle()
                 time.sleep(0.1)  # Need timeout to change layout
-            pass
+
+            # Len can differ because there is a bug in Windows that I have 2 ukrainian layouts
+            # assert len(layouts_klid) == len(layouts_hkl)
+
+            # Convert KLID into HKL
+            for hkl, klid1 in layouts_hkl.items():
+                for lang, klid2 in layouts_klid.items():
+                    if klid1[-5:] == klid2[-5:]:
+                        layouts[lang] = hkl
+                        break
+                    # English language is not too precise
+                    elif klid1[-3:] == klid2[-3:] and not layouts.get(lang):
+                        layouts[lang] = hkl
+                        break
+
+            return layouts
         elif "Linux" in platform.platform():
             get_layouts_command = "imports.ui.status.keyboard.getInputSourceManager().inputSources"
             command = self._ubuntu_call.format(command=get_layouts_command)
             result = self._subprocess_execute(command)
-            result_dict = json.loads(re.findall(r"\{.*\}", result)[0])
-            for key, value in result_dict.items():
-                layouts[value["id"]] = int(key)
-            pass
-
-        # Convert lang names and persist order
-        adapted_layouts = {}
-        for key, value in layouts.items():
-            key = "en" if key == "us" else key
-            key = "uk" if key == "ua" else key
-            adapted_layouts[key] = value
-
-        return adapted_layouts
+            if "true" in result:
+                result_dict = json.loads(re.findall(r"\{.*\}", result)[0])
+                for key, value in result_dict.items():
+                    layouts[value["id"]] = int(key)
+                adapted_layouts = {}
+                for key, value in layouts.items():
+                    key = adapt_lang_codes(key)
+                    adapted_layouts[key] = value
+                layouts = adapted_layouts
+            else:
+                command = "gsettings get org.gnome.desktop.input-sources sources"
+                result = self._subprocess_execute(command)
+                for i in re.findall(r"'(.*?)'", result)[1::2]:
+                    i = adapt_lang_codes(i)
+                    layouts[i] = i
+            return layouts
 
     def _subprocess_execute(self, command, shell=False):
         if isinstance(command, list):
             pass
         elif isinstance(command, str):
             command = shlex.split(command)
         process = subprocess.Popen(command, shell=shell, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
```

