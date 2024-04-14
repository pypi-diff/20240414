# Comparing `tmp/tum_esm_utils-2.0.0.tar.gz` & `tmp/tum_esm_utils-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tum_esm_utils-2.0.0.tar", last modified: Sun Apr 14 14:26:51 2024, max compression
+gzip compressed data, was "tum_esm_utils-2.0.1.tar", last modified: Sun Apr 14 16:12:04 2024, max compression
```

## Comparing `tum_esm_utils-2.0.0.tar` & `tum_esm_utils-2.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    34888 2024-04-14 14:19:39.952724 tum_esm_utils-2.0.0/LICENSE
--rw-r--r--   0        0        0     1754 2024-03-04 14:23:31.095903 tum_esm_utils-2.0.0/README.md
--rw-r--r--   0        0        0     2140 2024-04-14 14:26:51.205495 tum_esm_utils-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      556 2024-04-14 14:19:39.955953 tum_esm_utils-2.0.0/tum_esm_utils/__init__.py
--rw-r--r--   0        0        0     2421 2024-04-14 14:19:39.956240 tum_esm_utils-2.0.0/tum_esm_utils/code.py
--rw-r--r--   0        0        0     3302 2024-01-24 23:37:06.907517 tum_esm_utils-2.0.0/tum_esm_utils/datastructures.py
--rw-r--r--   0        0        0     1241 2024-03-24 14:30:26.221385 tum_esm_utils-2.0.0/tum_esm_utils/decorators.py
--rw-r--r--   0        0        0     6911 2024-04-14 14:19:39.956577 tum_esm_utils-2.0.0/tum_esm_utils/em27.py
--rw-r--r--   0        0        0     4982 2024-04-14 14:19:39.956813 tum_esm_utils-2.0.0/tum_esm_utils/files.py
--rw-r--r--   0        0        0       64 2023-08-02 15:33:55.496271 tum_esm_utils-2.0.0/tum_esm_utils/ifg_parser/.gitignore
--rw-r--r--   0        0        0     2462 2023-08-02 15:33:55.496337 tum_esm_utils-2.0.0/tum_esm_utils/ifg_parser/glob_OPUSparms.F90
--rw-r--r--   0        0        0     2459 2023-08-02 15:33:55.496400 tum_esm_utils-2.0.0/tum_esm_utils/ifg_parser/glob_prepro4.F90
--rw-r--r--   0        0        0    28408 2023-08-02 15:33:55.496530 tum_esm_utils-2.0.0/tum_esm_utils/ifg_parser/ifg_parser.F90
--rw-r--r--   0        0        0      758 2023-08-02 15:33:55.496606 tum_esm_utils-2.0.0/tum_esm_utils/ifg_parser/ifg_parser.template.inp
--rw-r--r--   0        0        0   983040 2023-08-02 15:33:55.499240 tum_esm_utils-2.0.0/tum_esm_utils/ifg_parser/refspec.dat
--rw-r--r--   0        0        0   983040 2023-08-02 15:33:55.501952 tum_esm_utils-2.0.0/tum_esm_utils/ifg_parser/refspec2.dat
--rw-r--r--   0        0        0      380 2024-04-14 10:18:02.509797 tum_esm_utils-2.0.0/tum_esm_utils/mathematics.py
--rw-r--r--   0        0        0     4415 2024-04-14 14:19:39.957004 tum_esm_utils-2.0.0/tum_esm_utils/plotting.py
--rw-r--r--   0        0        0     3060 2023-11-13 14:46:00.947794 tum_esm_utils-2.0.0/tum_esm_utils/processes.py
--rw-r--r--   0        0        0        0 2023-08-02 15:33:55.502312 tum_esm_utils-2.0.0/tum_esm_utils/py.typed
--rw-r--r--   0        0        0     3720 2024-04-14 14:19:39.957264 tum_esm_utils-2.0.0/tum_esm_utils/shell.py
--rw-r--r--   0        0        0     1871 2024-04-14 14:19:39.957483 tum_esm_utils-2.0.0/tum_esm_utils/system.py
--rw-r--r--   0        0        0     2082 2024-04-14 14:19:39.957802 tum_esm_utils-2.0.0/tum_esm_utils/text.py
--rw-r--r--   0        0        0     4780 2024-04-14 14:19:39.958049 tum_esm_utils-2.0.0/tum_esm_utils/timing.py
--rw-r--r--   0        0        0     2171 2024-04-14 14:19:39.958359 tum_esm_utils-2.0.0/tum_esm_utils/validators.py
--rw-r--r--   0        0        0     3400 1970-01-01 00:00:00.000000 tum_esm_utils-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    34888 2024-04-14 14:19:39.952724 tum_esm_utils-2.0.1/LICENSE
+-rw-r--r--   0        0        0     1754 2024-04-14 16:07:45.718345 tum_esm_utils-2.0.1/README.md
+-rw-r--r--   0        0        0     2095 2024-04-14 16:12:04.556482 tum_esm_utils-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      556 2024-04-14 14:19:39.955953 tum_esm_utils-2.0.1/tum_esm_utils/__init__.py
+-rw-r--r--   0        0        0     2421 2024-04-14 14:19:39.956240 tum_esm_utils-2.0.1/tum_esm_utils/code.py
+-rw-r--r--   0        0        0     3397 2024-04-14 15:59:57.269809 tum_esm_utils-2.0.1/tum_esm_utils/datastructures.py
+-rw-r--r--   0        0        0     1437 2024-04-14 15:41:47.672621 tum_esm_utils-2.0.1/tum_esm_utils/decorators.py
+-rw-r--r--   0        0        0     7328 2024-04-14 16:01:30.940351 tum_esm_utils-2.0.1/tum_esm_utils/em27.py
+-rw-r--r--   0        0        0     5234 2024-04-14 16:02:35.509373 tum_esm_utils-2.0.1/tum_esm_utils/files.py
+-rw-r--r--   0        0        0       64 2023-08-02 15:33:55.496271 tum_esm_utils-2.0.1/tum_esm_utils/ifg_parser/.gitignore
+-rw-r--r--   0        0        0     2462 2023-08-02 15:33:55.496337 tum_esm_utils-2.0.1/tum_esm_utils/ifg_parser/glob_OPUSparms.F90
+-rw-r--r--   0        0        0     2459 2023-08-02 15:33:55.496400 tum_esm_utils-2.0.1/tum_esm_utils/ifg_parser/glob_prepro4.F90
+-rw-r--r--   0        0        0    28408 2023-08-02 15:33:55.496530 tum_esm_utils-2.0.1/tum_esm_utils/ifg_parser/ifg_parser.F90
+-rw-r--r--   0        0        0      758 2023-08-02 15:33:55.496606 tum_esm_utils-2.0.1/tum_esm_utils/ifg_parser/ifg_parser.template.inp
+-rw-r--r--   0        0        0   983040 2023-08-02 15:33:55.499240 tum_esm_utils-2.0.1/tum_esm_utils/ifg_parser/refspec.dat
+-rw-r--r--   0        0        0   983040 2023-08-02 15:33:55.501952 tum_esm_utils-2.0.1/tum_esm_utils/ifg_parser/refspec2.dat
+-rw-r--r--   0        0        0      381 2024-04-14 16:02:47.777922 tum_esm_utils-2.0.1/tum_esm_utils/mathematics.py
+-rw-r--r--   0        0        0     4533 2024-04-14 16:03:35.124703 tum_esm_utils-2.0.1/tum_esm_utils/plotting.py
+-rw-r--r--   0        0        0     3428 2024-04-14 15:46:07.935669 tum_esm_utils-2.0.1/tum_esm_utils/processes.py
+-rw-r--r--   0        0        0        0 2023-08-02 15:33:55.502312 tum_esm_utils-2.0.1/tum_esm_utils/py.typed
+-rw-r--r--   0        0        0     3779 2024-04-14 16:07:15.811102 tum_esm_utils-2.0.1/tum_esm_utils/shell.py
+-rw-r--r--   0        0        0     1922 2024-04-14 16:04:30.167681 tum_esm_utils-2.0.1/tum_esm_utils/system.py
+-rw-r--r--   0        0        0     2537 2024-04-14 16:05:45.880077 tum_esm_utils-2.0.1/tum_esm_utils/text.py
+-rw-r--r--   0        0        0     5119 2024-04-14 16:06:55.042381 tum_esm_utils-2.0.1/tum_esm_utils/timing.py
+-rw-r--r--   0        0        0     2171 2024-04-14 14:19:39.958359 tum_esm_utils-2.0.1/tum_esm_utils/validators.py
+-rw-r--r--   0        0        0     3350 1970-01-01 00:00:00.000000 tum_esm_utils-2.0.1/PKG-INFO
```

### Comparing `tum_esm_utils-2.0.0/LICENSE` & `tum_esm_utils-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-2.0.0/README.md` & `tum_esm_utils-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-2.0.0/pyproject.toml` & `tum_esm_utils-2.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tum_esm_utils"
-version = "2.0.0"
+version = "2.0.1"
 description = "Python utilities by the Professorship of Environmental Sensing and Modeling at the Technical University of Munich"
 authors = [
     { name = "Moritz Makowski", email = "moritz.makowski@tum.de" },
 ]
 dependencies = [
     "filelock>=3.13.4",
     "requests>=2.31.0",
@@ -13,15 +13,14 @@
     "pytz>=2024.1",
 ]
 requires-python = ">=3.9,<4.0"
 readme = "README.md"
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 keywords = [
     "tum",
```

### Comparing `tum_esm_utils-2.0.0/tum_esm_utils/__init__.py` & `tum_esm_utils-2.0.1/tum_esm_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-2.0.0/tum_esm_utils/code.py` & `tum_esm_utils-2.0.1/tum_esm_utils/code.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-2.0.0/tum_esm_utils/datastructures.py` & `tum_esm_utils-2.0.1/tum_esm_utils/datastructures.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,35 +4,39 @@
 
 from __future__ import annotations
 from typing import Any
 
 
 class RingList:
     def __init__(self, max_size: int):
+        """Initialize a RingList with a maximum size."""
+
         assert max_size > 0, "a max_size of zero doesn't make any sense"
         self._max_size: int = max_size
         self._data: list[float] = [0 for _ in range(max_size)]
         self._current_index: int = -1  # -1 means empty
 
     def clear(self) -> None:
-        """removes all elements"""
+        """Removes all elements from the list."""
+
         self._current_index = -1
 
     def is_full(self) -> bool:
-        """returns true if list is full"""
+        """Returns True if the list is full."""
+
         return self._current_index >= (self._max_size - 1)
 
     def append(self, x: float) -> None:
-        """appends an element to the list"""
+        """Appends an element to the list."""
         self._current_index += 1
         bounded_current_index = self._current_index % self._max_size
         self._data[bounded_current_index] = x
 
     def get(self) -> list[float]:
-        """returns the list of elements"""
+        """Returns the list of elements."""
         # list is full
         if self._current_index >= (self._max_size - 1):
             bounded_current_index = self._current_index % self._max_size
             return (
                 self._data[bounded_current_index + 1 : self._max_size + 1] +
                 self._data[0 : bounded_current_index + 1]
             )
@@ -41,22 +45,22 @@
         elif self._current_index >= 0:
             return self._data[0 : self._current_index + 1]
 
         # list is empty
         return []
 
     def sum(self) -> float:
-        """returns the max size of the list"""
+        """Returns the max size of the list"""
         return sum(self.get())
 
     def get_max_size(self) -> int:
         return self._max_size
 
     def set_max_size(self, new_max_size: int) -> None:
-        """sets a new max size"""
+        """Sets a new max size fo the list."""
         current_list = self.get()
         self._max_size = new_max_size
         self._data = [0] * new_max_size
         self._current_index = -1
         for item in current_list:
             self.append(item)
```

### Comparing `tum_esm_utils-2.0.0/tum_esm_utils/decorators.py` & `tum_esm_utils-2.0.1/tum_esm_utils/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,22 @@
     See https://en.wikipedia.org/wiki/Semaphore_(programming).
     
     
     Credits for the typing of higher level decorators goes to
     https://github.com/python/mypy/issues/1551#issuecomment-253978622.
     """
     def __init__(self, lockfile_path: str, timeout: float = -1) -> None:
-        """A timeout of -1 means that the code waits forever."""
+        """Create a new filelock decorator.
+        
+        A timeout of -1 means that the code waits forever.
+        
+        Args:
+            lockfile_path: The path to the lockfile.
+            timeout:       The time to wait for the lock in seconds."""
+
         self.lockfile_path: str = lockfile_path
         self.timeout: float = timeout
 
     def __call__(self, f: F) -> F:
         @functools.wraps(f)
         def wrapper(*args: tuple[Any], **kwargs: dict[str, Any]) -> Any:
             with filelock.FileLock(self.lockfile_path, timeout=self.timeout):
```

### Comparing `tum_esm_utils-2.0.0/tum_esm_utils/em27.py` & `tum_esm_utils-2.0.1/tum_esm_utils/em27.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,15 +71,25 @@
     corrupt interferograms in the given directory.
 
     It will compile the fortran code using a given compiler
     to perform this task. The fortran code is derived from
     the preprocess source code of Proffast 2
     (https://www.imk-asf.kit.edu/english/3225.php). We use
     it because the retrieval using Proffast 2 will fail if
-    there are corrupt interferograms in the input."""
+    there are corrupt interferograms in the input.
+    
+    Args:
+        ifg_directory:     The directory containing the interferograms.
+        silent:            If set to False, print additional information.
+        fortran_compiler:  The fortran compiler to use.
+        force_recompile:   If set to True, the fortran code will be recompiled.
+
+    Returns:
+        A dictionary containing corrupt filenames as keys and a list of error
+        messages as values."""
 
     # compiling fortran code
     with filelock.FileLock(
         os.path.join(_PARSER_DIR, "ifg_parser.compile.lock"),
         timeout=30,
     ):
         # these sleeps are sadly necessary to eliminate race conditions between
```

### Comparing `tum_esm_utils-2.0.0/tum_esm_utils/files.py` & `tum_esm_utils-2.0.1/tum_esm_utils/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,15 +143,21 @@
 
 def expect_file_contents(
     filepath: str,
     required_content_blocks: list[str] = [],
     forbidden_content_blocks: list[str] = [],
 ) -> None:
     """Assert that the given file contains all of the required content
-    blocks, and/or none of the forbidden content blocks."""
+    blocks, and/or none of the forbidden content blocks.
+    
+    Args:
+        filepath:                 The path to the file.
+        required_content_blocks:  A list of strings that must be present in the file.
+        forbidden_content_blocks: A list of strings that must not be present in the file.
+    """
 
     with open(filepath, "r") as f:
         file_content = f.read()
 
     for b in required_content_blocks:
         assert b in file_content, f'required log content block not found "{b}"'
```

### Comparing `tum_esm_utils-2.0.0/tum_esm_utils/ifg_parser/glob_OPUSparms.F90` & `tum_esm_utils-2.0.1/tum_esm_utils/ifg_parser/glob_OPUSparms.F90`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-2.0.0/tum_esm_utils/ifg_parser/glob_prepro4.F90` & `tum_esm_utils-2.0.1/tum_esm_utils/ifg_parser/glob_prepro4.F90`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-2.0.0/tum_esm_utils/ifg_parser/ifg_parser.F90` & `tum_esm_utils-2.0.1/tum_esm_utils/ifg_parser/ifg_parser.F90`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-2.0.0/tum_esm_utils/ifg_parser/ifg_parser.template.inp` & `tum_esm_utils-2.0.1/tum_esm_utils/ifg_parser/ifg_parser.template.inp`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-2.0.0/tum_esm_utils/ifg_parser/refspec.dat` & `tum_esm_utils-2.0.1/tum_esm_utils/ifg_parser/refspec.dat`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-2.0.0/tum_esm_utils/ifg_parser/refspec2.dat` & `tum_esm_utils-2.0.1/tum_esm_utils/ifg_parser/refspec2.dat`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-2.0.0/tum_esm_utils/plotting.py` & `tum_esm_utils-2.0.1/tum_esm_utils/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,21 @@
     width: float = 10,
     height: float = 10,
     suptitle_y: float = 0.97,
     padding: float = 2,
     dpi: int = 250,
 ) -> Generator[plt.Figure, None, None]:
     """Create a figure for plotting.
+    
+    Usage:
 
+    ```python
+    with create_figure("path/to/figure.png", title="Title") as fig:
+        ...
+    ```
     Args:
         path: The path to save the figure to.
         title: The title of the figure.
         width: The width of the figure.
         height: The height of the figure.
         suptitle_y: The y-coordinate of the figure title.
         padding: The padding of the figure.
```

### Comparing `tum_esm_utils-2.0.0/tum_esm_utils/processes.py` & `tum_esm_utils-2.0.1/tum_esm_utils/processes.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 import os
 import time
 from typing import Optional
 import psutil
 
 
 def get_process_pids(script_path: str) -> list[int]:
-    """Return a list of PIDs that have the given script as their entrypoint"""
+    """Return a list of PIDs that have the given script as their entrypoint.
+    
+    Args:
+        script_path: The absolute path of the python file entrypoint."""
 
     pids: list[int] = []
     for p in psutil.process_iter():
         try:
             if p.cmdline()[1] == script_path:
                 pids.append(p.pid)
         except (
@@ -52,15 +55,23 @@
     script_path: str,
     termination_timeout: Optional[int] = None,
 ) -> list[int]:
     """Terminate all processes that have the given script as their
     entrypoint. Returns the list of terminated PIDs.
     
     If `termination_timeout` is not None, the processes will be
