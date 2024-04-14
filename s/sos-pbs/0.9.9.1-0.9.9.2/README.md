# Comparing `tmp/sos-pbs-0.9.9.1.tar.gz` & `tmp/sos-pbs-0.9.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sos-pbs-0.9.9.1.tar", last modified: Thu Oct  5 20:59:01 2017, max compression
+gzip compressed data, was "dist/sos-pbs-0.9.9.2.tar", last modified: Wed Oct 18 14:18:11 2017, max compression
```

## Comparing `sos-pbs-0.9.9.1.tar` & `sos-pbs-0.9.9.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-05 20:59:01.000000 sos-pbs-0.9.9.1/
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      337 2017-10-05 16:55:36.000000 sos-pbs-0.9.9.1/MANIFEST.in
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      858 2017-10-05 20:59:01.000000 sos-pbs-0.9.9.1/PKG-INFO
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)       34 2017-10-05 16:55:36.000000 sos-pbs-0.9.9.1/README.md
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)       38 2017-10-05 20:59:01.000000 sos-pbs-0.9.9.1/setup.cfg
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     2323 2017-10-05 20:48:33.000000 sos-pbs-0.9.9.1/setup.py
-drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-05 20:59:01.000000 sos-pbs-0.9.9.1/src/
-drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-05 20:59:01.000000 sos-pbs-0.9.9.1/src/sos_pbs/
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-05 16:55:36.000000 sos-pbs-0.9.9.1/src/sos_pbs/__init__.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     1716 2017-10-05 16:58:01.000000 sos-pbs-0.9.9.1/src/sos_pbs/_version.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    13031 2017-10-05 16:55:36.000000 sos-pbs-0.9.9.1/src/sos_pbs/sos_task.py
-drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-05 20:59:01.000000 sos-pbs-0.9.9.1/src/sos_pbs.egg-info/
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        1 2017-10-05 20:59:01.000000 sos-pbs-0.9.9.1/src/sos_pbs.egg-info/dependency_links.txt
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)       57 2017-10-05 20:59:01.000000 sos-pbs-0.9.9.1/src/sos_pbs.egg-info/entry_points.txt
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      858 2017-10-05 20:59:01.000000 sos-pbs-0.9.9.1/src/sos_pbs.egg-info/PKG-INFO
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        4 2017-10-05 20:59:01.000000 sos-pbs-0.9.9.1/src/sos_pbs.egg-info/requires.txt
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      361 2017-10-05 20:59:01.000000 sos-pbs-0.9.9.1/src/sos_pbs.egg-info/SOURCES.txt
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        8 2017-10-05 20:59:01.000000 sos-pbs-0.9.9.1/src/sos_pbs.egg-info/top_level.txt
-drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-05 20:59:01.000000 sos-pbs-0.9.9.1/test/
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    27001 2017-10-05 16:55:36.000000 sos-pbs-0.9.9.1/test/test_pbs_queue.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        9 2017-10-05 20:49:20.000000 sos-pbs-0.9.9.1/test/tt1.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        9 2017-10-05 20:53:25.000000 sos-pbs-0.9.9.1/test/ttt.py
+drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-18 14:18:11.000000 sos-pbs-0.9.9.2/
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      337 2017-10-05 13:27:46.000000 sos-pbs-0.9.9.2/MANIFEST.in
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      858 2017-10-18 14:18:11.000000 sos-pbs-0.9.9.2/PKG-INFO
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      682 2017-10-18 02:33:48.000000 sos-pbs-0.9.9.2/README.md
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)       38 2017-10-18 14:18:11.000000 sos-pbs-0.9.9.2/setup.cfg
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     2323 2017-10-06 22:35:56.000000 sos-pbs-0.9.9.2/setup.py
+drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-18 14:18:11.000000 sos-pbs-0.9.9.2/src/
+drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-18 14:18:11.000000 sos-pbs-0.9.9.2/src/sos_pbs/
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-04 22:50:33.000000 sos-pbs-0.9.9.2/src/sos_pbs/__init__.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     1716 2017-10-18 14:18:07.000000 sos-pbs-0.9.9.2/src/sos_pbs/_version.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    13053 2017-10-18 02:33:48.000000 sos-pbs-0.9.9.2/src/sos_pbs/sos_task.py
+drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-18 14:18:11.000000 sos-pbs-0.9.9.2/src/sos_pbs.egg-info/
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        1 2017-10-18 14:18:11.000000 sos-pbs-0.9.9.2/src/sos_pbs.egg-info/dependency_links.txt
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)       57 2017-10-18 14:18:11.000000 sos-pbs-0.9.9.2/src/sos_pbs.egg-info/entry_points.txt
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      858 2017-10-18 14:18:11.000000 sos-pbs-0.9.9.2/src/sos_pbs.egg-info/PKG-INFO
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        4 2017-10-18 14:18:11.000000 sos-pbs-0.9.9.2/src/sos_pbs.egg-info/requires.txt
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      387 2017-10-18 14:18:11.000000 sos-pbs-0.9.9.2/src/sos_pbs.egg-info/SOURCES.txt
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        8 2017-10-18 14:18:11.000000 sos-pbs-0.9.9.2/src/sos_pbs.egg-info/top_level.txt
+drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-18 14:18:11.000000 sos-pbs-0.9.9.2/test/
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    23393 2017-10-18 13:53:00.000000 sos-pbs-0.9.9.2/test/test_pbs_queue.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     3335 2017-10-07 17:39:08.000000 sos-pbs-0.9.9.2/test/test_task_spooler.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        9 2017-10-18 13:07:41.000000 sos-pbs-0.9.9.2/test/tt1.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        9 2017-10-07 01:11:11.000000 sos-pbs-0.9.9.2/test/ttt.py
```

### Comparing `sos-pbs-0.9.9.1/PKG-INFO` & `sos-pbs-0.9.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sos-pbs
-Version: 0.9.9.1
+Version: 0.9.9.2
 Summary: PBS task engine for Script of Scripts (SoS)
 Home-page: https://github.com/vatlab/SOS
 Author: Bo Peng
 Author-email: bpeng@mdanderson.org
 License: GPL3
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
```

### Comparing `sos-pbs-0.9.9.1/setup.py` & `sos-pbs-0.9.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `sos-pbs-0.9.9.1/src/sos_pbs/_version.py` & `sos-pbs-0.9.9.2/src/sos_pbs/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     raise SystemError('SOS requires Python 3.4 or higher. Please upgrade your Python {}.{}.{}.'
         .format(_py_ver.major, _py_ver.minor, _py_ver.micro))
 
 
 # version of the SoS language
 __sos_version__ = '1.0'
 # version of the sos command
-__version__ = '0.9.9.1'
+__version__ = '0.9.9.2'
 __py_version__ = '{}.{}.{}'.format(_py_ver.major, _py_ver.minor, _py_ver.micro)
 
 #
 SOS_FULL_VERSION='{} for Python {}.{}.{}'.format(__version__, _py_ver.major, _py_ver.minor, _py_ver.micro)
 SOS_COPYRIGHT = '''SoS {} : Copyright (c) 2016 Bo Peng'''.format(__version__)
 SOS_CONTACT = '''Please visit http://github.com/vatlab/SOS for more information.'''
```

