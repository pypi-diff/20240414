# Comparing `tmp/botasaurus2-1.2.1.tar.gz` & `tmp/botasaurus2-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botasaurus2-1.2.1.tar", max compression
+gzip compressed data, was "botasaurus2-1.3.0.tar", max compression
```

## Comparing `botasaurus2-1.2.1.tar` & `botasaurus2-1.3.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      217 2024-03-15 22:38:58.098040 botasaurus2-1.2.1/AUTHORS
--rw-r--r--   0        0        0     1073 2024-03-15 22:38:58.098040 botasaurus2-1.2.1/LICENSE
--rw-r--r--   0        0        0    50976 2024-03-19 13:44:59.662333 botasaurus2-1.2.1/README.md
--rw-r--r--   0        0        0      799 2024-03-19 20:47:06.016789 botasaurus2-1.2.1/botasaurus/__init__.py
--rw-r--r--   0        0        0      211 2024-03-15 22:38:58.098040 botasaurus2-1.2.1/botasaurus/_id.py
--rw-r--r--   0        0        0     1034 2024-03-15 22:38:58.098040 botasaurus2-1.2.1/botasaurus/accept_google_cookies.py
--rw-r--r--   0        0        0    57045 2024-03-20 15:48:31.569396 botasaurus2-1.2.1/botasaurus/anti_detect_driver.py
--rw-r--r--   0        0        0     4485 2024-04-11 15:00:22.756112 botasaurus2-1.2.1/botasaurus/anti_detect_requests.py
--rw-r--r--   0        0        0     3549 2024-03-15 22:38:58.098040 botasaurus2-1.2.1/botasaurus/base_data.py
--rw-r--r--   0        0        0      800 2024-03-15 22:38:58.098040 botasaurus2-1.2.1/botasaurus/beep_utils.py
--rw-r--r--   0        0        0     2868 2024-04-12 14:30:05.866696 botasaurus2-1.2.1/botasaurus/botasaurus_storage.py
--rw-r--r--   0        0        0      944 2024-04-11 21:17:56.332972 botasaurus2-1.2.1/botasaurus/bt.py
--rw-r--r--   0        0        0     7486 2024-03-15 22:38:58.098040 botasaurus2-1.2.1/botasaurus/cache.py
--rw-r--r--   0        0        0     2114 2024-03-15 22:38:58.098040 botasaurus2-1.2.1/botasaurus/calc_max_parallel_browsers.py
--rw-r--r--   0        0        0    28154 2024-04-11 15:00:22.756112 botasaurus2-1.2.1/botasaurus/captcha.py
--rw-r--r--   0        0        0      566 2024-03-15 22:38:58.098040 botasaurus2-1.2.1/botasaurus/check_and_download_driver.py
--rw-r--r--   0        0        0      362 2024-03-15 22:38:58.098040 botasaurus2-1.2.1/botasaurus/chrome_launcher_adapter.py
--rw-r--r--   0        0        0    14871 2024-03-15 22:38:58.098040 botasaurus2-1.2.1/botasaurus/cl.py
--rw-r--r--   0        0        0      946 2024-03-15 22:38:58.098040 botasaurus2-1.2.1/botasaurus/close.py
--rw-r--r--   0        0        0      256 2024-03-20 15:48:31.573396 botasaurus2-1.2.1/botasaurus/constants.py
--rw-r--r--   0        0        0    15195 2024-04-11 15:00:22.756112 botasaurus2-1.2.1/botasaurus/create_driver_utils.py
--rw-r--r--   0        0        0    12338 2024-04-11 15:00:22.756112 botasaurus2-1.2.1/botasaurus/create_stealth_driver.py
--rw-r--r--   0        0        0     1820 2024-03-15 22:38:58.102041 botasaurus2-1.2.1/botasaurus/creators.py
--rw-r--r--   0        0        0     4130 2024-03-15 22:38:58.102041 botasaurus2-1.2.1/botasaurus/decorator_helpers.py
--rw-r--r--   0        0        0    38953 2024-04-12 18:09:18.926557 botasaurus2-1.2.1/botasaurus/decorators.py
--rw-r--r--   0        0        0      491 2024-03-15 22:38:58.102041 botasaurus2-1.2.1/botasaurus/decorators_utils.py
--rw-r--r--   0        0        0     1617 2024-03-15 22:38:58.102041 botasaurus2-1.2.1/botasaurus/download_driver.py
--rw-r--r--   0        0        0      459 2024-03-15 22:38:58.102041 botasaurus2-1.2.1/botasaurus/driver_about.py
--rw-r--r--   0        0        0       48 2024-03-15 22:38:58.102041 botasaurus2-1.2.1/botasaurus/exceptions.py
--rw-r--r--   0        0        0       84 2024-03-15 22:38:58.102041 botasaurus2-1.2.1/botasaurus/formats.py
--rw-r--r--   0        0        0    14839 2024-03-15 22:38:58.102041 botasaurus2-1.2.1/botasaurus/get_chrome_version.py
--rw-r--r--   0        0        0     8679 2024-04-11 15:00:22.756112 botasaurus2-1.2.1/botasaurus/got_adapter.py
--rw-r--r--   0        0        0     2438 2024-04-12 14:30:10.786777 botasaurus2-1.2.1/botasaurus/ip_utils.py
--rw-r--r--   0        0        0     1534 2024-03-15 22:38:58.102041 botasaurus2-1.2.1/botasaurus/list_utils.py
--rw-r--r--   0        0        0     3326 2024-04-11 20:48:02.911490 botasaurus2-1.2.1/botasaurus/local_storage.py
--rw-r--r--   0        0        0     1674 2024-03-15 22:38:58.102041 botasaurus2-1.2.1/botasaurus/local_storage_driver.py
--rw-r--r--   0        0        0       77 2024-03-15 22:38:58.102041 botasaurus2-1.2.1/botasaurus/opponent.py
--rw-r--r--   0        0        0     7343 2024-03-19 13:44:59.666333 botasaurus2-1.2.1/botasaurus/output.py
--rw-r--r--   0        0        0     4964 2024-04-12 14:01:33.922678 botasaurus2-1.2.1/botasaurus/profile.py
--rw-r--r--   0        0        0      352 2024-03-19 19:06:20.087339 botasaurus2-1.2.1/botasaurus/shortcuts.py
--rw-r--r--   0        0        0    22453 2024-03-15 22:38:58.102041 botasaurus2-1.2.1/botasaurus/sitemap.py
--rw-r--r--   0        0        0     2031 2024-03-19 13:44:59.666333 botasaurus2-1.2.1/botasaurus/str_utils.py
--rw-r--r--   0        0        0     6298 2024-03-15 22:38:58.102041 botasaurus2-1.2.1/botasaurus/temp_mail.py
--rw-r--r--   0        0        0       54 2024-03-15 22:38:58.102041 botasaurus2-1.2.1/botasaurus/usage.py
--rw-r--r--   0        0        0     7457 2024-03-15 22:38:58.102041 botasaurus2-1.2.1/botasaurus/user_agent.py
--rw-r--r--   0        0        0     4194 2024-03-15 22:38:58.102041 botasaurus2-1.2.1/botasaurus/user_generator.py
--rw-r--r--   0        0        0     8520 2024-03-19 20:47:06.020789 botasaurus2-1.2.1/botasaurus/utils.py
--rw-r--r--   0        0        0       57 2024-03-15 22:38:58.102041 botasaurus2-1.2.1/botasaurus/wait.py
--rw-r--r--   0        0        0     1183 2024-03-15 22:38:58.102041 botasaurus2-1.2.1/botasaurus/window_size.py
--rw-r--r--   0        0        0      848 2024-04-12 18:09:27.642533 botasaurus2-1.2.1/pyproject.toml
--rw-r--r--   0        0        0    52119 1970-01-01 00:00:00.000000 botasaurus2-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0      217 2024-03-15 22:38:58.098040 botasaurus2-1.3.0/AUTHORS
+-rw-r--r--   0        0        0     1073 2024-03-15 22:38:58.098040 botasaurus2-1.3.0/LICENSE
+-rw-r--r--   0        0        0    50976 2024-03-19 13:44:59.662333 botasaurus2-1.3.0/README.md
+-rw-r--r--   0        0        0      799 2024-03-19 20:47:06.016789 botasaurus2-1.3.0/botasaurus/__init__.py
+-rw-r--r--   0        0        0      211 2024-03-15 22:38:58.098040 botasaurus2-1.3.0/botasaurus/_id.py
+-rw-r--r--   0        0        0     1034 2024-03-15 22:38:58.098040 botasaurus2-1.3.0/botasaurus/accept_google_cookies.py
+-rw-r--r--   0        0        0    57045 2024-03-20 15:48:31.569396 botasaurus2-1.3.0/botasaurus/anti_detect_driver.py
+-rw-r--r--   0        0        0     4485 2024-04-11 15:00:22.756112 botasaurus2-1.3.0/botasaurus/anti_detect_requests.py
+-rw-r--r--   0        0        0     3549 2024-03-15 22:38:58.098040 botasaurus2-1.3.0/botasaurus/base_data.py
+-rw-r--r--   0        0        0      800 2024-03-15 22:38:58.098040 botasaurus2-1.3.0/botasaurus/beep_utils.py
+-rw-r--r--   0        0        0     2868 2024-04-12 14:30:05.866696 botasaurus2-1.3.0/botasaurus/botasaurus_storage.py
+-rw-r--r--   0        0        0      944 2024-04-11 21:17:56.332972 botasaurus2-1.3.0/botasaurus/bt.py
+-rw-r--r--   0        0        0     7486 2024-03-15 22:38:58.098040 botasaurus2-1.3.0/botasaurus/cache.py
+-rw-r--r--   0        0        0     2114 2024-03-15 22:38:58.098040 botasaurus2-1.3.0/botasaurus/calc_max_parallel_browsers.py
+-rw-r--r--   0        0        0    28154 2024-04-11 15:00:22.756112 botasaurus2-1.3.0/botasaurus/captcha.py
+-rw-r--r--   0        0        0      566 2024-03-15 22:38:58.098040 botasaurus2-1.3.0/botasaurus/check_and_download_driver.py
+-rw-r--r--   0        0        0      362 2024-03-15 22:38:58.098040 botasaurus2-1.3.0/botasaurus/chrome_launcher_adapter.py
+-rw-r--r--   0        0        0    14871 2024-03-15 22:38:58.098040 botasaurus2-1.3.0/botasaurus/cl.py
+-rw-r--r--   0        0        0      946 2024-03-15 22:38:58.098040 botasaurus2-1.3.0/botasaurus/close.py
+-rw-r--r--   0        0        0      256 2024-03-20 15:48:31.573396 botasaurus2-1.3.0/botasaurus/constants.py
+-rw-r--r--   0        0        0    15195 2024-04-11 15:00:22.756112 botasaurus2-1.3.0/botasaurus/create_driver_utils.py
+-rw-r--r--   0        0        0    12338 2024-04-11 15:00:22.756112 botasaurus2-1.3.0/botasaurus/create_stealth_driver.py
+-rw-r--r--   0        0        0     1820 2024-03-15 22:38:58.102041 botasaurus2-1.3.0/botasaurus/creators.py
+-rw-r--r--   0        0        0     4130 2024-03-15 22:38:58.102041 botasaurus2-1.3.0/botasaurus/decorator_helpers.py
+-rw-r--r--   0        0        0    39088 2024-04-14 10:41:23.389902 botasaurus2-1.3.0/botasaurus/decorators.py
+-rw-r--r--   0        0        0      491 2024-03-15 22:38:58.102041 botasaurus2-1.3.0/botasaurus/decorators_utils.py
+-rw-r--r--   0        0        0     1617 2024-03-15 22:38:58.102041 botasaurus2-1.3.0/botasaurus/download_driver.py
+-rw-r--r--   0        0        0      459 2024-03-15 22:38:58.102041 botasaurus2-1.3.0/botasaurus/driver_about.py
+-rw-r--r--   0        0        0       48 2024-03-15 22:38:58.102041 botasaurus2-1.3.0/botasaurus/exceptions.py
+-rw-r--r--   0        0        0       84 2024-03-15 22:38:58.102041 botasaurus2-1.3.0/botasaurus/formats.py
+-rw-r--r--   0        0        0    14839 2024-03-15 22:38:58.102041 botasaurus2-1.3.0/botasaurus/get_chrome_version.py
+-rw-r--r--   0        0        0     8679 2024-04-11 15:00:22.756112 botasaurus2-1.3.0/botasaurus/got_adapter.py
+-rw-r--r--   0        0        0     2438 2024-04-12 14:30:10.786777 botasaurus2-1.3.0/botasaurus/ip_utils.py
+-rw-r--r--   0        0        0     1534 2024-03-15 22:38:58.102041 botasaurus2-1.3.0/botasaurus/list_utils.py
+-rw-r--r--   0        0        0     3326 2024-04-11 20:48:02.911490 botasaurus2-1.3.0/botasaurus/local_storage.py
+-rw-r--r--   0        0        0     1674 2024-03-15 22:38:58.102041 botasaurus2-1.3.0/botasaurus/local_storage_driver.py
+-rw-r--r--   0        0        0       77 2024-03-15 22:38:58.102041 botasaurus2-1.3.0/botasaurus/opponent.py
+-rw-r--r--   0        0        0     7343 2024-03-19 13:44:59.666333 botasaurus2-1.3.0/botasaurus/output.py
+-rw-r--r--   0        0        0     4964 2024-04-12 14:01:33.922678 botasaurus2-1.3.0/botasaurus/profile.py
+-rw-r--r--   0        0        0      352 2024-03-19 19:06:20.087339 botasaurus2-1.3.0/botasaurus/shortcuts.py
+-rw-r--r--   0        0        0    22453 2024-03-15 22:38:58.102041 botasaurus2-1.3.0/botasaurus/sitemap.py
+-rw-r--r--   0        0        0     2031 2024-03-19 13:44:59.666333 botasaurus2-1.3.0/botasaurus/str_utils.py
+-rw-r--r--   0        0        0     6298 2024-03-15 22:38:58.102041 botasaurus2-1.3.0/botasaurus/temp_mail.py
+-rw-r--r--   0        0        0       54 2024-03-15 22:38:58.102041 botasaurus2-1.3.0/botasaurus/usage.py
+-rw-r--r--   0        0        0     7457 2024-03-15 22:38:58.102041 botasaurus2-1.3.0/botasaurus/user_agent.py
+-rw-r--r--   0        0        0     4194 2024-03-15 22:38:58.102041 botasaurus2-1.3.0/botasaurus/user_generator.py
+-rw-r--r--   0        0        0     8520 2024-03-19 20:47:06.020789 botasaurus2-1.3.0/botasaurus/utils.py
+-rw-r--r--   0        0        0       57 2024-03-15 22:38:58.102041 botasaurus2-1.3.0/botasaurus/wait.py
+-rw-r--r--   0        0        0     1183 2024-03-15 22:38:58.102041 botasaurus2-1.3.0/botasaurus/window_size.py
+-rw-r--r--   0        0        0      848 2024-04-14 10:41:23.389902 botasaurus2-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    52119 1970-01-01 00:00:00.000000 botasaurus2-1.3.0/PKG-INFO
```

### Comparing `botasaurus2-1.2.1/LICENSE` & `botasaurus2-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/README.md` & `botasaurus2-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/__init__.py` & `botasaurus2-1.3.0/botasaurus/__init__.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/accept_google_cookies.py` & `botasaurus2-1.3.0/botasaurus/accept_google_cookies.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/anti_detect_driver.py` & `botasaurus2-1.3.0/botasaurus/anti_detect_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/anti_detect_requests.py` & `botasaurus2-1.3.0/botasaurus/anti_detect_requests.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/base_data.py` & `botasaurus2-1.3.0/botasaurus/base_data.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/beep_utils.py` & `botasaurus2-1.3.0/botasaurus/beep_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/botasaurus_storage.py` & `botasaurus2-1.3.0/botasaurus/botasaurus_storage.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/bt.py` & `botasaurus2-1.3.0/botasaurus/bt.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/cache.py` & `botasaurus2-1.3.0/botasaurus/cache.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/calc_max_parallel_browsers.py` & `botasaurus2-1.3.0/botasaurus/calc_max_parallel_browsers.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/captcha.py` & `botasaurus2-1.3.0/botasaurus/captcha.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/check_and_download_driver.py` & `botasaurus2-1.3.0/botasaurus/check_and_download_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/cl.py` & `botasaurus2-1.3.0/botasaurus/cl.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/close.py` & `botasaurus2-1.3.0/botasaurus/close.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/create_driver_utils.py` & `botasaurus2-1.3.0/botasaurus/create_driver_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/create_stealth_driver.py` & `botasaurus2-1.3.0/botasaurus/create_stealth_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/creators.py` & `botasaurus2-1.3.0/botasaurus/creators.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/decorator_helpers.py` & `botasaurus2-1.3.0/botasaurus/decorator_helpers.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/decorators.py` & `botasaurus2-1.3.0/botasaurus/decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -338,15 +338,16 @@
     output_formats: Optional[List[str]] = None,
     raise_exception: bool = False,
     must_raise_exceptions: Optional[List[Any]] = None,
     max_retry: Optional[int] = None,
     retry_wait: Optional[int] = None,
     create_error_logs: bool = True,
     create_driver: Optional[Callable] = None,
