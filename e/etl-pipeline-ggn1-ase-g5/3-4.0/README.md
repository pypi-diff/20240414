# Comparing `tmp/etl_pipeline_ggn1_ase_g5-3.tar.gz` & `tmp/etl_pipeline_ggn1_ase_g5-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etl_pipeline_ggn1_ase_g5-3.tar", last modified: Thu Mar 28 15:48:11 2024, max compression
+gzip compressed data, was "etl_pipeline_ggn1_ase_g5-4.0.tar", last modified: Sun Apr 14 18:47:36 2024, max compression
```

## Comparing `etl_pipeline_ggn1_ase_g5-3.tar` & `etl_pipeline_ggn1_ase_g5-4.0.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 15:48:11.048010 etl_pipeline_ggn1_ase_g5-3/
--rw-rw-rw-   0        0        0      161 2024-03-28 15:48:11.046009 etl_pipeline_ggn1_ase_g5-3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-28 15:48:11.039808 etl_pipeline_ggn1_ase_g5-3/etl_pipeline_ggn1_ase_g5/
--rw-rw-rw-   0        0        0       86 2024-03-26 13:32:44.000000 etl_pipeline_ggn1_ase_g5-3/etl_pipeline_ggn1_ase_g5/__init__.py
--rw-rw-rw-   0        0        0    16005 2024-03-27 03:21:32.000000 etl_pipeline_ggn1_ase_g5-3/etl_pipeline_ggn1_ase_g5/__main__.py
--rw-rw-rw-   0        0        0     9540 2024-03-26 14:28:01.000000 etl_pipeline_ggn1_ase_g5-3/etl_pipeline_ggn1_ase_g5/etl_db_manager.py
--rw-rw-rw-   0        0        0     4584 2024-03-27 02:56:01.000000 etl_pipeline_ggn1_ase_g5-3/etl_pipeline_ggn1_ase_g5/etl_task.py
--rw-rw-rw-   0        0        0      559 2024-03-26 13:32:35.000000 etl_pipeline_ggn1_ase_g5-3/etl_pipeline_ggn1_ase_g5/utility.py
-drwxrwxrwx   0        0        0        0 2024-03-28 15:48:11.045001 etl_pipeline_ggn1_ase_g5-3/etl_pipeline_ggn1_ase_g5.egg-info/
--rw-rw-rw-   0        0        0      161 2024-03-28 15:48:10.000000 etl_pipeline_ggn1_ase_g5-3/etl_pipeline_ggn1_ase_g5.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      507 2024-03-28 15:48:10.000000 etl_pipeline_ggn1_ase_g5-3/etl_pipeline_ggn1_ase_g5.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 15:48:10.000000 etl_pipeline_ggn1_ase_g5-3/etl_pipeline_ggn1_ase_g5.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-03-28 15:48:10.000000 etl_pipeline_ggn1_ase_g5-3/etl_pipeline_ggn1_ase_g5.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2024-03-28 15:48:10.000000 etl_pipeline_ggn1_ase_g5-3/etl_pipeline_ggn1_ase_g5.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2024-03-28 15:48:10.000000 etl_pipeline_ggn1_ase_g5-3/etl_pipeline_ggn1_ase_g5.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-28 15:48:11.048010 etl_pipeline_ggn1_ase_g5-3/setup.cfg
--rw-rw-rw-   0        0        0      340 2024-03-28 15:47:32.000000 etl_pipeline_ggn1_ase_g5-3/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-28 15:48:11.045001 etl_pipeline_ggn1_ase_g5-3/tests/
--rw-rw-rw-   0        0        0    17118 2024-03-27 03:17:38.000000 etl_pipeline_ggn1_ase_g5-3/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2024-04-14 18:47:36.003585 etl_pipeline_ggn1_ase_g5-4.0/
+-rw-rw-rw-   0        0        0      186 2024-04-14 18:47:36.003585 etl_pipeline_ggn1_ase_g5-4.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-14 18:47:36.003585 etl_pipeline_ggn1_ase_g5-4.0/etl_pipeline_ggn1_ase_g5/
+-rw-rw-rw-   0        0        0        0 2024-04-14 18:14:27.000000 etl_pipeline_ggn1_ase_g5-4.0/etl_pipeline_ggn1_ase_g5/__init__.py
+-rw-rw-rw-   0        0        0    15443 2024-04-14 18:36:19.000000 etl_pipeline_ggn1_ase_g5-4.0/etl_pipeline_ggn1_ase_g5/__main__.py
+-rw-rw-rw-   0        0        0     9629 2024-04-14 18:36:04.000000 etl_pipeline_ggn1_ase_g5-4.0/etl_pipeline_ggn1_ase_g5/etl_db_manager.py
+-rw-rw-rw-   0        0        0     4584 2024-04-12 19:08:46.000000 etl_pipeline_ggn1_ase_g5-4.0/etl_pipeline_ggn1_ase_g5/etl_task.py
+-rw-rw-rw-   0        0        0      559 2024-04-12 19:45:10.000000 etl_pipeline_ggn1_ase_g5-4.0/etl_pipeline_ggn1_ase_g5/utility.py
+drwxrwxrwx   0        0        0        0 2024-04-14 18:47:36.003585 etl_pipeline_ggn1_ase_g5-4.0/etl_pipeline_ggn1_ase_g5.egg-info/
+-rw-rw-rw-   0        0        0      186 2024-04-14 18:47:35.000000 etl_pipeline_ggn1_ase_g5-4.0/etl_pipeline_ggn1_ase_g5.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      488 2024-04-14 18:47:35.000000 etl_pipeline_ggn1_ase_g5-4.0/etl_pipeline_ggn1_ase_g5.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 18:47:35.000000 etl_pipeline_ggn1_ase_g5-4.0/etl_pipeline_ggn1_ase_g5.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-04-14 18:47:35.000000 etl_pipeline_ggn1_ase_g5-4.0/etl_pipeline_ggn1_ase_g5.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2024-04-14 18:47:35.000000 etl_pipeline_ggn1_ase_g5-4.0/etl_pipeline_ggn1_ase_g5.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-04-14 18:47:35.000000 etl_pipeline_ggn1_ase_g5-4.0/etl_pipeline_ggn1_ase_g5.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 18:47:36.003585 etl_pipeline_ggn1_ase_g5-4.0/setup.cfg
+-rw-rw-rw-   0        0        0      350 2024-04-14 18:47:19.000000 etl_pipeline_ggn1_ase_g5-4.0/setup.py
```

### Comparing `etl_pipeline_ggn1_ase_g5-3/etl_pipeline_ggn1_ase_g5/__main__.py` & `etl_pipeline_ggn1_ase_g5-4.0/etl_pipeline_ggn1_ase_g5/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 import os
 import time
 import signal
