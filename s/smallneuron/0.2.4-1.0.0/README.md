# Comparing `tmp/smallneuron-0.2.4.tar.gz` & `tmp/smallneuron-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smallneuron-0.2.4.tar", last modified: Mon Mar  4 20:39:49 2024, max compression
+gzip compressed data, was "smallneuron-1.0.0.tar", last modified: Sun Apr 14 21:38:09 2024, max compression
```

## Comparing `smallneuron-0.2.4.tar` & `smallneuron-1.0.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-03-04 20:39:49.901161 smallneuron-0.2.4/
--rw-rw-r--   0 andres    (1000) andres    (1000)      441 2024-02-20 00:54:30.000000 smallneuron-0.2.4/.gitignore
--rw-rw-r--   0 andres    (1000) andres    (1000)     1074 2024-02-18 18:56:34.000000 smallneuron-0.2.4/LICENSE
--rw-r--r--   0 andres    (1000) andres    (1000)     1053 2024-03-04 20:39:49.901161 smallneuron-0.2.4/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      558 2024-02-18 18:56:34.000000 smallneuron-0.2.4/README.md
--rw-rw-r--   0 andres    (1000) andres    (1000)     3641 2024-02-18 18:56:34.000000 smallneuron-0.2.4/example.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      655 2024-03-04 20:39:09.000000 smallneuron-0.2.4/pyproject.toml
--rw-rw-r--   0 andres    (1000) andres    (1000)       38 2024-03-04 20:39:49.901161 smallneuron-0.2.4/setup.cfg
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-03-04 20:39:49.897160 smallneuron-0.2.4/src/
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-03-04 20:39:49.901161 smallneuron-0.2.4/src/smallneuron/
--rw-rw-r--   0 andres    (1000) andres    (1000)      242 2024-02-18 18:56:34.000000 smallneuron-0.2.4/src/smallneuron/__init__.py
--rwxrwxr-x   0 andres    (1000) andres    (1000)      231 2024-02-18 18:56:34.000000 smallneuron-0.2.4/src/smallneuron/build
--rw-rw-r--   0 andres    (1000) andres    (1000)    21308 2024-02-18 18:56:34.000000 smallneuron-0.2.4/src/smallneuron/gpio_h3.c
--rw-rw-r--   0 andres    (1000) andres    (1000)     7411 2024-02-18 18:56:34.000000 smallneuron-0.2.4/src/smallneuron/gpio_h3.h
--rwxrwxr-x   0 andres    (1000) andres    (1000)    26760 2024-02-18 18:56:34.000000 smallneuron-0.2.4/src/smallneuron/gpio_h3.so
--rw-rw-r--   0 andres    (1000) andres    (1000)     1392 2024-02-20 00:53:18.000000 smallneuron-0.2.4/src/smallneuron/logger.py
--rw-rw-r--   0 andres    (1000) andres    (1000)    13530 2024-03-04 20:38:32.000000 smallneuron-0.2.4/src/smallneuron/smallneuron.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      993 2024-02-18 18:56:34.000000 smallneuron-0.2.4/src/smallneuron/sndummy.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     1410 2024-02-18 18:56:34.000000 smallneuron-0.2.4/src/smallneuron/sngpio.py
--rwxrwxr-x   0 andres    (1000) andres    (1000)     4038 2024-02-18 18:56:34.000000 smallneuron-0.2.4/src/smallneuron/snhttp.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     3003 2024-03-04 20:31:52.000000 smallneuron-0.2.4/src/smallneuron/sninput.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     2273 2024-02-18 18:56:34.000000 smallneuron-0.2.4/src/smallneuron/snmqtt.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     2542 2024-03-04 20:31:52.000000 smallneuron-0.2.4/src/smallneuron/snserial.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      977 2024-02-19 10:54:59.000000 smallneuron-0.2.4/src/smallneuron/sntimer.py
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-03-04 20:39:49.901161 smallneuron-0.2.4/src/smallneuron.egg-info/
--rw-r--r--   0 andres    (1000) andres    (1000)     1053 2024-03-04 20:39:49.000000 smallneuron-0.2.4/src/smallneuron.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      775 2024-03-04 20:39:49.000000 smallneuron-0.2.4/src/smallneuron.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-03-04 20:39:49.000000 smallneuron-0.2.4/src/smallneuron.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-03-04 20:39:49.000000 smallneuron-0.2.4/src/smallneuron.egg-info/top_level.txt
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-03-04 20:39:49.901161 smallneuron-0.2.4/src/smallneuron_pelainux.egg-info/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1062 2024-02-18 18:56:34.000000 smallneuron-0.2.4/src/smallneuron_pelainux.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      496 2024-02-18 18:56:34.000000 smallneuron-0.2.4/src/smallneuron_pelainux.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-02-18 18:56:34.000000 smallneuron-0.2.4/src/smallneuron_pelainux.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-02-18 18:56:34.000000 smallneuron-0.2.4/src/smallneuron_pelainux.egg-info/top_level.txt
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-14 21:38:09.146995 smallneuron-1.0.0/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      441 2024-02-20 00:54:30.000000 smallneuron-1.0.0/.gitignore
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1074 2024-02-18 18:56:34.000000 smallneuron-1.0.0/LICENSE
+-rw-r--r--   0 andres    (1000) andres    (1000)     1053 2024-04-14 21:38:09.146995 smallneuron-1.0.0/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      558 2024-02-18 18:56:34.000000 smallneuron-1.0.0/README.md
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3645 2024-04-14 20:50:42.000000 smallneuron-1.0.0/example.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      655 2024-04-14 21:16:52.000000 smallneuron-1.0.0/pyproject.toml
+-rw-rw-r--   0 andres    (1000) andres    (1000)       38 2024-04-14 21:38:09.146995 smallneuron-1.0.0/setup.cfg
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-14 21:38:09.142995 smallneuron-1.0.0/src/
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-14 21:38:09.146995 smallneuron-1.0.0/src/smallneuron/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      242 2024-02-18 18:56:34.000000 smallneuron-1.0.0/src/smallneuron/__init__.py
+-rwxrwxr-x   0 andres    (1000) andres    (1000)      231 2024-02-18 18:56:34.000000 smallneuron-1.0.0/src/smallneuron/build
+-rw-rw-r--   0 andres    (1000) andres    (1000)    21308 2024-02-18 18:56:34.000000 smallneuron-1.0.0/src/smallneuron/gpio_h3.c
+-rw-rw-r--   0 andres    (1000) andres    (1000)     7411 2024-02-18 18:56:34.000000 smallneuron-1.0.0/src/smallneuron/gpio_h3.h
+-rwxrwxr-x   0 andres    (1000) andres    (1000)    26760 2024-02-18 18:56:34.000000 smallneuron-1.0.0/src/smallneuron/gpio_h3.so
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1392 2024-02-20 00:53:18.000000 smallneuron-1.0.0/src/smallneuron/logger.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)    13759 2024-04-14 21:12:38.000000 smallneuron-1.0.0/src/smallneuron/smallneuron.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      993 2024-02-18 18:56:34.000000 smallneuron-1.0.0/src/smallneuron/sndummy.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1410 2024-02-18 18:56:34.000000 smallneuron-1.0.0/src/smallneuron/sngpio.py
+-rwxrwxr-x   0 andres    (1000) andres    (1000)     4038 2024-02-18 18:56:34.000000 smallneuron-1.0.0/src/smallneuron/snhttp.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3003 2024-03-04 20:31:52.000000 smallneuron-1.0.0/src/smallneuron/sninput.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     2273 2024-02-18 18:56:34.000000 smallneuron-1.0.0/src/smallneuron/snmqtt.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     2542 2024-03-04 20:31:52.000000 smallneuron-1.0.0/src/smallneuron/snserial.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      977 2024-02-19 10:54:59.000000 smallneuron-1.0.0/src/smallneuron/sntimer.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-14 21:38:09.146995 smallneuron-1.0.0/src/smallneuron.egg-info/
+-rw-r--r--   0 andres    (1000) andres    (1000)     1053 2024-04-14 21:38:09.000000 smallneuron-1.0.0/src/smallneuron.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      775 2024-04-14 21:38:09.000000 smallneuron-1.0.0/src/smallneuron.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-04-14 21:38:09.000000 smallneuron-1.0.0/src/smallneuron.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-04-14 21:38:09.000000 smallneuron-1.0.0/src/smallneuron.egg-info/top_level.txt
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-14 21:38:09.146995 smallneuron-1.0.0/src/smallneuron_pelainux.egg-info/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1062 2024-02-18 18:56:34.000000 smallneuron-1.0.0/src/smallneuron_pelainux.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      496 2024-02-18 18:56:34.000000 smallneuron-1.0.0/src/smallneuron_pelainux.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-02-18 18:56:34.000000 smallneuron-1.0.0/src/smallneuron_pelainux.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-02-18 18:56:34.000000 smallneuron-1.0.0/src/smallneuron_pelainux.egg-info/top_level.txt
```

### Comparing `smallneuron-0.2.4/LICENSE` & `smallneuron-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smallneuron-0.2.4/PKG-INFO` & `smallneuron-1.0.0/src/smallneuron_pelainux.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: smallneuron
-Version: 0.2.4
+Name: smallneuron_pelainux
+Version: 0.1.4
 Summary: Small Neuron Workflow
 Author-email: Andres Artigas <andres@artigas.cl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `smallneuron-0.2.4/README.md` & `smallneuron-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `smallneuron-0.2.4/example.py` & `smallneuron-1.0.0/example.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 # Ejemplo de nodo customizado
 # cuando llega a este nodo 
 # publica en mqtt y dibuja en tkinker
 class PubNode(Node) :
     def __init__(self, state):
         super().__init__(state)
         
