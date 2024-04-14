# Comparing `tmp/dataos-cookiecutter-0.0.3.tar.gz` & `tmp/dataos-cookiecutter-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataos-cookiecutter-0.0.3.tar", last modified: Wed Apr 10 11:12:02 2024, max compression
+gzip compressed data, was "dataos-cookiecutter-0.0.4.tar", last modified: Sun Apr 14 12:13:29 2024, max compression
```

## Comparing `dataos-cookiecutter-0.0.3.tar` & `dataos-cookiecutter-0.0.4.tar`

### file list

```diff
@@ -1,40 +1,39 @@
-drwxr-xr-x   0 rakesh     (502) staff       (20)        0 2024-04-10 11:12:02.515271 dataos-cookiecutter-0.0.3/
--rw-r--r--   0 rakesh     (502) staff       (20)     2098 2024-04-10 11:12:02.514830 dataos-cookiecutter-0.0.3/PKG-INFO
--rw-r--r--   0 rakesh     (502) staff       (20)     1685 2024-04-10 09:22:05.000000 dataos-cookiecutter-0.0.3/README.md
-drwxr-xr-x   0 rakesh     (502) staff       (20)        0 2024-04-10 11:12:02.490901 dataos-cookiecutter-0.0.3/dataos_cookiecutter.egg-info/
--rw-r--r--   0 rakesh     (502) staff       (20)     2098 2024-04-10 11:12:02.000000 dataos-cookiecutter-0.0.3/dataos_cookiecutter.egg-info/PKG-INFO
--rw-r--r--   0 rakesh     (502) staff       (20)      891 2024-04-10 11:12:02.000000 dataos-cookiecutter-0.0.3/dataos_cookiecutter.egg-info/SOURCES.txt
--rw-r--r--   0 rakesh     (502) staff       (20)        1 2024-04-10 11:12:02.000000 dataos-cookiecutter-0.0.3/dataos_cookiecutter.egg-info/dependency_links.txt
--rw-r--r--   0 rakesh     (502) staff       (20)       43 2024-04-10 11:12:02.000000 dataos-cookiecutter-0.0.3/dataos_cookiecutter.egg-info/entry_points.txt
--rw-r--r--   0 rakesh     (502) staff       (20)       96 2024-04-10 11:12:02.000000 dataos-cookiecutter-0.0.3/dataos_cookiecutter.egg-info/requires.txt
--rw-r--r--   0 rakesh     (502) staff       (20)        6 2024-04-10 11:12:02.000000 dataos-cookiecutter-0.0.3/dataos_cookiecutter.egg-info/top_level.txt
-drwxr-xr-x   0 rakesh     (502) staff       (20)        0 2024-04-10 11:12:02.495805 dataos-cookiecutter-0.0.3/lens2/
--rw-r--r--   0 rakesh     (502) staff       (20)        0 2024-04-10 10:50:37.000000 dataos-cookiecutter-0.0.3/lens2/__init__.py
-drwxr-xr-x   0 rakesh     (502) staff       (20)        0 2024-04-10 11:12:02.499616 dataos-cookiecutter-0.0.3/lens2/checks/
--rw-r--r--   0 rakesh     (502) staff       (20)        0 2024-03-15 11:23:17.000000 dataos-cookiecutter-0.0.3/lens2/checks/__init__.py
--rw-r--r--   0 rakesh     (502) staff       (20)    10330 2024-04-10 10:08:02.000000 dataos-cookiecutter-0.0.3/lens2/checks/create_checks.py
--rw-r--r--   0 rakesh     (502) staff       (20)     2871 2024-04-10 09:32:27.000000 dataos-cookiecutter-0.0.3/lens2/checks/schema_check.py
--rw-r--r--   0 rakesh     (502) staff       (20)     5636 2024-03-12 13:05:50.000000 dataos-cookiecutter-0.0.3/lens2/checks/soda_cl_sql_mappings.py
--rw-r--r--   0 rakesh     (502) staff       (20)      278 2024-04-09 12:28:48.000000 dataos-cookiecutter-0.0.3/lens2/constants.py
-drwxr-xr-x   0 rakesh     (502) staff       (20)        0 2024-04-10 11:12:02.502666 dataos-cookiecutter-0.0.3/lens2/lens/
--rw-r--r--   0 rakesh     (502) staff       (20)        0 2024-03-15 11:23:24.000000 dataos-cookiecutter-0.0.3/lens2/lens/__init__.py
--rw-r--r--   0 rakesh     (502) staff       (20)     3814 2024-04-10 10:03:38.000000 dataos-cookiecutter-0.0.3/lens2/lens/create_lens.py
--rw-r--r--   0 rakesh     (502) staff       (20)     3010 2024-04-10 10:00:58.000000 dataos-cookiecutter-0.0.3/lens2/lens/env_vars_mapping.py
-drwxr-xr-x   0 rakesh     (502) staff       (20)        0 2024-04-10 11:12:02.509350 dataos-cookiecutter-0.0.3/lens2/lens/resources/
--rw-r--r--   0 rakesh     (502) staff       (20)      155 2024-03-28 11:42:35.000000 dataos-cookiecutter-0.0.3/lens2/lens/resources/Makefile
--rw-r--r--   0 rakesh     (502) staff       (20)     2012 2024-04-10 09:46:04.000000 dataos-cookiecutter-0.0.3/lens2/lens/resources/docker-compose.yaml
--rw-r--r--   0 rakesh     (502) staff       (20)      323 2024-04-10 09:44:35.000000 dataos-cookiecutter-0.0.3/lens2/lens/resources/env.env
--rw-r--r--   0 rakesh     (502) staff       (20)       39 2024-03-14 07:46:27.000000 dataos-cookiecutter-0.0.3/lens2/lens/resources/sql_sample.sql
--rw-r--r--   0 rakesh     (502) staff       (20)     1323 2024-04-10 10:04:49.000000 dataos-cookiecutter-0.0.3/lens2/lens/resources/table_sample.yaml
--rw-r--r--   0 rakesh     (502) staff       (20)      485 2024-03-14 07:46:55.000000 dataos-cookiecutter-0.0.3/lens2/lens/resources/view_sample.yaml
--rwxr-xr-x   0 rakesh     (502) staff       (20)      725 2024-04-10 11:05:55.000000 dataos-cookiecutter-0.0.3/lens2/lens2.py
-drwxr-xr-x   0 rakesh     (502) staff       (20)        0 2024-04-10 11:12:02.513660 dataos-cookiecutter-0.0.3/lens2/rill/
--rw-r--r--   0 rakesh     (502) staff       (20)        0 2024-03-15 11:23:32.000000 dataos-cookiecutter-0.0.3/lens2/rill/__init__.py
--rw-r--r--   0 rakesh     (502) staff       (20)      464 2024-03-29 10:53:53.000000 dataos-cookiecutter-0.0.3/lens2/rill/create_rill.py
--rw-r--r--   0 rakesh     (502) staff       (20)     9014 2024-04-10 09:33:14.000000 dataos-cookiecutter-0.0.3/lens2/rill/generate_rill.py
--rw-r--r--   0 rakesh     (502) staff       (20)      515 2024-04-10 09:36:01.000000 dataos-cookiecutter-0.0.3/lens2/rill/start_rill.py
--rw-r--r--   0 rakesh     (502) staff       (20)      364 2024-04-10 11:08:18.000000 dataos-cookiecutter-0.0.3/lens2/setup.py
--rw-r--r--   0 rakesh     (502) staff       (20)      965 2024-04-10 11:08:01.000000 dataos-cookiecutter-0.0.3/lens2/utils.py
--rw-r--r--   0 rakesh     (502) staff       (20)      147 2024-03-29 13:54:13.000000 dataos-cookiecutter-0.0.3/pyproject.toml
--rw-r--r--   0 rakesh     (502) staff       (20)       38 2024-04-10 11:12:02.515415 dataos-cookiecutter-0.0.3/setup.cfg
--rw-r--r--   0 rakesh     (502) staff       (20)     1107 2024-04-10 11:09:03.000000 dataos-cookiecutter-0.0.3/setup.py
+drwxr-xr-x   0 rakesh     (502) staff       (20)        0 2024-04-14 12:13:29.199767 dataos-cookiecutter-0.0.4/
+-rw-r--r--   0 rakesh     (502) staff       (20)     2282 2024-04-14 12:13:29.199210 dataos-cookiecutter-0.0.4/PKG-INFO
+-rw-r--r--   0 rakesh     (502) staff       (20)     1869 2024-04-14 12:12:46.000000 dataos-cookiecutter-0.0.4/README.md
+drwxr-xr-x   0 rakesh     (502) staff       (20)        0 2024-04-14 12:13:29.157629 dataos-cookiecutter-0.0.4/dataos_cookiecutter.egg-info/
+-rw-r--r--   0 rakesh     (502) staff       (20)     2282 2024-04-14 12:13:28.000000 dataos-cookiecutter-0.0.4/dataos_cookiecutter.egg-info/PKG-INFO
+-rw-r--r--   0 rakesh     (502) staff       (20)      867 2024-04-14 12:13:28.000000 dataos-cookiecutter-0.0.4/dataos_cookiecutter.egg-info/SOURCES.txt
+-rw-r--r--   0 rakesh     (502) staff       (20)        1 2024-04-14 12:13:28.000000 dataos-cookiecutter-0.0.4/dataos_cookiecutter.egg-info/dependency_links.txt
+-rw-r--r--   0 rakesh     (502) staff       (20)       43 2024-04-14 12:13:28.000000 dataos-cookiecutter-0.0.4/dataos_cookiecutter.egg-info/entry_points.txt
+-rw-r--r--   0 rakesh     (502) staff       (20)       96 2024-04-14 12:13:28.000000 dataos-cookiecutter-0.0.4/dataos_cookiecutter.egg-info/requires.txt
+-rw-r--r--   0 rakesh     (502) staff       (20)        6 2024-04-14 12:13:28.000000 dataos-cookiecutter-0.0.4/dataos_cookiecutter.egg-info/top_level.txt
+drwxr-xr-x   0 rakesh     (502) staff       (20)        0 2024-04-14 12:13:29.166298 dataos-cookiecutter-0.0.4/lens2/
+-rw-r--r--   0 rakesh     (502) staff       (20)        0 2024-04-14 09:53:15.000000 dataos-cookiecutter-0.0.4/lens2/__init__.py
+drwxr-xr-x   0 rakesh     (502) staff       (20)        0 2024-04-14 12:13:29.173072 dataos-cookiecutter-0.0.4/lens2/board/
+-rw-r--r--   0 rakesh     (502) staff       (20)        0 2024-03-15 11:23:32.000000 dataos-cookiecutter-0.0.4/lens2/board/__init__.py
+-rw-r--r--   0 rakesh     (502) staff       (20)      731 2024-04-14 10:36:46.000000 dataos-cookiecutter-0.0.4/lens2/board/create_board.py
+-rw-r--r--   0 rakesh     (502) staff       (20)     9419 2024-04-14 09:46:36.000000 dataos-cookiecutter-0.0.4/lens2/board/generate_board.py
+-rw-r--r--   0 rakesh     (502) staff       (20)      544 2024-04-14 09:43:23.000000 dataos-cookiecutter-0.0.4/lens2/board/start_board.py
+drwxr-xr-x   0 rakesh     (502) staff       (20)        0 2024-04-14 12:13:29.180655 dataos-cookiecutter-0.0.4/lens2/checks/
+-rw-r--r--   0 rakesh     (502) staff       (20)        0 2024-03-15 11:23:17.000000 dataos-cookiecutter-0.0.4/lens2/checks/__init__.py
+-rw-r--r--   0 rakesh     (502) staff       (20)    10687 2024-04-14 09:09:10.000000 dataos-cookiecutter-0.0.4/lens2/checks/create_checks.py
+-rw-r--r--   0 rakesh     (502) staff       (20)     2895 2024-04-14 09:38:22.000000 dataos-cookiecutter-0.0.4/lens2/checks/schema_check.py
+-rw-r--r--   0 rakesh     (502) staff       (20)     5636 2024-03-12 13:05:50.000000 dataos-cookiecutter-0.0.4/lens2/checks/soda_cl_sql_mappings.py
+-rw-r--r--   0 rakesh     (502) staff       (20)      256 2024-04-14 09:16:48.000000 dataos-cookiecutter-0.0.4/lens2/constants.py
+drwxr-xr-x   0 rakesh     (502) staff       (20)        0 2024-04-14 12:13:29.185522 dataos-cookiecutter-0.0.4/lens2/lens/
+-rw-r--r--   0 rakesh     (502) staff       (20)        0 2024-03-15 11:23:24.000000 dataos-cookiecutter-0.0.4/lens2/lens/__init__.py
+-rw-r--r--   0 rakesh     (502) staff       (20)     3579 2024-04-14 07:37:19.000000 dataos-cookiecutter-0.0.4/lens2/lens/create_lens.py
+drwxr-xr-x   0 rakesh     (502) staff       (20)        0 2024-04-14 12:13:29.197851 dataos-cookiecutter-0.0.4/lens2/lens/resources/
+-rw-r--r--   0 rakesh     (502) staff       (20)      155 2024-04-14 07:40:57.000000 dataos-cookiecutter-0.0.4/lens2/lens/resources/Makefile
+-rw-r--r--   0 rakesh     (502) staff       (20)      546 2024-04-14 06:48:57.000000 dataos-cookiecutter-0.0.4/lens2/lens/resources/docker-compose.yaml
+-rw-r--r--   0 rakesh     (502) staff       (20)      785 2024-04-14 06:50:23.000000 dataos-cookiecutter-0.0.4/lens2/lens/resources/env.env
+-rw-r--r--   0 rakesh     (502) staff       (20)       39 2024-03-14 07:46:27.000000 dataos-cookiecutter-0.0.4/lens2/lens/resources/sql_sample.sql
+-rw-r--r--   0 rakesh     (502) staff       (20)     1954 2024-04-14 07:17:31.000000 dataos-cookiecutter-0.0.4/lens2/lens/resources/table_sample.yaml
+-rw-r--r--   0 rakesh     (502) staff       (20)      458 2024-04-12 11:41:13.000000 dataos-cookiecutter-0.0.4/lens2/lens/resources/view_sample.yaml
+-rwxr-xr-x   0 rakesh     (502) staff       (20)      794 2024-04-14 10:36:52.000000 dataos-cookiecutter-0.0.4/lens2/lens2.py
+-rw-r--r--   0 rakesh     (502) staff       (20)      364 2024-04-12 11:17:19.000000 dataos-cookiecutter-0.0.4/lens2/setup.py
+-rw-r--r--   0 rakesh     (502) staff       (20)      953 2024-04-14 07:30:09.000000 dataos-cookiecutter-0.0.4/lens2/utils.py
+-rw-r--r--   0 rakesh     (502) staff       (20)      147 2024-03-29 13:54:13.000000 dataos-cookiecutter-0.0.4/pyproject.toml
+-rw-r--r--   0 rakesh     (502) staff       (20)       38 2024-04-14 12:13:29.200027 dataos-cookiecutter-0.0.4/setup.cfg
+-rw-r--r--   0 rakesh     (502) staff       (20)     1107 2024-04-12 11:17:15.000000 dataos-cookiecutter-0.0.4/setup.py
```

### Comparing `dataos-cookiecutter-0.0.3/PKG-INFO` & `dataos-cookiecutter-0.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataos-cookiecutter
-Version: 0.0.3
+Version: 0.0.4
 Summary: Dataos Cookiecutter
 Home-page: https://bitbucket.org/rubik_/dataos-cookiecutter
 Author: devendrasr
 Author-email: devendra@tmdc.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,33 +28,33 @@
 dataos-cookiecutter offers several commands to simplify Lens2-related tasks:
 
 1. **lens2 lens**: This command allows users to get started by creating a sample template along with folder structure, which they can modify based on their needs. It includes two flags:
    - `-n lens_name`: Specifies the name of the Lens.
    - `-s source_type`: Specifies the type of data source.
 
     ```bash
-    lens2 lens create -n <lens_name> -s <source_type>
+    lens2 create -n <lens2_name> -d <lens2_dir_name> -s <source_type>
     ```
 
 2. **lens2 checks**: This command provides two subcommands:
