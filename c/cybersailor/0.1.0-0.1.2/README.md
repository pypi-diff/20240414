# Comparing `tmp/cybersailor-0.1.0.tar.gz` & `tmp/cybersailor-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybersailor-0.1.0.tar", last modified: Wed Mar 20 01:48:41 2024, max compression
+gzip compressed data, was "cybersailor-0.1.2.tar", last modified: Sat Apr 13 09:53:53 2024, max compression
```

## Comparing `cybersailor-0.1.0.tar` & `cybersailor-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-03-20 01:48:41.568335 cybersailor-0.1.0/
--rw-r--r--   0 wanglei    (501) staff       (20)      374 2024-03-20 01:48:41.567554 cybersailor-0.1.0/PKG-INFO
--rw-r--r--   0 wanglei    (501) staff       (20)       11 2024-03-19 04:35:41.000000 cybersailor-0.1.0/README.md
-drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-03-20 01:48:41.563399 cybersailor-0.1.0/cybersailor/
--rw-r--r--   0 wanglei    (501) staff       (20)       50 2024-03-19 06:42:00.000000 cybersailor-0.1.0/cybersailor/__init__.py
--rw-r--r--   0 wanglei    (501) staff       (20)      493 2024-03-19 06:40:57.000000 cybersailor-0.1.0/cybersailor/logger.py
--rw-r--r--   0 wanglei    (501) staff       (20)     4858 2024-03-19 16:53:49.000000 cybersailor-0.1.0/cybersailor/sdk.py
-drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-03-20 01:48:41.566805 cybersailor-0.1.0/cybersailor.egg-info/
--rw-r--r--   0 wanglei    (501) staff       (20)      374 2024-03-20 01:48:41.000000 cybersailor-0.1.0/cybersailor.egg-info/PKG-INFO
--rw-r--r--   0 wanglei    (501) staff       (20)      257 2024-03-20 01:48:41.000000 cybersailor-0.1.0/cybersailor.egg-info/SOURCES.txt
--rw-r--r--   0 wanglei    (501) staff       (20)        1 2024-03-20 01:48:41.000000 cybersailor-0.1.0/cybersailor.egg-info/dependency_links.txt
--rw-r--r--   0 wanglei    (501) staff       (20)       34 2024-03-20 01:48:41.000000 cybersailor-0.1.0/cybersailor.egg-info/requires.txt
--rw-r--r--   0 wanglei    (501) staff       (20)       12 2024-03-20 01:48:41.000000 cybersailor-0.1.0/cybersailor.egg-info/top_level.txt
--rw-r--r--   0 wanglei    (501) staff       (20)       38 2024-03-20 01:48:41.568506 cybersailor-0.1.0/setup.cfg
--rw-r--r--   0 wanglei    (501) staff       (20)      608 2024-03-19 04:49:34.000000 cybersailor-0.1.0/setup.py
+drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-04-13 09:53:53.490049 cybersailor-0.1.2/
+-rw-r--r--   0 wanglei    (501) staff       (20)      372 2024-04-13 09:53:53.489636 cybersailor-0.1.2/PKG-INFO
+-rw-r--r--   0 wanglei    (501) staff       (20)       11 2024-03-19 04:35:41.000000 cybersailor-0.1.2/README.md
+drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-04-13 09:53:53.486363 cybersailor-0.1.2/cybersailor/
+-rw-r--r--   0 wanglei    (501) staff       (20)       50 2024-03-19 06:42:00.000000 cybersailor-0.1.2/cybersailor/__init__.py
+-rw-r--r--   0 wanglei    (501) staff       (20)      533 2024-03-20 02:22:34.000000 cybersailor-0.1.2/cybersailor/logger.py
+-rw-r--r--   0 wanglei    (501) staff       (20)     5639 2024-04-12 10:37:14.000000 cybersailor-0.1.2/cybersailor/sdk.py
+drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-04-13 09:53:53.489086 cybersailor-0.1.2/cybersailor.egg-info/
+-rw-r--r--   0 wanglei    (501) staff       (20)      372 2024-04-13 09:53:53.000000 cybersailor-0.1.2/cybersailor.egg-info/PKG-INFO
+-rw-r--r--   0 wanglei    (501) staff       (20)      257 2024-04-13 09:53:53.000000 cybersailor-0.1.2/cybersailor.egg-info/SOURCES.txt
+-rw-r--r--   0 wanglei    (501) staff       (20)        1 2024-04-13 09:53:53.000000 cybersailor-0.1.2/cybersailor.egg-info/dependency_links.txt
+-rw-r--r--   0 wanglei    (501) staff       (20)       34 2024-04-13 09:53:53.000000 cybersailor-0.1.2/cybersailor.egg-info/requires.txt
+-rw-r--r--   0 wanglei    (501) staff       (20)       12 2024-04-13 09:53:53.000000 cybersailor-0.1.2/cybersailor.egg-info/top_level.txt
+-rw-r--r--   0 wanglei    (501) staff       (20)       38 2024-04-13 09:53:53.490154 cybersailor-0.1.2/setup.cfg
+-rw-r--r--   0 wanglei    (501) staff       (20)      562 2024-04-13 09:53:42.000000 cybersailor-0.1.2/setup.py
```

### Comparing `cybersailor-0.1.0/cybersailor/sdk.py` & `cybersailor-0.1.2/cybersailor/sdk.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,55 @@
 from typing import Any
 from carthooks import Client
 from .logger import Logger
 import os
