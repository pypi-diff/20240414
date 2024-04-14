# Comparing `tmp/pyscript-ltk-0.1.8.tar.gz` & `tmp/pyscript-ltk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscript-ltk-0.1.8.tar", last modified: Wed Nov 29 08:01:33 2023, max compression
+gzip compressed data, was "pyscript-ltk-0.1.9.tar", last modified: Sun Dec  3 10:43:23 2023, max compression
```

## Comparing `pyscript-ltk-0.1.8.tar` & `pyscript-ltk-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-11-29 08:01:33.569855 pyscript-ltk-0.1.8/
--rw-r--r--   0 laffra     (501) staff       (20)    11357 2023-10-31 14:04:54.000000 pyscript-ltk-0.1.8/LICENSE
--rw-r--r--   0 laffra     (501) staff       (20)      100 2023-11-12 15:12:06.000000 pyscript-ltk-0.1.8/MANIFEST.in
--rw-r--r--   0 laffra     (501) staff       (20)    17789 2023-11-29 08:01:33.569147 pyscript-ltk-0.1.8/PKG-INFO
--rw-r--r--   0 laffra     (501) staff       (20)     4288 2023-11-25 13:49:57.000000 pyscript-ltk-0.1.8/README.md
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-11-29 08:01:33.564109 pyscript-ltk-0.1.8/ltk/
--rw-r--r--   0 laffra     (501) staff       (20)      179 2023-11-27 17:06:38.000000 pyscript-ltk-0.1.8/ltk/__init__.py
--rw-r--r--   0 laffra     (501) staff       (20)     4064 2023-11-27 17:06:38.000000 pyscript-ltk-0.1.8/ltk/jquery.py
--rw-r--r--   0 laffra     (501) staff       (20)    12747 2023-11-27 17:17:29.000000 pyscript-ltk-0.1.8/ltk/logger.py
--rw-r--r--   0 laffra     (501) staff       (20)     7117 2023-11-28 20:51:56.000000 pyscript-ltk-0.1.8/ltk/ltk.css
--rw-r--r--   0 laffra     (501) staff       (20)     3564 2023-11-27 17:06:38.000000 pyscript-ltk-0.1.8/ltk/ltk.js
--rw-r--r--   0 laffra     (501) staff       (20)     3868 2023-11-28 10:50:58.000000 pyscript-ltk-0.1.8/ltk/pubsub.py
--rw-r--r--   0 laffra     (501) staff       (20)    19441 2023-11-28 21:20:01.000000 pyscript-ltk-0.1.8/ltk/widgets.py
--rw-r--r--   0 laffra     (501) staff       (20)      735 2023-11-29 08:01:00.000000 pyscript-ltk-0.1.8/pyproject.toml
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-11-29 08:01:33.567901 pyscript-ltk-0.1.8/pyscript_ltk.egg-info/
--rw-r--r--   0 laffra     (501) staff       (20)    17789 2023-11-29 08:01:33.000000 pyscript-ltk-0.1.8/pyscript_ltk.egg-info/PKG-INFO
--rw-r--r--   0 laffra     (501) staff       (20)      319 2023-11-29 08:01:33.000000 pyscript-ltk-0.1.8/pyscript_ltk.egg-info/SOURCES.txt
--rw-r--r--   0 laffra     (501) staff       (20)        1 2023-11-29 08:01:33.000000 pyscript-ltk-0.1.8/pyscript_ltk.egg-info/dependency_links.txt
--rw-r--r--   0 laffra     (501) staff       (20)       19 2023-11-29 08:01:33.000000 pyscript-ltk-0.1.8/pyscript_ltk.egg-info/requires.txt
--rw-r--r--   0 laffra     (501) staff       (20)        4 2023-11-29 08:01:33.000000 pyscript-ltk-0.1.8/pyscript_ltk.egg-info/top_level.txt
--rw-r--r--   0 laffra     (501) staff       (20)       38 2023-11-29 08:01:33.569967 pyscript-ltk-0.1.8/setup.cfg
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-12-03 10:43:23.000674 pyscript-ltk-0.1.9/
+-rw-r--r--   0 laffra     (501) staff       (20)    11357 2023-10-31 14:04:54.000000 pyscript-ltk-0.1.9/LICENSE
+-rw-r--r--   0 laffra     (501) staff       (20)      100 2023-11-12 15:12:06.000000 pyscript-ltk-0.1.9/MANIFEST.in
+-rw-r--r--   0 laffra     (501) staff       (20)    17789 2023-12-03 10:43:22.999510 pyscript-ltk-0.1.9/PKG-INFO
+-rw-r--r--   0 laffra     (501) staff       (20)     4288 2023-11-25 13:49:57.000000 pyscript-ltk-0.1.9/README.md
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-12-03 10:43:22.990761 pyscript-ltk-0.1.9/ltk/
+-rw-r--r--   0 laffra     (501) staff       (20)      179 2023-11-27 17:06:38.000000 pyscript-ltk-0.1.9/ltk/__init__.py
+-rw-r--r--   0 laffra     (501) staff       (20)     4028 2023-12-02 19:32:08.000000 pyscript-ltk-0.1.9/ltk/jquery.py
+-rw-r--r--   0 laffra     (501) staff       (20)    12854 2023-12-03 10:41:55.000000 pyscript-ltk-0.1.9/ltk/logger.py
+-rw-r--r--   0 laffra     (501) staff       (20)     7117 2023-12-02 09:19:32.000000 pyscript-ltk-0.1.9/ltk/ltk.css
+-rw-r--r--   0 laffra     (501) staff       (20)     3564 2023-11-27 17:06:38.000000 pyscript-ltk-0.1.9/ltk/ltk.js
+-rw-r--r--   0 laffra     (501) staff       (20)     3918 2023-12-02 09:29:40.000000 pyscript-ltk-0.1.9/ltk/pubsub.py
+-rw-r--r--   0 laffra     (501) staff       (20)    19679 2023-12-02 19:27:33.000000 pyscript-ltk-0.1.9/ltk/widgets.py
+-rw-r--r--   0 laffra     (501) staff       (20)      735 2023-12-03 10:41:04.000000 pyscript-ltk-0.1.9/pyproject.toml
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-12-03 10:43:22.996552 pyscript-ltk-0.1.9/pyscript_ltk.egg-info/
+-rw-r--r--   0 laffra     (501) staff       (20)    17789 2023-12-03 10:43:22.000000 pyscript-ltk-0.1.9/pyscript_ltk.egg-info/PKG-INFO
+-rw-r--r--   0 laffra     (501) staff       (20)      319 2023-12-03 10:43:22.000000 pyscript-ltk-0.1.9/pyscript_ltk.egg-info/SOURCES.txt
+-rw-r--r--   0 laffra     (501) staff       (20)        1 2023-12-03 10:43:22.000000 pyscript-ltk-0.1.9/pyscript_ltk.egg-info/dependency_links.txt
+-rw-r--r--   0 laffra     (501) staff       (20)       19 2023-12-03 10:43:22.000000 pyscript-ltk-0.1.9/pyscript_ltk.egg-info/requires.txt
+-rw-r--r--   0 laffra     (501) staff       (20)        4 2023-12-03 10:43:22.000000 pyscript-ltk-0.1.9/pyscript_ltk.egg-info/top_level.txt
+-rw-r--r--   0 laffra     (501) staff       (20)       38 2023-12-03 10:43:23.000825 pyscript-ltk-0.1.9/setup.cfg
```

### Comparing `pyscript-ltk-0.1.8/LICENSE` & `pyscript-ltk-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscript-ltk-0.1.8/PKG-INFO` & `pyscript-ltk-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscript-ltk
-Version: 0.1.8
+Version: 0.1.9
 Summary: A little toolkit for writing UIs in PyScript
 Author-email: Chris Laffra <chris@chrislaffra.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `pyscript-ltk-0.1.8/README.md` & `pyscript-ltk-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyscript-ltk-0.1.8/ltk/jquery.py` & `pyscript-ltk-0.1.9/ltk/jquery.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 
 jQuery = window.jQuery
 find = jQuery
 create = jQuery
 parse_int = window.parseInt
 parse_float = window.parseFloat
 local_storage = window.localStorage
-
-_timers = {}
+timers = {}
 
 
 def get_time():
     return window.get_time() / 1000
 
 
 def find_list(selector):
@@ -52,20 +51,20 @@
     except:
         try:
             return json.loads(window.to_py(jsobj)) # Micropython has no built-in to_py
         except:
             return str(jsobj)
 
 
-def schedule(python_function, timeout_seconds=0.1):
+def schedule(python_function, key, timeout_seconds=0.1):
     if not python_function:
         raise ValueError(f"schedule: Expecting a function, not {python_function}")
-    if python_function in _timers:
-        window.clearTimeout(_timers[python_function])
-    _timers[python_function] = window.setTimeout(proxy(python_function), int(timeout_seconds * 1000))
+    if key in timers:
+        window.clearTimeout(timers[key])
+    timers[key] = window.setTimeout(proxy(python_function), int(timeout_seconds * 1000))
 
 
 def repeat(python_function, timeout_seconds=1):
     window.setInterval(proxy(python_function), int(timeout_seconds * 1000))
 
 
 def get(route, handler, kind="json"):
```