-   - **schema-check**: Validates that all dimensions used in Lens2 tables are fulfilled by the SQL provided for them.
+   - **schema-check**: Validates that all dimensions used in Lens2 tables are fulfilled by the SQL provided of table.
    - **create**: Creates checks YAML files and stores them in the checks folder.
 
     ```bash
     # Validate dimensions in Lens2 tables
-    lens2 checks schema-check
+    lens2 checks schema-check -n tables/views '(comma separated)'
     
     # Create checks YAML files
-    lens2 checks create
+    lens2 checks create -n tables/views '(comma separated)'
     ```
 
-3. **lens2 rill**: This command provides two subcommands for Rill-related tasks:
-   - **create**: Creates Rill dashboard YAML for views made public in Lens2 and stores files in the Rill folder.
-   - **start**: Uses the generated Rill content and starts Rill to initiate the dashboard.
+3. **lens2 board**: This command provides two subcommands for Board-related tasks:
+   - **create**: Creates View Board YAML made public in Lens2 and stores files in the Board/View_name folder.
+   - **start**: Uses the generated Board content and starts Board to explore. This will only start board for only for first view/table.
 
     ```bash
     # Create Rill dashboard YAML for Lens2 views
-    lens2 rill create
+    lens2 board create -n tables/views '(comma separated)'
     
     # Start Rill with generated content
-    lens2 rill start
+    lens2 board start -n table/view
     ```