-    def run(self, event, dict_eventargs, stateFrom):
-        print("PubNode: Run:", self.state, "event trigger:", event, "from", stateFrom )
+    def enter(self, event, dict_eventargs, stateFrom):
+        print("PubNode: Enter:", self.state, "event trigger:", event, "from", stateFrom )
         mqtt.publish("EsteRecontraTopico/"+self.state)
         tkinter.setText("trigger")
 
 
             
 if __name__ == '__main__': 
     #########################
```

### Comparing `smallneuron-0.2.4/pyproject.toml` & `smallneuron-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 
 [project]
 name = "smallneuron"
-version = "0.2.4"
+version = "1.0.0"
 authors = [
   { name="Andres Artigas", email="andres@artigas.cl" },
 ]
 description = "Small Neuron Workflow"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `smallneuron-0.2.4/src/smallneuron/gpio_h3.c` & `smallneuron-1.0.0/src/smallneuron/gpio_h3.c`

 * *Files identical despite different names*

### Comparing `smallneuron-0.2.4/src/smallneuron/gpio_h3.h` & `smallneuron-1.0.0/src/smallneuron/gpio_h3.h`

 * *Files identical despite different names*

### Comparing `smallneuron-0.2.4/src/smallneuron/gpio_h3.so` & `smallneuron-1.0.0/src/smallneuron/gpio_h3.so`

 * *Files identical despite different names*