+import time
 
 class Task:
-    def __init__(self, handler, app_id, collection_id, task_status_field, task_status_values,
+    def __init__(self, handler, app_id, collection_id, 
                 trigger="pulling_items", 
                 filter=None, 
                 pagelimit=1,
                 include_locked=False,
                 sort=['created'], 
                 pulling_interval=30):
         self.handler = handler
         self.trigger = trigger
+        self.last_pull = 0
         self.pulling_options = {
             "app_id": app_id,
             "collection_id": collection_id,
-            "task_status_field": task_status_field,
-            "task_status_values": task_status_values,
             "filter": filter,
             "sort": sort,
             "pulling_interval": pulling_interval,
             "pagelimit": pagelimit,
             "include_locked": include_locked
         }
+    
+    def pulling_now(self):
+        self.last_pull = time.time()
+
+    def is_pull_able(self):
+        return time.time() - self.last_pull > self.pulling_options["pulling_interval"]
 
 class Record:
     def __init__(self, sailor, app_id, collection_id, item_id, data):
         self.sailor = sailor
         self.app_id = app_id
         self.collection_id = collection_id
         self.item_id = item_id
         self.__record = data
         self.id = data["id"]
         self.created_at = data["created_at"]
         self.updated_at = data["updated_at"]
         self.title = data["title"]
         self.data = data["fields"]
+    
+    def __getitem__(self, key):
+        return self.__record.get(key)
 
     def __str__(self) -> str:
         return f"Record(title={self.__record.get('title')}, item_id={self.item_id})"
     
     def __repr__(self) -> str:
         return f"Record(app_id={self.app_id}, collection_id={self.collection_id}, item_id={self.item_id})"
     
@@ -56,74 +65,92 @@
     
 class Context:
     def __init__(self, sailor, task, logger):
         self.task = task
         self.sailor = sailor
         self.logger = logger
 
-    def create(self, app_id, collection_id, data):
-        return self.sailor.create(app_id, collection_id, data)
+    # def __getattribute__(self, __name: str) -> Any:
+    #     return self.sailor.client.__getattribute__(__name)
+
+    # def create(self, app_id, collection_id, data):
+    #     return self.sailor.create(app_id, collection_id, data)
 
 class Sailor:
-    def __init__(self, url=None, token=None, sailor_id=None):
-        self.url = url
-        self.token = token
+    def __init__(self, token=None, sailor_id=None):
         self.tasks = []
         self.logger = Logger("cybersailor")
+        self.client = Client()
+        self.client.setAccessToken(token)
         if sailor_id == None:
             self.sailor_id = os.uname().nodename
         else:
             self.sailor_id = sailor_id
 
     def subscribe(self, **kwargs):
         task = Task(**kwargs)
         self.tasks.append(task)
 
     def lock(self, record, lock_timeout=600, subject=None):
-        self.logger.info(f"Locking task: {record}")
-        return self.client.lock_item(record.app_id, record.collection_id, record.item_id, lock_timeout=lock_timeout, lock_id=self.sailor_id, subject=subject)
+        self.logger.debug(f"Locking task: {record}")
+        return self.client.lockItem(record.app_id, record.collection_id, record.item_id, lock_timeout=lock_timeout, lock_id=self.sailor_id, subject=subject)
 
     def unlock(self, record):
-        self.logger.info(f"Unlocking task: {record}")
-        return self.client.unlock_item(record.app_id, record.collection_id, record.item_id, lock_id=self.sailor_id)
+        self.logger.debug(f"Unlocking task: {record}")
+        return self.client.unlockItem(record.app_id, record.collection_id, record.item_id, lock_id=self.sailor_id)
 
     def update(self, task, map):
-        self.logger.info(f"Updating task: {task} with map: {map}")
-        pass
+        self.logger.debug(f"Updating task: {task} with map: {map}")
+        return self.client.updateItem(task.app_id, task.collection_id, task.item_id, map)
 
     def create(self, app_id, collection_id, data):
-        self.logger.info(f"Creating record in app_id: {app_id}, collection_id: {collection_id} with data: {data}")
-        result = self.client.create_item(app_id, collection_id, data)
+        self.logger.debug(f"Creating record in app_id: {app_id}, collection_id: {collection_id} with data: {data}")
+        result = self.client.createItem(app_id, collection_id, data)
         return result
 
     def run(self):
-        self.logger.info("Running...")
-
-        self.client = Client(base_url = self.url)
-        self.client.set_access_token(self.token)
+        self.logger.debug("Running...")
 
-        for task in self.tasks:
-            if task.trigger == "pulling_items":
-                print(task.pulling_options)
-                app_id = task.pulling_options["app_id"]
-                collection_id = task.pulling_options["collection_id"]
-                self.logger.info(f"Pulling items from app_id: {app_id}, collection_id: {collection_id}")
-
-                options = {
-                    "limit": task.pulling_options["pagelimit"],
-                }
-
-                if task.pulling_options["include_locked"] == False:
-                    options["unlockedOrLockedBy"] = self.sailor_id
-
-                result = self.client.get_items(app_id, collection_id, **options)
-                            # filter=task.pulling_options.filter, 
-                            # limit=task.pulling_options["pagelimit"],
-                            # sort=task.pulling_options.sort
-                        # )
-                items = result.data
-                if items.__len__() > 0:
-                    context = Context(sailor=self, task=task, logger=self.logger)
-                    for item in items:
-                        self.logger.info(f"Handling item: {item['id']}")
-                        record = Record(sailor=self, app_id=app_id, collection_id=collection_id, item_id=item['id'], data=item)
-                        task.handler(context, record)
+        while True:
+            for task in self.tasks:
+                if task.trigger == "pulling_items" and task.is_pull_able():
+                    self.pull(task)
+            time.sleep(1)
+
+    def pull(self,task):
+        try:
+            app_id = task.pulling_options["app_id"]
+            collection_id = task.pulling_options["collection_id"]
+            self.logger.debug(f"Pulling items from app_id: {app_id}, collection_id: {collection_id}")
+
+            options = {
+                "limit": task.pulling_options["pagelimit"],
+            }
+
+            if task.pulling_options["sort"] != None:
+                options["sort"] = task.pulling_options["sort"]
+
+            if task.pulling_options["filter"] != None:
+                for column in task.pulling_options["filter"]:
+                    for operator in task.pulling_options["filter"][column]:
+                        options[f"filters[{column}][{operator}]"] = task.pulling_options["filter"][column][operator]
+
+            if task.pulling_options["include_locked"] == False:
+                options["unlockedOrLockedBy"] = self.sailor_id
+
+            # print(options)
+
+            result = self.client.getItems(app_id, collection_id, **options)
+            
+            items = result.data
+            task.pulling_now()
+            if items.__len__() > 0:
+                context = Context(sailor=self, task=task, logger=self.logger)
+                for item in items:
+                    self.logger.debug(f"Handling item: {item['id']}")
+                    record = Record(sailor=self, app_id=app_id, collection_id=collection_id, item_id=item['id'], data=item)
+                    self.logger.debug(f"Record: {record}")
+                    task.handler(context, record)
+        except Exception as e:
+            self.logger.error(f"Error: {e}")
+            print(e.__list__())
+            time.sleep(5)
```

### Comparing `cybersailor-0.1.0/setup.py` & `cybersailor-0.1.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cybersailor',
-    version='0.1.0',
+    version='0.1.2',
     packages=find_packages(),
-    description='A simple example package',
+    description='Cybersailor Python SDK',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Carthooks',
     author_email='developer@carthooks.com',
     license='MIT',
     install_requires=[
-        # 列出你的包的依赖，例如
         'requests>=2.23.0',
-        'carthooks>=0.1.0'
+        'carthooks>=0.1.2'
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
     ],
 )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

