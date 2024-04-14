# Comparing `tmp/provisioner_runtime-0.1.2-py3-none-any.whl.zip` & `tmp/provisioner_runtime-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 117233 bytes, number of entries: 135
+Zip file size: 117286 bytes, number of entries: 135
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 external/ansible_playbooks/__init__.py
 -rwxr-xr-x  2.0 unx      368 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/apt_update_upgrade.yaml
 -rwxr-xr-x  2.0 unx     5549 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/common/shell_lib.sh
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/group_vars/all
 -rwxr-xr-x  2.0 unx      678 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/reboot.yaml
 -rwxr-xr-x  2.0 unx      353 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/roles/anchor/defaults/main.yaml
 -rwxr-xr-x  2.0 unx    10424 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/roles/anchor/files/anchor_run.sh
@@ -52,24 +52,24 @@
 -rwxr-xr-x  2.0 unx     2084 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/roles/rpi_config_node/defaults/main.yaml
 -rwxr-xr-x  2.0 unx     7734 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/roles/rpi_config_node/files/raspi_configure_node.sh
 -rwxr-xr-x  2.0 unx     5549 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/roles/rpi_config_node/files/shell_lib.sh
 -rwxr-xr-x  2.0 unx     1529 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/roles/rpi_config_node/tasks/main.yaml
 -rwxr-xr-x  2.0 unx      419 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/shutdown.yaml
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/__init__.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/cli/__init__.py
--rwxr-xr-x  2.0 unx     3471 b- defN 80-Jan-01 00:00 provisioner/cli/entrypoint.py
+-rwxr-xr-x  2.0 unx     3651 b- defN 80-Jan-01 00:00 provisioner/cli/entrypoint.py
 -rwxr-xr-x  2.0 unx     2325 b- defN 80-Jan-01 00:00 provisioner/cli/state.py
 -rwxr-xr-x  2.0 unx     1400 b- defN 80-Jan-01 00:00 provisioner/cli/typer_callbacks.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/colors/__init__.py
 -rwxr-xr-x  2.0 unx      380 b- defN 80-Jan-01 00:00 provisioner/colors/color.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/config/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/config/domain/__init__.py
 -rw-r--r--  2.0 unx      605 b- defN 80-Jan-01 00:00 provisioner/config/domain/config.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/config/manager/__init__.py
--rw-r--r--  2.0 unx     5608 b- defN 80-Jan-01 00:00 provisioner/config/manager/config_manager.py
+-rw-r--r--  2.0 unx     5580 b- defN 80-Jan-01 00:00 provisioner/config/manager/config_manager.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/config/reader/__init__.py
 -rwxr-xr-x  2.0 unx     1599 b- defN 80-Jan-01 00:00 provisioner/config/reader/config_reader.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/domain/__init__.py
 -rwxr-xr-x  2.0 unx     1535 b- defN 80-Jan-01 00:00 provisioner/domain/serialize.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/errors/__init__.py
 -rwxr-xr-x  2.0 unx     1045 b- defN 80-Jan-01 00:00 provisioner/errors/cli_errors.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/func/__init__.py
@@ -79,15 +79,15 @@
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/info/__init__.py
 -rwxr-xr-x  2.0 unx     3950 b- defN 80-Jan-01 00:00 provisioner/info/system_reader.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/infra/__init__.py
 -rwxr-xr-x  2.0 unx     2452 b- defN 80-Jan-01 00:00 provisioner/infra/context.py
 -rwxr-xr-x  2.0 unx     2682 b- defN 80-Jan-01 00:00 provisioner/infra/evaluator.py
 -rwxr-xr-x  2.0 unx     4102 b- defN 80-Jan-01 00:00 provisioner/infra/log.py
 -rwxr-xr-x  2.0 unx      962 b- defN 80-Jan-01 00:00 provisioner/infra/remote_context.py
--rwxr-xr-x  2.0 unx     1673 b- defN 80-Jan-01 00:00 provisioner/main.py
+-rwxr-xr-x  2.0 unx     1668 b- defN 80-Jan-01 00:00 provisioner/main.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/resources/__init__.py
 -rw-r--r--  2.0 unx       26 b- defN 80-Jan-01 00:00 provisioner/resources/config.yaml
 -rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 provisioner/resources/version.txt
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/runner/__init__.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/runner/ansible/__init__.py
 -rw-r--r--  2.0 unx    16182 b- defN 80-Jan-01 00:00 provisioner/runner/ansible/ansible_runner.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/runner/ansible/resources/__init__.py