-    local_storage_dir: Union[str, Path] = None
+    local_storage_dir: Union[str, Path] = None,
+    remote: bool = False
 ) -> Callable:
     def decorator_browser(func: Callable) -> Callable:
         if not hasattr(func, '_scraper_type'):
             func._scraper_type = "browser"
 
         def close_driver(driver: AntiDetectDriver):
             if tiny_profile:
@@ -397,15 +398,15 @@
 
             nonlocal parallel, data, cache, block_resources, block_images, window_size, metadata, add_arguments, extensions
             nonlocal tiny_profile, is_eager, lang, headless, beep
             nonlocal close_on_crash, async_queue, run_async, profile
             nonlocal proxy, user_agent, reuse_driver, keep_drivers_alive, raise_exception, must_raise_exceptions
 
             nonlocal output, output_formats, max_retry, retry_wait, create_driver, create_error_logs
-            nonlocal capabilities, local_storage_dir
+            nonlocal capabilities, local_storage_dir, remote
 
             parallel = kwargs.get("parallel", parallel)
             data = kwargs.get("data", data)
             cache = kwargs.get("cache", cache)
             block_images = kwargs.get("block_images", block_images)
             block_resources = kwargs.get("block_resources", block_resources)
             add_arguments = kwargs.get("add_arguments", add_arguments)
