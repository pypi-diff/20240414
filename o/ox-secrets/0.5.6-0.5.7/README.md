# Comparing `tmp/ox_secrets-0.5.6.tar.gz` & `tmp/ox_secrets-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ox_secrets-0.5.6.tar", last modified: Fri Mar 29 02:30:39 2024, max compression
+gzip compressed data, was "ox_secrets-0.5.7.tar", last modified: Sun Apr 14 17:30:04 2024, max compression
```

## Comparing `ox_secrets-0.5.6.tar` & `ox_secrets-0.5.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 emin      (1000) emin      (1000)        0 2024-03-29 02:30:39.322566 ox_secrets-0.5.6/
--rw-r--r--   0 emin      (1000) emin      (1000)     1325 2020-12-16 18:45:56.000000 ox_secrets-0.5.6/LICENSE.txt
--rw-r--r--   0 emin      (1000) emin      (1000)     7884 2024-03-29 02:30:39.322566 ox_secrets-0.5.6/PKG-INFO
--rw-r--r--   0 emin      (1000) emin      (1000)     6076 2024-03-29 02:24:51.000000 ox_secrets-0.5.6/README.rst
-drwxr-xr-x   0 emin      (1000) emin      (1000)        0 2024-03-29 02:30:39.322566 ox_secrets-0.5.6/ox_secrets/
--rw-r--r--   0 emin      (1000) emin      (1000)     3535 2024-03-29 02:24:30.000000 ox_secrets-0.5.6/ox_secrets/__init__.py
-drwxr-xr-x   0 emin      (1000) emin      (1000)        0 2024-03-29 02:30:39.322566 ox_secrets-0.5.6/ox_secrets/core/
--rw-r--r--   0 emin      (1000) emin      (1000)       42 2020-12-16 18:45:56.000000 ox_secrets-0.5.6/ox_secrets/core/__init__.py
--rw-r--r--   0 emin      (1000) emin      (1000)     5011 2024-03-29 01:48:47.000000 ox_secrets-0.5.6/ox_secrets/core/aws.py
--rw-r--r--   0 emin      (1000) emin      (1000)    14131 2024-03-29 02:16:00.000000 ox_secrets-0.5.6/ox_secrets/core/common.py
--rw-r--r--   0 emin      (1000) emin      (1000)     4373 2022-09-07 16:33:57.000000 ox_secrets-0.5.6/ox_secrets/core/evs.py
--rw-r--r--   0 emin      (1000) emin      (1000)     5658 2023-10-07 23:33:55.000000 ox_secrets-0.5.6/ox_secrets/core/fss.py
--rw-r--r--   0 emin      (1000) emin      (1000)     4457 2023-10-07 23:33:55.000000 ox_secrets-0.5.6/ox_secrets/server.py
--rw-r--r--   0 emin      (1000) emin      (1000)     1109 2022-08-15 16:56:47.000000 ox_secrets-0.5.6/ox_secrets/settings.py
-drwxr-xr-x   0 emin      (1000) emin      (1000)        0 2024-03-29 02:30:39.322566 ox_secrets-0.5.6/ox_secrets/ui/
--rw-r--r--   0 emin      (1000) emin      (1000)       48 2023-10-07 23:33:55.000000 ox_secrets-0.5.6/ox_secrets/ui/__init__.py
--rw-r--r--   0 emin      (1000) emin      (1000)     2101 2023-10-15 02:10:10.000000 ox_secrets-0.5.6/ox_secrets/ui/cli.py
-drwxr-xr-x   0 emin      (1000) emin      (1000)        0 2024-03-29 02:30:39.322566 ox_secrets-0.5.6/ox_secrets.egg-info/
--rw-r--r--   0 emin      (1000) emin      (1000)     7884 2024-03-29 02:30:39.000000 ox_secrets-0.5.6/ox_secrets.egg-info/PKG-INFO
--rw-r--r--   0 emin      (1000) emin      (1000)      474 2024-03-29 02:30:39.000000 ox_secrets-0.5.6/ox_secrets.egg-info/SOURCES.txt
--rw-r--r--   0 emin      (1000) emin      (1000)        1 2024-03-29 02:30:39.000000 ox_secrets-0.5.6/ox_secrets.egg-info/dependency_links.txt
--rw-r--r--   0 emin      (1000) emin      (1000)       55 2024-03-29 02:30:39.000000 ox_secrets-0.5.6/ox_secrets.egg-info/entry_points.txt
--rw-r--r--   0 emin      (1000) emin      (1000)        7 2024-03-29 02:30:39.000000 ox_secrets-0.5.6/ox_secrets.egg-info/requires.txt
--rw-r--r--   0 emin      (1000) emin      (1000)       11 2024-03-29 02:30:39.000000 ox_secrets-0.5.6/ox_secrets.egg-info/top_level.txt
--rw-r--r--   0 emin      (1000) emin      (1000)       38 2024-03-29 02:30:39.322566 ox_secrets-0.5.6/setup.cfg
--rw-r--r--   0 emin      (1000) emin      (1000)     1974 2023-10-07 23:33:55.000000 ox_secrets-0.5.6/setup.py
+drwxr-xr-x   0 emin      (1000) emin      (1000)        0 2024-04-14 17:30:04.453441 ox_secrets-0.5.7/
+-rw-r--r--   0 emin      (1000) emin      (1000)     1325 2020-12-16 18:45:56.000000 ox_secrets-0.5.7/LICENSE.txt
+-rw-r--r--   0 emin      (1000) emin      (1000)     7884 2024-04-14 17:30:04.443441 ox_secrets-0.5.7/PKG-INFO
+-rw-r--r--   0 emin      (1000) emin      (1000)     6076 2024-04-14 17:17:08.000000 ox_secrets-0.5.7/README.rst
+drwxr-xr-x   0 emin      (1000) emin      (1000)        0 2024-04-14 17:30:04.443441 ox_secrets-0.5.7/ox_secrets/
+-rw-r--r--   0 emin      (1000) emin      (1000)     3535 2024-04-14 17:24:24.000000 ox_secrets-0.5.7/ox_secrets/__init__.py
+drwxr-xr-x   0 emin      (1000) emin      (1000)        0 2024-04-14 17:30:04.443441 ox_secrets-0.5.7/ox_secrets/core/
+-rw-r--r--   0 emin      (1000) emin      (1000)       42 2020-12-16 18:45:56.000000 ox_secrets-0.5.7/ox_secrets/core/__init__.py
+-rw-r--r--   0 emin      (1000) emin      (1000)     5011 2024-03-29 01:48:47.000000 ox_secrets-0.5.7/ox_secrets/core/aws.py
+-rw-r--r--   0 emin      (1000) emin      (1000)    16245 2024-04-14 17:29:29.000000 ox_secrets-0.5.7/ox_secrets/core/common.py
+-rw-r--r--   0 emin      (1000) emin      (1000)     4373 2022-09-07 16:33:57.000000 ox_secrets-0.5.7/ox_secrets/core/evs.py
+-rw-r--r--   0 emin      (1000) emin      (1000)     5658 2023-10-07 23:33:55.000000 ox_secrets-0.5.7/ox_secrets/core/fss.py
+-rw-r--r--   0 emin      (1000) emin      (1000)     4457 2023-10-07 23:33:55.000000 ox_secrets-0.5.7/ox_secrets/server.py
+-rw-r--r--   0 emin      (1000) emin      (1000)     1109 2022-08-15 16:56:47.000000 ox_secrets-0.5.7/ox_secrets/settings.py
+drwxr-xr-x   0 emin      (1000) emin      (1000)        0 2024-04-14 17:30:04.443441 ox_secrets-0.5.7/ox_secrets/ui/
+-rw-r--r--   0 emin      (1000) emin      (1000)       48 2023-10-07 23:33:55.000000 ox_secrets-0.5.7/ox_secrets/ui/__init__.py
+-rw-r--r--   0 emin      (1000) emin      (1000)     2101 2023-10-15 02:10:10.000000 ox_secrets-0.5.7/ox_secrets/ui/cli.py
+drwxr-xr-x   0 emin      (1000) emin      (1000)        0 2024-04-14 17:30:04.443441 ox_secrets-0.5.7/ox_secrets.egg-info/
+-rw-r--r--   0 emin      (1000) emin      (1000)     7884 2024-04-14 17:30:04.000000 ox_secrets-0.5.7/ox_secrets.egg-info/PKG-INFO
+-rw-r--r--   0 emin      (1000) emin      (1000)      474 2024-04-14 17:30:04.000000 ox_secrets-0.5.7/ox_secrets.egg-info/SOURCES.txt
+-rw-r--r--   0 emin      (1000) emin      (1000)        1 2024-04-14 17:30:04.000000 ox_secrets-0.5.7/ox_secrets.egg-info/dependency_links.txt
+-rw-r--r--   0 emin      (1000) emin      (1000)       55 2024-04-14 17:30:04.000000 ox_secrets-0.5.7/ox_secrets.egg-info/entry_points.txt
+-rw-r--r--   0 emin      (1000) emin      (1000)        7 2024-04-14 17:30:04.000000 ox_secrets-0.5.7/ox_secrets.egg-info/requires.txt
+-rw-r--r--   0 emin      (1000) emin      (1000)       11 2024-04-14 17:30:04.000000 ox_secrets-0.5.7/ox_secrets.egg-info/top_level.txt
+-rw-r--r--   0 emin      (1000) emin      (1000)       38 2024-04-14 17:30:04.453441 ox_secrets-0.5.7/setup.cfg
+-rw-r--r--   0 emin      (1000) emin      (1000)     1974 2023-10-07 23:33:55.000000 ox_secrets-0.5.7/setup.py
```

### Comparing `ox_secrets-0.5.6/LICENSE.txt` & `ox_secrets-0.5.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.6/PKG-INFO` & `ox_secrets-0.5.7/ox_secrets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: ox_secrets
-Version: 0.5.6
+Name: ox-secrets
+Version: 0.5.7
 Summary: Simple secret server for python
 Home-page: http://github.com/emin63/ox_secrets
 Author: Emin Martinian
 Author-email: emin.martinian@gmail.com
 License: custom
 Description: Introduction
         ============
