# Comparing `tmp/ts_soup-0.1.6.tar.gz` & `tmp/ts_soup-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\PythonProjects\load_predict\ts-soup\dist\.tmp-q0k8u2zj\ts_soup-0.1.6.tar", last modified: Sun Apr 14 00:58:08 2024, max compression
+gzip compressed data, was "D:\PythonProjects\load_predict\ts-soup\dist\.tmp-b__gxc0a\ts_soup-0.1.7.tar", last modified: Sun Apr 14 04:33:43 2024, max compression
```

## Comparing `ts_soup-0.1.6.tar` & `ts_soup-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 00:58:08.901709 ts_soup-0.1.6/
--rw-rw-rw-   0        0        0     1028 2024-04-14 00:58:08.901709 ts_soup-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      686 2024-04-05 12:25:36.000000 ts_soup-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-14 00:58:08.901709 ts_soup-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      607 2024-04-14 00:57:46.000000 ts_soup-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:58:08.886094 ts_soup-0.1.6/ts_soup/
--rw-rw-rw-   0        0        0      373 2024-04-11 23:30:37.000000 ts_soup-0.1.6/ts_soup/__init__.py
--rw-rw-rw-   0        0        0     1418 2024-04-05 21:49:15.000000 ts_soup-0.1.6/ts_soup/app.py
--rw-rw-rw-   0        0        0    15226 2024-04-14 00:57:30.000000 ts_soup-0.1.6/ts_soup/common.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:58:08.901709 ts_soup-0.1.6/ts_soup/workers/
--rw-rw-rw-   0        0        0       78 2024-04-05 04:01:53.000000 ts_soup-0.1.6/ts_soup/workers/__init__.py
--rw-rw-rw-   0        0        0     3689 2024-04-05 09:36:43.000000 ts_soup-0.1.6/ts_soup/workers/sources.py
--rw-rw-rw-   0        0        0     4674 2024-04-12 00:28:33.000000 ts_soup-0.1.6/ts_soup/workers/targets.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:58:08.901709 ts_soup-0.1.6/ts_soup.egg-info/
--rw-rw-rw-   0        0        0     1028 2024-04-14 00:58:08.000000 ts_soup-0.1.6/ts_soup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-04-14 00:58:08.000000 ts_soup-0.1.6/ts_soup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 00:58:08.000000 ts_soup-0.1.6/ts_soup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-14 00:58:08.000000 ts_soup-0.1.6/ts_soup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-14 04:33:43.845490 ts_soup-0.1.7/
+-rw-rw-rw-   0        0        0     1028 2024-04-14 04:33:43.845490 ts_soup-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2024-04-05 12:25:36.000000 ts_soup-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-14 04:33:43.845490 ts_soup-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      607 2024-04-14 04:33:39.000000 ts_soup-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 04:33:43.829867 ts_soup-0.1.7/ts_soup/
+-rw-rw-rw-   0        0        0      373 2024-04-11 23:30:37.000000 ts_soup-0.1.7/ts_soup/__init__.py
+-rw-rw-rw-   0        0        0     1418 2024-04-05 21:49:15.000000 ts_soup-0.1.7/ts_soup/app.py
+-rw-rw-rw-   0        0        0    15226 2024-04-14 00:57:30.000000 ts_soup-0.1.7/ts_soup/common.py
+drwxrwxrwx   0        0        0        0 2024-04-14 04:33:43.845490 ts_soup-0.1.7/ts_soup/workers/
+-rw-rw-rw-   0        0        0       78 2024-04-05 04:01:53.000000 ts_soup-0.1.7/ts_soup/workers/__init__.py
+-rw-rw-rw-   0        0        0     3689 2024-04-05 09:36:43.000000 ts_soup-0.1.7/ts_soup/workers/sources.py
+-rw-rw-rw-   0        0        0     5401 2024-04-14 04:33:16.000000 ts_soup-0.1.7/ts_soup/workers/targets.py
+drwxrwxrwx   0        0        0        0 2024-04-14 04:33:43.845490 ts_soup-0.1.7/ts_soup.egg-info/
+-rw-rw-rw-   0        0        0     1028 2024-04-14 04:33:43.000000 ts_soup-0.1.7/ts_soup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-04-14 04:33:43.000000 ts_soup-0.1.7/ts_soup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 04:33:43.000000 ts_soup-0.1.7/ts_soup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-14 04:33:43.000000 ts_soup-0.1.7/ts_soup.egg-info/top_level.txt
```

### Comparing `ts_soup-0.1.6/PKG-INFO` & `ts_soup-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-soup
-Version: 0.1.6
+Version: 0.1.7
 Summary: date series data synchronization
 Author: feihan ye
 Author-email: 445280206@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ts_soup-0.1.6/README.md` & `ts_soup-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ts_soup-0.1.6/setup.py` & `ts_soup-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r",encoding='utf8') as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="ts-soup",