-import atexit
 import uvicorn
 import schedule
 import argparse
 import threading
 import logging.config
-from threading import Event
 from fastapi import FastAPI
 from .utility import base64decode_obj
 from .etl_db_manager import ETLDataBaseManager
 
 # Global variables.
 DB_MANAGER = None
 HOST = None
 PORT = None
 SCHEDULER_RUNNING = False
 SCHEDULED_JOBS = {}
+LOGGER = logging.getLogger("etl_pipeline")
 
-# Logger
-logger = logging.getLogger("etl_pipeline")
 def configure_logger(logs_dir):
     """ 
     Sets up the logger. 
     @param logs_dir: Path to directory within 
                           which logs are to be stored.
     """
     # Create logging directory if it does not already exist.
@@ -54,32 +51,24 @@
             "file": {
                 "class": "logging.handlers.RotatingFileHandler",
                 "level": "INFO",
                 "formatter": "detailed",
                 "filename": f"{logs_dir}/etl_pipeline.log",
                 "maxBytes": 10000000,
                 "backupCount": 3,
-            },
-            "queue_handler": {
-                "class": "logging.handlers.QueueHandler",
-                "handlers": ["stderr", "file"],
-                "respect_handler_level": True
             }
         },
         "loggers": {
-            "root": {"level": "DEBUG", "handlers": ["queue_handler"]}
+            "root": {
+                "level": "DEBUG", 
+                "handlers": ["stderr", "file"]
+            }
         }
     })
 
-    # Set up non-blocking logger on a separate thread.
-    queue_handler = logging.getHandlerByName("queue_handler")
-    if queue_handler is not None:
-        queue_handler.listener.start() # Start this thread.
-        atexit.register(queue_handler.listener.stop)
-
     print(
         "Logger 'etl_pipeline' was successfully set up.",
         f"Logs shall be saved at {logs_dir}"
     )
 
 # Utility functions.
 def run_scheduler():
@@ -119,25 +108,27 @@
     response = {'status': 200, 'message': f'', 'data':[]}
     task = None
     try:
         if SCHEDULER_RUNNING == False:
             start_scheduler()
         task = base64decode_obj(task_str) # Get ETL Task from base64 encoded string.
         DB_MANAGER.create_task(task) # Add task into DB.