### Comparing `smallneuron-0.2.4/src/smallneuron/logger.py` & `smallneuron-1.0.0/src/smallneuron/logger.py`

 * *Files identical despite different names*

### Comparing `smallneuron-0.2.4/src/smallneuron/smallneuron.py` & `smallneuron-1.0.0/src/smallneuron/smallneuron.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,30 +28,33 @@
     nodelist = {}
 
     def __init__(self, state, desc="", style=""):
         self.state = state
         self.event_manager = None  # Este link es llenado durante addEdge del event manager
         self.desc = desc
         self.style = style
-        self.changeState = True
+        self._cmd=False
         if state in Node.nodelist:
             raise "Estado ya existe como Nodo" + state
         Node.nodelist[state] = self
 
-    def run(self, event, args, stateFrom):
-        print("Node: Run:", self.state, "event trigger:", event, "from", stateFrom)
+    def enter(self, event, args, stateFrom):
+        print("Node: Enter:", self.state, "event trigger:", event, "from", stateFrom)
+
+    def leave(self, event, args, stateTo):
+        print("Node: Leave:", self.state, "event trigger:", event, "to", stateTo)
 
     def __eq__(self, other):
         return self.state == other.state
 
 
 class LambdaNode(Node):
-    def __init__(self, state, lambdaRun, desc="", style=""):
+    def __init__(self, state, lambdaEnter, desc="", style=""):
         super().__init__(state, desc, style)
-        self.run = lambdaRun
+        self.enter = lambdaEnter
 
     def __eq__(self, other):
         return self.state == other.state
 
 
 # def TimerThread(queue, event, args, time, logging):
 #     # print("TimerThread ", event, time, "s")
@@ -60,14 +63,15 @@
 #     # print("TimerThread ", event, " done")
 
 
 class EventManager:
     def __init__(self, graphDir_and_prefix="."):
         self.currentState = None
         self.currentArgs = None
