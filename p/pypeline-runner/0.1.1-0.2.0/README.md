# Comparing `tmp/pypeline_runner-0.1.1.tar.gz` & `tmp/pypeline_runner-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypeline_runner-0.1.1.tar", max compression
+gzip compressed data, was "pypeline_runner-0.2.0.tar", max compression
```

## Comparing `pypeline_runner-0.1.1.tar` & `pypeline_runner-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1066 2024-04-12 09:33:54.893064 pypeline_runner-0.1.1/LICENSE
--rw-r--r--   0        0        0     4611 2024-04-12 09:33:54.893064 pypeline_runner-0.1.1/README.md
--rw-r--r--   0        0        0     3925 2024-04-12 09:33:55.629059 pypeline_runner-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-12 09:33:55.629059 pypeline_runner-0.1.1/src/pypeline/__init__.py
--rw-r--r--   0        0        0      350 2024-04-12 09:33:54.893064 pypeline_runner-0.1.1/src/pypeline/__run.py
--rw-r--r--   0        0        0        0 2024-04-12 09:33:54.893064 pypeline_runner-0.1.1/src/pypeline/domain/__init__.py
--rw-r--r--   0        0        0     1355 2024-04-12 09:33:54.893064 pypeline_runner-0.1.1/src/pypeline/domain/artifacts.py
--rw-r--r--   0        0        0     1491 2024-04-12 09:33:54.893064 pypeline_runner-0.1.1/src/pypeline/domain/config.py
--rw-r--r--   0        0        0     1101 2024-04-12 09:33:54.893064 pypeline_runner-0.1.1/src/pypeline/domain/execution_context.py
--rw-r--r--   0        0        0      817 2024-04-12 09:33:54.893064 pypeline_runner-0.1.1/src/pypeline/domain/pipeline.py
--rw-r--r--   0        0        0      894 2024-04-12 09:33:54.893064 pypeline_runner-0.1.1/src/pypeline/domain/project_slurper.py
--rw-r--r--   0        0        0        0 2024-04-12 09:33:54.893064 pypeline_runner-0.1.1/src/pypeline/kickstart/__init__.py
--rw-r--r--   0        0        0     2410 2024-04-12 09:33:54.893064 pypeline_runner-0.1.1/src/pypeline/kickstart/create.py
--rw-r--r--   0        0        0     5772 2024-04-12 09:33:54.893064 pypeline_runner-0.1.1/src/pypeline/kickstart/templates/bootstrap/bootstrap.ps1
--rw-r--r--   0        0        0    15971 2024-04-12 09:33:54.893064 pypeline_runner-0.1.1/src/pypeline/kickstart/templates/bootstrap/bootstrap.py
--rw-r--r--   0        0        0       13 2024-04-12 09:33:54.893064 pypeline_runner-0.1.1/src/pypeline/kickstart/templates/project/.gitignore
--rw-r--r--   0        0        0       34 2024-04-12 09:33:54.893064 pypeline_runner-0.1.1/src/pypeline/kickstart/templates/project/poetry.toml
--rw-r--r--   0        0        0       36 2024-04-12 09:33:54.893064 pypeline_runner-0.1.1/src/pypeline/kickstart/templates/project/pypeline.ps1
--rw-r--r--   0        0        0      219 2024-04-12 09:33:54.893064 pypeline_runner-0.1.1/src/pypeline/kickstart/templates/project/pypeline.yaml
--rw-r--r--   0        0        0      225 2024-04-12 09:33:54.893064 pypeline_runner-0.1.1/src/pypeline/kickstart/templates/project/pyproject.toml
--rw-r--r--   0        0        0      219 2024-04-12 09:33:54.893064 pypeline_runner-0.1.1/src/pypeline/kickstart/templates/project/scoopfile.json
--rw-r--r--   0        0        0      651 2024-04-12 09:33:54.893064 pypeline_runner-0.1.1/src/pypeline/kickstart/templates/project/steps/my_step.py
--rw-r--r--   0        0        0     3406 2024-04-12 09:33:54.893064 pypeline_runner-0.1.1/src/pypeline/main.py
--rw-r--r--   0        0        0        0 2024-04-12 09:33:54.893064 pypeline_runner-0.1.1/src/pypeline/py.typed
--rw-r--r--   0        0        0     4235 2024-04-12 09:33:54.893064 pypeline_runner-0.1.1/src/pypeline/pypeline.py
--rw-r--r--   0        0        0        0 2024-04-12 09:33:54.893064 pypeline_runner-0.1.1/src/pypeline/steps/__init__.py
--rw-r--r--   0        0        0     1599 2024-04-12 09:33:54.893064 pypeline_runner-0.1.1/src/pypeline/steps/create_venv.py
--rw-r--r--   0        0        0     3257 2024-04-12 09:33:54.893064 pypeline_runner-0.1.1/src/pypeline/steps/scoop_install.py
--rw-r--r--   0        0        0     1860 2024-04-12 09:33:54.893064 pypeline_runner-0.1.1/src/pypeline/steps/west_install.py
--rw-r--r--   0        0        0     5850 1970-01-01 00:00:00.000000 pypeline_runner-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-14 16:33:24.497637 pypeline_runner-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5929 2024-04-14 16:33:24.497637 pypeline_runner-0.2.0/README.md
+-rw-r--r--   0        0        0     3925 2024-04-14 16:33:25.293635 pypeline_runner-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-14 16:33:25.293635 pypeline_runner-0.2.0/src/pypeline/__init__.py
+-rw-r--r--   0        0        0      350 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/__run.py
+-rw-r--r--   0        0        0        0 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/domain/__init__.py
+-rw-r--r--   0        0        0     1355 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/domain/artifacts.py
+-rw-r--r--   0        0        0     1491 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/domain/config.py
+-rw-r--r--   0        0        0     1101 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/domain/execution_context.py
+-rw-r--r--   0        0        0      980 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/domain/pipeline.py
+-rw-r--r--   0        0        0      894 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/domain/project_slurper.py
+-rw-r--r--   0        0        0        0 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/kickstart/__init__.py
+-rw-r--r--   0        0        0     2235 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/kickstart/create.py
+-rw-r--r--   0        0        0     5772 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/kickstart/templates/bootstrap/bootstrap.ps1
+-rw-r--r--   0        0        0    15971 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/kickstart/templates/bootstrap/bootstrap.py
+-rw-r--r--   0        0        0       13 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/kickstart/templates/project/.gitignore
+-rw-r--r--   0        0        0       34 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/kickstart/templates/project/poetry.toml
+-rw-r--r--   0        0        0       36 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/kickstart/templates/project/pypeline.ps1
+-rw-r--r--   0        0        0      219 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/kickstart/templates/project/pypeline.yaml
+-rw-r--r--   0        0        0      225 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/kickstart/templates/project/pyproject.toml
+-rw-r--r--   0        0        0      219 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/kickstart/templates/project/scoopfile.json
+-rw-r--r--   0        0        0      651 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/kickstart/templates/project/steps/my_step.py
+-rw-r--r--   0        0        0     3382 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/main.py
+-rw-r--r--   0        0        0        0 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/py.typed
+-rw-r--r--   0        0        0     4359 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/pypeline.py
+-rw-r--r--   0        0        0        0 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/steps/__init__.py
+-rw-r--r--   0        0        0     1954 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/steps/create_venv.py
+-rw-r--r--   0        0        0     3356 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/steps/scoop_install.py
+-rw-r--r--   0        0        0     1930 2024-04-14 16:33:24.501637 pypeline_runner-0.2.0/src/pypeline/steps/west_install.py
+-rw-r--r--   0        0        0     7168 1970-01-01 00:00:00.000000 pypeline_runner-0.2.0/PKG-INFO
```

### Comparing `pypeline_runner-0.1.1/LICENSE` & `pypeline_runner-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.1.1/README.md` & `pypeline_runner-0.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Python Pipeline
+# Pypeline
 
 <p align="center">
   <a href="https://github.com/cuinixam/pypeline/actions/workflows/ci.yml?query=branch%3Amain">
     <img src="https://img.shields.io/github/actions/workflow/status/cuinixam/pypeline/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >
   </a>
   <a href="https://pypeline-runner.readthedocs.io">
     <img src="https://img.shields.io/readthedocs/pypeline-runner.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">
