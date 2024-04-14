# Comparing `tmp/fstumbler-1.0.0.tar.gz` & `tmp/fstumbler-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fstumbler-1.0.0.tar", last modified: Mon Apr  8 02:17:25 2024, max compression
+gzip compressed data, was "fstumbler-1.1.0.tar", last modified: Sun Apr 14 20:06:39 2024, max compression
```

## Comparing `fstumbler-1.0.0.tar` & `fstumbler-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 ferit     (1000) ferit     (1000)        0 2024-04-08 02:17:25.589285 fstumbler-1.0.0/
--rw-r--r--   0 ferit     (1000) ferit     (1000)    26525 2024-04-08 01:12:57.000000 fstumbler-1.0.0/LICENSE
--rw-r--r--   0 ferit     (1000) ferit     (1000)     1207 2024-04-08 02:17:25.589285 fstumbler-1.0.0/PKG-INFO
--rw-r--r--   0 ferit     (1000) ferit     (1000)      558 2024-04-08 01:10:13.000000 fstumbler-1.0.0/README.md
-drwxr-xr-x   0 ferit     (1000) ferit     (1000)        0 2024-04-08 02:17:25.589285 fstumbler-1.0.0/fstumbler/
--rw-r--r--   0 ferit     (1000) ferit     (1000)      931 2024-04-08 01:13:59.000000 fstumbler-1.0.0/fstumbler/__init__.py
--rw-r--r--   0 ferit     (1000) ferit     (1000)     3005 2024-04-08 01:12:15.000000 fstumbler-1.0.0/fstumbler/core.py
--rw-r--r--   0 ferit     (1000) ferit     (1000)     1868 2024-04-08 01:12:27.000000 fstumbler-1.0.0/fstumbler/node.py
--rw-r--r--   0 ferit     (1000) ferit     (1000)     1199 2024-04-08 01:12:36.000000 fstumbler-1.0.0/fstumbler/util.py
-drwxr-xr-x   0 ferit     (1000) ferit     (1000)        0 2024-04-08 02:17:25.589285 fstumbler-1.0.0/fstumbler.egg-info/
--rw-r--r--   0 ferit     (1000) ferit     (1000)     1207 2024-04-08 02:17:25.000000 fstumbler-1.0.0/fstumbler.egg-info/PKG-INFO
--rw-r--r--   0 ferit     (1000) ferit     (1000)      240 2024-04-08 02:17:25.000000 fstumbler-1.0.0/fstumbler.egg-info/SOURCES.txt
--rw-r--r--   0 ferit     (1000) ferit     (1000)        1 2024-04-08 02:17:25.000000 fstumbler-1.0.0/fstumbler.egg-info/dependency_links.txt
--rw-r--r--   0 ferit     (1000) ferit     (1000)       10 2024-04-08 02:17:25.000000 fstumbler-1.0.0/fstumbler.egg-info/top_level.txt
--rw-r--r--   0 ferit     (1000) ferit     (1000)      618 2024-04-08 02:14:19.000000 fstumbler-1.0.0/pyproject.toml
--rw-r--r--   0 ferit     (1000) ferit     (1000)       38 2024-04-08 02:17:25.589285 fstumbler-1.0.0/setup.cfg
+drwxr-xr-x   0 ferit     (1000) ferit     (1000)        0 2024-04-14 20:06:39.669051 fstumbler-1.1.0/
+-rw-r--r--   0 ferit     (1000) ferit     (1000)    26525 2024-04-08 01:12:57.000000 fstumbler-1.1.0/LICENSE
+-rw-r--r--   0 ferit     (1000) ferit     (1000)     1207 2024-04-14 20:06:39.669051 fstumbler-1.1.0/PKG-INFO
+-rw-r--r--   0 ferit     (1000) ferit     (1000)      558 2024-04-08 01:10:13.000000 fstumbler-1.1.0/README.md
+drwxr-xr-x   0 ferit     (1000) ferit     (1000)        0 2024-04-14 20:06:39.669051 fstumbler-1.1.0/fstumbler/
+-rw-r--r--   0 ferit     (1000) ferit     (1000)      931 2024-04-14 20:04:26.000000 fstumbler-1.1.0/fstumbler/__init__.py
+-rw-r--r--   0 ferit     (1000) ferit     (1000)     4553 2024-04-14 19:46:27.000000 fstumbler-1.1.0/fstumbler/core.py
+-rw-r--r--   0 ferit     (1000) ferit     (1000)      496 2024-04-14 19:47:26.000000 fstumbler-1.1.0/fstumbler/main.py
+-rw-r--r--   0 ferit     (1000) ferit     (1000)     2180 2024-04-08 12:23:27.000000 fstumbler-1.1.0/fstumbler/node.py
+-rw-r--r--   0 ferit     (1000) ferit     (1000)     1416 2024-04-14 19:46:27.000000 fstumbler-1.1.0/fstumbler/util.py
+drwxr-xr-x   0 ferit     (1000) ferit     (1000)        0 2024-04-14 20:06:39.669051 fstumbler-1.1.0/fstumbler.egg-info/
+-rw-r--r--   0 ferit     (1000) ferit     (1000)     1207 2024-04-14 20:06:39.000000 fstumbler-1.1.0/fstumbler.egg-info/PKG-INFO
+-rw-r--r--   0 ferit     (1000) ferit     (1000)      258 2024-04-14 20:06:39.000000 fstumbler-1.1.0/fstumbler.egg-info/SOURCES.txt
+-rw-r--r--   0 ferit     (1000) ferit     (1000)        1 2024-04-14 20:06:39.000000 fstumbler-1.1.0/fstumbler.egg-info/dependency_links.txt
+-rw-r--r--   0 ferit     (1000) ferit     (1000)       10 2024-04-14 20:06:39.000000 fstumbler-1.1.0/fstumbler.egg-info/top_level.txt
+-rw-r--r--   0 ferit     (1000) ferit     (1000)      618 2024-04-14 20:04:31.000000 fstumbler-1.1.0/pyproject.toml
+-rw-r--r--   0 ferit     (1000) ferit     (1000)       38 2024-04-14 20:06:39.669051 fstumbler-1.1.0/setup.cfg
```

### Comparing `fstumbler-1.0.0/LICENSE` & `fstumbler-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fstumbler-1.0.0/PKG-INFO` & `fstumbler-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fstumbler
-Version: 1.0.0
+Version: 1.1.0
 Summary: The filesystem is a linked list!
 Author-email: "F. Y. BALABAN" <fyb@fybx.dev>
 Project-URL: homepage, https://github.com/fybx/fstumbler
 Project-URL: issues, https://github.com/fybx/fstumbler/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `fstumbler-1.0.0/README.md` & `fstumbler-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `fstumbler-1.0.0/fstumbler/__init__.py` & `fstumbler-1.1.0/fstumbler/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,11 +15,11 @@
 #   You should have received a copy of the GNU Lesser General Public
 #   License along with this library; if not, write to the Free Software
 #   Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301
 #   USA.
 
 from . import fstumbler
 