### Comparing `pyscript-ltk-0.1.8/ltk/logger.py` & `pyscript-ltk-0.1.9/ltk/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
             ltk.find(".ltk-log-header").width(self.width())
             ltk.find(".ltk-log-buttons").css("right", 10)
             self.last_width = self.element.width()
 
     def _set_level(self, selected):
         self.level = self.levels[selected]
         self._filter_rows()
+        ltk.pubsub.show_publish = self.level == logging.DEBUG
 
     def _apply_filter(self):
         self._filter_rows()
         self.sequence_ui.filter_messages()
 
     def _filter_rows(self):
         filter_text = ltk.find("#ltk-log-filter").val()
@@ -236,15 +237,15 @@
         )
         self.element.append(self.dot.element)
         self.set_index(index)
     
     def set_index(self, index):
         self.index = index
         self.display("block")
-        ltk.schedule(self.set_position)
+        ltk.schedule(self.set_position, f"{self}.set_position")
     
     def set_position(self):
         left = min(self.sender.title.position().left, self.receiver.title.position().left)
         right = max(self.sender.title.position().left, self.receiver.title.position().left)
         top = self.sender.title.position().top
         width = self.sender.title.width()
         height = self.sender.title.height()
@@ -290,15 +291,15 @@
     components = {}
     calls = []
     last_width = 0
 
     def __init__(self):
         ltk.HBox.__init__(self,
             ltk.Div(
-                ltk.Text("State Sequence Diagram").css("margin", 3)
+                ltk.Text("State Sequence Diagram").css("margin", 3),
             ).addClass("ltk-sequence-header"),
         )
         self.element.attr("id", "ltk-sequence-ui")
         ltk.observe(self.element, self.changed)
         self.last_width = self.element.width()
         self.on("resize", lambda event, ui: self.resize())
         self.set_width()