```

### Comparing `dataos-cookiecutter-0.0.3/README.md` & `dataos-cookiecutter-0.0.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -15,33 +15,33 @@
 dataos-cookiecutter offers several commands to simplify Lens2-related tasks:
 
 1. **lens2 lens**: This command allows users to get started by creating a sample template along with folder structure, which they can modify based on their needs. It includes two flags:
    - `-n lens_name`: Specifies the name of the Lens.
    - `-s source_type`: Specifies the type of data source.
 
     ```bash
-    lens2 lens create -n <lens_name> -s <source_type>
+    lens2 create -n <lens2_name> -d <lens2_dir_name> -s <source_type>
     ```
 
 2. **lens2 checks**: This command provides two subcommands:
-   - **schema-check**: Validates that all dimensions used in Lens2 tables are fulfilled by the SQL provided for them.
+   - **schema-check**: Validates that all dimensions used in Lens2 tables are fulfilled by the SQL provided of table.
    - **create**: Creates checks YAML files and stores them in the checks folder.
 
     ```bash
     # Validate dimensions in Lens2 tables
-    lens2 checks schema-check
+    lens2 checks schema-check -n tables/views '(comma separated)'
     
     # Create checks YAML files
-    lens2 checks create
+    lens2 checks create -n tables/views '(comma separated)'
     ```
 