@@ -432,15 +433,16 @@
             retry_wait = kwargs.get("retry_wait", retry_wait)
             create_error_logs = kwargs.get("create_error_logs", create_error_logs)
 
             raise_exception = kwargs.get("raise_exception", raise_exception)
             create_driver = kwargs.get("create_driver", create_driver)
             capabilities = kwargs.get("capabilities", capabilities)
             local_storage_dir = kwargs.get("local_storage_dir", local_storage_dir)
-
+            remote = kwargs.get("remote", remote)
+            
             local_storage = LocalStorageClass(local_storage_dir)
             profile = ProfileClass(local_storage_dir)
             Profile = profile  # TODO: alter thourghout this module
             fn_name = func.__name__
 
             if cache:
                 _create_cache_directory_if_not_exists(func)
@@ -469,15 +471,16 @@
                     evaluated_profile = str(evaluated_profile)
 
                 if retry_driver is not None:
                     driver = retry_driver
                 elif reuse_driver and len(_driver_pool) > 0:
                     driver = _driver_pool.pop()
                 else:
-                    check_and_download_driver()
+                    if not remote:
+                        check_and_download_driver()
 
                     (
                         options,
                         driver_attributes,
                         close_proxy,
                     ) = create_options_and_driver_attributes_and_close_proxy(
                         tiny_profile,
```

### Comparing `botasaurus2-1.2.1/botasaurus/download_driver.py` & `botasaurus2-1.3.0/botasaurus/download_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/get_chrome_version.py` & `botasaurus2-1.3.0/botasaurus/get_chrome_version.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/got_adapter.py` & `botasaurus2-1.3.0/botasaurus/got_adapter.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/ip_utils.py` & `botasaurus2-1.3.0/botasaurus/ip_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/list_utils.py` & `botasaurus2-1.3.0/botasaurus/list_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/local_storage.py` & `botasaurus2-1.3.0/botasaurus/local_storage.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/local_storage_driver.py` & `botasaurus2-1.3.0/botasaurus/local_storage_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/output.py` & `botasaurus2-1.3.0/botasaurus/output.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/profile.py` & `botasaurus2-1.3.0/botasaurus/profile.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/sitemap.py` & `botasaurus2-1.3.0/botasaurus/sitemap.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/str_utils.py` & `botasaurus2-1.3.0/botasaurus/str_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/temp_mail.py` & `botasaurus2-1.3.0/botasaurus/temp_mail.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/user_agent.py` & `botasaurus2-1.3.0/botasaurus/user_agent.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/user_generator.py` & `botasaurus2-1.3.0/botasaurus/user_generator.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/utils.py` & `botasaurus2-1.3.0/botasaurus/utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/botasaurus/window_size.py` & `botasaurus2-1.3.0/botasaurus/window_size.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.2.1/pyproject.toml` & `botasaurus2-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "botasaurus2"
-version = "1.2.1"
+version = "1.3.0"
 description = "Patching fork of botasaurus, The All in One Framework to build Awesome Scrapers."
 authors = ["Chetan Jain <chetan@omkar.cloud>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "botasaurus", from = "."}]
 
 [tool.poetry.dependencies]
```

### Comparing `botasaurus2-1.2.1/PKG-INFO` & `botasaurus2-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botasaurus2
-Version: 1.2.1
+Version: 1.3.0
 Summary: Patching fork of botasaurus, The All in One Framework to build Awesome Scrapers.
 License: MIT
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: botasaurus2 Version: 1.2.1 Summary: Patching fork
+Metadata-Version: 2.1 Name: botasaurus2 Version: 1.3.0 Summary: Patching fork
 of botasaurus, The All in One Framework to build Awesome Scrapers. License: MIT
 Author: Chetan Jain Author-email: chetan@omkar.cloud Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: aigents (>=0.5.0,<0.6.0)
 Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0) Requires-Dist: botasaurus-
```