+        print("[DEBUG] Task created in DB.")
         if not task.name in SCHEDULED_JOBS:
             job = task.schedule(schedule=schedule, host=HOST, port=PORT) # Schedule task.
+            print("[DEBUG] Task scheduled.")
             SCHEDULED_JOBS[task.name] = job # Keep a reference of this scheduled job.
         response['message'] = f"Success. Task created and scheduled {task.name}."
     except Exception as e:
         response = read_task(task.name, fields='status')
         if 'data' in response and response['data']['status'] == 'running':
             stop_task(task.name) # Stop this task if running/scheduled and then delete.
             delete_task(task.name) # Remove partially correct entered task.
         response['status'] = 400
-        logger.error(f'Failure. Could not create task due to "{e}".')
+        LOGGER.error(f'Failure. Could not create task due to "{e}".')
         response['message'] = f'Failure. Could not create task "{task.name}" due to "{e}".'
     return response
 
 @app.delete("/task/")
 def delete_task(task_name: str):
     """
     Deletes a task with given name if it exists.
@@ -153,15 +144,15 @@
             response['message'] = f'Task "{task_name}" is scheduled. Please stop it before deleting.'
         else:
             DB_MANAGER.delete_task(name=task_name)
             print(f'If the task "{task_name}" existed, it has been deleted.')
             response['status'] = 200
             response['message'] = f'Success. If the task "{task_name}" existed, it has been deleted.'
     except Exception as e:
-        logger.error(f'Failure. Could not delete task "{task_name}" due to "{e}".')
+        LOGGER.error(f'Failure. Could not delete task "{task_name}" due to "{e}".')
         response['status'] = 400
         response['message'] = f'Failure. Could not delete task "{task_name}" due to "{e}".'
     return response
 
 @app.get("/task/")
 def read_task(task_name:str, fields:str=''):
     """
@@ -187,15 +178,15 @@
             response['status'] = 200
             response["message"] = f'Success. No such task as "{task_name}".'
         else:
             response['status'] = 200
             response["data"] = task
             response["message"] = f'Success. Retrieved task "{task_name}".'
     except Exception as e:
-        logger.error(f'Failure. Could not get task "{task_name}" due to "{e}".')
+        LOGGER.error(f'Failure. Could not get task "{task_name}" due to "{e}".')
         response['status'] = 400
         response['message'] = f'Failure. Could not get task "{task_name}" due to "{e}".'
     return response
 
 @app.get("/task/all/")
 def read_all_tasks():
     """
@@ -213,15 +204,15 @@
                 'repeat_time_unit': task.repeat_time_unit,
                 'repeat_interval': task.repeat_interval,
                 'time_run_last_start': str(task.time_run_last_start),
                 'time_run_last_end': str(task.time_run_last_end)
             })
         response["message"] = f"Success. Retrieved tasks."
     except Exception as e:
-        logger.error(f'Failure. Could not get tasks due to "{e}".')
+        LOGGER.error(f'Failure. Could not get tasks due to "{e}".')
         response['status'] = 400
         response['message'] = f'Failure. Could not get tasks due to "{e}".'
     return response
 
 @app.put("/task/")
 def update_task(task_name: str, new_values: dict):
     """
@@ -250,15 +241,15 @@
             print(f'Task "{task_name}" is scheduled. Please stop it before updating.')
             response['status'] = 400
             response['message'] = f'Task "{task_name}" is scheduled. Please stop it before updating.'
         else:
             DB_MANAGER.update_task(name=task_name, new_values=new_values)
             response["message"] = f'Success. Status of task "{task_name}" updated with new values {new_values}.'
     except Exception as e:
-        logger.error(f'Failure. Could not update status of task "{task_name}" due to "{e}".')
+        LOGGER.error(f'Failure. Could not update status of task "{task_name}" due to "{e}".')
         response['status'] = 400
         response['message'] = f'Failure. Could not update status of task "{task_name}" due to "{e}".'
     return response
 
 @app.put("/task/start")
 def start_task(task_name:str):
     """ 
@@ -283,15 +274,15 @@
                     SCHEDULED_JOBS[task.name] = job
                     response["message"] += f"Started task '{task_name}'. "
                     print(f'Started task "{task_name}".')
                 else:
                     response["message"] += f"Task '{task_name}' is already scheduled/running. "
                     print(f"Task '{task_name}' is already scheduled.")
     except Exception as e:
-        logger.error(f'Failed to start task "{task_name}" due to "{e}".')
+        LOGGER.error(f'Failed to start task "{task_name}" due to "{e}".')
         response['status'] = 400
         response["message"] = f'Failed to start task "{task_name}" due to "{e}".'
     return response
 
 @app.put("/task/stop/")
 def stop_task(task_name: str):
     """
