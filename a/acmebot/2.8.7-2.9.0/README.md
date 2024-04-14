# Comparing `tmp/acmebot-2.8.7.tar.gz` & `tmp/acmebot-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acmebot-2.8.7.tar", last modified: Sun Aug 13 01:04:18 2023, max compression
+gzip compressed data, was "acmebot-2.9.0.tar", last modified: Sun Aug 13 22:13:11 2023, max compression
```

## Comparing `acmebot-2.8.7.tar` & `acmebot-2.9.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-13 01:04:18.886538 acmebot-2.8.7/
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-08-13 01:04:17.000000 acmebot-2.8.7/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-08-13 01:04:17.000000 acmebot-2.8.7/.gitlab-ci.env
--rw-rw-rw-   0 root         (0) root         (0)     2077 2023-08-13 01:04:17.000000 acmebot-2.8.7/.gitlab-ci.yaml
--rw-rw-rw-   0 root         (0) root         (0)    35141 2023-08-13 01:04:17.000000 acmebot-2.8.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)    84263 2023-08-13 01:04:18.886538 acmebot-2.8.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    83967 2023-08-13 01:04:17.000000 acmebot-2.8.7/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-13 01:04:18.882538 acmebot-2.8.7/config/
--rw-rw-rw-   0 root         (0) root         (0)    19324 2023-08-13 01:04:17.000000 acmebot-2.8.7/config/acmebot.example.json
--rw-rw-rw-   0 root         (0) root         (0)    13983 2023-08-13 01:04:17.000000 acmebot-2.8.7/config/acmebot.example.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-13 01:04:18.882538 acmebot-2.8.7/logrotate.d/
--rw-rw-rw-   0 root         (0) root         (0)      136 2023-08-13 01:04:17.000000 acmebot-2.8.7/logrotate.d/acmebot
--rw-rw-rw-   0 root         (0) root         (0)     1299 2023-08-13 01:04:17.000000 acmebot-2.8.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-13 01:04:18.886538 acmebot-2.8.7/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-13 01:04:18.878538 acmebot-2.8.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-13 01:04:18.882538 acmebot-2.8.7/src/acmebot/
--rw-rw-rw-   0 root         (0) root         (0)      586 2023-08-13 01:04:17.000000 acmebot-2.8.7/src/acmebot/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)   202565 2023-08-13 01:04:17.000000 acmebot-2.8.7/src/acmebot/acmebot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-13 01:04:18.886538 acmebot-2.8.7/src/acmebot.egg-info/
--rw-r--r--   0 root         (0) root         (0)    84263 2023-08-13 01:04:18.000000 acmebot-2.8.7/src/acmebot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      410 2023-08-13 01:04:18.000000 acmebot-2.8.7/src/acmebot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-13 01:04:18.000000 acmebot-2.8.7/src/acmebot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-08-13 01:04:18.000000 acmebot-2.8.7/src/acmebot.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      507 2023-08-13 01:04:18.000000 acmebot-2.8.7/src/acmebot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-08-13 01:04:18.000000 acmebot-2.8.7/src/acmebot.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-13 22:13:11.703695 acmebot-2.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-08-13 01:04:17.000000 acmebot-2.9.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-08-13 01:04:17.000000 acmebot-2.9.0/.gitlab-ci.env
+-rw-rw-rw-   0 root         (0) root         (0)     2077 2023-08-13 01:04:17.000000 acmebot-2.9.0/.gitlab-ci.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    35141 2023-08-13 01:04:17.000000 acmebot-2.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    84701 2023-08-13 22:13:11.703695 acmebot-2.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    84405 2023-08-13 22:13:10.000000 acmebot-2.9.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-13 22:13:11.699695 acmebot-2.9.0/config/
+-rw-rw-rw-   0 root         (0) root         (0)    19324 2023-08-13 01:04:17.000000 acmebot-2.9.0/config/acmebot.example.json
+-rw-rw-rw-   0 root         (0) root         (0)    13983 2023-08-13 01:04:17.000000 acmebot-2.9.0/config/acmebot.example.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-13 22:13:11.699695 acmebot-2.9.0/logrotate.d/
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-08-13 01:04:17.000000 acmebot-2.9.0/logrotate.d/acmebot
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2023-08-13 01:04:17.000000 acmebot-2.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-13 22:13:11.703695 acmebot-2.9.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-13 22:13:11.695695 acmebot-2.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-13 22:13:11.699695 acmebot-2.9.0/src/acmebot/
+-rw-rw-rw-   0 root         (0) root         (0)      586 2023-08-13 01:04:17.000000 acmebot-2.9.0/src/acmebot/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)   203132 2023-08-13 22:13:10.000000 acmebot-2.9.0/src/acmebot/acmebot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-13 22:13:11.703695 acmebot-2.9.0/src/acmebot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    84701 2023-08-13 22:13:11.000000 acmebot-2.9.0/src/acmebot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      410 2023-08-13 22:13:11.000000 acmebot-2.9.0/src/acmebot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-13 22:13:11.000000 acmebot-2.9.0/src/acmebot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-08-13 22:13:11.000000 acmebot-2.9.0/src/acmebot.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      507 2023-08-13 22:13:11.000000 acmebot-2.9.0/src/acmebot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-13 22:13:11.000000 acmebot-2.9.0/src/acmebot.egg-info/top_level.txt
```

### Comparing `acmebot-2.8.7/.gitlab-ci.yaml` & `acmebot-2.9.0/.gitlab-ci.yaml`

 * *Files identical despite different names*

### Comparing `acmebot-2.8.7/LICENSE` & `acmebot-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `acmebot-2.8.7/PKG-INFO` & `acmebot-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acmebot
-Version: 2.8.7
+Version: 2.9.0
 Summary: ACME protocol automatic certitificate manager
 Author-email: Peter Linss <peter@linss.com>
 Project-URL: homepage, https://acmebot.org
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
@@ -566,14 +566,20 @@
   You can run ``openssl ecparam -list_curves`` to find a list of available curves.
 * ``file_user`` specifies the name of the user that will own certificate and private key files.
   The default value is ``"root"``.
   Note that this tool must run as root, or another user that has rights to set the file ownership to this user.
 * ``file_group`` speficies the name of the group that will own certificate and private key files.
   The default value is ``"ssl-cert"``.
   Note that this tool must run as root, or another user that has rights to set the file ownership to this group.
+* ``log_user`` specifies the name of the user that will own log files.
+  The default value is ``"root"``.
+  Note that this tool must run as root, or another user that has rights to set the file ownership to this user.
+* ``log_group`` speficies the name of the group that will own log files.
+  The default value is ``"adm"``.
+  Note that this tool must run as root, or another user that has rights to set the file ownership to this group.
 * ``hpkp_days`` specifies the number of days that HPKP pins should be cached for.
   The default value is ``60``.
   HPKP pin files can be turned off by setting this value to ``0`` or ``null``.
 * ``pin_subdomains`` specifies whether the ``includeSubdomains`` directive should be included in the HPKP headers.
   The default value is ``true``.
 * ``hpkp_report_uri`` specifies the uri to report HPKP failures to.
   The default value is ``null``.
```

