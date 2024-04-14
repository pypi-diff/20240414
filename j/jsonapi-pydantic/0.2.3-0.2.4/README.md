# Comparing `tmp/jsonapi_pydantic-0.2.3.tar.gz` & `tmp/jsonapi_pydantic-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonapi_pydantic-0.2.3.tar", max compression
+gzip compressed data, was "jsonapi_pydantic-0.2.4.tar", max compression
```

## Comparing `jsonapi_pydantic-0.2.3.tar` & `jsonapi_pydantic-0.2.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      101 2023-12-06 08:03:54.699313 jsonapi_pydantic-0.2.3/jsonapi_pydantic/__init__.py
--rw-r--r--   0        0        0      223 2022-10-15 16:23:47.000000 jsonapi_pydantic-0.2.3/jsonapi_pydantic/constants.py
--rw-r--r--   0        0        0      315 2022-09-13 11:40:10.000000 jsonapi_pydantic-0.2.3/jsonapi_pydantic/v1_0/__init__.py
--rw-r--r--   0        0        0     1055 2023-08-04 11:32:28.323520 jsonapi_pydantic-0.2.3/jsonapi_pydantic/v1_0/error.py
--rw-r--r--   0        0        0      358 2023-08-04 11:32:28.323520 jsonapi_pydantic-0.2.3/jsonapi_pydantic/v1_0/jsonapi.py
--rw-r--r--   0        0        0      809 2023-08-04 11:32:28.323520 jsonapi_pydantic-0.2.3/jsonapi_pydantic/v1_0/links.py
--rw-r--r--   0        0        0       73 2022-07-16 14:53:20.000000 jsonapi_pydantic-0.2.3/jsonapi_pydantic/v1_0/meta.py
--rw-r--r--   0        0        0      176 2022-07-16 14:32:16.000000 jsonapi_pydantic-0.2.3/jsonapi_pydantic/v1_0/resource/__init__.py
--rw-r--r--   0        0        0     1130 2023-09-05 12:19:54.281301 jsonapi_pydantic-0.2.3/jsonapi_pydantic/v1_0/resource/relationship.py
--rw-r--r--   0        0        0      948 2023-08-04 11:32:28.324519 jsonapi_pydantic-0.2.3/jsonapi_pydantic/v1_0/resource/relationship_links.py
--rw-r--r--   0        0        0     2182 2023-12-06 07:41:32.356242 jsonapi_pydantic-0.2.3/jsonapi_pydantic/v1_0/resource/resource.py
--rw-r--r--   0        0        0      455 2023-08-29 11:53:16.320452 jsonapi_pydantic-0.2.3/jsonapi_pydantic/v1_0/resource_identifier.py
--rw-r--r--   0        0        0     1965 2023-09-05 12:19:54.279301 jsonapi_pydantic-0.2.3/jsonapi_pydantic/v1_0/toplevel.py
--rw-r--r--   0        0        0     1142 2023-12-06 08:04:01.661314 jsonapi_pydantic-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2802 2022-07-27 18:48:54.000000 jsonapi_pydantic-0.2.3/readme.md
--rw-r--r--   0        0        0     3831 1970-01-01 00:00:00.000000 jsonapi_pydantic-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      101 2024-04-14 13:12:29.646841 jsonapi_pydantic-0.2.4/jsonapi_pydantic/__init__.py
+-rw-r--r--   0        0        0      223 2022-10-15 16:23:47.000000 jsonapi_pydantic-0.2.4/jsonapi_pydantic/constants.py
+-rw-r--r--   0        0        0      267 2024-04-14 13:19:02.062988 jsonapi_pydantic-0.2.4/jsonapi_pydantic/utils.py
+-rw-r--r--   0        0        0      315 2022-09-13 11:40:10.000000 jsonapi_pydantic-0.2.4/jsonapi_pydantic/v1_0/__init__.py
+-rw-r--r--   0        0        0     1055 2023-08-04 11:32:28.323520 jsonapi_pydantic-0.2.4/jsonapi_pydantic/v1_0/error.py
+-rw-r--r--   0        0        0      358 2023-08-04 11:32:28.323520 jsonapi_pydantic-0.2.4/jsonapi_pydantic/v1_0/jsonapi.py
+-rw-r--r--   0        0        0      809 2023-08-04 11:32:28.323520 jsonapi_pydantic-0.2.4/jsonapi_pydantic/v1_0/links.py
+-rw-r--r--   0        0        0       73 2022-07-16 14:53:20.000000 jsonapi_pydantic-0.2.4/jsonapi_pydantic/v1_0/meta.py
+-rw-r--r--   0        0        0      176 2022-07-16 14:32:16.000000 jsonapi_pydantic-0.2.4/jsonapi_pydantic/v1_0/resource/__init__.py
+-rw-r--r--   0        0        0     1130 2023-09-05 12:19:54.281301 jsonapi_pydantic-0.2.4/jsonapi_pydantic/v1_0/resource/relationship.py
+-rw-r--r--   0        0        0      948 2023-08-04 11:32:28.324519 jsonapi_pydantic-0.2.4/jsonapi_pydantic/v1_0/resource/relationship_links.py
+-rw-r--r--   0        0        0     2738 2024-04-14 13:19:14.973125 jsonapi_pydantic-0.2.4/jsonapi_pydantic/v1_0/resource/resource.py
+-rw-r--r--   0        0        0      901 2024-04-14 13:20:05.757664 jsonapi_pydantic-0.2.4/jsonapi_pydantic/v1_0/resource_identifier.py
+-rw-r--r--   0        0        0     2271 2024-04-14 13:41:44.374878 jsonapi_pydantic-0.2.4/jsonapi_pydantic/v1_0/toplevel.py
+-rw-r--r--   0        0        0     1306 2024-04-14 13:43:51.853157 jsonapi_pydantic-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2924 2023-12-12 07:46:43.536044 jsonapi_pydantic-0.2.4/readme.md
+-rw-r--r--   0        0        0     4014 1970-01-01 00:00:00.000000 jsonapi_pydantic-0.2.4/PKG-INFO
```

### Comparing `jsonapi_pydantic-0.2.3/jsonapi_pydantic/v1_0/error.py` & `jsonapi_pydantic-0.2.4/jsonapi_pydantic/v1_0/error.py`

 * *Files identical despite different names*

### Comparing `jsonapi_pydantic-0.2.3/jsonapi_pydantic/v1_0/links.py` & `jsonapi_pydantic-0.2.4/jsonapi_pydantic/v1_0/links.py`

 * *Files identical despite different names*

### Comparing `jsonapi_pydantic-0.2.3/jsonapi_pydantic/v1_0/resource/relationship.py` & `jsonapi_pydantic-0.2.4/jsonapi_pydantic/v1_0/resource/relationship.py`

 * *Files identical despite different names*

### Comparing `jsonapi_pydantic-0.2.3/jsonapi_pydantic/v1_0/resource/relationship_links.py` & `jsonapi_pydantic-0.2.4/jsonapi_pydantic/v1_0/resource/relationship_links.py`

 * *Files identical despite different names*

### Comparing `jsonapi_pydantic-0.2.3/jsonapi_pydantic/v1_0/toplevel.py` & `jsonapi_pydantic-0.2.4/jsonapi_pydantic/v1_0/toplevel.py`

 * *Files 17% similar despite different names*

```diff
@@ -34,21 +34,31 @@
     jsonapi: JsonApi = Field(None, title="JSON:API")
     links: Links = Field(None, title="Links")
     included: Included = Field(None, title="Included")
 
     @model_validator(mode="before")
     def check_all_values(cls, data: dict) -> dict:
         # More about these restrictions: https://jsonapi.org/format/#document-top-level