-3. **lens2 rill**: This command provides two subcommands for Rill-related tasks:
-   - **create**: Creates Rill dashboard YAML for views made public in Lens2 and stores files in the Rill folder.
-   - **start**: Uses the generated Rill content and starts Rill to initiate the dashboard.
+3. **lens2 board**: This command provides two subcommands for Board-related tasks:
+   - **create**: Creates View Board YAML made public in Lens2 and stores files in the Board/View_name folder.
+   - **start**: Uses the generated Board content and starts Board to explore. This will only start board for only for first view/table.
 
     ```bash
     # Create Rill dashboard YAML for Lens2 views
-    lens2 rill create
+    lens2 board create -n tables/views '(comma separated)'
     
     # Start Rill with generated content
-    lens2 rill start
+    lens2 board start -n table/view
     ```
```

### Comparing `dataos-cookiecutter-0.0.3/dataos_cookiecutter.egg-info/PKG-INFO` & `dataos-cookiecutter-0.0.4/dataos_cookiecutter.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataos-cookiecutter
-Version: 0.0.3
+Version: 0.0.4
 Summary: Dataos Cookiecutter
 Home-page: https://bitbucket.org/rubik_/dataos-cookiecutter
 Author: devendrasr
 Author-email: devendra@tmdc.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,33 +28,33 @@
 dataos-cookiecutter offers several commands to simplify Lens2-related tasks:
 
 1. **lens2 lens**: This command allows users to get started by creating a sample template along with folder structure, which they can modify based on their needs. It includes two flags:
    - `-n lens_name`: Specifies the name of the Lens.
    - `-s source_type`: Specifies the type of data source.
 
     ```bash
-    lens2 lens create -n <lens_name> -s <source_type>
+    lens2 create -n <lens2_name> -d <lens2_dir_name> -s <source_type>
     ```
 
 2. **lens2 checks**: This command provides two subcommands:
-   - **schema-check**: Validates that all dimensions used in Lens2 tables are fulfilled by the SQL provided for them.
+   - **schema-check**: Validates that all dimensions used in Lens2 tables are fulfilled by the SQL provided of table.
    - **create**: Creates checks YAML files and stores them in the checks folder.
 
     ```bash
     # Validate dimensions in Lens2 tables
-    lens2 checks schema-check
+    lens2 checks schema-check -n tables/views '(comma separated)'
     
     # Create checks YAML files
-    lens2 checks create
+    lens2 checks create -n tables/views '(comma separated)'
     ```
 
-3. **lens2 rill**: This command provides two subcommands for Rill-related tasks:
-   - **create**: Creates Rill dashboard YAML for views made public in Lens2 and stores files in the Rill folder.
-   - **start**: Uses the generated Rill content and starts Rill to initiate the dashboard.
+3. **lens2 board**: This command provides two subcommands for Board-related tasks:
+   - **create**: Creates View Board YAML made public in Lens2 and stores files in the Board/View_name folder.
+   - **start**: Uses the generated Board content and starts Board to explore. This will only start board for only for first view/table.
 
     ```bash
     # Create Rill dashboard YAML for Lens2 views
-    lens2 rill create
+    lens2 board create -n tables/views '(comma separated)'
     
     # Start Rill with generated content
-    lens2 rill start
+    lens2 board start -n table/view
     ```
```

### Comparing `dataos-cookiecutter-0.0.3/dataos_cookiecutter.egg-info/SOURCES.txt` & `dataos-cookiecutter-0.0.4/dataos_cookiecutter.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -8,24 +8,23 @@
 dataos_cookiecutter.egg-info/requires.txt
 dataos_cookiecutter.egg-info/top_level.txt
 lens2/__init__.py
 lens2/constants.py
 lens2/lens2.py
 lens2/setup.py
 lens2/utils.py
+lens2/board/__init__.py
+lens2/board/create_board.py
+lens2/board/generate_board.py
+lens2/board/start_board.py
 lens2/checks/__init__.py
 lens2/checks/create_checks.py
 lens2/checks/schema_check.py
 lens2/checks/soda_cl_sql_mappings.py
 lens2/lens/__init__.py
 lens2/lens/create_lens.py
-lens2/lens/env_vars_mapping.py
 lens2/lens/resources/Makefile
 lens2/lens/resources/docker-compose.yaml
 lens2/lens/resources/env.env
 lens2/lens/resources/sql_sample.sql
 lens2/lens/resources/table_sample.yaml
-lens2/lens/resources/view_sample.yaml
-lens2/rill/__init__.py
-lens2/rill/create_rill.py
-lens2/rill/generate_rill.py
-lens2/rill/start_rill.py
+lens2/lens/resources/view_sample.yaml
```

### Comparing `dataos-cookiecutter-0.0.3/lens2/checks/create_checks.py` & `dataos-cookiecutter-0.0.4/lens2/checks/create_checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 from lens2.checks.schema_check import schema_check
 from lens2.checks.soda_cl_sql_mappings import check_type_sql_mappings
 from lens2.utils import get_lens_meta, get_env_or_throw
 from lens2.constants import LENS2_CHECKS_PATH
 
 