-    terminated forcefully after the given timeout (in seconds)."""
+    terminated forcefully after the given timeout (in seconds).
+    
+    Args:
+        script_path:         The absolute path of the python file entrypoint.
+        termination_timeout: The timeout in seconds after which the
+                             processes will be terminated forcefully.
+
+    Returns:
+        The list of terminated PIDs."""
 
     processes_to_terminate: list[psutil.Process] = []
 
     # terminate the processes gracefully
     for p in psutil.process_iter():
         try:
             if p.cmdline()[1] == script_path:
```

### Comparing `tum_esm_utils-2.0.0/tum_esm_utils/shell.py` & `tum_esm_utils-2.0.1/tum_esm_utils/shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing import Callable, Literal, Optional
 import os
 import re
 import subprocess
 
 
 class CommandLineException(Exception):
+    """Exception raised for errors in the command line."""
     def __init__(self, value: str, details: Optional[str] = None) -> None:
         self.value = value
         self.details = details
         Exception.__init__(self)
 
     def __str__(self) -> str:
         return repr(self.value)
```

### Comparing `tum_esm_utils-2.0.0/tum_esm_utils/system.py` & `tum_esm_utils-2.0.1/tum_esm_utils/system.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,10 +69,13 @@
     """Returns the UTC offset of the system.
 
     ```python
     x = get_utc_offset()
     local time == utc time + x
     ```
     
-    Credits to https://stackoverflow.com/a/35058476/8255842"""
+    Credits to https://stackoverflow.com/a/35058476/8255842
+    
+    Returns:
+        The UTC offset in hours."""
 
     return round((-time.timezone) / 3600, 3)
```

### Comparing `tum_esm_utils-2.0.0/tum_esm_utils/text.py` & `tum_esm_utils-2.0.1/tum_esm_utils/text.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,39 +8,57 @@
 import re
 import datetime
 import random
 import string
 
 
 def get_random_string(length: int, forbidden: list[str] = []) -> str:
-    """Return a random string from lowercase letter, the strings
-    from the list passed as `forbidden` will not be generated"""
+    """Return a random string from lowercase letters.
+    
+    Args:
+        length:     The length of the random string.
+        forbidden:  A list of strings that should not be generated.
+    
+    Returns:
+        A random string."""
+
     output: str = ""
     while True:
         output = "".join(random.choices(string.ascii_lowercase, k=length))
         if output not in forbidden:
             break
     return output
 
 
 def pad_string(
     text: str,
     min_width: int,
     pad_position: Literal["left", "right"] = "left",
     fill_char: Literal["0", " ", "-", "_"] = " ",
 ) -> str:
+    """Pad a string with a fill character to a minimum width.
+
+    Args:
+        text:         The text to pad.
+        min_width:    The minimum width of the text.
+        pad_position: The position of the padding. Either "left" or "right".
+        fill_char:    The character to use for padding.
+    
+    Returns:
+        The padded string."""
+
     if len(text) >= min_width:
         return text
     else:
         pad = fill_char * (min_width - len(text))
         return (pad + text) if (pad_position == "left") else (text + pad)
 
 
 def is_date_string(date_string: str) -> bool:
-    """Returns `True` if string is in a valid `YYYYMMDD` format"""
+    """Returns `True` if string is in a valid `YYYYMMDD` format."""
     try:
         datetime.datetime.strptime(date_string, "%Y%m%d")
         return True
     except ValueError:
         return False
```

### Comparing `tum_esm_utils-2.0.0/tum_esm_utils/timing.py` & `tum_esm_utils-2.0.1/tum_esm_utils/timing.py`

 * *Files 11% similar despite different names*

```diff
@@ -132,18 +132,22 @@
 def wait_for_condition(
     is_successful: Callable[[], bool],
     timeout_message: str,
     timeout_seconds: float = 5,
     check_interval_seconds: float = 0.25,
 ) -> None:
     """Wait for the given condition to be true, or raise a TimeoutError
