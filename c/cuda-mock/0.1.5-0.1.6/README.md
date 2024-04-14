# Comparing `tmp/cuda-mock-0.1.5.tar.gz` & `tmp/cuda-mock-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuda-mock-0.1.5.tar", last modified: Fri Mar 29 09:55:03 2024, max compression
+gzip compressed data, was "cuda-mock-0.1.6.tar", last modified: Sun Apr 14 13:47:52 2024, max compression
```

## Comparing `cuda-mock-0.1.5.tar` & `cuda-mock-0.1.6.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 09:55:03.805377 cuda-mock-0.1.5/
--rw-r--r--   0 root         (0) root         (0)     1495 2024-03-29 09:44:17.000000 cuda-mock-0.1.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-29 09:44:17.000000 cuda-mock-0.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3472 2024-03-29 09:55:03.805377 cuda-mock-0.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3164 2024-03-29 09:44:17.000000 cuda-mock-0.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 09:55:03.797376 cuda-mock-0.1.5/include/
--rw-r--r--   0 root         (0) root         (0)     1066 2024-03-29 09:44:17.000000 cuda-mock-0.1.5/include/GlobalVarMgr.h
--rw-r--r--   0 root         (0) root         (0)     3118 2024-03-29 09:44:17.000000 cuda-mock-0.1.5/include/backtrace.h
--rw-r--r--   0 root         (0) root         (0)     1505 2024-03-29 09:44:17.000000 cuda-mock-0.1.5/include/cuda_mock.h
--rw-r--r--   0 root         (0) root         (0)     3205 2024-03-29 09:44:17.000000 cuda-mock-0.1.5/include/env_util.h
--rw-r--r--   0 root         (0) root         (0)    13039 2024-03-29 09:44:17.000000 cuda-mock-0.1.5/include/hook.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 09:55:03.801377 cuda-mock-0.1.5/include/logger/
--rw-r--r--   0 root         (0) root         (0)     1899 2024-03-29 09:44:17.000000 cuda-mock-0.1.5/include/logger/StringRef.h
--rw-r--r--   0 root         (0) root         (0)    16267 2024-03-29 09:44:17.000000 cuda-mock-0.1.5/include/logger/logger.h
--rw-r--r--   0 root         (0) root         (0)      658 2024-03-29 09:44:17.000000 cuda-mock-0.1.5/include/logger/logger_stl.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 09:55:03.801377 cuda-mock-0.1.5/include/profile/
--rw-r--r--   0 root         (0) root         (0)     1603 2024-03-29 09:44:17.000000 cuda-mock-0.1.5/include/profile/Timer.h
--rw-r--r--   0 root         (0) root         (0)    24151 2024-03-29 09:44:17.000000 cuda-mock-0.1.5/include/support.h
--rw-r--r--   0 root         (0) root         (0)      340 2024-03-29 09:44:17.000000 cuda-mock-0.1.5/include/xpu_mock.h
--rw-r--r--   0 root         (0) root         (0)      350 2024-03-29 09:44:17.000000 cuda-mock-0.1.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-29 09:55:03.805377 cuda-mock-0.1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2516 2024-03-29 09:44:17.000000 cuda-mock-0.1.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 09:55:03.793377 cuda-mock-0.1.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 09:55:03.801377 cuda-mock-0.1.5/src/cuda_mock/
--rw-r--r--   0 root         (0) root         (0)      117 2024-03-29 09:44:17.000000 cuda-mock-0.1.5/src/cuda_mock/__init__.py
--rw-r--r--   0 root         (0) root         (0)      216 2024-03-29 09:44:17.000000 cuda-mock-0.1.5/src/cuda_mock/ctypes_helper.py
--rw-r--r--   0 root         (0) root         (0)     8492 2024-03-29 09:44:17.000000 cuda-mock-0.1.5/src/cuda_mock/cuda_mock_impl.py
--rw-r--r--   0 root         (0) root         (0)     2701 2024-03-29 09:44:17.000000 cuda-mock-0.1.5/src/cuda_mock/dynamic_obj.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 09:55:03.805377 cuda-mock-0.1.5/src/cuda_mock.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3472 2024-03-29 09:55:03.000000 cuda-mock-0.1.5/src/cuda_mock.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      592 2024-03-29 09:55:03.000000 cuda-mock-0.1.5/src/cuda_mock.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-29 09:55:03.000000 cuda-mock-0.1.5/src/cuda_mock.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-29 09:44:53.000000 cuda-mock-0.1.5/src/cuda_mock.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-29 09:55:03.000000 cuda-mock-0.1.5/src/cuda_mock.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 13:47:52.925115 cuda-mock-0.1.6/
+-rw-r--r--   0 root         (0) root         (0)     1495 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3472 2024-04-14 13:47:52.925115 cuda-mock-0.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3164 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 13:47:52.917116 cuda-mock-0.1.6/include/
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/include/GlobalVarMgr.h
+-rw-r--r--   0 root         (0) root         (0)     3118 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/include/backtrace.h
+-rw-r--r--   0 root         (0) root         (0)     1505 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/include/cuda_mock.h
+-rw-r--r--   0 root         (0) root         (0)     3205 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/include/env_util.h
+-rw-r--r--   0 root         (0) root         (0)    13039 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/include/hook.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 13:47:52.917116 cuda-mock-0.1.6/include/logger/
+-rw-r--r--   0 root         (0) root         (0)     1899 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/include/logger/StringRef.h
+-rw-r--r--   0 root         (0) root         (0)    16271 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/include/logger/logger.h
+-rw-r--r--   0 root         (0) root         (0)      658 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/include/logger/logger_stl.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 13:47:52.921115 cuda-mock-0.1.6/include/profile/
+-rw-r--r--   0 root         (0) root         (0)     1603 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/include/profile/Timer.h
+-rw-r--r--   0 root         (0) root         (0)    24151 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/include/support.h
+-rw-r--r--   0 root         (0) root         (0)      340 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/include/xpu_mock.h
+-rw-r--r--   0 root         (0) root         (0)      350 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-14 13:47:52.925115 cuda-mock-0.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2516 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 13:47:52.913116 cuda-mock-0.1.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 13:47:52.921115 cuda-mock-0.1.6/src/cuda_mock/
+-rw-r--r--   0 root         (0) root         (0)      147 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/src/cuda_mock/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      216 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/src/cuda_mock/ctypes_helper.py
+-rw-r--r--   0 root         (0) root         (0)     8620 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/src/cuda_mock/cuda_mock_impl.py
+-rw-r--r--   0 root         (0) root         (0)     2701 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/src/cuda_mock/dynamic_obj.py
+-rw-r--r--   0 root         (0) root         (0)    16779 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/src/cuda_mock/gpu_validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 13:47:52.925115 cuda-mock-0.1.6/src/cuda_mock.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3472 2024-04-14 13:47:52.000000 cuda-mock-0.1.6/src/cuda_mock.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      624 2024-04-14 13:47:52.000000 cuda-mock-0.1.6/src/cuda_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-14 13:47:52.000000 cuda-mock-0.1.6/src/cuda_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-14 13:37:51.000000 cuda-mock-0.1.6/src/cuda_mock.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-14 13:47:52.000000 cuda-mock-0.1.6/src/cuda_mock.egg-info/top_level.txt
```

### Comparing `cuda-mock-0.1.5/LICENSE` & `cuda-mock-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.5/PKG-INFO` & `cuda-mock-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuda-mock
-Version: 0.1.5
+Version: 0.1.6
 Summary: mock cuda runtime api
 Home-page: https://github.com/lipracer/torch-cuda-mock
 Author: lipracer
 Author-email: lipracer <lipracer@gmail.com>
 License: BSD-3-Clause
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cuda-mock-0.1.5/README.md` & `cuda-mock-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.5/include/GlobalVarMgr.h` & `cuda-mock-0.1.6/include/GlobalVarMgr.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.5/include/backtrace.h` & `cuda-mock-0.1.6/include/backtrace.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.5/include/cuda_mock.h` & `cuda-mock-0.1.6/include/cuda_mock.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.5/include/env_util.h` & `cuda-mock-0.1.6/include/env_util.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.5/include/hook.h` & `cuda-mock-0.1.6/include/hook.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.5/include/logger/StringRef.h` & `cuda-mock-0.1.6/include/logger/StringRef.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.5/include/logger/logger.h` & `cuda-mock-0.1.6/include/logger/logger.h`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 namespace logger {
 enum class LogLevel { info = 0, warning, error, fatal, last };
 enum class LogModule { profile, trace, hook, python, last };
 
 class LogModuleHelper {
    public:
     static auto& enum_strs() {
-        static std::array<const char*, 5> strs = {"profile", "trace", "hook",
-                                                         "python", "last"};
+        static std::array<const char*, 5> strs = {"PROFILE", "TRACE", "HOOK",
+                                                         "PYTHON", "LAST"};
         return strs;
     }
     static auto begin() { return enum_strs().begin(); }
     static auto end() { return enum_strs().end(); }
 
     template <size_t N>
     static int strToEnum(const char(name)[N]) {
@@ -231,15 +231,15 @@
     const std::string& logHeader() { return logHeader_; }
 
    private:
     LogLevel level_ = LogLevel::warning;
     std::stringstream ss_;
     std::shared_ptr<LogConsumer> logConsumer_;
     std::shared_ptr<LogConfig> cfg_;
-    LogLevel module_set_[static_cast<size_t>(LogModule::last)] = {
+    LogLevel module_set_[static_cast<size_t>(LogModule::last) + 1] = {
         LogLevel::info};
     std::chrono::steady_clock::time_point start_point_{
         std::chrono::steady_clock::now()};
     std::string logHeader_;
 };
 
 inline bool LOG_CONDITATION(LogLevel level) {
```

