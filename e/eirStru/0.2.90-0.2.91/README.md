# Comparing `tmp/eirStru-0.2.90.tar.gz` & `tmp/eirStru-0.2.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eirStru-0.2.90.tar", last modified: Fri Mar 29 03:39:44 2024, max compression
+gzip compressed data, was "eirStru-0.2.91.tar", last modified: Sun Apr 14 20:06:53 2024, max compression
```

## Comparing `eirStru-0.2.90.tar` & `eirStru-0.2.91.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-03-29 03:39:44.636904 eirStru-0.2.90/
--rw-r--r--   0 wangwh     (501) staff       (20)     1060 2024-01-25 06:27:18.000000 eirStru-0.2.90/LICENSE
--rw-r--r--   0 wangwh     (501) staff       (20)       26 2024-01-25 06:27:18.000000 eirStru-0.2.90/MANIFEST.in
--rw-r--r--   0 wangwh     (501) staff       (20)     2964 2024-03-29 03:39:44.636667 eirStru-0.2.90/PKG-INFO
--rw-r--r--   0 wangwh     (501) staff       (20)     2338 2024-01-25 06:27:18.000000 eirStru-0.2.90/README.md
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-03-29 03:39:44.635773 eirStru-0.2.90/eirStru/
--rw-r--r--   0 wangwh     (501) staff       (20)       43 2024-03-14 03:14:41.000000 eirStru-0.2.90/eirStru/__init__.py
--rw-r--r--   0 wangwh     (501) staff       (20)      352 2024-01-25 06:27:18.000000 eirStru-0.2.90/eirStru/__version__.py
--rwxr--r--   0 wangwh     (501) staff       (20)     5220 2024-03-14 03:14:41.000000 eirStru-0.2.90/eirStru/aiomysql_helper.py
--rwxr--r--   0 wangwh     (501) staff       (20)    17511 2024-03-28 08:36:46.000000 eirStru-0.2.90/eirStru/common.py
--rw-r--r--   0 wangwh     (501) staff       (20)     3584 2024-02-29 12:42:57.000000 eirStru-0.2.90/eirStru/eirjob_intf.py
--rw-r--r--   0 wangwh     (501) staff       (20)     5271 2024-03-14 03:14:41.000000 eirStru-0.2.90/eirStru/eirlogin_intf.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1190 2024-02-29 02:15:20.000000 eirStru-0.2.90/eirStru/redis_utils.py
--rw-r--r--   0 wangwh     (501) staff       (20)      421 2024-03-15 21:24:26.000000 eirStru-0.2.90/eirStru/test.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1428 2024-03-14 03:14:41.000000 eirStru-0.2.90/eirStru/utils.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1670 2024-03-15 21:25:26.000000 eirStru-0.2.90/eirStru/wx_push.py
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-03-29 03:39:44.636453 eirStru-0.2.90/eirStru.egg-info/
--rw-r--r--   0 wangwh     (501) staff       (20)     2964 2024-03-29 03:39:44.000000 eirStru-0.2.90/eirStru.egg-info/PKG-INFO
--rw-r--r--   0 wangwh     (501) staff       (20)      373 2024-03-29 03:39:44.000000 eirStru-0.2.90/eirStru.egg-info/SOURCES.txt
--rw-r--r--   0 wangwh     (501) staff       (20)        1 2024-03-29 03:39:44.000000 eirStru-0.2.90/eirStru.egg-info/dependency_links.txt
--rw-r--r--   0 wangwh     (501) staff       (20)        8 2024-03-29 03:39:44.000000 eirStru-0.2.90/eirStru.egg-info/top_level.txt
--rw-r--r--   0 wangwh     (501) staff       (20)       38 2024-03-29 03:39:44.636959 eirStru-0.2.90/setup.cfg
--rw-r--r--   0 wangwh     (501) staff       (20)     3777 2024-03-29 03:39:30.000000 eirStru-0.2.90/setup.py
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-14 20:06:53.329193 eirStru-0.2.91/
+-rw-r--r--   0 wangwh     (501) staff       (20)     1060 2024-01-25 06:27:18.000000 eirStru-0.2.91/LICENSE
+-rw-r--r--   0 wangwh     (501) staff       (20)       26 2024-01-25 06:27:18.000000 eirStru-0.2.91/MANIFEST.in
+-rw-r--r--   0 wangwh     (501) staff       (20)     2964 2024-04-14 20:06:53.328934 eirStru-0.2.91/PKG-INFO
+-rw-r--r--   0 wangwh     (501) staff       (20)     2338 2024-01-25 06:27:18.000000 eirStru-0.2.91/README.md
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-14 20:06:53.327944 eirStru-0.2.91/eirStru/
+-rw-r--r--   0 wangwh     (501) staff       (20)       43 2024-03-14 03:14:41.000000 eirStru-0.2.91/eirStru/__init__.py
+-rw-r--r--   0 wangwh     (501) staff       (20)      352 2024-01-25 06:27:18.000000 eirStru-0.2.91/eirStru/__version__.py
+-rwxr--r--   0 wangwh     (501) staff       (20)     5220 2024-03-14 03:14:41.000000 eirStru-0.2.91/eirStru/aiomysql_helper.py
+-rwxr--r--   0 wangwh     (501) staff       (20)    17689 2024-04-14 20:03:49.000000 eirStru-0.2.91/eirStru/common.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     3584 2024-02-29 12:42:57.000000 eirStru-0.2.91/eirStru/eirjob_intf.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     5271 2024-03-14 03:14:41.000000 eirStru-0.2.91/eirStru/eirlogin_intf.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1190 2024-02-29 02:15:20.000000 eirStru-0.2.91/eirStru/redis_utils.py
+-rw-r--r--   0 wangwh     (501) staff       (20)      421 2024-03-15 21:24:26.000000 eirStru-0.2.91/eirStru/test.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1428 2024-03-14 03:14:41.000000 eirStru-0.2.91/eirStru/utils.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1670 2024-03-15 21:25:26.000000 eirStru-0.2.91/eirStru/wx_push.py
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-14 20:06:53.328714 eirStru-0.2.91/eirStru.egg-info/
+-rw-r--r--   0 wangwh     (501) staff       (20)     2964 2024-04-14 20:06:53.000000 eirStru-0.2.91/eirStru.egg-info/PKG-INFO
+-rw-r--r--   0 wangwh     (501) staff       (20)      373 2024-04-14 20:06:53.000000 eirStru-0.2.91/eirStru.egg-info/SOURCES.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)        1 2024-04-14 20:06:53.000000 eirStru-0.2.91/eirStru.egg-info/dependency_links.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)        8 2024-04-14 20:06:53.000000 eirStru-0.2.91/eirStru.egg-info/top_level.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)       38 2024-04-14 20:06:53.329257 eirStru-0.2.91/setup.cfg
+-rw-r--r--   0 wangwh     (501) staff       (20)     3777 2024-04-14 20:06:50.000000 eirStru-0.2.91/setup.py
```

### Comparing `eirStru-0.2.90/LICENSE` & `eirStru-0.2.91/LICENSE`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.90/PKG-INFO` & `eirStru-0.2.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eirStru
-Version: 0.2.90
+Version: 0.2.91
 Summary: My short description for my project.
 Home-page: https://github.com/me/myproject
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `eirStru-0.2.90/README.md` & `eirStru-0.2.91/README.md`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.90/eirStru/aiomysql_helper.py` & `eirStru-0.2.91/eirStru/aiomysql_helper.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.90/eirStru/common.py` & `eirStru-0.2.91/eirStru/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,16 @@
     end_time: Optional[datetime] = datetime.strptime(
         datetime.strftime(datetime.now() + timedelta(hours=4), '%Y-%m-%d %H:%M:%S'),
         '%Y-%m-%d %H:%M:%S')  # 刷箱结束时间
     plan_amount: Optional[int] = 0  # 计划数 todo
     memo: Optional[str] = None  # 备注
     cyname: Optional[str] = None
     account_list: Optional[List[dict]] = []
+    vessel: Optional[str] = None
+    vogage: Optional[str] = None
 
     def log(self, msg: str) -> str:
         logger.info(f'{self} {msg}')
         return msg
 
     def __str__(self):
         return f'{self.carrier_id} {self.bill_no}'
@@ -229,14 +231,19 @@
 
 class TaskResult(BaseModel):
     order_guid: Optional[str] = None
     status: Optional[BillStatus] = None
     memo: Optional[str] = None
     vessel: Optional[str] = None  # 船名
     voyage: Optional[str] = None  # 航次
+    rel_vessel: Optional[str] = None
+    rel_voyage: Optional[str] = None
+
+    vessel_id: Optional[str] = None
+
     ctns: List[CtnInfo] = []  # 申请的集装箱列表
     time_stamp: int = time.time_ns()
 
 
 class BillInfo(BaseModel):
     """
     提单信息
```

### Comparing `eirStru-0.2.90/eirStru/eirjob_intf.py` & `eirStru-0.2.91/eirStru/eirjob_intf.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.90/eirStru/eirlogin_intf.py` & `eirStru-0.2.91/eirStru/eirlogin_intf.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.90/eirStru/redis_utils.py` & `eirStru-0.2.91/eirStru/redis_utils.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.90/eirStru/utils.py` & `eirStru-0.2.91/eirStru/utils.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.90/eirStru/wx_push.py` & `eirStru-0.2.91/eirStru/wx_push.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.90/eirStru.egg-info/PKG-INFO` & `eirStru-0.2.91/eirStru.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eirStru
-Version: 0.2.90
+Version: 0.2.91
 Summary: My short description for my project.
 Home-page: https://github.com/me/myproject
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `eirStru-0.2.90/setup.py` & `eirStru-0.2.91/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'eirStru'
 DESCRIPTION = 'My short description for my project.'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'me@example.com'
 AUTHOR = 'Awesome Soul'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.2.90'
+VERSION = '0.2.91'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

