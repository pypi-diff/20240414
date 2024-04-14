# Comparing `tmp/vtjson-1.7.2.tar.gz` & `tmp/vtjson-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtjson-1.7.2.tar", last modified: Sat Apr 13 01:37:25 2024, max compression
+gzip compressed data, was "vtjson-1.7.3.tar", last modified: Sun Apr 14 21:44:32 2024, max compression
```

## Comparing `vtjson-1.7.2.tar` & `vtjson-1.7.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:37:25.144340 vtjson-1.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-13 01:37:20.000000 vtjson-1.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18640 2024-04-13 01:37:25.144340 vtjson-1.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18019 2024-04-13 01:37:20.000000 vtjson-1.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-13 01:37:20.000000 vtjson-1.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 01:37:25.144340 vtjson-1.7.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:37:25.144340 vtjson-1.7.2/vtjson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18640 2024-04-13 01:37:25.000000 vtjson-1.7.2/vtjson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-13 01:37:25.000000 vtjson-1.7.2/vtjson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 01:37:25.000000 vtjson-1.7.2/vtjson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-13 01:37:25.000000 vtjson-1.7.2/vtjson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-13 01:37:25.000000 vtjson-1.7.2/vtjson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    28578 2024-04-13 01:37:20.000000 vtjson-1.7.2/vtjson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:44:32.766792 vtjson-1.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-14 21:44:27.000000 vtjson-1.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19228 2024-04-14 21:44:32.766792 vtjson-1.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18607 2024-04-14 21:44:27.000000 vtjson-1.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-14 21:44:27.000000 vtjson-1.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 21:44:32.766792 vtjson-1.7.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:44:32.766792 vtjson-1.7.3/vtjson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19228 2024-04-14 21:44:32.000000 vtjson-1.7.3/vtjson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-14 21:44:32.000000 vtjson-1.7.3/vtjson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 21:44:32.000000 vtjson-1.7.3/vtjson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-14 21:44:32.000000 vtjson-1.7.3/vtjson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-14 21:44:32.000000 vtjson-1.7.3/vtjson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    28578 2024-04-14 21:44:27.000000 vtjson-1.7.3/vtjson.py
```

### Comparing `vtjson-1.7.2/LICENSE` & `vtjson-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vtjson-1.7.2/PKG-INFO` & `vtjson-1.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtjson
-Version: 1.7.2
+Version: 1.7.3
 Summary: A lightweight package for validating JSON like Python objects
 Author-email: Michel Van den Bergh <michel.vandenbergh@uhasselt.be>
 Project-URL: Homepage, https://github.com/vdbergh/vtjson
 Project-URL: Bug Tracker, https://github.com/vdbergh/vtjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -249,15 +249,21 @@
 - `size(lowerbound, upperbound)`. Matches the objects (which support `len()` such as strings or lists) whose length is in the interval `[upperbound, lowerbound]`. The value of `upperbound` can be `...` (ellipsis).
 ## Conditional schemas
 - `ifthen(if_schema, then_schema, else_schema=None)`. It the object matches the `if_schema` then it should also match the `then_schema`. If the object does not match the `if_schema` then it should match
 the `else_schema`, if present.
 - `cond((if_schema1, then_schema1), ... , (if_schemaN, then_schemaN))`. An object is successively validated against `if_schema1`, `if_schema2`, ... until a validation succeeds. When this happens the object should
 match the corresponding `then_schema`. If no `if_schema` succeeds then the object is considered to have been validated. If one sets `if_schemaN` equal to `anything` then this serves as a catch all.
 ## Pre-compiling a schema