-VERSION = "1.0.0"
+VERSION = "1.1.0"
 __all__ = [
     "fstumbler",
 ]
```

### Comparing `fstumbler-1.0.0/fstumbler/core.py` & `fstumbler-1.1.0/fstumbler/node.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,77 +15,61 @@
 #   You should have received a copy of the GNU Lesser General Public
 #   License along with this library; if not, write to the Free Software
 #   Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301
 #   USA.
 
 import os
 
-import shutil
 from typing import Optional
-from node import Node
-from util import fast_forward
 
 
-def tumble(root_directory: str) -> Optional[Node]:
-    if not os.path.exists(root_directory):
-        return None
-    
-    full_path = os.path.abspath(root_directory)
-    name = os.path.basename(full_path)
-    root = Node(os.path.dirname(full_path), name)
-    pointer = root
-    
-    for rootname, dirnames, filenames in os.walk(full_path):
-        for filename in filenames:
-            node = Node(rootname, filename, False)
-            pointer.next = node
-            pointer = node
-        
-        for dirname in dirnames:
-            node = Node(rootname, dirname)
-            pointer.next = node
-            pointer = node
-    
-    return root
-
-
-def tree(node: Node):
-    print(node.full_path)
-    if node.next:
-        tree(node.next)
-
-
-def dry_cp(source: Node, destination: Node):
-    if not source.directory:
-        select = fast_forward(destination, True)
-        keep = select.next
-        select.next = source.copyWith(select.parent, select.name, False)
-        select.next.next = keep
-        return
-    
-    pSrc, pDst = source, fast_forward(destination)
-    while pSrc:
-        pDst.next = pSrc.copyWith(pDst.full_path if pDst.directory else pDst.parent,
-                                  pSrc.name, pSrc.directory)
-        pSrc, pDst = pSrc.next, pDst.next
-
-
-def cp(source: Node, destination: Node):
-    if not source.directory:
-        select = fast_forward(destination, True)
-        keep = select.next
-        select.next = source.copyWith(select.parent, select.name, False)
-        select.next.next = keep
-        shutil.copy(source.full_path, select.next.full_path)
-        return
-    
-    pSrc, pDst = source, fast_forward(destination)
-    while pSrc:
-        pDst.next = pSrc.copyWith(pDst.full_path if pDst.directory else pDst.parent,
-                                  pSrc.name, pSrc.directory)
-        
-        if pSrc.directory:
-            os.makedirs(pDst.next.full_path, exist_ok=True)
-        else:
-            shutil.copy(pSrc.full_path, pDst.next.full_path)
-        pSrc, pDst = pSrc.next, pDst.next
-    
+class Node:  
+    def __init__(self, parent: str, name: str, directory=True):
+        self.directory = directory
+        self.name = name
+        self.next: Optional[Node] = None
+        self.parent = parent
+ 
+ 
+    def __str__(self):
+        return self.full_path
+    
+    
+    @property
+    def full_path(self):
+        return os.path.join(self.parent, self.name)
+    
+    
+    def elements(self):
+        if self.directory: 
+            next = self.next
+            count = 0
+            while next:
+                count += 1
+                next = next.next
+                if next and next.directory:
+                    count += 1
+                    break
+            return count
+        return -1
+
+    
+    def ll_count(self) -> int:
+        """Returns the total amount of nodes in this linked list.
+
+        Returns:
+            int: 1 by default.
+        """
+        count = 1
+        pointer = self.next
+        while pointer:
+            count += 1
+            pointer = pointer.next
+        return count
+
+
+    def copy(self):
+        return Node(self.parent, self.name, self.directory)
+
+    def copyWith(self, parent: str, name: str, directory=True):
+        return Node(parent if parent else self.parent,
+                    name if name else self.name, directory)
```

### Comparing `fstumbler-1.0.0/fstumbler/util.py` & `fstumbler-1.1.0/fstumbler/util.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,7 +28,16 @@
     return temp
 
 def __fast_forward(node: Node):
     temp = node
     while temp.next:
         temp = temp.next
     return temp
+
+def contains(str: str, any: list[str]):
+    for some in any:
+        if some in str:
+            return True
+    return False
+
+def level_diff(str1: str, str2: str) -> int:
+    return str1.count('/') - str2.count('/')
```

### Comparing `fstumbler-1.0.0/fstumbler.egg-info/PKG-INFO` & `fstumbler-1.1.0/fstumbler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fstumbler
-Version: 1.0.0
+Version: 1.1.0
 Summary: The filesystem is a linked list!
 Author-email: "F. Y. BALABAN" <fyb@fybx.dev>
 Project-URL: homepage, https://github.com/fybx/fstumbler
 Project-URL: issues, https://github.com/fybx/fstumbler/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `fstumbler-1.0.0/pyproject.toml` & `fstumbler-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fstumbler"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
     { name = "F. Y. BALABAN", email = "fyb@fybx.dev" },
 ]
 description = "The filesystem is a linked list!"
 readme = "README.md"
 requires-python = ">3.7"
 classifiers = [
```