-  version="0.1.6",
+  version="0.1.7",
   author="feihan ye",
   author_email="445280206@qq.com",
   description="date series data synchronization",
   long_description=long_description,
   long_description_content_type="text/markdown",
   # url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `ts_soup-0.1.6/ts_soup/app.py` & `ts_soup-0.1.7/ts_soup/app.py`

 * *Files identical despite different names*

### Comparing `ts_soup-0.1.6/ts_soup/common.py` & `ts_soup-0.1.7/ts_soup/common.py`

 * *Files identical despite different names*

### Comparing `ts_soup-0.1.6/ts_soup/workers/sources.py` & `ts_soup-0.1.7/ts_soup/workers/sources.py`

 * *Files identical despite different names*

### Comparing `ts_soup-0.1.6/ts_soup/workers/targets.py` & `ts_soup-0.1.7/ts_soup/workers/targets.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,42 +8,51 @@
     def __init__(self, tb,
                  db: str = None,
                  index_field: str = 'date',
                  drop_axis=0,
                  drop_na_subset=None,
                  drop_na_thresh=None,
                  has_unique_idx=False,
+                 is_empty_effect=True
                  ):
         """
         目标表信息，如果该表需要分表，则tb传入没有分表年份的表名，年份在写入时会自动加入，同时is_seperated设置为True
         :param tb:表名，
         :param db:数据库
         :param index_field:作为索引的字段，一般为日期
         :param drop_axis:如果存在空数据，drop_na的轴
         :param drop_na_subset:需要考虑删除na的列（或行）
+        :param drop_na_thresh:如果该轴不为nan的值的个数少于 drop_na_thresh设置的值，进行dropna操作
         :param has_unique_idx:是否存在唯一索引或主键，以使用replace_into语句，默认关闭，需要表添加唯一索引或主键后才能开启
                 否则会出现数据重复
+        :param is_empty_effect:表示该target  数据为空 是否影响update_state设置为 1 ,True表示数据为空，不能设置为 1
+        否则会出现数据重复
         """
         super().__init__(
                          db,
                          )
         self.tb = tb
         self.index_field = index_field
         self.drop_axis = drop_axis
         self.drop_na_subset = drop_na_subset
         self.drop_na_thresh = drop_na_thresh
         self.has_unique_idx = has_unique_idx
-
+        self.is_empty_effect = is_empty_effect
 
     def build_output(self, cur_result):
         # 写库
 
-        # 处理经过dropna以后如果全为空的情况，视为全为空，原理同上
+        # is_empty_effect 为True，表示如果该target数据为空，需要在以后再同步，因此当天update_state 不能设置为1
+        # 返回none则不会进行交集，因此不影响其他target update_state设置完成情况
         if cur_result.empty:
-            print(f'{self.tb} 无数据同步,返回结果为empty')
+
+            if self.is_empty_effect:
+                print(f'{self.tb} 无数据同步,影响最终update_state状态日期设置')
+                return []
+            print(f'{self.tb} 无数据同步,不影响最终update_state状态日期设置')
             return
 
         # 统一把index_field字段转为str类型，防止后面在insert_update_state 和各表插入数据时 使用datetime64 或 int等类型
         # datetime.date 在dataframe中有可能是Object类型
         if str(cur_result[self.index_field].dtypes) == 'datetime64' or str(
                 cur_result[self.index_field].dtypes).lower() == 'object':
             cur_result[self.index_field] = pd.to_datetime(cur_result[self.index_field]).apply(
```

### Comparing `ts_soup-0.1.6/ts_soup.egg-info/PKG-INFO` & `ts_soup-0.1.7/ts_soup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-soup
-Version: 0.1.6
+Version: 0.1.7
 Summary: date series data synchronization
 Author: feihan ye
 Author-email: 445280206@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

