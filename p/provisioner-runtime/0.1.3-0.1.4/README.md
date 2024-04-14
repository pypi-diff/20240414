# Comparing `tmp/provisioner_runtime-0.1.3-py3-none-any.whl.zip` & `tmp/provisioner_runtime-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 117286 bytes, number of entries: 135
+Zip file size: 131179 bytes, number of entries: 152
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 external/ansible_playbooks/__init__.py
 -rwxr-xr-x  2.0 unx      368 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/apt_update_upgrade.yaml
 -rwxr-xr-x  2.0 unx     5549 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/common/shell_lib.sh
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/group_vars/all
 -rwxr-xr-x  2.0 unx      678 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/reboot.yaml
 -rwxr-xr-x  2.0 unx      353 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/roles/anchor/defaults/main.yaml
 -rwxr-xr-x  2.0 unx    10424 b- defN 80-Jan-01 00:00 external/ansible_playbooks/playbooks/roles/anchor/files/anchor_run.sh
@@ -64,14 +64,15 @@
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/config/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/config/domain/__init__.py
 -rw-r--r--  2.0 unx      605 b- defN 80-Jan-01 00:00 provisioner/config/domain/config.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/config/manager/__init__.py
 -rw-r--r--  2.0 unx     5580 b- defN 80-Jan-01 00:00 provisioner/config/manager/config_manager.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/config/reader/__init__.py
 -rwxr-xr-x  2.0 unx     1599 b- defN 80-Jan-01 00:00 provisioner/config/reader/config_reader.py
+-rwxr-xr-x  2.0 unx     1869 b- defN 80-Jan-01 00:00 provisioner/config/reader/config_reader_fakes.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/domain/__init__.py
 -rwxr-xr-x  2.0 unx     1535 b- defN 80-Jan-01 00:00 provisioner/domain/serialize.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/errors/__init__.py
 -rwxr-xr-x  2.0 unx     1045 b- defN 80-Jan-01 00:00 provisioner/errors/cli_errors.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/func/__init__.py
 -rw-r--r--  2.0 unx     2838 b- defN 80-Jan-01 00:00 provisioner/func/either.py
 -rw-r--r--  2.0 unx      178 b- defN 80-Jan-01 00:00 provisioner/func/environment.py
@@ -85,22 +86,24 @@
 -rwxr-xr-x  2.0 unx      962 b- defN 80-Jan-01 00:00 provisioner/infra/remote_context.py
 -rwxr-xr-x  2.0 unx     1668 b- defN 80-Jan-01 00:00 provisioner/main.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/resources/__init__.py
 -rw-r--r--  2.0 unx       26 b- defN 80-Jan-01 00:00 provisioner/resources/config.yaml
 -rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 provisioner/resources/version.txt
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/runner/__init__.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/runner/ansible/__init__.py
+-rwxr-xr-x  2.0 unx     1228 b- defN 80-Jan-01 00:00 provisioner/runner/ansible/ansible_fakes.py
 -rw-r--r--  2.0 unx    16182 b- defN 80-Jan-01 00:00 provisioner/runner/ansible/ansible_runner.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/runner/ansible/resources/__init__.py
 -rwxr-xr-x  2.0 unx     1957 b- defN 80-Jan-01 00:00 provisioner/runner/ansible/resources/ansible.cfg
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/runner/ansible/resources/callback_plugins/__init__.py
 -rwxr-xr-x  2.0 unx     5455 b- defN 80-Jan-01 00:00 provisioner/runner/ansible/resources/callback_plugins/custom_yaml.py
 -rwxr-xr-x  2.0 unx     1081 b- defN 80-Jan-01 00:00 provisioner/runner/ansible/resources/callback_plugins/fail_on_missing_hosts.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/shared/__init__.py
 -rwxr-xr-x  2.0 unx     5942 b- defN 80-Jan-01 00:00 provisioner/shared/collaborators.py
