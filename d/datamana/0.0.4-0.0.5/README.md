# Comparing `tmp/datamana-0.0.4.tar.gz` & `tmp/datamana-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamana-0.0.4.tar", last modified: Sun Apr 14 09:23:27 2024, max compression
+gzip compressed data, was "datamana-0.0.5.tar", last modified: Sun Apr 14 11:07:29 2024, max compression
```

## Comparing `datamana-0.0.4.tar` & `datamana-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:23:27.972068 datamana-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-14 09:23:17.000000 datamana-0.0.4/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-14 09:23:17.000000 datamana-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-14 09:23:27.968068 datamana-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 09:23:17.000000 datamana-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:23:27.968068 datamana-0.0.4/csrc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 09:23:17.000000 datamana-0.0.4/csrc/mqueue.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-14 09:23:17.000000 datamana-0.0.4/csrc/semaphore.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:23:27.968068 datamana-0.0.4/datamana/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 09:23:17.000000 datamana-0.0.4/datamana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 09:23:17.000000 datamana-0.0.4/datamana/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-14 09:23:17.000000 datamana-0.0.4/datamana/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:23:27.968068 datamana-0.0.4/datamana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-14 09:23:27.000000 datamana-0.0.4/datamana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-14 09:23:27.000000 datamana-0.0.4/datamana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 09:23:27.000000 datamana-0.0.4/datamana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 09:23:27.000000 datamana-0.0.4/datamana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 09:23:27.000000 datamana-0.0.4/datamana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-14 09:23:17.000000 datamana-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 09:23:27.972068 datamana-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-14 09:23:17.000000 datamana-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:07:29.208389 datamana-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-14 11:07:19.000000 datamana-0.0.5/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-14 11:07:19.000000 datamana-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-14 11:07:29.204389 datamana-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 11:07:19.000000 datamana-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:07:29.204389 datamana-0.0.5/csrc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-14 11:07:19.000000 datamana-0.0.5/csrc/mqueue.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-14 11:07:19.000000 datamana-0.0.5/csrc/python.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-14 11:07:19.000000 datamana-0.0.5/csrc/semaphore.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:07:29.204389 datamana-0.0.5/datamana/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 11:07:19.000000 datamana-0.0.5/datamana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 11:07:19.000000 datamana-0.0.5/datamana/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-14 11:07:19.000000 datamana-0.0.5/datamana/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:07:29.204389 datamana-0.0.5/datamana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-14 11:07:29.000000 datamana-0.0.5/datamana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-14 11:07:29.000000 datamana-0.0.5/datamana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 11:07:29.000000 datamana-0.0.5/datamana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 11:07:29.000000 datamana-0.0.5/datamana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 11:07:29.000000 datamana-0.0.5/datamana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-14 11:07:19.000000 datamana-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 11:07:29.208389 datamana-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-14 11:07:19.000000 datamana-0.0.5/setup.py
```

### Comparing `datamana-0.0.4/CMakeLists.txt` & `datamana-0.0.5/CMakeLists.txt`

 * *Files 22% similar despite different names*

```diff
@@ -11,8 +11,12 @@
 
 execute_process(
   COMMAND "${Python_EXECUTABLE}" -m nanobind --cmake_dir
   OUTPUT_STRIP_TRAILING_WHITESPACE OUTPUT_VARIABLE NB_DIR)
 list(APPEND CMAKE_PREFIX_PATH "${NB_DIR}")
 find_package(nanobind CONFIG REQUIRED)
 
