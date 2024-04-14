# Comparing `tmp/pdfsyntax-0.0.8.tar.gz` & `tmp/pdfsyntax-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfsyntax-0.0.8.tar", last modified: Sun Jan 21 18:24:46 2024, max compression
+gzip compressed data, was "pdfsyntax-0.1.0.tar", last modified: Sun Apr 14 20:58:52 2024, max compression
```

## Comparing `pdfsyntax-0.0.8.tar` & `pdfsyntax-0.1.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 dej       (1000) dej       (1000)        0 2024-01-21 18:24:46.570536 pdfsyntax-0.0.8/
--rw-r--r--   0 dej       (1000) dej       (1000)     1092 2024-01-20 19:09:05.000000 pdfsyntax-0.0.8/LICENSE
--rw-r--r--   0 dej       (1000) dej       (1000)     5788 2024-01-21 18:24:46.569536 pdfsyntax-0.0.8/PKG-INFO
--rw-r--r--   0 dej       (1000) dej       (1000)     3795 2023-09-10 20:01:07.000000 pdfsyntax-0.0.8/README.md
-drwxr-xr-x   0 dej       (1000) dej       (1000)        0 2024-01-21 18:24:46.565536 pdfsyntax-0.0.8/pdfsyntax/
--rw-r--r--   0 dej       (1000) dej       (1000)       58 2022-08-09 20:53:21.000000 pdfsyntax-0.0.8/pdfsyntax/__init__.py
--rw-r--r--   0 dej       (1000) dej       (1000)       32 2022-05-02 17:43:04.000000 pdfsyntax-0.0.8/pdfsyntax/__main__.py
--rw-r--r--   0 dej       (1000) dej       (1000)     9155 2024-01-20 18:56:46.000000 pdfsyntax-0.0.8/pdfsyntax/api.py
--rw-r--r--   0 dej       (1000) dej       (1000)     5061 2024-01-14 16:08:33.000000 pdfsyntax-0.0.8/pdfsyntax/cli.py
--rw-r--r--   0 dej       (1000) dej       (1000)     9185 2023-12-31 21:04:26.000000 pdfsyntax-0.0.8/pdfsyntax/display.py
--rw-r--r--   0 dej       (1000) dej       (1000)    20127 2024-01-20 19:07:59.000000 pdfsyntax-0.0.8/pdfsyntax/docstruct.py
--rw-r--r--   0 dej       (1000) dej       (1000)    19646 2024-01-20 19:06:56.000000 pdfsyntax-0.0.8/pdfsyntax/filestruct.py
--rw-r--r--   0 dej       (1000) dej       (1000)     3412 2024-01-21 14:38:09.000000 pdfsyntax-0.0.8/pdfsyntax/filters.py
--rw-r--r--   0 dej       (1000) dej       (1000)     4672 2023-12-29 22:30:13.000000 pdfsyntax-0.0.8/pdfsyntax/graphics.py
--rw-r--r--   0 dej       (1000) dej       (1000)     4561 2023-12-29 22:31:00.000000 pdfsyntax-0.0.8/pdfsyntax/layout.py
--rw-r--r--   0 dej       (1000) dej       (1000)     9389 2024-01-16 20:36:31.000000 pdfsyntax-0.0.8/pdfsyntax/objects.py
--rw-r--r--   0 dej       (1000) dej       (1000)     7093 2024-01-14 16:11:22.000000 pdfsyntax-0.0.8/pdfsyntax/text.py
-drwxr-xr-x   0 dej       (1000) dej       (1000)        0 2024-01-21 18:24:46.569536 pdfsyntax-0.0.8/pdfsyntax.egg-info/
--rw-r--r--   0 dej       (1000) dej       (1000)     5788 2024-01-21 18:24:46.000000 pdfsyntax-0.0.8/pdfsyntax.egg-info/PKG-INFO
--rw-r--r--   0 dej       (1000) dej       (1000)      622 2024-01-21 18:24:46.000000 pdfsyntax-0.0.8/pdfsyntax.egg-info/SOURCES.txt
--rw-r--r--   0 dej       (1000) dej       (1000)        1 2024-01-21 18:24:46.000000 pdfsyntax-0.0.8/pdfsyntax.egg-info/dependency_links.txt
--rw-r--r--   0 dej       (1000) dej       (1000)       10 2024-01-21 18:24:46.000000 pdfsyntax-0.0.8/pdfsyntax.egg-info/top_level.txt
--rw-r--r--   0 dej       (1000) dej       (1000)      856 2024-01-21 18:17:49.000000 pdfsyntax-0.0.8/pyproject.toml
--rw-r--r--   0 dej       (1000) dej       (1000)       38 2024-01-21 18:24:46.571536 pdfsyntax-0.0.8/setup.cfg
-drwxr-xr-x   0 dej       (1000) dej       (1000)        0 2024-01-21 18:24:46.568536 pdfsyntax-0.0.8/tests/
--rw-r--r--   0 dej       (1000) dej       (1000)     1499 2024-01-06 20:43:45.000000 pdfsyntax-0.0.8/tests/test_bdata.py
--rw-r--r--   0 dej       (1000) dej       (1000)      705 2023-09-10 19:21:38.000000 pdfsyntax-0.0.8/tests/test_dependencies.py
--rw-r--r--   0 dej       (1000) dej       (1000)     2668 2023-06-29 21:07:04.000000 pdfsyntax-0.0.8/tests/test_parsing.py
--rw-r--r--   0 dej       (1000) dej       (1000)      303 2022-09-13 20:49:14.000000 pdfsyntax-0.0.8/tests/test_serialization.py
--rw-r--r--   0 dej       (1000) dej       (1000)      458 2023-09-10 19:21:40.000000 pdfsyntax-0.0.8/tests/test_simplefile.py
--rw-r--r--   0 dej       (1000) dej       (1000)     1044 2023-04-20 21:04:55.000000 pdfsyntax-0.0.8/tests/test_text.py
--rw-r--r--   0 dej       (1000) dej       (1000)     2349 2023-07-20 03:31:13.000000 pdfsyntax-0.0.8/tests/test_tokenization.py
--rw-r--r--   0 dej       (1000) dej       (1000)      359 2023-09-10 19:21:36.000000 pdfsyntax-0.0.8/tests/test_updating.py
--rw-r--r--   0 dej       (1000) dej       (1000)      542 2023-04-02 20:58:32.000000 pdfsyntax-0.0.8/tests/test_xref.py
+drwxr-xr-x   0 dej       (1000) dej       (1000)        0 2024-04-14 20:58:52.217604 pdfsyntax-0.1.0/
+-rw-r--r--   0 dej       (1000) dej       (1000)     1092 2024-01-20 19:09:05.000000 pdfsyntax-0.1.0/LICENSE
+-rw-r--r--   0 dej       (1000) dej       (1000)     6011 2024-04-14 20:58:52.216604 pdfsyntax-0.1.0/PKG-INFO
+-rw-r--r--   0 dej       (1000) dej       (1000)     4019 2024-04-14 16:40:39.000000 pdfsyntax-0.1.0/README.md
+drwxr-xr-x   0 dej       (1000) dej       (1000)        0 2024-04-14 20:58:52.205604 pdfsyntax-0.1.0/pdfsyntax/
+-rw-r--r--   0 dej       (1000) dej       (1000)       58 2022-08-09 20:53:21.000000 pdfsyntax-0.1.0/pdfsyntax/__init__.py
+-rw-r--r--   0 dej       (1000) dej       (1000)       32 2022-05-02 17:43:04.000000 pdfsyntax-0.1.0/pdfsyntax/__main__.py
+-rw-r--r--   0 dej       (1000) dej       (1000)     9155 2024-03-17 19:03:38.000000 pdfsyntax-0.1.0/pdfsyntax/api.py
+-rw-r--r--   0 dej       (1000) dej       (1000)    11497 2024-04-14 16:30:54.000000 pdfsyntax-0.1.0/pdfsyntax/cli.py
+-rw-r--r--   0 dej       (1000) dej       (1000)     9185 2023-12-31 21:04:26.000000 pdfsyntax-0.1.0/pdfsyntax/display.py
+-rw-r--r--   0 dej       (1000) dej       (1000)    23271 2024-04-14 15:39:42.000000 pdfsyntax-0.1.0/pdfsyntax/docstruct.py
+-rw-r--r--   0 dej       (1000) dej       (1000)    21565 2024-04-14 09:53:18.000000 pdfsyntax-0.1.0/pdfsyntax/filestruct.py
+-rw-r--r--   0 dej       (1000) dej       (1000)     4131 2024-04-13 21:33:36.000000 pdfsyntax-0.1.0/pdfsyntax/filters.py
+-rw-r--r--   0 dej       (1000) dej       (1000)     4672 2023-12-29 22:30:13.000000 pdfsyntax-0.1.0/pdfsyntax/graphics.py
+-rw-r--r--   0 dej       (1000) dej       (1000)     4561 2023-12-29 22:31:00.000000 pdfsyntax-0.1.0/pdfsyntax/layout.py
+-rw-r--r--   0 dej       (1000) dej       (1000)    16331 2024-04-14 09:54:39.000000 pdfsyntax-0.1.0/pdfsyntax/objects.py
+-rw-r--r--   0 dej       (1000) dej       (1000)     7093 2024-01-14 16:11:22.000000 pdfsyntax-0.1.0/pdfsyntax/text.py
+drwxr-xr-x   0 dej       (1000) dej       (1000)        0 2024-04-14 20:58:52.216604 pdfsyntax-0.1.0/pdfsyntax.egg-info/
+-rw-r--r--   0 dej       (1000) dej       (1000)     6011 2024-04-14 20:58:52.000000 pdfsyntax-0.1.0/pdfsyntax.egg-info/PKG-INFO
+-rw-r--r--   0 dej       (1000) dej       (1000)      622 2024-04-14 20:58:52.000000 pdfsyntax-0.1.0/pdfsyntax.egg-info/SOURCES.txt
+-rw-r--r--   0 dej       (1000) dej       (1000)        1 2024-04-14 20:58:52.000000 pdfsyntax-0.1.0/pdfsyntax.egg-info/dependency_links.txt
+-rw-r--r--   0 dej       (1000) dej       (1000)       10 2024-04-14 20:58:52.000000 pdfsyntax-0.1.0/pdfsyntax.egg-info/top_level.txt
+-rw-r--r--   0 dej       (1000) dej       (1000)      855 2024-04-14 20:46:18.000000 pdfsyntax-0.1.0/pyproject.toml
+-rw-r--r--   0 dej       (1000) dej       (1000)       38 2024-04-14 20:58:52.217604 pdfsyntax-0.1.0/setup.cfg
+drwxr-xr-x   0 dej       (1000) dej       (1000)        0 2024-04-14 20:58:52.215604 pdfsyntax-0.1.0/tests/
+-rw-r--r--   0 dej       (1000) dej       (1000)     1499 2024-01-06 20:43:45.000000 pdfsyntax-0.1.0/tests/test_bdata.py
+-rw-r--r--   0 dej       (1000) dej       (1000)      705 2023-09-10 19:21:38.000000 pdfsyntax-0.1.0/tests/test_dependencies.py
+-rw-r--r--   0 dej       (1000) dej       (1000)     2668 2023-06-29 21:07:04.000000 pdfsyntax-0.1.0/tests/test_parsing.py
+-rw-r--r--   0 dej       (1000) dej       (1000)      303 2022-09-13 20:49:14.000000 pdfsyntax-0.1.0/tests/test_serialization.py
+-rw-r--r--   0 dej       (1000) dej       (1000)      458 2023-09-10 19:21:40.000000 pdfsyntax-0.1.0/tests/test_simplefile.py
+-rw-r--r--   0 dej       (1000) dej       (1000)     1044 2023-04-20 21:04:55.000000 pdfsyntax-0.1.0/tests/test_text.py
+-rw-r--r--   0 dej       (1000) dej       (1000)     2548 2024-03-29 23:39:04.000000 pdfsyntax-0.1.0/tests/test_tokenization.py
+-rw-r--r--   0 dej       (1000) dej       (1000)      359 2023-09-10 19:21:36.000000 pdfsyntax-0.1.0/tests/test_updating.py
+-rw-r--r--   0 dej       (1000) dej       (1000)      980 2024-04-07 15:30:15.000000 pdfsyntax-0.1.0/tests/test_xref.py
```

### Comparing `pdfsyntax-0.0.8/LICENSE` & `pdfsyntax-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfsyntax-0.0.8/PKG-INFO` & `pdfsyntax-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfsyntax
-Version: 0.0.8
+Version: 0.1.0
 Summary: A Python library to inspect and modify the internal structure of a PDF file
 Author-email: "Martin D." <desgeeko@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2024 Martin D. <desgeeko@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,15 +26,15 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/desgeeko/pdfsyntax
 Project-URL: Bug Tracker, https://github.com/desgeeko/pdfsyntax/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -51,14 +51,20 @@
 
 1. CLI: It started as a command-line interface to inspect the internal structure of a PDF file.
 2. API: Now the internal functions are being exposed as a toolkit for PDF read/write operations.
 
 ## Project status
 
 WORK IN PROGRESS! This is ALPHA quality software. The API may change anytime.
