# Comparing `tmp/silicon-analyser-1.0.3.tar.gz` & `tmp/silicon_analyser-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silicon-analyser-1.0.3.tar", last modified: Sat Apr 13 08:20:05 2024, max compression
+gzip compressed data, was "silicon_analyser-1.0.4.tar", last modified: Sun Apr 14 09:46:57 2024, max compression
```

## Comparing `silicon-analyser-1.0.3.tar` & `silicon_analyser-1.0.4.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 08:20:04.000000 silicon-analyser-1.0.3/
--rw-rw-rw-   0        0        0     1087 2024-04-07 16:13:23.000000 silicon-analyser-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     2622 2024-04-13 08:20:05.000000 silicon-analyser-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1841 2024-04-13 07:40:59.000000 silicon-analyser-1.0.3/README.md
--rw-rw-rw-   0        0        0     1141 2024-04-13 08:19:53.000000 silicon-analyser-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-13 08:20:05.000000 silicon-analyser-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-13 08:20:04.000000 silicon-analyser-1.0.3/silicon_analyser/
-drwxrwxrwx   0        0        0        0 2024-04-13 08:20:04.000000 silicon-analyser-1.0.3/silicon_analyser/dialogs/
--rw-rw-rw-   0        0        0     3444 2024-04-10 15:06:41.000000 silicon-analyser-1.0.3/silicon_analyser/dialogs/compute_stats.py
--rw-rw-rw-   0        0        0     1508 2024-04-06 18:45:56.000000 silicon-analyser-1.0.3/silicon_analyser/dialogs/compute_stats.ui
--rw-rw-rw-   0        0        0     2950 2024-04-11 17:04:32.000000 silicon-analyser-1.0.3/silicon_analyser/grid.py
-drwxrwxrwx   0        0        0        0 2024-04-13 08:20:04.000000 silicon-analyser-1.0.3/silicon_analyser/helper/
-drwxrwxrwx   0        0        0        0 2024-04-13 08:20:04.000000 silicon-analyser-1.0.3/silicon_analyser/helper/abstract/
--rw-rw-rw-   0        0        0     2305 2024-04-11 17:08:12.000000 silicon-analyser-1.0.3/silicon_analyser/helper/abstract/abstractimage.py
--rw-rw-rw-   0        0        0     2693 2024-04-13 07:27:03.000000 silicon-analyser-1.0.3/silicon_analyser/helper/abstract/abstractmywindow.py
--rw-rw-rw-   0        0        0     1024 2024-04-13 06:54:26.000000 silicon-analyser-1.0.3/silicon_analyser/helper/abstract/abstracttreehelper.py
--rw-rw-rw-   0        0        0      719 2024-04-13 07:29:28.000000 silicon-analyser-1.0.3/silicon_analyser/helper/addgridbtn.py
--rw-rw-rw-   0        0        0      696 2024-04-08 17:17:53.000000 silicon-analyser-1.0.3/silicon_analyser/helper/addlabelbtn.py
--rw-rw-rw-   0        0        0     1310 2024-04-13 08:15:14.000000 silicon-analyser-1.0.3/silicon_analyser/helper/ai.py
--rw-rw-rw-   0        0        0    14281 2024-04-11 17:16:10.000000 silicon-analyser-1.0.3/silicon_analyser/helper/computebtn.py
--rw-rw-rw-   0        0        0    19934 2024-04-13 08:19:36.000000 silicon-analyser-1.0.3/silicon_analyser/helper/fullimage.py
--rw-rw-rw-   0        0        0     1520 2024-04-13 07:43:17.000000 silicon-analyser-1.0.3/silicon_analyser/helper/minimap.py
--rw-rw-rw-   0        0        0     3353 2024-04-08 17:17:18.000000 silicon-analyser-1.0.3/silicon_analyser/helper/properties.py
--rw-rw-rw-   0        0        0    16134 2024-04-13 07:03:47.000000 silicon-analyser-1.0.3/silicon_analyser/helper/tree.py
--rw-rw-rw-   0        0        0      263 2024-04-08 17:15:10.000000 silicon-analyser-1.0.3/silicon_analyser/main.py
--rw-rw-rw-   0        0        0     6523 2024-04-11 17:42:11.000000 silicon-analyser-1.0.3/silicon_analyser/main_window.ui
--rw-rw-rw-   0        0        0     8618 2024-04-13 07:34:30.000000 silicon-analyser-1.0.3/silicon_analyser/mywindow.py
--rw-rw-rw-   0        0        0      134 2024-04-07 08:11:27.000000 silicon-analyser-1.0.3/silicon_analyser/rect.py
--rw-rw-rw-   0        0        0     2043 2024-04-13 06:38:05.000000 silicon-analyser-1.0.3/silicon_analyser/savefiles.py
--rw-rw-rw-   0        0        0     1279 2024-04-05 16:48:05.000000 silicon-analyser-1.0.3/silicon_analyser/treeitem.py
-drwxrwxrwx   0        0        0        0 2024-04-13 08:20:04.000000 silicon-analyser-1.0.3/silicon_analyser.egg-info/
--rw-rw-rw-   0        0        0     2622 2024-04-13 08:20:05.000000 silicon-analyser-1.0.3/silicon_analyser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      998 2024-04-13 08:20:05.000000 silicon-analyser-1.0.3/silicon_analyser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 08:20:05.000000 silicon-analyser-1.0.3/silicon_analyser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-04-13 08:20:05.000000 silicon-analyser-1.0.3/silicon_analyser.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2024-04-13 08:20:05.000000 silicon-analyser-1.0.3/silicon_analyser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-13 08:20:04.000000 silicon-analyser-1.0.3/silicon_analyser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-14 09:46:56.000000 silicon_analyser-1.0.4/
+-rw-rw-rw-   0        0        0     1087 2024-04-07 16:13:23.000000 silicon_analyser-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2770 2024-04-14 09:46:57.000000 silicon_analyser-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1989 2024-04-14 09:44:53.000000 silicon_analyser-1.0.4/README.md
+-rw-rw-rw-   0        0        0     1141 2024-04-13 12:59:51.000000 silicon_analyser-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-14 09:46:57.000000 silicon_analyser-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-14 09:46:56.000000 silicon_analyser-1.0.4/silicon_analyser/
+drwxrwxrwx   0        0        0        0 2024-04-14 09:46:56.000000 silicon_analyser-1.0.4/silicon_analyser/dialogs/
+-rw-rw-rw-   0        0        0     3487 2024-04-13 14:15:10.000000 silicon_analyser-1.0.4/silicon_analyser/dialogs/compute_stats.py
+-rw-rw-rw-   0        0        0     1508 2024-04-06 18:45:56.000000 silicon_analyser-1.0.4/silicon_analyser/dialogs/compute_stats.ui
+-rw-rw-rw-   0        0        0     3340 2024-04-14 09:21:04.000000 silicon_analyser-1.0.4/silicon_analyser/dialogs/pixel_image.py
+-rw-rw-rw-   0        0        0     3752 2024-04-14 09:20:00.000000 silicon_analyser-1.0.4/silicon_analyser/dialogs/pixel_image.ui
+-rw-rw-rw-   0        0        0     3052 2024-04-14 07:08:53.000000 silicon_analyser-1.0.4/silicon_analyser/grid.py
+drwxrwxrwx   0        0        0        0 2024-04-14 09:46:56.000000 silicon_analyser-1.0.4/silicon_analyser/helper/
+drwxrwxrwx   0        0        0        0 2024-04-14 09:46:56.000000 silicon_analyser-1.0.4/silicon_analyser/helper/abstract/
+-rw-rw-rw-   0        0        0     2313 2024-04-13 13:47:07.000000 silicon_analyser-1.0.4/silicon_analyser/helper/abstract/abstractimage.py
+-rw-rw-rw-   0        0        0     2771 2024-04-14 06:57:02.000000 silicon_analyser-1.0.4/silicon_analyser/helper/abstract/abstractmywindow.py
+-rw-rw-rw-   0        0        0     1024 2024-04-13 06:54:26.000000 silicon_analyser-1.0.4/silicon_analyser/helper/abstract/abstracttreehelper.py
+-rw-rw-rw-   0        0        0      719 2024-04-13 07:29:28.000000 silicon_analyser-1.0.4/silicon_analyser/helper/addgridbtn.py
+-rw-rw-rw-   0        0        0      696 2024-04-08 17:17:53.000000 silicon_analyser-1.0.4/silicon_analyser/helper/addlabelbtn.py
+-rw-rw-rw-   0        0        0     1304 2024-04-13 14:13:44.000000 silicon_analyser-1.0.4/silicon_analyser/helper/ai.py
+-rw-rw-rw-   0        0        0    14402 2024-04-13 13:49:48.000000 silicon_analyser-1.0.4/silicon_analyser/helper/computebtn.py
+-rw-rw-rw-   0        0        0    20548 2024-04-14 09:34:44.000000 silicon_analyser-1.0.4/silicon_analyser/helper/fullimage.py
+-rw-rw-rw-   0        0        0     1532 2024-04-13 13:40:26.000000 silicon_analyser-1.0.4/silicon_analyser/helper/minimap.py
+-rw-rw-rw-   0        0        0     3499 2024-04-13 13:39:46.000000 silicon_analyser-1.0.4/silicon_analyser/helper/properties.py
+-rw-rw-rw-   0        0        0    18798 2024-04-14 08:01:35.000000 silicon_analyser-1.0.4/silicon_analyser/helper/tree.py
+-rw-rw-rw-   0        0        0      263 2024-04-08 17:15:10.000000 silicon_analyser-1.0.4/silicon_analyser/main.py
+-rw-rw-rw-   0        0        0     6663 2024-04-14 06:53:38.000000 silicon_analyser-1.0.4/silicon_analyser/main_window.ui
+-rw-rw-rw-   0        0        0     8907 2024-04-14 06:57:21.000000 silicon_analyser-1.0.4/silicon_analyser/mywindow.py
+-rw-rw-rw-   0        0        0      134 2024-04-07 08:11:27.000000 silicon_analyser-1.0.4/silicon_analyser/rect.py
+-rw-rw-rw-   0        0        0     2053 2024-04-13 13:22:20.000000 silicon_analyser-1.0.4/silicon_analyser/savefiles.py
+-rw-rw-rw-   0        0        0     1365 2024-04-13 14:16:41.000000 silicon_analyser-1.0.4/silicon_analyser/treeitem.py
+drwxrwxrwx   0        0        0        0 2024-04-14 09:46:56.000000 silicon_analyser-1.0.4/silicon_analyser.egg-info/
+-rw-rw-rw-   0        0        0     2770 2024-04-14 09:46:56.000000 silicon_analyser-1.0.4/silicon_analyser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1078 2024-04-14 09:46:56.000000 silicon_analyser-1.0.4/silicon_analyser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 09:46:56.000000 silicon_analyser-1.0.4/silicon_analyser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-04-14 09:46:56.000000 silicon_analyser-1.0.4/silicon_analyser.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2024-04-14 09:46:56.000000 silicon_analyser-1.0.4/silicon_analyser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-14 09:46:56.000000 silicon_analyser-1.0.4/silicon_analyser.egg-info/top_level.txt
```

### Comparing `silicon-analyser-1.0.3/LICENSE` & `silicon_analyser-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `silicon-analyser-1.0.3/PKG-INFO` & `silicon_analyser-1.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silicon-analyser
-Version: 1.0.3
+Version: 1.0.4
 Summary: helps to analyse integrated circuit die images (for example from siliconpr0n.org) with the help of ai.
 Author-email: CrazyT <crazyt2019+sa@gmail.com>
 Project-URL: Homepage, https://github.com/TheCrazyT/SiliconAnalyser
 Project-URL: Bug Tracker, https://github.com/TheCrazyT/SiliconAnalyser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -61,15 +61,22 @@
       * the amount of cells you selected
       * how good your grid matches the current image
       * the quality of your image
       * ...
     * "acc" stands for "accuracy", "val" for "validation"
 * found ai-cells will be drawn green
 
+# Keys
+
+* Use up/down/left/right to navigate
+* Hold shift to move faster
+* Scroll-wheel to zoom out
+* Click on minimap to get directly to a position
+
 ![image](https://raw.githubusercontent.com/TheCrazyT/SiliconAnalyser/main/docs/small_tutorial.gif)
 
 # TODO
 
-* export of ai-cells as bit-image
 * auto-compute to calculate in background while you are selecting new cells for your labels
+* ai-model configuration
 * possibility to rotate grid
 * maybe store your model on a public place? (for others to use)
```

