# Comparing `tmp/imgw_data-0.1.1.tar.gz` & `tmp/imgw_data-0.1.2.tar.gz`

## Comparing `imgw_data-0.1.1.tar` & `imgw_data-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 imgw_data-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 imgw_data-0.1.1/CONTRIBUTING.md
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 imgw_data-0.1.1/requirements-dev.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 imgw_data-0.1.1/src/imgw_data/__about__.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 imgw_data-0.1.1/src/imgw_data/__init__.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 imgw_data-0.1.1/src/imgw_data/consts.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 imgw_data-0.1.1/src/imgw_data/get.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 imgw_data-0.1.1/src/imgw_data/export/__init__.py
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 imgw_data-0.1.1/src/imgw_data/export/export.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 imgw_data-0.1.1/src/imgw_data/utils/__init__.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 imgw_data-0.1.1/src/imgw_data/utils/parse.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 imgw_data-0.1.1/src/imgw_data/utils/translate.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 imgw_data-0.1.1/src/imgw_data/utils/urljoin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 imgw_data-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 imgw_data-0.1.1/.gitignore
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 imgw_data-0.1.1/LICENSE
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 imgw_data-0.1.1/README.md
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 imgw_data-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 imgw_data-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 imgw_data-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 imgw_data-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 imgw_data-0.1.2/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 imgw_data-0.1.2/src/imgw_data/__about__.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 imgw_data-0.1.2/src/imgw_data/__init__.py
+-rw-r--r--   0        0        0    91808 2020-02-02 00:00:00.000000 imgw_data-0.1.2/src/imgw_data/consts.py
+-rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 imgw_data-0.1.2/src/imgw_data/get.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 imgw_data-0.1.2/src/imgw_data/export/__init__.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 imgw_data-0.1.2/src/imgw_data/export/export.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 imgw_data-0.1.2/src/imgw_data/utils/__init__.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 imgw_data-0.1.2/src/imgw_data/utils/parse.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 imgw_data-0.1.2/src/imgw_data/utils/translate.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 imgw_data-0.1.2/src/imgw_data/utils/urljoin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 imgw_data-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 imgw_data-0.1.2/tests/test_load.py
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 imgw_data-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 imgw_data-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 imgw_data-0.1.2/README.md
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 imgw_data-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 imgw_data-0.1.2/PKG-INFO
```

### Comparing `imgw_data-0.1.1/CONTRIBUTING.md` & `imgw_data-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `imgw_data-0.1.1/src/imgw_data/get.py` & `imgw_data-0.1.2/src/imgw_data/get.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from typing import Union
-
 import requests
-from src.imgw_data.consts import IMGWUrls, IMGWDataFormats
+from src.imgw_data.consts import IMGWUrls, IMGWDataFormats, IMGWStationsCoordinates
 from src.imgw_data.export.export import export_to_file
-from src.imgw_data.utils.parse import parse_response
+from src.imgw_data.utils.parse import parse_response, add_coordinates
 from src.imgw_data.utils.translate import translate_synoptic
 from src.imgw_data.utils.urljoin import urljoin
 
 
 def _build_format_url(urlbase: str,
                       is_json=True,
                       is_csv=False,
@@ -30,86 +28,98 @@
 
     Returns
     -------
     url : str
     """
 
     if is_json:
-        return urlbase
+        return urlbase, 'json'
     elif is_csv:
-        return urljoin(urlbase, 'format', IMGWDataFormats.CSV.value)
+        return urljoin(urlbase, 'format', IMGWDataFormats.CSV.value), 'csv'
     elif is_xml:
-        return urljoin(urlbase, 'format', IMGWDataFormats.XML.value)
+        return urljoin(urlbase, 'format', IMGWDataFormats.XML.value), 'xml'
     elif is_html:
-        return urljoin(urlbase, 'format', IMGWDataFormats.HTML.value)
+        return urljoin(urlbase, 'format', IMGWDataFormats.HTML.value), 'html'
 
-    return urlbase
+    return urlbase, 'json'
 
 
 def get_current_weather(
         fname: str = None,
         translate_to_english=True,
+        add_station_coordinates=True,
         as_json=False,
         as_csv=False,
         as_xml=False,
         as_html=False,
+        raise_error_on_missing_coordinates=False
 ):
     """
     Function gets current weather from IMGW website.
 
     Parameters
     ----------
     fname : str, optional
         Filename where to store readings. If provided then function saves data instead of returning it.
 
     translate_to_english : bool, default = true
         Translate weather readings keys to English.
 
+    add_station_coordinates : bool, default = True
+        Add station coordinates. Works only with json output.
+
     as_json : bool, default = False
         Save output to json.
 
     as_csv : bool, default = False
         Save output to csv.
 
     as_xml : bool, default = False
         Save output as xml file.
 
     as_html : bool, default = False
         Save output as html.
 
+    raise_error_on_missing_coordinates : bool, default = False
+        Raise ``ValueError`` if coordinates are missing.
+
     Notes
     -----
     If all file type parameters are set to ``False`` then system downloads default JSON.
     """
 
     base_url = IMGWUrls.SYNOPTIC.value
 
-    url = _build_format_url(
+    url, ftype = _build_format_url(
         urlbase=base_url,
         is_json=as_json,
         is_csv=as_csv,
         is_xml=as_xml,
         is_html=as_html
     )
 
     response = requests.get(url=url)
 
     # Parse response
     parsed = parse_response(
-        response, url
+        response, ftype
     )
 
     if translate_to_english:
         parsed = translate_synoptic(parsed)
 
+    if add_station_coordinates and ftype == 'json':
+        parsed = add_coordinates(
+            readings=parsed,
+            coordinates=IMGWStationsCoordinates.stations['data'],
+            raise_error_if_missing=raise_error_on_missing_coordinates
+        )
+
     if fname is None:
         return parsed
     else:
         # Save data
         export_to_file(
             ds=parsed,
             fname=fname,
-            as_json=as_json,
-            as_csv=as_csv,
-            as_xml=as_xml,
-            as_html=as_html
+            ftype=ftype
         )
```

