# Comparing `tmp/nonebot_plugin_chikari_economy-0.0.6.tar.gz` & `tmp/nonebot_plugin_chikari_economy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_chikari_economy-0.0.6.tar", last modified: Sat Apr  6 03:32:01 2024, max compression
+gzip compressed data, was "nonebot_plugin_chikari_economy-0.0.7.tar", last modified: Sun Apr 14 00:32:57 2024, max compression
```

## Comparing `nonebot_plugin_chikari_economy-0.0.6.tar` & `nonebot_plugin_chikari_economy-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 03:32:01.657017 nonebot_plugin_chikari_economy-0.0.6/
--rw-rw-rw-   0        0        0     1065 2024-02-11 07:24:25.000000 nonebot_plugin_chikari_economy-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     4492 2024-04-06 03:32:01.657017 nonebot_plugin_chikari_economy-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3924 2024-04-04 13:03:33.000000 nonebot_plugin_chikari_economy-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 03:32:01.648042 nonebot_plugin_chikari_economy-0.0.6/nonebot_plugin_chikari_economy/
--rw-rw-rw-   0        0        0     1151 2024-04-06 03:31:21.000000 nonebot_plugin_chikari_economy-0.0.6/nonebot_plugin_chikari_economy/__init__.py
--rw-rw-rw-   0        0        0     4352 2024-04-04 12:04:52.000000 nonebot_plugin_chikari_economy-0.0.6/nonebot_plugin_chikari_economy/data_handles.py
--rw-rw-rw-   0        0        0     1159 2024-04-06 03:31:18.000000 nonebot_plugin_chikari_economy-0.0.6/nonebot_plugin_chikari_economy/handles.py
-drwxrwxrwx   0        0        0        0 2024-04-06 03:32:01.656020 nonebot_plugin_chikari_economy-0.0.6/nonebot_plugin_chikari_economy.egg-info/
--rw-rw-rw-   0        0        0     4492 2024-04-06 03:32:01.000000 nonebot_plugin_chikari_economy-0.0.6/nonebot_plugin_chikari_economy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2024-04-06 03:32:01.000000 nonebot_plugin_chikari_economy-0.0.6/nonebot_plugin_chikari_economy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 03:32:01.000000 nonebot_plugin_chikari_economy-0.0.6/nonebot_plugin_chikari_economy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-04-06 03:32:01.000000 nonebot_plugin_chikari_economy-0.0.6/nonebot_plugin_chikari_economy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2024-04-06 03:32:01.000000 nonebot_plugin_chikari_economy-0.0.6/nonebot_plugin_chikari_economy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-04-06 03:32:01.658014 nonebot_plugin_chikari_economy-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      785 2024-04-06 03:31:25.000000 nonebot_plugin_chikari_economy-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 00:32:57.461006 nonebot_plugin_chikari_economy-0.0.7/
+-rw-rw-rw-   0        0        0     1065 2024-02-11 07:24:25.000000 nonebot_plugin_chikari_economy-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     4492 2024-04-14 00:32:57.460008 nonebot_plugin_chikari_economy-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3924 2024-04-04 13:03:33.000000 nonebot_plugin_chikari_economy-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 00:32:57.453027 nonebot_plugin_chikari_economy-0.0.7/nonebot_plugin_chikari_economy/
+-rw-rw-rw-   0        0        0     1151 2024-04-14 00:32:02.000000 nonebot_plugin_chikari_economy-0.0.7/nonebot_plugin_chikari_economy/__init__.py
+-rw-rw-rw-   0        0        0     5682 2024-04-14 00:31:56.000000 nonebot_plugin_chikari_economy-0.0.7/nonebot_plugin_chikari_economy/data_handles.py
+-rw-rw-rw-   0        0        0     1159 2024-04-06 03:31:18.000000 nonebot_plugin_chikari_economy-0.0.7/nonebot_plugin_chikari_economy/handles.py
+drwxrwxrwx   0        0        0        0 2024-04-14 00:32:57.459011 nonebot_plugin_chikari_economy-0.0.7/nonebot_plugin_chikari_economy.egg-info/
+-rw-rw-rw-   0        0        0     4492 2024-04-14 00:32:57.000000 nonebot_plugin_chikari_economy-0.0.7/nonebot_plugin_chikari_economy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2024-04-14 00:32:57.000000 nonebot_plugin_chikari_economy-0.0.7/nonebot_plugin_chikari_economy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 00:32:57.000000 nonebot_plugin_chikari_economy-0.0.7/nonebot_plugin_chikari_economy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-14 00:32:57.000000 nonebot_plugin_chikari_economy-0.0.7/nonebot_plugin_chikari_economy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2024-04-14 00:32:57.000000 nonebot_plugin_chikari_economy-0.0.7/nonebot_plugin_chikari_economy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-04-14 00:32:57.461006 nonebot_plugin_chikari_economy-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      785 2024-04-14 00:32:06.000000 nonebot_plugin_chikari_economy-0.0.7/setup.py
```

### Comparing `nonebot_plugin_chikari_economy-0.0.6/LICENSE` & `nonebot_plugin_chikari_economy-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_economy-0.0.6/PKG-INFO` & `nonebot_plugin_chikari_economy-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_chikari_economy
-Version: 0.0.6
+Version: 0.0.7
 Summary: A economy plugin for nonebot 2
 Home-page: https://github.com/mrqx0195/nonebot_plugin_chikari_economy
 Author: mrqx0195
 Author-email: 2317249571@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot_plugin_chikari_economy-0.0.6/README.md` & `nonebot_plugin_chikari_economy-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_economy-0.0.6/nonebot_plugin_chikari_economy/__init__.py` & `nonebot_plugin_chikari_economy-0.0.7/nonebot_plugin_chikari_economy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     description="一个经济插件（库），可由其他插件调用，以便插件间的经济联动",
     usage="",
     type="library",
     homepage="https://github.com/mrqx0195/nonebot_plugin_chikari_economy",
     supported_adapters={}
 )
 
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 
 from .data_handles import def_money_type as def_money_type
 from .data_handles import set_money as set_money
 from .data_handles import add_money as add_money
 from .data_handles import inquire_money as inquire_money
 
 __all__ = (
```

### Comparing `nonebot_plugin_chikari_economy-0.0.6/nonebot_plugin_chikari_economy/data_handles.py` & `nonebot_plugin_chikari_economy-0.0.7/nonebot_plugin_chikari_economy/data_handles.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 
 from pathlib import Path
 import nonebot_plugin_localstore as store
 
 plugin_data_file: Path = store.get_data_file("chikari_economy", "data.json")
 plugin_config_file: Path = store.get_config_file("chikari_economy", "config.json")
 
-#用户数据文件初始化及载入
-
 if not os.path.exists(plugin_data_file):
     f = open(plugin_data_file,'w')
     f.close
 with open(plugin_data_file,encoding='utf-8')as datafile:
     datastr = datafile.read()
     if not os.path.exists(plugin_data_file) or not datastr:
         f = open(plugin_data_file,'w')
@@ -21,16 +19,14 @@
         }
         json.dump(init_data,f,indent=4)
         f.close
         data = init_data
     else:
         data = json.loads(datastr,strict=False)
         