-- An object matches the schema `compile(schema)` if it matches `schema`. `vtjson` compiles the schema before performing a validation so pre-compiling is not necessary but, in some cases, it may gain a bit of performance. 
+An object matches the schema `compile(schema)` if it matches `schema`. `vtjson` compiles a schema before performing a validation against it, so pre-compiling is not necessary but it gains a bit of performance as it needs to be done only once. Compiling is an idempotent operation. It does nothing for an already compiled schema.
+
+The full signature of `compile()` is
+```python
+compile(schema, _deferred_compiles=None)
+```
+but the optional argument `_deferred_compiles` should not be set by the user.
 ## Format
 A schema can be, in order of precedence:
 - A class with the following properties:
   - it has a no-argument constructor;
   - the instances have a `__validate__` method with signature
   ```python
   __validate__(self, object, name, strict)
@@ -268,15 +274,15 @@
   __validate__(object, name, strict)
   ```
   as above.
 - An object having a `__compile__` attribute with signature
   ```python
   __compile__(_deferred_compiles=None)
   ```
-  This is an advanced feature which is used for the implementation of wrapper schemas. Please consult the source code of `vtjson` for more details.
+  This is an advanced feature which is used for the implementation of wrapper schemas. `__compile__()`, which is invoked by `compile()`, should produce an object with a `__validate__` attribute as described above. The optional argument `_deferred_compiles` is an opaque data structure for handling recursive schemas. It should be passed unmodified to any internal invokations of `compile()`. Please consult the source code of `vtjson` for more details.
 - A Python type. In that case validation is done by checking membership.
 - A callable. Validation is done by applying the callable to the object. If applying the callable throws an exception then the corresponding message will be part of the non-validation message.
 - A `list` or a `tuple`. Validation is done by first checking membership of the corresponding types, and then performing validation for each of the entries of the object being validated against the corresponding entries of the schema.
 - A dictionary. Validation is done by first checking membership of the `dict` type, and then performing validation for each of the items of the object being validated against the corresponding items of the schema.
 - A `set`. A set validates an object, if one of its members does.
 - An arbitrary Python object. Validation is done by checking equality of the schema and the object, except when the schema is of type `float`, in which case `math.isclose` is used.
 ## Creating types
@@ -321,21 +327,21 @@
 - `vtjson` can validate objects which are more general than strictly `JSON`. See the introductory example above. 
 - More fundamentally, the design philosophy of `vtsjon` is different. A `JSON` schema  is language independent and fully declarative. These are very nice properties but, this being said, declarative languages have a tendency to suffer from feature creep as they try to deal with more and more exotic use cases (e.g. `css`).  A `vtjson` schema on the other hand leverages the versatility of the Python language. It is generally declarative, with a limited, but easily extendable set of primitives. But if more functionality is needed then it can be extended by using appropriate bits of Python code (as the `ordered_pair` example below illustrates). In practice this is what you will need in any case since a purely declarative language will never be able to deal with every possible validation scenario. 
 
 Q: How is this different from https://pypi.org/project/json-checker/ \?
 
 A: Good question! I discovered `json-checker` after I had written `vtjson`. Although the details are different `json-checker` and `vtjson` share many of the same principles.
 