-        if data.get("data") and data.get("errors"):
+        if "data" in data and "errors" in data:
             raise ValueError("The members data and errors MUST NOT coexist in the same document.")
-        if data.get("included") and not data.get("data"):
+
+        if "included" in data and "data" not in data:
             raise ValueError(
                 "If a document does not contain a top-level data key, the included member MUST NOT be present either."
             )
-        if not data.get("data") and not data.get("errors") and not data.get("meta"):
+
+        if "data" not in data and "errors" not in data and "meta" not in data:
             raise ValueError(
                 "A document MUST contain at least one of the following top-level members: data, errors, meta."
             )
+
+        if isinstance(data.get("data"), list):
+            hashes = {d._hash for d in data["data"]}
+            if len(data["data"]) > len(hashes):
+                raise ValueError(
+                    "A compound document MUST NOT include more than one resource object for each type and id pair."
+                )
+
         return data
 
 
 __all__ = ["TopLevel"]
```

### Comparing `jsonapi_pydantic-0.2.3/pyproject.toml` & `jsonapi_pydantic-0.2.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 [tool.poetry]
 name = "jsonapi-pydantic"
-version = "0.2.3"
+version = "0.2.4"
 description = "JSON:API implementation with pydantic."
 
 authors = ["impocode <impocode@impocode.com>"]
 maintainers = ["impocode <impocode@impocode.com>"]
 
 license= "MIT"
 readme = "readme.md"
 
 keywords = ["jsonapi", "pydantic"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Typing :: Typed",
 ]
 
 homepage = "https://github.com/impocode/jsonapi-pydantic"
 repository = "https://github.com/impocode/jsonapi-pydantic"
 documentation = "https://github.com/impocode/jsonapi-pydantic"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8.1"
 pydantic = "^2.1.1"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/impocode/jsonapi-pydantic/issues"
 