@@ -125,13 +125,13 @@
 -rwxr-xr-x  2.0 unx     2427 b- defN 80-Jan-01 00:00 provisioner/utils/printer.py
 -rwxr-xr-x  2.0 unx     2103 b- defN 80-Jan-01 00:00 provisioner/utils/process.py
 -rwxr-xr-x  2.0 unx     8950 b- defN 80-Jan-01 00:00 provisioner/utils/progress_indicator.py
 -rwxr-xr-x  2.0 unx     8629 b- defN 80-Jan-01 00:00 provisioner/utils/prompter.py
 -rwxr-xr-x  2.0 unx     2165 b- defN 80-Jan-01 00:00 provisioner/utils/properties.py
 -rwxr-xr-x  2.0 unx     2080 b- defN 80-Jan-01 00:00 provisioner/utils/summary.py
 -rwxr-xr-x  2.0 unx     2598 b- defN 80-Jan-01 00:00 provisioner/utils/yaml_util.py
--rw-r--r--  2.0 unx     1071 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      802 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.2.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx    14179 b- defN 16-Jan-01 00:00 provisioner_runtime-0.1.2.dist-info/RECORD
-135 files, 296663 bytes uncompressed, 93637 bytes compressed:  68.4%
+-rw-r--r--  2.0 unx     1071 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      792 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.3.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    14179 b- defN 16-Jan-01 00:00 provisioner_runtime-0.1.3.dist-info/RECORD
+135 files, 296800 bytes uncompressed, 93690 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -384,23 +384,23 @@
 
 Filename: provisioner/utils/summary.py
 Comment: 
 
 Filename: provisioner/utils/yaml_util.py
 Comment: 
 
-Filename: provisioner_runtime-0.1.2.dist-info/LICENSE
+Filename: provisioner_runtime-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: provisioner_runtime-0.1.2.dist-info/METADATA
+Filename: provisioner_runtime-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: provisioner_runtime-0.1.2.dist-info/WHEEL
+Filename: provisioner_runtime-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: provisioner_runtime-0.1.2.dist-info/entry_points.txt
+Filename: provisioner_runtime-0.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: provisioner_runtime-0.1.2.dist-info/RECORD
+Filename: provisioner_runtime-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## provisioner/cli/entrypoint.py

```diff
@@ -1,19 +1,21 @@
 #!/usr/bin/env python3
 
+import pathlib
 from typing import Callable, Optional
 
+from loguru import logger
 import typer
 
 from provisioner.cli.state import CliGlobalArgs
 from provisioner.infra.context import Context
 from provisioner.infra.log import LoggerManager
 from provisioner.utils.paths import Paths
 
-STATIC_VERSION_PACKAGE_PATH = None
+STATIC_RESOURCES_PACKAGE = "provisioner.resources"
 
 MODIFIERS_FLAGS_HELP_TITLE = "Modifiers"
 
 
 def main_runner(
     verbose: Optional[bool] = typer.Option(
         False,
@@ -84,34 +86,36 @@
     logger_mgr.initialize(verbose, dry_run)
 
 
 def try_read_version() -> str:
     content = "no version"
     try:
         file_path = Paths.create(Context.create()).get_file_path_from_python_package(
-            STATIC_VERSION_PACKAGE_PATH, "version.txt"
+            STATIC_RESOURCES_PACKAGE, "version.txt"
         )
         with open(file_path, "r+") as opened_file:
             content = opened_file.read()
             opened_file.close()
-    except Exception:
+    except Exception as ex:
+        logger.error(f"Failed to read version file. ex: {ex}")
         pass
     return content
 
 
 class EntryPoint:
     @staticmethod
     def create_typer(
         title: str,
         config_resolver_fn: Optional[Callable] = None,
-        version_package_path: Optional[str] = "resources",
+        version_package_path: Optional[str] = STATIC_RESOURCES_PACKAGE,
     ) -> typer.Typer:
 
-        global STATIC_VERSION_PACKAGE_PATH
-        STATIC_VERSION_PACKAGE_PATH = version_package_path
+        if len(version_package_path) > 0:
+            global STATIC_RESOURCES_PACKAGE
+            STATIC_RESOURCES_PACKAGE = version_package_path
 
         if config_resolver_fn:
             config_resolver_fn()
 
         # Use invoke_without_command=True to allow usage of --version flags which are NoOp commands
         # Use also no_args_is_help=True to print the help menu if no arguments were supplied
         return typer.Typer(
```

## provisioner/config/manager/config_manager.py

