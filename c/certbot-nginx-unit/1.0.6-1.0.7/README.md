# Comparing `tmp/certbot-nginx-unit-1.0.6.tar.gz` & `tmp/certbot_nginx_unit-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-nginx-unit-1.0.6.tar", last modified: Tue Feb 13 00:03:54 2024, max compression
+gzip compressed data, was "certbot_nginx_unit-1.0.7.tar", last modified: Sat Apr 13 15:58:37 2024, max compression
```

## Comparing `certbot-nginx-unit-1.0.6.tar` & `certbot_nginx_unit-1.0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 00:03:54.428121 certbot-nginx-unit-1.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 00:03:54.424121 certbot-nginx-unit-1.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 00:03:54.424121 certbot-nginx-unit-1.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-02-13 00:03:41.000000 certbot-nginx-unit-1.0.6/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-02-13 00:03:41.000000 certbot-nginx-unit-1.0.6/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-13 00:03:41.000000 certbot-nginx-unit-1.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    21568 2024-02-13 00:03:41.000000 certbot-nginx-unit-1.0.6/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-02-13 00:03:41.000000 certbot-nginx-unit-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-02-13 00:03:54.428121 certbot-nginx-unit-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-02-13 00:03:41.000000 certbot-nginx-unit-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 00:03:54.424121 certbot-nginx-unit-1.0.6/certbot_nginx_unit/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-13 00:03:41.000000 certbot-nginx-unit-1.0.6/certbot_nginx_unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16793 2024-02-13 00:03:41.000000 certbot-nginx-unit-1.0.6/certbot_nginx_unit/configurator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 00:03:54.428121 certbot-nginx-unit-1.0.6/certbot_nginx_unit/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-13 00:03:41.000000 certbot-nginx-unit-1.0.6/certbot_nginx_unit/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-02-13 00:03:41.000000 certbot-nginx-unit-1.0.6/certbot_nginx_unit/tests/configurator_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-02-13 00:03:41.000000 certbot-nginx-unit-1.0.6/certbot_nginx_unit/unitc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 00:03:54.428121 certbot-nginx-unit-1.0.6/certbot_nginx_unit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-02-13 00:03:54.000000 certbot-nginx-unit-1.0.6/certbot_nginx_unit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-02-13 00:03:54.000000 certbot-nginx-unit-1.0.6/certbot_nginx_unit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 00:03:54.000000 certbot-nginx-unit-1.0.6/certbot_nginx_unit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-13 00:03:54.000000 certbot-nginx-unit-1.0.6/certbot_nginx_unit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-13 00:03:54.000000 certbot-nginx-unit-1.0.6/certbot_nginx_unit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-13 00:03:54.000000 certbot-nginx-unit-1.0.6/certbot_nginx_unit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-02-13 00:03:41.000000 certbot-nginx-unit-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-13 00:03:54.428121 certbot-nginx-unit-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-02-13 00:03:41.000000 certbot-nginx-unit-1.0.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-02-13 00:03:41.000000 certbot-nginx-unit-1.0.6/snapcraft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-02-13 00:03:41.000000 certbot-nginx-unit-1.0.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:58:37.468018 certbot_nginx_unit-1.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:58:37.464018 certbot_nginx_unit-1.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:58:37.468018 certbot_nginx_unit-1.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-13 15:58:33.000000 certbot_nginx_unit-1.0.7/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-13 15:58:33.000000 certbot_nginx_unit-1.0.7/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-13 15:58:33.000000 certbot_nginx_unit-1.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    21568 2024-04-13 15:58:33.000000 certbot_nginx_unit-1.0.7/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-13 15:58:33.000000 certbot_nginx_unit-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-13 15:58:37.468018 certbot_nginx_unit-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-13 15:58:33.000000 certbot_nginx_unit-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:58:37.468018 certbot_nginx_unit-1.0.7/certbot_nginx_unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-13 15:58:33.000000 certbot_nginx_unit-1.0.7/certbot_nginx_unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16926 2024-04-13 15:58:33.000000 certbot_nginx_unit-1.0.7/certbot_nginx_unit/configurator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:58:37.468018 certbot_nginx_unit-1.0.7/certbot_nginx_unit/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-13 15:58:33.000000 certbot_nginx_unit-1.0.7/certbot_nginx_unit/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-04-13 15:58:33.000000 certbot_nginx_unit-1.0.7/certbot_nginx_unit/tests/configurator_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-13 15:58:33.000000 certbot_nginx_unit-1.0.7/certbot_nginx_unit/unitc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:58:37.468018 certbot_nginx_unit-1.0.7/certbot_nginx_unit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-13 15:58:37.000000 certbot_nginx_unit-1.0.7/certbot_nginx_unit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-13 15:58:37.000000 certbot_nginx_unit-1.0.7/certbot_nginx_unit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:58:37.000000 certbot_nginx_unit-1.0.7/certbot_nginx_unit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-13 15:58:37.000000 certbot_nginx_unit-1.0.7/certbot_nginx_unit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 15:58:37.000000 certbot_nginx_unit-1.0.7/certbot_nginx_unit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-13 15:58:37.000000 certbot_nginx_unit-1.0.7/certbot_nginx_unit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-13 15:58:33.000000 certbot_nginx_unit-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 15:58:37.468018 certbot_nginx_unit-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-13 15:58:33.000000 certbot_nginx_unit-1.0.7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-13 15:58:33.000000 certbot_nginx_unit-1.0.7/snapcraft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-13 15:58:33.000000 certbot_nginx_unit-1.0.7/tox.ini
```

### Comparing `certbot-nginx-unit-1.0.6/.github/workflows/publish-to-pypi.yml` & `certbot_nginx_unit-1.0.7/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `certbot-nginx-unit-1.0.6/.pylintrc` & `certbot_nginx_unit-1.0.7/.pylintrc`

 * *Files identical despite different names*

