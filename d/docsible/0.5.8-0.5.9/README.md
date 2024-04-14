# Comparing `tmp/docsible-0.5.8.tar.gz` & `tmp/docsible-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docsible-0.5.8.tar", max compression
+gzip compressed data, was "docsible-0.5.9.tar", max compression
```

## Comparing `docsible-0.5.8.tar` & `docsible-0.5.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1079 2023-09-05 22:49:19.991131 docsible-0.5.8/LICENSE
--rw-r--r--   0        0        0     4043 2024-02-06 18:36:44.373788 docsible-0.5.8/README.md
--rw-r--r--   0        0        0        0 2023-09-05 22:00:43.145585 docsible-0.5.8/docsible/__init__.py
--rw-r--r--   0        0        0     6929 2024-02-06 18:36:44.373788 docsible-0.5.8/docsible/cli.py
--rw-r--r--   0        0        0     5294 2024-02-06 18:36:44.373788 docsible-0.5.8/docsible/markdown_template.py
--rw-r--r--   0        0        0        0 2023-09-11 08:20:14.156264 docsible-0.5.8/docsible/utils/__init__.py
--rw-r--r--   0        0        0     6208 2024-02-06 18:36:44.373788 docsible-0.5.8/docsible/utils/mermaid.py
--rw-r--r--   0        0        0     1823 2024-01-24 19:17:56.690945 docsible-0.5.8/docsible/utils/special_tasks_keys.py
--rw-r--r--   0        0        0     5012 2024-02-06 18:36:44.373788 docsible-0.5.8/docsible/utils/yaml.py
--rw-r--r--   0        0        0      849 2024-02-06 18:36:44.373788 docsible-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     5096 1970-01-01 00:00:00.000000 docsible-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-09-05 22:49:19.991131 docsible-0.5.9/LICENSE
+-rw-r--r--   0        0        0     4043 2024-04-12 18:22:58.929952 docsible-0.5.9/README.md
+-rw-r--r--   0        0        0        0 2023-09-05 22:00:43.145585 docsible-0.5.9/docsible/__init__.py
+-rw-r--r--   0        0        0     6929 2024-04-14 15:01:51.729122 docsible-0.5.9/docsible/cli.py
+-rw-r--r--   0        0        0     5392 2024-04-14 15:01:51.729122 docsible-0.5.9/docsible/markdown_template.py
+-rw-r--r--   0        0        0        0 2023-09-11 08:20:14.156264 docsible-0.5.9/docsible/utils/__init__.py
+-rw-r--r--   0        0        0     6208 2024-02-06 18:36:44.373788 docsible-0.5.9/docsible/utils/mermaid.py
+-rw-r--r--   0        0        0     1823 2024-01-24 19:17:56.690945 docsible-0.5.9/docsible/utils/special_tasks_keys.py
+-rw-r--r--   0        0        0     4644 2024-04-14 15:01:51.729122 docsible-0.5.9/docsible/utils/yaml.py
+-rw-r--r--   0        0        0      849 2024-04-14 15:01:51.729122 docsible-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     5096 1970-01-01 00:00:00.000000 docsible-0.5.9/PKG-INFO
```

### Comparing `docsible-0.5.8/LICENSE` & `docsible-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `docsible-0.5.8/README.md` & `docsible-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `docsible-0.5.8/docsible/cli.py` & `docsible-0.5.9/docsible/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from jinja2 import Environment, BaseLoader
 from docsible.markdown_template import static_template
 from docsible.utils.mermaid import generate_mermaid_playbook, generate_mermaid_role_tasks_per_file
 from docsible.utils.yaml import load_yaml_generic, load_yaml_files_from_dir_custom, get_task_commensts
 from docsible.utils.special_tasks_keys import process_special_task_keys
 
 def get_version():
-    return "0.5.8"
+    return "0.5.9"
 
 # Initialize the Jinja2 Environment
 env = Environment(loader=BaseLoader)
 env.from_string(static_template)
 
 
 def initialize_docsible(docsible_path, default_data):
