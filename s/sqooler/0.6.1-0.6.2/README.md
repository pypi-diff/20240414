# Comparing `tmp/sqooler-0.6.1.tar.gz` & `tmp/sqooler-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqooler-0.6.1.tar", max compression
+gzip compressed data, was "sqooler-0.6.2.tar", max compression
```

## Comparing `sqooler-0.6.1.tar` & `sqooler-0.6.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1211 2024-03-18 17:38:21.370303 sqooler-0.6.1/LICENSE
--rw-r--r--   0        0        0     3928 2024-03-21 16:38:07.651464 sqooler-0.6.1/README.md
--rw-r--r--   0        0        0     1035 2024-04-03 17:36:13.735396 sqooler-0.6.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-18 17:38:21.374962 sqooler-0.6.1/src/sqooler/__init__.py
--rw-r--r--   0        0        0    12140 2024-04-03 16:25:44.628605 sqooler-0.6.1/src/sqooler/schemes.py
--rw-r--r--   0        0        0     8775 2024-03-29 14:08:39.014572 sqooler-0.6.1/src/sqooler/security.py
--rw-r--r--   0        0        0    27142 2024-04-03 16:25:44.628916 sqooler-0.6.1/src/sqooler/spoolers.py
--rw-r--r--   0        0        0        0 2024-03-21 16:38:07.659018 sqooler-0.6.1/src/sqooler/storage_providers/__init__.py
--rw-r--r--   0        0        0    21471 2024-03-29 14:08:39.015790 sqooler-0.6.1/src/sqooler/storage_providers/base.py
--rw-r--r--   0        0        0    26457 2024-03-29 14:08:39.017351 sqooler-0.6.1/src/sqooler/storage_providers/dropbox.py
--rw-r--r--   0        0        0    22695 2024-03-29 14:08:39.018459 sqooler-0.6.1/src/sqooler/storage_providers/local.py
--rw-r--r--   0        0        0    27073 2024-03-29 14:08:39.019764 sqooler-0.6.1/src/sqooler/storage_providers/mongodb.py
--rw-r--r--   0        0        0     5718 2024-03-29 19:21:38.051011 sqooler-0.6.1/src/sqooler/utils.py
--rw-r--r--   0        0        0     4927 1970-01-01 00:00:00.000000 sqooler-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-03-18 17:38:21.370303 sqooler-0.6.2/LICENSE
+-rw-r--r--   0        0        0     3928 2024-03-21 16:38:07.651464 sqooler-0.6.2/README.md
+-rw-r--r--   0        0        0     1057 2024-04-14 17:29:05.618373 sqooler-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-18 17:38:21.374962 sqooler-0.6.2/src/sqooler/__init__.py
+-rw-r--r--   0        0        0    12140 2024-04-03 16:25:44.628605 sqooler-0.6.2/src/sqooler/schemes.py
+-rw-r--r--   0        0        0     8775 2024-03-29 14:08:39.014572 sqooler-0.6.2/src/sqooler/security.py
+-rw-r--r--   0        0        0    27199 2024-04-14 14:39:47.120255 sqooler-0.6.2/src/sqooler/spoolers.py
+-rw-r--r--   0        0        0        0 2024-03-21 16:38:07.659018 sqooler-0.6.2/src/sqooler/storage_providers/__init__.py
+-rw-r--r--   0        0        0    21846 2024-04-07 17:16:12.295483 sqooler-0.6.2/src/sqooler/storage_providers/base.py
+-rw-r--r--   0        0        0    26455 2024-04-05 16:52:36.004035 sqooler-0.6.2/src/sqooler/storage_providers/dropbox.py
+-rw-r--r--   0        0        0    22693 2024-04-14 14:40:25.633341 sqooler-0.6.2/src/sqooler/storage_providers/local.py
+-rw-r--r--   0        0        0    27299 2024-04-07 17:16:05.334587 sqooler-0.6.2/src/sqooler/storage_providers/mongodb.py
+-rw-r--r--   0        0        0     6472 2024-04-14 14:40:46.943889 sqooler-0.6.2/src/sqooler/utils.py
+-rw-r--r--   0        0        0     4927 1970-01-01 00:00:00.000000 sqooler-0.6.2/PKG-INFO
```

### Comparing `sqooler-0.6.1/LICENSE` & `sqooler-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqooler-0.6.1/README.md` & `sqooler-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `sqooler-0.6.1/pyproject.toml` & `sqooler-0.6.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqooler"
-version = "0.6.1"
+version = "0.6.2"
 description = "Code that enables validated cloud access to quantum hardware (simulators)"
 authors = ["fretchen <fred.jendrzejewski@gmail.com>"]
 repository = "https://github.com/Alqor-UG/sqooler"
 documentation = "https://alqor-ug.github.io/sqooler"
 license = "Unlicense"
 readme = "README.md"
 packages = [{include = "sqooler", from = "src"}]
@@ -24,14 +24,15 @@
 black = "^24.1.1"
 pytest = "^8.0.2"
 pylint = "^3.0.3"
 mypy = "^1.8.0"
 python-decouple = "^3.6"
 ipykernel = "^6.28.0"
 icecream = "^2.1.3"
+pytest-cov = "^5.0.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mike = "^2.0.0"
 mkdocs-material = "^9.1.5"
```