### Comparing `silicon-analyser-1.0.3/README.md` & `silicon_analyser-1.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -40,15 +40,22 @@
       * the amount of cells you selected
       * how good your grid matches the current image
       * the quality of your image
       * ...
     * "acc" stands for "accuracy", "val" for "validation"
 * found ai-cells will be drawn green
 
+# Keys
+
+* Use up/down/left/right to navigate
+* Hold shift to move faster
+* Scroll-wheel to zoom out
+* Click on minimap to get directly to a position
+
 ![image](https://raw.githubusercontent.com/TheCrazyT/SiliconAnalyser/main/docs/small_tutorial.gif)
 
 # TODO
 
-* export of ai-cells as bit-image
 * auto-compute to calculate in background while you are selecting new cells for your labels
+* ai-model configuration
 * possibility to rotate grid
 * maybe store your model on a public place? (for others to use)
```

### Comparing `silicon-analyser-1.0.3/pyproject.toml` & `silicon_analyser-1.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "silicon-analyser"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="CrazyT", email="crazyt2019+sa@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `silicon-analyser-1.0.3/silicon_analyser/dialogs/compute_stats.py` & `silicon_analyser-1.0.4/silicon_analyser/dialogs/compute_stats.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+import typing
 from PyQt5 import uic
 from PyQt5 import QtGui
 from PyQt5.QtCore import pyqtSignal
 from PyQt5.QtWidgets import QDialog, QLabel, QPushButton
 from pyqtgraph import PlotWidget
 from numpy import linspace
 import os.path as p
 
 class ComputeStatsDlg(QDialog):
     _lossgraph: PlotWidget
     _accuracygraph: PlotWidget
-    _loss: any
-    _val_loss: any
-    _accuracy: any
-    _val_accuracy: any
+    _loss: typing.Any
+    _val_loss: typing.Any
+    _accuracy: typing.Any
+    _val_accuracy: typing.Any
     _lblStatus: QLabel
     _btnStop: QPushButton
     request_graph_update = pyqtSignal([dict,int])
     
     def __init__(self):
         super().__init__()
         uic.loadUi(p.abspath(p.join(p.dirname(__file__), '.')) + '/compute_stats.ui', self)
```

### Comparing `silicon-analyser-1.0.3/silicon_analyser/dialogs/compute_stats.ui` & `silicon_analyser-1.0.4/silicon_analyser/dialogs/compute_stats.ui`

 * *Files identical despite different names*

### Comparing `silicon-analyser-1.0.3/silicon_analyser/grid.py` & `silicon_analyser-1.0.4/silicon_analyser/grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 class Grid:
-    _rects: dict[list[list[int]]]
-    _rectsActive: dict[bool]
+    _rects: dict[str,list[list[int]]]
+    _rectsActive: dict[str,bool]
     def __init__(self, name, x, y, cols, rows, width, height):
         self.name = name
         self.x = x
         self.y = y
         self.cols = cols
         self.rows = rows
         self.width = width
@@ -24,15 +24,15 @@
         for k in self._rects:
             for cx,cy in list(self._rects[k]):
                 if cx < 0 or cy < 0:
                     self._rects[k].remove([cx,cy])
         self._rectsActive = grid._rectsActive
         
     def getLabels(self) -> list[str]:
-        return self._rects.keys()
+        return list(self._rects.keys())
     
     def removeRectGroup(self, label):
         del self._rects[label]
         del self._rectsActive[label]
     
     def addRectGroup(self, text):
         self._rects[text] = []
@@ -63,15 +63,15 @@
         
     def unsetRect(self, col, row, label):
         print(f"unsetRect {col} {row}")
         r = [col, row]
         if r in self._rects[label]:
             self._rects[label].remove(r)
     
-    def rectLabel(self, col, row) -> str:
+    def rectLabel(self, col, row) -> str|None:
         r = [col, row]
         keys = self._rects.keys()
         for k in keys:
             if self._rectsActive[k]:
                 if r in self._rects[k]:
                     return k
     
@@ -82,15 +82,17 @@
         else:
             keys = [key]
         for k in keys:
             if self._rectsActive[k]:
                 if r in self._rects[k]:
                     return True
         return False
-    
+
+    def getRects(self, key: str) -> list[list[int]]:
+        return self._rects[key]
     
 def getAllCellRects(grid: Grid):
     cellRects = []
     for cx in range(0,grid.cols):
         for cy in range(0,grid.rows):
             cellRects.append((cx,cy))
     return cellRects
```

### Comparing `silicon-analyser-1.0.3/silicon_analyser/helper/abstract/abstractimage.py` & `silicon_analyser-1.0.4/silicon_analyser/helper/abstract/abstractimage.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,18 +58,18 @@
     
     def appendAIGrid(self, text):
         raise NotImplementedError()
     
     def activateAIGrid(self, text):
         raise NotImplementedError()
     
-    def getRects(self) -> list[Rect]:
+    def getRects(self) -> dict[str,Rect]:
         raise NotImplementedError()
     
-    def getGrids(self) -> dict[Grid]:
+    def getGrids(self) -> dict[str,Grid]:
          raise NotImplementedError()
     
     def removeRectGroup(self, label):
         raise NotImplementedError()
     
     def removeGrid(self, label):
         raise NotImplementedError()
```

### Comparing `silicon-analyser-1.0.3/silicon_analyser/helper/abstract/abstractmywindow.py` & `silicon_analyser-1.0.4/silicon_analyser/helper/abstract/abstractmywindow.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from PyQt5.QtWidgets import QMainWindow, QPushButton
+from PyQt5.QtCore import QItemSelection
+from PyQt5.QtWidgets import QMainWindow, QPushButton, QAction
 from PyQt5.QtGui import QStandardItem
-from PyQt5.QtWidgets import QAction
 
 from silicon_analyser.helper.abstract.abstractimage import AbstractImage
 from silicon_analyser.helper.abstract.abstracttreehelper import AbstractTreeHelper
 
 class AbstractMyWindow(QMainWindow):
     _actionGridAddRowTop: QAction
     _actionSaveModel: QAction
     _actionLoadModel: QAction
     _actionRemoveGrid: QAction
     _actionRemoveLabel: QAction
     _actionSaveAsCsv: QAction
+    _actionViewAsPixelimage: QAction
     autosave: bool
     def __init__(self):
         QMainWindow.__init__(self)
         
     def getManualItem(self) -> QStandardItem:
         raise NotImplementedError()
     
@@ -69,15 +70,15 @@
 
     def imageHeight(self):
         raise NotImplementedError()
     
     def reloadProperyWindowByGrid(self, grid):
         raise NotImplementedError()
     
-    def reloadPropertyWindow(self):
+    def reloadPropertyWindow(self, selection: QItemSelection):
         raise NotImplementedError()
     
     def getImage(self) -> AbstractImage:
         raise NotImplementedError()
     
     def getAIItem(self) -> QStandardItem:
         raise NotImplementedError()
```

### Comparing `silicon-analyser-1.0.3/silicon_analyser/helper/abstract/abstracttreehelper.py` & `silicon_analyser-1.0.4/silicon_analyser/helper/abstract/abstracttreehelper.py`

 * *Files identical despite different names*

### Comparing `silicon-analyser-1.0.3/silicon_analyser/helper/addgridbtn.py` & `silicon_analyser-1.0.4/silicon_analyser/helper/addgridbtn.py`

 * *Files identical despite different names*

### Comparing `silicon-analyser-1.0.3/silicon_analyser/helper/addlabelbtn.py` & `silicon_analyser-1.0.4/silicon_analyser/helper/addlabelbtn.py`

 * *Files identical despite different names*

### Comparing `silicon-analyser-1.0.3/silicon_analyser/helper/ai.py` & `silicon_analyser-1.0.4/silicon_analyser/helper/ai.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     if maxH % MP != 0:
         maxH += MP - (maxH % MP)
     return maxW, maxH
 
 def appendFoundCellRects(img: AbstractImage, grid: Grid, aiGrid: Grid, maxW, maxH, model: keras.Sequential):
     if maxW is None or maxH is None:
         maxW, maxH = getDefaultMaxWMaxH(grid)
-    labels = list(grid.getLabels())
+    labels = grid.getLabels()
     allCellRects = getAllCellRects(grid)
     dataList = []
     dataIndexes = []
     for cx,cy in allCellRects:
         x = int(grid.x + cx*maxW)
         y = int(grid.y + cy*maxH)
         ex = x + maxW - 1
```

### Comparing `silicon-analyser-1.0.3/silicon_analyser/helper/computebtn.py` & `silicon_analyser-1.0.4/silicon_analyser/helper/computebtn.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,45 +88,48 @@
                 subdataIdx += 1
 
         class MyPlottingCallback(keras.callbacks.Callback):
             def __init__(self, plotDlg: ComputeStatsDlg):
                 self._plotDlg = plotDlg
             
             def on_epoch_end(self, epoch, logs=None): 
+                if logs is None:
+                    return
                 self._plotDlg.request_graph_update.emit(logs, epoch)
                 if self._plotDlg.isStop():
-                    self.model.stop_training = True
+                    self.model.stop_training = True # type: ignore
             
         class MyThresholdCallback(keras.callbacks.Callback):
             def __init__(self, threshold, patience):
                 super(MyThresholdCallback, self).__init__()
                 self.threshold = threshold
                 self.patience = patience
                 self.count = 0
 
             def on_epoch_end(self, epoch, logs=None): 
+                if logs is None:
+                    return
                 val_acc = logs["val_accuracy"]
                 if val_acc >= self.threshold:
                     if self.count > self.patience:
-                        self.model.stop_training = True
+                        self.model.stop_training = True # type: ignore
                     else:
                         self.count += 1
                 else:
                     self.count = 0
         
         print("_worker runs")
         try:
             self._computeStatsDlg.reset()
             selectedType = self._myWindow.getTree().selectedType()
             gridMode = (selectedType == TreeItem.TYPE_GRID) or (selectedType == TreeItem.TYPE_GRID_ITEM) or (selectedType == TreeItem.TYPE_AI_GRID) or (selectedType == TreeItem.TYPE_AI_GRID_ITEM)
             rects = self._myWindow.getImage().getRects()
             ignoreRects = self._myWindow.getImage().getAIIgnoreRects()
             self._myWindow.setStatusText("training in progress")
 
-            grid = None        
             if gridMode:
                 grid: Grid = self._myWindow.getTree().getSelectedGrid()
                 maxW, maxH, labels, countGroups, MP, train, vals = self.initTrainAndValsForGrid(grid)
             else:
                 maxW, maxH, countGroups, MP, train, vals = self.initTrainAndValsForRects(rects, ignoreRects)
 
             model_conv, model_train = self.createModels(keras, countGroups, maxW, maxH, MP)
```

### Comparing `silicon-analyser-1.0.3/silicon_analyser/helper/fullimage.py` & `silicon_analyser-1.0.4/silicon_analyser/helper/fullimage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from PyQt5.QtCore import Qt, QRect, QSize, QTimer
 from PyQt5.QtWidgets import QLabel, QSizePolicy
 from PyQt5.QtGui import QImage, QPixmap, QColor, QMouseEvent, QPainter, QPen, QBrush
 import numpy as np
 from silicon_analyser.helper.abstract.abstractmywindow import AbstractMyWindow
-from silicon_analyser.savefiles import saveGrids,saveRects
+from silicon_analyser.savefiles import triggerSaveGrids, triggerSaveRects, saveGrids, saveRects
 from silicon_analyser.grid import Grid
 from silicon_analyser.rect import Rect
 from silicon_analyser.treeitem import TreeItem
 
 class FullImage(QLabel):
-    _rects: dict[Rect]
-    _aiRects: dict[Rect]
-    _rectActive: dict[bool]
-    _grids: dict[Grid]
-    _aiGrids: dict[Grid]
-    _gridsActive: dict[bool]
-    _aiGridsActive: dict[bool]
+    _rects: dict[str, list[Rect]]
+    _aiRects: dict[str, list[Rect]]
+    _rectActive: dict[str, bool]
+    _grids: dict[str, Grid]
+    _aiGrids: dict[str, Grid]
+    _gridsActive: dict[str, bool]
+    _aiGridsActive: dict[str, bool]
     _moveStartX: int
     _moveStartY: int
     _moveDeltaX: int
     _moveDeltaY: int
     _moveTimer: QTimer
+    _saveTimer: QTimer
     
     def __init__(self, parent):
         QLabel.__init__(self, parent)
         self._drawRectStart = False
         self._rectStartX = 0
         self._rectStartY = 0
         self._rectEndX = 0
@@ -39,32 +40,40 @@
         self._aiRectActive = {}
         self._aiIgnoreRects = []
         self.setSizePolicy(QSizePolicy.Policy.Expanding,QSizePolicy.Policy.Expanding)
         self._moveTimer = QTimer()
         self._moveTimer.timeout.connect(self.moveUpdate)
         self._moveTimer.setInterval(int(1000 * 0.2))
         self._moveStart = False
-    
+        self._saveTimer = QTimer()
+        self._saveTimer.timeout.connect(self.doSave)
+        self._saveTimer.setInterval(int(1000 * 10)) #save every 10 seconds
+        self._saveTimer.start()
+    
+    def doSave(self):
+        saveRects(self._rects)
+        saveGrids(self._grids)
+        
     def moveUpdate(self):
         posX, posY = self._myWindow.getPos()
         posX += self._moveDeltaX
         posY += self._moveDeltaY
         self._myWindow.setPosX(posX)
         self._myWindow.setPosY(posY)
         self._myWindow.drawImgAndMinimap()
     
     def initialize(self, myWindow: AbstractMyWindow, pixmap: QPixmap):
         self._myWindow = myWindow
         self._pixmap: QPixmap = pixmap
         self._currentImg = pixmap
     
-    def getRects(self) -> list[Rect]:
+    def getRects(self) -> dict[str,list[Rect]]:
         return self._rects
     
-    def getAiRects(self) -> list[Rect]:
+    def getAiRects(self) -> dict[str,list[Rect]]:
         return self._aiRects
     
     def getAIIgnoreRects(self) -> list:
         return self._aiIgnoreRects
     
     def markGridItem(self,evx,evy,button):
         scale = self._myWindow.getScale()
@@ -81,41 +90,41 @@
                 if ex<x:
                     x,ex = ex,x
                 if ey<y:
                     y,ey = ey,y
                 if x < evx and y < evy and ex > evx and ey > evy:
                     tevx = self._translateEventToPixel(evx)
                     tevy = self._translateEventToPixel(evy)
-                    if button == Qt.LeftButton:
+                    if button == Qt.MouseButton.LeftButton:
                         grid.setRect(int((tevx - (grid.x - posX))/(grid.width/grid.cols)),int((tevy - (grid.y - posY))/(grid.height/grid.rows)), self._myWindow.getTree().selectedLabel())
-                    if button == Qt.RightButton:
+                    if button == Qt.MouseButton.RightButton:
                         grid.unsetRect(int((tevx - (grid.x - posX))/(grid.width/grid.cols)),int((tevy - (grid.y - posY))/(grid.height/grid.rows)), self._myWindow.getTree().selectedLabel())
                     if self._myWindow.autosave:
-                        saveGrids(self._grids)
+                        triggerSaveGrids()
                     
     def mousePressEvent(self, event: QMouseEvent):
-        if event.button() == Qt.MiddleButton:
+        if event.button() == Qt.MouseButton.MiddleButton:
             self._moveStart = True
             self._moveStartX = event.x()
             self._moveStartY = event.y()
             self._moveDeltaX = 0
             self._moveDeltaY = 0
         tree = self._myWindow.getTree()
         if tree.selectedType() == TreeItem.TYPE_GRID_ITEM:
             self.markGridItem(event.x(),event.y(),event.button())
             return
-        if event.button() == Qt.LeftButton:
+        if event.button() == Qt.MouseButton.LeftButton:
             print("FullImage: mousePressEvent",self._drawRectStart)
             if tree.selectedType() is not None:
                 if not self._drawRectStart:
                     self._drawRectStart = True
                     self._rectStartX = self._translateEventToPixel(event.x())
                     self._rectStartY = self._translateEventToPixel(event.y())
     
-    def mouseMoveEvent(self, event: QMouseEvent | None) -> None:
+    def mouseMoveEvent(self, event: QMouseEvent) -> None:
         if self._moveStart:
             self._moveDeltaX = event.x() - self._moveStartX
             self._moveDeltaY = event.y() - self._moveStartY
             self._moveTimer.start()
 
         if self._drawRectStart:
             self._rectEndX = self._translateEventToPixel(event.x())
@@ -123,31 +132,31 @@
             if(self._rectEndX < self._rectStartX):
                 self._rectEndX, self._rectStartX = self._rectStartX, self._rectEndX
             if(self._rectEndY < self._rectStartY):
                 self._rectEndY, self._rectStartY = self._rectStartY, self._rectEndY
             pixmap = self._currentImg.copy()
             qp = QPainter(pixmap)
             brush = QBrush(QColor(255,0,0,127))
-            pen = QPen(Qt.red, 2)
+            pen = QPen(Qt.GlobalColor.red, 2)
             qp.setBrush(brush)
             qp.setPen(pen)
             qp.drawRect(
                 self._translatePixelToScaled(self._rectStartX),
                 self._translatePixelToScaled(self._rectStartY),
                 self._translatePixelToScaled(self._rectEndX)-self._translatePixelToScaled(self._rectStartX),
                 self._translatePixelToScaled(self._rectEndY)-self._translatePixelToScaled(self._rectStartY))
             qp.end()
             self.setPixmap(pixmap)
      
     def mouseReleaseEvent(self, event: QMouseEvent):
-        if event.button() == Qt.MiddleButton:
+        if event.button() == Qt.MouseButton.MiddleButton:
             self._moveStart = False
             self._moveTimer.stop()
             
-        if event.button() == Qt.LeftButton:
+        if event.button() == Qt.MouseButton.LeftButton:
             self._drawRectStart = False
             print("mouseReleaseEvent",self._rectStartX,self._rectStartY,self._rectEndX,self._rectEndY)
             selectedKey: str = self._myWindow.getTree().selectedLabel()
             if selectedKey is not None:
                 x = self._rectStartX
                 y = self._rectStartY
                 ex = self._rectEndX
@@ -161,17 +170,17 @@
                     grid.y = posY+y
                     grid.width = ex-x
                     grid.height = ey-y
                     self._grids[selectedKey] = grid
                     print(f"grid resized: {id(grid)}")
                     self._myWindow.reloadProperyWindowByGrid(grid)
                     if self._myWindow.autosave:
-                        saveGrids(self._grids)
+                        triggerSaveGrids()
                 self.drawImage()
-        if event.button() == Qt.RightButton:
+        if event.button() == Qt.MouseButton.RightButton:
             print("right click")
             self.removeRectAt(event.x(),event.y())
             
     def removeRectGroup(self, label):
         del self._rects[label]
         del self._aiRects[label]
         del self._rectActive[label]
@@ -228,21 +237,21 @@
             for i in sorted(toRemove, reverse=True):
                 print(f"remove {i}")
                 self._aiIgnoreRects.append(self._aiRects[k][i])
                 del self._aiRects[k][i]
                 
         self.drawImage()
         if  self._myWindow.autosave:
-            saveRects(self._rects)
-            saveGrids(self._grids)
+            triggerSaveRects()
+            triggerSaveGrids()
 
     def appendRect(self,key,x,y,ex,ey):
         self._appendRect(key, self._rects, x, y, ex, ey)
         if self._myWindow.autosave:
-            saveRects(self._rects)
+            triggerSaveRects()
 
     def _appendRect(self, key, rects, x, y, ex, ey, ignorePos = False):
         if ignorePos:
             rects[key].append(Rect(
                 x,
                 y,
                 ex,
@@ -260,15 +269,15 @@
     def appendAIRect(self,key,x,y,ex,ey):
         self._appendRect(key, self._aiRects, x, y, ex, ey, True)
 
     def fetchFullData(self):
         temp = QImage(self._pixmap.toImage())
         ptr = temp.constBits()
         ptr.setsize(temp.byteCount())
-        arr = np.frombuffer(ptr, dtype=np.ubyte).reshape(temp.height(), temp.width(), 4)
+        arr = np.frombuffer(ptr, dtype=np.ubyte).reshape(temp.height(), temp.width(), 4) # type: ignore
         return arr
     
     def fetchData(self,x,y,ex,ey):
         x = int(x)
         ex = int(ex)
         y = int(y)
         ey = int(ey)
@@ -296,29 +305,29 @@
         self._aiGrids = {}
         self._aiRects = {}
         self._aiRectActive = {}
     
     def drawRectOnScaledImg(self, scaledImg: QPixmap):
         qp = QPainter(scaledImg)
         brush = QBrush(QColor(0,0,255,80))
-        pen = QPen(Qt.blue, 2)
+        pen = QPen(Qt.GlobalColor.blue, 2)
         qp.setBrush(brush)
         qp.setPen(pen)
         self._drawRectOnScaledImg(self._rects, self._rectActive, qp)
         brush = QBrush(QColor(0,255,0,80))
-        pen = QPen(Qt.green, 2)
+        pen = QPen(Qt.GlobalColor.green, 2)
         qp.setBrush(brush)
         qp.setPen(pen)
         self._drawRectOnScaledImg(self._aiRects, self._aiRectActive, qp)
         qp.end()
         
     def drawGridOnScaledImg(self, scaledImg: QPixmap):
         qp = QPainter(scaledImg)
         brush = QBrush(QColor(0,0,255,80))
-        pen = QPen(Qt.blue, 2)
+        pen = QPen(Qt.GlobalColor.blue, 2)
         qp.setBrush(brush)
         qp.setPen(pen)
         self._drawGridOnScaledImg(self._grids, self._gridsActive, qp, TreeItem.TYPE_GRID_ITEM)
 
         brush = QBrush(QColor(0,255,0,80))
         pen = QPen(QColor(0,0,0,0), 2)
         qp.setBrush(brush)
@@ -348,15 +357,15 @@
         endCol = max(int(startCol + maxColsCnt),endCol)
         endRow = max(int(startRow + maxRowsCnt),endRow)
         endCol = int(min(endCol, grid.cols))
         endRow = int(min(endRow, grid.rows))
         
         return (startCol, startRow, endCol, endRow)
         
-    def getGrids(self) -> dict[Grid]:
+    def getGrids(self) -> dict[str,Grid]:
         return self._grids
         
     def _drawGridOnScaledImg(self, grids, gridsActive, qp:QPainter, gridItemType:str, rectSetColor:QColor = QColor(0,255,255,40), rectSetActiveColor:QColor = QColor(0,255,255,127), rectUnsetColor:QColor = QColor(0,0,255,20)):
         posX, posY = self._myWindow.getPos()
         scale = self._myWindow.getScale()
         sposX, sposY = posX*scale, posY*scale
         for k in grids.keys():
@@ -427,61 +436,61 @@
         return aiGrid
     
     def appendGrid(self, text):
         grid = Grid(text,0,0,20,20,20*10,20*10)
         self._grids[text] = grid
         self._myWindow.reloadProperyWindowByGrid(grid)
         if self._myWindow.autosave:
-            saveGrids(self._grids)
+            triggerSaveGrids()
         return self._grids[text]
     
     def activateAIGrid(self, text):
         self._aiGridsActive[text] = True
         self.drawImage()
 
-    def activateGrid(self, text):
+    def activateGrid(self, text: str):
         self._gridsActive[text] = True
         self.drawImage()
 
-    def deactivateGrid(self, text):
+    def deactivateGrid(self, text: str):
         self._gridsActive[text] = False
         self.drawImage()
     
-    def appendAIGridRectGroup(self, grid: Grid, text):
+    def appendAIGridRectGroup(self, grid: Grid, text: str):
         grid.addRectGroup(text)
     
-    def appendGridRectGroup(self, grid: Grid, text):
+    def appendGridRectGroup(self, grid: Grid, text: str):
         grid.addRectGroup(text)
     
-    def activateAIGridRectGroup(self, grid: Grid, text):
+    def activateAIGridRectGroup(self, grid: Grid, text: str):
         grid.rectActive(text)
 
-    def deactivateAIGridRectGroup(self, grid: Grid, text):
+    def deactivateAIGridRectGroup(self, grid: Grid, text: str):
         grid.rectDeactive(text)
 
-    def activateGridRectGroup(self, grid: Grid, text):
+    def activateGridRectGroup(self, grid: Grid, text: str):
         grid.rectActive(text)
 
-    def deactivateGridRectGroup(self, grid: Grid, text):
+    def deactivateGridRectGroup(self, grid: Grid, text: str):
         grid.rectDeactive(text)
 
-    def appendRectGroup(self, text):
+    def appendRectGroup(self, text: str):
         self._rects[text] = []
     
-    def activateRectGroup(self, text):
+    def activateRectGroup(self, text: str):
         self._rectActive[text] = True
         self.drawImage()
 
-    def deactivateRectGroup(self, text):
+    def deactivateRectGroup(self, text: str):
         self._rectActive[text] = False
         self.drawImage()
         
-    def appendAIRectGroup(self, text):
+    def appendAIRectGroup(self, text: str):
         self._aiRects[text] = []
     
-    def activateAIRectGroup(self, text):
+    def activateAIRectGroup(self, text: str):
         self._aiRectActive[text] = True
         self.drawImage()
 
-    def deactivateAIRectGroup(self, text):
+    def deactivateAIRectGroup(self, text: str):
         self._aiRectActive[text] = False
         self.drawImage()
```

### Comparing `silicon-analyser-1.0.3/silicon_analyser/helper/minimap.py` & `silicon_analyser-1.0.4/silicon_analyser/helper/minimap.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         return 300/self._pixmap.height()
 
     def drawMinimap(self):
         minimapPm = self._pixmap.scaled(QSize(300, 300))
         posX, posY = self._myWindow.getPos()
         scale = self._myWindow.getScale()
         qp = QPainter(minimapPm)
-        pen = QPen(Qt.red, 2)
+        pen = QPen(Qt.GlobalColor.red, 2)
         qp.setPen(pen)
         sc1x = self.scaleMinimapX()
         sc2x = sc1x/scale
         sc1y = self.scaleMinimapY()
         sc2y = sc1y/scale
         qp.drawRect(int(posX*sc1x),int(posY*sc1y),int(300*sc2x),int(300*sc2y))
         qp.end()
```

### Comparing `silicon-analyser-1.0.3/silicon_analyser/helper/properties.py` & `silicon_analyser-1.0.4/silicon_analyser/helper/properties.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+import typing
 from PyQt5.QtWidgets import QTableView
-from PyQt5.QtCore import QItemSelection, QModelIndex, Qt
+from PyQt5.QtCore import QItemSelection, QModelIndex, Qt, QAbstractItemModel
 from PyQt5.QtGui import QStandardItem, QStandardItemModel
 from silicon_analyser.savefiles import saveGrids
 from silicon_analyser.grid import Grid
 from silicon_analyser.treeitem import TreeItem
 from silicon_analyser.helper.abstract.abstractmywindow import AbstractMyWindow
 
 class PropertiesUtil:
@@ -14,18 +15,18 @@
     
     def dataChanged(self,*args,**kwargs):
         print("dataChanged")
         valueCol: QModelIndex = args[0]
         if valueCol.column() != 1:
             return
         row = valueCol.row()
-        model: QStandardItemModel = self._properties.model()
+        model: QStandardItemModel = typing.cast(QStandardItemModel,self._properties.model())
         nameCol = model.item(row,0)
-        name = nameCol.data(Qt.DisplayRole)
-        value = valueCol.data(Qt.DisplayRole)
+        name = nameCol.data(Qt.ItemDataRole.DisplayRole)
+        value = valueCol.data(Qt.ItemDataRole.DisplayRole)
         print(name)
         print(value)
         grid: Grid = self._myWindow.getTree().getSelectedGrid()
         if(name == "cols"):
             grid.cols = int(value)
         if(name == "rows"):
             grid.rows = int(value)
@@ -53,15 +54,15 @@
         typeStr = sel.indexes()[0].data(TreeItem.TYPE)
         if(typeStr == TreeItem.TYPE_GRID):
             grid: Grid = sel.indexes()[0].data(TreeItem.OBJECT)
             self.reloadProperyWindowByGrid(grid)
 
     def reloadProperyWindowByGrid(self, grid):
         table: QTableView = self._properties
-        model = table.model()
+        model: QStandardItemModel = typing.cast(QStandardItemModel, table.model())
         rowPosition = model.rowCount()
         model.removeRows(0,model.rowCount())
         model.insertRow(rowPosition,[QStandardItem("name"),QStandardItem(grid.name)])
         if grid is not None:
             rowPosition = model.rowCount()
             model.insertRow(rowPosition,[QStandardItem("x"),QStandardItem(f"{grid.x}")])
             rowPosition = model.rowCount()
```

### Comparing `silicon-analyser-1.0.3/silicon_analyser/helper/tree.py` & `silicon_analyser-1.0.4/silicon_analyser/helper/tree.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,95 +1,126 @@
-from PyQt5.QtCore import QItemSelection, pyqtSignal
+import typing
+from PyQt5.QtCore import QItemSelection, pyqtSignal, QItemSelectionModel
 from PyQt5 import QtCore
 from PyQt5.QtWidgets import QTreeView, QWidget, QAction, QFileDialog
-from PyQt5.QtGui import QStandardItem
+from PyQt5.QtGui import QStandardItem, QStandardItemModel
 from silicon_analyser.helper.abstract.abstractmywindow import AbstractMyWindow
 from silicon_analyser.grid import Grid
 from silicon_analyser.helper.abstract.abstracttreehelper import AbstractTreeHelper
 from silicon_analyser.helper.abstract.abstractimage import AbstractImage
 from silicon_analyser.treeitem import TreeItem
 from silicon_analyser.grid import Grid
+from silicon_analyser.dialogs.pixel_image import PixelImageDlg
 
 class Tree(AbstractTreeHelper):
     _myWindow: AbstractMyWindow
     _actionGridAddRowTop: QAction
     _actionSaveModel: QAction
     _actionLoadModel: QAction
     _actionRemoveGrid: QAction
     _actionRemoveLabel: QAction
     _actionSaveAsCsv: QAction
+    _actionViewAsPixelimage: QAction
+    _pixelImageDlg: PixelImageDlg
     evtTreeSelectionChanged: pyqtSignal = pyqtSignal(QItemSelection)
 
-    def __init__(self, parent: QWidget | None = ...) -> None:
+    def __init__(self, parent: QWidget | None = ...) -> None: # type: ignore
         super().__init__(parent)
     
     def initialize(self, myWindow: AbstractMyWindow):
         self._myWindow = myWindow
         self.selectionModel().selectionChanged.connect(self.treeSelectionChanged)
         self._actionGridAddRowTop = self._myWindow._actionGridAddRowTop
         self._actionSaveModel = self._myWindow._actionSaveModel
         self._actionLoadModel = self._myWindow._actionLoadModel
         self._actionRemoveGrid = self._myWindow._actionRemoveGrid
         self._actionRemoveLabel = self._myWindow._actionRemoveLabel
         self._actionSaveAsCsv = self._myWindow._actionSaveAsCsv
+        self._actionViewAsPixelimage = self._myWindow._actionViewAsPixelimage
         self.addAction(self._actionGridAddRowTop)
         self.addAction(self._actionSaveModel)
         self.addAction(self._actionLoadModel)
         self.addAction(self._actionRemoveGrid)
         self.addAction(self._actionRemoveLabel)
         self.addAction(self._actionSaveAsCsv)
+        self.addAction(self._actionViewAsPixelimage)
         self._actionGridAddRowTop.triggered.connect(self.addTopRow)
         self._actionSaveModel.triggered.connect(self.saveModel)
         self._actionLoadModel.triggered.connect(self.loadModel)
         self._actionRemoveGrid.triggered.connect(self.removeGrid)
         self._actionRemoveLabel.triggered.connect(self.removeLabel)
         self._actionSaveAsCsv.triggered.connect(self.saveAsCsv)
+        self._actionViewAsPixelimage.triggered.connect(self.viewAsPixelimage)
+        self._pixelImageDlg = PixelImageDlg()
+    
+    def viewAsPixelimage(self, *args, **kwargs):
+        print("viewAsPixelimage")
+        grid: Grid|None
+        selectedType = self.selectedType()
+        if selectedType == TreeItem.TYPE_GRID_ITEM:
+            grid = self.getSelectedGrid()
+        elif selectedType == TreeItem.TYPE_AI_GRID_ITEM:
+            grid = self.getSelectedAIGrid()
+        if grid is None:
+            return
+        label = self.selectedLabel()
+        if label is not None: 
+            self._pixelImageDlg.show()
+            self._pixelImageDlg.drawRects(grid.getRects(label))
     
     def saveAsCsv(self, *args, **kwargs):
         print("saveAsCsv")
         dlg = QFileDialog()
         dlg.setLabelText(QFileDialog.DialogLabel.Accept, "Save")
         filenames = []
         filenames = dlg.getSaveFileName(caption="Save csv",filter="Comma separated values (*.csv)",initialFilter="Comma separated values (*.csv)")
         if(len(filenames) >= 1):
-            grid:Grid 
+            grid:Grid|None
             if self.selectedType() == TreeItem.TYPE_GRID:
                 grid = self.getSelectedGrid()
             if self.selectedType() == TreeItem.TYPE_AI_GRID:
                 grid = self.getSelectedAIGrid()
+            if grid is None:
+                return
             with open(filenames[0],"w") as f:
                 for r in range(0,grid.rows):
                     cells = []
                     for c in range(0,grid.cols):
-                        for l in list(grid.getLabels()):
+                        labelFound = False
+                        for l in grid.getLabels():
                             if grid.isRectSet(c,r,l):
+                                labelFound = True
                                 if l.isnumeric():
                                     cells.append(f'{l}')
                                 else:
                                     cells.append(f'"{l}"')
+                                break
+                        if not labelFound:
+                            cells.append(f'')
                     f.write(",".join(cells))
                     f.write("\n")
     
     def saveModel(self, *args, **kwargs):
         print("saveModel")
         dlg = QFileDialog()
         dlg.setLabelText(QFileDialog.DialogLabel.Accept, "Save")
         filenames = []
         filenames = dlg.getSaveFileName(caption="Save trained model",filter="Trained model (*.h5)",initialFilter="Trained model (*.h5)")
         if(len(filenames) >= 1):
             from keras.models import Sequential
             grid = self.getSelectedGrid()
-            model: Sequential = self._myWindow.getModel(grid.name)
-            model.save(filenames[0])
+            if grid is not None:
+                model: Sequential = self._myWindow.getModel(grid.name)
+                model.save(filenames[0])
     
     
     def recreateAiTree(self, grid:Grid):
         self.clearAIItem(grid.name)
         aiGrid, aiTreeItem = self.addTreeItem(grid.name,TreeItem.TYPE_AI_GRID)
-        for l in list(grid.getLabels()):
+        for l in grid.getLabels():
             self.addTreeItem(l,TreeItem.TYPE_AI_GRID_ITEM,aiGrid,aiTreeItem)
         return aiGrid
     
     def loadModel(self, *args, **kwargs):
         print("loadModel")
         myWindow: AbstractMyWindow = self._myWindow
         dlg = QFileDialog()
@@ -97,26 +128,29 @@
         dlg.setNameFilter("Trained model (*.h5)")
         filenames = []
         if dlg.exec_():
             filenames = dlg.selectedFiles()
         if(len(filenames) == 1):
             from keras.models import load_model
             from silicon_analyser.helper.ai import appendFoundCellRects
-            grid: Grid = self.getSelectedGrid()
-            model = load_model(filenames[0])
-            aiGrid = self.recreateAiTree(grid)
-            myWindow.setLastModel(grid.name, model)
-            img: AbstractImage = myWindow.getImage()
-            appendFoundCellRects(img, grid, aiGrid, None, None, model)
-            img.drawImage()
+            grid: Grid|None = self.getSelectedGrid()
+            if grid is not None:
+                model = load_model(filenames[0])
+                aiGrid = self.recreateAiTree(grid)
+                myWindow.setLastModel(grid.name, model)
+                img: AbstractImage = myWindow.getImage()
+                appendFoundCellRects(img, grid, aiGrid, None, None, model) # type: ignore
+                img.drawImage()
     
     def removeGrid(self, *args, **kwargs):
         print("removeGrid")
         myWindow: AbstractMyWindow = self._myWindow
-        grid: Grid = self.getSelectedGrid()
+        grid: Grid|None = self.getSelectedGrid()
+        if grid is None:
+            return
         myWindow.getImage().removeGrid(grid.name)
         myWindow.getImage().drawImage()
         self.removeSelectedRow()
 
     def removeSelectedRow(self):
         index_list: list[QtCore.QModelIndex] = []                                                          
         for model_index in self.selectionModel().selectedRows():       
@@ -127,35 +161,41 @@
             self.model().removeRow(index.row(),index.parent())
 
     def removeLabel(self, *args, **kwargs):
         print("removeLabel")
         myWindow: AbstractMyWindow = self._myWindow
         label = self.selectedLabel()
         if(self.selectedType() == TreeItem.TYPE_GRID_ITEM):
-            grid: Grid = self.getSelectedGrid()
+            grid: Grid|None = self.getSelectedGrid()
+            if grid is None:
+                return
             grid.removeRectGroup(label)
         elif(self.selectedType() == TreeItem.TYPE_MANUAL):
             myWindow.getImage().removeRectGroup(label)
         myWindow.getImage().drawImage()
         self.removeSelectedRow()
 
     def addTopRow(self, *args, **kwargs):
         print("addTopRow")
-        grid: Grid = self.getSelectedGrid()
+        grid: Grid|None = self.getSelectedGrid()
+        if grid is None:
+            return
         grid.addTopRow()
         
     def treeSelectionChanged(self, selection: QItemSelection):
         print("treeSelectionChanged")
         myWindow: AbstractMyWindow = self._myWindow
         myWindow.reloadPropertyWindow(selection)
         tree = self
         selectedType = tree.selectedType()
         if((selectedType == TreeItem.TYPE_GRID_ITEM) or (selectedType == TreeItem.TYPE_GRID)):
             self._actionGridAddRowTop.setVisible(True)
-            grid: Grid = self.getSelectedGrid()
+            grid: Grid|None = self.getSelectedGrid()
+            if grid is None:
+                return
             if myWindow.hasModel(grid.name):
                 self._actionSaveModel.setVisible(True)
             self._actionLoadModel.setVisible(True)
         else:
             self._actionGridAddRowTop.setVisible(False)
             self._actionSaveModel.setVisible(False)
             self._actionLoadModel.setVisible(False)
@@ -173,22 +213,26 @@
             self._actionRemoveLabel.setVisible(True)
         else:
             self._actionRemoveLabel.setVisible(False)
         if(selectedType == TreeItem.TYPE_GRID_ITEM):
             self._actionRemoveLabel.setVisible(True)
         else:
             self._actionRemoveLabel.setVisible(False)
+        if(selectedType == TreeItem.TYPE_AI_GRID_ITEM) or (selectedType == TreeItem.TYPE_GRID_ITEM):
+            self._actionViewAsPixelimage.setVisible(True)
+        else:
+            self._actionViewAsPixelimage.setVisible(False)
         if(selectedType == TreeItem.TYPE_GRID_ITEM):
             myWindow.getImage().drawImage()
         if(selectedType == TreeItem.TYPE_AI_GRID_ITEM):
             myWindow.getImage().drawImage()
         self.evtTreeSelectionChanged.emit(selection)
             
-    def addTreeItem(self, text, type="auto", parent_obj=None, parent_item=None) -> tuple[Grid, TreeItem]:
-        obj = None
+    def addTreeItem(self, text, type="auto", parent_obj=None, parent_item=None) -> tuple[typing.Any | None, TreeItem]:
+        obj: typing.Any = None
         myWindow: AbstractMyWindow = self._myWindow
         img = myWindow.getImage()
         tree: Tree = self
         if type == "auto":
             if tree.selectedType() == TreeItem.TYPE_GRID:
                 type = TreeItem.TYPE_GRID_ITEM
             elif tree.selectedType() == TreeItem.TYPE_GRID_ITEM:
@@ -225,103 +269,120 @@
         if type == TreeItem.TYPE_AI:
             treeItem: QStandardItem = myWindow.getAIItem()
         if type == TreeItem.TYPE_GRID:
             treeItem: QStandardItem = myWindow.getManualItem()
         if type == TreeItem.TYPE_AI_GRID:
             treeItem: QStandardItem = myWindow.getAIItem()
         if type == TreeItem.TYPE_GRID_ITEM:
-            treeItem: QStandardItem = self.getSelectedItem().parent()
+            selectedItem = self.getSelectedItem()
+            if selectedItem is not None:
+                treeItem: QStandardItem = selectedItem.parent()
         if type == TreeItem.TYPE_AI_GRID_ITEM:
-            treeItem: QStandardItem = self.getSelectedItem().parent()
+            selectedItem = self.getSelectedItem()
+            if selectedItem is not None:
+                treeItem: QStandardItem = selectedItem.parent()
         if parent_item is not None:
             treeItem: QStandardItem = parent_item
-        tree: QTreeView = self
+        tree: Tree = self
         treeItem.appendRow(item)
         tree.expandAll()
         selModel = tree.selectionModel()
         tree.clearSelection()
-        selModel.select(tree.model().indexFromItem(item), selModel.Select)
-        item.setFlags(QtCore.Qt.ItemIsUserCheckable |
-                        QtCore.Qt.ItemIsEnabled |
-                        QtCore.Qt.ItemIsSelectable)
-        item.setCheckState(QtCore.Qt.Checked)
+        model: QStandardItemModel = typing.cast(QStandardItemModel, tree.model())
+        selModel.select(model.indexFromItem(item), QItemSelectionModel.SelectionFlag.Select)
+        item.setFlags(item.flags() | QtCore.Qt.ItemFlag.ItemIsUserCheckable |
+                        QtCore.Qt.ItemFlag.ItemIsEnabled |
+                        QtCore.Qt.ItemFlag.ItemIsSelectable)
+        item.setCheckState(QtCore.Qt.CheckState.Checked)
         if type in [TreeItem.TYPE_AI_GRID,TreeItem.TYPE_GRID,TreeItem.TYPE_MANUAL]:
             item.onChecked = self.itemChecked
         if type == TreeItem.TYPE_GRID_ITEM:
             item.onChecked = self.gridRectGroupChecked
         if type == TreeItem.TYPE_AI_GRID_ITEM:
             item.onChecked = self.aiGridRectGroupChecked
         if type == TreeItem.TYPE_AI:
             item.onChecked = self.aiItemChecked
         return obj, item
     
-    def getSelectedItem(self) -> QStandardItem:
+    def getSelectedItem(self) -> QStandardItem|None:
         tree: QTreeView = self
         selection = tree.selectedIndexes()
         cnt = len(selection)
         if(cnt == 0):
-            return
+            return None
         sel = selection[0]
-        return tree.model().itemFromIndex(sel)
+        model = typing.cast(QStandardItemModel, tree.model())
+        return model.itemFromIndex(sel)
     
-    def getSelectedGrid(self):
+    def getSelectedGrid(self) -> Grid|None:
         myWindow: AbstractMyWindow = self._myWindow
-        type = self.getSelectedItem().data(TreeItem.TYPE)
+        selectedItem = self.getSelectedItem()
+        if selectedItem is None:
+            return None
+        type = selectedItem.data(TreeItem.TYPE)
         if type == TreeItem.TYPE_GRID_ITEM:
-            return self.getSelectedItem().parent().data(TreeItem.OBJECT)
+            return selectedItem.parent().data(TreeItem.OBJECT)
         if type == TreeItem.TYPE_AI_GRID_ITEM:
-            gridName = self.getSelectedItem().parent().data(TreeItem.TEXT)
+            gridName = selectedItem.parent().data(TreeItem.TEXT)
             manual: QStandardItem = myWindow.getManualItem()
             for r in range(0,manual.rowCount()):
                 if manual.child(r).data(TreeItem.TEXT) == gridName:
                     return manual.child(r).data(TreeItem.OBJECT)
         if type == TreeItem.TYPE_AI_GRID:
-            gridName = self.getSelectedItem().data(TreeItem.TEXT)
+            gridName = selectedItem.data(TreeItem.TEXT)
             manual: QStandardItem = myWindow.getManualItem()
             for r in range(0,manual.rowCount()):
                 if manual.child(r).data(TreeItem.TEXT) == gridName:
                     return manual.child(r).data(TreeItem.OBJECT)
-        return None if type != TreeItem.TYPE_GRID else self.getSelectedItem().data(TreeItem.OBJECT)
+        return None if type != TreeItem.TYPE_GRID else selectedItem.data(TreeItem.OBJECT)
 
     def getSelectedAIGrid(self):
-        type = self.getSelectedItem().data(TreeItem.TYPE)
-        return None if type != TreeItem.TYPE_AI_GRID else self.getSelectedItem().data(TreeItem.OBJECT)
+        selectedItem = self.getSelectedItem()
+        if selectedItem is None:
+            return
+        type = selectedItem.data(TreeItem.TYPE)
+        if type == TreeItem.TYPE_AI_GRID_ITEM:
+            return selectedItem.parent().data(TreeItem.OBJECT)
+        return None if type != TreeItem.TYPE_AI_GRID else selectedItem.data(TreeItem.OBJECT)
     
     def isItemSelected(self, rectLabel, gridName, gridItemType) -> bool:
-        type = self.getSelectedItem().data(TreeItem.TYPE)
+        selectedItem = self.getSelectedItem()
+        if selectedItem is None:
+            return False
+        type = selectedItem.data(TreeItem.TYPE)
         if type != gridItemType:
             return False
-        if self.getSelectedItem().parent().data(TreeItem.TEXT) != gridName:
+        if selectedItem.parent().data(TreeItem.TEXT) != gridName:
             return False
-        if self.getSelectedItem().data(TreeItem.TEXT) != rectLabel:
+        if selectedItem.data(TreeItem.TEXT) != rectLabel:
             return False
         return True
     
-    def clearAIItem(self, name:str = None):
+    def clearAIItem(self, name:str|None = None):
         myWindow: AbstractMyWindow = self._myWindow
         treeAIItem = myWindow.getAIItem()
         if treeAIItem.hasChildren():
             if name is None:
                 treeAIItem.removeRows(0,treeAIItem.rowCount())
                 treeAIItem.clearData()
                 myWindow.getImage().clearAIRects()
             else:
-                for i in range(0,treeAIItem.rowCount):
+                for i in range(0,treeAIItem.rowCount()):
                     child = treeAIItem.child(i)
                     if child.data(TreeItem.TEXT) == name:
                         child.removeRows(0,treeAIItem.rowCount())
                         child.clearData()
     
-    def selectedType(self) -> str:
+    def selectedType(self) -> str|None:
         sel = self.getSelectedItem()
         if sel is None:
             return None
         return sel.data(TreeItem.TYPE)
     
-    def selectedLabel(self) -> str:
+    def selectedLabel(self) -> str|None:
         sel = self.getSelectedItem()
         if sel is None:
             return None
         return sel.data(TreeItem.TEXT)
     
     def aiGridRectGroupChecked(self, treeItem: TreeItem, checked, text):
         myWindow: AbstractMyWindow = self._myWindow
```

### Comparing `silicon-analyser-1.0.3/silicon_analyser/main_window.ui` & `silicon_analyser-1.0.4/silicon_analyser/main_window.ui`

 * *Files 2% similar despite different names*

#### Comparing `silicon-analyser-1.0.3/silicon_analyser/main_window.ui` & `silicon_analyser-1.0.4/silicon_analyser/main_window.ui`

```diff
@@ -202,14 +202,19 @@
       <property name="text">
         <string>Save as csv</string>
       </property>
       <property name="toolTip">
         <string>Save as csv</string>
       </property>
     </action>
+    <action name="_actionViewAsPixelimage">
+      <property name="text">
+        <string>View as pixelimage</string>
+      </property>
+    </action>
   </widget>
   <customwidgets>
     <customwidget>
       <class>ComputeBtn</class>
       <extends>QPushButton</extends>
       <header>silicon_analyser.helper.computebtn</header>
     </customwidget>
```

### Comparing `silicon-analyser-1.0.3/silicon_analyser/mywindow.py` & `silicon_analyser-1.0.4/silicon_analyser/mywindow.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyQt5 import QtCore, uic
+from PyQt5 import QtCore, QtGui, uic
 from PyQt5.QtCore import Qt, QItemSelection
 from PyQt5.QtWidgets import QFileDialog, QTableView, QStatusBar, QAction, QPushButton
 from PyQt5.QtGui import QPixmap, QStandardItem, QStandardItemModel
 from os import path as p
 import sys
 
 import silicon_analyser.savefiles
@@ -26,45 +26,47 @@
     _properties: QTableView
     _addLabelBtn: AddLabelBtn
     _computeBtn: ComputeBtn
     _addGridBtn: AddGridBtn
     _statusBar: QStatusBar
     _minimap: MiniMap
     _image: FullImage
-    _models: dict
+    _models: dict[str,object]
     _actionGridAddRowTop: QAction
     _actionSaveModel: QAction
     _actionLoadModel: QAction
     _actionRemoveGrid: QAction
     _actionRemoveLabel: QAction
     _actionMade_by_TheCrazyT: QAction
     _actionUrl: QAction
     _actionSaveAsCsv: QAction
+    _actionViewAsPixelimage: QAction
     autosave: bool
     
     def __init__(self):
         AbstractMyWindow.__init__(self)
-        uic.loadUi(p.abspath(p.join(p.dirname(__file__), '.')) + '/main_window.ui', self)
+        path: str = p.abspath(p.join(p.dirname(__file__), '.')) + '/main_window.ui'
+        uic.loadUi(path, self)
         tree: Tree = self._tree
         properties: QTableView = self._properties
                 
         self._treeModel = QStandardItemModel()
         self._propertiesModel = QStandardItemModel()
         properties.setModel(self._propertiesModel)
         self._propertiesUtil = PropertiesUtil(self,self._properties)
         
         self._treeManualItem = QStandardItem("Manual")
-        self._treeManualItem.setFlags(QtCore.Qt.ItemIsUserCheckable |
-                          QtCore.Qt.ItemIsEnabled)
-        self._treeManualItem.setCheckState(QtCore.Qt.Unchecked)
+        self._treeManualItem.setFlags(self._treeManualItem.flags() | QtCore.Qt.ItemFlag.ItemIsUserCheckable |
+                          QtCore.Qt.ItemFlag.ItemIsEnabled)
+        self._treeManualItem.setCheckState(QtCore.Qt.CheckState.Unchecked)
         self._treeModel.appendRow(self._treeManualItem)
         self._treeAIItem = QStandardItem("AI")
-        self._treeAIItem.setFlags(QtCore.Qt.ItemIsUserCheckable |
-                          QtCore.Qt.ItemIsEnabled)
-        self._treeAIItem.setCheckState(QtCore.Qt.Unchecked)
+        self._treeAIItem.setFlags(self._treeAIItem.flags() |QtCore.Qt.ItemFlag.ItemIsUserCheckable |
+                          QtCore.Qt.ItemFlag.ItemIsEnabled)
+        self._treeAIItem.setCheckState(QtCore.Qt.CheckState.Unchecked)
         self._treeModel.appendRow(self._treeAIItem)
         tree.setModel(self._treeModel)
         self._models = {}
         self._actionUrl.triggered.connect(self.openMainUrl)
 
         if(len(sys.argv) < 2):
             dlg = QFileDialog()
@@ -102,46 +104,46 @@
         if p.isfile(silicon_analyser.savefiles.SAVE_RECTS):
             with open(silicon_analyser.savefiles.SAVE_RECTS,"r") as f:
                 rects = loadRects()
                 for k in rects.keys():
                     self.getTree().addTreeItem(k)
                 image.loadRects(rects)
         if p.isfile(silicon_analyser.savefiles.SAVE_GRIDS):
-            grids: dict[Grid] = loadGrids()
+            grids: dict[str, Grid] = loadGrids()
             for gridKey in grids.keys():
                 grid, parentTreeItem = self.getTree().addTreeItem(gridKey,TreeItem.TYPE_GRID)
                 for gridItemKey in grids[gridKey].getLabels():
                     _, treeItem = self.getTree().addTreeItem(gridItemKey,TreeItem.TYPE_GRID_ITEM, grid, parentTreeItem)
                     text = treeItem.data(TreeItem.TEXT)
                     if(not grids[gridKey]._rectsActive[text]):
-                        treeItem.setCheckState(QtCore.Qt.Unchecked)
+                        treeItem.setCheckState(QtCore.Qt.CheckState.Unchecked)
             image.loadGrids(grids)
         
         image.drawImage()
         self.autosave = True
         
     def treeSelectionChanged(self, selection: QItemSelection):
         tree: Tree = self._tree
-        selectedType: str = tree.selectedType()
+        selectedType: str|None = tree.selectedType()
         computeBtn: ComputeBtn = self._computeBtn
         addLabelBtn: AddLabelBtn = self._addLabelBtn
         if((selectedType == TreeItem.TYPE_GRID_ITEM)
            or (selectedType == TreeItem.TYPE_GRID)
            or (selectedType == TreeItem.TYPE_AI_GRID)
            or (selectedType == TreeItem.TYPE_AI_GRID_ITEM)
            ):
             computeBtn.setDisabled(False)
             addLabelBtn.setDisabled(False)
         else:
             computeBtn.setDisabled(True)
             addLabelBtn.setDisabled(True)
 
-    def openMainUrl(self):
+    def openMainUrl(self) -> None:
         import webbrowser
-        return webbrowser.open('https://github.com/TheCrazyT/SiliconAnalyser')
+        webbrowser.open('https://github.com/TheCrazyT/SiliconAnalyser')
         
     def getModel(self, name):
         if name in self._models:
             return self._models[name]
         return None
     
     def hasModel(self, name) -> bool:
@@ -200,28 +202,28 @@
     
     def reloadProperyWindowByGrid(self, grid):
         return self._propertiesUtil.reloadProperyWindowByGrid(grid)
     
     def reloadPropertyWindow(self, selection: QItemSelection):
         return self._propertiesUtil.reloadPropertyWindow(selection)
     
-    def keyPressEvent(self, event):
+    def keyPressEvent(self, keyEvent: QtGui.QKeyEvent):
         c = 10
-        if event.modifiers() & Qt.ShiftModifier:
+        if keyEvent.modifiers() == Qt.KeyboardModifier.ShiftModifier:
             c = 100
-        if event.key() == Qt.Key_Left:
+        if keyEvent.key() == Qt.Key.Key_Left:
             self._posX -= c
             self._posX = max(self._posX,0)
-        if event.key() == Qt.Key_Right:
+        if keyEvent.key() == Qt.Key.Key_Right:
             self._posX += c
             self._posX = min(self._posX,self._pixmap.width())
-        if event.key() == Qt.Key_Up:
+        if keyEvent.key() == Qt.Key.Key_Up:
             self._posY -= c
             self._posY = max(self._posY,0)
-        if event.key() == Qt.Key_Down:
+        if keyEvent.key() == Qt.Key.Key_Down:
             self._posY += c
             self._posY = min(self._posY,self._pixmap.height())
         self.drawImgAndMinimap()
             
     def wheelEvent(self,event):
         #print(event.angleDelta())
         if event.angleDelta().y() > 0:
```

### Comparing `silicon-analyser-1.0.3/silicon_analyser/savefiles.py` & `silicon_analyser-1.0.4/silicon_analyser/savefiles.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,19 +32,19 @@
             grids[gridName] = g
         return grids
         
 class MyJSONEncoder(JSONEncoder):
         def default(self, o):
             return o.__dict__
 
-def loadRects() -> dict[Rect]:
+def loadRects() -> dict[str, Rect]:
     with open(SAVE_RECTS,"r") as f:
         return json.load(f)
 
-def loadGrids() -> dict[Grid]:
+def loadGrids() -> dict[str, Grid]:
     with open(SAVE_GRIDS,"r") as f:
         return json.load(f, cls=JSONGridDecoder)
     
 def triggerSaveRects():
     global doSaveRects
     print("triggerSaveRects")
     doSaveRects = True
```

### Comparing `silicon-analyser-1.0.3/silicon_analyser/treeitem.py` & `silicon_analyser-1.0.4/silicon_analyser/treeitem.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,35 +10,37 @@
     TYPE_GRID = "grid"
     TYPE_AI_GRID = "aiGrid"
     TYPE_GRID_ITEM = "gridItem"
     TYPE_AI_GRID_ITEM = "aiGridItem"
     TYPE_MANUAL = "manual"
     TYPE_AI = "ai"
     
+    onChecked: typing.Callable|None
+    
     def __init__(self, text, type, obj):
         QStandardItem.__init__(self,text)
-        self.onChecked = None
         self._text = text
         self._type = type
         self._obj  = obj
+        self.onChecked = None
     
-    def data(self, role: int = ...):
+    def data(self, role: int = ...): # type: ignore
         if(role == TreeItem.TYPE):
             return self._type
         if(role == TreeItem.OBJECT):
             return self._obj
         if(role == TreeItem.TEXT):
             return self._text
         return super().data(role)
     
     def getObject(self):
         return self._obj
     
-    def setData(self, value: typing.Any, role: int = ...) -> None:
-        if role == Qt.CheckStateRole:
+    def setData(self, value: typing.Any, role: int = ...) -> None: # type: ignore
+        if role == Qt.ItemDataRole.CheckStateRole:
             if self.onChecked is not None:
                 if value == 0:
                     self.onChecked(self,False,self._text)
                 else:
                     self.onChecked(self,True,self._text)
         return super().setData(value, role)
```

### Comparing `silicon-analyser-1.0.3/silicon_analyser.egg-info/PKG-INFO` & `silicon_analyser-1.0.4/silicon_analyser.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silicon-analyser
-Version: 1.0.3
+Version: 1.0.4
 Summary: helps to analyse integrated circuit die images (for example from siliconpr0n.org) with the help of ai.
 Author-email: CrazyT <crazyt2019+sa@gmail.com>
 Project-URL: Homepage, https://github.com/TheCrazyT/SiliconAnalyser
 Project-URL: Bug Tracker, https://github.com/TheCrazyT/SiliconAnalyser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -61,15 +61,22 @@
       * the amount of cells you selected
       * how good your grid matches the current image
       * the quality of your image
       * ...
     * "acc" stands for "accuracy", "val" for "validation"
 * found ai-cells will be drawn green
 
+# Keys
+
+* Use up/down/left/right to navigate
+* Hold shift to move faster
+* Scroll-wheel to zoom out
+* Click on minimap to get directly to a position
+
 ![image](https://raw.githubusercontent.com/TheCrazyT/SiliconAnalyser/main/docs/small_tutorial.gif)
 
 # TODO
 
-* export of ai-cells as bit-image
 * auto-compute to calculate in background while you are selecting new cells for your labels
+* ai-model configuration
 * possibility to rotate grid
 * maybe store your model on a public place? (for others to use)
```

### Comparing `silicon-analyser-1.0.3/silicon_analyser.egg-info/SOURCES.txt` & `silicon_analyser-1.0.4/silicon_analyser.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 silicon_analyser.egg-info/SOURCES.txt
 silicon_analyser.egg-info/dependency_links.txt
 silicon_analyser.egg-info/entry_points.txt
 silicon_analyser.egg-info/requires.txt
 silicon_analyser.egg-info/top_level.txt
 silicon_analyser/dialogs/compute_stats.py
 silicon_analyser/dialogs/compute_stats.ui
+silicon_analyser/dialogs/pixel_image.py
+silicon_analyser/dialogs/pixel_image.ui
 silicon_analyser/helper/addgridbtn.py
 silicon_analyser/helper/addlabelbtn.py
 silicon_analyser/helper/ai.py
 silicon_analyser/helper/computebtn.py
 silicon_analyser/helper/fullimage.py
 silicon_analyser/helper/minimap.py
 silicon_analyser/helper/properties.py
```