```diff
@@ -1,10 +1,9 @@
 #!/usr/bin/env python3
 
-from typing import Optional
 
 from loguru import logger
 
 from provisioner.config.reader.config_reader import ConfigReader
 from provisioner.domain.serialize import SerializationBase
 from provisioner.errors.cli_errors import FailedToMergeConfiguration, FailedToReadConfigurationFile
 from provisioner.infra.context import Context
```

## provisioner/main.py

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 
 import os
 import pathlib
 
 from loguru import logger
+
 from provisioner.cli.entrypoint import EntryPoint
 from provisioner.config.domain.config import ProvisionerConfig
 from provisioner.config.manager.config_manager import ConfigManager
 from provisioner.utils.package_loader import PackageLoader
 
 CONFIG_USER_PATH = os.path.expanduser("~/.config/provisioner/config.yaml")
 CONFIG_INTERNAL_PATH = f"{pathlib.Path(__file__).parent}/resources/config.yaml"
@@ -22,29 +23,27 @@
 debug_pre_init = os.getenv(key=ENV_VAR_ENABLE_PRE_INIT_DEBUG, default=False)
 
 if not debug_pre_init:
     logger.remove()
 
 app = EntryPoint.create_typer(
     title="Provision Everything Anywhere (install plugins from https://zachinachshon.com/provisioner)",
-    config_resolver_fn=lambda: ConfigManager.instance().load(
-        CONFIG_INTERNAL_PATH, CONFIG_USER_PATH, ProvisionerConfig
-    ),
+    config_resolver_fn=lambda: ConfigManager.instance().load(CONFIG_INTERNAL_PATH, CONFIG_USER_PATH, ProvisionerConfig),
 )
 
 
 def load_plugin(plugin_module):
     plugin_module.load_config()
     plugin_module.append_to_cli(app)
 
 
 PackageLoader.create().load_modules_fn(
     filter_keyword="provisioner",
     import_path="main",
-    exclusions=["provisioner", "provisioner-features-lib"],
+    exclusions=["provisioner-runtime", "provisioner-features-lib"],
     callback=lambda module: load_plugin(plugin_module=module),
     debug=debug_pre_init,
 )
 
 # ==============
 # ENTRY POINT
 # To run from source:
```

## provisioner/resources/version.txt

```diff
@@ -1 +1 @@
-0.1.1
+0.1.3
```

## provisioner/utils/paths.py

 * *Ordering differences only*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 
 import os
 import pathlib
 import sys
 from importlib import resources
+from importlib.resources import files
 from pathlib import Path
 from typing import Optional
-from importlib.resources import files
 
 from loguru import logger
 
 from provisioner.infra.context import Context
 
 
 class Paths:
```

## Comparing `provisioner_runtime-0.1.2.dist-info/LICENSE` & `provisioner_runtime-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `provisioner_runtime-0.1.2.dist-info/METADATA` & `provisioner_runtime-0.1.3.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: provisioner-runtime
-Version: 0.1.2
+Version: 0.1.3
 Summary: Provision Everything Anywhere
 Author: Zachi Nachshon
 Author-email: zachi.nachshon@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: ansible (>=7.3.0,<8.0.0)
+Requires-Dist: ansible (>=7.3,<10.0)
 Requires-Dist: ansible-runner (>=2.3.2,<3.0.0)