+[tool.poetry.group.dev.dependencies]
+black = "^23.12.0"
+isort = "^5.13.2"
+flake8 = "^6.1.0"
+pytest = "^8.1.1"
+
 [tool.isort]
-line_length = 99
+line_length = 100
 multi_line_output = 3
 include_trailing_comma = false
 
 [tool.black]
-line-length = 99
+line-length = 100
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `jsonapi_pydantic-0.2.3/readme.md` & `jsonapi_pydantic-0.2.4/readme.md`

 * *Files 20% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     "included": [
         {"type": "people", "id": "42", "attributes": {"name": "John", "age": 80, "gender": "male"}}
     ],
 }
 
 top_level = TopLevel(**external_data)
 
-print(top_level.dict(exclude_unset=True))
+print(top_level.model_dump(exclude_unset=True))
 """
 {
     "data": [
         {
             "type": "articles",
             "id": "1",
             "attributes": {
@@ -94,10 +94,14 @@
         links=None,
         meta=None,
     )
 ]
 """
 ```
 
+## Examples
+
+More examples can be found [here](https://github.com/impocode/jsonapi-pydantic/tree/master/examples).
+
 ## License
 
 See [license.md](https://github.com/impocode/jsonapi-pydantic/blob/master/license.md).
```

#### html2text {}