-def transformed_lens_meta_checks(meta):
+def transformed_lens_meta_checks(meta, tables_views):
     # column name, table name, check definition
     data = {}
     for table in meta.get('tables', []):
-        if table.get('public'):
+        if table.get('public') and table['name'] in tables_views:
             table_name = table['name']
             data[table_name] = {}
             for d in table.get('dimensions', []):
                 if d.get('meta', {}).get('checks') and d.get('public'):
                     data[table_name][d['name'].split('.')[1]] = d.get('meta', {}).get('checks')
     return data
 
@@ -147,19 +147,22 @@
                         print("aborted")
                 else:
                     with open(os.path.join(checks_file_path, f"{table_name}_checks.yaml"), 'w') as file:
                         file.write(yaml.dump({check_for: definition}, default_flow_style=False, sort_keys=False))
 
 
 def add_subparser(subparsers):
-    parser = subparsers.add_parser("checks")
-    # Add arguments for the "checks" sub-command
-    parser.add_argument("action", choices=["create", "schema-check"], help="Create checks yaml")
+    parser = subparsers.add_parser("checks", help="Create lens2 table checks or schema check")
+    parser.add_argument("action", choices=["create", "schema-check"], help="Create checks yaml or check table schema")
+
+    parser.add_argument("-n", "--name", required=True, help="Name of the tables/views (comma separated) to perform "
+                                                            "checks on")
 
 
 def execute_checks(args):
     lens_meta = get_lens_meta()
+    tables_views = [name.strip() for name in args.name.split(',')]
     if args.action == "create":
-        transformed_lens_meta = transformed_lens_meta_checks(lens_meta)
+        transformed_lens_meta = transformed_lens_meta_checks(lens_meta, tables_views)
         generate_soda_checks_yaml(transformed_lens_meta)
     elif args.action == "schema-check":
-        schema_check(lens_meta)
+        schema_check(lens_meta, tables_views)
```

### Comparing `dataos-cookiecutter-0.0.3/lens2/checks/schema_check.py` & `dataos-cookiecutter-0.0.4/lens2/checks/schema_check.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,41 +29,41 @@
             remaining_dims = [dim for dim in all_dims if dim not in missing_dims]
             return execute_query(cursor, remaining_dims, missing_dims, table)
         else:
             # If the error is not due to missing columns, return the final list of missing dimensions
             return missing_dims
 
 
-def schema_check(lens_meta):
+def schema_check(lens_meta, tables_views):
     # check if env file exist or not
     curr_dir = os.getcwd()
     folder_name = os.path.basename(curr_dir)
     env_file = ".env"
     if os.path.exists(env_file) is False:
         raise FileNotFoundError(
             f"`.env` file not found in folder - `{folder_name}`. Create a `.env` file in folder - `{folder_name}`")
 
     # check if required env exist or not.
     load_dotenv('.env')
-    required_envs = {'LENS2_DATAOS_USER_NAME': None,
-                     'LENS2_DATAOS_USER_APIKEY': None}
+    required_envs = {'DATAOS_USER_NAME': None,
+                     'DATAOS_USER_APIKEY': None}
     for k in required_envs.keys():
         required_envs[k] = get_env_or_throw(k)
 
     connection = psycopg2.connect(
         dbname="db",
-        user=required_envs['LENS2_DATAOS_USER_NAME'],
-        password=required_envs['LENS2_DATAOS_USER_APIKEY'],
+        user=required_envs['DATAOS_USER_NAME'],
+        password=required_envs['DATAOS_USER_APIKEY'],
         host="localhost",
         port=15432
     )
     cur = connection.cursor()
 
     for table in lens_meta.get('tables', []):
-        if table['public']:
+        if table['public'] and table['name'] in tables_views:
             all_dims = []
             for dim in table.get('dimensions', []):
                 if dim['public']:
                     name = dim['name']
                     dim_name = name.split('.')[1] if '.' in name else name
                     all_dims.append(dim_name)
             missing_dims = []
```

### Comparing `dataos-cookiecutter-0.0.3/lens2/checks/soda_cl_sql_mappings.py` & `dataos-cookiecutter-0.0.4/lens2/checks/soda_cl_sql_mappings.py`

 * *Files identical despite different names*

### Comparing `dataos-cookiecutter-0.0.3/lens2/lens/create_lens.py` & `dataos-cookiecutter-0.0.4/lens2/lens/create_lens.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import os
 import shutil
 
 import pkg_resources
 
-from lens2.lens.env_vars_mapping import env_var_mappings
-
 
 def create_project_structure(args):
     # Extract folder names from command line arguments
     lens_name = args.name
+    lens_dir = args.dir_name
     source_type = args.source_type
     parent_dir = args.parent_dir if args.parent_dir else os.getcwd()
 
     # Create main directory
-    main_dir = os.path.join(parent_dir, lens_name)
+    main_dir = os.path.join(parent_dir, lens_dir)
 
     # Check if the directory already exists
     if os.path.exists(main_dir):
         overwrite = input(
             f"The directory '{main_dir}' already exists. Do you want to overwrite it? (Y/n): ").strip().lower() or 'n'
         if overwrite != 'y':
             print("Aborted.")
@@ -58,40 +57,34 @@
                     os.path.join(main_dir, 'docker-compose.yaml'))
 
     shutil.copyfile(pkg_resources.resource_filename('lens2', 'lens/resources/Makefile'),
                     os.path.join(main_dir, 'Makefile'))
 
     shutil.copyfile(pkg_resources.resource_filename('lens2', 'lens/resources/env.env'), os.path.join(main_dir, '.env'))
 