-Requires-Dist: inquirer (>=2.10.0,<3.0.0)
-Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: inquirer (>=2.10,<4.0)
+Requires-Dist: loguru (>=0.6,<0.8)
 Requires-Dist: python-hosts (>=1.0.3,<2.0.0)
 Requires-Dist: python-libnmap (>=0.7.3,<0.8.0)
 Requires-Dist: python3-nmap (>=1.5.4,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: rich (>=12.5.1,<13.0.0)
-Requires-Dist: typer (>=0.6.1,<0.7.0)
+Requires-Dist: rich (>=12.5.1,<14.0.0)
+Requires-Dist: typer (>=0.6.1,<0.13.0)
```

## Comparing `provisioner_runtime-0.1.2.dist-info/RECORD` & `provisioner_runtime-0.1.3.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -51,24 +51,24 @@
 external/ansible_playbooks/playbooks/roles/rpi_config_node/defaults/main.yaml,sha256=SrOwxbGR7euzGhg2igWyNLqG-q6U2n628A1h5Yzy2NE,2084
 external/ansible_playbooks/playbooks/roles/rpi_config_node/files/raspi_configure_node.sh,sha256=hpj7IxJZxlD4k09XlwxfXykRmB_9pIneBr38Fk_tts4,7734
 external/ansible_playbooks/playbooks/roles/rpi_config_node/files/shell_lib.sh,sha256=azJjTVQelJP3ValKDPsNpKL587P456KdRzM2Ev-Oi38,5549
 external/ansible_playbooks/playbooks/roles/rpi_config_node/tasks/main.yaml,sha256=09EagGfqvctPhoXUjBIUFFXbboAbpEgpIegbrmBdw60,1529
 external/ansible_playbooks/playbooks/shutdown.yaml,sha256=juJBsgpK-MlHYHB-awhmMC_tmbBZQJ3UrDM0dNpA2VE,419
 provisioner/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-provisioner/cli/entrypoint.py,sha256=X9wAFGzfbhtYmPJIz_J4rXT3JDGmKqapP5Q1N5yf9AM,3471
+provisioner/cli/entrypoint.py,sha256=BR5wKMrs8C1hGBJgsl3VdYXWofUA9u0QS3qR5-xV-W4,3651
 provisioner/cli/state.py,sha256=Kkz62UrJKO_nxw78BHg1yPa0vQ-DWN50_tozcc4VtLM,2325
 provisioner/cli/typer_callbacks.py,sha256=4M6shmRnPHUQxsAGEGJU5fn1tesTnFGfZHAaiLP-xwQ,1400
 provisioner/colors/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/colors/color.py,sha256=Gk-x59hUyLvadnhqmQpE7OahO7dQgRXh87btlaaZusg,380
 provisioner/config/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/config/domain/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/config/domain/config.py,sha256=41CGkxWuN14O26Uf1sWmVR9o7kr7Nu4BoJA5LXlbjoU,605
 provisioner/config/manager/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-provisioner/config/manager/config_manager.py,sha256=CumzidPq42nWDPUOOwMJ52wCdTPfDNe9ySILSWJEkyo,5608
+provisioner/config/manager/config_manager.py,sha256=8zH3coyGJxBq1a0S0VliIeyDbvDZPjYdPl17onYMHa4,5580
 provisioner/config/reader/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/config/reader/config_reader.py,sha256=na_akhCk3bejjjjB6tPWdGQKCLu-Vxn5FthvgOlTHko,1599
 provisioner/domain/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/domain/serialize.py,sha256=yyfJ8qB0T1jjxPa_IkD2ZHQ59tXFnW4CHCE64iAnbrQ,1535
 provisioner/errors/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/errors/cli_errors.py,sha256=9ufroiazMcp7tVBrN5IgA5YD9ugRbV_Xr8rrRr3qz84,1045
 provisioner/func/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -78,18 +78,18 @@
 provisioner/info/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/info/system_reader.py,sha256=xpmz1wWOBS32xqjVRoV0UAjYSfKobzjoSe71NQ1PVLQ,3950
 provisioner/infra/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/infra/context.py,sha256=XKhLaNFaBxCCJrPKCH__cGDK2lzMRSl7OSjvfMT2b40,2452
 provisioner/infra/evaluator.py,sha256=kEukOBHkFgqD9_ntkXRuodfiU9sLgZ4d5mWsyeD02Is,2682
 provisioner/infra/log.py,sha256=61ST3qmrIf-CZUZtJVnKRgZp49vGeViQpUMp0nkVaqI,4102
 provisioner/infra/remote_context.py,sha256=U-7juzMelcFbuWzUfmgylMxrj88CczOo7vZ6fRyGlTQ,962
-provisioner/main.py,sha256=g1CaEd8t4g6BcpygFN-0y3p0fBAEIn_4PynzKCzlsE4,1673
+provisioner/main.py,sha256=xLg-poqJ_0yRT_1TuABTGTDBgi9q6xwyKRpUIYZZ9PU,1668
 provisioner/resources/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/resources/config.yaml,sha256=loN-e5Ptp7nKPssrjJ867g5RHppCYzwvVLfm5NoaVRE,26
-provisioner/resources/version.txt,sha256=Ee4juPwvxhnW6rYnettaUnJhBnrAHM_D4RhX9Vvxi80,5
+provisioner/resources/version.txt,sha256=2_CXjsK1h6XWGH_cxBzOn_LA647vrboOtR84QKtu60Y,5
 provisioner/runner/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/runner/ansible/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/runner/ansible/ansible_runner.py,sha256=eMOczcQPhp9flK481wyq0eMBAfGLdKhPkOew9CXgPgw,16182
 provisioner/runner/ansible/resources/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/runner/ansible/resources/ansible.cfg,sha256=SXL8xHPL8xT-g-DbOzqUlQzYRKEyHU6UfVGVE4ApCjo,1957
 provisioner/runner/ansible/resources/callback_plugins/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/runner/ansible/resources/callback_plugins/custom_yaml.py,sha256=zkuML167l04C6ddi15fQ64v-UZ-oICLiYlFCDcocfxI,5455
@@ -115,21 +115,21 @@
 provisioner/utils/hosts_file.py,sha256=JLMUUywOGaCxkb3_2Yc9UhewQc5WZBtrwE_QnvQsRag,1955
 provisioner/utils/httpclient.py,sha256=-zhvG0fLUuzP5YRCMIY_aUDBUuGAMK2qUhBCg_-b2yM,6136
 provisioner/utils/io_utils.py,sha256=k_5NEWHCfZfFiFoZfyWblVt6_rZ2YcypcI5NiMndIDc,7052
 provisioner/utils/json_util.py,sha256=ktri9CwcYL1BQS1g6oEIj3zLx4ichqkTRQopS9IoXuA,2130
 provisioner/utils/network.py,sha256=DrRPNVmD7LB7_fePjh4UJdZL6bTf_UOiG7uB6pkpIho,4259
 provisioner/utils/os.py,sha256=TKexh743-Ho9bmcQ1Arax17SZJ43bjL_f1lxC5o7A9s,2043
 provisioner/utils/package_loader.py,sha256=aIMe5hvmLfEPzMjGrjEZDXSy7xi27Uw6U_7R7dpvdOk,4204
-provisioner/utils/paths.py,sha256=rRS8vUhWOhmPSxEfpVD1qDzIuFHlK0KYdqbEx1yZZYs,5034
+provisioner/utils/paths.py,sha256=ifqRgTjdDV7AbMB9myEGS3VwLzwYhVDHWIX9o5Z4oXY,5034
 provisioner/utils/patterns.py,sha256=rAzcbwFjZ3RDVlsoGBUhEFzN_EnEucETcmQV-f74FQM,2045
 provisioner/utils/printer.py,sha256=mv11OXCcuaZZL7wToF9Tq1MD3MA7SiBA2FXz86RK5tc,2427
 provisioner/utils/process.py,sha256=9J2ZKkYKifgd51cpJ7JW8lYSMkBVKfXFdJelJ5z5XPc,2103
 provisioner/utils/progress_indicator.py,sha256=hS2HuwUH-Fe5N3t-ClTyULiTwOhV20RHx16qrZTGCkA,8950
 provisioner/utils/prompter.py,sha256=RWhDat_577wsM1die636ctuuhNB1-dZWJqlA9bobLJw,8629
 provisioner/utils/properties.py,sha256=pPAV_NFRCfNvy6G87p_a2JpC7P5VRlviEFgORIiucBg,2165
 provisioner/utils/summary.py,sha256=U9dYFFJe_Nodw-1y52K650HOO2d35IVQoCZNU8qPUD4,2080
 provisioner/utils/yaml_util.py,sha256=-i1hIyh05hhJYa8bJBjreMfEaZdNkheU6zSvnhgVe-Y,2598
-provisioner_runtime-0.1.2.dist-info/LICENSE,sha256=rcr78KAutoVDcl3EaX33JjBsvfatzmlKWJ0-Ji3I7tk,1071
-provisioner_runtime-0.1.2.dist-info/METADATA,sha256=xpnnwi-2BxFKLNcnAAo0Lx7uqQxtJN0zrO_U75nyzuQ,802
-provisioner_runtime-0.1.2.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-provisioner_runtime-0.1.2.dist-info/entry_points.txt,sha256=YyXkOvQA01nCNiVumyuvhjPWhndn3ZwrvVGFQQ6O74k,53
-provisioner_runtime-0.1.2.dist-info/RECORD,,
+provisioner_runtime-0.1.3.dist-info/LICENSE,sha256=rcr78KAutoVDcl3EaX33JjBsvfatzmlKWJ0-Ji3I7tk,1071
+provisioner_runtime-0.1.3.dist-info/METADATA,sha256=sYDfOnwi3iGvMTFEhXtaVLeQFbIvzx_yOlzQbBROZQE,792
+provisioner_runtime-0.1.3.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+provisioner_runtime-0.1.3.dist-info/entry_points.txt,sha256=YyXkOvQA01nCNiVumyuvhjPWhndn3ZwrvVGFQQ6O74k,53
+provisioner_runtime-0.1.3.dist-info/RECORD,,
```

