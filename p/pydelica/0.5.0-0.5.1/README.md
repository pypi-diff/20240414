# Comparing `tmp/pydelica-0.5.0.tar.gz` & `tmp/pydelica-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydelica-0.5.0.tar", max compression
+gzip compressed data, was "pydelica-0.5.1.tar", max compression
```

## Comparing `pydelica-0.5.0.tar` & `pydelica-0.5.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1085 2022-08-04 06:40:59.808129 pydelica-0.5.0/LICENSE
--rw-r--r--   0        0        0     7619 2022-08-04 06:40:59.808129 pydelica-0.5.0/README.md
--rw-r--r--   0        0        0    21965 2023-10-03 07:53:10.341319 pydelica-0.5.0/pydelica/__init__.py
--rw-r--r--   0        0        0    12374 2023-10-03 07:53:10.341319 pydelica-0.5.0/pydelica/compiler.py
--rw-r--r--   0        0        0     3029 2022-08-04 06:40:59.808129 pydelica-0.5.0/pydelica/exception.py
--rw-r--r--   0        0        0      319 2022-08-04 06:40:59.808129 pydelica-0.5.0/pydelica/logger.py
--rw-r--r--   0        0        0     5659 2022-08-04 06:40:59.808129 pydelica-0.5.0/pydelica/model.py
--rw-r--r--   0        0        0     8512 2023-10-03 07:53:10.341319 pydelica-0.5.0/pydelica/options.py
--rw-r--r--   0        0        0     1685 2022-08-04 06:40:59.808129 pydelica-0.5.0/pydelica/solutions.py
--rw-r--r--   0        0        0      937 2024-01-03 08:45:26.856757 pydelica-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     8654 1970-01-01 00:00:00.000000 pydelica-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-02-06 18:54:01.314679 pydelica-0.5.1/LICENSE
+-rw-r--r--   0        0        0    22030 2024-03-02 14:35:33.838136 pydelica-0.5.1/pydelica/__init__.py
+-rw-r--r--   0        0        0    12374 2024-02-06 18:54:01.317684 pydelica-0.5.1/pydelica/compiler.py
+-rw-r--r--   0        0        0     3324 2024-04-14 08:05:31.229243 pydelica-0.5.1/pydelica/exception.py
+-rw-r--r--   0        0        0      319 2024-02-06 18:54:01.318686 pydelica-0.5.1/pydelica/logger.py
+-rw-r--r--   0        0        0     5659 2024-02-06 18:54:01.318686 pydelica-0.5.1/pydelica/model.py
+-rw-r--r--   0        0        0     8603 2024-03-02 14:34:49.787536 pydelica-0.5.1/pydelica/options.py
+-rw-r--r--   0        0        0     1685 2024-02-06 18:54:01.320064 pydelica-0.5.1/pydelica/solutions.py
+-rw-r--r--   0        0        0      937 2024-03-02 14:37:34.394230 pydelica-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     9196 2024-04-14 08:20:31.870965 pydelica-0.5.1/README.md
+-rw-r--r--   0        0        0    10231 1970-01-01 00:00:00.000000 pydelica-0.5.1/PKG-INFO
```

### Comparing `pydelica-0.5.0/LICENSE` & `pydelica-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydelica-0.5.0/README.md` & `pydelica-0.5.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+<p align="center">
+<img src="https://gitlab.com/krizar/pydelica/-/raw/main/media/pyd_logo.svg", width="200">
+</p>
+
 # PyDelica: Serverless OpenModelica with Python
 
 ## About
 
 PyDelica is an API providing a quick and easy to use interface to compile, customise and run OpenModelica models with Python. Unlike OMPython it does not require the launch of a server session to use OMShell but rather dynamically adjusts files produced after model compilation in order to update options and parameters. The lack of server requirement means models can be run in tandem without calling multiple OMC sessions which can be very taxing on CPU. Furthermore PyDelica is able to detect errors during model runs by reading the `stderr` and `stdout` from OpenModelica and throw appropriate exceptions to terminate the program execution.
 
 ## Installation