### Comparing `imgw_data-0.1.1/src/imgw_data/export/export.py` & `imgw_data-0.1.2/src/imgw_data/export/export.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,47 +16,41 @@
     checked : str
     """
     if fname.endswith(suffix):
         return fname
     return fname + '.' + suffix
 
 
-def export_to_file(ds, fname: str, as_json=False, as_csv=False, as_xml=False, as_html=False):
+def export_to_file(ds, fname: str, ftype: str):
     """
     Function exports dataset to a specific file.
 
     Parameters
     ----------
     ds : Union[list[dict], str]
 
     fname : str
 
-    as_json : bool, default=False
-
-    as_csv : bool, default=False
-
-    as_xml : bool, default=False
-
-    as_html : bool, default=False
+    ftype : str
     """
 
-    if as_json:
+    if ftype == 'json':
         fname = _check_filesuffix(fname, suffix='json')
         if isinstance(ds, list):
             with open(fname, 'w', encoding='utf8') as fin:
                 json.dump(ds, fin, indent=2, ensure_ascii=False)
         elif isinstance(ds, str):
             with open(fname, 'w', encoding='utf8') as fin:
                 serialized = json.dumps(ds, ensure_ascii=False).encode('utf-8')
                 fin.write(serialized)
     else:
-        if as_csv:
+        if ftype == 'csv':
             fname = _check_filesuffix(fname, suffix='csv')
-        elif as_xml:
+        elif ftype == 'xml':
             fname = _check_filesuffix(fname, suffix='xml')
-        elif as_html:
+        elif ftype == 'html':
             fname = _check_filesuffix(fname, suffix='html')
         else:
-            raise TypeError('Output file format must be set!')
+            raise TypeError('Unknown output file type!')
 
         with open(fname, 'w', encoding='utf8') as fin:
             fin.write(ds)
```

### Comparing `imgw_data-0.1.1/src/imgw_data/utils/translate.py` & `imgw_data-0.1.2/src/imgw_data/utils/translate.py`

 * *Files identical despite different names*

### Comparing `imgw_data-0.1.1/src/imgw_data/utils/urljoin.py` & `imgw_data-0.1.2/src/imgw_data/utils/urljoin.py`

 * *Files identical despite different names*

### Comparing `imgw_data-0.1.1/.gitignore` & `imgw_data-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `imgw_data-0.1.1/LICENSE` & `imgw_data-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `imgw_data-0.1.1/README.md` & `imgw_data-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `imgw_data-0.1.1/pyproject.toml` & `imgw_data-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "imgw-data"
-version = "0.1.1"
+version = "0.1.2"
 description = 'Python API for public IMGW data - atmospheric measurement from Polish weather stations'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "BSD-3-Clause"
 keywords = ["weather", "weather stations", "poland", "api", "atmospheric science"]
 authors = [
   { name = "Szymon Moliński", email = "simon@ml-gis-service.com" },
```

### Comparing `imgw_data-0.1.1/PKG-INFO` & `imgw_data-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: imgw-data
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python API for public IMGW data - atmospheric measurement from Polish weather stations
 Project-URL: Documentation, https://github.com/SimonMolinsky/imgw-data-loader#readme
 Project-URL: Issues, https://github.com/SimonMolinsky/imgw-data-loader/issues
 Project-URL: Source, https://github.com/SimonMolinsky/imgw-data-loader
 Author-email: Szymon Moliński <simon@ml-gis-service.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
```