+-rwxr-xr-x  2.0 unx     7806 b- defN 80-Jan-01 00:00 provisioner/shared/collaborators_fakes.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/test_data/__init__.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/test_data/ansible/__init__.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/test_data/ansible/playbooks/__init__.py
 -rw-r--r--  2.0 unx     2668 b- defN 80-Jan-01 00:00 provisioner/test_data/domain.py
 -rwxr-xr-x  2.0 unx      256 b- defN 80-Jan-01 00:00 provisioner/test_data/internal_config.yaml
 -rwxr-xr-x  2.0 unx      180 b- defN 80-Jan-01 00:00 provisioner/test_data/user_config.yaml
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/test_lib/__init__.py
@@ -108,30 +111,44 @@
 -rw-r--r--  2.0 unx     5577 b- defN 80-Jan-01 00:00 provisioner/test_lib/faker.py
 -rw-r--r--  2.0 unx      321 b- defN 80-Jan-01 00:00 provisioner/test_lib/test_cli_runner.py
 -rwxr-xr-x  2.0 unx     2383 b- defN 80-Jan-01 00:00 provisioner/test_lib/test_env.py
 -rwxr-xr-x  2.0 unx      280 b- defN 80-Jan-01 00:00 provisioner/test_lib/test_errors.py
 -rwxr-xr-x  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner/utils/__init__.py
 -rwxr-xr-x  2.0 unx      184 b- defN 80-Jan-01 00:00 provisioner/utils/browser.py
 -rwxr-xr-x  2.0 unx     1057 b- defN 80-Jan-01 00:00 provisioner/utils/checks.py
+-rwxr-xr-x  2.0 unx      931 b- defN 80-Jan-01 00:00 provisioner/utils/checks_fakes.py
 -rwxr-xr-x  2.0 unx     2268 b- defN 80-Jan-01 00:00 provisioner/utils/github.py
+-rwxr-xr-x  2.0 unx     4589 b- defN 80-Jan-01 00:00 provisioner/utils/github_fakes.py
 -rwxr-xr-x  2.0 unx     1955 b- defN 80-Jan-01 00:00 provisioner/utils/hosts_file.py
+-rwxr-xr-x  2.0 unx      949 b- defN 80-Jan-01 00:00 provisioner/utils/hosts_file_fakes.py
 -rwxr-xr-x  2.0 unx     6136 b- defN 80-Jan-01 00:00 provisioner/utils/httpclient.py
+-rwxr-xr-x  2.0 unx     1807 b- defN 80-Jan-01 00:00 provisioner/utils/httpclient_fakes.py
 -rwxr-xr-x  2.0 unx     7052 b- defN 80-Jan-01 00:00 provisioner/utils/io_utils.py
+-rwxr-xr-x  2.0 unx     5893 b- defN 80-Jan-01 00:00 provisioner/utils/io_utils_fakes.py
 -rwxr-xr-x  2.0 unx     2130 b- defN 80-Jan-01 00:00 provisioner/utils/json_util.py
 -rwxr-xr-x  2.0 unx     4259 b- defN 80-Jan-01 00:00 provisioner/utils/network.py
+-rwxr-xr-x  2.0 unx      929 b- defN 80-Jan-01 00:00 provisioner/utils/network_fakes.py
 -rwxr-xr-x  2.0 unx     2043 b- defN 80-Jan-01 00:00 provisioner/utils/os.py
 -rwxr-xr-x  2.0 unx     4204 b- defN 80-Jan-01 00:00 provisioner/utils/package_loader.py
 -rwxr-xr-x  2.0 unx     5034 b- defN 80-Jan-01 00:00 provisioner/utils/paths.py
+-rwxr-xr-x  2.0 unx     2444 b- defN 80-Jan-01 00:00 provisioner/utils/paths_fakes.py
 -rwxr-xr-x  2.0 unx     2045 b- defN 80-Jan-01 00:00 provisioner/utils/patterns.py