### Comparing `cuda-mock-0.1.5/include/logger/logger_stl.h` & `cuda-mock-0.1.6/include/logger/logger_stl.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.5/include/profile/Timer.h` & `cuda-mock-0.1.6/include/profile/Timer.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.5/include/support.h` & `cuda-mock-0.1.6/include/support.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.5/setup.py` & `cuda-mock-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
         subprocess.check_call(['cmake', f'{script_dir}'] + cmake_args + ninja_args, cwd=build_dir)
         subprocess.check_call(['cmake', '--build', '.'], cwd=build_dir)
         subprocess.check_call([f'{install_cmd}', 'install'], cwd=build_dir)
 
 setup(
     name="cuda-mock",
-    version="0.1.5",
+    version="0.1.6",
     author="lipracer",
     author_email="lipracer@gmail.com",
     description="a tools hook some api call at runtime",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
 
     url="https://github.com/lipracer/torch-cuda-mock",
```

### Comparing `cuda-mock-0.1.5/src/cuda_mock/cuda_mock_impl.py` & `cuda-mock-0.1.6/src/cuda_mock/cuda_mock_impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,25 +37,28 @@
     target_symbols = convert_arg_list_of_str(target_symbols)
     cuda_mock_impl.print_hook_initialize(target_libs, target_symbols)
     
 
 def patch_runtime():
     return cuda_mock_impl.patch_runtime()
 
-def log(*args):
+def log(*args, level=0):
     caller_frame = inspect.currentframe().f_back
     caller_filename = inspect.getframeinfo(caller_frame).filename
     caller_lineno = inspect.getframeinfo(caller_frame).lineno
-    for arg in args:
-        assert isinstance(arg, str), f"expect str type but got {type(arg)}"
     new_args = [f'[{caller_filename}:{caller_lineno}]{arg}' for arg in args]
     new_args = [ctypes.c_char_p(arg.encode('utf-8')) for arg in new_args]
-    return cuda_mock_impl.py_log(*new_args)
+    if level == 0:
+        return cuda_mock_impl.py_log_info(*new_args)
+    elif level == 1:
+        return cuda_mock_impl.py_log_warn(*new_args)
+    else:
+        return cuda_mock_impl.py_log_error(*new_args)
 
-cuda_version = os.environ.get('CUDA_VERSION', None)
+is_nvidia_gpu = os.environ.get('CUDA_VERSION', None) or os.environ.get('NVIDIA_VISIBLE_DEVICES', None)
 
 class ProfileDataCollection:
     def __init__(self, device):
         self.data = []
         self.device = device
     def append_gpu(self, key, data):
         self.load_from_cache()
@@ -93,15 +96,15 @@
         elif time_str.endswith("s"):
             return float(time_str.replace("s", "")) * 1000 * 1000 * 1000
         raise RuntimeError(f"error uint:{time_str}")
 
     def statistic_data(self, data, device):
         total = 0.0
         for it in data:
-            if cuda_version:
+            if is_nvidia_gpu:
                 total += self.get_gpu_time(it)
             else:
                 total += self.get_xpu_time(it)
         data = {"total" : total, "data" : data}
         return data
 
     def load_from_cache(self):
@@ -112,15 +115,15 @@
         # except Exception:
         #     pass
 
     def dump_to_cache(self):
         with open(f"{self.device}-profile_data.json", "wt") as f:
             json.dump(self.data, f, indent=4)
 
-gProfileDataCollection = ProfileDataCollection("gpu" if cuda_version else "xpu")
+gProfileDataCollection = ProfileDataCollection("gpu" if is_nvidia_gpu else "xpu")
 gDefaultTargetLib = ["libxpucuda.so", "libcuda.so"]
 gDefaultTargetSymbols = ["__printf_chk", "printf","fprintf","__fprintf","vfprintf",]
 class __XpuRuntimeProfiler:
     def __init__(self, target_libs = gDefaultTargetLib, target_symbols = gDefaultTargetSymbols):
         print_hook_initialize(target_libs=target_libs, target_symbols=target_symbols)
     def start_capture(self):
         cuda_mock_impl.print_hook_start_capture()
@@ -169,15 +172,15 @@
             data.append(('total', matches[0]))
         else:
             data.append(('total', "0.0ms"))
         self.data = data
         gProfileDataCollection.append_gpu(op_key, self.data)
         log(f"{op_key}:{self.data}")
 
-RuntimeProfiler = __XpuRuntimeProfiler if not cuda_version else __GpuRuntimeProfiler
+RuntimeProfiler = __GpuRuntimeProfiler if is_nvidia_gpu else __XpuRuntimeProfiler
 
 
 class HookInstaller:
     def __init__(self, lib):
         self.lib = ctypes.CDLL(lib)
         c_python_object = ctypes.py_object(self)
         c_string_lib = ctypes.c_char_p(lib.encode('utf-8'))
```

### Comparing `cuda-mock-0.1.5/src/cuda_mock/dynamic_obj.py` & `cuda-mock-0.1.6/src/cuda_mock/dynamic_obj.py`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.5/src/cuda_mock.egg-info/PKG-INFO` & `cuda-mock-0.1.6/src/cuda_mock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuda-mock
-Version: 0.1.5
+Version: 0.1.6
 Summary: mock cuda runtime api
 Home-page: https://github.com/lipracer/torch-cuda-mock
 Author: lipracer
 Author-email: lipracer <lipracer@gmail.com>
 License: BSD-3-Clause
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cuda-mock-0.1.5/src/cuda_mock.egg-info/SOURCES.txt` & `cuda-mock-0.1.6/src/cuda_mock.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -14,12 +14,13 @@
 include/logger/logger.h
 include/logger/logger_stl.h
 include/profile/Timer.h
 src/cuda_mock/__init__.py
 src/cuda_mock/ctypes_helper.py
 src/cuda_mock/cuda_mock_impl.py
 src/cuda_mock/dynamic_obj.py
+src/cuda_mock/gpu_validation.py
 src/cuda_mock.egg-info/PKG-INFO
 src/cuda_mock.egg-info/SOURCES.txt
 src/cuda_mock.egg-info/dependency_links.txt
 src/cuda_mock.egg-info/not-zip-safe
 src/cuda_mock.egg-info/top_level.txt
```