-Q: Why are there no variables in vtjson (see https://opis.io/json-schema/2.x/variables.html)?
+Q: Why are there no variables in `vtjson` (see https://opis.io/json-schema/2.x/variables.html)?
 
 A: They did not seem to be essential yet. In our use cases conditional schemas were sufficient to achieve the required functionality. See for example the `action_schema` in <a href=https://raw.githubusercontent.com/official-stockfish/fishtest/master/server/fishtest/schemas.py>`schemas.py`</a>. More importantly `vtjson` has a strict separation between the definition of a schema and its subsequent use for validation. By allowing a schema to refer directly to the object being validated this separation would become blurred. This being said, I am still thinking about a good way to introduce variables.
 
-Q: Does vtjson support recursive schemas?
+Q: Does `vtjson` support recursive schemas?
 
-A: Yes but it requires a bit of Python gymnastics to create them. Here is an example
+A: Yes. But it requires a bit of Python gymnastics to create them. Here is an example
 ```python
 person={}
 person["mother"]=union(person, None)
 person["father"]=union(person, None)
 ```
 which matches e.g.
 ```python
```

### Comparing `vtjson-1.7.2/README.md` & `vtjson-1.7.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -232,15 +232,21 @@
 - `size(lowerbound, upperbound)`. Matches the objects (which support `len()` such as strings or lists) whose length is in the interval `[upperbound, lowerbound]`. The value of `upperbound` can be `...` (ellipsis).
 ## Conditional schemas
 - `ifthen(if_schema, then_schema, else_schema=None)`. It the object matches the `if_schema` then it should also match the `then_schema`. If the object does not match the `if_schema` then it should match
 the `else_schema`, if present.
 - `cond((if_schema1, then_schema1), ... , (if_schemaN, then_schemaN))`. An object is successively validated against `if_schema1`, `if_schema2`, ... until a validation succeeds. When this happens the object should
 match the corresponding `then_schema`. If no `if_schema` succeeds then the object is considered to have been validated. If one sets `if_schemaN` equal to `anything` then this serves as a catch all.
 ## Pre-compiling a schema
-- An object matches the schema `compile(schema)` if it matches `schema`. `vtjson` compiles the schema before performing a validation so pre-compiling is not necessary but, in some cases, it may gain a bit of performance. 
+An object matches the schema `compile(schema)` if it matches `schema`. `vtjson` compiles a schema before performing a validation against it, so pre-compiling is not necessary but it gains a bit of performance as it needs to be done only once. Compiling is an idempotent operation. It does nothing for an already compiled schema.
+
+The full signature of `compile()` is
+```python
+compile(schema, _deferred_compiles=None)
+```
+but the optional argument `_deferred_compiles` should not be set by the user.
 ## Format
 A schema can be, in order of precedence:
 - A class with the following properties:
   - it has a no-argument constructor;
   - the instances have a `__validate__` method with signature
   ```python
   __validate__(self, object, name, strict)
@@ -251,15 +257,15 @@
   __validate__(object, name, strict)
   ```
   as above.
 - An object having a `__compile__` attribute with signature
   ```python
   __compile__(_deferred_compiles=None)
   ```
-  This is an advanced feature which is used for the implementation of wrapper schemas. Please consult the source code of `vtjson` for more details.
+  This is an advanced feature which is used for the implementation of wrapper schemas. `__compile__()`, which is invoked by `compile()`, should produce an object with a `__validate__` attribute as described above. The optional argument `_deferred_compiles` is an opaque data structure for handling recursive schemas. It should be passed unmodified to any internal invokations of `compile()`. Please consult the source code of `vtjson` for more details.
 - A Python type. In that case validation is done by checking membership.
 - A callable. Validation is done by applying the callable to the object. If applying the callable throws an exception then the corresponding message will be part of the non-validation message.
 - A `list` or a `tuple`. Validation is done by first checking membership of the corresponding types, and then performing validation for each of the entries of the object being validated against the corresponding entries of the schema.
 - A dictionary. Validation is done by first checking membership of the `dict` type, and then performing validation for each of the items of the object being validated against the corresponding items of the schema.
 - A `set`. A set validates an object, if one of its members does.
 - An arbitrary Python object. Validation is done by checking equality of the schema and the object, except when the schema is of type `float`, in which case `math.isclose` is used.
 ## Creating types
@@ -304,21 +310,21 @@
 - `vtjson` can validate objects which are more general than strictly `JSON`. See the introductory example above. 
 - More fundamentally, the design philosophy of `vtsjon` is different. A `JSON` schema  is language independent and fully declarative. These are very nice properties but, this being said, declarative languages have a tendency to suffer from feature creep as they try to deal with more and more exotic use cases (e.g. `css`).  A `vtjson` schema on the other hand leverages the versatility of the Python language. It is generally declarative, with a limited, but easily extendable set of primitives. But if more functionality is needed then it can be extended by using appropriate bits of Python code (as the `ordered_pair` example below illustrates). In practice this is what you will need in any case since a purely declarative language will never be able to deal with every possible validation scenario. 
 
 Q: How is this different from https://pypi.org/project/json-checker/ \?
 
 A: Good question! I discovered `json-checker` after I had written `vtjson`. Although the details are different `json-checker` and `vtjson` share many of the same principles.
 
-Q: Why are there no variables in vtjson (see https://opis.io/json-schema/2.x/variables.html)?
+Q: Why are there no variables in `vtjson` (see https://opis.io/json-schema/2.x/variables.html)?
 
 A: They did not seem to be essential yet. In our use cases conditional schemas were sufficient to achieve the required functionality. See for example the `action_schema` in <a href=https://raw.githubusercontent.com/official-stockfish/fishtest/master/server/fishtest/schemas.py>`schemas.py`</a>. More importantly `vtjson` has a strict separation between the definition of a schema and its subsequent use for validation. By allowing a schema to refer directly to the object being validated this separation would become blurred. This being said, I am still thinking about a good way to introduce variables.
 
-Q: Does vtjson support recursive schemas?
+Q: Does `vtjson` support recursive schemas?
 
-A: Yes but it requires a bit of Python gymnastics to create them. Here is an example
+A: Yes. But it requires a bit of Python gymnastics to create them. Here is an example
 ```python
 person={}
 person["mother"]=union(person, None)
 person["father"]=union(person, None)
 ```
 which matches e.g.
 ```python
```

### Comparing `vtjson-1.7.2/pyproject.toml` & `vtjson-1.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vtjson-1.7.2/vtjson.egg-info/PKG-INFO` & `vtjson-1.7.3/vtjson.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtjson
-Version: 1.7.2
+Version: 1.7.3
 Summary: A lightweight package for validating JSON like Python objects
 Author-email: Michel Van den Bergh <michel.vandenbergh@uhasselt.be>
 Project-URL: Homepage, https://github.com/vdbergh/vtjson
 Project-URL: Bug Tracker, https://github.com/vdbergh/vtjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -249,15 +249,21 @@
 - `size(lowerbound, upperbound)`. Matches the objects (which support `len()` such as strings or lists) whose length is in the interval `[upperbound, lowerbound]`. The value of `upperbound` can be `...` (ellipsis).
 ## Conditional schemas
 - `ifthen(if_schema, then_schema, else_schema=None)`. It the object matches the `if_schema` then it should also match the `then_schema`. If the object does not match the `if_schema` then it should match
 the `else_schema`, if present.
 - `cond((if_schema1, then_schema1), ... , (if_schemaN, then_schemaN))`. An object is successively validated against `if_schema1`, `if_schema2`, ... until a validation succeeds. When this happens the object should
 match the corresponding `then_schema`. If no `if_schema` succeeds then the object is considered to have been validated. If one sets `if_schemaN` equal to `anything` then this serves as a catch all.
 ## Pre-compiling a schema
-- An object matches the schema `compile(schema)` if it matches `schema`. `vtjson` compiles the schema before performing a validation so pre-compiling is not necessary but, in some cases, it may gain a bit of performance. 
+An object matches the schema `compile(schema)` if it matches `schema`. `vtjson` compiles a schema before performing a validation against it, so pre-compiling is not necessary but it gains a bit of performance as it needs to be done only once. Compiling is an idempotent operation. It does nothing for an already compiled schema.
+
+The full signature of `compile()` is
+```python
+compile(schema, _deferred_compiles=None)
+```
+but the optional argument `_deferred_compiles` should not be set by the user.
 ## Format
 A schema can be, in order of precedence:
 - A class with the following properties:
   - it has a no-argument constructor;
   - the instances have a `__validate__` method with signature
   ```python
   __validate__(self, object, name, strict)
@@ -268,15 +274,15 @@
   __validate__(object, name, strict)
   ```
   as above.
 - An object having a `__compile__` attribute with signature
   ```python
   __compile__(_deferred_compiles=None)
   ```
-  This is an advanced feature which is used for the implementation of wrapper schemas. Please consult the source code of `vtjson` for more details.
+  This is an advanced feature which is used for the implementation of wrapper schemas. `__compile__()`, which is invoked by `compile()`, should produce an object with a `__validate__` attribute as described above. The optional argument `_deferred_compiles` is an opaque data structure for handling recursive schemas. It should be passed unmodified to any internal invokations of `compile()`. Please consult the source code of `vtjson` for more details.
 - A Python type. In that case validation is done by checking membership.
 - A callable. Validation is done by applying the callable to the object. If applying the callable throws an exception then the corresponding message will be part of the non-validation message.
 - A `list` or a `tuple`. Validation is done by first checking membership of the corresponding types, and then performing validation for each of the entries of the object being validated against the corresponding entries of the schema.
 - A dictionary. Validation is done by first checking membership of the `dict` type, and then performing validation for each of the items of the object being validated against the corresponding items of the schema.
 - A `set`. A set validates an object, if one of its members does.
 - An arbitrary Python object. Validation is done by checking equality of the schema and the object, except when the schema is of type `float`, in which case `math.isclose` is used.
 ## Creating types
@@ -321,21 +327,21 @@
 - `vtjson` can validate objects which are more general than strictly `JSON`. See the introductory example above. 
 - More fundamentally, the design philosophy of `vtsjon` is different. A `JSON` schema  is language independent and fully declarative. These are very nice properties but, this being said, declarative languages have a tendency to suffer from feature creep as they try to deal with more and more exotic use cases (e.g. `css`).  A `vtjson` schema on the other hand leverages the versatility of the Python language. It is generally declarative, with a limited, but easily extendable set of primitives. But if more functionality is needed then it can be extended by using appropriate bits of Python code (as the `ordered_pair` example below illustrates). In practice this is what you will need in any case since a purely declarative language will never be able to deal with every possible validation scenario. 
 
 Q: How is this different from https://pypi.org/project/json-checker/ \?
 
 A: Good question! I discovered `json-checker` after I had written `vtjson`. Although the details are different `json-checker` and `vtjson` share many of the same principles.
 
-Q: Why are there no variables in vtjson (see https://opis.io/json-schema/2.x/variables.html)?
+Q: Why are there no variables in `vtjson` (see https://opis.io/json-schema/2.x/variables.html)?
 
 A: They did not seem to be essential yet. In our use cases conditional schemas were sufficient to achieve the required functionality. See for example the `action_schema` in <a href=https://raw.githubusercontent.com/official-stockfish/fishtest/master/server/fishtest/schemas.py>`schemas.py`</a>. More importantly `vtjson` has a strict separation between the definition of a schema and its subsequent use for validation. By allowing a schema to refer directly to the object being validated this separation would become blurred. This being said, I am still thinking about a good way to introduce variables.
 
-Q: Does vtjson support recursive schemas?
+Q: Does `vtjson` support recursive schemas?
 
-A: Yes but it requires a bit of Python gymnastics to create them. Here is an example
+A: Yes. But it requires a bit of Python gymnastics to create them. Here is an example
 ```python
 person={}
 person["mother"]=union(person, None)
 person["father"]=union(person, None)
 ```
 which matches e.g.
 ```python
```

### Comparing `vtjson-1.7.2/vtjson.py` & `vtjson-1.7.3/vtjson.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     from types import GenericAlias as _GenericAlias
 except ImportError:
     # For compatibility with older Pythons
     class _GenericAlias(type):
         pass
 
 
-__version__ = "1.7.2"
+__version__ = "1.7.3"
 
 
 _dns_resolver = None
 
 
 def _get_dns_resolver():
     global _dns_resolver
```

