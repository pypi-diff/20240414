# Comparing `tmp/easydebugger-1.2.0.tar.gz` & `tmp/easydebugger-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easydebugger-1.2.0.tar", last modified: Thu Apr 11 16:44:56 2024, max compression
+gzip compressed data, was "easydebugger-1.2.1.tar", last modified: Sun Apr 14 00:13:36 2024, max compression
```

## Comparing `easydebugger-1.2.0.tar` & `easydebugger-1.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 16:44:56.127041 easydebugger-1.2.0/
--rw-rw-rw-   0        0        0    35823 2024-04-08 15:41:48.000000 easydebugger-1.2.0/LICENSE
--rw-rw-rw-   0        0        0      259 2024-04-11 16:44:56.124041 easydebugger-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    15173 2024-04-11 10:32:10.000000 easydebugger-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 16:44:56.102040 easydebugger-1.2.0/easydebugger/
--rw-rw-rw-   0        0        0     6628 2024-04-11 16:43:53.000000 easydebugger-1.2.0/easydebugger/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 16:44:56.123042 easydebugger-1.2.0/easydebugger.egg-info/
--rw-rw-rw-   0        0        0      259 2024-04-11 16:44:55.000000 easydebugger-1.2.0/easydebugger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2024-04-11 16:44:56.000000 easydebugger-1.2.0/easydebugger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 16:44:55.000000 easydebugger-1.2.0/easydebugger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-11 16:44:55.000000 easydebugger-1.2.0/easydebugger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 16:44:56.127041 easydebugger-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      522 2024-04-11 16:44:13.000000 easydebugger-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 00:13:36.159222 easydebugger-1.2.1/
+-rw-rw-rw-   0        0        0    35823 2024-04-08 15:41:48.000000 easydebugger-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0      259 2024-04-14 00:13:36.156218 easydebugger-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    18828 2024-04-14 00:11:35.000000 easydebugger-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 00:13:36.131359 easydebugger-1.2.1/easydebugger/
+-rw-rw-rw-   0        0        0     6612 2024-04-14 00:06:38.000000 easydebugger-1.2.1/easydebugger/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 00:13:36.154240 easydebugger-1.2.1/easydebugger.egg-info/
+-rw-rw-rw-   0        0        0      259 2024-04-14 00:13:35.000000 easydebugger-1.2.1/easydebugger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2024-04-14 00:13:35.000000 easydebugger-1.2.1/easydebugger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 00:13:35.000000 easydebugger-1.2.1/easydebugger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-14 00:13:35.000000 easydebugger-1.2.1/easydebugger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 00:13:36.159222 easydebugger-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      522 2024-04-14 00:08:41.000000 easydebugger-1.2.1/setup.py
```

### Comparing `easydebugger-1.2.0/LICENSE` & `easydebugger-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easydebugger-1.2.0/README.md` & `easydebugger-1.2.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 # easydebugger
 a Python debugging tool made by blob2763
 
 [![PyPI](https://img.shields.io/pypi/v/easydebugger?label=pypi)](https://pypi.org/project/easydebugger/)
-[![Downloads](https://pepy.tech/badge/easydebugger)](https://www.pepy.tech/projects/easydebugger)
+[![Downloads](https://pepy.tech/badge/easydebugger)](https://www.pepy.tech/projects/easydebugger?versions=1.*&versions=0.*)
 
+## contents
+- [setting it up](https://github.com/Blob2763/easydebugger?tab=readme-ov-file#setting-it-up)
+- [docs](https://github.com/Blob2763/easydebugger?tab=readme-ov-file#docs)
+- [faq](https://github.com/Blob2763/easydebugger?tab=readme-ov-file#faq)
+- [changelog](https://github.com/Blob2763/easydebugger?tab=readme-ov-file#changelog)
+- [future plans](https://github.com/Blob2763/easydebugger?tab=readme-ov-file#future-plans)
 
 ## setting it up
 simple stuff for installing any library
 
 ### 1. installation
 install the library using `pip install easydebugger`
 
 ### 2. importing the library
 ```py
 import easydebugger as ed
 ```
 
-## functions
+## docs
 
 ### messages
 there are 3 types of messages to choose from:
 - error
 - warn
 - success
 
@@ -355,14 +361,15 @@
 | `ed.success()`                                  | `SUCCESS`  | `"120"`        |
 | `ed.variable()`                                 | `VARIABLE` | `"208"`        |
 | `ed.log()`                                      | `LOG`      | `"15"`         |
 | `ed.start_timer()`                              | `TIME`     | `"93"`         |
 | `ed.end_timer()`                                | `TIME`     | `"93"`         |
 | `ed.trace()`                                    | `TRACE`    | `"27"`         |
 | `ed.display_history()`                          | `HISTORY`  | `"57"`         |
+| `ed.display_stack()`                            | `STACK`    | `"37"`         |
 | all functions above (and `ed.display_message()` | `ESCAPE`   | `u"\u001b[0m"` |
 
 `ed.ESCAPE` contains the escape characters to stop formatting at the end of a message. you shouldn't edit this variable, but you can if you want to
 ```py
 import easydebugger as ed
 
 print(ed.ESCAPE)
@@ -372,12 +379,82 @@
 ed.success("success message")
 ```
 ![image](https://github.com/Blob2763/easydebugger/assets/88489444/6323a581-5f0e-4f4f-abcc-fd4f322be543)
 
 ### start time
 `ed.START_TIME` is the UNIX time in seconds when the code started. it is used for timestamps in history, but you can use it in other places if you want
 
-## plans for the future
+### the stack
+the stack stores the part of the code which is currently running. you can display the stack using `ed.display_stack()`
+```py
+import easydebugger as ed
+
+ed.display_stack()
+```
+![image](https://github.com/Blob2763/easydebugger/assets/88489444/456a81d7-971b-4e6a-a87e-a5a68fab9c37)
+
+each layer of the stack is called a frame. here is how to read each frame
+![image](https://github.com/Blob2763/easydebugger/assets/88489444/88343eb9-bc83-4d2e-ae8d-9eb054ab43c5)
+
+here's another example with more frames
+```py
+import easydebuggertest as ed
+
+
+def foo():
+    ed.display_stack()
+    
+
+def bar():
+    foo()
+
+
+bar()
+```
+![image](https://github.com/Blob2763/easydebugger/assets/88489444/214ea562-c7ed-42fb-89fd-eb8881600261)
+
+here's a diagram to explain the same stack:
+
+![image](https://github.com/Blob2763/easydebugger/assets/88489444/cf12aaea-74ef-4c83-9aae-9078945e8f84)
+
+## faq
+### why don't i have all the features?
+make sure you are using the latest version of easydebugger. run `pip install --upgrade easydebugger` in the terminal. if you aren't on the latest version, this command will update easydebugger for you.
+
+### i have found a bug, what do i do?
+if you have found a bug, check any existing issues first to make sure someone else hasn't already found it. if you've found a new bug, [create an issue](https://github.com/Blob2763/easydebugger/issues/new). here are some tips to create the best bug report:
+- explain clearly what the bug is. what was the intended result and what actually happened?
+- explain or show how to recreate the bug. if you can, include code that recreates the bug
+- try to include a screenshot of the bug, especially what happened as a result of the bug
+- include any other information you find relevant
+- most importantly, add the bug label to the issue. this helps me find it faster
+
+### i have an idea for a feature to be added, what should i do?
+all ideas are welcome! if you have an idea you think would make easydebugger better, [create an issue](https://github.com/Blob2763/easydebugger/issues/new). follow these steps to create the best feature request:
+- explain clearly what you want to see added.
+- give a reason why you want to see it added. something like "i think it would be cool" is a valid reason, but try to be more specific if you can.
+- most importantly, add the enhancement label to the issue. this helps me find it faster
+
+### i have a question that isn't answered here
+[create an issue](https://github.com/Blob2763/easydebugger/issues/new) using the question label, and put a question you have in the issue. i will try to answer your question, and it might even make it to the faq!
+
+## changelog
+### 0.0.1
+- library first published
+### 1.0.0
+- initial release
+- long description added to pypi
+### 1.0.1
+- added docs
+### 1.1.0
+- attempted to fix [#1](https://github.com/Blob2763/easydebugger/issues/1)
+### 1.1.1
+- actually fixed [#1](https://github.com/Blob2763/easydebugger/issues/1)
+### 1.2.0
+- added `ed.display_stack()`
+### 1.2.1
+- fixed [#2](https://github.com/Blob2763/easydebugger/issues/2)
+
+## future plans
 im really happy with how this has turned out, but i still want to add more:
 - automatically try to detect variable name in `ed.variable()`
 - make some usage examples
-- an faq
```

### Comparing `easydebugger-1.2.0/easydebugger/__init__.py` & `easydebugger-1.2.1/easydebugger/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 timers = {}
 traces = []
 history = []
 
 
 def format_text(code, text, is_background=False):
     if is_background:
-        return u"\u001b[48;5;" + code + "m" + text + ESCAPE
+        return f"\u001b[48;5;{code}m{text}{ESCAPE}"
     else:
-        return u"\u001b[38;5;" + code + "m" + text + ESCAPE
+        return f"\u001b[38;5;{code}m{text}{ESCAPE}"
 
 
 def history_log(symbol, colour, message, label, line_number):
     now = t.time()
     seconds_since_start = now - START_TIME
     
     stack = inspect.stack()
```

### Comparing `easydebugger-1.2.0/setup.py` & `easydebugger-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 NAME = "easydebugger"
-VERSION = '1.2.0'
+VERSION = '1.2.1'
 DESCRIPTION = 'A clean Python debugging tool'
 LONG_DESCRIPTION = 'A clean Python debugging tool. Documentation at https://github.com/Blob2763/easydebugger'
 
 # Setting up
 setup(
     name=NAME,
     version=VERSION,
```

