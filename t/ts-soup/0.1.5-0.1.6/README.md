# Comparing `tmp/ts-soup-0.1.5.tar.gz` & `tmp/ts_soup-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\PythonProjects\load_predict\ts-soup\dist\.tmp-cc3eiarc\ts-soup-0.1.5.tar", last modified: Fri Apr 12 03:34:58 2024, max compression
+gzip compressed data, was "D:\PythonProjects\load_predict\ts-soup\dist\.tmp-q0k8u2zj\ts_soup-0.1.6.tar", last modified: Sun Apr 14 00:58:08 2024, max compression
```

## Comparing `ts-soup-0.1.5.tar` & `ts_soup-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 03:34:58.141756 ts-soup-0.1.5/
--rw-rw-rw-   0        0        0     1028 2024-04-12 03:34:58.141756 ts-soup-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      686 2024-04-05 12:25:36.000000 ts-soup-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-12 03:34:58.141756 ts-soup-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      607 2024-04-12 03:34:43.000000 ts-soup-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 03:34:58.141756 ts-soup-0.1.5/ts_soup/
--rw-rw-rw-   0        0        0      373 2024-04-11 23:30:37.000000 ts-soup-0.1.5/ts_soup/__init__.py
--rw-rw-rw-   0        0        0     1418 2024-04-05 21:49:15.000000 ts-soup-0.1.5/ts_soup/app.py
--rw-rw-rw-   0        0        0    15580 2024-04-12 00:28:33.000000 ts-soup-0.1.5/ts_soup/common.py
-drwxrwxrwx   0        0        0        0 2024-04-12 03:34:58.141756 ts-soup-0.1.5/ts_soup/workers/
--rw-rw-rw-   0        0        0       78 2024-04-05 04:01:53.000000 ts-soup-0.1.5/ts_soup/workers/__init__.py
--rw-rw-rw-   0        0        0     3689 2024-04-05 09:36:43.000000 ts-soup-0.1.5/ts_soup/workers/sources.py
--rw-rw-rw-   0        0        0     4674 2024-04-12 00:28:33.000000 ts-soup-0.1.5/ts_soup/workers/targets.py
-drwxrwxrwx   0        0        0        0 2024-04-12 03:34:58.141756 ts-soup-0.1.5/ts_soup.egg-info/
--rw-rw-rw-   0        0        0     1028 2024-04-12 03:34:58.000000 ts-soup-0.1.5/ts_soup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-04-12 03:34:58.000000 ts-soup-0.1.5/ts_soup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 03:34:58.000000 ts-soup-0.1.5/ts_soup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-12 03:34:58.000000 ts-soup-0.1.5/ts_soup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-14 00:58:08.901709 ts_soup-0.1.6/
+-rw-rw-rw-   0        0        0     1028 2024-04-14 00:58:08.901709 ts_soup-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2024-04-05 12:25:36.000000 ts_soup-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-14 00:58:08.901709 ts_soup-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      607 2024-04-14 00:57:46.000000 ts_soup-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 00:58:08.886094 ts_soup-0.1.6/ts_soup/
+-rw-rw-rw-   0        0        0      373 2024-04-11 23:30:37.000000 ts_soup-0.1.6/ts_soup/__init__.py
+-rw-rw-rw-   0        0        0     1418 2024-04-05 21:49:15.000000 ts_soup-0.1.6/ts_soup/app.py
+-rw-rw-rw-   0        0        0    15226 2024-04-14 00:57:30.000000 ts_soup-0.1.6/ts_soup/common.py
+drwxrwxrwx   0        0        0        0 2024-04-14 00:58:08.901709 ts_soup-0.1.6/ts_soup/workers/
+-rw-rw-rw-   0        0        0       78 2024-04-05 04:01:53.000000 ts_soup-0.1.6/ts_soup/workers/__init__.py
+-rw-rw-rw-   0        0        0     3689 2024-04-05 09:36:43.000000 ts_soup-0.1.6/ts_soup/workers/sources.py
+-rw-rw-rw-   0        0        0     4674 2024-04-12 00:28:33.000000 ts_soup-0.1.6/ts_soup/workers/targets.py
+drwxrwxrwx   0        0        0        0 2024-04-14 00:58:08.901709 ts_soup-0.1.6/ts_soup.egg-info/
+-rw-rw-rw-   0        0        0     1028 2024-04-14 00:58:08.000000 ts_soup-0.1.6/ts_soup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-04-14 00:58:08.000000 ts_soup-0.1.6/ts_soup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 00:58:08.000000 ts_soup-0.1.6/ts_soup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-14 00:58:08.000000 ts_soup-0.1.6/ts_soup.egg-info/top_level.txt
```

### Comparing `ts-soup-0.1.5/PKG-INFO` & `ts_soup-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-soup
-Version: 0.1.5
+Version: 0.1.6
 Summary: date series data synchronization
 Author: feihan ye
 Author-email: 445280206@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ts-soup-0.1.5/README.md` & `ts_soup-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ts-soup-0.1.5/setup.py` & `ts_soup-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r",encoding='utf8') as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="ts-soup",