-    if source_type in env_var_mappings.keys():
-        env_vars = env_var_mappings[source_type.lower()]
-        defaults = env_var_mappings['required']
-        pg_configs = env_var_mappings['lens_other_config']
-        defaults['LENS2_NAME'] = lens_name
-        env_vars.update(defaults)
-        env_vars.update(pg_configs)
-
-        with open(f"{main_dir}/.env", 'a+') as f:
-            f.write("\n")
-            for key, value in env_vars.items():
-                if key == 'LENS2_NAME':
-                    f.write(f"\n #Lens Configs\n")
-                    f.write(f"{key}={value}\n")
-                elif key == 'LENS2_BASE_URL':
-                    f.write(f"\n")
-                    f.write(f"{key}={value}\n")
-                else:
-                    f.write(f"{key}={value}\n")
+    with open(os.path.join(main_dir, '.env'), "r") as env_file:
+        lines = env_file.readlines()
+
+    for i, line in enumerate(lines):
+        if line.startswith("LENS2_NAME"):
+            lines[i] = f"{'LENS2_NAME'}={lens_name}\n"
+        elif line.startswith("LENS2_SOURCE_TYPE"):
+            lines[i] = f"{'LENS2_SOURCE_TYPE'}={source_type}\n"
+
+    # Write the modified lines back to the .env file
+    with open(os.path.join(main_dir, '.env'), "w") as env_file:
+        env_file.writelines(lines)
 
 
 def add_subparser(subparsers):
-    parser = subparsers.add_parser("lens")
+    parser = subparsers.add_parser("create", help="Create lens2 template")
     parser.set_defaults(func=execute_lens)
-    parser.add_argument("action", choices=["create"], help="Create lens yaml")
+    parser.add_argument("-d", "--dir-name", required=True, help="Name of lens folder")
     parser.add_argument("-n", "--name", required=True, help="Name of the lens")
-    parser.add_argument("-s", "--source-type", required=True, help="Type of the source (e.g., postgres, mysql)")
-    parser.add_argument("-p", "--parent-dir", help="Parent directory where the lens directory will be created")
+    parser.add_argument("-s", "--source-type", required=False,
+                        help="Type of the source (e.g., depot, themis or minerva)")
+    parser.add_argument("-p", "--parent-dir", required=False,
+                        help="Parent directory where the lens directory will be created")
 
 
 def execute_lens(args):
-    if args.action == "create":
-        create_project_structure(args)
+    create_project_structure(args)
```

### Comparing `dataos-cookiecutter-0.0.3/lens2/lens/resources/table_sample.yaml` & `dataos-cookiecutter-0.0.4/lens2/lens/resources/table_sample.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,57 @@
 tables:
   - name: table_name
-    sql: {{ load_sql('sql_file_name') }}
+    # Path of the sql file, example - {{table_name.sql}}
+    sql: {{ load_sql('sql_sample') }}
     description: Table description
-    data_source: data_source
+    # For visibility control of table
     public: true
 
-    joins:
-      - name: target_table
-        relationship: one_to_one
-        sql: TABLE.dimension_name = target_table.dimension_name
+    # To establish relationship with other table (this will always create left join)
+    # joins:
+    #   - name: target_table
+    #     relationship: one_to_one
+    #     sql: TABLE.dimension_name = target_table.dimension_name
 
     dimensions:
+        # Name should follow snake-case format
       - name: dimension_name
         title: dimension_title
         description: Dimension description
+        # Mapping of specific column from sql of the table to the dimension
         sql: dimension_sql
+        # Data type of the dimension (types - time, string, number and boolean)
         type: dimension_type
-        primary_key: true
+        # To make this dimension primary key set to true
+        primary_key: false
+        # To make this dimension accessible set to true
         public: true
-        sub_query: false
+        # To associate additional key value properties
         meta:
           key: value
 
     measures:
       - name: measure_name
         title: measure_title
+        description: Measure description
+        # Define custome SQL snippet or map dimension
         sql: measure_sql
+        # Set type for this measure (types - string,time,boolean,number,count,count_distinct,count_distinct_approx,sum,avg,min,max)
         type: string
-        description: string
         drill_members:
           - drill_members_name
+        # To apply additional filter
         filters:
           - sql: "{TABLE}.dimension_name = 'dimension_value' "
         meta:
           key: value
 
+    # To create pre-defined filter for table
     segments:
       - name: segment_name
         public: true
+        # SQL statement for filter
         sql: "{TABLE}.dimension_name = 'dimension_value' "
-
-#    pre_aggregations:
-#      - name: pre_aggregation_name
-#        dimensions:
-#          - dimension_name
-#        measures:
-#          - measure_name
-#        time_dimension: {TABLE}.time_dimension_name
-#        granularity: second
-#        partition_granularity: hour
-#        segments:
-#          - segment_name
+        meta:
+          # To apply pre-defined filter by default to user groups
+          secure:
+            user_group: default
```

### Comparing `dataos-cookiecutter-0.0.3/lens2/lens2.py` & `dataos-cookiecutter-0.0.4/lens2/lens2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # main script
 import argparse
 from lens2.checks import create_checks
 from lens2.lens import create_lens
-from lens2.rill import create_rill
+from lens2.board import create_board
 
 
 def main():
     parser = argparse.ArgumentParser(description="Command-line interface for lens2")
     subparsers = parser.add_subparsers(dest="subcommand")
 
     create_checks.add_subparser(subparsers)
     create_lens.add_subparser(subparsers)
-    create_rill.add_subparser(subparsers)
+    create_board.add_subparser(subparsers)
 
     args = parser.parse_args()
 
-    if args.subcommand == "lens":
+    if args.subcommand == "create":
         create_lens.execute_lens(args)
     elif args.subcommand == "checks":
         create_checks.execute_checks(args)
-    elif args.subcommand == "rill":
-        create_rill.execute_rill(args)
+    elif args.subcommand == "board":
+        create_board.execute_board(args)
     else:
         parser.print_help()
+
+# Add table name soda view names board checks run schedule
+
```

### Comparing `dataos-cookiecutter-0.0.3/lens2/rill/generate_rill.py` & `dataos-cookiecutter-0.0.4/lens2/board/generate_board.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import subprocess
 
 import yaml
 from dotenv import load_dotenv
 from lens2.checks.schema_check import get_env_or_throw
 from sql_metadata import Parser
 
-from lens2.constants import LENS2_RILL_PATH
+from lens2.constants import LENS2_BOARD_PATH
 from lens2.utils import get_lens_meta
 
 load_dotenv('.env')
 
 
 def get_rill_version():
     try:
@@ -51,38 +51,38 @@
         return f"COUNT(DISTINCT {sql})"
     elif agg_type in ["count", "sum", "avg", "min", "max"]:
         return f"{agg_type}({sql})"
     elif agg_type in ["string", "time", "boolean", "number"]:
         return f"{sql}"
 
 
-def create_rill_json():
+def create_rill_json(views=None):
     lens_meta = get_lens_meta()
     lens_name = lens_meta['name']
     transformed_lens_meta = measure_dimension_sqls(lens_meta)
-    rill_data = {}
+    boards_data = {}
     for v in lens_meta['tables']:
-        if v['type'] == 'view':
-            print(f"Generating rill yaml for - {v['name']}")
-            rill_data[v['name']] = {'sql': '',
-                                    'dimensions': [],
-                                    'measures': [],
-                                    'timeseries': ''
-                                    }
+        if v['type'] == 'view' and v['name'] in views:
+            print(f"Generating board yaml for - {v['name']}")
+            boards_data[v['name']] = {'sql': '',
+                                      'dimensions': [],
+                                      'measures': [],
+                                      'timeseries': ''
+                                      }
             existing_dimensions = []
 
             if len(v['dimensions']) == 0:
                 print(f"No dimension found  for view - `{v['name']}`")
 
             for d in v['dimensions']:
                 d_name = d['name'].split('.')[1]
                 # check if dimension is type of time