### Comparing `sqooler-0.6.1/src/sqooler/schemes.py` & `sqooler-0.6.2/src/sqooler/schemes.py`

 * *Files identical despite different names*

### Comparing `sqooler-0.6.1/src/sqooler/security.py` & `sqooler-0.6.2/src/sqooler/security.py`

 * *Files identical despite different names*

### Comparing `sqooler-0.6.1/src/sqooler/spoolers.py` & `sqooler-0.6.2/src/sqooler/spoolers.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,14 +127,15 @@
             "simulator": True,
             "supported_instructions": list(self.ins_schema_dict.keys()),
             "num_wires": self.n_wires,
             "wire_order": self.wire_order,
             "num_species": self.num_species,
             "operational": self.operational,
             "display_name": self.display_name,
+            "sign": self.sign,
         }
         return BackendConfigSchemaIn(**backend_config_dict)
 
     def check_instructions(self, ins_list: list) -> tuple[str, bool]:
         """
         Check all the instruction to make sure that they are valid and part
         of the allowed instructions.
@@ -405,17 +406,15 @@
             json_dict: The job dictonary of all the instructions.
             job_id: the id of the the job we are treating.
 
         Returns:
             result_dict: The dictionary with the results of the job.
             status_msg_dict: The status dictionary of the job.
         """
-
         result_dict, status_msg_dict, clean_dict = self._prep_job(json_dict, job_id)
-
         if status_msg_dict.status == "ERROR":
             return result_dict, status_msg_dict
         # now we can generate the circuit for each experiment
         for exp_name, exp_info in clean_dict.items():
             try:
                 result_dict.results.append(self.gen_circuit(exp_name, exp_info))
                 logging.info("Experiment %s done.", exp_name)
@@ -610,23 +609,23 @@
             code = f"Experiment.{inst.name}({inst.wires}, {inst.params})\n"
             # we should add proper error handling here
             # pylint: disable=bare-except
             try:
                 with open(exp_script, "a", encoding="UTF-8") as script_file:
                     script_file.write(code)
             except:
-                print("Something wrong. Does file path exists?")
+                logging.error("Something wrong. Does file path exists?")
 
         code = "Experiment.final_action()" + "\n" + "stop(Experiment.t+0.1)"
         # pylint: disable=bare-except
         try:
             with open(exp_script, "a", encoding="UTF-8") as script_file:
                 script_file.write(code)
         except:
-            print("Something wrong. Does file path exists?")
+            logging.error("Something wrong. Does file path exists?")
         self.remote_client.set_labscript_file(
             exp_script
         )  # CAUTION !! This command only selects the file. It does not generate it!
 
         # be careful. This is not a blocking command
         self.remote_client.engage()
 
@@ -656,15 +655,15 @@
                 # it here.
                 # pylint: disable=W0718
                 try:
                     # append the result to the array
                     shots_array.append(this_run.get_results("/measure", "nat"))
                     got_nat = True
                 except Exception as exc:
-                    print(exc)
+                    logging.exception(exc)
                     sleep(self.labscript_params.t_wait)
                     n_tries += 1
         exp_sub_dict = create_memory_data(shots_array, exp_name, n_shots, ins_list)
         return exp_sub_dict
 
 
 def gate_dict_from_list(inst_list: list) -> GateDict:
```

### Comparing `sqooler-0.6.1/src/sqooler/storage_providers/base.py` & `sqooler-0.6.2/src/sqooler/storage_providers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -402,15 +402,15 @@
         """
         if config_dict.sign:
             # get the private key
             if private_jwk is None:
                 raise ValueError(
                     "The private key is not given, but the backend needs to be signed."
                 )
-            # we should sign the result
+            # we sign the result now
             signed_config = sign_payload(config_dict.model_dump(), private_jwk)
             upload_dict = signed_config.model_dump()
         else:
             upload_dict = config_dict.model_dump()
         return upload_dict
 
     def _format_update_config(
@@ -442,28 +442,35 @@
                 )
             if set(old_config_jws.keys()) == expected_keys_for_jws:
                 # the old config is signed and we need to check if the private key is the same
                 payload = old_config_jws["payload"]
 
                 # now proof that the new private key would create the same signature for the old
                 # config to validate that we still have the same private key
-                test_signature = sign_payload(payload, private_jwk)
+
+                # the following transformation is necessary to make avoid slight differences
+                # in the serialization and then the signing
+                old_config_dict = BackendConfigSchemaIn(**payload)
+                test_signature = sign_payload(old_config_dict.model_dump(), private_jwk)
                 if not test_signature.signature == old_config_jws["signature"]:
                     raise ValueError(
                         "The new private key does not create the same signature as the old one."
                     )
 
             # now that we know that the private key is the same, we can sign the new config
             signed_config = sign_payload(config_dict.model_dump(), private_jwk)
             upload_dict = signed_config.model_dump()
         else:
             # the old and the new are not signed
             upload_dict = config_dict.model_dump()
         return upload_dict
 
+    def _get_default_next_schema_dict(self) -> dict:
+        return {"job_id": "None", "job_json_path": "None"}
+
     def _adapt_get_config(self, config_dict: dict) -> BackendConfigSchemaIn:
         """
         Adapt the config dict to the BackendConfigSchemaIn.
 
         Args:
             config_dict: The dictionary containing the configuration
 
@@ -518,15 +525,15 @@
             None
         """
 
         # first let us get the current configuration
         config_dict = self.get_config(display_name)
 
         # get the current time
-        current_time = datetime.now(timezone.utc)
+        current_time = datetime.now(timezone.utc).replace(microsecond=0)
 
         # update the time stamp
         config_dict.last_queue_check = current_time
 
         # upload the new configuration
         self.update_config(config_dict, display_name, private_jwk)
```

### Comparing `sqooler-0.6.1/src/sqooler/storage_providers/dropbox.py` & `sqooler-0.6.2/src/sqooler/storage_providers/dropbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -665,15 +665,15 @@
             private_jwk: The private JWK to sign the job with
 
 
         Returns:
             the path towards the job
         """
         job_json_dir = "/Backend_files/Queued_Jobs/" + display_name + "/"
-        job_dict = {"job_id": 0, "job_json_path": "None"}
+        job_dict = self._get_default_next_schema_dict()
         job_list = self.get_file_queue(job_json_dir)
 
         # time stamp when we last looked for a job
         self.timestamp_queue(display_name, private_jwk)
 
         # if there is a job, we should move it
         if job_list:
```

### Comparing `sqooler-0.6.1/src/sqooler/storage_providers/local.py` & `sqooler-0.6.2/src/sqooler/storage_providers/local.py`

 * *Files 1% similar despite different names*

```diff
@@ -615,15 +615,15 @@
             display_name: The name of the backend
             private_jwk: The private key of the backend
 
         Returns:
             the dict of the next job
         """
         queue_dir = "jobs/queued/" + display_name
-        job_dict = {"job_id": 0, "job_json_path": "None"}
+        job_dict = self._get_default_next_schema_dict()
         job_list = self.get_file_queue(queue_dir)
 
         # update the time stamp of the last job
         self.timestamp_queue(display_name, private_jwk)
 
         # if there is a job, we should move it
         if job_list:
```

### Comparing `sqooler-0.6.1/src/sqooler/storage_providers/mongodb.py` & `sqooler-0.6.2/src/sqooler/storage_providers/mongodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """
 The module that contains all the necessary logic for communication with the MongoDb storage providers.
 """
 
 import uuid
 from typing import Optional
+from datetime import timezone
 
 # necessary for the mongodb provider
 from pymongo.mongo_client import MongoClient
 from bson.objectid import ObjectId
 from bson.errors import InvalidId
+from bson.codec_options import CodecOptions
 
 from ..schemes import (
     ResultDict,
     StatusMsgDict,
     MongodbLoginInformation,
     BackendStatusSchemaOut,
     BackendConfigSchemaIn,
@@ -239,16 +241,14 @@
         backend_names: list[DisplayNameStr] = []
         for config_dict in config_collection.find():
             config_dict.pop("_id")
             expected_keys_for_jws = {"header", "payload", "signature"}
             if set(config_dict.keys()) == expected_keys_for_jws:
                 backend_names.append(config_dict["payload"]["display_name"])
             else:
-                if not "display_name" in config_dict:
-                    print(config_dict)
                 backend_names.append(config_dict["display_name"])
         return backend_names
 
     def get_backend_status(
         self, display_name: DisplayNameStr
     ) -> BackendStatusSchemaOut:
         """
@@ -353,20 +353,26 @@
 
         # get the database on which we work
         database = self.client["backends"]
 
         # get the collection on which we work
         collection = database["configs"]
 
+        # now make sure that we add the timezone as we open the file
+        collection_with_tz = collection.with_options(
+            codec_options=CodecOptions(tz_aware=True, tzinfo=timezone.utc)
+        )
         # first we have to check if the device already exists in the database
         document_to_find = {"display_name": display_name}
-        result_found = collection.find_one(document_to_find)
+        result_found = collection_with_tz.find_one(document_to_find)
 
         signed_document_to_find = {"payload.display_name": display_name}
-        signed_backend_config_dict = collection.find_one(signed_document_to_find)
+        signed_backend_config_dict = collection_with_tz.find_one(
+            signed_document_to_find
+        )
 
         if result_found:
             old_config_jws = result_found
             job_id = result_found["_id"]
         elif signed_backend_config_dict:
             old_config_jws = signed_backend_config_dict
             job_id = signed_backend_config_dict["_id"]
@@ -723,15 +729,16 @@
             private_jwk: The private JWK to sign the result with
 
         Returns:
             the job dict
         """
 
         queue_dir = "jobs/queued/" + display_name
-        job_dict = {"job_id": 0, "job_json_path": "None"}
+
+        job_dict = self._get_default_next_schema_dict()
         job_list = self.get_file_queue(queue_dir)
 
         # update the time stamp of the last job
         self.timestamp_queue(display_name, private_jwk)
 
         # if there is a job, we should move it
         if job_list:
```

### Comparing `sqooler-0.6.1/src/sqooler/utils.py` & `sqooler-0.6.2/src/sqooler/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 """
 
 import time
 import traceback
 import logging
 
 import regex as re