### Comparing `sos-pbs-0.9.9.1/src/sos_pbs/sos_task.py` & `sos-pbs-0.9.9.2/src/sos_pbs/sos_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,17 +176,17 @@
             return result
 
     def _query_job_status(self, job_id, task_id):
         job_id.update({'task': task_id, 'verbosity': 1})
         cmd = cfg_interpolate(self.status_cmd, job_id)
         return self.agent.check_output(cmd)
 
-    def query_tasks(self, tasks=None, verbosity=1, html=False, start_time=True, age=None):
+    def query_tasks(self, tasks=None, verbosity=1, html=False, start_time=True, age=None, tags=None):
         if verbosity <= 2:
-            status_lines = super(PBS_TaskEngine, self).query_tasks(tasks, verbosity, html, start_time, age=age)
+            status_lines = super(PBS_TaskEngine, self).query_tasks(tasks, verbosity, html, start_time, age=age, tags=tags)
             # there is a change that a job is submitted, but failed before the sos command is executed
             # so we will have to ask the task engine about the submitted jobs #608
             if not html:
                 res = ''
                 for line in status_lines.split('\n'):
                     if not line.strip():
                         continue
```

### Comparing `sos-pbs-0.9.9.1/src/sos_pbs.egg-info/PKG-INFO` & `sos-pbs-0.9.9.2/src/sos_pbs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sos-pbs
-Version: 0.9.9.1
+Version: 0.9.9.2
 Summary: PBS task engine for Script of Scripts (SoS)
 Home-page: https://github.com/vatlab/SOS
 Author: Bo Peng
 Author-email: bpeng@mdanderson.org
 License: GPL3
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
```

### Comparing `sos-pbs-0.9.9.1/test/test_pbs_queue.py` & `sos-pbs-0.9.9.2/test/test_pbs_queue.py`

 * *Files 5% similar despite different names*

```diff
@@ -293,137 +293,14 @@
                 'sig_mode': 'force',
                 }).run()
         self.assertTrue(FileTarget('tt1.py.bak').exists('target'))
         # the files should be the same
         with open('tt1.py') as ori, open('tt1.py.bak') as bak:
             self.assertEqual(ori.read(), bak.read())
 