```diff
@@ -7,20 +7,22 @@
 ```python from jsonapi_pydantic.v1_0 import TopLevel external_data = { "data":
 [ { "type": "articles", "id": "1", "attributes": { "title": "JSON:API paints my
 bikeshed!", "body": "The shortest article. Ever.", "created": "2015-05-22T14:
 56:29.000Z", "updated": "2015-05-22T14:56:28.000Z", }, "relationships":
 {"author": {"data": {"id": "42", "type": "people"}}}, } ], "included": [
 {"type": "people", "id": "42", "attributes": {"name": "John", "age": 80,
 "gender": "male"}} ], } top_level = TopLevel(**external_data) print
-(top_level.dict(exclude_unset=True)) """ { "data": [ { "type": "articles",
-"id": "1", "attributes": { "title": "JSON:API paints my bikeshed!", "body":
-"The shortest article. Ever.", "created": "2015-05-22T14:56:29.000Z",
+(top_level.model_dump(exclude_unset=True)) """ { "data": [ { "type":
+"articles", "id": "1", "attributes": { "title": "JSON:API paints my bikeshed!",
+"body": "The shortest article. Ever.", "created": "2015-05-22T14:56:29.000Z",
 "updated": "2015-05-22T14:56:28.000Z", }, "relationships": {"author": {"data":
 {"id": "42", "type": "people"}}}, } ], "included": [ {"type": "people", "id":
 "42", "attributes": {"name": "John", "age": 80, "gender": "male"}} ], } """
 print(top_level.data) """ [ Resource( type="articles", id="1", attributes=
 { "title": "JSON:API paints my bikeshed!", "body": "The shortest article.
 Ever.", "created": "2015-05-22T14:56:29.000Z", "updated": "2015-05-22T14:56:
 28.000Z", }, relationships={ "author": Relationship( links=None,
 data=ResourceIdentifier(id="42", type="people", meta=None), meta=None ) },
-links=None, meta=None, ) ] """ ``` ## License See [license.md](https://
-github.com/impocode/jsonapi-pydantic/blob/master/license.md).
+links=None, meta=None, ) ] """ ``` ## Examples More examples can be found
+[here](https://github.com/impocode/jsonapi-pydantic/tree/master/examples). ##
+License See [license.md](https://github.com/impocode/jsonapi-pydantic/blob/
+master/license.md).
```

### Comparing `jsonapi_pydantic-0.2.3/PKG-INFO` & `jsonapi_pydantic-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: jsonapi-pydantic
-Version: 0.2.3
+Version: 0.2.4
 Summary: JSON:API implementation with pydantic.
 Home-page: https://github.com/impocode/jsonapi-pydantic
 License: MIT
 Keywords: jsonapi,pydantic
 Author: impocode
 Author-email: impocode@impocode.com
 Maintainer: impocode
 Maintainer-email: impocode@impocode.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Typing :: Typed
 Requires-Dist: pydantic (>=2.1.1,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/impocode/jsonapi-pydantic/issues
 Project-URL: Documentation, https://github.com/impocode/jsonapi-pydantic
 Project-URL: Repository, https://github.com/impocode/jsonapi-pydantic
 Description-Content-Type: text/markdown
 
@@ -75,15 +76,15 @@
     "included": [
         {"type": "people", "id": "42", "attributes": {"name": "John", "age": 80, "gender": "male"}}
     ],
 }
 
 top_level = TopLevel(**external_data)
 
-print(top_level.dict(exclude_unset=True))
+print(top_level.model_dump(exclude_unset=True))
 """
 {
     "data": [
         {
             "type": "articles",
             "id": "1",
             "attributes": {
@@ -120,11 +121,15 @@
         links=None,
         meta=None,
     )
 ]
 """
 ```
 
+## Examples
+
+More examples can be found [here](https://github.com/impocode/jsonapi-pydantic/tree/master/examples).
+
 ## License
 
 See [license.md](https://github.com/impocode/jsonapi-pydantic/blob/master/license.md).
```

#### html2text {}

