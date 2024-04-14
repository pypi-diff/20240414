# Comparing `tmp/objd-2.tar.gz` & `tmp/objd-3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objd-2.tar", last modified: Fri Apr 12 22:46:09 2024, max compression
+gzip compressed data, was "objd-3.tar", last modified: Fri Apr 12 23:42:45 2024, max compression
```

## Comparing `objd-2.tar` & `objd-3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-12 22:46:09.371814 objd-2/
--rw-r--r--   0 bart      (1000) bart      (1000)     3715 2024-04-12 22:46:09.371814 objd-2/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     3192 2024-04-12 22:29:33.000000 objd-2/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-12 22:46:09.367814 objd-2/bin/
--rwxr-xr-x   0 bart      (1000) bart      (1000)     4014 2024-04-12 14:30:42.000000 objd-2/bin/objd
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-12 22:46:09.371814 objd-2/objd/
--rw-r--r--   0 bart      (1000) bart      (1000)      411 2024-04-12 15:45:57.000000 objd-2/objd/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1414 2024-04-12 14:26:34.000000 objd-2/objd/broker.py
--rw-r--r--   0 bart      (1000) bart      (1000)      206 2024-04-12 14:26:34.000000 objd-2/objd/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1000)      377 2024-04-12 14:26:34.000000 objd-2/objd/err.py
--rw-r--r--   0 bart      (1000) bart      (1000)      388 2024-04-12 14:26:34.000000 objd-2/objd/flt.py
--rw-r--r--   0 bart      (1000) bart      (1000)      746 2024-04-12 14:26:34.000000 objd-2/objd/fnd.py
--rw-r--r--   0 bart      (1000) bart      (1000)    17463 2024-04-12 21:59:34.000000 objd-2/objd/irc.py
--rw-r--r--   0 bart      (1000) bart      (1000)      681 2024-04-12 14:26:34.000000 objd-2/objd/log.py
--rw-r--r--   0 bart      (1000) bart      (1000)      235 2024-04-12 14:26:34.000000 objd-2/objd/mod.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2395 2024-04-12 14:26:34.000000 objd-2/objd/req.py
--rw-r--r--   0 bart      (1000) bart      (1000)     9730 2024-04-12 14:26:34.000000 objd-2/objd/rss.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1090 2024-04-12 14:26:34.000000 objd-2/objd/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1030 2024-04-12 14:26:34.000000 objd-2/objd/thr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     4980 2024-04-12 14:26:34.000000 objd-2/objd/tmr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1235 2024-04-12 14:26:34.000000 objd-2/objd/utils.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-12 22:46:09.371814 objd-2/objd.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     3715 2024-04-12 22:46:09.000000 objd-2/objd.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      395 2024-04-12 22:46:09.000000 objd-2/objd.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-12 22:46:09.000000 objd-2/objd.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)       10 2024-04-12 22:46:09.000000 objd-2/objd.egg-info/requires.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        5 2024-04-12 22:46:09.000000 objd-2/objd.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-12 22:46:09.000000 objd-2/objd.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1000)      775 2024-04-12 15:36:27.000000 objd-2/pyproject.toml
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-12 22:46:09.371814 objd-2/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-04-12 14:25:38.000000 objd-2/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-12 23:42:45.463729 objd-3/
+-rw-r--r--   0 bart      (1000) bart      (1000)     3805 2024-04-12 23:42:45.463729 objd-3/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     3282 2024-04-12 23:42:19.000000 objd-3/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-12 23:42:45.459729 objd-3/bin/
+-rwxr-xr-x   0 bart      (1000) bart      (1000)     4006 2024-04-12 23:36:50.000000 objd-3/bin/objd
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-12 23:42:45.459729 objd-3/objd/
+-rw-r--r--   0 bart      (1000) bart      (1000)      411 2024-04-12 15:45:57.000000 objd-3/objd/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1414 2024-04-12 14:26:34.000000 objd-3/objd/broker.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      206 2024-04-12 14:26:34.000000 objd-3/objd/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      377 2024-04-12 14:26:34.000000 objd-3/objd/err.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      388 2024-04-12 14:26:34.000000 objd-3/objd/flt.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      746 2024-04-12 14:26:34.000000 objd-3/objd/fnd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    17463 2024-04-12 21:59:34.000000 objd-3/objd/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      681 2024-04-12 14:26:34.000000 objd-3/objd/log.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      235 2024-04-12 14:26:34.000000 objd-3/objd/mod.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2395 2024-04-12 14:26:34.000000 objd-3/objd/req.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     9730 2024-04-12 14:26:34.000000 objd-3/objd/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1090 2024-04-12 14:26:34.000000 objd-3/objd/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1030 2024-04-12 14:26:34.000000 objd-3/objd/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     4980 2024-04-12 14:26:34.000000 objd-3/objd/tmr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1235 2024-04-12 14:26:34.000000 objd-3/objd/utils.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-12 23:42:45.463729 objd-3/objd.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     3805 2024-04-12 23:42:45.000000 objd-3/objd.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      395 2024-04-12 23:42:45.000000 objd-3/objd.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-12 23:42:45.000000 objd-3/objd.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)       10 2024-04-12 23:42:45.000000 objd-3/objd.egg-info/requires.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        5 2024-04-12 23:42:45.000000 objd-3/objd.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-12 23:42:45.000000 objd-3/objd.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1000)      775 2024-04-12 23:37:50.000000 objd-3/pyproject.toml
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-12 23:42:45.463729 objd-3/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-04-12 14:25:38.000000 objd-3/setup.py
```

### Comparing `objd-2/PKG-INFO` & `objd-3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objd
-Version: 2
+Version: 3
 Summary: object daemon
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/objd
 Project-URL: bugs, https://github.com/xobjectz/objd/issues
 Project-URL: source, https://github.com/xobjectz/objd
 Classifier: Development Status :: 3 - Alpha