### Comparing `acmebot-2.8.7/README.rst` & `acmebot-2.9.0/src/acmebot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: acmebot
+Version: 2.9.0
+Summary: ACME protocol automatic certitificate manager
+Author-email: Peter Linss <peter@linss.com>
+Project-URL: homepage, https://acmebot.org
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
+License-File: LICENSE
+
 .. _bindtool: https://github.com/plinss/bindtool
 
 *******
 acmebot
 *******
 
 ACME protocol automatic certitificate manager.
@@ -555,14 +566,20 @@
   You can run ``openssl ecparam -list_curves`` to find a list of available curves.
 * ``file_user`` specifies the name of the user that will own certificate and private key files.
   The default value is ``"root"``.
   Note that this tool must run as root, or another user that has rights to set the file ownership to this user.
 * ``file_group`` speficies the name of the group that will own certificate and private key files.
   The default value is ``"ssl-cert"``.
   Note that this tool must run as root, or another user that has rights to set the file ownership to this group.
+* ``log_user`` specifies the name of the user that will own log files.
+  The default value is ``"root"``.
+  Note that this tool must run as root, or another user that has rights to set the file ownership to this user.
+* ``log_group`` speficies the name of the group that will own log files.
+  The default value is ``"adm"``.
+  Note that this tool must run as root, or another user that has rights to set the file ownership to this group.
 * ``hpkp_days`` specifies the number of days that HPKP pins should be cached for.
   The default value is ``60``.
   HPKP pin files can be turned off by setting this value to ``0`` or ``null``.
 * ``pin_subdomains`` specifies whether the ``includeSubdomains`` directive should be included in the HPKP headers.
   The default value is ``true``.
 * ``hpkp_report_uri`` specifies the uri to report HPKP failures to.
   The default value is ``null``.
