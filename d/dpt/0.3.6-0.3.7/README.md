# Comparing `tmp/dpt-0.3.6.tar.gz` & `tmp/dpt-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpt-0.3.6.tar", last modified: Sun Feb 18 20:22:04 2024, max compression
+gzip compressed data, was "dpt-0.3.7.tar", last modified: Sun Apr 14 14:31:47 2024, max compression
```

## Comparing `dpt-0.3.6.tar` & `dpt-0.3.7.tar`

### file list

```diff
@@ -1,26 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-02-18 20:22:04.345521 dpt-0.3.6/
--rw-rw-rw-   0        0        0      188 2024-02-18 20:22:04.344521 dpt-0.3.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-02-18 20:22:04.323812 dpt-0.3.6/dpt/
--rw-rw-rw-   0        0        0      155 2024-02-16 20:18:31.000000 dpt-0.3.6/dpt/__init__.py
--rw-rw-rw-   0        0        0     1515 2024-02-18 20:17:03.000000 dpt-0.3.6/dpt/api.py
-drwxrwxrwx   0        0        0        0 2024-02-18 20:22:04.339520 dpt-0.3.6/dpt/deployment/
--rw-rw-rw-   0        0        0        4 2024-02-01 03:57:26.000000 dpt-0.3.6/dpt/deployment/__init__.py
--rw-rw-rw-   0        0        0      110 2024-02-01 20:25:45.000000 dpt-0.3.6/dpt/deployment/common.py
--rw-rw-rw-   0        0        0     9076 2024-02-03 03:11:15.000000 dpt-0.3.6/dpt/deployment/deploy.py
--rw-rw-rw-   0        0        0     1054 2024-02-01 20:24:35.000000 dpt-0.3.6/dpt/deployment/extract.py
--rw-rw-rw-   0        0        0     1981 2024-02-01 20:24:46.000000 dpt-0.3.6/dpt/management.py
-drwxrwxrwx   0        0        0        0 2024-02-18 20:22:04.343520 dpt-0.3.6/dpt/mongo/
--rw-rw-rw-   0        0        0        4 2024-02-01 03:59:35.000000 dpt-0.3.6/dpt/mongo/__init__.py
--rw-rw-rw-   0        0        0      266 2024-01-27 22:13:49.000000 dpt-0.3.6/dpt/mongo/commands.py
--rw-rw-rw-   0        0        0     1032 2024-01-28 00:52:12.000000 dpt-0.3.6/dpt/mongo/files.py
--rw-rw-rw-   0        0        0    18970 2024-02-17 16:26:23.000000 dpt-0.3.6/dpt/processor.py
--rw-rw-rw-   0        0        0     4279 2024-02-07 13:01:49.000000 dpt-0.3.6/dpt/storage.py
--rw-rw-rw-   0        0        0     4353 2024-02-17 21:06:03.000000 dpt-0.3.6/dpt/workflow_graph.py
-drwxrwxrwx   0        0        0        0 2024-02-18 20:22:04.335521 dpt-0.3.6/dpt.egg-info/
--rw-rw-rw-   0        0        0      188 2024-02-18 20:22:04.000000 dpt-0.3.6/dpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      407 2024-02-18 20:22:04.000000 dpt-0.3.6/dpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-18 20:22:04.000000 dpt-0.3.6/dpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2024-02-18 20:22:04.000000 dpt-0.3.6/dpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-02-18 20:22:04.000000 dpt-0.3.6/dpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-18 20:22:04.345521 dpt-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0      529 2024-02-18 20:21:30.000000 dpt-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 14:31:47.789672 dpt-0.3.7/
+-rw-rw-rw-   0        0        0      188 2024-04-14 14:31:47.788671 dpt-0.3.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-14 14:31:47.759775 dpt-0.3.7/dpt/
+-rw-rw-rw-   0        0        0      123 2024-03-05 23:00:59.000000 dpt-0.3.7/dpt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 14:31:47.783671 dpt-0.3.7/dpt/deployment/
+-rw-rw-rw-   0        0        0        4 2024-02-01 03:57:26.000000 dpt-0.3.7/dpt/deployment/__init__.py
+-rw-rw-rw-   0        0        0      110 2024-02-01 20:25:45.000000 dpt-0.3.7/dpt/deployment/common.py
+-rw-rw-rw-   0        0        0     9457 2024-04-07 23:03:50.000000 dpt-0.3.7/dpt/deployment/deploy.py
+-rw-rw-rw-   0        0        0     1054 2024-02-01 20:24:35.000000 dpt-0.3.7/dpt/deployment/extract.py
+-rw-rw-rw-   0        0        0     1981 2024-02-01 20:24:46.000000 dpt-0.3.7/dpt/management.py
+drwxrwxrwx   0        0        0        0 2024-04-14 14:31:47.786671 dpt-0.3.7/dpt/mongo/
+-rw-rw-rw-   0        0        0        4 2024-02-01 03:59:35.000000 dpt-0.3.7/dpt/mongo/__init__.py
+-rw-rw-rw-   0        0        0      266 2024-01-27 22:13:49.000000 dpt-0.3.7/dpt/mongo/commands.py
+-rw-rw-rw-   0        0        0     1032 2024-01-28 00:52:12.000000 dpt-0.3.7/dpt/mongo/files.py
+-rw-rw-rw-   0        0        0    13237 2024-04-12 03:20:41.000000 dpt-0.3.7/dpt/processor.py
+-rw-rw-rw-   0        0        0     5729 2024-04-12 03:20:41.000000 dpt-0.3.7/dpt/storage.py
+drwxrwxrwx   0        0        0        0 2024-04-14 14:31:47.776674 dpt-0.3.7/dpt.egg-info/
+-rw-rw-rw-   0        0        0      188 2024-04-14 14:31:47.000000 dpt-0.3.7/dpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2024-04-14 14:31:47.000000 dpt-0.3.7/dpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 14:31:47.000000 dpt-0.3.7/dpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-04-14 14:31:47.000000 dpt-0.3.7/dpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-14 14:31:47.000000 dpt-0.3.7/dpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 14:31:47.789672 dpt-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      338 2024-04-14 14:31:41.000000 dpt-0.3.7/setup.py
```

### Comparing `dpt-0.3.6/dpt/deployment/deploy.py` & `dpt-0.3.7/dpt/deployment/deploy.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,41 +84,48 @@
         }
     )
     upsert_one_with_timestamp(
         collection,
         filter,
         fields,
     )