-    @unittest.skipIf(not has_docker, "Docker container not usable")
-    def testMaxMem(self):
-        '''Test server restriction max_mem'''
-        script = SoS_Script('''
-[10]
-task: mem='2G'
-print('a')
-''')
-        wf = script.workflow()
-        self.assertRaises(Exception, Base_Executor(wf, config={
-                'config_file': '~/docker.yml',
-                # do not wait for jobs
-                'wait_for_task': True,
-                'default_queue': 'docker_limited',
-                'sig_mode': 'force',
-                }).run)
-
-    def testLocalMaxMem(self):
-        '''Test server restriction max_mem'''
-        script = SoS_Script('''
-[10]
-task: mem='2G'
-print('a')
-''')
-        wf = script.workflow()
-        self.assertRaises(Exception, Base_Executor(wf, config={
-                'config_file': '~/docker.yml',
-                # do not wait for jobs
-                'wait_for_task': True,
-                'default_queue': 'local_limited',
-                'sig_mode': 'force',
-                }).run)
-
-    @unittest.skipIf(not has_docker, "Docker container not usable")
-    def testRuntimeMaxWalltime(self):
-        '''Test server max_walltime option'''
-        script = SoS_Script('''
-[10]
-task:
-import time
-time.sleep(15)
-''')
-        wf = script.workflow()
-        self.assertRaises(Exception, Base_Executor(wf, config={
-                'config_file': '~/docker.yml',
-                # do not wait for jobs
-                'wait_for_task': True,
-                'default_queue': 'docker_limited',
-                'sig_mode': 'force',
-                }).run)
-
-    def testLocalRuntimeMaxWalltime(self):
-        '''Test server max_walltime option'''
-        script = SoS_Script('''
-[10]
-task:
-import time
-time.sleep(15)
-''')
-        wf = script.workflow()
-        self.assertRaises(Exception, Base_Executor(wf, config={
-                'config_file': '~/docker.yml',
-                # do not wait for jobs
-                'wait_for_task': True,
-                'default_queue': 'local_limited',
-                'sig_mode': 'force',
-                }).run)
-
-    @unittest.skipIf(not has_docker, "Docker container not usable")
-    def testMaxCores(self):
-        '''Test server restriction max_cores'''
-        script = SoS_Script('''
-[10]
-task: cores=8
-print('a')
-''')
-        wf = script.workflow()
-        self.assertRaises(Exception, Base_Executor(wf, config={
-                'config_file': '~/docker.yml',
-                # do not wait for jobs
-                'wait_for_task': True,
-                'default_queue': 'docker_limited',
-                'sig_mode': 'force',
-                }).run)
-
-    def testLocalMaxCores(self):
-        '''Test server restriction max_cores'''
-        script = SoS_Script('''
-[10]
-task: cores=8
-print('a')
-''')
-        wf = script.workflow()
-        self.assertRaises(Exception, Base_Executor(wf, config={
-                'config_file': '~/docker.yml',
-                # do not wait for jobs
-                'wait_for_task': True,
-                'default_queue': 'local_limited',
-                'sig_mode': 'force',
-                }).run)
-
-    def testListHosts(self):
-        '''test list hosts using sos status -q'''
-        for v in ['0', '1', '3', '4']:
-            output = subprocess.check_output(['sos', 'status', '-c', '~/docker.yml', '-q', '-v', v]).decode()
-            self.assertTrue('ts' in output)
-
-    @unittest.skipIf(not has_docker, "Docker container not usable")
-    def testMaxWalltime(self):
-        '''Test server restriction max_walltime'''
-        script = SoS_Script('''
-[10]
-task: walltime='1:00:00'
-print('a')
-''')
-        wf = script.workflow()
-        self.assertRaises(Exception, Base_Executor(wf, config={
-                'config_file': '~/docker.yml',
-                # do not wait for jobs
-                'wait_for_task': True,
-                'default_queue': 'docker_limited',
-                'sig_mode': 'force',
-                }).run)
 
     @unittest.skipIf(not has_docker, "Docker container not usable")
     def testSoSExecute(self):
         '''Test sos execute'''
         subprocess.check_output('sos purge -c ~/docker.yml -q docker', shell=True)
         script = SoS_Script('''
 [10]
@@ -720,15 +597,15 @@
         self.assertTrue(os.path.isfile('llp'))
         os.remove('llp')
 
     @unittest.skipIf(sys.platform == 'win32' or not has_docker, 'appveyor does not have docker with linux')
     def testRemoteTaskFromJupyter(self):
         '''Test the execution of tasks with -q '''
         from ipykernel.tests.utils import execute
-        from sos.jupyter.test_utils import sos_kernel, get_display_data
+        from sos_notebook.test_utils import sos_kernel, get_display_data
         subprocess.call(['sos', 'purge'])
         with sos_kernel() as kc:
             # the cell will actually be executed several times
             # with automatic-reexecution
             code = """
 %run -s force -W -q ts -c ~/docker.yml
 [10]
@@ -753,9 +630,16 @@
             execute(kc=kc, code='%taskinfo -q ts ' + tid)
             res = get_display_data(kc.iopub_channel, 'text/html')
             self.assertTrue(tid in res, 'expect {} in {}'.format(tid, res))
             # there should be two tasks
             lines = subprocess.check_output(['sos', 'status', '-q', 'ts', '-c', '~/docker.yml']).decode().splitlines()
             self.assertGreaterEqual(len(lines), 2)
 
+    def testListHosts(self):
+        '''test list hosts using sos status -q'''
+        for v in ['0', '1', '3', '4']:
+            # ts of type pbs should be in output
+            output = subprocess.check_output(['sos', 'status', '-c', '~/docker.yml', '-q', '-v', v]).decode()
+            self.assertTrue('ts' in output)
+
 if __name__ == '__main__':
     unittest.main()
```