```diff
@@ -1,39 +1,42 @@
-Metadata-Version: 2.1 Name: jsonapi-pydantic Version: 0.2.3 Summary: JSON:API
+Metadata-Version: 2.1 Name: jsonapi-pydantic Version: 0.2.4 Summary: JSON:API
 implementation with pydantic. Home-page: https://github.com/impocode/jsonapi-
 pydantic License: MIT Keywords: jsonapi,pydantic Author: impocode Author-email:
 impocode@impocode.com Maintainer: impocode Maintainer-email:
-impocode@impocode.com Requires-Python: >=3.7,<4.0 Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Typing :: Typed Requires-Dist: pydantic
-(>=2.1.1,<3.0.0) Project-URL: Bug Tracker, https://github.com/impocode/jsonapi-
-pydantic/issues Project-URL: Documentation, https://github.com/impocode/
-jsonapi-pydantic Project-URL: Repository, https://github.com/impocode/jsonapi-
-pydantic Description-Content-Type: text/markdown # jsonapi-pydantic
+impocode@impocode.com Requires-Python: >=3.8.1,<4.0.0 Classifier: License ::
+OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Classifier: Programming
+Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
+3.8 Classifier: Typing :: Typed Requires-Dist: pydantic (>=2.1.1,<3.0.0)
+Project-URL: Bug Tracker, https://github.com/impocode/jsonapi-pydantic/issues
+Project-URL: Documentation, https://github.com/impocode/jsonapi-pydantic
+Project-URL: Repository, https://github.com/impocode/jsonapi-pydantic
+Description-Content-Type: text/markdown # jsonapi-pydantic
                     _JJ_SS_OO_NN_::_AA_PP_II iimmpplleemmeennttaattiioonn wwiitthh _PP_yy_dd_aa_nn_tt_ii_cc_..
                                 _[_P_y_P_I_]_[_L_i_c_e_n_s_e_]
 ## Description `jsonapi-pydantic` provides a suite of Pydantic models matching
 the JSON:API specification. ## Install ```shell $ pip install jsonapi-pydantic
 ``` Or use your python package manager. ## Usage Object with primary data:
 ```python from jsonapi_pydantic.v1_0 import TopLevel external_data = { "data":
 [ { "type": "articles", "id": "1", "attributes": { "title": "JSON:API paints my
 bikeshed!", "body": "The shortest article. Ever.", "created": "2015-05-22T14:
 56:29.000Z", "updated": "2015-05-22T14:56:28.000Z", }, "relationships":
 {"author": {"data": {"id": "42", "type": "people"}}}, } ], "included": [
 {"type": "people", "id": "42", "attributes": {"name": "John", "age": 80,
 "gender": "male"}} ], } top_level = TopLevel(**external_data) print
-(top_level.dict(exclude_unset=True)) """ { "data": [ { "type": "articles",
-"id": "1", "attributes": { "title": "JSON:API paints my bikeshed!", "body":
-"The shortest article. Ever.", "created": "2015-05-22T14:56:29.000Z",
+(top_level.model_dump(exclude_unset=True)) """ { "data": [ { "type":
+"articles", "id": "1", "attributes": { "title": "JSON:API paints my bikeshed!",
+"body": "The shortest article. Ever.", "created": "2015-05-22T14:56:29.000Z",
 "updated": "2015-05-22T14:56:28.000Z", }, "relationships": {"author": {"data":
 {"id": "42", "type": "people"}}}, } ], "included": [ {"type": "people", "id":
 "42", "attributes": {"name": "John", "age": 80, "gender": "male"}} ], } """
 print(top_level.data) """ [ Resource( type="articles", id="1", attributes=
 { "title": "JSON:API paints my bikeshed!", "body": "The shortest article.
 Ever.", "created": "2015-05-22T14:56:29.000Z", "updated": "2015-05-22T14:56:
 28.000Z", }, relationships={ "author": Relationship( links=None,
 data=ResourceIdentifier(id="42", type="people", meta=None), meta=None ) },
-links=None, meta=None, ) ] """ ``` ## License See [license.md](https://
-github.com/impocode/jsonapi-pydantic/blob/master/license.md).
+links=None, meta=None, ) ] """ ``` ## Examples More examples can be found
+[here](https://github.com/impocode/jsonapi-pydantic/tree/master/examples). ##
+License See [license.md](https://github.com/impocode/jsonapi-pydantic/blob/
+master/license.md).
```