-    _update_modules_info(db, project, temp_path)
+    _update_modules_info(db, project, temp_path, version_info)
     _update_processors_info(db, project, temp_path, version_info)
     client.close()
     _logger.info(f"Upload project: success")
     _logger.info(f"- {fields}")
 
 
-def _normalize_def_in_file(info: dict, root_path):
-    info["defined_in_file"] = (
-        os.path.relpath(info["defined_in_file"], start=root_path)
+def _normalize_def_in_file(info: dict, root_path, version_info):
+
+    # info["defined_in_file"] = (
+    #     os.path.relpath(info["defined_in_file"], start=root_path)
+    #     .replace("\\", "/")
+    #     .replace("../", "")
+    # )
+    path = (
+        os.path.relpath(info["defined_in_file"], start=version_info["git_dir"])
         .replace("\\", "/")
         .replace("../", "")
     )
+    info["defined_in_file"] = path
 
 
-def _update_modules_info(db: Database, project: Project, temp_path: str):
+def _update_modules_info(db: Database, project: Project, temp_path: str, version_info):
     collection = db[f"{coll_prefix}module"]
     info_list = []
     for module in project.modules.values():
         info = _dict_from_obj(module)
         info.update(
             {
                 "workspace": common.workspace_name,
                 "project": project.name,
             }
         )
-        _normalize_def_in_file(info, temp_path)
+        _normalize_def_in_file(info, temp_path, version_info)
         info_list.append(info)
 
     collection.delete_many(
         {
             "project": project.name,
             "workspace": common.workspace_name,
         }
@@ -136,24 +143,28 @@
             info = _dict_from_obj(processor)
 
             info.update(
                 {
                     "workspace": common.workspace_name,
                     "project": project.name,
                     "module": module.name,
-                    "source_link": f"http://gl.astu.lan/dpt/dpt-python/-/blob/main/configuration/{processor.defined_in_file}",
                 }
             )
 
-            _normalize_def_in_file(info, temp_path)
+            _normalize_def_in_file(info, temp_path, version_info)
             if version_info != None:
                 repo: str = version_info["repository"]
                 repo = repo.rstrip(".git")
-                # todo упустил часть пути, /configuration доработать _normalize_def_in_file
-                link = f"{repo}/-/blob/{version_info['branch']}/configuration/{info['defined_in_file']}"
+
+                repo_root = "http://gl.astu.lan/"
+                repo_without_root = repo.replace(repo_root, "")
+
+                # TODO усовершенствовать алгоритм определения ссылки вынести в настройки частично
+                link = f"{repo_root}-/ide/project/{repo_without_root}/edit/{version_info['branch']}/-/{info['defined_in_file']}"
+
                 info.update(
                     {
                         "source_link": link,
                     }
                 )
 
             def make_port_info(ports: dict[str, Port]):
@@ -186,14 +197,15 @@
 
         repo = git.Repo(search_parent_directories=True)
         version_info = {
             "repository": repo.remotes.origin.url,
             "branch": repo.active_branch.name,
             "commit": repo.head.commit.hexsha,
             "is_dirty": bool(repo.is_dirty()),
+            "git_dir": repo.git_dir,
         }
     except:
         _logger.info("Get version info: git repository not found")  # todo не проверено
         return None
     if version_info != None:
         _logger.info("Get version info: success")
         _logger.info(version_info)
```

### Comparing `dpt-0.3.6/dpt/deployment/extract.py` & `dpt-0.3.7/dpt/deployment/extract.py`

 * *Files identical despite different names*

### Comparing `dpt-0.3.6/dpt/management.py` & `dpt-0.3.7/dpt/management.py`

 * *Files identical despite different names*

### Comparing `dpt-0.3.6/dpt/mongo/files.py` & `dpt-0.3.7/dpt/mongo/files.py`

 * *Files identical despite different names*

### Comparing `dpt-0.3.6/dpt/processor.py` & `dpt-0.3.7/dpt/processor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from __future__ import annotations
 import enum
 import os
 from types import ModuleType
 from typing import Any, Callable, TYPE_CHECKING, List, Union
-
-# from dpt.workflow_graph import WorkflowInfo, WorkflowTaskInfo
 from .storage import (
     DatabaseInfo,
     ConnectionInfo,
     DbReader,
     DbWriter,
     MemoryReader,
     MemoryWriter,
@@ -49,24 +47,14 @@
             raise Exception(f"module '{name}' is not defined")
         return self.modules[name]
 
     def add_modules(self, modules: list[Module]):
         for item in modules:
             self.add_module(item)
 
-    def get_processor(
-        self, module_info: str | ModuleType, processor_info: str | ModuleType
-    ):
-        return self.get_module(module_info).get_processor(processor_info)
-
-    def create_task(
-        self, module_info: str | ModuleType, processor_info: str | ModuleType
-    ):
-        return self.get_processor(module_info, processor_info).create_task()
-
 
 class Port:
     def __init__(
         self,
         name: str,
         title: str = None,
         description: str = None,
@@ -78,35 +66,47 @@
         self.title = title
         self.description = description
         self.default_binding = default_binding
         self.read_only = read_only
         self.schema = schema
 
 
+def _default_action(params: Task):
+    print(f"Processor {params.processor.name} has no action defined")
+
+
 def _get_source_file_name():
     caller_frame = inspect.stack()[2]
     return (
         caller_frame.filename
         # .replace(os.getcwd(), "")
         .replace("\\", "/")
         # .rstrip("/")[1:]
     )
 
 
-def _get_name_from_path(path):
+def _get_module_name_from_path(path: str):
+    # TODO усовершенствовать убрать хардкод
+    rel_path = path.split("processors/")[1].lower()
+    rel_path = rel_path.replace("/__init__.py", "").replace(".py", "")
+    rel_path = rel_path.replace("/", ".")
+    return rel_path
+
+
+def _get_processor_name_from_path(path):
     return path.rsplit("/", 1)[-1].split(".", 1)[0]
 
 
 class Module:
     project: Project
 
     def __init__(self, name: str = None):
         self.defined_in_file = _get_source_file_name()
         if name == None:
-            name = _get_name_from_path(self.defined_in_file)
+            name = _get_module_name_from_path(self.defined_in_file)
         self.name = name
         self.processors = dict[str, Processor]()
         self.project = None
 
     def add_processor(self, processor: Processor):
         if processor.name in self.processors:
             raise Exception(f"duplicated processor name '{processor.name}'")
@@ -129,33 +129,26 @@
 
     def create_task(self, processor_info: str | ModuleType):
         return self.get_processor(processor_info).create_task()
 
 
 class Processor:
     module: Module
-    _workflow_builder: Callable[[Workflow], None]
-    _workflow: Workflow
 
     def __init__(self, title: str = None, description: str = None, name: str = None):
-        def default_action(params: Task):
-            print(f"Processor {params.processor.name} has no action defined")
-
         self.defined_in_file = _get_source_file_name()
         if name == None:
-            name = _get_name_from_path(self.defined_in_file)
+            name = _get_processor_name_from_path(self.defined_in_file)
         self.name = name
         self.title = title
         self.description = description
         self.inputs = dict[str, Port]()
         self.outputs = dict[str, Port]()
-        self.action = default_action
+        self.action = _default_action
         self.module = None
-        self._workflow_builder = None
-        self._workflow = None
 
     def add_named_input(
         self,
         name: str,
         title: str = None,
         description: str = None,
         schema: dict[str, Any] = None,
@@ -213,146 +206,72 @@
             "default", title, description, schema, default_binding, read_only
         )
 
     def set_action(self, action: Callable[[str], None]):
         self.action = action
 
     def create_task(self) -> Task:
-        self._build_workflow_if_need()
         return Task(self)
 
-    def get_workflow(self) -> Workflow:
-        self._build_workflow_if_need()
-        return self._workflow
-
-    def set_workflow_builder(self, workflow_builder_func: Callable[[Workflow], None]):
-        self._workflow_builder = workflow_builder_func
-
-    def _build_workflow_if_need(self):
-        if self._workflow_builder == None:
-            return
-        if self._workflow == None:
-            self._workflow = Workflow(self)
-            self._workflow_builder(self._workflow)
-
 
 class Task:
     _database: DatabaseInfo
-    _workflow: Workflow
-    _title: str
 
     def __init__(self, processor: Processor):
         self.processor = processor
         self._input_binding = dict[str, str | list[dict[str, Any]] | dict[str, Any]]()
         self._output_binding = dict[str, str | str | list[dict[str, Any]]]()
         self._writers = dict[str, DbWriter | MemoryWriter]()
         self._readers = dict[str, DbReader | MemoryReader]()
         self._database = None
-        self._name = None
-        self._workflow = None
-        self._title = None
-        self._input_refs = dict[TaskInputRef]()
-        self._output_refs = dict[TaskOutputRef]()
 
     # Config
 
-    def set_name(self, name: str):
-        if self._workflow != None:
-            self._workflow._rename_task(self._name, name)
-        self._name = name
-
-    def get_name(self):
-        return self._name or self.processor.name
-
-    def set_title(self, value: str):
-        self._title = value
-
-    def get_title(self):
-        return self._title or self.processor.title
-
     def _remove_input_binging(self, name: str):
         if name in self._input_binding:
             del self._input_binding[name]
 
     def _remove_output_binging(self, name: str):
         if name in self._output_binding:
             del self._output_binding[name]
 
     def bind_named_input(
-        self,
-        input_name: str,
-        source: list[dict[str, Any]] | dict[str, Any] | str | TaskOutputRef,
+        self, input_name: str, source: list[dict[str, Any]] | dict[str, Any] | str
     ):
         self._remove_input_binging(input_name)
         if not input_name in self.processor.inputs:
             raise Exception(f"Input '{input_name}' is not declared")
         if isinstance(source, list):
             source = source.copy()
-        elif isinstance(source, TaskOutputRef):
-            # обратная связь
-            self._input_binding[input_name] = source
-            if source.task._output_binding.get(source.name) != self.get_named_input(
-                input_name
-            ):
-                source.task.bind_named_output(
-                    source.name, self.get_named_input(input_name)
-                )
-        elif not isinstance(source, (dict, str)):
-            raise Exception(
-                f"Incorrect binding for input '{self.get_name()}.{input_name}', bound value: {source}"
-            )
         self._input_binding[input_name] = source
 
-    def bind_named_output(
-        self, output_name: str, target: list[dict[str, Any]] | str | TaskInputRef
-    ):
+    def bind_named_output(self, output_name: str, target: list[dict[str, Any]] | str):
         self._remove_output_binging(output_name)
         if not output_name in self.processor.outputs:
             raise Exception(f"Output '{output_name}' is not declared")
-
-        if isinstance(target, TaskInputRef):
-            self._output_binding[output_name] = target
-            # обратная связь
-            if target.task._input_binding.get(target.name) != self.get_named_output(
-                output_name
-            ):
-                target.task.bind_named_input(
-                    target.name, self.get_named_output(output_name)
-                )
-        elif not isinstance(target, (list, str)):
-            raise Exception(
-                f"Incorrect binding for output '{self.get_name()}.{output_name}', bound value: {target}"
-            )
-
         self._output_binding[output_name] = target
 
-    def bind_params(
-        self, source: list[dict[str, Any]] | dict[str, Any] | str | TaskOutputRef
-    ):
+    def bind_params(self, source: list[dict[str, Any]] | dict[str, Any] | str):
         self.bind_named_input("params", source)
 
-    def bind_input(
-        self, source: list[dict[str, Any]] | dict[str, Any] | str | TaskOutputRef
-    ):
+    def bind_input(self, source: list[dict[str, Any]] | dict[str, Any] | str):
         self.bind_named_input("default", source)
 
-    def bind_output(self, target: list[dict[str, Any]] | str | TaskInputRef):
+    def bind_output(self, target: list[dict[str, Any]] | str):
         self.bind_named_output("default", target)
 
     def bind_inputs(
         self,
-        input_bindings: dict[
-            str, Union[str, List[dict[str, Any]], dict[str, Any], TaskOutputRef]
-        ],
+        input_bindings: dict[str, Union[str, List[dict[str, Any]], dict[str, Any]]],
     ):
         for name in input_bindings:
             self.bind_named_input(name, input_bindings[name])
 
     def bind_outputs(
-        self, output_bindings: dict[str, Union[str, List[dict[str, Any]], TaskInputRef]]
+        self, output_bindings: dict[str, Union[str, List[dict[str, Any]]]]
     ):
         for name in output_bindings:
             self.bind_named_output(name, output_bindings[name])
 
     def _print_bindings(self, ports: dict, bindings: dict):
         for name in ports:
             val = None
@@ -365,40 +284,25 @@
                 text = val
             elif isinstance(val, dict):
                 text = str(val)
             else:
                 text = "list[]"
             print("- " + name + ": " + text)
 
-    # todo Перемудрил в попытке сделать универсально для входов и выходов, переделать при случае. Возможно свести входы и выходы в единый массив
-    def _get_port_binging(self, port_type, port_name):
-        if port_type == "input":
-            ports = self.processor.inputs
-            bindings = self._input_binding
-        else:
-            ports = self.processor.outputs
-            bindings = self._output_binding
-
-        port = ports[port_name]
-        if port_name in bindings:
-            binding = bindings[port_name]
-        else:
-            if port.default_binding != None:
-                binding = port.default_binding
-            else:
-                raise Exception(
-                    f"Processor '{self.processor.name}' {port_type} port '{port_name}' is not bound"
-                )
-        return binding
-
-    def apply_default_binding(self):
+    def _apply_default_binding(self):
         def apply(ports: dict[str, Port], bindings: dict, type: str):
             for name in ports:
                 if name not in bindings:
-                    bindings[name] = self._get_port_binging(type, name)
+                    port = ports[name]
+                    if port.default_binding != None:
+                        bindings[name] = port.default_binding
+                    else:
+                        raise Exception(
+                            f"Processor '{self.processor.name}' {type} port '{name}' is not bound"
+                        )
 
             for name in bindings:
                 if name not in ports:
                     raise Exception(
                         f"Invalid binding. Processor '{self.processor.name}' does not contain {type} '{name}'"
                     )
 
@@ -408,15 +312,15 @@
     def get_input_binding_info(self):
         return self._input_binding.copy()
 
     def get_output_binding_info(self):
         return self._output_binding.copy()
 
     def prepare(self):
-        self.apply_default_binding()
+        self._apply_default_binding()
 
     def run(self):
         print("")
         print(f"Start processor '{self.processor.name}' task")
         self.prepare()
         print("input binding")
         self._print_bindings(self.processor.inputs, self._input_binding)
@@ -486,86 +390,12 @@
 
     def get_params_reader(self) -> DbReader | MemoryReader:
         return self.get_named_reader("params")
 
     def get_writer(self) -> DbWriter:
         return self.get_named_writer("default")
 
-    # workflow
-
-    def get_output(self):
-        return self.get_named_output("default")
 
-    def get_input(self):
-        return self.get_named_input("default")
-
-    def get_named_output(self, name):
-        if not name in self.processor.outputs:
-            raise Exception(f"Output '{self.get_name()}.{name}' is not declared")
-        if name not in self._output_refs:
-            self._output_refs[name] = TaskOutputRef(self, name)
-        return self._output_refs[name]
-
-    def get_named_input(self, name):
-        if not name in self.processor.inputs:
-            raise Exception(f"Input '{self.get_name()}.{name}' is not declared")
-        if name not in self._input_refs:
-            self._input_refs[name] = TaskInputRef(self, name)
-        return self._input_refs[name]
-
-    # def to_model(self) -> WorkflowTaskInfo:
-    #     model = WorkflowTaskInfo(
-    #         name=self.get_name(),
-    #         module=self.processor.module.name,
-    #         processor=self.processor.name,
-    #         title=self.get_title(),
-    #     )
-    #     return model
-
-
-class TaskOutputRef:
-    def __init__(self, task: Task, name: str):
-        self.task = task
-        self.name = name
-
-
-class TaskInputRef:
-    def __init__(self, task: Task, name: str):
-        self.task = task
-        self.name = name
-
-
-class Workflow:
-    tasks = dict[str, Task]
-
-    def __init__(self, processor: Processor):
-        self.processor = processor
-        self.tasks = dict[str, Task]()
-
-    def create_task(
-        self, module_info: str | ModuleType, processor_info: str | ModuleType
-    ):
-        task = self.processor.module.project.create_task(module_info, processor_info)
-        task_name = task.processor.name
-        i = 1
-        while task_name in self.tasks:
-            i += 1
-            task_name = task.processor.name + f"_{i}"
-        task._name = task_name
-        self.tasks[task_name] = task
-
-        return task
-
-    def _rename_task(self, old_name, new_name):
-        if new_name in self.tasks:
-            raise Exception(
-                f"duplicated task name '{new_name}' in processor '{self.processor.name}' workflow"
-            )
-        task = self.tasks.pop(old_name)
-        self.tasks[new_name] = task
-
-    # def to_model(self) -> WorkflowInfo:
-    #     model = WorkflowInfo()
-    #     for name in self._tasks:
-    #         task_model = self._tasks[name].to_model()
-    #         model.tasks.append(task_model)
-    #     return model
+# class TaskContext:
+#     def __init__(self, task: Task):
+#         self.task = task
+#         self._writers = dict[str, DbWriter | MemoryWriter]()
```