+        self.currentNode =None
         self.prevState = None
         self.count = 0 # state count
         self.graph_n = 0
         self.events = queue.SimpleQueue()
         self.net = (
             {}
         )  # estructura es { "evento1": { "estado Origen1" : (nodoDestino1, "event_desc1" ), "estadoOrigen2": (nodoDestino2, "event_desc2") }, "evento2"...
@@ -103,25 +107,25 @@
             else:
                 self.net[event][nodeFrom.state] = (nodeTo, desc)
         else:
             self.net[event] = {nodeFrom.state: (nodeTo, desc)}
             nodeFrom.event_manager = self
             nodeTo.event_manager = self
 
-    def linkCmd(self, event, nodeTo: Node, changeState=False, desc=""):
+    def linkCmd(self, event, nodeTo: Node, desc=""):
         if event in self.cmds:
             print("Error event already in cmds ", event)
             raise "Error event already in cmds "
         elif event in self.net:
             print("Error event already in edges ", event)
             raise "Error event already in edges "
         else:
             self.cmds[event] = (nodeTo, desc)
             nodeTo.event_manager = self
-            nodeTo.changeState = changeState
+            nodeTo._cmd =True
 
     def graph(self, f, bold_event=None):
         f.write("digraph { \n")
         f.write('  layout="dot" \n')
         f.write("  //rankdir=LR \n")
         f.write('  graph [ overlap="true" fontsize = 10 ] \n')
         f.write('  node [ style="rounded,filled" shape="rect" fillcolor="#0000a0", fontcolor=white ]')
@@ -131,15 +135,15 @@
             style = node.style
             if node.desc != "":
                 style = style + ' tooltip="' + ttfmt(node.desc) + '"'
             if state == self.currentState:
                 style = style + ' fillcolor="#a00000"'
             elif state == self.prevState:
                 style = style + ' fillcolor="#fed104" fontcolor=black'
-            if node.changeState == False:
+            if node._cmd == True:
                 style = style + ' fillcolor="#a0a0a0"'
 
             f.write("%s [%s]\n" % (state, style))
 
         # print("write ", len(self.net), "events")
         for event in self.net:
             for state_from in self.net[event]:
@@ -160,15 +164,14 @@
                     f.write('%s -> %s [ label = "%s" %s  ]\n' % (state_from, state_to, event, tooltip))
 
         # print("write ", len(self.cmds), "commands")
         if len(self.cmds) > 0:
             f.write(
                 '"*" [ label="" style="filled" fixedsize=true width=0.2 shape="circle" fillcolor="red" tooltip = "desde todos los estados" ]\n'
             )
-
             for event in self.cmds:
                 state_to = self.cmds[event][0].state
                 desc = self.cmds[event][1]
 
                 tooltip = ""
                 if desc != "":
                     tooltip = 'labeltooltip="' + ttfmt(desc) + '" tooltip="' + ttfmt(desc) + '"'
@@ -207,56 +210,60 @@
         n_start = Node(
             "_start_",
             desc="start",
             style='label="" style="filled" fixedsize=true width=0.2 shape="circle" fillcolor="green"',
         )
         self.linkEdge("_start_", n_start, n_first, desc="start")
         self.currentState = "_start_"
+        self.currentNode=n_start
         threading.Thread(target=self.loop).start()
         self.putEvent("_start_")  # lanzamos evento de inicio
 
     def loop(self):
         try:
             self.printGraph()
             while True:
                 log.notice("[",self.count,"] State:", self.currentState)
                 eventTuple = self.events.get()
                 event  = eventTuple[0]  # text del evento
                 params = eventTuple[1]  # argumentos del evento
 
                 log.notice("[",self.count,"] Event:", event, params)
+                
 
-                # eliminamos el validUntil
+                # eliminamos el validUntil, para que no quede en un loop
                 validUntil=self.count
                 if type(params) == dict:
                     validUntil=params.pop("validUntil", self.count)
 
                 if validUntil < self.count:
                     log.warn("[",self.count,"] ", event, " is caduced ", validUntil, "<", self.count)
 
                 elif event in self.net:
                     if not self.currentState in self.net[event]:
                         log.warn("[",self.count,"] ", event, " not valid for state ", self.currentState, "discarted!")
                     else:
                         node: Node = self.net[event][self.currentState][0]