```

### Comparing `acmebot-2.8.7/config/acmebot.example.json` & `acmebot-2.9.0/config/acmebot.example.json`

 * *Files identical despite different names*

### Comparing `acmebot-2.8.7/config/acmebot.example.yaml` & `acmebot-2.9.0/config/acmebot.example.yaml`

 * *Files identical despite different names*

### Comparing `acmebot-2.8.7/pyproject.toml` & `acmebot-2.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `acmebot-2.8.7/src/acmebot/__init__.py` & `acmebot-2.9.0/src/acmebot/__init__.py`

 * *Files identical despite different names*

### Comparing `acmebot-2.8.7/src/acmebot/acmebot.py` & `acmebot-2.9.0/src/acmebot/acmebot.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,14 +259,16 @@
                 'key_cipher': 'blowfish',
                 'key_passphrase': None,
                 'key_provided': False,
                 'dhparam_size': 2048,
                 'ecparam_curve': ['secp521r1', 'secp384r1', 'secp256k1'],
                 'file_user': 'root',
                 'file_group': 'ssl-cert',
+                'log_user': 'root',
+                'log_group': 'adm',
                 'hpkp_days': 60,
                 'pin_subdomains': True,
                 'hpkp_report_uri': None,
                 'ocsp_must_staple': False,
                 'ocsp_responder_urls': ['http://ocsp.int-x3.letsencrypt.org'],
                 'ct_submit_logs': ['google_argon', 'google_xenon'],
                 'renewal_days': 30,
@@ -682,20 +684,21 @@
         self._log(message)
         raise AcmeError(message)
 
     def _log(self, *args):
         if (hasattr(self, 'config') and self._directory('log') and self._file_name('log') and self._setting('log_level')):
             log_file_path = self._file_path('log', self.script_name)
             try:
-                with self._open_file(log_file_path, mode='a+', chmod=0o640, warn=False) as log_file:
+                with self._open_file(log_file_path, mode='a+', chmod=0o640, warn=False,
+                                     user=self._setting('log_user'), group=self._setting('log_group')) as log_file:
                     log_file.write(self._message(*args))
             except Exception:
                 sys.stderr.write('Unable to write to log file ' + log_file_path + '\n')
 
-    def _makedir(self, dir_path, chmod=None, warn=True):
+    def _makedir(self, dir_path, *, chmod=None, warn=True, user=None, group=None):
         if (not os.path.isdir(dir_path)):
             try:
                 os.makedirs(dir_path)
                 if (chmod):
                     if (chmod & 0o700):
                         chmod |= 0o100
                     if (chmod & 0o070):
@@ -704,38 +707,41 @@
                         chmod |= 0o001
                     try:
                         os.chmod(dir_path, chmod)
                     except PermissionError as error:
                         if (warn):
                             self._error('Unable to set directory mode for ', dir_path, '\n', self._indent(error), '\n', code=ErrorCode.PERMISSION)
                     try:
-                        os.chown(dir_path, self._get_user_id(self._setting('file_user')), self._get_group_id(self._setting('file_group')))
+                        os.chown(dir_path, self._get_user_id(user or self._setting('file_user')), self._get_group_id(group or self._setting('file_group')))
                     except PermissionError as error:
                         if (warn):
                             self._error('Unable to set directory ownership for ', dir_path, ' to ',
                                         self._setting('file_user'), ':', self._setting('file_group'), '\n', self._indent(error), '\n',
                                         code=ErrorCode.PERMISSION)
             except Exception as error:
                 if (warn):
                     self._error('Unable to create directory ', dir_path, '\n', self._indent(error), '\n', code=ErrorCode.PERMISSION)
 
-    def _open_file(self, file_path, mode='r', chmod=0o666, warn=True):
+    def _open_file(self, file_path, *, mode='r', chmod=0o666, warn=True, user=None, group=None):
         def opener(file_path, flags):
-            return os.open(file_path, flags, mode=chmod)
+            file = os.open(file_path, flags, mode=chmod)
+            if (user or group):
+                os.chown(file_path, self._get_user_id(user or self._setting('file_user')), self._get_group_id(group or self._setting('file_group')))
+            return file
         if ((('w' in mode) or ('a' in mode)) and isinstance(file_path, str)):