-    if the condition is not met within the given timeout.
-
-    `check_interval_seconds` controls, how long to wait inbetween
-    `is_successful()` calls."""
+    if the condition is not met within the given timeout. The condition
+    is passed as a function that will be called periodically.
+    
+    Args:
+        is_successful:             A function that returns True if the condition is met.
+        timeout_message:           The message to include in the TimeoutError.
+        timeout_seconds:           The maximum time to wait for the condition to be met.
+        check_interval_seconds:    How long to wait inbetween `is_successful()` calls."""
 
     start_time = time.time()
     while True:
         if is_successful():
             break
         if (time.time() - start_time) > timeout_seconds:
             raise TimeoutError(timeout_message)
```

### Comparing `tum_esm_utils-2.0.0/tum_esm_utils/validators.py` & `tum_esm_utils-2.0.1/tum_esm_utils/validators.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-2.0.0/PKG-INFO` & `tum_esm_utils-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: tum_esm_utils
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python utilities by the Professorship of Environmental Sensing and Modeling at the Technical University of Munich
 Keywords: tum,utils,utilities,environmental,sensing,modeling,python,library,utilities,pydoc-markdown
 Author-Email: Moritz Makowski <moritz.makowski@tum.de>
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: <4.0,>=3.9
 Requires-Dist: filelock>=3.13.4
 Requires-Dist: requests>=2.31.0
```