```

### Comparing `docsible-0.5.8/docsible/markdown_template.py` & `docsible-0.5.9/docsible/markdown_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 {# Cicle used for decide to set Title and Required Column #}
 {% set ns = namespace (details_required = false) %}{% set ns = namespace (details_title = false) %}
 {% for key, details in defaultfile.data.items() %}{% if details.required is not none %}{% set ns.details_required = true %}{% endif %}{% if details.title is not none %}{% set ns.details_title = true %}{% endif %}{% endfor %}
 | Var          | Type         | Value       |{% if ns.details_required %}Required    |{% endif %}{% if ns.details_title %} Title       |{% endif %}
 |--------------|--------------|-------------|{% if ns.details_required %}-------------|{% endif %}{% if ns.details_title %}-------------|{% endif %}
 {%- for key, details in defaultfile.data.items() %}
 {%- set var_type = details.value.__class__.__name__ %}
-| {{ key }}    | {{ var_type }}   | {{ details.value }}  | {% if ns.details_required %} {{ details.required }}  |{% endif %} {% if ns.details_title %} {{ details.title }} |{% endif %}
+| [{{ key }}](defaults/{{ defaultfile.file }}#L{{details.line}})   | {{ var_type }}   | {{ details.value }}  | {% if ns.details_required %} {{ details.required }}  |{% endif %} {% if ns.details_title %} {{ details.title }} |{% endif %}
 {%- endfor %}
 {%- endfor %}
 {%- else %}
 No defaults available.
 {%- endif %}
 
 ### Vars
@@ -54,15 +54,15 @@
 #### File: {{ varsfile.file }}
 {# Cicle used for decide to set Title and Required Column #}
 {% set ns = namespace (details_required = false) %}{% set ns = namespace (details_title = false) %}{% for key, details in varsfile.data.items() %}{% if details.required is not none %}{% set ns.details_required = true %}{% endif %}{% if details.title is not none %}{% set ns.details_title = true %}{% endif %}{% endfor %}
 | Var          | Type         | Value       |{% if ns.details_required %} Required    |{% endif %}{% if ns.details_title %} Title       |{% endif %}
 |--------------|--------------|-------------|{% if ns.details_required %}-------------|{% endif %}{% if ns.details_title %}-------------|{% endif %}
 {%- for key, details in varsfile.data.items() %}
 {%- set var_type = details.value.__class__.__name__ %}
-| {{ key }}    | {{ var_type }}   | {{ details.value }}  |{% if ns.details_required %} {{ details.required }} |{% endif %}{% if ns.details_title %} {{ details.title }} |{% endif %}
+| [{{ key }}](vars/{{ varsfile.file }}#L{{details.line}})    | {{ var_type }}   | {{ details.value }}  |{% if ns.details_required %} {{ details.required }} |{% endif %}{% if ns.details_title %} {{ details.title }} |{% endif %}
 {%- endfor %}
 {%- endfor %}
 {%- else %}
 No vars available.
 {%- endif %}
```

### Comparing `docsible-0.5.8/docsible/utils/mermaid.py` & `docsible-0.5.9/docsible/utils/mermaid.py`

 * *Files identical despite different names*

### Comparing `docsible-0.5.8/docsible/utils/special_tasks_keys.py` & `docsible-0.5.9/docsible/utils/special_tasks_keys.py`

 * *Files identical despite different names*

### Comparing `docsible-0.5.8/pyproject.toml` & `docsible-0.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docsible"
-version = "0.5.8"
+version = "0.5.9"
 description = "Document generator for ansible role"
 authors = ["Lucian BLETAN <neuraluc@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
```

### Comparing `docsible-0.5.8/PKG-INFO` & `docsible-0.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docsible
-Version: 0.5.8
+Version: 0.5.9
 Summary: Document generator for ansible role
 License: MIT
 Author: Lucian BLETAN
 Author-email: neuraluc@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