-                        log.info("[",self.count,"] run ", node.state, eventTuple[1], self.currentState)
-                        node.run(event, eventTuple[1], self.currentState)
-                        if node.changeState:
-                            self.prevState = self.currentState
-                            self.currentState = node.state
-                            self.currentArgs = params
-                            self.count = self.count + 1  # increment event count
+                        log.info("[",self.count,"] enter ", node.state, params, self.currentState)
+                        
+                        # indicamos al nodo actual que salimos
+                        self.currentNode.leave(event,params,node.state)
+                        
+                        # Entramos al nodo nuevo
+                        node.enter(event, params, self.currentState)
+                        self.currentNode=node
+                        self.prevState = self.currentState
+                        self.currentState = node.state
+                        self.currentArgs = params
+                        self.count = self.count + 1  # increment event count
                         self.printGraph(event)
                 elif event in self.cmds:
                     log.info("[", self.count, "] Manager new  cmd ", event)
                     node: Node = self.cmds[event][0]
-                    node.run(event, eventTuple[1], self.currentState)
-                    if node.changeState:
-                        self.currentState = node.state
-                        self.count = self.count + 1  # increment event count
+                    node.enter(event, params, self.currentState)
                     self.printGraph(event)
                 else:
                     log.warn("[",self.count,"] ", event, " not exist")
         except Exception as e:
             log.error(e)
             log.error(traceback.format_exc())
             exit(1)
@@ -264,15 +271,15 @@
 
 class SnWatcher():
     '''
     Cada instancia de esta clase monitorea la funcion check() del bridge, con bridge_args como parametros,
     Si la respuesta contiene el bridge_pattern se dispara el evento con event_args que se le agrega "data": respuesta
 
     Consideraciones importantes de la funcion check:
-        1. Debe recibir como parametros los mismo elementos del dict bridge_args de run()
+        1. Debe recibir como parametros los mismo elementos del dict bridge_args de enter()
         2. Debe retornar un diccionario con almenos el elemento data, todo el diccionario retornado
            seran parte del argumento del evento junto a los event_args
         3. Si se repiten los elementos retornados por check() con los events_args mandan los de check()
     una respuesta  hasta que  respuesta, bloqueando
     '''
     def __init__(self, eventManager, event, event_args={}, event_pattern=None):
         self.em=eventManager
```

### Comparing `smallneuron-0.2.4/src/smallneuron/sndummy.py` & `smallneuron-1.0.0/src/smallneuron/sndummy.py`

 * *Files identical despite different names*

### Comparing `smallneuron-0.2.4/src/smallneuron/sngpio.py` & `smallneuron-1.0.0/src/smallneuron/sngpio.py`

 * *Files identical despite different names*

### Comparing `smallneuron-0.2.4/src/smallneuron/snhttp.py` & `smallneuron-1.0.0/src/smallneuron/snhttp.py`

 * *Files identical despite different names*

### Comparing `smallneuron-0.2.4/src/smallneuron/sninput.py` & `smallneuron-1.0.0/src/smallneuron/sninput.py`

 * *Files identical despite different names*

### Comparing `smallneuron-0.2.4/src/smallneuron/snmqtt.py` & `smallneuron-1.0.0/src/smallneuron/snmqtt.py`

 * *Files identical despite different names*

### Comparing `smallneuron-0.2.4/src/smallneuron/snserial.py` & `smallneuron-1.0.0/src/smallneuron/snserial.py`

 * *Files identical despite different names*

### Comparing `smallneuron-0.2.4/src/smallneuron/sntimer.py` & `smallneuron-1.0.0/src/smallneuron/sntimer.py`

 * *Files identical despite different names*

### Comparing `smallneuron-0.2.4/src/smallneuron.egg-info/PKG-INFO` & `smallneuron-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smallneuron
-Version: 0.2.4
+Version: 1.0.0
 Summary: Small Neuron Workflow
 Author-email: Andres Artigas <andres@artigas.cl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `smallneuron-0.2.4/src/smallneuron.egg-info/SOURCES.txt` & `smallneuron-1.0.0/src/smallneuron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smallneuron-0.2.4/src/smallneuron_pelainux.egg-info/PKG-INFO` & `smallneuron-1.0.0/src/smallneuron.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: smallneuron_pelainux
-Version: 0.1.4
+Name: smallneuron
+Version: 1.0.0
 Summary: Small Neuron Workflow
 Author-email: Andres Artigas <andres@artigas.cl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