@@ -19,22 +19,35 @@
     <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json" alt="ruff">
   </a>
   <a href="https://github.com/pre-commit/pre-commit">
     <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">
   </a>
 </p>
 <p align="center">
-  <a href="https://pypi.org/project/pypeline/">
-    <img src="https://img.shields.io/pypi/v/pypeline.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">
+  <a href="https://pypi.org/project/pypeline-runner/">
+    <img src="https://img.shields.io/pypi/v/pypeline-runner.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">
   </a>
-  <img src="https://img.shields.io/pypi/pyversions/pypeline.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">
-  <img src="https://img.shields.io/pypi/l/pypeline.svg?style=flat-square" alt="License">
+  <img src="https://img.shields.io/pypi/pyversions/pypeline-runner.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">
+  <img src="https://img.shields.io/pypi/l/pypeline-runner.svg?style=flat-square" alt="License">
 </p>
 
-Configure and execute pipelines with Python (similar to GitHub workflows or Jenkins pipelines).
+Pypeline is a Python application designed to streamline and automate the software development lifecycle, particularly the pipeline execution processes across various environments such as GitHub and Jenkins.
+The primary motivation for developing Pypeline stemmed from the need to unify and simplify the creation of build, test, and deployment pipelines that are traditionally defined separately across these platforms using GitHub workflows (YAML) and Jenkins pipelines (Jenkinsfile).
+
+**Key Features**
+
+- **Unified Pipeline Definition**: Users can define their entire pipeline in a single YAML file, eliminating the need to switch between different syntaxes and configurations for different CI/CD tools.
+
+- **Extensibility**: Pypeline supports execution steps defined not only through local scripts but also from installed Python packages.
+
+- **Execution Context**: Each step in the pipeline receives an execution context that can be updated during step execution. This allows for the sharing of information and state between steps.
+
+- **Dependency Handling**: Dependency management ensures that only the necessary steps are executed, reducing runtime and resource usage by avoiding unnecessary operations.
+
+- **Ease of Use**: With Pypeline, setting up and running pipelines becomes more straightforward, enabling developers to focus more on coding and less on configuring pipeline specifics.
 
 ## Installation
 
 Install this via pip (or your favourite package manager):
 
 `pip install pypeline-runner`
 