+-rwxr-xr-x  2.0 unx     1278 b- defN 80-Jan-01 00:00 provisioner/utils/patterns_fakes.py
 -rwxr-xr-x  2.0 unx     2427 b- defN 80-Jan-01 00:00 provisioner/utils/printer.py
+-rwxr-xr-x  2.0 unx     1531 b- defN 80-Jan-01 00:00 provisioner/utils/printer_fakes.py
 -rwxr-xr-x  2.0 unx     2103 b- defN 80-Jan-01 00:00 provisioner/utils/process.py
+-rwxr-xr-x  2.0 unx     1256 b- defN 80-Jan-01 00:00 provisioner/utils/process_fakes.py
 -rwxr-xr-x  2.0 unx     8950 b- defN 80-Jan-01 00:00 provisioner/utils/progress_indicator.py
+-rwxr-xr-x  2.0 unx     3215 b- defN 80-Jan-01 00:00 provisioner/utils/progress_indicator_fakes.py
 -rwxr-xr-x  2.0 unx     8629 b- defN 80-Jan-01 00:00 provisioner/utils/prompter.py
+-rwxr-xr-x  2.0 unx     2400 b- defN 80-Jan-01 00:00 provisioner/utils/prompter_fakes.py
 -rwxr-xr-x  2.0 unx     2165 b- defN 80-Jan-01 00:00 provisioner/utils/properties.py
+-rwxr-xr-x  2.0 unx     1310 b- defN 80-Jan-01 00:00 provisioner/utils/properties_fakes.py
 -rwxr-xr-x  2.0 unx     2080 b- defN 80-Jan-01 00:00 provisioner/utils/summary.py
+-rwxr-xr-x  2.0 unx     1401 b- defN 80-Jan-01 00:00 provisioner/utils/summary_fakes.py
 -rwxr-xr-x  2.0 unx     2598 b- defN 80-Jan-01 00:00 provisioner/utils/yaml_util.py
--rw-r--r--  2.0 unx     1071 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx      792 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.3.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx    14179 b- defN 16-Jan-01 00:00 provisioner_runtime-0.1.3.dist-info/RECORD
-135 files, 296800 bytes uncompressed, 93690 bytes compressed:  68.4%
+-rw-r--r--  2.0 unx     1071 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx      792 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 80-Jan-01 00:00 provisioner_runtime-0.1.4.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    15772 b- defN 16-Jan-01 00:00 provisioner_runtime-0.1.4.dist-info/RECORD
+152 files, 339229 bytes uncompressed, 105037 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -201,14 +201,17 @@
 
 Filename: provisioner/config/reader/__init__.py
 Comment: 
 
 Filename: provisioner/config/reader/config_reader.py
 Comment: 
 
+Filename: provisioner/config/reader/config_reader_fakes.py
+Comment: 
+
 Filename: provisioner/domain/__init__.py
 Comment: 
 
 Filename: provisioner/domain/serialize.py
 Comment: 
 
 Filename: provisioner/errors/__init__.py
@@ -264,14 +267,17 @@
 
 Filename: provisioner/runner/__init__.py
 Comment: 
 
 Filename: provisioner/runner/ansible/__init__.py
 Comment: 
 
+Filename: provisioner/runner/ansible/ansible_fakes.py
+Comment: 
+
 Filename: provisioner/runner/ansible/ansible_runner.py
 Comment: 
 
 Filename: provisioner/runner/ansible/resources/__init__.py
 Comment: 
 
 Filename: provisioner/runner/ansible/resources/ansible.cfg
@@ -288,14 +294,17 @@
 
 Filename: provisioner/shared/__init__.py
 Comment: 
 
 Filename: provisioner/shared/collaborators.py
 Comment: 
 
+Filename: provisioner/shared/collaborators_fakes.py
+Comment: 
+
 Filename: provisioner/test_data/__init__.py
 Comment: 
 
 Filename: provisioner/test_data/ansible/__init__.py
 Comment: 
 
 Filename: provisioner/test_data/ansible/playbooks/__init__.py