+Next on TO-DO list:
+- Cut & append pages
+- Lossless compression
+- More filters
+- Improve text extraction
+- Augment text extraction with layout detection
 
 ## Design
 
 PDFSyntax favors non-destructive edits allowed by the PDF Specification: by default incremental updates are added at the end of the original file.
 
 It is mostly made of simple functions working on built-in types and named tuples. Shallow copying of the Doc object structure performed by pure functions offers some kind of - *experimental* - immutability.
 
@@ -74,15 +80,16 @@
 
 The general form of the CLI usage is:
 
     python3 -m pdfsyntax COMMAND FILE
 
 You can get quick insights on a PDF file with these commands:
 - `overview` outputs text data about the structure and the metadata. 
-- `inspect` outputs static html data that lets you browse the internal structure of the PDF file: the PDF source is pretty-printed and augmented with hyperlinks.
+- `browse` outputs static html data that lets you browse the internal structure of the PDF file: the PDF source is pretty-printed and augmented with hyperlinks.
+- `text` outputs extracted text spatially, as if it was a kind of scan.
 
 ## API overview
 
 Please refer to the [API README](https://github.com/desgeeko/pdfsyntax/blob/main/docs/api.md) for details.
 
 PDFSyntax is mostly made of simple functions. Example:
```

### Comparing `pdfsyntax-0.0.8/README.md` & `pdfsyntax-0.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 
 1. CLI: It started as a command-line interface to inspect the internal structure of a PDF file.
 2. API: Now the internal functions are being exposed as a toolkit for PDF read/write operations.
 
 ## Project status
 
 WORK IN PROGRESS! This is ALPHA quality software. The API may change anytime.
+Next on TO-DO list:
+- Cut & append pages
+- Lossless compression
+- More filters
+- Improve text extraction
+- Augment text extraction with layout detection
 
 ## Design
 
 PDFSyntax favors non-destructive edits allowed by the PDF Specification: by default incremental updates are added at the end of the original file.
 
 It is mostly made of simple functions working on built-in types and named tuples. Shallow copying of the Doc object structure performed by pure functions offers some kind of - *experimental* - immutability.
 
@@ -34,15 +40,16 @@
 
 The general form of the CLI usage is:
 
     python3 -m pdfsyntax COMMAND FILE
 
 You can get quick insights on a PDF file with these commands:
 - `overview` outputs text data about the structure and the metadata. 
-- `inspect` outputs static html data that lets you browse the internal structure of the PDF file: the PDF source is pretty-printed and augmented with hyperlinks.
+- `browse` outputs static html data that lets you browse the internal structure of the PDF file: the PDF source is pretty-printed and augmented with hyperlinks.
+- `text` outputs extracted text spatially, as if it was a kind of scan.
 
 ## API overview
 
 Please refer to the [API README](https://github.com/desgeeko/pdfsyntax/blob/main/docs/api.md) for details.
 
 PDFSyntax is mostly made of simple functions. Example:
```

### Comparing `pdfsyntax-0.0.8/pdfsyntax/api.py` & `pdfsyntax-0.1.0/pdfsyntax/api.py`

 * *Files identical despite different names*

### Comparing `pdfsyntax-0.0.8/pdfsyntax/display.py` & `pdfsyntax-0.1.0/pdfsyntax/display.py`

 * *Files identical despite different names*

### Comparing `pdfsyntax-0.0.8/pdfsyntax/docstruct.py` & `pdfsyntax-0.1.0/pdfsyntax/docstruct.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,29 +90,25 @@
     else:
         container = idx[rev][key]['env_num']
         bdata, a0, _, _ = fdata(idx[rev][container]['abs_pos'],
                                 idx[rev][container]['abs_next'] - idx[rev][container]['abs_pos'])
         i, j, _ = next_token(bdata, a0)
         i, j, _ = next_token(bdata, j)
         i, j, _ = next_token(bdata, j)
-        i, j, _ = next_token(bdata, j)
+        i, j, _ = next_token(bdata, j) #/ObjStm
         text = bdata
-        c_obj = parse_obj(text, i)
-        if container > key:
-            cache += (container-key) * [None]
-        cache[container] = c_obj
-        offset = int(c_obj['entries']['/First'])
-        nb_obj = int(c_obj['entries']['/N'])
-        x_array = parse_obj(b'[' + c_obj['stream'][:offset] + b']')
-        for x in range(nb_obj):
-            if int(x_array[2 * x]) >= len(cache):
-                cache += (int(x_array[2 * x])-len(cache)+1) * [None]
-            cache[int(x_array[2 * x])] = parse_obj(c_obj['stream'], offset + int(x_array[2 * x + 1]))
-        if key == 0 and type(cache[0]) == Stream:
-            cache[0] = cache[0]['entries']
+        stream_obj = parse_obj(text, i)
+        if container >= len(cache):
+            cache += (container-len(cache)+1) * [None]
+        cache[container] = stream_obj
+        _, _, _, obj_list = parse_object_stream(stream_obj, container)
+        for o_num, embedded_obj, _, _, _ in obj_list:
+            if o_num >= len(cache):
+                cache += (o_num-len(cache)+1) * [None]
+            cache[o_num] = embedded_obj
     return cache
 
 
 def get_object(doc: Doc, obj):
     """Return raw object or the target of an indirect reference."""
     if isinstance(obj, complex) == True:
         ref = int(obj.imag)
@@ -124,15 +120,15 @@
 
 def flat_page_tree(doc: Doc, num=None, inherited={}, max_nb=None) -> list:
     """Recursively list the pages of a node."""
     accu = []
     if num:
         node = get_object(doc, num)
     else:
-        node = get_object(doc, catalog(doc)['/Pages'])
+        node = get_object(doc, catalog(doc)[0]['/Pages'])
     if node['/Type'] == '/Pages':
         for kid in node['/Kids']:
             e = {k: node.get(k) for k in INHERITABLE_ATTRS if node.get(k) is not None}
             inherited.update(e)
             accu = accu + flat_page_tree(doc, kid, inherited.copy(), max_nb)
             if max_nb is not None and len(accu) == max_nb:
                 return accu
@@ -145,62 +141,101 @@
     """Initialize cache with trailer."""
     size = len(index[-1])
     cache = size * [None]
     memoize_obj_in_cache(index, fdata, 0, cache)
     return cache
 
 
+def get_iref(doc: Doc, o_num: int, rev: int=-1) -> complex:
+    """Build the relevant indirect reference for o_num in a doc revision."""
+    current = doc.index[rev]
+    o_gen = current[o_num]['o_gen']
+    return complex(o_gen, o_num)
+
+
+def in_use(doc: Doc, rev: int=-1) -> list:
+    """List objects in use (not deleted)."""
+    res = []
+    current = doc.index[rev]
+    for i in range(1, len(current)):
+        iref = get_iref(doc, i, rev)
+        if 'DELETED' not in current[i]:
+            res.append(iref)
+    return res
+
+
 def changes(doc: Doc, rev: int=-1):
     """List deleted/updated/added objects."""
     res = []
     current = doc.index[rev]
     if len(doc.index) == 1:
         previous = [None] * len(current)
     else:
         previous = doc.index[rev-1]
     for i in range(1, len(current)):
+        iref = get_iref(doc, i, rev)
         if i > len(previous)-1:
-            res.append((i, 'a'))
+            res.append((iref, 'a'))
         elif i < len(previous) and previous[i] == current[i]:
             pass
         elif previous[i] != None and 'DELETED' not in previous[i] and 'DELETED' in current[i]:
-            res.append((i, 'd'))
+            res.append((iref, 'd'))
         elif previous[i] != None and current[i] != previous[i]:
-            res.append((i, 'u'))
+            res.append((iref, 'u'))
         else:
-            res.append((i, 'a'))
+            res.append((iref, 'a'))
     return res
 
 
 #def group_obj_into_stream(doc: Doc):
 #    """Provision a ObjStm object and tag all changes to target this envelope."""
 #    doc2, _ = add_object(doc, b'')
 #    current = doc2.index[-1]
 #    o_num = current[-2]['o_num']
 #    chgs = changes(doc)
-#    for i, _ in chgs:
+#    for c, _ in chgs:
+#        i = int(c.imag)
 #        if i == o_num:
 #            continue
 #        current[i]['env_num'] = o_num
 #    d = {'/Type': '/ObjStm', '/Length': 0, '/N': 0, '/First': 0, '/FirstLine': []}
 #    doc2.cache[o_num] = Stream(d, b'', b'')
 #    return doc2
 
 
+def envelope_objects(doc: Doc):
+    """List objects streams that envelope other objects."""
+    return {o.get('env_num') for o in doc.index[-1] if o.get('env_num')}
+
+
 def version(doc: Doc) -> str:
     """Return PDF version."""
     fdata = doc.data[0]['fdata']
     bdata, a0, _, _ = fdata(5, 3)
     ver = bdata[a0:a0+3]
-    cat = catalog(doc)
-    if '/Version' in cat and cat['/Version'] > ver.decode('ascii'):
-            return cat['/Version'].decode('ascii')
+    cat, _ = catalog(doc)
+    if '/Version' in cat and cat['/Version'][1:] > ver.decode('ascii'):
+            return cat['/Version'][1:]
     return ver.decode('ascii')
 
 
+def update_version(doc: Doc, ver: str) -> Doc:
+    """Upgrade PDF version in incremental update."""
+    cat, i_ref = catalog(doc)
+    if '/Version' in cat:
+        if cat['/Version'][1:] < ver:
+            cat['/Version'] = '/' + ver
+            return update_object(doc, int(i_ref.imag), cat)
+        else:
+            return doc
+    else:
+        cat['/Version'] = '/' + ver
+        return update_object(doc, int(i_ref.imag), cat)
+
+
 def updates(doc: Doc) -> int:
     """Return the number of updates the document received."""
     upd = len(doc.index) - 1
     return upd
 
 
 def trailer(doc: Doc):
@@ -224,28 +259,29 @@
         return True
     else:
         return False
 
 
 def catalog(doc: Doc):
     """Return doc Root/Catalog dictionary."""
-    return get_object(doc, trailer(doc)['/Root'])
+    root = trailer(doc)['/Root']
+    return get_object(doc, root), root
 
 
 def info(doc: Doc):
     """Return doc Info dictionary if present."""
     trail = trailer(doc)
     info = trail.get('/Info')
     if info:
         return get_object(doc, info)
 
 
 def number_pages(doc: Doc):
     """Return doc number of pages."""
-    p = get_object(doc, catalog(doc)['/Pages'])
+    p = get_object(doc, catalog(doc)[0]['/Pages'])
     return p['/Count']
 
 
 def pages(doc: Doc, max_nb=None) -> list:
     """List page objects."""
     pl = []
     for num, in_attr in flat_page_tree(doc, max_nb=max_nb):
@@ -319,24 +355,27 @@
     new_v = [new_index0] + [new_doc.index[-1][i] for i in range(1,len(new_doc.index[-1]))] 
     new_doc.index.append(new_v)
     new_trailer = doc.cache[0].copy()
     if type(new_doc.index[-2][0]) == list: #Linearized
         new_trailer['/Prev'] = new_doc.index[-2][1].get('xref_table_pos') or new_doc.index[-2][1].get('xref_stream_pos')
     else:
         new_trailer['/Prev'] = new_doc.index[-2][0].get('xref_table_pos') or new_doc.index[-2][0].get('xref_stream_pos')
+    if '/XRefStm' in new_trailer:
+        del new_trailer['/XRefStm']
     new_doc.cache[0] = new_trailer
     return new_doc
 
 
 def prepare_revision(doc: Doc, rev:int = -1, idx:int = 0) -> tuple:
     """Build bytes representing incremental update."""
     chg = changes(doc, rev)
     if not chg:
         return b''
-    for num, _ in chg:
+    for c, _ in chg:
+        num = int(c.imag)
         memoize_obj_in_cache(doc.index, doc.data[rev]['fdata'], num, doc.cache, rev=-1)
     if version(doc) < '1.5':
         use_xref_stream = False
     else:
         use_xref_stream = True
     fragments, new_index = build_revision_byte_stream(chg, doc.index[rev], doc.cache, idx, use_xref_stream)
     return fragments, new_index
@@ -368,45 +407,88 @@
         new_doc = Doc(doc.index.copy(), len(doc.index[-1]) * [None], doc.data.copy())
         new_doc.data[-1] = new_doc.data[-1].copy()
     else:
         return None
     return new_doc
 
 
-def update_object(doc: Doc, num: int, new_o) -> Doc:
+def update_object(doc: Doc, num: int, new_o, immut=True) -> Doc:
     """Update object in the current revision."""
     ver = len(doc.index)
     old_i = doc.index[-1][num]
     new_i = {
         'o_num': num,
         'o_gen': old_i['o_gen'],
         'o_ver': old_i['o_ver']+1,
         'doc_ver': ver-1,
     }
     if new_o is None:
         new_i['DELETED'] = True
-    new_doc = copy_doc(doc, revision='SAME')
+    if immut:
+        new_doc = copy_doc(doc, revision='SAME')
+    else:
+        new_doc = doc
     new_doc.index[-1][num] = new_i
     new_doc.cache[num] = new_o
     return new_doc
 
 
-def add_object(doc: Doc, new_o) -> tuple:
+def add_object(doc: Doc, new_o, immut=True) -> tuple:
     """Add new object at the end of current index."""
     ver = len(doc.index)
     num = len(doc.index[-1])
     new_i = {'o_num': num, 'o_gen': 0, 'o_ver': 0, 'doc_ver': ver-1}
-    new_doc = copy_doc(doc, revision='SAME')
+    if immut:
+        new_doc = copy_doc(doc, revision='SAME')
+    else:
+        new_doc = doc
     new_doc.index[-1].append(None)
     new_doc.index[-1][num] = new_i
     new_doc.cache.append(None)
     new_doc.cache[num] = new_o
     return new_doc, complex(0, num)
 
 
+def max_num(doc: Doc, rev: int=-1) -> int:
+    """Return the biggest object number in doc revision."""
+    return len(doc.index[rev]) - 1
+
+
+def concatenate_docs(doc1: Doc, doc2: Doc) -> Doc:
+    """Add pages from doc2 at the end of doc1."""
+    mapping = {}
+    new_doc = copy_doc(doc1, revision='SAME')
+    start_num = max_num(new_doc) + 1
+    cat, cat_iref = catalog(new_doc)
+    doc2 = squash(doc2)
+    cat2, cat_iref2 = catalog(doc2)
+    pages_iref2 = cat2['/Pages']
+    pages2 = get_object(doc2, pages_iref2)
+    pcount2 = get_object(doc2, pages2['/Count'])
+    doc2 = update_object(doc2, int(cat_iref2.imag), None) #TODO: remove xref stream
+    objs = in_use(doc2)
+    ir = complex(0, start_num)
+    for iref in objs:
+        mapping[iref] = ir
+        ir += 1j
+    for iref in objs:
+        obj = get_object(doc2, iref)
+        new_obj = deep_ref_retarget(obj, mapping)
+        new_doc, _ = add_object(new_doc, new_obj, immut=False)
+    pages_iref = cat['/Pages']
+    pages = get_object(new_doc, pages_iref)
+    pcount = get_object(new_doc, pages['/Count'])
+    kids = get_object(new_doc, pages['/Kids'])
+    kids.append(mapping[pages_iref2])
+    pages['/Kids'] = kids
+    pages['/Count'] = pcount + pcount2
+    new_doc = update_object(new_doc, int(pages_iref.imag), pages, immut=False)
+    return new_doc
+
+
 def dependencies(doc: Doc, obj: Any) -> set:
     """Recursively list indirect references found inside object.""" 
     if type(obj) == dict:
         res = set()
         for k, v in obj.items():
             if k == '/Parent' or k == '/P':
                 continue
@@ -423,65 +505,78 @@
         return res
     else:   
         return set()
 
 
 def delete_pages(doc: Doc, del_pages) -> Doc:
     """Delete one (an int) or more (an array of int) pages."""
+    new_doc = copy_doc(doc, revision='SAME')
     if type(del_pages) != list:
         del_pages = [del_pages]
-    pages = flat_page_tree(doc)
+    pages = flat_page_tree(new_doc)
     del_ref = {pages[p][0] for p in del_pages}
     keep_ref = {p[0] for p in pages} - del_ref
     del_dep = set()
     keep_dep = set()
     for i in del_ref:
-        del_dep = del_dep | dependencies(doc, i)
+        del_dep = del_dep | dependencies(new_doc, i)
     for i in keep_ref:
-        keep_dep = keep_dep | dependencies(doc, i)
+        keep_dep = keep_dep | dependencies(new_doc, i)
     for ref in del_ref:
-        parent = get_object(doc, ref)['/Parent']
-        new_parent = get_object(doc, parent)
+        parent = get_object(new_doc, ref)['/Parent']
+        new_parent = get_object(new_doc, parent)
         kids = new_parent['/Kids']
         kids.remove(ref)
         new_parent['/Count'] = new_parent['/Count'] - 1
-        doc = update_object(doc, int(parent.imag), new_parent)
+        new_doc = update_object(new_doc, int(parent.imag), new_parent, immut=False)
         while '/Parent' in new_parent:
             p = new_parent['/Parent']
-            new_parent = get_object(doc, p)
+            new_parent = get_object(new_doc, p)
             new_parent['/Count'] = new_parent['/Count'] - 1
-            doc = update_object(doc, int(p.imag), new_parent)
+            new_doc = update_object(new_doc, int(p.imag), new_parent, immut=False)
     for ref in del_dep - keep_dep:
-        doc = update_object(doc, int(ref.imag), None)
-    return doc
+        new_doc = update_object(new_doc, int(ref.imag), None, immut=False)
+    return new_doc
+
+
+#def detect_unused(doc: Doc) -> dict:
+#    """ WORK IN PROGRESS """
+#    current_index = doc.index[-1]
+#    for i in range(1, len(current_index)):
+#        ref = complex(current_index[i]['o_ver'], current_index[i]['o_num'])
+#        obj = get_object(doc, ref)
+#        refs = deep_ref_detect(obj, set())
+#    return
 
 
-def defragment_map(current_index: list) -> tuple:
+def defragment_map(current_index: list, excluded={}) -> tuple:
     """Build new index without empty slots (ie deleted objects)."""
     new_index = [None]
     mapping = {}
     nb = 0
     for i, o in enumerate(current_index):
         if i == 0: #trailer
             continue
-        if 'DELETED' in o:
+        if 'DELETED' in o or i in excluded:
             continue
         else:
             nb += 1
             old_ref = complex(o['o_gen'], o['o_num']) 
             new_index.append({'o_num': nb, 'o_gen': 0, 'o_ver': 0, 'doc_ver': 0, 'OLD_REF': old_ref})
             new_ref = complex(0, nb) 
             if old_ref != new_ref:
                 mapping[old_ref] = new_ref
     return new_index, mapping
 
 
 def squash(doc: Doc) -> Doc:
-    """Group all revisions into a single one"""
-    new_index, mapping = defragment_map(doc.index[-1])
+    """Group all revisions into a single one."""
+    obj_stms = envelope_objects(doc)
+    old_index = doc.index[-1]
+    new_index, mapping = defragment_map(old_index, obj_stms)
     if new_index[0] is None:
         new_index[0] = {}
     new_cache = len(new_index) * [None]
     new_data = [{}]
     new_cache[0] = trailer(doc)
     for i in range(1, len(new_index)):
         old_ref = new_index[i]['OLD_REF']
@@ -503,14 +598,15 @@
     new_bdata, new_i = build_revision_byte_stream(chg,
                                                new_doc.index[0],
                                                new_doc.cache,
                                                len(header),
                                                use_xref_stream)
     new_data[-1]['fdata'] = bdata_dummy(header + new_bdata)
     new_doc.index[0] = new_i
+    new_doc = commit(new_doc) #TODO: keep?
     return new_doc
 
 
 def prepare_w(w, default_w):
     """Decode widths for type0 / CID fonts."""
     i = 0
     width = {}
```

### Comparing `pdfsyntax-0.0.8/pdfsyntax/filestruct.py` & `pdfsyntax-0.1.0/pdfsyntax/filestruct.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Module pdfsyntax.filestruct: how objects are stored in a PDF file"""
 
 from typing import Callable
 from typing import IO
 from .objects import *
 import os
+import math
 from copy import deepcopy
 from .filters import *
 
 MARGIN = b'\n'
 
 
 def bdata_provider(data_source, mode: str = "SINGLE"):
@@ -78,38 +79,87 @@
 
 def bdata_all(bdata: Callable) -> bytes:
     """Return full bdata content as bytes."""
     bdata, _, _, _ = bdata(0, -1)
     return bdata
 
 
+def file_object_map(fdata: Callable) -> list:
+    """Parse whole file in sequential order without using xref."""
+    sections = []
+    bdata, _, _, length = fdata(0, -1) #Read all
+    i = 0
+    j = 0
+    while i < length:
+        mo = parse_region(bdata, i)
+        if mo is None:
+            break
+        bo, eo, t, content = mo
+        sections.append(mo)
+        if t == 'XREFTABLE':
+            table = content['table']
+            subsection = -1
+            for a in table:
+                if len(a) == 2:
+                    subsection += 1
+                    ln = 0
+                    continue
+                index, i_num, i_gen, s = a
+                a_pos = subsection, ln
+                s = (a_pos, None, 'XREF', ('XREF_T', index, i_num, i_gen, s))
+                sections.append(s)
+                ln += 1
+        elif t == 'IND_OBJ' and type(content['obj']) == Stream:
+            if content['obj']['entries'].get('/Type') == '/XRef':
+                _, _, typ, obj = parse_xref_stream_raw(content['obj'])
+                table = obj['table']
+                current_sub = -1
+                for index, env_num, i_num, i_gen, s, raw_line, subsection in table:
+                    if subsection != current_sub:
+                        ln = -1
+                        current_sub = subsection
+                    ln += 1
+                    a_pos = subsection, ln
+                    s = (a_pos, None, 'XREF', ('XREF_S', index, i_num, i_gen, s, env_num, raw_line))
+                    sections.append(s)
+            elif content['obj']['entries'].get('/Type') == '/ObjStm':
+                _, _, typ, obj = parse_object_stream(content['obj'], content['o_num'])
+                for embedded in obj:
+                    i_num, obj, env_num, theorical_pos, actual_pos = embedded
+                    if theorical_pos:
+                        a_pos = j, actual_pos
+                        j += 1
+                    else:
+                        a_pos = -1, actual_pos
+                    s = (a_pos, None, 'IND_OBJ', {'o_num':i_num, 'o_gen':None, 'obj':obj, 'env_num':env_num})
+                    sections.append(s)
+        i = eo
+    return sections
+
+
 def parse_xref_table(bdata: bytes, start_pos: int, general_offset: int) -> list:
     """Return a list of dicts indexing indirect objects.
 
     - abs_pos is the absolute position of the object
     - o_num is the object number
     - o_gen is the object generation number
     """
     xref = []
     table = []
+    _, _, _, xref_table = parse_xref_table_raw(bdata, start_pos)
+    lines = xref_table['table']
     trailer_pos = bdata.find(b'trailer', start_pos)
-    lines = bdata[start_pos:trailer_pos].splitlines()
     for line in lines:
-        line_a = line.strip(b'\n\r ').split()
-        l = len(line_a)
-        if  l == 2:
-            o_num = int(line_a[0])
-            table.append((line, None))
-        elif l == 3:
-            offset = int(line_a[0])
-            o_ver = int(line_a[1])
-            keyword = line_a[2]
+        if len(line) == 2:
+            table.append((f"{line[0]} {line[1]}".encode('ascii'), None))
+        elif len(line) == 4:
+            offset, o_num, o_gen, keyword = line
             if keyword != b'f' and o_num != 0:
-                xref.append({'abs_pos': offset, 'o_num': o_num, 'o_gen': o_ver})
-            table.append((line, o_num))
+                xref.append({'abs_pos': offset, 'o_num': o_num, 'o_gen': o_gen})
+            table.append((f"{offset:010d} {o_gen:05d} {keyword.decode('ascii')} ".encode('ascii'), o_num))
             o_num += 1
     trailer = {
         'o_num': 0,
         'o_gen': 0,
         'abs_pos': general_offset + trailer_pos,
         'xref_table_pos':general_offset + start_pos,
         'xref_table':table,
@@ -127,50 +177,43 @@
     - o_gen is the object generation number
     for objects embedded in object streams:
     - env_num is the number of the envelope object
     - o_num is the object number
     - o_gen is the object generation number
     - o_pos is the position of the object within the stream
     """
+    xref_stream_num = o_num
     xref = []
     table = []
-    cols = xref_stream['entries']['/W']
-    i = 0
-    if '/Index' in xref_stream['entries']:
-        obj_range = xref_stream['entries']['/Index']
-    else:
-        obj_range = [0, xref_stream['entries']['/Size']]
-    start_obj, nb_obj = int(obj_range[0]), int(obj_range[1])
-    obj_num = start_obj
-    while i < len(xref_stream['stream']):
-        params = []
-        ppr = b''
-        for col in cols:
-            x = xref_stream['stream'][i:i+int(col)]
-            #struct.unpack cannot work with 3-byte words
-            params.append(int.from_bytes(x, byteorder='big'))
-            i += int(col)
-            ppr += asciihex(x) + b' '
-        table.append((ppr, obj_num))
-        if params[0] == 1:
-            xref.append({'abs_pos': params[1], 'o_num': obj_num, 'o_gen': params[2]})
-        elif params[0] == 2:
-            xref.append({'env_num': params[1], 'o_num': obj_num, 'o_gen': 0, 'o_pos': params[2]})
-        obj_num += 1
+    _, _, _, xref_table = parse_xref_stream_raw(xref_stream)
+    lines = xref_table['table']
+    for line in lines:
+        offset, env_iref, o_num, o_gen, keyword, raw_line, _ = line
+        if o_num == 0:
+            table.append((raw_line, o_num))
+            continue
+        if keyword == b'f':
+            continue
+        if env_iref:
+            xref.append({'o_pos': offset, 'env_num':env_iref, 'o_num': o_num, 'o_gen': o_gen})
+        else:
+            xref.append({'abs_pos': offset, 'o_num': o_num, 'o_gen': o_gen})
+        table.append((raw_line, o_num))
+        o_num += 1
     trailer = {
         'o_num': 0,
         'o_gen': 0,
         'abs_pos': trailer_pos,
         'xref_stream_pos': trailer_pos,
         'xref_stream': table,
-        'xref_stream_num': o_num,
+        'xref_stream_num': xref_stream_num,
     }
     xref.insert(0, trailer)
     return xref
-    
+
 
 def build_chrono_from_xref(fdata: Callable) -> list:
     """Return a merged list of all entries sequentially found in xref tables or xref streams.
 
     Chrono means that the sequence goes from the oldest (first revision)
     to the newest (last revision) entries.
     An xref+trailer or an /Xref is seen as a virtual object #0
@@ -325,19 +368,21 @@
     return i
 
 
 def circular_deleted(changes: list) -> dict:
     """Build lookup dict to ref of next deleted object."""
     res = {}
     deleted = [x for x in changes if x[1] == 'd']
-    for i, d in enumerate([(0, 'd')] + deleted):
+    for i, d in enumerate([(0j, 'd')] + deleted):
+        e = int(d[0].imag)
         if i == len(deleted):
-            res[d[0]] = 0
+            res[e] = 0
         else:
-            res[d[0]] = deleted[i][0]
+            t = deleted[i][0]
+            res[e] = int(t.imag)
     return res
 
 
 def format_xref_table(elems: list, trailer: dict, next_free: dict) -> bytes:
     """Build XREF table."""
     xref_table = []
     for use, num, o_gen, counter, _ in elems:
@@ -377,25 +422,27 @@
     """Build XREF stream object."""
     xref_stream = []
     index = []
     o_num = trailer['/Size'] - 1
     trailer['/Type'] = '/XRef'
     trailer['/Length'] = -1
     trailer['/Filter'] = '/ASCIIHexDecode'
-    trailer['/W'] = [1, 3, 3]
+    max_counter = max([e[3] for e in elems if e[3] is not None])
+    b = (int(math.log2(max_counter+1)) // 8) + 1
+    trailer['/W'] = [1, b, b]
     for use, num, o_gen, counter, env_num in elems:
         if use == 'f':
-            ref = b'\x00' + (next_free[num]).to_bytes(3, "big") + (o_gen+1).to_bytes(3, "big")
+            ref = b'\x00' + (next_free[num]).to_bytes(b, "big") + (o_gen+1).to_bytes(b, "big")
             xref_stream.append((ref, num))
         else:
             if env_num:
-                ref = b'\x02' + (env_num).to_bytes(3, "big") + (counter).to_bytes(3, "big")
+                ref = b'\x02' + (env_num).to_bytes(b, "big") + (counter).to_bytes(b, "big")
                 xref_stream.append((ref, num))
             else:
-                ref = b'\x01' + (counter).to_bytes(3, "big") + (o_gen).to_bytes(3, "big")
+                ref = b'\x01' + (counter).to_bytes(b, "big") + (o_gen).to_bytes(b, "big")
                 xref_stream.append((ref, num))
     # Index 
     i = len(xref_stream) - 1
     num = xref_stream[i][1]
     nb = 1
     while i >= 1:
         i -= 1
@@ -406,17 +453,14 @@
             nb = 1
         num = xref_stream[i][1]
     index = [num, nb] + index
     trailer['/Index'] = index
     st = b''
     for x, _ in xref_stream:
         st += x
-    #encoded = encode_stream(st, trailer)
-    #s = Stream(trailer, st, encoded)
-    #update_internal_stream_length(s)
     s, _ = forge_stream(trailer, st)
     ser0 = serialize(s)
     build_xref_stream = b''
     build_xref_stream += f'{o_num}'.encode('ascii')
     build_xref_stream += b' 0 obj\n'
     build_xref_stream += ser0 
     build_xref_stream += b'\n'
@@ -463,17 +507,14 @@
         header += f'{i} '.encode('ascii')
     header += b'\n'
     entries['/First'] = len(header)
     entries['/N'] = len(tokens) // 2
     del entries['/FirstLine']
     entries['/Length'] = -1
     new_ser = header + envelope['stream']
-    #encoded = encode_stream(new_ser, entries)
-    #envelope = Stream(entries, new_ser, encoded)
-    #update_internal_stream_length(envelope)
     envelope, _ = forge_stream(entries, new_ser)
     return envelope
 
 
 def build_revision_byte_stream(
         changes: list, current_index: list, cache: list,
         starting_pos: int, use_xref_stream: bool) -> tuple:
@@ -481,15 +522,16 @@
     fragments = []
     xref_table = []
     res = b''
     new_index = deepcopy(current_index)
     counter = starting_pos + len(MARGIN)
     fragments.append(MARGIN)
     next_free = circular_deleted(changes)
-    for num, action in ([(0, 'd')] + changes):
+    for c, action in ([(0j, 'd')] + changes):
+        num = int(c.imag)
         env_num = None
         if action == 'd':
             if num == 0:
                 o_gen = 65535 - 1
             else:
                 o_gen = current_index[num]['o_gen']
             xref_table.append(('f', num, o_gen, None, None))
@@ -507,21 +549,23 @@
                     obj = finalize_stream(obj)
                 block = serialize_fragment(num, o_gen, obj)
                 fragments.append(block)
                 xref_table.append(('n', num, o_gen, counter, env_num))
                 new_index[num]['abs_pos'] = counter
                 new_index[num]['abs_next'] = counter + len(block)
             counter += len(block)
-    cache[0]['/Size'] = len(current_index)
     if not use_xref_stream:
+        cache[0]['/Size'] = len(current_index)
         built_xref = format_xref_table(xref_table, cache[0], next_free)
         new_index[0]['xref_table_pos'] = counter
         new_index[0]['abs_pos'] = starting_pos + built_xref.rfind(b'trailer')
         new_index[0]['abs_next'] = starting_pos + len(built_xref)
     else:
+        cache[0]['/Size'] = len(current_index) + 1
+        xref_table.append(('n', len(current_index), 0, counter, None))
         built_xref = format_xref_stream(xref_table, cache[0], next_free)
         new_index[0]['xref_stream_pos'] = counter
         new_index[0]['abs_pos'] = starting_pos
         new_index[0]['abs_next'] = starting_pos + len(built_xref)
     fragments.append(built_xref)
     fragments.append(f'startxref\n{counter}\n'.encode('ascii'))
     fragments.append(b'%%EOF\n')
```

### Comparing `pdfsyntax-0.0.8/pdfsyntax/filters.py` & `pdfsyntax-0.1.0/pdfsyntax/filters.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,72 +20,98 @@
         res += bytes(decoded_row[1:])
         i += columns
     return res
 
 
 def decode_stream(stream, stream_def):
     """Apply all specified filters in order to decode stream."""
+#    b1 = b'stream' + b'\r\n'
+#    b2 = b'stream' + b'\n'
+#    e1 = b'\r\n' + b'endstream'
+#    e2 = b'\n' + b'endstream'
+#    e3 = b'\r' + b'endstream'
+#    if stream[:len(b1)] == b1:
+#        b = len(b1)
+#    elif stream[:len(b2)] == b2:
+#        b = len(b2)
+#    else:
+#        return None
+#    if stream[-len(e1):] == e1:
+#        e = len(e1)
+#    elif stream[-len(e2):] == e2:
+#        e = len(e2)
+#    elif stream[-len(e3):] == e3:
+#        e = len(e3)
+#    else:
+#        return None
+#    s = stream[b:-e]
+    s = stream
     if '/Filter' not in stream_def:
-        return stream
+        return s
     filters = stream_def['/Filter']
     if type(filters) == str:
         filters = [filters]
     if '/DecodeParms' not in stream_def:
         parms = [None] * len(filters)
     else:
         parms = stream_def['/DecodeParms']
-        if type(parms) == str:
+        if type(parms) == dict:
             parms = [parms]
-    res = stream
+    #res = s
     for i, f in enumerate(filters):
         if f == '/FlateDecode':
             try:
-                res = zlib.decompress(res)
+                res = zlib.decompress(s)
                 if parms[i] and '/Predictor' in parms[i]:
                     predictor = int(parms[i]['/Predictor'])
                     columns = int(parms[i]['/Columns'])
                     res = decode_predictor(res, predictor, columns)
             except:
                 return b'#PDFSyntaxException: cannot decode Flate'
         elif f == '/ASCIIHexDecode':
             try:
-                res = binascii.unhexlify(res)
+                res = binascii.unhexlify(s)
             except:
                 return b'#PDFSyntaxException: cannot decode ASCIIHex'
         elif f == '/ASCII85Decode':
             try:
-                res = base64.a85decode(res, adobe=True)
+                res = base64.a85decode(s, adobe=True)
             except:
                 return b'#PDFSyntaxException: cannot decode ASCII85'
         else:
             return b'#PDFSyntaxException: unsupported filter'
     return res
 
 
 def encode_stream(stream, stream_def):
     """Apply all specified filters in order to encode stream."""
+    #b = b'stream\n'
+    #e = b'\nendstream'
     if '/Filter' not in stream_def:
         return stream
     filters = stream_def['/Filter']
     if type(filters) == str:
         filters = [filters]
     res = stream
     for _, f in enumerate(filters):
         if f == '/FlateDecode':
             try:
+                #res = b + zlib.compress(res) + e
                 res = zlib.compress(res)
             except:
                 return b'#PDFSyntaxException: cannot encode Flate'
         elif f == '/ASCIIHexDecode':
             try:
+                #res = b + asciihex(res) + e
                 res = asciihex(res)
             except:
                 return b'#PDFSyntaxException: cannot encode ASCIIHex'
         elif f == '/ASCII85Decode':
             try:
+                #res = b + base64.a85encode(res, adobe=True) + e
                 res = base64.a85encode(res, adobe=True)
             except:
                 return b'#PDFSyntaxException: cannot encode ASCII85'
         else:
             return b'#PDFSyntaxException: unsupported filter'
     return res
```

### Comparing `pdfsyntax-0.0.8/pdfsyntax/graphics.py` & `pdfsyntax-0.1.0/pdfsyntax/graphics.py`

 * *Files identical despite different names*

### Comparing `pdfsyntax-0.0.8/pdfsyntax/layout.py` & `pdfsyntax-0.1.0/pdfsyntax/layout.py`

 * *Files identical despite different names*

### Comparing `pdfsyntax-0.0.8/pdfsyntax/text.py` & `pdfsyntax-0.1.0/pdfsyntax/text.py`

 * *Files identical despite different names*

### Comparing `pdfsyntax-0.0.8/pdfsyntax.egg-info/PKG-INFO` & `pdfsyntax-0.1.0/pdfsyntax.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfsyntax
-Version: 0.0.8
+Version: 0.1.0
 Summary: A Python library to inspect and modify the internal structure of a PDF file
 Author-email: "Martin D." <desgeeko@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2024 Martin D. <desgeeko@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,15 +26,15 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/desgeeko/pdfsyntax
 Project-URL: Bug Tracker, https://github.com/desgeeko/pdfsyntax/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -51,14 +51,20 @@
 
 1. CLI: It started as a command-line interface to inspect the internal structure of a PDF file.
 2. API: Now the internal functions are being exposed as a toolkit for PDF read/write operations.
 
 ## Project status
 
 WORK IN PROGRESS! This is ALPHA quality software. The API may change anytime.
+Next on TO-DO list:
+- Cut & append pages
+- Lossless compression
+- More filters
+- Improve text extraction
+- Augment text extraction with layout detection
 
 ## Design
 
 PDFSyntax favors non-destructive edits allowed by the PDF Specification: by default incremental updates are added at the end of the original file.
 
 It is mostly made of simple functions working on built-in types and named tuples. Shallow copying of the Doc object structure performed by pure functions offers some kind of - *experimental* - immutability.
 
@@ -74,15 +80,16 @@
 
 The general form of the CLI usage is:
 
     python3 -m pdfsyntax COMMAND FILE
 
 You can get quick insights on a PDF file with these commands:
 - `overview` outputs text data about the structure and the metadata. 
-- `inspect` outputs static html data that lets you browse the internal structure of the PDF file: the PDF source is pretty-printed and augmented with hyperlinks.
+- `browse` outputs static html data that lets you browse the internal structure of the PDF file: the PDF source is pretty-printed and augmented with hyperlinks.
+- `text` outputs extracted text spatially, as if it was a kind of scan.
 
 ## API overview
 
 Please refer to the [API README](https://github.com/desgeeko/pdfsyntax/blob/main/docs/api.md) for details.
 
 PDFSyntax is mostly made of simple functions. Example:
```

### Comparing `pdfsyntax-0.0.8/pdfsyntax.egg-info/SOURCES.txt` & `pdfsyntax-0.1.0/pdfsyntax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdfsyntax-0.0.8/pyproject.toml` & `pdfsyntax-0.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 requires = [
     "setuptools>=61.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pdfsyntax"
-version = "0.0.8"
+version = "0.1.0"
 authors = [ 
     { name="Martin D.", email="desgeeko@gmail.com" } 
 ]
 description = "A Python library to inspect and modify the internal structure of a PDF file"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries",
     "Topic :: Utilities"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/desgeeko/pdfsyntax"
```

### Comparing `pdfsyntax-0.0.8/tests/test_bdata.py` & `pdfsyntax-0.1.0/tests/test_bdata.py`

 * *Files identical despite different names*

### Comparing `pdfsyntax-0.0.8/tests/test_dependencies.py` & `pdfsyntax-0.1.0/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `pdfsyntax-0.0.8/tests/test_parsing.py` & `pdfsyntax-0.1.0/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `pdfsyntax-0.0.8/tests/test_text.py` & `pdfsyntax-0.1.0/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `pdfsyntax-0.0.8/tests/test_tokenization.py` & `pdfsyntax-0.1.0/tests/test_tokenization.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,11 +58,17 @@
     def test_dictionary2(self):
         self.assertEqual(pdf.next_token(b'<< /Type /abc >>'), (0, 16, 'DICT'))
 
     def test_dictionary3(self):
         self.assertEqual(pdf.next_token(b'<</Type/abc>>'), (0, 13, 'DICT'))
 
     def test_stream(self):
-        self.assertEqual(pdf.next_token(b'stream\n xyz \nendstream '), (7, 12, 'STREAM'))
+        self.assertEqual(pdf.next_token(b'stream\n xyz \nendstream '), (0, 22, 'STREAM'))
 
     def test_comment(self):
         self.assertEqual(pdf.next_token(b' %something\n '), (1, 11, 'COMMENT'))
+
+    def test_line(self):
+        self.assertEqual(pdf.next_line(b'\n\rabc\n\rdef\n\r'), (2, 5))
+
+    def test_line2(self):
+        self.assertEqual(pdf.next_line(b'\n\rabc\n\rdef\n\r', 6), (7, 10))
```

