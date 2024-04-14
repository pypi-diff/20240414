# Comparing `tmp/term_ascii_diagram-0.0.4.tar.gz` & `tmp/term_ascii_diagram-0.0.5.tar.gz`

## Comparing `term_ascii_diagram-0.0.4.tar` & `term_ascii_diagram-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.4/src/term_ascii_diagram/__init__.py
--rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.4/src/term_ascii_diagram/core.py
--rw-r--r--   0        0        0    22268 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.4/src/term_ascii_diagram/diagram.py
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.4/src/term_ascii_diagram/main.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.4/src/term_ascii_diagram/status_bar.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.4/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.4/LICENSE
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.4/README.md
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.5/.github/workflows/publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.5/src/term_ascii_diagram/__init__.py
+-rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.5/src/term_ascii_diagram/core.py
+-rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.5/src/term_ascii_diagram/diagram.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.5/src/term_ascii_diagram/main.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.5/src/term_ascii_diagram/status_bar.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.5/LICENSE
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.5/README.md
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 term_ascii_diagram-0.0.5/PKG-INFO
```

### Comparing `term_ascii_diagram-0.0.4/.github/workflows/publish.yml` & `term_ascii_diagram-0.0.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `term_ascii_diagram-0.0.4/src/term_ascii_diagram/core.py` & `term_ascii_diagram-0.0.5/src/term_ascii_diagram/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import curses
 from dataclasses import dataclass
 from enum import Enum
-from typing import Optional, Tuple, overload
+from typing import Optional, Tuple, Union, overload
 
 
 @dataclass
 class Size:
     w: int
     h: int
 
@@ -25,16 +25,17 @@
     def __add__(self, other: Size) -> "Point":
         return Point(self.x + other.w, self.y + other.h)
 
     @overload
     def __sub__(self, other: "Point") -> Size: ...
     @overload
     def __sub__(self, other: Size) -> "Point": ...
-
-    def __sub__(self, other):
+    def __sub__(  # noqa: E301
+        self, other: Union["Point", Size]
+    ) -> Union["Point", Size]:
         if isinstance(other, Point):
             return Size(other.x - self.x, other.y - self.y)
         elif isinstance(other, Size):
             return Point(self.x - other.w, self.y - other.h)
         else:
             ValueError(f"Type {type(other).__name__} is not supported.")
 
@@ -66,15 +67,15 @@
     HAND = 0
     MOVE = 1
 
 
 class Canvas:
     stdscr: curses.window
 
-    def __init__(self, stdscr):
+    def __init__(self, stdscr: curses.window) -> None:
         self.stdscr = stdscr
 
     def getmaxxy(self) -> Tuple[int, int]:
         max_y, max_x = self.stdscr.getmaxyx()
         # Switch to be the same as other structures
         return max_x, max_y
```

### Comparing `term_ascii_diagram-0.0.4/src/term_ascii_diagram/diagram.py` & `term_ascii_diagram-0.0.5/src/term_ascii_diagram/diagram.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,69 +21,75 @@
         position: Optional[Point] = None,
         size: Optional[Size] = None,
     ):
         self.position = position or Point(0, 0)
         self.size = size or Size(6, 3)
 
     @property
-    def normalized_position(self):
+    def normalized_position(self) -> Point:
         x = self.position.x
         y = self.position.y
         if self.size.w < 0:
             x += self.size.w
         if self.size.h < 0:
             y += self.size.h
         return Point(x, y)
 
     @property
-    def normalized_size(self):
+    def normalized_size(self) -> Size:
         return Size(abs(self.size.w), abs(self.size.h))
 
     @property
-    def top_left(self):
+    def top_left(self) -> Point:
         return self.position
 
     @property
-    def normalized_top_left(self):
+    def normalized_top_left(self) -> Point:
         return self.normalized_position
 
     @property
-    def top_right(self):
+    def top_right(self) -> Point:
         return Point(self.position.x + self.size.w, self.position.y)
 
     @property
-    def normalized_top_right(self):
+    def normalized_top_right(self) -> Point:
         return Point(
             self.normalized_position.x + self.normalized_size.w,
             self.normalized_position.y,
         )
 
     @property
-    def bottom_left(self):
+    def bottom_left(self) -> Point:
         return Point(self.position.x, self.position.y + self.size.h)
 
     @property
-    def normalized_bottom_left(self):
+    def normalized_bottom_left(self) -> Point:
         return Point(
             self.normalized_position.x,
             self.normalized_position.y + self.normalized_size.h,
         )
 
     @property
-    def bottom_right(self):
+    def bottom_right(self) -> Point:
         return self.position + self.size
 
     @property
-    def normalized_bottom_right(self):
+    def normalized_bottom_right(self) -> Point:
         return self.normalized_position + self.normalized_size
 
-    def draw(self, canvas: Canvas):
+    def draw(self, canvas: Canvas) -> None:
         """Draw the object on the canvas."""
         raise NotImplementedError("DiagramObject should not be used directly")
 