@@ -308,15 +299,15 @@
             del SCHEDULED_JOBS[task_name]
             print(f'Task "{task_name}" stopped.')
             response['message'] = 'Success. Task has been stopped.'
         else:
             print(f'Task "{task_name}" is not running or scheduled.')
             response['message'] = f'Task "{task_name}" is not running or scheduled.'
     except Exception as e:
-        logger.error(f'Failure. Could not stop task "{task_name}" due to "{e}".')
+        LOGGER.error(f'Failure. Could not stop task "{task_name}" due to "{e}".')
         print(f'Task "{task_name}" could not be stopped.')
         response['status'] = 400
         response['message'] = f'Failure. Could not stop task "{task_name}" due to "{e}".'
     return response
 
 @app.get("/scheduler/start/")
 def start_scheduler():
@@ -335,15 +326,14 @@
             print('Scheduler started.')
             response["status"] = 200
             response["message"] = f"Scheduler started."
     except Exception as e:
         response["message"] = f'Scheduler could not be started due to "{e}".'
         response["status"] = 400
         response["message"] = f'Scheduler could not be started due to "{e}".'
-    print('[DEBUG] start_scheduler(...): # ACTIVE THREADS =', threading.active_count())
     return response
 
 @app.get("/scheduler/stop/")
 def stop_scheduler():
     """ Stop the task scheduler. """
     global SCHEDULER_RUNNING
     response = {"status": 200, "message": "", "data":[]}
@@ -354,18 +344,17 @@
             response["message"] = "Scheduler is not running."
         else:
             SCHEDULER_RUNNING = False
             response["status"] = 200
             print("Scheduler stopped.")
             response["message"] = "Scheduler stopped."
     except Exception as e:
-        logger.log(f'Scheduler could not be stopped due to "{e}".')
+        LOGGER.log(f'Scheduler could not be stopped due to "{e}".')
         response["status"] = 400
         response["message"] = f'Scheduler could not be stopped due to "{e}".'
-    print('[DEBUG] stop_scheduler(...): # ACTIVE THREADS =', threading.active_count())
     return response
 
 @app.get("/end")
 def end_process():
     """
     This function ends the program gracefully.
     """
```

### Comparing `etl_pipeline_ggn1_ase_g5-3/etl_pipeline_ggn1_ase_g5/etl_db_manager.py` & `etl_pipeline_ggn1_ase_g5-4.0/etl_pipeline_ggn1_ase_g5/etl_db_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,25 +220,27 @@
         @param name: Name of the task.
         """
         # If a task with given name exists, then delete this task.
         self.query(f"DELETE FROM etl_tasks WHERE name='{name}';")
 
     def load_tasks(self, filters:dict={}):
         """
-        Loads tasks from the DB while respecting given fiter
+        Loads tasks from the DB while respecting given filter
         conditions.
         @param filters: A dictionary of filter conditions where
                         the key is the column in the DB table and
                         the value is the condition to be met.
         @return: ETLTask objects that meet the conditions.
         """
         q = "SELECT * FROM etl_tasks"
         conditions = []
         for k, v in filters.items():
-            conditions.append(f"{k}={'\''+ v +'\''if type(v)==str else v}")
+            # conditions.append(f"{k}={'\''+ v +'\''if type(v)==str else v}")
+            if type(v)==str: v = f"'{v}'"
+            conditions.append(f"{k}={v}")
         if len(conditions) > 0:
             q = q + " WHERE " + " AND ".join(conditions)
         task_details = self.query(q=q, is_get=True)
         tasks = []
         for td in task_details:
             tasks.append(ETLTask(
                 name=td[0],
```

### Comparing `etl_pipeline_ggn1_ase_g5-3/etl_pipeline_ggn1_ase_g5/etl_task.py` & `etl_pipeline_ggn1_ase_g5-4.0/etl_pipeline_ggn1_ase_g5/etl_task.py`

 * *Files identical despite different names*

### Comparing `etl_pipeline_ggn1_ase_g5-3/etl_pipeline_ggn1_ase_g5/utility.py` & `etl_pipeline_ggn1_ase_g5-4.0/etl_pipeline_ggn1_ase_g5/utility.py`

 * *Files identical despite different names*