@@ -82,11 +95,8 @@
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 <!-- prettier-ignore-end -->
 
 This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
 
 ## Credits
 
-This package was created with
-[Copier](https://copier.readthedocs.io/) and the
-[cuinixam/pypackage-template](https://github.com/cuinixam/pypackage-template)
-project template.
+This package was created with [Copier](https://copier.readthedocs.io/) and the [cuinixam/pypackage-template](https://github.com/cuinixam/pypackage-template) project template.
```

#### html2text {}

```diff
@@ -1,21 +1,38 @@
-# Python Pipeline
+# Pypeline
           _[_C_I_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_T_e_s_t_ _c_o_v_e_r_a_g_e_ _p_e_r_c_e_n_t_a_g_e_]
                           _[_P_o_e_t_r_y_]_[_r_u_f_f_]_[_p_r_e_-_c_o_m_m_i_t_]
               _[_P_y_P_I_ _V_e_r_s_i_o_n_][Supported Python versions][License]
-Configure and execute pipelines with Python (similar to GitHub workflows or
-Jenkins pipelines). ## Installation Install this via pip (or your favourite
-package manager): `pip install pypeline-runner` ## Start developing The project
-uses Poetry for dependencies management and packaging. Run the `bootstrap.ps1`
-script to install Python and create the virtual environment. ```powershell
-.\bootstrap.ps1 ``` This will also generate a `poetry.lock` file, you should
-track this file in version control. To execute the test suite, call pytest
-inside Poetry's virtual environment via `poetry run`: ```shell .venv/Scripts/
-poetry run pytest ``` Check out the Poetry documentation for more information
-on the available commands. For those using [VS Code](https://
+Pypeline is a Python application designed to streamline and automate the
+software development lifecycle, particularly the pipeline execution processes
+across various environments such as GitHub and Jenkins. The primary motivation
+for developing Pypeline stemmed from the need to unify and simplify the
+creation of build, test, and deployment pipelines that are traditionally
+defined separately across these platforms using GitHub workflows (YAML) and
+Jenkins pipelines (Jenkinsfile). **Key Features** - **Unified Pipeline
+Definition**: Users can define their entire pipeline in a single YAML file,
+eliminating the need to switch between different syntaxes and configurations
+for different CI/CD tools. - **Extensibility**: Pypeline supports execution
+steps defined not only through local scripts but also from installed Python
+packages. - **Execution Context**: Each step in the pipeline receives an
+execution context that can be updated during step execution. This allows for
+the sharing of information and state between steps. - **Dependency Handling**:
+Dependency management ensures that only the necessary steps are executed,
+reducing runtime and resource usage by avoiding unnecessary operations. -
+**Ease of Use**: With Pypeline, setting up and running pipelines becomes more
+straightforward, enabling developers to focus more on coding and less on
+configuring pipeline specifics. ## Installation Install this via pip (or your
+favourite package manager): `pip install pypeline-runner` ## Start developing
+The project uses Poetry for dependencies management and packaging. Run the
+`bootstrap.ps1` script to install Python and create the virtual environment.
+```powershell .\bootstrap.ps1 ``` This will also generate a `poetry.lock` file,
+you should track this file in version control. To execute the test suite, call
+pytest inside Poetry's virtual environment via `poetry run`: ```shell .venv/
+Scripts/poetry run pytest ``` Check out the Poetry documentation for more
+information on the available commands. For those using [VS Code](https://
 code.visualstudio.com/) there are tasks defined for the most common commands: -
 bootstrap - install dependencies - run tests - run all checks configured for
 pre-commit - generate documentation See the `.vscode/tasks.json` for more
 details. ## Committing changes This repository uses [commitlint](https://
 github.com/conventional-changelog/commitlint) for checking if the commit
 message meets the [conventional commit format](https://
 www.conventionalcommits.org/en). ## Contributors â¨ Thanks goes to these
```

### Comparing `pypeline_runner-0.1.1/pyproject.toml` & `pypeline_runner-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypeline-runner"
-version = "0.1.1"
+version = "0.2.0"
 description = "Configure and execute pipelines with Python (similar to GitHub workflows or Jenkins pipelines)."
 authors = ["cuinixam <me@cuinixam.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/cuinixam/pypeline"
 documentation = "https://pypeline-runner.readthedocs.io"
 classifiers = [
@@ -23,15 +23,15 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/cuinixam/pypeline/issues"
 "Changelog" = "https://github.com/cuinixam/pypeline/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-py-app-dev = "^2.1.0"
+py-app-dev = "^2.1.1"
 typer = {extras = ["all"], version = "^0.12.0"}
 pyyaml = "^6.0.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.0"
 pre-commit = "^3.1.1"
```

### Comparing `pypeline_runner-0.1.1/src/pypeline/domain/artifacts.py` & `pypeline_runner-0.2.0/src/pypeline/domain/artifacts.py`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.1.1/src/pypeline/domain/config.py` & `pypeline_runner-0.2.0/src/pypeline/domain/config.py`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.1.1/src/pypeline/domain/execution_context.py` & `pypeline_runner-0.2.0/src/pypeline/domain/execution_context.py`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.1.1/src/pypeline/domain/pipeline.py` & `pypeline_runner-0.2.0/src/pypeline/kickstart/templates/project/steps/my_step.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,25 @@
-from abc import abstractmethod
 from pathlib import Path
-from typing import Type
+from typing import List
 
-from py_app_dev.core.runnable import Runnable
+from py_app_dev.core.logging import logger
 
-from .execution_context import ExecutionContext
+from pypeline.domain.pipeline import PipelineStep
 
 
-class PipelineStep(Runnable):
-    def __init__(self, execution_context: ExecutionContext, output_dir: Path) -> None:
-        self.execution_context = execution_context
-        self.output_dir = output_dir
-        self.project_root_dir = self.execution_context.project_root_dir
+class MyStep(PipelineStep):
+    def run(self) -> None:
+        logger.info(f"Run {self.get_name()} found install dirs:")
+        for install_dir in self.execution_context.install_dirs:
+            logger.info(f" {install_dir}")
 
-    @abstractmethod
-    def update_execution_context(self) -> None:
-        pass
+    def get_inputs(self) -> List[Path]:
+        return []
+
+    def get_outputs(self) -> List[Path]:
+        return []
 
+    def get_name(self) -> str:
+        return self.__class__.__name__
 
-class PipelineStepReference:
-    def __init__(self, group_name: str, _class: Type[PipelineStep]) -> None:
-        self.group_name = group_name
-        self._class = _class
-
-    @property
-    def name(self) -> str:
-        return self._class.__name__
+    def update_execution_context(self) -> None:
+        pass
```

### Comparing `pypeline_runner-0.1.1/src/pypeline/domain/project_slurper.py` & `pypeline_runner-0.2.0/src/pypeline/domain/project_slurper.py`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.1.1/src/pypeline/kickstart/create.py` & `pypeline_runner-0.2.0/src/pypeline/kickstart/create.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,32 +27,30 @@
 
     def resolve_file_path(self, file: Union[Path, str]) -> Path:
         return self.input_dir.joinpath(file) if isinstance(file, str) else file
 
     @staticmethod
     def _check_target_directory(project_dir: Path) -> None:
         if project_dir.is_dir() and any(project_dir.iterdir()):
-            raise UserNotificationException(f"Project directory '{project_dir}' is not empty." " The target directory shall either be empty or not exist.")
+            raise UserNotificationException(f"Project directory '{project_dir}' is not empty. Use --force to override.")
 
     def build(self) -> None:
         if self.check_target_directory_flag:
             self._check_target_directory(self.project_dir)
         for dir in self.dirs:
             shutil.copytree(dir, self.project_dir, dirs_exist_ok=True)
 
 
 class KickstartProject:
-    def __init__(self, project_dir: Path, bootstrap_only: bool = False, force: bool = False) -> None:
+    def __init__(self, project_dir: Path, force: bool = False) -> None:
         self.logger = logger.bind()
         self.project_dir = project_dir
-        self.bootstrap_only = bootstrap_only
         self.force = force
 
     def run(self) -> None:
         self.logger.info(f"Kickstart new project in '{self.project_dir.absolute().as_posix()}'")
         project_builder = ProjectBuilder(self.project_dir)
-        project_builder.with_dir("bootstrap")
-        if self.bootstrap_only or self.force:
+        if self.force:
             project_builder.with_disable_target_directory_check()
-        if not self.bootstrap_only:
-            project_builder.with_dir("project")
+        project_builder.with_dir("bootstrap")
+        project_builder.with_dir("project")
         project_builder.build()
```

### Comparing `pypeline_runner-0.1.1/src/pypeline/kickstart/templates/bootstrap/bootstrap.ps1` & `pypeline_runner-0.2.0/src/pypeline/kickstart/templates/bootstrap/bootstrap.ps1`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.1.1/src/pypeline/kickstart/templates/bootstrap/bootstrap.py` & `pypeline_runner-0.2.0/src/pypeline/kickstart/templates/bootstrap/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pypeline_runner-0.1.1/src/pypeline/main.py` & `pypeline_runner-0.2.0/src/pypeline/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,18 +27,17 @@
         raise typer.Exit()
 
 
 @app.command()
 @time_it("init")
 def init(
     project_dir: Path = typer.Option(Path.cwd().absolute(), help="The project directory"),  # noqa: B008
-    bootstrap_only: bool = typer.Option(False, help="Initialize only the bootstrap files."),
     force: bool = typer.Option(False, help="Force the initialization of the project even if the directory is not empty."),
 ) -> None:
-    KickstartProject(project_dir, bootstrap_only, force).run()
+    KickstartProject(project_dir, force).run()
 
 
 @app.command()
 @time_it("run")
 def run(
     project_dir: Path = typer.Option(Path.cwd().absolute(), help="The project directory"),  # noqa: B008,
     step: Optional[str] = typer.Option(
@@ -56,18 +55,22 @@
         is_flag=True,
     ),
     force_run: bool = typer.Option(
         False,
         help="Force the execution of a step even if it is not dirty.",
         is_flag=True,
     ),
+    dry_run: bool = typer.Option(
+        False,
+        help="Do not run any step, just print the steps that would be executed.",
+        is_flag=True,
+    ),
 ) -> None:
     project_slurper = ProjectSlurper(project_dir)
     if print:
-        logger.warning("TODO: print pipeline steps")
         logger.info("Pipeline steps:")
         for group, step_configs in project_slurper.pipeline.items():
             logger.info(f"    Group: {group}")
             for step_config in step_configs:
                 logger.info(f"        {step_config.step}")
         return
     if not project_slurper.pipeline:
@@ -76,19 +79,15 @@
     steps_references = PipelineScheduler(project_slurper.pipeline, project_dir).get_steps_to_run(step, single)
     if not steps_references:
         if step:
             raise UserNotificationException(f"Step '{step}' not found in the pipeline.")
         logger.info("No steps to run.")
         return
 
-    PipelineStepsExecutor(
-        project_slurper.artifacts_locator,
-        steps_references,
-        force_run,
-    ).run()
+    PipelineStepsExecutor(project_slurper.artifacts_locator, steps_references, force_run, dry_run).run()
 
 
 def main(args: Optional[List[str]] = None) -> int:
     try:
         setup_logger()
         if args is None:
             args = sys.argv[1:]
```

### Comparing `pypeline_runner-0.1.1/src/pypeline/pypeline.py` & `pypeline_runner-0.2.0/src/pypeline/pypeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,40 +22,42 @@
 
     def __init__(self, pipeline_config: PipelineConfig, project_root_dir: Path) -> None:
         self.pipeline_config = pipeline_config
         self.project_root_dir = project_root_dir
         self._loader = GenericPipelineLoader[PipelineStep](self.pipeline_config, self.project_root_dir)
 
     def load_steps_references(self) -> List[PipelineStepReference]:
-        return [PipelineStepReference(step_reference.group_name, step_reference._class) for step_reference in self._loader.load_steps()]
+        return [PipelineStepReference(step_reference.group_name, step_reference._class, step_reference.config) for step_reference in self._loader.load_steps()]
 
 
 class PipelineStepsExecutor:
     """Executes a list of pipeline steps sequentially."""
 
     def __init__(
         self,
         artifacts_locator: ProjectArtifactsLocator,
         steps_references: List[PipelineStepReference],
         force_run: bool = False,
+        dry_run: bool = False,
     ) -> None:
         self.logger = logger.bind()
         self.artifacts_locator = artifacts_locator
         self.steps_references = steps_references
         self.force_run = force_run
+        self.dry_run = dry_run
 
     def run(self) -> None:
         execution_context = ExecutionContext(project_root_dir=self.artifacts_locator.project_root_dir, install_dirs=[])
         for step_reference in self.steps_references:
             step_output_dir = self.artifacts_locator.build_dir / step_reference.group_name
             # Create the step output directory, to make sure that files can be created.
             step_output_dir.mkdir(parents=True, exist_ok=True)
-            step = step_reference._class(execution_context, step_output_dir)
+            step = step_reference._class(execution_context, step_output_dir, step_reference.config)
             # Execute the step is necessary. If the step is not dirty, it will not be executed
-            Executor(step.output_dir, self.force_run).execute(step)
+            Executor(step.output_dir, self.force_run, self.dry_run).execute(step)
             # Independent if the step was executed or not, every step shall update the context
             step.update_execution_context()
 
         return
 
 
 class PipelineScheduler:
```

### Comparing `pypeline_runner-0.1.1/src/pypeline/steps/scoop_install.py` & `pypeline_runner-0.2.0/src/pypeline/steps/scoop_install.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import io
 import json
 import traceback
 from dataclasses import dataclass
 from pathlib import Path
-from typing import ClassVar, List
+from typing import Any, ClassVar, Dict, List, Optional
 
 from mashumaro.config import TO_DICT_ADD_OMIT_NONE_FLAG, BaseConfig
 from mashumaro.mixins.json import DataClassJSONMixin
 from py_app_dev.core.exceptions import UserNotificationException
 from py_app_dev.core.logging import logger
 from py_app_dev.core.scoop_wrapper import ScoopWrapper
 
@@ -42,16 +42,16 @@
 
 
 def create_scoop_wrapper() -> ScoopWrapper:
     return ScoopWrapper()
 
 
 class ScoopInstall(PipelineStep):
-    def __init__(self, execution_context: ExecutionContext, output_dir: Path) -> None:
-        super().__init__(execution_context, output_dir)
+    def __init__(self, execution_context: ExecutionContext, output_dir: Path, config: Optional[Dict[str, Any]] = None) -> None:
+        super().__init__(execution_context, output_dir, config)
         self.logger = logger.bind()
         self.execution_info = ScoopInstallExecutionInfo([])
         # One needs to keep track of the installed apps to get the required paths
         # even if the step does not need to run.
         self.execution_info_file = self.output_dir.joinpath("scoop_install_exec_info.json")
 
     def get_name(self) -> str:
@@ -73,15 +73,15 @@
         self.execution_info.to_json_file(self.execution_info_file)
         return 0
 
     def get_inputs(self) -> List[Path]:
         return [self.scoop_file]
 
     def get_outputs(self) -> List[Path]:
-        return self.install_dirs
+        return [self.execution_info_file, *self.install_dirs]
 
     def update_execution_context(self) -> None:
         install_dirs = ScoopInstallExecutionInfo.from_json_file(self.execution_info_file).install_dirs
         # Make the list unique and keep the order
         unique_paths = list(dict.fromkeys(install_dirs))
         # Update the install directories for the subsequent steps
         self.execution_context.add_install_dirs(unique_paths)
```

### Comparing `pypeline_runner-0.1.1/src/pypeline/steps/west_install.py` & `pypeline_runner-0.2.0/src/pypeline/steps/west_install.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from pathlib import Path
-from typing import List
+from typing import Any, Dict, List, Optional
 
 from py_app_dev.core.exceptions import UserNotificationException
 from py_app_dev.core.logging import logger
 
 from ..domain.execution_context import ExecutionContext
 from ..domain.pipeline import PipelineStep
 
 
 class WestInstall(PipelineStep):
-    def __init__(self, execution_context: ExecutionContext, output_dir: Path) -> None:
-        super().__init__(execution_context, output_dir)
+    def __init__(self, execution_context: ExecutionContext, output_dir: Path, config: Optional[Dict[str, Any]] = None) -> None:
+        super().__init__(execution_context, output_dir, config)
         self.logger = logger.bind()
         self.artifacts_locator = execution_context.create_artifacts_locator()
 
     def get_name(self) -> str:
         return self.__class__.__name__
 
     @property
```

### Comparing `pypeline_runner-0.1.1/PKG-INFO` & `pypeline_runner-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypeline-runner
-Version: 0.1.1
+Version: 0.2.0
 Summary: Configure and execute pipelines with Python (similar to GitHub workflows or Jenkins pipelines).
 Home-page: https://github.com/cuinixam/pypeline
 License: MIT
 Author: cuinixam
 Author-email: me@cuinixam.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,24 +13,24 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: py-app-dev (>=2.1.0,<3.0.0)
+Requires-Dist: py-app-dev (>=2.1.1,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: typer[all] (>=0.12.0,<0.13.0)
 Project-URL: Bug Tracker, https://github.com/cuinixam/pypeline/issues
 Project-URL: Changelog, https://github.com/cuinixam/pypeline/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://pypeline-runner.readthedocs.io
 Project-URL: Repository, https://github.com/cuinixam/pypeline
 Description-Content-Type: text/markdown
 
-# Python Pipeline
+# Pypeline
 
 <p align="center">
   <a href="https://github.com/cuinixam/pypeline/actions/workflows/ci.yml?query=branch%3Amain">
     <img src="https://img.shields.io/github/actions/workflow/status/cuinixam/pypeline/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >
   </a>
   <a href="https://pypeline-runner.readthedocs.io">
     <img src="https://img.shields.io/readthedocs/pypeline-runner.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">
@@ -47,22 +47,35 @@
     <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json" alt="ruff">
   </a>
   <a href="https://github.com/pre-commit/pre-commit">
     <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">
   </a>
 </p>
 <p align="center">
-  <a href="https://pypi.org/project/pypeline/">
-    <img src="https://img.shields.io/pypi/v/pypeline.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">
+  <a href="https://pypi.org/project/pypeline-runner/">
+    <img src="https://img.shields.io/pypi/v/pypeline-runner.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">
   </a>
-  <img src="https://img.shields.io/pypi/pyversions/pypeline.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">
-  <img src="https://img.shields.io/pypi/l/pypeline.svg?style=flat-square" alt="License">
+  <img src="https://img.shields.io/pypi/pyversions/pypeline-runner.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">
+  <img src="https://img.shields.io/pypi/l/pypeline-runner.svg?style=flat-square" alt="License">
 </p>
 
-Configure and execute pipelines with Python (similar to GitHub workflows or Jenkins pipelines).
+Pypeline is a Python application designed to streamline and automate the software development lifecycle, particularly the pipeline execution processes across various environments such as GitHub and Jenkins.
+The primary motivation for developing Pypeline stemmed from the need to unify and simplify the creation of build, test, and deployment pipelines that are traditionally defined separately across these platforms using GitHub workflows (YAML) and Jenkins pipelines (Jenkinsfile).
+
+**Key Features**
+
+- **Unified Pipeline Definition**: Users can define their entire pipeline in a single YAML file, eliminating the need to switch between different syntaxes and configurations for different CI/CD tools.
+
+- **Extensibility**: Pypeline supports execution steps defined not only through local scripts but also from installed Python packages.
+
+- **Execution Context**: Each step in the pipeline receives an execution context that can be updated during step execution. This allows for the sharing of information and state between steps.
+
+- **Dependency Handling**: Dependency management ensures that only the necessary steps are executed, reducing runtime and resource usage by avoiding unnecessary operations.
+
+- **Ease of Use**: With Pypeline, setting up and running pipelines becomes more straightforward, enabling developers to focus more on coding and less on configuring pipeline specifics.
 
 ## Installation
 
 Install this via pip (or your favourite package manager):
 
 `pip install pypeline-runner`
 
@@ -110,12 +123,9 @@
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 <!-- prettier-ignore-end -->
 
 This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
 
 ## Credits
 
-This package was created with
-[Copier](https://copier.readthedocs.io/) and the
-[cuinixam/pypackage-template](https://github.com/cuinixam/pypackage-template)
-project template.
+This package was created with [Copier](https://copier.readthedocs.io/) and the [cuinixam/pypackage-template](https://github.com/cuinixam/pypackage-template) project template.
```

#### html2text {}

```diff
@@ -1,37 +1,54 @@
-Metadata-Version: 2.1 Name: pypeline-runner Version: 0.1.1 Summary: Configure
+Metadata-Version: 2.1 Name: pypeline-runner Version: 0.2.0 Summary: Configure
 and execute pipelines with Python (similar to GitHub workflows or Jenkins
 pipelines). Home-page: https://github.com/cuinixam/pypeline License: MIT
 Author: cuinixam Author-email: me@cuinixam.com Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
-Software Development :: Libraries Requires-Dist: py-app-dev (>=2.1.0,<3.0.0)
+Software Development :: Libraries Requires-Dist: py-app-dev (>=2.1.1,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-Dist: typer[all]
 (>=0.12.0,<0.13.0) Project-URL: Bug Tracker, https://github.com/cuinixam/
 pypeline/issues Project-URL: Changelog, https://github.com/cuinixam/pypeline/
 blob/main/CHANGELOG.md Project-URL: Documentation, https://pypeline-
 runner.readthedocs.io Project-URL: Repository, https://github.com/cuinixam/
-pypeline Description-Content-Type: text/markdown # Python Pipeline
+pypeline Description-Content-Type: text/markdown # Pypeline
           _[_C_I_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_T_e_s_t_ _c_o_v_e_r_a_g_e_ _p_e_r_c_e_n_t_a_g_e_]
                           _[_P_o_e_t_r_y_]_[_r_u_f_f_]_[_p_r_e_-_c_o_m_m_i_t_]
               _[_P_y_P_I_ _V_e_r_s_i_o_n_][Supported Python versions][License]
-Configure and execute pipelines with Python (similar to GitHub workflows or
-Jenkins pipelines). ## Installation Install this via pip (or your favourite
-package manager): `pip install pypeline-runner` ## Start developing The project
-uses Poetry for dependencies management and packaging. Run the `bootstrap.ps1`
-script to install Python and create the virtual environment. ```powershell
-.\bootstrap.ps1 ``` This will also generate a `poetry.lock` file, you should
-track this file in version control. To execute the test suite, call pytest
-inside Poetry's virtual environment via `poetry run`: ```shell .venv/Scripts/
-poetry run pytest ``` Check out the Poetry documentation for more information
-on the available commands. For those using [VS Code](https://
+Pypeline is a Python application designed to streamline and automate the
+software development lifecycle, particularly the pipeline execution processes
+across various environments such as GitHub and Jenkins. The primary motivation
+for developing Pypeline stemmed from the need to unify and simplify the
+creation of build, test, and deployment pipelines that are traditionally
+defined separately across these platforms using GitHub workflows (YAML) and
+Jenkins pipelines (Jenkinsfile). **Key Features** - **Unified Pipeline
+Definition**: Users can define their entire pipeline in a single YAML file,
+eliminating the need to switch between different syntaxes and configurations
+for different CI/CD tools. - **Extensibility**: Pypeline supports execution
+steps defined not only through local scripts but also from installed Python
+packages. - **Execution Context**: Each step in the pipeline receives an
+execution context that can be updated during step execution. This allows for
+the sharing of information and state between steps. - **Dependency Handling**:
+Dependency management ensures that only the necessary steps are executed,
+reducing runtime and resource usage by avoiding unnecessary operations. -
+**Ease of Use**: With Pypeline, setting up and running pipelines becomes more
+straightforward, enabling developers to focus more on coding and less on
+configuring pipeline specifics. ## Installation Install this via pip (or your
+favourite package manager): `pip install pypeline-runner` ## Start developing
+The project uses Poetry for dependencies management and packaging. Run the
+`bootstrap.ps1` script to install Python and create the virtual environment.
+```powershell .\bootstrap.ps1 ``` This will also generate a `poetry.lock` file,
+you should track this file in version control. To execute the test suite, call
+pytest inside Poetry's virtual environment via `poetry run`: ```shell .venv/
+Scripts/poetry run pytest ``` Check out the Poetry documentation for more
+information on the available commands. For those using [VS Code](https://
 code.visualstudio.com/) there are tasks defined for the most common commands: -
 bootstrap - install dependencies - run tests - run all checks configured for
 pre-commit - generate documentation See the `.vscode/tasks.json` for more
 details. ## Committing changes This repository uses [commitlint](https://
 github.com/conventional-changelog/commitlint) for checking if the commit
 message meets the [conventional commit format](https://
 www.conventionalcommits.org/en). ## Contributors â¨ Thanks goes to these
```