+    def toggle(self) -> None:
+        """Toggle the object main attribute.
+
+        For example change the line orientation."""
+        pass
+
     def serialize(self) -> Dict[str, Any]:
         return {
             "type": type(self).__name__,
             "position": asdict(self.position),
             "size": asdict(self.size),
         }
 
@@ -108,15 +114,15 @@
         super().__init__(position, size)
         self.text = text
         self.show_border = show_border
 
     def toggle(self) -> None:
         self.show_border = not self.show_border
 
-    def draw(self, canvas: Canvas):
+    def draw(self, canvas: Canvas) -> None:
         if self.show_border:
             canvas.fill(self.top_left, self.top_right, Ascii.H_LINE)
             canvas.fill(self.bottom_left, self.bottom_right, Ascii.H_LINE)
             canvas.fill(self.top_right, self.bottom_right, Ascii.V_LINE)
             canvas.fill(self.top_left, self.bottom_left, Ascii.V_LINE)
             for point, char in [
                 (self.normalized_top_left, Ascii.TL_CORNER),
@@ -146,15 +152,15 @@
         return data
 
     def deserialize(self, data: Dict[str, Any]) -> None:
         super().deserialize(data)
         self.text = data["text"]
         self.show_border = data["show_border"]
 
-    def edit(self, canvas: Canvas):
+    def edit(self, canvas: Canvas) -> None:
         buf = []
         for y in range(1, self.size.h):
             for x in range(1, self.size.w):
                 ch = canvas.get_ch(
                     Point(
                         self.position.x + x,
                         self.position.y + y,
@@ -211,15 +217,15 @@
         size: Optional[Size] = None,
         orientation: Optional[Orientation] = Orientation.HORIZONTAL,
     ):
         super().__init__(position, size)
         self.orientation = orientation or Line.Orientation.HORIZONTAL
         self.is_arrow = is_arrow
 
-    def toggle(self):
+    def toggle(self) -> None:
         """Toggle the line starting orientation."""
         self.orientation = (
             Line.Orientation.HORIZONTAL
             if self.orientation == Line.Orientation.VERTICAL
             else Line.Orientation.VERTICAL
         )
 
@@ -317,15 +323,15 @@
     canvas: Canvas
     stdscr: curses.window
     status_bar: StatusBar
     objects: List[DiagramObject]
     selected_object_index: int
     cursor: Point
     cursor_mode: CursorMode
-    key_bindings: Dict[int, Callable]
+    key_bindings: Dict[int, Callable[[], None]]
     sticky_mode: bool
 
     def __init__(
         self,
         stdscr: curses.window,
         window: curses.window,
         status_bar: StatusBar,
@@ -347,23 +353,23 @@
         self.cursor = Point(0, 0)
         self.cursor_mode = CursorMode.HAND
         self.objects = []
         self.key_bindings = self._get_key_bindings()
         self.sticky_mode = True
 
     @property
-    def selected_object(self):
+    def selected_object(self) -> Optional[DiagramObject]:
         if 0 <= self.selected_object_index < len(self.objects):
             return self.objects[self.selected_object_index]
         return None
 
     def _find_lines(self) -> Iterable[Line]:
         for obj in self.objects:
             if isinstance(obj, Line):
-                yield cast(Line, obj)
+                yield obj
 
     def _get_connected_lines(self) -> Tuple[List[Line], List[Line]]:
         starting_connected_lines: List[Line] = []
         ending_connected_lines: List[Line] = []
         if self.selected_object is None:
             return starting_connected_lines, ending_connected_lines
         # Move arrows too if they're connected
@@ -409,20 +415,20 @@
                     arrow.size.h += dy
         else:
             if 0 <= self.cursor.x + dx < max_x:
                 self.cursor.x += dx
             if 0 <= self.cursor.y + dy < max_y:
                 self.cursor.y += dy
 
-    def _on_cursor_move_resize(self, dx: int, dy: int):
+    def _on_cursor_move_resize(self, dx: int, dy: int) -> None:
         if self.selected_object:
             self.selected_object.size.w += dx
             self.selected_object.size.h += dy
 
-    def _on_switch_object(self, reverse: bool):
+    def _on_switch_object(self, reverse: bool) -> None:
         next_cursor_mode = CursorMode.MOVE
 
         # Rotate selection
         if reverse:
             if self.selected_object_index == -1:
                 self.selected_object_index = len(self.objects) - 1
             else:
@@ -519,15 +525,15 @@
                 if self.cursor.is_within(obj.top_left, obj.bottom_right):
                     self.selected_object_index = i
         else:
             if hasattr(self.selected_object, "edit"):
                 self.selected_object.edit(self.canvas)
 
     def _toggle_object(self) -> None:
-        if hasattr(self.selected_object, "toggle"):
+        if self.selected_object:
             self.selected_object.toggle()
 
     def _toggle_sticky_mode(self) -> None:
         self.sticky_mode = not self.sticky_mode
 
     def save(self, file_name: Optional[str] = None) -> None:
         if file_name is None:
@@ -548,15 +554,15 @@
             objects = json.load(file)
             self.deserialize(objects)
 
     ##################
     # End of commands
     ##################
 
-    def _get_key_bindings(self) -> Dict[int, Callable]:
+    def _get_key_bindings(self) -> Dict[int, Callable[[], None]]:
         move_up = lambda: self._on_cursor_move(0, -1)  # noqa: E731
         move_down = lambda: self._on_cursor_move(0, 1)  # noqa: E731
         move_left = lambda: self._on_cursor_move(-1, 0)  # noqa: E731
         move_right = lambda: self._on_cursor_move(1, 0)  # noqa: E731
         resize_up = lambda: self._on_cursor_move_resize(0, -1)  # noqa: E731
         resize_down = lambda: self._on_cursor_move_resize(0, 1)  # noqa: E731
         resize_left = lambda: self._on_cursor_move_resize(-1, 0)  # noqa: E731
@@ -607,15 +613,15 @@
     def _confirm_exit(self) -> bool:
         res = self.status_bar.message(
             "Quit? [y/N]",
             curses.color_pair(4),
         )
         return chr(res).lower() == "y"
 
-    def loop(self):
+    def loop(self) -> None:
         while True:
             try:
                 self.canvas.clear()
                 self.draw()
                 self.canvas.refresh()
                 self._update_status_bar()
```

### Comparing `term_ascii_diagram-0.0.4/src/term_ascii_diagram/main.py` & `term_ascii_diagram-0.0.5/src/term_ascii_diagram/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import argparse
 import curses
 import curses.ascii
 import os
+from typing import Any, Callable
 
 from term_ascii_diagram.diagram import Designer
 from term_ascii_diagram.status_bar import StatusBar
 
 
-def wrapped(args):
-    def main(stdscr: curses.window):
+def wrapped(args: Any) -> Callable[[curses.window], None]:
+    def main(stdscr: curses.window) -> None:
         stdscr.keypad(True)
         max_y, max_x = stdscr.getmaxyx()
 
         # Status bar
         status_bar_window = stdscr.subwin(1, max_x, max_y - 1, 0)
         status_bar = StatusBar(stdscr, status_bar_window, curses.color_pair(3))
         status_bar.set_shortcut("Q", "uit")
@@ -39,15 +40,15 @@
             designer.open(args.filename)
 
         designer.loop()
 
     return main
 
 
-def cli():
+def cli() -> None:
     parser = argparse.ArgumentParser(
         prog="term-ascii-diagram",
         description="Terminal ASCII Diagram Builder.",
     )
 
     parser.add_argument("filename", nargs="?")
     parser.add_argument("-r", "--render")
```

### Comparing `term_ascii_diagram-0.0.4/src/term_ascii_diagram/status_bar.py` & `term_ascii_diagram-0.0.5/src/term_ascii_diagram/status_bar.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         return self.window.getch()
 
     def resize(self) -> None:
         max_y, max_x = self.root_window.getmaxyx()
         self.window.resize(1, max_x)
         self.window.mvwin(max_y - 1, 0)
 
-    def invalidate(self):
+    def invalidate(self) -> None:
         _, max_x = self.window.getmaxyx()
         self.window.addstr(0, 0, " " * (max_x - 1), self.bg_color)
         x = 0
         try:
             for key, label in self.shortcuts.items():
                 self.window.addstr(0, x, key)
                 x += len(key)
```

### Comparing `term_ascii_diagram-0.0.4/.gitignore` & `term_ascii_diagram-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `term_ascii_diagram-0.0.4/LICENSE` & `term_ascii_diagram-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `term_ascii_diagram-0.0.4/README.md` & `term_ascii_diagram-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `term_ascii_diagram-0.0.4/pyproject.toml` & `term_ascii_diagram-0.0.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 name = "term-ascii-diagram"
-version = "0.0.4"
+dynamic = ["version"]
 authors = [
   { name="Amir Karimi", email="me@amirkarimi.dev" },
 ]
 description = "Build ASCII diagrams in terminal using keyboard."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -21,7 +21,10 @@
 
 [project.urls]
 Homepage = "https://github.com/amirkarimi/term-ascii-diagram"
 Issues = "https://github.com/amirkarimi/term-ascii-diagram/issues"
 
 [project.scripts]
 term-ascii-diagram = "term_ascii_diagram.main:cli"
+
+[tool.hatch.version]
+source = "vcs"
```

### Comparing `term_ascii_diagram-0.0.4/PKG-INFO` & `term_ascii_diagram-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: term-ascii-diagram
-Version: 0.0.4
+Version: 0.0.5
 Summary: Build ASCII diagrams in terminal using keyboard.
 Project-URL: Homepage, https://github.com/amirkarimi/term-ascii-diagram
 Project-URL: Issues, https://github.com/amirkarimi/term-ascii-diagram/issues
 Author-email: Amir Karimi <me@amirkarimi.dev>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
```