@@ -57,20 +61,47 @@
 session.build_model(model_path, 'M.A')
 ```
 
 The `build_model` function also allows you to specify additional flags/options to hand to the OMC compiler, these are given
 in the form of a dictionary where the value can be `None` if the flag does not take any input. You can also directly set the profiling level for profiling the Modelica code. When set, the profile dictionary is also stored in the session after the simulation and is accessible via the `code_profile` and `code_info` attributes:
 
 ```python
-session.build_model(model_path, 'M.A', profiling="all", omc_build_flags={"-g": "MetaModelica"})
+session.build_model(
+    model_path,
+    model_addr='M.A'
+    profiling="all",
+    omc_build_flags={"-g": "MetaModelica"}
+)
 session.simulate()
 print(session.code_profile)
 print(session.code_info)
 ```
 
+#### Specifying Additional Model-Based Dependencies
+
+If additional model files are required to execute the main model these can be specified with the `extra_models` argument:
+
+```python
+session.build_model(
+    model_path,
+    extra_models=["extra_model.mo"]
+)
+```
+
+#### Using Alternative Inputs Location
+
+If your model inputs are stored in an alternative directory, this can be specified with the `update_input_paths_to` argument:
+
+```python
+session.build_model(
+    model_path,
+    update_input_paths_to="/path/to/inputs"
+)
+```
+
 #### Examining Parameters and Options
 We can examine all parameters for a given model using the `get_parameters` method which will return a Python dictionary:
 
 ```python
 session.get_parameters('SineCurrentModel')
 ```
 
@@ -140,16 +171,16 @@
 Possible values ranked by order (highest at the top):
 
 |**Value**|**Description**|
 |---|---|
 |`'never'`|Do not throw an exception on Modelica assertion violation|
 |`'error'`|Default. Throw an exception on an assertion of level `AssertionLevel.error`|
 |`'warning'`|Throw an exception on assertion of level `AssertionLevel.warning`|
-|`'info'`|Throw an exception on any `assert | info` statement|
-|`'debug'`|Throw an exception on any `assert | debug` statement|
+|`'info'`|Throw an exception on any `assert \| info` statement|
+|`'debug'`|Throw an exception on any `assert \| debug` statement|
 
 #### Running the Simulation
 To run the simulation use the `simulate` method. If a model name is specified then that model is run,
 else this is the first model in the model list. At the simulation step parameter values are written to the
 XML file read by the binary before the model binary is executed.
 
 ```python
@@ -167,29 +198,62 @@
 The variables for each model are stored as a Pandas dataframe.
 
 #### Using Alternative Libraries
 
 **NOTE:** Currently only works in WSL on Windows machines.
 
 You can use an alternative library version via the `use_library` method:
-```python3
+```python
 session.use_library("Modelica", "3.2.3")
 ```
 you can also optionally specify the location of this library:
-```python3
+```python
 session.use_library("Modelica", "3.2.3", library_directory="/home/user/my_om_libraries")
 ```
 
