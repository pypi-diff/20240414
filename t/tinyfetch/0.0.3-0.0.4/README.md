# Comparing `tmp/tinyfetch-0.0.3.tar.gz` & `tmp/tinyfetch-0.0.4.tar.gz`

## Comparing `tinyfetch-0.0.3.tar` & `tinyfetch-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 tinyfetch-0.0.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 tinyfetch-0.0.3/.github/workflows/test.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tinyfetch-0.0.3/src/tinyfetch/__init__.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 tinyfetch-0.0.3/src/tinyfetch/cli.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 tinyfetch-0.0.3/src/tinyfetch/core.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 tinyfetch-0.0.3/src/tinyfetch/module.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyfetch-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 tinyfetch-0.0.3/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 tinyfetch-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 tinyfetch-0.0.3/README.md
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 tinyfetch-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 tinyfetch-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 tinyfetch-0.0.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 tinyfetch-0.0.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 tinyfetch-0.0.4/src/tinyfetch/__init__.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 tinyfetch-0.0.4/src/tinyfetch/cli.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 tinyfetch-0.0.4/src/tinyfetch/core.py
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 tinyfetch-0.0.4/src/tinyfetch/module.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyfetch-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 tinyfetch-0.0.4/tests/test.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 tinyfetch-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 tinyfetch-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 tinyfetch-0.0.4/README.md
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 tinyfetch-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 tinyfetch-0.0.4/PKG-INFO
```

### Comparing `tinyfetch-0.0.3/.github/workflows/publish.yml` & `tinyfetch-0.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `tinyfetch-0.0.3/.github/workflows/test.yml` & `tinyfetch-0.0.4/.github/workflows/test.yml`

 * *Files 21% similar despite different names*

```diff
@@ -21,12 +21,15 @@
     - uses: actions/checkout@v4
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
-    - name: Install Tinyfeth
-      run: pip install --upgrade tinyfetch
+    - name: Install Hatch
+      run: pip install --upgrade hatch
 
-    - name: Run Tinyfeth
-      run: tinyfetch
+    - name: Run test
+      run: hatch run test
+
+    - name: Install and Run Tinyfeth
+      run: pip install -U tinyfetch && tinyfetch
```

### Comparing `tinyfetch-0.0.3/src/tinyfetch/module.py` & `tinyfetch-0.0.4/src/tinyfetch/module.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,63 @@
 import csv
 import getpass
 import os
 import platform
 from dataclasses import dataclass, field
+from enum import Enum
 from pathlib import Path
+from typing import Union
 
-RESET = "\u001b[0m"
 BOLD = "\u001b[1m"
-MAIN = BOLD + "\u001b[034m"
+RESET = "\u001b[0m"
+
+
+class Color(Enum):
+    red = "\u001b[31m"
+    green = "\u001b[32m"
+    yellow = "\u001b[33m"
+    blue = "\u001b[34m"
+    magenta = "\u001b[35m"
+    cyan = "\u001b[36m"
 
 
 @dataclass
 class Module:
-    title: str = field(init=False, default=None)
+    title: Union[str, None] = field(init=False, default=None)
     value: str = field(init=False)
+    title_color: str = field(default=Color["blue"])
+    no_color: bool = field(default=False)
 
-    def output(self):
+    def output(self) -> str:
         if self.title is None:
             return self.value
-        return f"{MAIN}{self.title}:{RESET} {self.value}"
+        if self.no_color:
+            return f"{self.title}: {self.value}"
+        return f"{BOLD}{self.title_color.value}{self.title}:{RESET} {self.value}"
 
 
 @dataclass
 class Space(Module):
     def __post_init__(self):
-        self.value = " "
+        self.value = ""
 
 
 @dataclass
 class UserHost(Module):
     def __post_init__(self):
         user = getpass.getuser()
         host = os.uname().nodename
         self.userhost = f"{user}@{host}"
-        self.value = MAIN + self.userhost + RESET
 
-    def __len__(self):
+        if self.no_color:
+            self.value = self.userhost
+        else:
+            self.value = f"{BOLD}{self.title_color.value}{self.userhost}{RESET}"
+
+    def __len__(self) -> int:
         return len(self.userhost)
 
 
 @dataclass
 class SplitLine(Module):
     char: str = field(init=False, default="-")
 
@@ -98,12 +116,12 @@
 class OperationSystem(Module):
     def __post_init__(self):
         self.title = "OS"
 
         if os.name == "posix":
             self.value = self.posix_os_name()
 
-    def posix_os_name(self):
+    def posix_os_name(self) -> str:
         path = Path("/etc/os-release")
         with open(path) as file:
             reader = csv.reader(file, delimiter="=")
             return dict(reader)["PRETTY_NAME"] + " " + os.uname().machine
```

### Comparing `tinyfetch-0.0.3/.gitignore` & `tinyfetch-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `tinyfetch-0.0.3/LICENSE.txt` & `tinyfetch-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tinyfetch-0.0.3/pyproject.toml` & `tinyfetch-0.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -27,15 +27,15 @@
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = []
 
 [project.urls]
 Source = "https://github.com/beucismis/tinyfetch"
 Issues = "https://github.com/beucismis/tinyfetch/issues"
-Documentation = "https://github.com/beucismis/tinyfetch#readme"
+Documentation = "https://github.com/beucismis/tinyfetch?tab=readme-ov-file#documentation"
 
 [project.scripts]
 tfetch = "tinyfetch.cli:main"
 tinyfetch = "tinyfetch.cli:main"
 
 [tool.hatch.version]
 path = "src/tinyfetch/__init__.py"
```