-#配置数据文件初始化及载入
-
 if not os.path.exists(plugin_config_file):
     f = open(plugin_config_file,'w')
     f.close
 with open(plugin_config_file,encoding='utf-8')as configfile:
     configstr = configfile.read()
     if not os.path.exists(plugin_config_file) or not configstr:
         f = open(plugin_config_file,'w')
@@ -39,14 +35,52 @@
         }
         json.dump(init_data,f,indent=4)
         f.close
         configdata = init_data
     else:
         configdata = json.loads(configstr,strict=False)
 
+def file_read():
+    """数据文件初始化及载入
+    """
+    
+    global data
+    global configdata
+    if not os.path.exists(plugin_data_file):
+        f = open(plugin_data_file,'w')
+        f.close
+    with open(plugin_data_file,encoding='utf-8')as datafile:
+        datastr = datafile.read()
+        if not os.path.exists(plugin_data_file) or not datastr:
+            f = open(plugin_data_file,'w')
+            init_data = {
+                
+            }
+            json.dump(init_data,f,indent=4)
+            f.close
+            data = init_data
+        else:
+            data = json.loads(datastr,strict=False)
+            
+    if not os.path.exists(plugin_config_file):
+        f = open(plugin_config_file,'w')
+        f.close
+    with open(plugin_config_file,encoding='utf-8')as configfile:
+        configstr = configfile.read()
+        if not os.path.exists(plugin_config_file) or not configstr:
+            f = open(plugin_config_file,'w')
+            init_data = {
+                "money_types":{"defaultmoney":("Chikari币","Chikari_economy提供的默认钱币")}
+            }
+            json.dump(init_data,f,indent=4)
+            f.close
+            configdata = init_data
+        else:
+            configdata = json.loads(configstr,strict=False)
+
 def file_save():
     """将内存中的数据保存至文件
     """
     
     global data
     global configdata
     f = open(plugin_data_file,'w')