@@ -322,31 +323,31 @@
         sender = self.get_component(sender_name)
         receiver = self.get_component(receiver_name)
         call = _Call(sender, receiver, f"{type}:{topic}", data, len(self.calls))
         self.calls.append(call)
         self.append(call.element)
         self.filter_messages()
         self.set_width()
-        ltk.schedule(lambda: self.changed(force=True), 1.5)
+        ltk.schedule(lambda: self.changed(force=True), f"{self}.changed", 1.5)
 
     def clear(self):
         ltk.find(".ltk-sequence-call").animate(
             ltk.to_js({ "opacity": 0}),
             lambda: ltk.find(".ltk-sequence-call").remove()
         )
         self.calls = []
 
     def filter_messages(self):
         filter = ltk.find("#ltk-log-filter").val()
         ltk.find(".ltk-sequence-call").css("display", "none")
-        index = len(self.calls) - 1
-        for n, call in enumerate(self.calls):
-            if filter in call.text():
-                call.set_index(index)
-                index -= 1
+        calls = [call for call in self.calls if filter in call.text()]
+        index = len(calls) - 1
+        for call in calls:
+            call.set_index(index)
+            index -= 1
 
     def get_component(self, name):
         if not name in self.components:
             component = _Component(name)
             self.components[name] = component
             component.appendTo(self.element)
         return self.components[name]
```

### Comparing `pyscript-ltk-0.1.8/ltk/ltk.css` & `pyscript-ltk-0.1.9/ltk/ltk.css`

 * *Files 1% similar despite different names*

```diff
@@ -322,15 +322,15 @@
 }
 .ltk-vertical-dragger:hover {
     background-color: gray;
 }
 .ltk-log-list .ui-resizable-n {
     cursor: ns-resize;
     height: 32px;
-    width: calc(100% - 180px);
+    width: calc(100% - 210px);
 }
 .ltk-log-list .ui-resizable-e {
     cursor: ew-resize;
     width: 15px;
 }
 .ltk-arrow{
     display: block;
```

### Comparing `pyscript-ltk-0.1.8/ltk/ltk.js` & `pyscript-ltk-0.1.9/ltk/ltk.js`

 * *Files identical despite different names*

### Comparing `pyscript-ltk-0.1.8/ltk/pubsub.py` & `pyscript-ltk-0.1.9/ltk/pubsub.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     "log.warning": _logger.warning,
     "log.critical": _logger.critical,
 }
 
 _name = "pubsub_mpy" if "MicroPython" in sys.version else "pubsub_py"
 workers = {}
 start = time.time()