+#### Including Extra C Resources
+
+When building a model extra C file resources can be specified using the `c_source_dir` argument to `build_model`:
+
+```python
+session.build_model(
+    model_path,
+    c_source_dir=os.path.join(model_dir, "Resources", "Include")
+)
+```
+
+## Docker
+
+A Docker image is available for OpenModelica with Pydelica:
+
+```sh
+$ docker pull artemisbeta/pydelica
+```
+
+You can try out Pydelica within a Jupyter notebook by running:
+
+```sh
+$ docker run -ti artemisbeta/pydelica jupyter notebook --ip 0.0.0.0 --no-browser
+```
+
+and opening the resulting URL within your browser.
+
 ## Troubleshooting
 
 ### Simulation fails with no error thrown
 Try setting the assertion level to a lower level, for some reason OM ranks missing input file errors
 as type `debug`, see [here](#failing-simulation-on-lower-assertion-level).
 
 ```
 stdout | info | ... loading "data" from "Default/myInput.mat"
 assert | debug | Not possible to open file "Default/myInput.mat": No such file or directory
 assert | info | simulation terminated by an assertion at initialization
 ```
 
 ### PyDelica cannot find OMC
 PyDelica relies on either locating OMC on UNIX using the `which` command, or in the case of Windows using the `OPENMODELICAHOME` environment variable. Ensure at least one of these is available after installating OpenModelica.
+
+## Use Cases
+
+_Pydelica_ is currently being used in the following projects, if you would like to be included in this list please open an issue:
+
+* [_Power Balance Models_](https://github.com/ukaea/powerbalance), _United Kingdom Atomic Energy Authority_: A tokamak power balance model with Python API and CLI
```

### Comparing `pydelica-0.5.0/pydelica/__init__.py` & `pydelica-0.5.1/pydelica/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import pandas
 
 import pydelica.exception as pde
 from pydelica.compiler import Compiler
 from pydelica.logger import OMLogLevel
 from pydelica.model import Model
-from pydelica.options import SimulationOptions, Solver
+from pydelica.options import SimulationOptions, Solver, OutputFormat
 from pydelica.solutions import SolutionHandler
 
 
 class Session:
     def __init__(self, log_level: OMLogLevel = OMLogLevel.NORMAL) -> None:
         """Session object which handles model runs.
 
@@ -228,15 +228,15 @@
             # Option to update any variable recognised as an input
             # i.e. .mat/.csv to point to the correct location as an
             # absolute path
             if update_input_paths_to:
                 self._set_input_files_directory(_model_name, update_input_paths_to)
 
             # Allows easy creation of a Pandas dataframe for displaying solutions
-            self._set_output_to_csv()
+            self.set_output_format(OutputFormat.CSV)
 
     def _get_cache_key(self, model_name: str, member_dict: typing.Dict) -> str:
         """Retrieve Model Name in cache dictionary
 
         Retrieves model name as stored within the given dictionary. In some versions of OM
         '.' in the model name is replaced by '_' in the files.
         """
@@ -501,17 +501,17 @@
 
         for path in _required:
             if path not in _path_entries:
                 _path_entries.append(path)
 
         _env["PATH"] = f"{_separator}".join(_path_entries)
 
-    def _set_output_to_csv(self):
+    def set_output_format(self, format: OutputFormat) -> None:
         for model in self._simulation_opts:
-            self._simulation_opts[model].set_option("outputFormat", "csv")
+            self._simulation_opts[model].set_option("outputFormat", format.value)
 
     def set_solver(self, solver: Solver, model_name: str = None) -> None:
         if model_name:
             _model_name: str = self._get_cache_key(model_name, self._simulation_opts)
             self._simulation_opts[_model_name].set_option("solver", solver.value)
         else:
             for model in self._simulation_opts:
```

### Comparing `pydelica-0.5.0/pydelica/compiler.py` & `pydelica-0.5.1/pydelica/compiler.py`

 * *Files identical despite different names*

### Comparing `pydelica-0.5.0/pydelica/exception.py` & `pydelica-0.5.1/pydelica/exception.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,21 +63,32 @@
 class UnknownLibraryError(Exception):
     def __init__(self, msg):
         Exception.__init__(self, msg)
 
 
 def parse_error_string_compiler(out_string: str, error_string: str):
     if "Failed to parse file" in out_string:
+        print(out_string)
         _error = [i for i in out_string.split("\n") if i and i[0] == "["]
         raise OMParsingError(", ".join(_error))
     elif "Execution failed!" in error_string:
         raise OMExecutionError(f"Failed to execute compiled code:\n{out_string}")
-    elif "failed" in out_string:
+
+    # Check if "failed" is present within output, ignore print out of code
+    # assuming all lines containing the term end with ';'
+
+    _lines: list[str] = [
+       i for i in out_string.split("\n")
+       if "failed" in i.lower()
+       and not i.strip().endswith(";") # Do not include lines from code
+    ]
+ 
+    if "failed" in out_string and _lines:
         raise OMBuildError(
-            ", ".join([i for i in out_string.split("\n") if "failed" in i.lower()])
+            ", ".join(_lines)
         )
 
 
 def parse_error_string_simulate(out_string: str, terminate_on_assert: str = "error"):
     print(out_string)
     if "division by zero" in out_string:
         _line = [i for i in out_string.split("\n") if "division by zero" in i]
```

### Comparing `pydelica-0.5.0/pydelica/model.py` & `pydelica-0.5.1/pydelica/model.py`

 * *Files identical despite different names*

### Comparing `pydelica-0.5.0/pydelica/options.py` & `pydelica-0.5.1/pydelica/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,26 @@
 from typing import Any, Iterable, List
 
 import defusedxml.ElementTree as ET
 
 from pydelica.exception import UnknownLibraryError, UnknownOptionError
 
 
-class Solver(enum.Enum):
+class Solver(str, enum.Enum):
     DASSL = "dassl"
     EULER = "euler"
     RUNGE_KUTTA = "rungekutta"
 
 
+class OutputFormat(str, enum.Enum):
+    CSV = "csv"
+    MAT = "mat"
+    PLT = "plt"
+
+
 class LibrarySetup:
     """Object containing setup for a particular Modelica library version"""
 
     def __init__(self) -> None:
         """Create a setup object
 
         Parameters
```

### Comparing `pydelica-0.5.0/pydelica/solutions.py` & `pydelica-0.5.1/pydelica/solutions.py`

 * *Files identical despite different names*

### Comparing `pydelica-0.5.0/pyproject.toml` & `pydelica-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydelica"
-version = "0.5.0"
+version = "0.5.1"
 description = "Light-weight serverless API for OpenModelica"
 authors = ["Kristian Zarebski <krizar312@gmail.com>"]
 license = "MIT"
 keywords = ["modelica", "openmodelica"]
 repository = "https://gitlab.com/krizar/pydelica"
 readme = "README.md"
 include = [
```

### Comparing `pydelica-0.5.0/PKG-INFO` & `pydelica-0.5.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydelica
-Version: 0.5.0
+Version: 0.5.1
 Summary: Light-weight serverless API for OpenModelica
 Home-page: https://gitlab.com/krizar/pydelica
 License: MIT
 Keywords: modelica,openmodelica
 Author: Kristian Zarebski
 Author-email: krizar312@gmail.com
 Requires-Python: >=3.9,<3.13
@@ -21,14 +21,18 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: pandas (>=2.0,<3.0)
 Project-URL: Repository, https://gitlab.com/krizar/pydelica
 Description-Content-Type: text/markdown
 
+<p align="center">
+<img src="https://gitlab.com/krizar/pydelica/-/raw/main/media/pyd_logo.svg", width="200">
+</p>
+
 # PyDelica: Serverless OpenModelica with Python
 
 ## About
 
 PyDelica is an API providing a quick and easy to use interface to compile, customise and run OpenModelica models with Python. Unlike OMPython it does not require the launch of a server session to use OMShell but rather dynamically adjusts files produced after model compilation in order to update options and parameters. The lack of server requirement means models can be run in tandem without calling multiple OMC sessions which can be very taxing on CPU. Furthermore PyDelica is able to detect errors during model runs by reading the `stderr` and `stdout` from OpenModelica and throw appropriate exceptions to terminate the program execution.
 
 ## Installation
@@ -84,20 +88,47 @@
 session.build_model(model_path, 'M.A')
 ```
 
 The `build_model` function also allows you to specify additional flags/options to hand to the OMC compiler, these are given
 in the form of a dictionary where the value can be `None` if the flag does not take any input. You can also directly set the profiling level for profiling the Modelica code. When set, the profile dictionary is also stored in the session after the simulation and is accessible via the `code_profile` and `code_info` attributes:
 
 ```python
-session.build_model(model_path, 'M.A', profiling="all", omc_build_flags={"-g": "MetaModelica"})
+session.build_model(
+    model_path,
+    model_addr='M.A'
+    profiling="all",
+    omc_build_flags={"-g": "MetaModelica"}
+)
 session.simulate()
 print(session.code_profile)
 print(session.code_info)
 ```
 
+#### Specifying Additional Model-Based Dependencies
+
+If additional model files are required to execute the main model these can be specified with the `extra_models` argument:
+
+```python
+session.build_model(
+    model_path,
+    extra_models=["extra_model.mo"]
+)
+```
+
+#### Using Alternative Inputs Location
+
+If your model inputs are stored in an alternative directory, this can be specified with the `update_input_paths_to` argument:
+
+```python
+session.build_model(
+    model_path,
+    update_input_paths_to="/path/to/inputs"
+)
+```
+
 #### Examining Parameters and Options
 We can examine all parameters for a given model using the `get_parameters` method which will return a Python dictionary:
 
 ```python
 session.get_parameters('SineCurrentModel')
 ```
 
@@ -167,16 +198,16 @@
 Possible values ranked by order (highest at the top):
 
 |**Value**|**Description**|
 |---|---|
 |`'never'`|Do not throw an exception on Modelica assertion violation|
 |`'error'`|Default. Throw an exception on an assertion of level `AssertionLevel.error`|
 |`'warning'`|Throw an exception on assertion of level `AssertionLevel.warning`|
-|`'info'`|Throw an exception on any `assert | info` statement|
-|`'debug'`|Throw an exception on any `assert | debug` statement|
+|`'info'`|Throw an exception on any `assert \| info` statement|
+|`'debug'`|Throw an exception on any `assert \| debug` statement|
 
 #### Running the Simulation
 To run the simulation use the `simulate` method. If a model name is specified then that model is run,
 else this is the first model in the model list. At the simulation step parameter values are written to the
 XML file read by the binary before the model binary is executed.
 
 ```python
@@ -194,22 +225,49 @@
 The variables for each model are stored as a Pandas dataframe.
 
 #### Using Alternative Libraries
 
 **NOTE:** Currently only works in WSL on Windows machines.
 
 You can use an alternative library version via the `use_library` method:
-```python3
+```python
 session.use_library("Modelica", "3.2.3")
 ```
 you can also optionally specify the location of this library:
-```python3
+```python
 session.use_library("Modelica", "3.2.3", library_directory="/home/user/my_om_libraries")
 ```
 
+#### Including Extra C Resources
+
+When building a model extra C file resources can be specified using the `c_source_dir` argument to `build_model`:
+
+```python
+session.build_model(
+    model_path,
+    c_source_dir=os.path.join(model_dir, "Resources", "Include")
+)
+```
+
+## Docker
+
+A Docker image is available for OpenModelica with Pydelica:
+
+```sh
+$ docker pull artemisbeta/pydelica
+```
+
+You can try out Pydelica within a Jupyter notebook by running:
+
+```sh
+$ docker run -ti artemisbeta/pydelica jupyter notebook --ip 0.0.0.0 --no-browser
+```
+
+and opening the resulting URL within your browser.
+
 ## Troubleshooting
 
 ### Simulation fails with no error thrown
 Try setting the assertion level to a lower level, for some reason OM ranks missing input file errors
 as type `debug`, see [here](#failing-simulation-on-lower-assertion-level).
 
 ```
@@ -217,7 +275,13 @@
 assert | debug | Not possible to open file "Default/myInput.mat": No such file or directory
 assert | info | simulation terminated by an assertion at initialization
 ```
 
 ### PyDelica cannot find OMC
 PyDelica relies on either locating OMC on UNIX using the `which` command, or in the case of Windows using the `OPENMODELICAHOME` environment variable. Ensure at least one of these is available after installating OpenModelica.
 
+## Use Cases
+
+_Pydelica_ is currently being used in the following projects, if you would like to be included in this list please open an issue:
+
+* [_Power Balance Models_](https://github.com/ukaea/powerbalance), _United Kingdom Atomic Energy Authority_: A tokamak power balance model with Python API and CLI
+
```