@@ -62,14 +96,15 @@
     Args:
         uid (str): 用户id
         key (str): 数据键值
         value (_type_): 数据
     """
     
     global data
+    file_read()
     if uid not in data.keys:
         data[uid] = {
             "defaultmoney": 0.0
         }
     data[uid][key] = value
     file_save()
     return
@@ -79,14 +114,15 @@
 
     Args:
         key (str): 配置键值
         value (_type_): 数据
     """
     
     global configdata
+    file_read()
     configdata[key] = value
     file_save()
     return
 
 def def_money_type(id: str,name: str,description: str):
     """定义一种新的货币种类
     
@@ -99,14 +135,15 @@
         name (str): 货币的名字
         description (str): 货币的描述
 
     Returns:
         tuple: 一个二元组，应当为(name, description)
     """
     global configdata
+    file_read()
     configdata_set(id,(name, description))
     return configdata["money_types"][id]
 
 def set_money(uid: str,id: str,value: float):
     """设置用户的某种货币数量
 
     Args:
@@ -114,14 +151,15 @@
         id (str): 货币id
         value (float): 货币要设置成的值
 
     Returns:
         float: 货币设置后的值
     """
     global data,configdata
+    file_read()
     if id not in configdata["money_types"].keys:
         raise NameError(f"Undefined money type:{id}")
     data_set(uid,id,float(value))
     return data[uid][id]
 
 def add_money(uid: str,id: str,value: float):
     """增加（或减少）用户的某种货币数量
@@ -131,14 +169,15 @@
         id (str): 货币id
         value (float): 货币要增加（负数为减少）的值
 
     Returns:
         float: 货币增加（或减少）后的值
     """
     global data
+    file_read()
     if id not in configdata["money_types"].keys:
         raise NameError(f"Undefined money type:{id}")
     set_money(uid,id,data[uid][id] + value)
     return data[uid][id]
 
 def inquire_money(uid: str,id: str):
     """查询用户的某种货币数量
@@ -147,12 +186,13 @@
         uid (str): 用户id
         id (str): 货币id
 
     Returns:
         float: 货币当前数量
     """
     global data
+    file_read()
     if id not in configdata["money_types"].keys:
         raise NameError(f"Undefined money type:{id}")
     if id not in data[uid].keys:
         return 0.0
     return data[uid][id]
```

### Comparing `nonebot_plugin_chikari_economy-0.0.6/nonebot_plugin_chikari_economy/handles.py` & `nonebot_plugin_chikari_economy-0.0.7/nonebot_plugin_chikari_economy/handles.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_economy-0.0.6/nonebot_plugin_chikari_economy.egg-info/PKG-INFO` & `nonebot_plugin_chikari_economy-0.0.7/nonebot_plugin_chikari_economy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_chikari_economy
-Version: 0.0.6
+Version: 0.0.7
 Summary: A economy plugin for nonebot 2
 Home-page: https://github.com/mrqx0195/nonebot_plugin_chikari_economy
 Author: mrqx0195
 Author-email: 2317249571@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot_plugin_chikari_economy-0.0.6/setup.py` & `nonebot_plugin_chikari_economy-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot_plugin_chikari_economy",
-    version="0.0.6",
+    version="0.0.7",
     author="mrqx0195",
     author_email="2317249571@qq.com",
     description="A economy plugin for nonebot 2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mrqx0195/nonebot_plugin_chikari_economy",
     packages=setuptools.find_packages(),
```

