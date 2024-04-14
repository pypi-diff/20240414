# Comparing `tmp/graphene_django_extended-1.0.0.tar.gz` & `tmp/graphene_django_extended-1.0.1.tar.gz`

## Comparing `graphene_django_extended-1.0.0.tar` & `graphene_django_extended-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,24 @@
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.0/.gitignore
--rw-r--r--   0        0        0    17098 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.0/LICENSE
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.0/README.md
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.1/graphene_django_extended/__init__.py
+-rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.1/graphene_django_extended/connection.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.1/graphene_django_extended/converter.py
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.1/graphene_django_extended/interface.py
+-rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.1/graphene_django_extended/mutation.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.1/graphene_django_extended/_mutations/Pipfile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.1/graphene_django_extended/_mutations/__init__.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.1/graphene_django_extended/_mutations/delete_mutation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.1/graphene_django_extended/_mutations/fields.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.1/graphene_django_extended/_mutations/global_id_serializer_mutation.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.1/graphene_django_extended/_mutations/inputs.py
+-rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.1/graphene_django_extended/_mutations/model_mutation.py
+-rw-r--r--   0        0        0     5667 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.1/graphene_django_extended/_mutations/mutations.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.1/graphene_django_extended/search/__init__.py
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.1/graphene_django_extended/search/connection.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.1/graphene_django_extended/search/field.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.1/graphene_django_extended/search/node.py
+-rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.1/graphene_django_extended/search/types.py
+-rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.1/graphene_django_extended/tests/test_interface.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.1/.gitignore
+-rw-r--r--   0        0        0    17098 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.1/LICENSE
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.1/README.md
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.1/PKG-INFO
```

### Comparing `graphene_django_extended-1.0.0/LICENSE` & `graphene_django_extended-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene_django_extended-1.0.0/README.md` & `graphene_django_extended-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,7 +8,8 @@
 - generate html instead of md ???
 - add general introduction and usage guide on the docs
 
 Build
 `hatch build` or `python -m hatch build`
 `hatch publish` or `python -m hatch publish` with username `__token__`. Make sure the [keyrings backend](https://github.com/jaraco/keyrings.alt) is installed. 
 On arch `pacman -S python-hatch python-keyrings-alt`, publish with `username:__token__`
+The default keyring is located at `~/.local/share/python_keyring/` and uses the name "main". Again this is not a recommended implementation, just a quick and dirty keyring usage
```

### Comparing `graphene_django_extended-1.0.0/pyproject.toml` & `graphene_django_extended-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "graphene-django-extended"
-version = "1.0.0"
+version = "1.0.1"
 #authors = [
 #  { name="Example Author", email="author@example.com" },
 #]
 description = "A collection of utility classes to extend the base functionality of graphene_django"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `graphene_django_extended-1.0.0/PKG-INFO` & `graphene_django_extended-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: graphene-django-extended
-Version: 1.0.0
+Version: 1.0.1
 Summary: A collection of utility classes to extend the base functionality of graphene_django
 Project-URL: Homepage, https://github.com/AztlanEngineering/graphene-django-extended
 Project-URL: Issues, https://github.com/AztlanEngineering/graphene-django-extended/issues
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -21,7 +21,8 @@
 - generate html instead of md ???
 - add general introduction and usage guide on the docs
 
 Build
 `hatch build` or `python -m hatch build`
 `hatch publish` or `python -m hatch publish` with username `__token__`. Make sure the [keyrings backend](https://github.com/jaraco/keyrings.alt) is installed. 
 On arch `pacman -S python-hatch python-keyrings-alt`, publish with `username:__token__`
+The default keyring is located at `~/.local/share/python_keyring/` and uses the name "main". Again this is not a recommended implementation, just a quick and dirty keyring usage
```