-            self._makedir(os.path.dirname(file_path), chmod=chmod, warn=warn)
+            self._makedir(os.path.dirname(file_path), chmod=chmod, warn=warn, user=user, group=group)
         return open(file_path, mode, opener=opener)
 
     def _archive_file(self, file_type, file_path, archive_name='', archive_date=datetime.datetime.now()):
         if (os.path.isfile(file_path) and (not os.path.islink(file_path)) and (archive_name is not None)):
             archive_file_path = os.path.join(self._directory('archive'),
                                              archive_name,
                                              archive_date.strftime('%Y_%m_%d_%H%M%S') if (archive_date) else '',
                                              file_type + '.' + os.path.basename(file_path))
-            self._makedir(os.path.dirname(archive_file_path), 0o640)
+            self._makedir(os.path.dirname(archive_file_path), chmod=0o640)
             shutil.move(file_path, archive_file_path)
             self._detail('Archived ', file_path, ' as ', archive_file_path, '\n')
             return (file_path, archive_file_path)
         return (None, None)
 
     def _get_user_id(self, user_name):
         try:
@@ -745,30 +751,30 @@
 
     def _get_group_id(self, group_name):
         try:
             return grp.getgrnam(group_name).gr_gid
         except Exception:
             return -1
 
-    def _rename_file(self, old_file_path, new_file_path, chmod=None, timestamp=None):
+    def _rename_file(self, old_file_path, new_file_path, *, chmod=None, timestamp=None, user=None, group=None):
         if (os.path.isfile(old_file_path)):
-            self._makedir(os.path.dirname(new_file_path), chmod)
+            self._makedir(os.path.dirname(new_file_path), chmod=chmod)
             shutil.move(old_file_path, new_file_path)
             if (chmod):
                 try:
                     os.chmod(new_file_path, chmod)
                 except PermissionError as error:
                     self._error('Unable to set file mode for ', new_file_path, '\n', self._indent(error), '\n', code=ErrorCode.PERMISSION)
             if (timestamp):
                 try:
                     os.utime(new_file_path, (timestamp, timestamp))
                 except PermissionError as error:
                     self._error('Unable to set file time for ', new_file_path, '\n', self._indent(error), '\n', code=ErrorCode.PERMISSION)
             try:
-                os.chown(new_file_path, self._get_user_id(self._setting('file_user')), self._get_group_id(self._setting('file_group')))
+                os.chown(new_file_path, self._get_user_id(user or self._setting('file_user')), self._get_group_id(group or self._setting('file_group')))
             except PermissionError as error:
                 self._error('Unable to set file ownership for ', new_file_path, ' to ',
                             self._setting('file_user'), ':', self._setting('file_group'), '\n', self._indent(error), '\n', code=ErrorCode.PERMISSION)
             return new_file_path
         return None
 
     def _commit_file_transactions(self, file_transactions, archive_name=''):
@@ -1829,15 +1835,15 @@
                 client_key_file.write(client_key_pem.decode('ascii'))
                 self._status('Client key exported to ', client_key_file_path, '\n')
         except Exception as error:
             self._fatal('Unbale to write client key to ', client_key_file_path, '\n', error, '\n', code=ErrorCode.PERMISSION)
 
     def connect_client(self):
         resource_dir = os.path.join(self.script_dir, self._directory('resource'))
-        self._makedir(resource_dir, 0o600)
+        self._makedir(resource_dir, chmod=0o600)
         generated_client_key = False
         client_key_path = os.path.join(resource_dir, 'client_key.json')
         if (os.path.isfile(client_key_path)):
             with open(client_key_path) as client_key_file:
                 self.client_key = josepy.JWKRSA.fields_from_json(json.load(client_key_file))
                 self._detail('Loaded clent key ', client_key_path, '\n')
         else:
@@ -1911,15 +1917,15 @@
         if (self.acme_client):
             del self.acme_client
 
     def _load_public_suffix_list(self):
         if (hasattr(self, '_public_suffixes')):
             return
         resource_dir = os.path.join(self.script_dir, self._directory('resource'))
-        self._makedir(resource_dir, 0o600)
+        self._makedir(resource_dir, chmod=0o600)
         public_suffix_list_path = os.path.join(resource_dir, 'public_suffix_list.dat')
         fetch = True
         last_update = None
         if (os.path.isfile(public_suffix_list_path)):
             last_update = datetime.datetime.utcfromtimestamp(os.path.getmtime(public_suffix_list_path))
             if ((datetime.datetime.utcnow() - last_update).days < 1):
                 fetch = False
@@ -2039,15 +2045,15 @@
                         challenge = self._get_challenge(authorization_resource, challenge_types[domain_name])
                         if (not challenge):
                             self._error('Unable to use http-01 challenge for ', domain_name, '\n', code=ErrorCode.ACME)
                             continue
                         challenge_file_path = os.path.join(http_challenge_directory, challenge.chall.encode('token'))
                         self._debug('Setting http acme-challenge for ', domain_name, ' in file ', challenge_file_path, '\n')
                         try:
-                            with self._open_file(challenge_file_path, 'w', 0o644) as challenge_file:
+                            with self._open_file(challenge_file_path, mode='w', chmod=0o644) as challenge_file:
                                 challenge_file.write(challenge.validation(self.client_key))
                             challenge_http_responses[domain_name] = challenge_file_path
                             self._add_hook('set_http_challenge', domain=domain_name, challenge_file=challenge_http_responses[domain_name])
                         except Exception as error:
                             self._error('Unable to create acme-challenge file ', challenge_file_path, '\n', self._indent(error), '\n',
                                         code=ErrorCode.PERMISSION)
                     else:
@@ -2063,15 +2069,15 @@
             if (zone_responses):
                 zone_key = self._zone_key(zone_name)
                 if (zone_key):
                     if (self._set_dns_challenges(zone_name, zone_key, zone_responses)):
                         challenge_dns_responses[zone_name] = zone_responses
                 else:
                     try:
-                        with self._open_file(self._file_path('challenge', zone_name), 'w', 0o644) as challenge_file:
+                        with self._open_file(self._file_path('challenge', zone_name), mode='w', chmod=0o644) as challenge_file:
                             json.dump({domain_name: response.response for domain_name, response in zone_responses.items()}, challenge_file)
                         challenge_dns_responses[zone_name] = zone_responses
                     except Exception as error:
                         self._error('Unable to create acme-challenge file for zone ', zone_name, '\n', self._indent(error), '\n', code=ErrorCode.PERMISSION)
                     if (zone_name in challenge_dns_responses):
                         self._reload_zone(zone_name)
                 self._add_hook('dns_zone_update', zone=zone_name)
@@ -3404,15 +3410,15 @@
             if (self._process_running(pid_file_path)):
                 self._detail('Waiting for other running client instance\n')
                 while (self._process_running(pid_file_path)):
                     time.sleep(random.randrange(5, 30))
         else:
             if (self._process_running(pid_file_path)):
                 self._fatal('Client already running\n')
-        with self._open_file(pid_file_path, 'w') as pid_file:
+        with self._open_file(pid_file_path, mode='w') as pid_file:
             pid_file.write(str(os.getpid()))
         try:
             if (not (self.args.revoke or self.args.auth or self.args.certs or self.args.tlsa or self.args.sct or self.args.ocsp or self.args.verify
                      or self.args.register or self.args.export_client or self.args.show_config)):
                 self.args.auth = True
                 self.args.certs = True
                 self.args.tlsa = True
```

### Comparing `acmebot-2.8.7/src/acmebot.egg-info/PKG-INFO` & `acmebot-2.9.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: acmebot
-Version: 2.8.7
-Summary: ACME protocol automatic certitificate manager
-Author-email: Peter Linss <peter@linss.com>
-Project-URL: homepage, https://acmebot.org
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-License-File: LICENSE
-
 .. _bindtool: https://github.com/plinss/bindtool
 
 *******
 acmebot
 *******
 
 ACME protocol automatic certitificate manager.
@@ -566,14 +555,20 @@
   You can run ``openssl ecparam -list_curves`` to find a list of available curves.
 * ``file_user`` specifies the name of the user that will own certificate and private key files.
   The default value is ``"root"``.
   Note that this tool must run as root, or another user that has rights to set the file ownership to this user.
 * ``file_group`` speficies the name of the group that will own certificate and private key files.
   The default value is ``"ssl-cert"``.
   Note that this tool must run as root, or another user that has rights to set the file ownership to this group.
+* ``log_user`` specifies the name of the user that will own log files.
+  The default value is ``"root"``.
+  Note that this tool must run as root, or another user that has rights to set the file ownership to this user.
+* ``log_group`` speficies the name of the group that will own log files.
+  The default value is ``"adm"``.
+  Note that this tool must run as root, or another user that has rights to set the file ownership to this group.
 * ``hpkp_days`` specifies the number of days that HPKP pins should be cached for.
   The default value is ``60``.
   HPKP pin files can be turned off by setting this value to ``0`` or ``null``.
 * ``pin_subdomains`` specifies whether the ``includeSubdomains`` directive should be included in the HPKP headers.
   The default value is ``true``.
 * ``hpkp_report_uri`` specifies the uri to report HPKP failures to.
   The default value is ``null``.
```