@@ -333,74 +342,116 @@
 
 Filename: provisioner/utils/browser.py
 Comment: 
 
 Filename: provisioner/utils/checks.py
 Comment: 
 
+Filename: provisioner/utils/checks_fakes.py
+Comment: 
+
 Filename: provisioner/utils/github.py
 Comment: 
 
+Filename: provisioner/utils/github_fakes.py
+Comment: 
+
 Filename: provisioner/utils/hosts_file.py
 Comment: 
 
+Filename: provisioner/utils/hosts_file_fakes.py
+Comment: 
+
 Filename: provisioner/utils/httpclient.py
 Comment: 
 
+Filename: provisioner/utils/httpclient_fakes.py
+Comment: 
+
 Filename: provisioner/utils/io_utils.py
 Comment: 
 
+Filename: provisioner/utils/io_utils_fakes.py
+Comment: 
+
 Filename: provisioner/utils/json_util.py
 Comment: 
 
 Filename: provisioner/utils/network.py
 Comment: 
 
+Filename: provisioner/utils/network_fakes.py
+Comment: 
+
 Filename: provisioner/utils/os.py
 Comment: 
 
 Filename: provisioner/utils/package_loader.py
 Comment: 
 
 Filename: provisioner/utils/paths.py
 Comment: 
 
+Filename: provisioner/utils/paths_fakes.py
+Comment: 
+
 Filename: provisioner/utils/patterns.py
 Comment: 
 
+Filename: provisioner/utils/patterns_fakes.py
+Comment: 
+
 Filename: provisioner/utils/printer.py
 Comment: 
 
+Filename: provisioner/utils/printer_fakes.py
+Comment: 
+
 Filename: provisioner/utils/process.py
 Comment: 
 
+Filename: provisioner/utils/process_fakes.py
+Comment: 
+
 Filename: provisioner/utils/progress_indicator.py
 Comment: 
 
+Filename: provisioner/utils/progress_indicator_fakes.py
+Comment: 
+
 Filename: provisioner/utils/prompter.py
 Comment: 
 
+Filename: provisioner/utils/prompter_fakes.py
+Comment: 
+
 Filename: provisioner/utils/properties.py
 Comment: 
 
+Filename: provisioner/utils/properties_fakes.py
+Comment: 
+
 Filename: provisioner/utils/summary.py
 Comment: 
 
+Filename: provisioner/utils/summary_fakes.py
+Comment: 
+
 Filename: provisioner/utils/yaml_util.py
 Comment: 
 
-Filename: provisioner_runtime-0.1.3.dist-info/LICENSE
+Filename: provisioner_runtime-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: provisioner_runtime-0.1.3.dist-info/METADATA
+Filename: provisioner_runtime-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: provisioner_runtime-0.1.3.dist-info/WHEEL
+Filename: provisioner_runtime-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: provisioner_runtime-0.1.3.dist-info/entry_points.txt
+Filename: provisioner_runtime-0.1.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: provisioner_runtime-0.1.3.dist-info/RECORD
+Filename: provisioner_runtime-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## provisioner/resources/version.txt

```diff
@@ -1 +1 @@
-0.1.3
+0.1.4
```

## Comparing `provisioner_runtime-0.1.3.dist-info/LICENSE` & `provisioner_runtime-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `provisioner_runtime-0.1.3.dist-info/METADATA` & `provisioner_runtime-0.1.4.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: provisioner-runtime
-Version: 0.1.3
+Version: 0.1.4
 Summary: Provision Everything Anywhere
 Author: Zachi Nachshon
 Author-email: zachi.nachshon@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

## Comparing `provisioner_runtime-0.1.3.dist-info/RECORD` & `provisioner_runtime-0.1.4.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 provisioner/config/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/config/domain/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/config/domain/config.py,sha256=41CGkxWuN14O26Uf1sWmVR9o7kr7Nu4BoJA5LXlbjoU,605
 provisioner/config/manager/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/config/manager/config_manager.py,sha256=8zH3coyGJxBq1a0S0VliIeyDbvDZPjYdPl17onYMHa4,5580
 provisioner/config/reader/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/config/reader/config_reader.py,sha256=na_akhCk3bejjjjB6tPWdGQKCLu-Vxn5FthvgOlTHko,1599