```

### Comparing `ox_secrets-0.5.6/README.rst` & `ox_secrets-0.5.7/README.rst`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.6/ox_secrets/__init__.py` & `ox_secrets-0.5.7/ox_secrets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,9 +97,9 @@
     oss.get_server(mode='aws').store_secrets(
         {'test_storage':'foobar', category=AWS_PARAM_NAME,
         service_name='ssm')
 
 
 """
 
-VERSION = '0.5.6'
+VERSION = '0.5.7'
 __version__ = VERSION
```

### Comparing `ox_secrets-0.5.6/ox_secrets/core/aws.py` & `ox_secrets-0.5.7/ox_secrets/core/aws.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.6/ox_secrets/core/common.py` & `ox_secrets-0.5.7/ox_secrets/core/common.py`

 * *Files 9% similar despite different names*

```diff
@@ -176,30 +176,74 @@
         with cls._lock:
             return dict(cls._cache[category])  # return shallow copy
 
     @classmethod
     def setup_env_from_secrets(cls, category, *args,
                                param_names=None,
                                log_env_var='{category}__RESULTS',
-                               **kwargs):
+                               resetup: str = 'duplicate', **kwargs):
+        """Setup environment variables from secrets.
+
+        :param category:    String category to use to lookup secret dict.
+
+        :param *args:   As for `get_secret_dict`.
+
+        :param param_names=None:   Optional list of strings indicating
+                                   parameter names to set. If None, then
+                                   we set everything in the secret dict.
+
+        :param log_env_var='{category}__RESULTS':   Name of environment
+                                                    variable to set with
+                                                    log info.
+
+        :param resetup:  What to do if we are redoing the setup. If 'strict',
+                         then calling this method twice is not allowed. If
+                         'duplicate', then allow calling multiple times provided
+                         we are just setting up the same values again (but no
+                         changing values allowed). If 'overwrite', then allow
+                         overwriting old values.
+
+        :param **kwargs:    Passed to `get_secret_dict`.
+
+        ~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-
+
+        PURPOSE:  Call `get_secret_dict` and then set `param_names` as
+                  environment variables.
+
+        """
+        assert resetup in {'duplicate', 'strict', 'ovewrite'}, (
+            'Invalid value {resetup} for "resetup"')
         log_env_var = log_env_var.format(category=category)
         if os.environ.get(log_env_var, None) is not None:
-            raise ValueError(f'Refusing to setup category {category}' +
-                             f' already setup as {log_env_var}=' +
-                             os.environ[log_env_var])
+            if resetup == 'strict':
+                raise ValueError(
+                    'Since resetup=strict, refusing to setup' +
+                    f' category {category} already setup as {log_env_var}=' +
+                    os.environ[log_env_var])
+            logging.warning('Doing resetup of category %s via %s=%s',
+                            category, log_env_var, os.environ[log_env_var])
         info = cls.get_secret_dict(category, *args, **kwargs)
         param_names = param_names if param_names is not None else list(info)
-        action_list = []        
+        action_list = []
         for name in param_names:
-            old = os.environ.get(name, None)
-            if old == info[name]:
-                logging.info('%s set; no reset from %s', name, category)
+            if info.get(name, None) is None:
+                logging.warning('No value provide for %s; skipping', name)
                 continue
-            elif old is not None:
-                logging.warning('Overwriting %s via %s', name, category)
+            old = os.environ.get(name, None)
+            if old is not None:
+                if old == str(info[name]):
+                    logging.info('%s set; no reset from %s since unchanged',
+                                 name, category)
+                    continue
+                if resetup == 'overwrite':
+                    logging.warning('Overwriting %s to new value via %s',
+                                    name, category)
+                else:
+                    raise ValueError(f'Refuse overwrite {name} from {category}'
+                                     f' since resetup={resetup}')
             os.environ[name] = str(info[name])
             logging.info('Set %s via %s', name, category)
             action_list.append(f'SET_{name}')
         os.environ[log_env_var] = (f'SET_{category}__AT__' + (
             datetime.datetime.utcnow().strftime('%Y-%m-%dT%H-%M-%S')) +
                                    '__' + '_'.join(action_list))
         logging.info('Set env var %s to log setup', log_env_var)
```

### Comparing `ox_secrets-0.5.6/ox_secrets/core/evs.py` & `ox_secrets-0.5.7/ox_secrets/core/evs.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.6/ox_secrets/core/fss.py` & `ox_secrets-0.5.7/ox_secrets/core/fss.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.6/ox_secrets/server.py` & `ox_secrets-0.5.7/ox_secrets/server.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.6/ox_secrets/settings.py` & `ox_secrets-0.5.7/ox_secrets/settings.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.6/ox_secrets/ui/cli.py` & `ox_secrets-0.5.7/ox_secrets/ui/cli.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.6/ox_secrets.egg-info/PKG-INFO` & `ox_secrets-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: ox-secrets
-Version: 0.5.6
+Name: ox_secrets
+Version: 0.5.7
 Summary: Simple secret server for python
 Home-page: http://github.com/emin63/ox_secrets
 Author: Emin Martinian
 Author-email: emin.martinian@gmail.com
 License: custom
 Description: Introduction
         ============
```

### Comparing `ox_secrets-0.5.6/setup.py` & `ox_secrets-0.5.7/setup.py`

 * *Files identical despite different names*