+show_publish = False
 
 class _Message():
     def __init__(self, sender, receiver, topic, data):
         self.sender = sender
         self.receiver = receiver
         self.topic = topic
         self.data = data
@@ -90,15 +91,16 @@
         self.queue[f"{_name}-{time.time()}"] = message
 
     def remove_from_queue(self, key):
         del self.queue[key]
 
     def publish(self, sender, receiver, topic, data):
         self.add_to_queue(_Message(sender, receiver, topic, data))
-        _logger.info(f"[Pubsub] {json.dumps(['publish', sender, receiver, topic, str(data)[:32]])}")
+        if show_publish:
+            _logger.info(f"[Pubsub] {json.dumps(['publish', sender, receiver, topic, str(data)[:32]])}")
         self.process_queue()
 
     def subscribe(self, name, topic, handler):
         self.subscribers.append([name, topic, handler])
         self.process_queue()
```

### Comparing `pyscript-ltk-0.1.8/ltk/widgets.py` & `pyscript-ltk-0.1.9/ltk/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,14 +192,21 @@
 
 
 class Switch(HBox):
     """ A checkbox with special styling to resemble a switch/toggle """
     classes = [ "ltk-switch-container ltk-hbox" ]
 
     def __init__(self, label, checked, style=DEFAULT_CSS):
+        """
+        Create a new switch
+
+        Args:
+            label:str: The label for the switch
+            checked:bool Whether the switch is checked or not
+        """
         def toggle_edit(event):
             checked = self.element.find(".ltk-checkbox").prop("checked")
             self.element.prop("checked", checked)
         id = f"edit-switch-{get_time()}"
         HBox.__init__(self, 
             Div(label).addClass("ltk-switch-label"),
             Checkbox(True).attr("id", id).addClass("ltk-switch-checkbox").on("change", toggle_edit),
@@ -497,25 +504,25 @@
     def __init__(self, language, code, style=DEFAULT_CSS):
         Widget.__init__(self, style)
         if not hasattr(window, "hljs"):
             inject_css("https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/styles/default.min.css")
             inject_script("https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/highlight.min.js")
             inject_script(f"https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/languages/{language}.min.js")
         self.element.text(code).css("opacity", 0)
-        schedule(self.highlight)
+        schedule(self.highlight, f"{self}.highlight")
 
     def highlight(self):
         if self.highlighted:
             return
         if hasattr(window, "hljs"):
             window.hljs.highlightElement(self.element[0])
             self.element.animate(to_js({ "opacity": 1}))
             self.highlighted = True
         else:
-            schedule(self.highlight, 0.1)
+            schedule(self.highlight, f"{self}.highlight", 0.1)
 
 
 class Image(Widget):
     """ Wraps an HTML element of type <img> """
     classes = [ "ltk-image" ]
     tag = "img"
 
@@ -622,15 +629,15 @@
             [
                 Option(text).prop("selected", "selected" if text == selected else "")
                 for text in options
             ],
             style
         )
         self.handler = handler
-        self.element.on("change", proxy(lambda event: schedule(self.changed)))
+        self.element.on("change", proxy(lambda event: schedule(self.changed, f"{self}.changed")))
 
     def get_selected_index(self):
         return self.element.prop("selectedIndex")
 
     def changed(self):
         option = self.element.find("option").eq(self.get_selected_index())
         self.handler(self.get_selected_index(), option)
```

### Comparing `pyscript-ltk-0.1.8/pyproject.toml` & `pyscript-ltk-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyscript-ltk"
-version = "0.1.8"
+version = "0.1.9"
 description = "A little toolkit for writing UIs in PyScript"
 readme = "README.md"
 authors = [{ name = "Chris Laffra", email = "chris@chrislaffra.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `pyscript-ltk-0.1.8/pyscript_ltk.egg-info/PKG-INFO` & `pyscript-ltk-0.1.9/pyscript_ltk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscript-ltk
-Version: 0.1.8
+Version: 0.1.9
 Summary: A little toolkit for writing UIs in PyScript
 Author-email: Chris Laffra <chris@chrislaffra.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