+provisioner/config/reader/config_reader_fakes.py,sha256=KBoctfdPZezObOujku5h--mAfxt4IO-o57YKD_5vbAo,1869
 provisioner/domain/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/domain/serialize.py,sha256=yyfJ8qB0T1jjxPa_IkD2ZHQ59tXFnW4CHCE64iAnbrQ,1535
 provisioner/errors/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/errors/cli_errors.py,sha256=9ufroiazMcp7tVBrN5IgA5YD9ugRbV_Xr8rrRr3qz84,1045
 provisioner/func/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/func/either.py,sha256=T5ypL9aHtipylkjIhKYPJmX9VYOn2poFmOejshIvmME,2838
 provisioner/func/environment.py,sha256=ZiWzqlGaf9FATqHk9-qlimKScNLcThdNngQJz9P9pdQ,178
@@ -81,25 +82,27 @@
 provisioner/infra/context.py,sha256=XKhLaNFaBxCCJrPKCH__cGDK2lzMRSl7OSjvfMT2b40,2452
 provisioner/infra/evaluator.py,sha256=kEukOBHkFgqD9_ntkXRuodfiU9sLgZ4d5mWsyeD02Is,2682
 provisioner/infra/log.py,sha256=61ST3qmrIf-CZUZtJVnKRgZp49vGeViQpUMp0nkVaqI,4102
 provisioner/infra/remote_context.py,sha256=U-7juzMelcFbuWzUfmgylMxrj88CczOo7vZ6fRyGlTQ,962
 provisioner/main.py,sha256=xLg-poqJ_0yRT_1TuABTGTDBgi9q6xwyKRpUIYZZ9PU,1668
 provisioner/resources/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/resources/config.yaml,sha256=loN-e5Ptp7nKPssrjJ867g5RHppCYzwvVLfm5NoaVRE,26
-provisioner/resources/version.txt,sha256=2_CXjsK1h6XWGH_cxBzOn_LA647vrboOtR84QKtu60Y,5
+provisioner/resources/version.txt,sha256=RTMGWu18lgJhojG0A1zJvOyL_2HOazONQ-nFDRU6RUY,5
 provisioner/runner/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/runner/ansible/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+provisioner/runner/ansible/ansible_fakes.py,sha256=1fIDJ4v8X2B7BBfmo_Ge6_If6mTaNEPOE-Mrz7066rQ,1228
 provisioner/runner/ansible/ansible_runner.py,sha256=eMOczcQPhp9flK481wyq0eMBAfGLdKhPkOew9CXgPgw,16182
 provisioner/runner/ansible/resources/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/runner/ansible/resources/ansible.cfg,sha256=SXL8xHPL8xT-g-DbOzqUlQzYRKEyHU6UfVGVE4ApCjo,1957
 provisioner/runner/ansible/resources/callback_plugins/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/runner/ansible/resources/callback_plugins/custom_yaml.py,sha256=zkuML167l04C6ddi15fQ64v-UZ-oICLiYlFCDcocfxI,5455
 provisioner/runner/ansible/resources/callback_plugins/fail_on_missing_hosts.py,sha256=VBPELMNY380V7UDAYUfyo4oEyuzypfLEgHSe-HazZ_k,1081
 provisioner/shared/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/shared/collaborators.py,sha256=eAHJ5y7xMJluYLyMsjyYAK2nvOixpGtu_SVhRHMHwkQ,5942