-nanobind_add_module(core STABLE_ABI csrc/semaphore.cpp csrc/mqueue.cpp)
+nanobind_add_module(
+  core STABLE_ABI
+  csrc/semaphore.hpp csrc/mqueue.hpp
+  csrc/python.cpp
+)
```

### Comparing `datamana-0.0.4/LICENSE` & `datamana-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `datamana-0.0.4/PKG-INFO` & `datamana-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamana
-Version: 0.0.4
+Version: 0.0.5
 Summary: Dataset Manager
 Author-email: Jiau Zhang <jiauzhang@163.com>
 Project-URL: Homepage, https://github.com/jiauzhang/datamana
 Keywords: Deep Learning,Dataset Manager,Artificial Intelligence
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datamana-0.0.4/csrc/semaphore.cpp` & `datamana-0.0.5/csrc/mqueue.hpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,43 @@
 #include <fcntl.h>           /* For O_* constants */
 #include <sys/stat.h>        /* For mode constants */
-#include <semaphore.h>
+#include <mqueue.h>
 #include <nanobind/nanobind.h>
 #include <nanobind/stl/string.h>
 
 namespace nb = nanobind;
 
-struct Semaphore {
-    sem_t *sem;
+struct MQueue {
+    mqd_t mqd;
+    const int o_rdonly = O_RDONLY;
+    const int o_wronly = O_WRONLY;
+    const int o_rdwr = O_RDWR;
     const int o_creat = O_CREAT;
     const int o_excl = O_EXCL;
-    const int o_trunc = O_TRUNC;
+    const int o_nonblock = O_NONBLOCK;
 
-    Semaphore() : sem((sem_t *)0) {}
+    MQueue() : mqd((mqd_t)-1) {}
 
-    int py_sem_open(const char *name, int oflag, unsigned int mode, unsigned int value) {
-        sem = sem_open(name, oflag, (mode_t)mode, value);
-        if (sem == (sem_t *)SEM_FAILED) {
-            sem = 0;
+    int py_mq_open(const char *name, int oflag, unsigned int mode, struct mq_attr *attr) {
+        mqd = mq_open(name, oflag, (mode_t)mode, attr);
+        if (mqd == (mqd_t)-1) {
             return -1;
         } else {
             return 0;
         }
     }
-    int py_sem_unlink(const char *name) {
-        return sem_unlink(name);
+    int py_mq_unlink(const char *name) {
+        return mq_unlink(name);
     }
-    int py_sem_close() {
-        return sem_close(sem);
+    int py_mq_close() {
+        return mq_close(mqd);
     }
-    int py_sem_post() {
-        return sem_post(sem);
+    int py_mq_send(std::string &msg, unsigned int msg_prio) {
+        return mq_send(mqd, (const char *)msg.c_str(), msg.size(), msg_prio);
     }
-    int py_sem_wait() {
-        return sem_wait(sem);
+    std::string py_mq_receive() {
+        unsigned int msg_prio;
+        std::string msg(32, '\0');
+        mq_receive(mqd, (char *)msg.c_str(), msg.size(), &msg_prio);
+        return msg;
     }
 };
-
-NB_MODULE(core, m) {
-    nb::class_<Semaphore>(m, "Semaphore")
-        .def(nb::init<>())
-        .def("open", &Semaphore::py_sem_open)
-        .def("close", &Semaphore::py_sem_close)
-        .def("unlink", &Semaphore::py_sem_unlink)
-        .def("wait", &Semaphore::py_sem_wait)
-        .def("post", &Semaphore::py_sem_post)
-        .def_prop_ro("O_CREAT", [](Semaphore &sem) { return sem.o_creat; })
-        .def_prop_ro("O_EXCL", [](Semaphore &sem) { return sem.o_excl; })
-        .def_prop_ro("O_TRUNC", [](Semaphore &sem) { return sem.o_trunc; });
-}
```

### Comparing `datamana-0.0.4/datamana/torch.py` & `datamana-0.0.5/datamana/torch.py`

 * *Files identical despite different names*

### Comparing `datamana-0.0.4/datamana.egg-info/PKG-INFO` & `datamana-0.0.5/datamana.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamana
-Version: 0.0.4
+Version: 0.0.5
 Summary: Dataset Manager
 Author-email: Jiau Zhang <jiauzhang@163.com>
 Project-URL: Homepage, https://github.com/jiauzhang/datamana
 Keywords: Deep Learning,Dataset Manager,Artificial Intelligence
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datamana-0.0.4/pyproject.toml` & `datamana-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "cmake >= 3.15",
     "nanobind >= 1.9.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datamana"
-version = "0.0.4"
+version = "0.0.5"
 description = "Dataset Manager"
 readme = "README.md"
 authors = [
     {name = "Jiau Zhang", email = "jiauzhang@163.com"},
 ]
 classifiers = [
     'Intended Audience :: Developers',
```

### Comparing `datamana-0.0.4/setup.py` & `datamana-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,11 +116,11 @@
         subprocess.run(
             ["cmake", "--build", ".", *build_args], cwd=build_temp, check=True
         )
 
 setup(
     ext_modules=[CMakeExtension("datamana.core", sourcedir=".", sources=[
         'CMakeLists.txt',
-        'csrc/semaphore.cpp', 'csrc/mqueue.cpp',
+        'csrc/semaphore.hpp', 'csrc/mqueue.hpp', 'csrc/python.cpp',
     ])],
     cmdclass={"build_ext": CMakeBuild},
 )
```