+from pydantic import ValidationError
 
-from .schemes import get_init_results, get_init_status
+from .schemes import get_init_results, get_init_status, NextJobSchema
 from .spoolers import Spooler
 from .storage_providers.base import StorageProvider
 from .security import public_from_private_jwk
 
 
 def update_backends(
     storage_provider: StorageProvider, backends: dict[str, Spooler]
@@ -74,32 +75,49 @@
     Args:
         storage_provider: The storage provider that should be used.
         backends: A dictionary of all the backends that should be updated.
         num_iter: The number of iterations that should be done. If 0, then the loop
             will run forever.
     """
     backends_list = list(backends.keys())
-
     # set the appropiate display names for all the back-ends
     for requested_backend, spooler in backends.items():
         # the content
         spooler.display_name = requested_backend
 
     counter = 0
     # loop which is looking for the jobs
     while num_iter == 0 or counter < num_iter:
         time.sleep(0.2)
-        logging.info("Running main loop.")
         # the following a fancy for loop of going through all the back-ends in the list
         requested_backend = backends_list[0]
         backends_list.append(backends_list.pop(0))
+
+        spooler = backends[requested_backend]
         # let us first see if jobs are waiting
-        job_dict = storage_provider.get_next_job_in_queue(requested_backend)
+        logging.info("Looking for jobs in %s", requested_backend)
+        if spooler.sign:
+            private_jwk = spooler.get_private_jwk()
+        else:
+            private_jwk = None
+        try:
+            job_dict = storage_provider.get_next_job_in_queue(
+                requested_backend, private_jwk
+            )
+        except ValidationError as val_err:
+            logging.error(
+                "Validation error in job queue.",
+                extra={"error_message": val_err.errors()},
+            )
+            job_dict = NextJobSchema(job_id="None", job_json_path="None")
+
         if job_dict.job_json_path == "None":
+            counter += 1
             continue
+        logging.debug("Got a job in %s", requested_backend)
         job_json_dict = storage_provider.get_job_content(
             storage_path=job_dict.job_json_path, job_id=job_dict.job_id
         )
 
         result_dict = get_init_results()
         # Fix this pylint issue whenever you have time, but be careful !
         # pylint: disable=W0703
@@ -124,16 +142,22 @@
             slimmed_tb = " ".join(tb_list)
             # Update status dict
             status_msg_dict.status = "ERROR"
             status_msg_dict.detail += "; " + slimmed_tb
             status_msg_dict.error_message += "; " + slimmed_tb
             logging.exception("Error in add_job for %s .", requested_backend)
 
+        logging.debug("Updating in database.")
+        spooler.get_private_jwk()
         storage_provider.update_in_database(
-            result_dict, status_msg_dict, job_dict.job_id, requested_backend
+            result_dict,
+            status_msg_dict,
+            job_dict.job_id,
+            requested_backend,
+            private_jwk,
         )
 
         counter += 1
 
 
 def run_json_circuit(json_dict: dict, job_id: str, spooler: Spooler) -> dict:
     """
@@ -147,10 +171,9 @@
     Returns:
         the results dict
     """
 
     result_dict, status_msg_dict = spooler.add_job(json_dict, job_id)
     if not status_msg_dict.status == "DONE":
         logging.error(status_msg_dict.error_message)
-        print(status_msg_dict.error_message)
         raise AssertionError("Job failed")
     return result_dict.model_dump()
```

### Comparing `sqooler-0.6.1/PKG-INFO` & `sqooler-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqooler
-Version: 0.6.1
+Version: 0.6.2
 Summary: Code that enables validated cloud access to quantum hardware (simulators)
 Home-page: https://github.com/Alqor-UG/sqooler
 License: Unlicense
 Keywords: pydantic,quantum-hardware,sdk-python
 Author: fretchen
 Author-email: fred.jendrzejewski@gmail.com
 Requires-Python: >=3.10,<4.0
```