+provisioner/shared/collaborators_fakes.py,sha256=NtnFb9-jWS_PtOxKllrk9k6KTGWdGygKvXd0iDiiVIk,7806
 provisioner/test_data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/test_data/ansible/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/test_data/ansible/playbooks/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/test_data/domain.py,sha256=LlO_PiSDVgD7bNv2fwxpXF6Twqtdq_NvSzfppqNUIiY,2668
 provisioner/test_data/internal_config.yaml,sha256=sVjXtaLCA0xsMTJwM_BFlr-eaI1yWsqoi8HzCW8g7aM,256
 provisioner/test_data/user_config.yaml,sha256=j0EVnae8sD71qtLubasS-pKRwlpS2p88nkjd6f-hRfk,180
 provisioner/test_lib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -107,29 +110,43 @@
 provisioner/test_lib/faker.py,sha256=bny4VDmavzx-kpNt56u9WUNE7T_-r78PvqsomsIpGHg,5577
 provisioner/test_lib/test_cli_runner.py,sha256=6cvBKYn0QP23Ncel0KR0alhrcnZjnd8k4we5Jr2jx6Q,321
 provisioner/test_lib/test_env.py,sha256=Z-fRIx3IHTzsTBXh5QzlqsA2yBB2Nl1rcPKktOTfIcI,2383
 provisioner/test_lib/test_errors.py,sha256=C9-3uUJUmU9WuaX1fzKzlili0W1CGGzf0GhGnXCzSZ0,280
 provisioner/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner/utils/browser.py,sha256=hcobhmcK1qnesTHwj-u5hgXJsVWUjVRGP2yHdmjejnE,184
 provisioner/utils/checks.py,sha256=9KIAPscTyT-i2-4bfZ2tUsxysFdctfiN58mxxJ31uyQ,1057
+provisioner/utils/checks_fakes.py,sha256=W48dnyWJSnC_DU0hsyP0LDk1oolCj1sBOOMqgZLT_UE,931
 provisioner/utils/github.py,sha256=wMFi3jJR82rEywiJZrdg85ngdEtxZG8qf-kSVjazw-M,2268
+provisioner/utils/github_fakes.py,sha256=W9_LyeuHSpmv7sgBHd0DKJ7SZtRilUNRsn08hloq79M,4589
 provisioner/utils/hosts_file.py,sha256=JLMUUywOGaCxkb3_2Yc9UhewQc5WZBtrwE_QnvQsRag,1955
+provisioner/utils/hosts_file_fakes.py,sha256=Cck6tHSYoqPg5Qt7sRYXxJalxSanJVrdmEvxu7Pm150,949
 provisioner/utils/httpclient.py,sha256=-zhvG0fLUuzP5YRCMIY_aUDBUuGAMK2qUhBCg_-b2yM,6136
+provisioner/utils/httpclient_fakes.py,sha256=i3wYxUYeVd_4KTJ0J5rdNED8nmKuH-MytbfaClDQRhs,1807
 provisioner/utils/io_utils.py,sha256=k_5NEWHCfZfFiFoZfyWblVt6_rZ2YcypcI5NiMndIDc,7052
+provisioner/utils/io_utils_fakes.py,sha256=3Xq2LBVS1K1d6HH4TSqaKHwjp36uaoaURbsqyTXPrQo,5893
 provisioner/utils/json_util.py,sha256=ktri9CwcYL1BQS1g6oEIj3zLx4ichqkTRQopS9IoXuA,2130
 provisioner/utils/network.py,sha256=DrRPNVmD7LB7_fePjh4UJdZL6bTf_UOiG7uB6pkpIho,4259
+provisioner/utils/network_fakes.py,sha256=p5ji7K8dKBBdTvTjcpjJWtXVZ01hKkT3IoHfO-sJJ-4,929
 provisioner/utils/os.py,sha256=TKexh743-Ho9bmcQ1Arax17SZJ43bjL_f1lxC5o7A9s,2043
 provisioner/utils/package_loader.py,sha256=aIMe5hvmLfEPzMjGrjEZDXSy7xi27Uw6U_7R7dpvdOk,4204
 provisioner/utils/paths.py,sha256=ifqRgTjdDV7AbMB9myEGS3VwLzwYhVDHWIX9o5Z4oXY,5034