@@ -63,20 +63,21 @@
 
     OBJD is Public Domain.
 
 USAGE
 
 ::
 
-    without any argument the program does nothing
+    without any argument the program starts a daemon
 
     $ objd
     $
 
-    see list of commands
+    with arguments the bot will run it as a command, use `cmd` to see list
+    of commands
 
     $ objd cmd
     cmd,err,mod,req,thr,ver
 
     list of modules
 
     $ objd mod
@@ -161,14 +162,15 @@
     RemainAfterExit=yes
 
     [Install]
     WantedBy=default.target
 
     then run this
 
+    $ pipx ensurepath
     $ mkdir ~/.objd
     $ sudo systemctl enable objd --now
 
     default channel/server is #objd on localhost
 
 FILES
 
@@ -178,14 +180,14 @@
     ~/.local/bin/objd
     ~/.local/pipx/venvs/objd/
 
 AUTHOR
 
 ::
 
-    Bart Thate <objx@proton.me>
+    Bart Thate <bthate@dds.nl>
 
 COPYRIGHT
 
 ::
 
     OBJD is Public Domain.
```

### Comparing `objd-2/README.rst` & `objd-3/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -47,20 +47,21 @@
 
     OBJD is Public Domain.
 
 USAGE
 
 ::
 
-    without any argument the program does nothing
+    without any argument the program starts a daemon
 
     $ objd
     $
 
-    see list of commands
+    with arguments the bot will run it as a command, use `cmd` to see list
+    of commands
 
     $ objd cmd
     cmd,err,mod,req,thr,ver
 
     list of modules
 
     $ objd mod
@@ -145,14 +146,15 @@
     RemainAfterExit=yes
 
     [Install]
     WantedBy=default.target
 
     then run this
 
+    $ pipx ensurepath
     $ mkdir ~/.objd
     $ sudo systemctl enable objd --now
 
     default channel/server is #objd on localhost
 
 FILES
 
@@ -162,14 +164,14 @@
     ~/.local/bin/objd
     ~/.local/pipx/venvs/objd/
 
 AUTHOR
 
 ::
 
-    Bart Thate <objx@proton.me>
+    Bart Thate <bthate@dds.nl>
 
 COPYRIGHT
 
 ::
 
     OBJD is Public Domain.
```

### Comparing `objd-2/bin/objd` & `objd-3/bin/objd`

 * *Files 1% similar despite different names*

```diff
@@ -149,30 +149,30 @@
 
 "runtime"
 
 
 def main():
     skel()
     parse_cmd(Cfg, " ".join(sys.argv[1:]))