-                if d['type'] == 'time' and rill_data[v['name']]['timeseries'] == '':
-                    rill_data[v['name']]['timeseries'] = d_name
-                rill_data[v['name']]['dimensions'].append({
+                if d['type'] == 'time' and boards_data[v['name']]['timeseries'] == '':
+                    boards_data[v['name']]['timeseries'] = d_name
+                boards_data[v['name']]['dimensions'].append({
                     "label": d['shortTitle'],
                     "description": d.get('description', d['title']),
                     "name": d_name,
                     "property": d_name
                 })
                 existing_dimensions.append(d_name)
             for m in v['measures']:
@@ -105,101 +105,108 @@
                         if m_dim_name_with_table not in existing_dimensions:
                             is_skip = True  # If any dimension is missing, we set to skip
                             print(
                                 f"Skipping measure - `{m_name}`, its dependent dimension - `{m_dim_name}` is missing "
                                 f"in view - `{v['name']}`")
                             break
                     if is_skip is False:
-                        rill_data[v['name']]['measures'].append({
+                        boards_data[v['name']]['measures'].append({
                             "label": m['shortTitle'],
                             "name": m_name,
                             "description": m.get('description', m['title']),
                             "expression": get_sql_expression(m['aggType'], measure_sql, m_alias.split('.')[0],
                                                              is_prefix)
                         })
 
-            rill_data[v['name']]['sql'] = f"SELECT {', '.join([_['name'] for _ in rill_data[v['name']]['dimensions']])}" \
-                                          f" FROM {v['name']}"
+            boards_data[v['name']][
+                'sql'] = f"SELECT {', '.join([_['name'] for _ in boards_data[v['name']]['dimensions']])}" \
+                         f" FROM {v['name']}"
     # print('\n')
-    return rill_data, lens_name
+    return boards_data, lens_name
 
 
-def dir_check(rill_path=None):
-    if not os.path.exists(rill_path):
-        os.makedirs(rill_path)
-    # Check if sub folders 'dashboards', 'models', and 'sources' exist within 'rill' folder
-    sub_folders_path = ['dashboards', 'models', 'sources']
-    for sub_folder in sub_folders_path:
-        sub_folder_path = os.path.join(rill_path, sub_folder)
-        if not os.path.exists(sub_folder_path):
-            os.makedirs(sub_folder_path)
-    return rill_path
+def dir_check_and_create(boards_path=None, views=None):
+    if not os.path.exists(boards_path):
+        os.makedirs(boards_path)
+
+    # Add dir for each view
+    for v in views:
+        view_board_dir = os.path.join(boards_path, v)
+        if not os.path.exists(view_board_dir):
+            os.makedirs(view_board_dir)
+        # Check if sub folders 'dashboards', 'models', and 'sources' exist within 'board' folder
+        sub_folders_path = ['dashboards', 'models', 'sources']
+        for sub_folder in sub_folders_path:
+            sub_folder_path = os.path.join(view_board_dir, sub_folder)
+            if not os.path.exists(sub_folder_path):
+                os.makedirs(sub_folder_path)
 
 
-def create_rill_files(data, rill_path=None, lens_name=None, rill_version=None):
+def create_board_files(data, board_path=None, lens_name=None, board_version=None):
     curr_dir = os.getcwd()
     folder_name = os.path.basename(curr_dir)
     env_file = ".env"
     if os.path.exists(env_file) is False:
         raise FileNotFoundError(
             f"`.env` file not found in folder - `{folder_name}`. Create a `.env` file in folder - `{folder_name}`")
 
     # check if required env exist or not.
-    required_envs = {'LENS2_DATAOS_USER_APIKEY': None,
-                     'LENS2_DATAOS_USER_NAME': None}
+    required_envs = {'DATAOS_USER_APIKEY': None,
+                     'DATAOS_USER_NAME': None}
     for k in required_envs.keys():
         required_envs[k] = get_env_or_throw(k)
 
     for k, v in data.items():
-        rill_yaml_path = os.path.join(rill_path, f"rill.yaml")
-        with open(rill_yaml_path, 'w') as file:
-            rill_data = {"compiler": "rill",
-                         "rill_version": rill_version,
-                         "name": lens_name}
-            file.write(yaml.dump(rill_data, default_flow_style=False, sort_keys=False))
+        view_board_path = os.path.join(board_path, k)
+        board_yaml_path = os.path.join(view_board_path, f"rill.yaml")
+        with open(board_yaml_path, 'w') as file:
+            board_data = {"compiler": "board",
+                          "rill_version": board_version,
+                          "name": lens_name}
+            file.write(yaml.dump(board_data, default_flow_style=False, sort_keys=False))
 
-        source_path = os.path.join(rill_path, f"sources/{k}.yaml")
+        source_path = os.path.join(view_board_path, f"sources/{k}.yaml")
         if os.path.exists(source_path):
             overwrite = input(f"The file `{source_path}` already exists. Do you want to overwrite it? (y/N): ")
             if overwrite.lower() != 'y':
                 break
         with open(source_path, 'w') as file:
             source = {"type": "postgres",
                       "sql": v['sql'],
-                      "database_url": f"postgres://{required_envs['LENS2_DATAOS_USER_NAME']}:"
-                                      f"{required_envs['LENS2_DATAOS_USER_APIKEY']}@localhost:15432/db"}
+                      "database_url": f"postgres://{required_envs['DATAOS_USER_NAME']}:"
+                                      f"{required_envs['DATAOS_USER_APIKEY']}@localhost:15432/db"}
             file.write(yaml.dump(source, default_flow_style=False, sort_keys=False))
 
-        model_path = os.path.join(rill_path, f"models/{k}_model.sql")
+        model_path = os.path.join(view_board_path, f"models/{k}_model.sql")
         if os.path.exists(model_path):
             overwrite = input(f"The file `{model_path}` already exists. Do you want to overwrite it? (y/N): ")
             if overwrite.lower() != 'y':
                 break
-        with open(os.path.join(rill_path, f"models/{k}_model.sql"), 'w') as file:
+        with open(os.path.join(view_board_path, f"models/{k}_model.sql"), 'w') as file:
             file.write(f"""SELECT * FROM {k}""")
 
-        dashboard_path = os.path.join(rill_path, f"dashboards/{k}_dashboard.yaml")
+        dashboard_path = os.path.join(view_board_path, f"dashboards/{k}_dashboard.yaml")
         if os.path.exists(dashboard_path):
             overwrite = input(f"The file `{dashboard_path}` already exists. Do you want to overwrite it? (y/N): ")
             if overwrite.lower() != 'y':
                 break
-        with open(os.path.join(rill_path, f"dashboards/{k}_dashboard.yaml"), 'w') as file:
+        with open(os.path.join(view_board_path, f"dashboards/{k}_dashboard.yaml"), 'w') as file:
             dashboard = {
                 "title": ' '.join([part.capitalize() for part in k.split('_')]),
                 "model": f"{k}_model",
                 "dimensions": v['dimensions'],
                 "measures": v['measures'],
                 "timeseries": v.get('timeseries', '')
             }
             file.write(yaml.dump(dashboard, default_flow_style=False, sort_keys=False))
 
 
 def add_create_subparser(subparsers):
     subparsers.set_defaults(func=execute_create)
 
 
-def execute_create():
-    rill_version = get_rill_version()
-    rill_path = get_env_or_throw(LENS2_RILL_PATH)
-    dir_check(rill_path)
-    rill_data, lens_name = create_rill_json()
-    create_rill_files(rill_data, rill_path=rill_path, lens_name=lens_name, rill_version=rill_version)
+def execute_create(views):
+    board_version = get_rill_version()
+    board_path = get_env_or_throw(LENS2_BOARD_PATH)
+    dir_check_and_create(board_path, views)
+    board_data, lens_name = create_rill_json(views)
+    create_board_files(board_data, board_path=board_path, lens_name=lens_name, board_version=board_version)
```

### Comparing `dataos-cookiecutter-0.0.3/lens2/rill/start_rill.py` & `dataos-cookiecutter-0.0.4/lens2/board/start_board.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-import re
 import subprocess
 import os
 from lens2.utils import get_env_or_throw
-from lens2.constants import LENS2_RILL_PATH
+from lens2.constants import LENS2_BOARD_PATH
 
 
 def add_start_subparser(subparsers):
     subparsers.set_defaults(func=executes_start)
 
 
-def executes_start():
+def executes_start(views):
     # Change directory to Rill directory
-    os.chdir(get_env_or_throw(LENS2_RILL_PATH))  # Change this to the actual path where Rill is installed
+    view_name = views[0]
+    view_board_path = os.path.join(get_env_or_throw(LENS2_BOARD_PATH), view_name)
 
-    # Run 'rill start --readonly' command
+    os.chdir(view_board_path)
+
+    # Run 'board start --readonly' command
     start_command = "rill start --readonly"
     subprocess.run(start_command, shell=True)
```

### Comparing `dataos-cookiecutter-0.0.3/lens2/utils.py` & `dataos-cookiecutter-0.0.4/lens2/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import requests
 
-from lens2.constants import LENS2_BASE_URL, LENS2_NAME, LENS2_META_PATH, LENS2_DATAOS_USER_APIKEY
+from lens2.constants import LENS2_BASE_URL, LENS2_NAME, LENS2_META_PATH, DATAOS_USER_APIKEY
 
 
 def get_env_or_throw(env_name):
     """Get the value of an environment variable or raise an error."""
     value = os.getenv(env_name)
     if value is None:
         raise ValueError(f"The environment variable '{env_name}' is not set.")
@@ -18,12 +18,12 @@
     return response.json()
 
 
 def get_lens_meta():
     lens2_base_url = get_env_or_throw(LENS2_BASE_URL)
     lens2_name = get_env_or_throw(LENS2_NAME)
     lens2_meta_path = get_env_or_throw(LENS2_META_PATH)
-    apikey = get_env_or_throw(LENS2_DATAOS_USER_APIKEY)
+    apikey = get_env_or_throw(DATAOS_USER_APIKEY)
 
     url = f"{lens2_base_url}/{lens2_name}{lens2_meta_path}?showPrivate=true"
     headers = {"Authorization": apikey}
     return make_api_call_with_headers(url, headers=headers)
```

### Comparing `dataos-cookiecutter-0.0.3/setup.py` & `dataos-cookiecutter-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 package_name = "dataos-cookiecutter"
-package_version = "0.0.3"
+package_version = "0.0.4"
 description = "Dataos cookiecutter python Package"
 
 setuptools.setup(
     name="dataos-cookiecutter",
     version=package_version,
     author="devendrasr",
     author_email="devendra@tmdc.io",
```