+provisioner/utils/paths_fakes.py,sha256=WXLUCMxoSRsNR0LXzJousT0Kks8k_QhppJAyMr3kcQY,2444
 provisioner/utils/patterns.py,sha256=rAzcbwFjZ3RDVlsoGBUhEFzN_EnEucETcmQV-f74FQM,2045
+provisioner/utils/patterns_fakes.py,sha256=crj_sgProqkdNcp0ywAo8BdD5mr-uNOZ14qlX6yoz34,1278
 provisioner/utils/printer.py,sha256=mv11OXCcuaZZL7wToF9Tq1MD3MA7SiBA2FXz86RK5tc,2427
+provisioner/utils/printer_fakes.py,sha256=DyctaeAsANV6G7Uof-YLFbMJUWh1nss_x7n5DPHFj7A,1531
 provisioner/utils/process.py,sha256=9J2ZKkYKifgd51cpJ7JW8lYSMkBVKfXFdJelJ5z5XPc,2103
+provisioner/utils/process_fakes.py,sha256=KCEvI2_OrJNWKQJXdpccHCiaVkxmE3TckySoKRweF7I,1256
 provisioner/utils/progress_indicator.py,sha256=hS2HuwUH-Fe5N3t-ClTyULiTwOhV20RHx16qrZTGCkA,8950
+provisioner/utils/progress_indicator_fakes.py,sha256=oQ7w5A-XvLdiZ46XSyHZMDC7ayG8JkIzODlGpCfjjQs,3215
 provisioner/utils/prompter.py,sha256=RWhDat_577wsM1die636ctuuhNB1-dZWJqlA9bobLJw,8629
+provisioner/utils/prompter_fakes.py,sha256=qqB7pikYvh8RIoArDFq1JYC1PaBdLleQFwC_Gp_ZbSY,2400
 provisioner/utils/properties.py,sha256=pPAV_NFRCfNvy6G87p_a2JpC7P5VRlviEFgORIiucBg,2165
+provisioner/utils/properties_fakes.py,sha256=1fsOQu9FTA12H2XH4I4Wn_H9Bg8hZqYVco-wn-pOHuk,1310
 provisioner/utils/summary.py,sha256=U9dYFFJe_Nodw-1y52K650HOO2d35IVQoCZNU8qPUD4,2080
+provisioner/utils/summary_fakes.py,sha256=YMm6sBiNw5MGCO-ILwnPx0u715_-vJOnyno1czLkeNM,1401
 provisioner/utils/yaml_util.py,sha256=-i1hIyh05hhJYa8bJBjreMfEaZdNkheU6zSvnhgVe-Y,2598
-provisioner_runtime-0.1.3.dist-info/LICENSE,sha256=rcr78KAutoVDcl3EaX33JjBsvfatzmlKWJ0-Ji3I7tk,1071
-provisioner_runtime-0.1.3.dist-info/METADATA,sha256=sYDfOnwi3iGvMTFEhXtaVLeQFbIvzx_yOlzQbBROZQE,792
-provisioner_runtime-0.1.3.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-provisioner_runtime-0.1.3.dist-info/entry_points.txt,sha256=YyXkOvQA01nCNiVumyuvhjPWhndn3ZwrvVGFQQ6O74k,53
-provisioner_runtime-0.1.3.dist-info/RECORD,,
+provisioner_runtime-0.1.4.dist-info/LICENSE,sha256=rcr78KAutoVDcl3EaX33JjBsvfatzmlKWJ0-Ji3I7tk,1071
+provisioner_runtime-0.1.4.dist-info/METADATA,sha256=X9i2MydGz8pAg-vNb8LSVSSGyl1E0y5SkZDcupMJnJA,792
+provisioner_runtime-0.1.4.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+provisioner_runtime-0.1.4.dist-info/entry_points.txt,sha256=YyXkOvQA01nCNiVumyuvhjPWhndn3ZwrvVGFQQ6O74k,53
+provisioner_runtime-0.1.4.dist-info/RECORD,,
```