+    if Cfg.txt:
+        return cmnd(Cfg.otxt, print)
     if 'a' in Cfg.opts:
         Cfg.mod = ",".join(objd.__dir__())
     if "v" in Cfg.opts:
         debug(f"{Cfg.name.upper()} {Cfg.opts.upper()} started {dte}")
     if "h" in Cfg.opts:
         print(__doc__)
         return
     if "c" in Cfg.opts:
         init(objd, Cfg.mod, Cfg.sets.dis, True)
         csl = Console()
         csl.start()
         while 1:
             time.sleep(1.0)
         return
-    if 'x' in Cfg.opts:
-        return cmnd(Cfg.otxt, print)
     Cfg.mod = ",".join(objd.__dir__())
     Cfg.user = getpass.getuser()
     daemon(Cfg.pidfile, "v" in Cfg.opts)
     privileges(Cfg.user)
     init(objd, Cfg.mod, Cfg.sets.dis, True)
     while 1:
         time.sleep(1.0)
```

### Comparing `objd-2/objd/broker.py` & `objd-3/objd/broker.py`

 * *Files identical despite different names*

### Comparing `objd-2/objd/fnd.py` & `objd-3/objd/fnd.py`

 * *Files identical despite different names*

### Comparing `objd-2/objd/irc.py` & `objd-3/objd/irc.py`

 * *Files identical despite different names*

### Comparing `objd-2/objd/log.py` & `objd-3/objd/log.py`

 * *Files identical despite different names*

### Comparing `objd-2/objd/req.py` & `objd-3/objd/req.py`

 * *Files identical despite different names*

### Comparing `objd-2/objd/rss.py` & `objd-3/objd/rss.py`

 * *Files identical despite different names*

### Comparing `objd-2/objd/tdo.py` & `objd-3/objd/tdo.py`

 * *Files identical despite different names*

### Comparing `objd-2/objd/thr.py` & `objd-3/objd/thr.py`

 * *Files identical despite different names*

### Comparing `objd-2/objd/tmr.py` & `objd-3/objd/tmr.py`

 * *Files identical despite different names*

### Comparing `objd-2/objd/utils.py` & `objd-3/objd/utils.py`

 * *Files identical despite different names*

### Comparing `objd-2/objd.egg-info/PKG-INFO` & `objd-3/objd.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objd
-Version: 2
+Version: 3
 Summary: object daemon
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/objd
 Project-URL: bugs, https://github.com/xobjectz/objd/issues
 Project-URL: source, https://github.com/xobjectz/objd
 Classifier: Development Status :: 3 - Alpha
@@ -63,20 +63,21 @@
 
     OBJD is Public Domain.
 
 USAGE
 
 ::
 
-    without any argument the program does nothing
+    without any argument the program starts a daemon
 
     $ objd
     $
 
-    see list of commands
+    with arguments the bot will run it as a command, use `cmd` to see list
+    of commands
 
     $ objd cmd
     cmd,err,mod,req,thr,ver
 
     list of modules
 
     $ objd mod
@@ -161,14 +162,15 @@
     RemainAfterExit=yes
 
     [Install]
     WantedBy=default.target
 
     then run this
 
+    $ pipx ensurepath
     $ mkdir ~/.objd
     $ sudo systemctl enable objd --now
 
     default channel/server is #objd on localhost
 
 FILES
 
@@ -178,14 +180,14 @@
     ~/.local/bin/objd
     ~/.local/pipx/venvs/objd/
 
 AUTHOR
 
 ::
 
-    Bart Thate <objx@proton.me>
+    Bart Thate <bthate@dds.nl>
 
 COPYRIGHT
 
 ::
 
     OBJD is Public Domain.
```

### Comparing `objd-2/pyproject.toml` & `objd-3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "objd"
 description = "object daemon"
-version = "2"
+version = "3"
 authors = [
     {name = "Bart Thate",email = "bthate@dds.nl"},
 ]
 readme = "README.rst"
 license = {text="Public Domain"}
 dependencies = [
     'objx',
```