-  version="0.1.5",
+  version="0.1.6",
   author="feihan ye",
   author_email="445280206@qq.com",
   description="date series data synchronization",
   long_description=long_description,
   long_description_content_type="text/markdown",
   # url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `ts-soup-0.1.5/ts_soup/app.py` & `ts_soup-0.1.6/ts_soup/app.py`

 * *Files identical despite different names*

### Comparing `ts-soup-0.1.5/ts_soup/common.py` & `ts_soup-0.1.6/ts_soup/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -115,36 +115,26 @@
     data_updated_state = pd.concat([data_updated_state, fill_date_range])
     data_updated_state['state'] = 1
     pivot_table = data_updated_state.pivot_table(index='update_date', columns='table_name', values='state')
 
     both_columns = [i for i in to_update_tables if i in pivot_table.columns.values.tolist()]  # 原来记录里有且现在仍需要的表
 
     non_columns = [i for i in to_update_tables if i not in pivot_table.columns.values.tolist()]  # 原来记录没有现在新增的表
-    state_table = pivot_table[both_columns].fillna(0)
-    state_table[non_columns] = 0
-    state_table = state_table.reset_index()
-    state_table['update_date'] = state_table['update_date'].apply(lambda x: x.strftime('%Y-%m-%d'))
-
-    if len(customized_time) > 0 and len(customized_table) == 0:  # 1、指定时间，未指定表格:
-        DATA_UPDATED_STATE = state_table.loc[state_table['update_date'].isin(customized_time)]
-        DATA_UPDATED_STATE.iloc[:, 1:] = 0
-        return to_update_tables
-
-    elif len(customized_time) == 0 and len(customized_table) > 0:  # 2、指定表格，未指定时间：
-        DATA_UPDATED_STATE = state_table
-        return customized_table
-
-    elif len(customized_time) > 0 and len(customized_table) > 0:  # 3、指定时间，指定表格:
-        DATA_UPDATED_STATE = state_table.loc[state_table['update_date'].isin(customized_time)]
-        DATA_UPDATED_STATE.loc[:, customized_table] = 0
-        return customized_table
-
-    else:
-        DATA_UPDATED_STATE = state_table  # 4、未指定时间，未指定表格:
-        return to_update_tables
+    DATA_UPDATED_STATE = pivot_table[both_columns].fillna(0)
+    DATA_UPDATED_STATE[non_columns] = 0
+    DATA_UPDATED_STATE = DATA_UPDATED_STATE.reset_index()
+    DATA_UPDATED_STATE['update_date'] = DATA_UPDATED_STATE['update_date'].apply(lambda x: x.strftime('%Y-%m-%d'))
+    to_update_tables = customized_table if len(customized_table)>0 else to_update_tables
+    if len(customized_time) > 0:
+        DATA_UPDATED_STATE = DATA_UPDATED_STATE.set_index('update_date')
+        for one_date in customized_time:
+            DATA_UPDATED_STATE.loc[one_date, to_update_tables] = 0
+        DATA_UPDATED_STATE = DATA_UPDATED_STATE.loc[customized_time, to_update_tables]
+        DATA_UPDATED_STATE = DATA_UPDATED_STATE.reset_index()
+    return to_update_tables
 
 
 class BaseSource(ABC):
     """
     定义需要使用在入口函数中注册的数据库连接的source的基类，即 如果需要使用数据库连接，则需要继承BaseSource
     """
     def __init__(self,
```

### Comparing `ts-soup-0.1.5/ts_soup/workers/sources.py` & `ts_soup-0.1.6/ts_soup/workers/sources.py`

 * *Files identical despite different names*

### Comparing `ts-soup-0.1.5/ts_soup/workers/targets.py` & `ts_soup-0.1.6/ts_soup/workers/targets.py`

 * *Files identical despite different names*

### Comparing `ts-soup-0.1.5/ts_soup.egg-info/PKG-INFO` & `ts_soup-0.1.6/ts_soup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-soup
-Version: 0.1.5
+Version: 0.1.6
 Summary: date series data synchronization
 Author: feihan ye
 Author-email: 445280206@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