### Comparing `certbot-nginx-unit-1.0.6/LICENSE` & `certbot_nginx_unit-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `certbot-nginx-unit-1.0.6/PKG-INFO` & `certbot_nginx_unit-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-nginx-unit
-Version: 1.0.6
+Version: 1.0.7
 Summary: Nginx Unit plugin for Certbot
 Author-email: Manuel Baldassarri <m.baldassarri@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Manuel Baldassarri
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -84,15 +84,15 @@
     ```
     python3 -m venv /some/path
     ```
 
     use the pip in the virtual environment to install or update
 
     ```
-    /some/path/bin/pip install -U certbot-nginx-unit
+    /some/path/bin/pip install -U certbot certbot-nginx-unit
     ```
 
     use the cerbot from the virtualenv, to avoid accidentally
     using one from a different environment that does not have this library
     ```
     /some/path/bin/certbot
     ```
```

### Comparing `certbot-nginx-unit-1.0.6/README.md` & `certbot_nginx_unit-1.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     ```
     python3 -m venv /some/path
     ```
 
     use the pip in the virtual environment to install or update
 
     ```
-    /some/path/bin/pip install -U certbot-nginx-unit
+    /some/path/bin/pip install -U certbot certbot-nginx-unit
     ```
 
     use the cerbot from the virtualenv, to avoid accidentally
     using one from a different environment that does not have this library
     ```
     /some/path/bin/certbot
     ```
```

### Comparing `certbot-nginx-unit-1.0.6/certbot_nginx_unit/configurator.py` & `certbot_nginx_unit-1.0.7/certbot_nginx_unit/configurator.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,14 +216,15 @@
         with open(fullchain_path, "rb") as f:
             certificates += f.read()
         return certificates
 
     def _get_unit_configuration(self, path: str):
         error_message = "nginx unit get configuration failed"
         configuration_str = self.unitc.get(path, "Get configuration", error_message)
+        logger.debug("Conf str '%s'", configuration_str)
 
         # @todo wrap configuration to a dedicated class
         return json.loads(configuration_str)
 
     def enhance(self, domain: str, enhancement: str, options: Optional[Union[List[str], str]] = None) -> None:
         pass
 
@@ -248,23 +249,24 @@
     def prepare(self) -> None:
         """Prepare the authenticator/installer."""
         # @todo verify "unitc" executable
         # @todo lock to prevent concurrent multi update
         if self._prepared:
             return
         self._configuration = self._get_unit_configuration("/config")
+        self._backup_routes = self._configuration.get("routes", [])
         self._prepared = True
 
     def more_info(self) -> str:  # pylint: disable=missing-function-docstring
         return self.MORE_INFO.format(self.conf("path"))
 
     ### Authenticator
     @classmethod
     def add_parser_arguments(cls, add: Callable[..., None]) -> None:
-        add("path", default=['/srv/www/unit/'],
+        add("path", default="/srv/www/unit/", type=str,
             help="public_html / webroot path. Only one catch 'em all temporary "
                  "directory --nginx-unit-path /srv/www/unit/ (default: /srv/www/unit/)")
 
     def get_chall_pref(self, domain: str) -> Iterable[Type[challenges.Challenge]]:
         # pylint: disable=unused-argument,missing-function-docstring
         return [challenges.HTTP01]
```

### Comparing `certbot-nginx-unit-1.0.6/certbot_nginx_unit/tests/configurator_test.py` & `certbot_nginx_unit-1.0.7/certbot_nginx_unit/tests/configurator_test.py`

 * *Files identical despite different names*

### Comparing `certbot-nginx-unit-1.0.6/certbot_nginx_unit/unitc.py` & `certbot_nginx_unit-1.0.7/certbot_nginx_unit/unitc.py`

 * *Files identical despite different names*

### Comparing `certbot-nginx-unit-1.0.6/certbot_nginx_unit.egg-info/PKG-INFO` & `certbot_nginx_unit-1.0.7/certbot_nginx_unit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-nginx-unit
-Version: 1.0.6
+Version: 1.0.7
 Summary: Nginx Unit plugin for Certbot
 Author-email: Manuel Baldassarri <m.baldassarri@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Manuel Baldassarri
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -84,15 +84,15 @@
     ```
     python3 -m venv /some/path
     ```
 
     use the pip in the virtual environment to install or update
 
     ```
-    /some/path/bin/pip install -U certbot-nginx-unit
+    /some/path/bin/pip install -U certbot certbot-nginx-unit
     ```
 
     use the cerbot from the virtualenv, to avoid accidentally
     using one from a different environment that does not have this library
     ```
     /some/path/bin/certbot
     ```
```

### Comparing `certbot-nginx-unit-1.0.6/certbot_nginx_unit.egg-info/SOURCES.txt` & `certbot_nginx_unit-1.0.7/certbot_nginx_unit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certbot-nginx-unit-1.0.6/pyproject.toml` & `certbot_nginx_unit-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `certbot-nginx-unit-1.0.6/snapcraft.yaml` & `certbot_nginx_unit-1.0.7/snapcraft.yaml`

 * *Files identical despite different names*

### Comparing `certbot-nginx-unit-1.0.6/tox.ini` & `certbot_nginx_unit-1.0.7/tox.ini`

 * *Files identical despite different names*

