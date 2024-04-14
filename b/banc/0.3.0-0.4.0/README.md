# Comparing `tmp/banc-0.3.0.tar.gz` & `tmp/banc-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/banc-0.3.0.tar", last modified: Tue Mar  5 22:07:22 2024, max compression
+gzip compressed data, was "dist/banc-0.4.0.tar", last modified: Sun Apr 14 16:15:27 2024, max compression
```

## Comparing `banc-0.3.0.tar` & `banc-0.4.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 jasper     (501) staff       (20)        0 2024-03-05 22:07:22.000000 banc-0.3.0/
--rw-rw-r--   0 jasper     (501) staff       (20)    35149 2023-08-04 20:01:20.000000 banc-0.3.0/LICENSE
--rw-rw-r--   0 jasper     (501) staff       (20)       75 2023-10-29 23:27:46.000000 banc-0.3.0/MANIFEST.in
--rw-rw-r--   0 jasper     (501) staff       (20)     6741 2024-03-05 22:07:22.000000 banc-0.3.0/PKG-INFO
--rw-rw-r--   0 jasper     (501) staff       (20)     5510 2024-03-05 22:02:03.000000 banc-0.3.0/README.md
-drwxrwxr-x   0 jasper     (501) staff       (20)        0 2024-03-05 22:07:22.000000 banc-0.3.0/banc/
--rw-rw-r--   0 jasper     (501) staff       (20)      329 2023-10-29 23:27:21.000000 banc-0.3.0/banc/__init__.py
--rw-rw-r--   0 jasper     (501) staff       (20)    21373 2024-02-25 23:47:22.000000 banc-0.3.0/banc/annotations.py
--rw-rw-r--   0 jasper     (501) staff       (20)     2164 2023-10-29 23:27:21.000000 banc-0.3.0/banc/auth.py
--rw-rw-r--   0 jasper     (501) staff       (20)     4410 2023-08-04 20:01:20.000000 banc-0.3.0/banc/connectivity.py
--rw-rw-r--   0 jasper     (501) staff       (20)    42132 2024-02-25 23:50:38.000000 banc-0.3.0/banc/lookup.py
--rw-rw-r--   0 jasper     (501) staff       (20)     2718 2023-11-16 21:58:08.000000 banc-0.3.0/banc/ngl_info.py
--rw-rw-r--   0 jasper     (501) staff       (20)    11937 2024-02-25 23:47:22.000000 banc-0.3.0/banc/publish.py
--rw-rw-r--   0 jasper     (501) staff       (20)     3258 2023-08-04 20:01:20.000000 banc-0.3.0/banc/render_neurons.py
--rw-rw-r--   0 jasper     (501) staff       (20)     8001 2023-08-04 20:01:20.000000 banc-0.3.0/banc/skeletonize.py
--rw-rw-r--   0 jasper     (501) staff       (20)    12355 2023-11-12 16:26:17.000000 banc-0.3.0/banc/statebuilder.py
--rw-rw-r--   0 jasper     (501) staff       (20)     1554 2023-08-04 20:01:20.000000 banc-0.3.0/banc/statemanager.py
--rw-rw-r--   0 jasper     (501) staff       (20)    10441 2024-02-25 23:50:38.000000 banc-0.3.0/banc/synaptic_links.py
--rw-rw-r--   0 jasper     (501) staff       (20)     3287 2023-08-04 20:01:20.000000 banc-0.3.0/banc/template_spaces.py
-drwxrwxr-x   0 jasper     (501) staff       (20)        0 2024-03-05 22:07:22.000000 banc-0.3.0/banc/transforms/
--rw-rw-r--   0 jasper     (501) staff       (20)       83 2023-08-04 20:01:20.000000 banc-0.3.0/banc/transforms/__init__.py
--rw-rw-r--   0 jasper     (501) staff       (20)    10088 2024-01-27 15:38:21.000000 banc-0.3.0/banc/transforms/realignment.py
--rw-rw-r--   0 jasper     (501) staff       (20)    15072 2023-08-04 20:01:20.000000 banc-0.3.0/banc/transforms/template_alignment.py
--rw-rw-r--   0 jasper     (501) staff       (20)    34205 2024-02-25 23:50:38.000000 banc-0.3.0/banc/upload.py
--rw-rw-r--   0 jasper     (501) staff       (20)    12518 2023-08-04 20:01:20.000000 banc-0.3.0/banc/visualize.py
-drwxrwxr-x   0 jasper     (501) staff       (20)        0 2024-03-05 22:07:22.000000 banc-0.3.0/banc.egg-info/
--rw-rw-r--   0 jasper     (501) staff       (20)     6741 2024-03-05 22:07:22.000000 banc-0.3.0/banc.egg-info/PKG-INFO
--rw-rw-r--   0 jasper     (501) staff       (20)      575 2024-03-05 22:07:22.000000 banc-0.3.0/banc.egg-info/SOURCES.txt
--rw-rw-r--   0 jasper     (501) staff       (20)        1 2024-03-05 22:07:22.000000 banc-0.3.0/banc.egg-info/dependency_links.txt
--rw-rw-r--   0 jasper     (501) staff       (20)      219 2024-03-05 22:07:22.000000 banc-0.3.0/banc.egg-info/requires.txt
--rw-rw-r--   0 jasper     (501) staff       (20)        5 2024-03-05 22:07:22.000000 banc-0.3.0/banc.egg-info/top_level.txt
--rw-rw-r--   0 jasper     (501) staff       (20)      219 2023-08-04 20:01:20.000000 banc-0.3.0/requirements.txt
--rw-rw-r--   0 jasper     (501) staff       (20)       38 2024-03-05 22:07:22.000000 banc-0.3.0/setup.cfg
--rw-rw-r--   0 jasper     (501) staff       (20)     1026 2024-03-05 22:05:29.000000 banc-0.3.0/setup.py
+drwxrwxr-x   0 jasper     (501) staff       (20)        0 2024-04-14 16:15:27.000000 banc-0.4.0/
+-rw-rw-r--   0 jasper     (501) staff       (20)    35149 2023-08-04 20:01:20.000000 banc-0.4.0/LICENSE
+-rw-rw-r--   0 jasper     (501) staff       (20)       75 2023-10-29 23:27:46.000000 banc-0.4.0/MANIFEST.in
+-rw-rw-r--   0 jasper     (501) staff       (20)     6741 2024-04-14 16:15:27.000000 banc-0.4.0/PKG-INFO
+-rw-rw-r--   0 jasper     (501) staff       (20)     5510 2024-03-05 22:02:03.000000 banc-0.4.0/README.md
+drwxrwxr-x   0 jasper     (501) staff       (20)        0 2024-04-14 16:15:27.000000 banc-0.4.0/banc/
+-rw-rw-r--   0 jasper     (501) staff       (20)      329 2024-03-30 18:16:01.000000 banc-0.4.0/banc/__init__.py
+-rw-rw-r--   0 jasper     (501) staff       (20)    23288 2024-04-07 19:35:06.000000 banc-0.4.0/banc/annotations.py
+-rw-rw-r--   0 jasper     (501) staff       (20)     3244 2024-04-05 12:56:17.000000 banc-0.4.0/banc/auth.py
+-rw-rw-r--   0 jasper     (501) staff       (20)     4410 2023-08-04 20:01:20.000000 banc-0.4.0/banc/connectivity.py
+-rw-rw-r--   0 jasper     (501) staff       (20)    43729 2024-04-14 16:14:02.000000 banc-0.4.0/banc/lookup.py
+-rw-rw-r--   0 jasper     (501) staff       (20)     2916 2024-03-18 21:24:24.000000 banc-0.4.0/banc/ngl_info.py
+-rw-rw-r--   0 jasper     (501) staff       (20)    11937 2024-02-25 23:47:22.000000 banc-0.4.0/banc/publish.py
+-rw-rw-r--   0 jasper     (501) staff       (20)     3258 2023-08-04 20:01:20.000000 banc-0.4.0/banc/render_neurons.py
+-rw-rw-r--   0 jasper     (501) staff       (20)     8001 2023-08-04 20:01:20.000000 banc-0.4.0/banc/skeletonize.py
+-rw-rw-r--   0 jasper     (501) staff       (20)    12689 2024-03-09 15:43:34.000000 banc-0.4.0/banc/statebuilder.py
+-rw-rw-r--   0 jasper     (501) staff       (20)     1554 2023-08-04 20:01:20.000000 banc-0.4.0/banc/statemanager.py
+-rw-rw-r--   0 jasper     (501) staff       (20)    10441 2024-04-14 16:14:02.000000 banc-0.4.0/banc/synaptic_links.py
+-rw-rw-r--   0 jasper     (501) staff       (20)     3287 2023-08-04 20:01:20.000000 banc-0.4.0/banc/template_spaces.py
+drwxrwxr-x   0 jasper     (501) staff       (20)        0 2024-04-14 16:15:27.000000 banc-0.4.0/banc/transforms/
+-rw-rw-r--   0 jasper     (501) staff       (20)       83 2023-08-04 20:01:20.000000 banc-0.4.0/banc/transforms/__init__.py
+-rw-rw-r--   0 jasper     (501) staff       (20)    10088 2024-01-27 15:38:21.000000 banc-0.4.0/banc/transforms/realignment.py
+-rw-rw-r--   0 jasper     (501) staff       (20)    15072 2023-08-04 20:01:20.000000 banc-0.4.0/banc/transforms/template_alignment.py
+-rw-rw-r--   0 jasper     (501) staff       (20)    35619 2024-04-14 16:14:02.000000 banc-0.4.0/banc/upload.py
+-rw-rw-r--   0 jasper     (501) staff       (20)    12518 2023-08-04 20:01:20.000000 banc-0.4.0/banc/visualize.py
+drwxrwxr-x   0 jasper     (501) staff       (20)        0 2024-04-14 16:15:27.000000 banc-0.4.0/banc.egg-info/
+-rw-rw-r--   0 jasper     (501) staff       (20)     6741 2024-04-14 16:15:27.000000 banc-0.4.0/banc.egg-info/PKG-INFO
+-rw-rw-r--   0 jasper     (501) staff       (20)      575 2024-04-14 16:15:27.000000 banc-0.4.0/banc.egg-info/SOURCES.txt
+-rw-rw-r--   0 jasper     (501) staff       (20)        1 2024-04-14 16:15:27.000000 banc-0.4.0/banc.egg-info/dependency_links.txt
+-rw-rw-r--   0 jasper     (501) staff       (20)      219 2024-04-14 16:15:27.000000 banc-0.4.0/banc.egg-info/requires.txt
+-rw-rw-r--   0 jasper     (501) staff       (20)        5 2024-04-14 16:15:27.000000 banc-0.4.0/banc.egg-info/top_level.txt
+-rw-rw-r--   0 jasper     (501) staff       (20)      219 2023-08-04 20:01:20.000000 banc-0.4.0/requirements.txt
+-rw-rw-r--   0 jasper     (501) staff       (20)       38 2024-04-14 16:15:27.000000 banc-0.4.0/setup.cfg
+-rw-rw-r--   0 jasper     (501) staff       (20)     1026 2024-04-14 16:14:39.000000 banc-0.4.0/setup.py
```

### Comparing `banc-0.3.0/LICENSE` & `banc-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `banc-0.3.0/PKG-INFO` & `banc-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: banc
-Version: 0.3.0
+Version: 0.4.0
 Summary: Tools for the GridTape-TEM dataset of an adult female fly's Brain And Nerve Cord
 Home-page: https://github.com/jasper-tms/the-BANC-fly-connectome
 Author: Jasper Phelps
 Author-email: jasper.s.phelps@gmail.com
 License: UNKNOWN
 Description: # The Brain And Nerve Cord fly connectome
```

### Comparing `banc-0.3.0/README.md` & `banc-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `banc-0.3.0/banc/annotations.py` & `banc-0.4.0/banc/annotations.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 This module specifies rules governing what annotations are allowed to be posted
 to certain "managed" CAVE tables (where only pre-approved types of annotations
 may be posted). These rules are typically used for centralized community tables
 to which many users can post annotations, in order to maintain some consistency
 in which annotations are posted to the table.
 """
 
+from datetime import datetime, timezone
+
 import anytree
 
-from . import lookup
+from . import auth, lookup
 
-help_url = 'https://fanc.community/Neuron-annotations#neuron_information'
+help_url = 'https://github.com/jasper-tms/the-BANC-fly-connectome/wiki/Annotations-(cell-types,-etc.)'
 help_msg = 'See the annotation scheme described at ' + help_url
 
 default_table = 'cell_info'
 
 
 cell_info = {
     'primary class': {
@@ -45,14 +47,24 @@
                 'T3 leg UM neuron': {},
                 'neck UM neuron': {},
                 'wing UM neuron': {},
                 'haltere UM neuron': {},
                 'abdominal UM neuron': {}}},
         'glia': {
             'trachea': {}}},
+    'fast neurotransmitter': {
+        'cholinergic': {},
+        'GABAergic': {},
+        'glutamatergic': {}},
+    'other neurotransmitter': {
+        'dopaminergic': {},
+        'histaminergic': {},
+        'octopaminergic': {},
+        'serotonergic': {},
+        'tyraminergic': {}},
     'soma side': {
         'soma on left': {},
         'soma on right': {},
         'soma on midline': {}},
     'soma segment': {
         'soma in brain': {
             'soma in central brain': {},
@@ -119,18 +131,19 @@
         'PDMN1 bundle': {},
         'PDMN2 bundle': {},
         'HN bundle': {},
         'T3 H1 bundle': {},
         'T3 H2 bundle': {},
         'T3 H3 bundle': {}},
     'neuron identity': {},
+    'freeform': {},
 }
 FANC_cell_info = cell_info.copy()
 FANC_cell_info['publication'] = {
-    'Azevedo Lesser Mark Phelps et al. 2022': {},
+    'Azevedo Lesser Phelps Mark et al. 2024': {},
     'Lesser Azevedo et al. 2023': {},
     'Cheong Boone Bennett et al. 2023': {},
     'Sapkal et al. 2023': {},
     'Yang et al. 2023': {},
     'Dallmann et al. 2023': {}
 }
 
@@ -163,14 +176,15 @@
             node = anytree.Node(annotation, parent=parent)
             nodes[annotation] = nodes.get(annotation, []) + [node]
             _build_tree(annotations[annotation], parent=node, nodes=nodes)
         return nodes
 
     return _build_tree(dictionary)
 
+
 # Convert any hierarchical dictionaries to a tree format that is easier to use
 rules_governing_tables = {table_name: _dict_to_anytree(annotations)
                           if isinstance(annotations, dict) else annotations
                           for table_name, annotations in rules_governing_tables.items()}
 
 
 def print_recognized_annotations(table_name: str = default_table):
@@ -228,71 +242,74 @@
         specifying the annotation hierarchy/rules directly. The dict must
         map annotation names (str) to anytree.Node objects, as output by
         running _dict_to_anytree() on a hierarchy of annotations.
     """
     if isinstance(table_name, str):
         try:
             annotations = rules_governing_tables[table_name]
-        except:
+        except KeyError:
             raise ValueError(f'Table name "{table_name}" not recognized.')
         if not isinstance(annotations, dict):
             raise ValueError(f'"{table_name}" does not use paired annotations.')
     elif isinstance(table_name, dict):
         annotations = table_name
     else:
         raise TypeError(f'Unrecognized type for table_name: {type(table_name)}')
 
     try:
         annotation_nodes = annotations[annotation]
-    except:
+    except KeyError:
         raise ValueError(f'Annotation "{annotation}" not recognized. {help_msg}')
 
     if len(annotation_nodes) > 1:
         raise ValueError(f'Class of "{annotation}" could not be guessed'
                          f' because it has multiple possible classes. {help_msg}')
 
     if annotation_nodes[0].is_root:
         raise ValueError(f'"{annotation}" is a base annotation with no class. {help_msg}')
     return annotation_nodes[0].parent.name
 
 
-def is_valid_annotation(annotation: str or tuple[str, str],
+def is_valid_annotation(annotation: str or tuple[str, str] or bool,
                         table_name: str = default_table,
+                        response_on_unrecognized_table='raise',
                         raise_errors: bool = True) -> bool:
     """
     Determine whether an annotation is a recognized/valid annotation
     for the given table.
 
     Parameters
     ----------
-    annotation : str or list/tuple of 2 strs
+    annotation : str or list/tuple of 2 strs or bool
         The annotation or annotation pair to check the validity of.
     table_name : str
         The name of the table whose rules should be used to determine the
         validity of the annotation.
         OR
         Users will not typically do this, but you can also pass in a list or
         dict specifying the valid annotations directly and it will be used. If
         a dictionary, must map annotation names (str) to anytree.Node objects,
         as output by running _dict_to_anytree() on a hierarchy of annotations.
     """
     if isinstance(table_name, str):
-        try:
-            annotations = rules_governing_tables[table_name]
-        except:
-            raise ValueError(f'Table name "{table_name}" not recognized.')
+        annotations = rules_governing_tables.get(table_name, None)
+        if annotations is None:
+            client = auth.get_caveclient()
+            if (client.annotation.get_table_metadata(table_name)['schema_type']
+                    != 'proofreading_boolstatus_user'):
+                if response_on_unrecognized_table == 'raise':
+                    raise ValueError(f'No annotation rules found for table "{table_name}"')
+                return response_on_unrecognized_table
+            annotations = [True, False]
     elif isinstance(table_name, (dict, list)):
         annotations = table_name
     else:
         raise TypeError(f'Unrecognized type for table_name: {type(table_name)}')
 
     if isinstance(annotations, list):
-        if not isinstance(annotation, str):
-            raise TypeError('annotation should be a str for this table, but'
-                            f' was {type(annotation)}')
         if (annotation not in annotations) and raise_errors:
             raise ValueError(f'Annotation "{annotation}" not recognized. {help_msg}')
         return annotation in annotations
 
     if raise_errors:
         annotation_class, annotation = parse_annotation_pair(annotation)
     else:
@@ -368,41 +385,41 @@
         specifying the valid annotations directly and it will be used. The
         dict must map annotation names (str) to anytree.Node objects, as
         output by running _dict_to_anytree() on a hierarchy of annotations.
     """
     if isinstance(table_name, str):
         try:
             annotations = rules_governing_tables[table_name]
-        except:
+        except KeyError:
             raise ValueError(f'Table name "{table_name}" not recognized.')
         if not isinstance(annotations, dict):
             raise ValueError(f'"{table_name}" does not use paired annotations.')
     elif isinstance(table_name, dict):
         annotations = table_name
     else:
         raise TypeError(f'Unrecognized type for table_name: {type(table_name)}')
 
-    if annotation_class == 'neuron identity':
+    if annotation_class in ['neuron identity', 'freeform']:
         if annotation in annotations:
             if raise_errors:
                 raise ValueError(f'The term "{annotation}" is a class,'
                                  f' not an identity. {help_msg}')
             return False
         return True
 
     try:
         class_nodes = annotations[annotation_class]
-    except:
+    except KeyError:
         if raise_errors:
             raise ValueError(f'Annotation class "{annotation_class}" not'
                              f' recognized. {help_msg}')
         return False
     try:
         annotation_nodes = annotations[annotation]
-    except:
+    except KeyError:
         if raise_errors:
             raise ValueError(f'Annotation "{annotation}" not recognized.'
                              f' {help_msg}')
         return False
 
     for class_node in class_nodes:
         for annotation_node in annotation_nodes:
@@ -421,16 +438,17 @@
             raise ValueError(f'Annotation "{annotation}" belongs to classes'
                              f' {parent_names} but you specified class'
                              f' "{annotation_class}". {help_msg}')
     return False
 
 
 def is_allowed_to_post(segid: int,
-                       annotation: str or tuple[str, str],
+                       annotation: str or tuple[str, str] or bool,
                        table_name: str = default_table,
+                       response_on_unrecognized_table='raise',
                        raise_errors: bool = True) -> bool:
     """
     Determine whether a particular segment is allowed to be annotated
     with the given annotation (or annotation_class+annotation pair, if the
     table uses paired annotations).
 
     For posting to be allowed:
@@ -440,14 +458,15 @@
       additional constraints apply:
       1. The given annotation pair may not be posted if the segment
       already has any annotation pair with the same annotation_class.
       This and also prevents a class from having multiple subclasses.
       This rule is NOT enforced for a few special annotation_classes
       that are allowed to have many subannotations:
         - 'neuron identity'
+        - 'freeform'
         - 'publication'
       2. The given annotation pair may only be posted if its
       annotation_class is at the root of the annotation tree (e.g.
       'primary class'), or if its annotation_class is already an
       annotation on the segment. In other words, allow posts will start
       from the root of the annotation tree, or add detail/subclass
       information to an annotation already on the segment.
@@ -467,20 +486,39 @@
       annotation_class+annotation pair in the given CAVE table without
       violating any rules about redundancy or mutual exclusivity.
     - False: The proposed annotation or annotation_class+annotation pair
       MAY NOT be posted for this segment without violating a rule.
       If `raise_errors` is True, an exception with an informative error
       message will be raised instead of returning False.
     """
-    try:
-        annotations = rules_governing_tables[table_name]
-    except:
-        raise ValueError(f'Table name "{table_name}" not recognized.')
+    annotations = rules_governing_tables.get(table_name, None)
+    if annotations is None:
+        client = auth.get_caveclient()
+        if (client.annotation.get_table_metadata(table_name)['schema_type']
+                != 'proofreading_boolstatus_user'):
+            if response_on_unrecognized_table == 'raise':
+                raise ValueError(f'No annotation rules found for table "{table_name}"')
+            return response_on_unrecognized_table
+        if not isinstance(annotation, bool):
+            raise ValueError(f'Table "{table_name}" only uses True/False annotations.')
+        existing_annos = client.materialize.live_live_query(
+            table_name,
+            datetime.now(timezone.utc),
+            filter_equal_dict={table_name: {
+                'valid_id': segid,
+                'proofread': {True: 't', False: 'f'}[annotation]
+            }}
+        )
+        if raise_errors and not existing_annos.empty:
+            raise ValueError(f'Segment {segid} already has this annotation'
+                             f' in the table "{table_name}".')
+        return existing_annos.empty
 
     if not is_valid_annotation(annotation, table_name=table_name,
+                               response_on_unrecognized_table=response_on_unrecognized_table,
                                raise_errors=raise_errors):
         return False
 
     existing_annos = lookup.annotations(segid, source_tables=table_name,
                                         return_details=True)
 
     if isinstance(annotations, list):
@@ -498,21 +536,23 @@
         try:
             annotation_class, annotation = parse_annotation_pair(annotation)
         except:
             return False
 
     # Rule 1
     multiple_subclasses_allowed = [
+        'other neurotransmitter',
         'neuron identity',
+        'freeform',
         'publication'
     ]
     if annotation_class in multiple_subclasses_allowed:
         # Check if any tag,tag2 pair is the same as annotation,annotation_class
         if ((existing_annos.tag == annotation) &
-            (existing_annos.tag2 == annotation_class)).any():
+                (existing_annos.tag2 == annotation_class)).any():
             if raise_errors:
                 raise ValueError(f'Segment {segid} already has this exact'
                                  ' annotation pair.')
             return False
         #------
         # The block of code below is not currently used due to a refactoring of
         # the annotation tree, but it might be useful to bring back later
```

### Comparing `banc-0.3.0/banc/connectivity.py` & `banc-0.4.0/banc/connectivity.py`

 * *Files identical despite different names*

### Comparing `banc-0.3.0/banc/lookup.py` & `banc-0.4.0/banc/lookup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #!/usr/bin/env python3
 
+import re
 import collections
 from concurrent import futures
 from datetime import datetime
+from typing import Literal
 
 import numpy as np
 import pandas as pd
 import requests
 import tqdm
 import cloudvolume
 
@@ -14,20 +16,20 @@
 
 #In this section where default tables are specified:
 # Tuples are always (table_name, column_name) to specify one column within one table
 # Lists are always [table_name1, table_name2, ...] to specify multiple tables,
 #   or [(table_name1, column_name1), (table_name2, column_name2), ...] to more
 #   explicitly specify multiple columns
 default_cellid_source = ('cell_ids', 'user_id')
-default_proofreading_tables = []
+default_proofreading_tables = ['backbone_proofread']
 default_annotation_sources = [('cell_info', 'tag'),
-                              ('proofreading_notes', 'tag'),
                               ('neck_connective_y92500', 'tag'),
-                              ('peripheral_nerves', 'tag')]
-default_anchor_point_sources = ['cell_ids', 'somas_v1', 'neck_connective_y92500', 'peripheral_nerves']
+                              ('peripheral_nerves', 'tag'),
+                              ('backbone_proofread', 'proofread')]
+default_anchor_point_sources = ['cell_ids', 'neck_connective_y92500', 'peripheral_nerves']
 default_svid_lookup_url = 'https://catmaid3.hms.harvard.edu/services/transform-service/query/dataset/banc_lookup_local/s/2/values_array_string_response'
 
 
 # --- START CAVE TABLES / ANNOTATIONS SECTION --- #
 def proofreading_status(segids: int or list[int],
                         source_tables: str or list[str] = default_proofreading_tables,
                         timestamp='now') -> None or str or tuple(str, list):
@@ -104,33 +106,35 @@
 
 
 def cells_annotated_with(tags: str or list[str],
                          *,
                          exclude_tags: str or list[str] = None,
                          source_tables=default_annotation_sources,
                          timestamp='now',
-                         return_as: ['list', 'url'] = 'list',
+                         return_as: Literal['list', 'url'] = 'list',
                          raise_not_found=True):
     """
     Get all the cells annotated with a given text tag / all of the given text
     tags.
 
     Arguments
     ---------
     tags: str or list of str
-      The tag(s) to query. If multiple are provided, only cells
-      with all the given tags will be returned.
+      The tag(s) to query. If multiple tags are provided,
+      only cells with ALL of the listed tags will be returned.
+      If a string contains ' and ' or ' AND ', it will be split into
+      a list of multiple tags.
       Any tag that starts with 'not ' or 'NOT ' will be moved
       to exclude_tags (see below).
 
     exclude_tags: str or list of str, default None
-      The tag(s) to exclude from the query. If multiple are provided, only
-      cells with none of the given tags will be returned.
-      You may also specify exclude_tags via the tags argument (above) by
-      prepending 'not ' or 'NOT ' to the tag name.
+      The tag(s) to exclude from the query. If multiple are provided,
+      only cells with NONE of the exclude_tags will be returned.
+      You may also specify exclude_tags by putting 'not {tag}' or
+      'NOT {tag}' in the `tags` argument above.
 
     source_tables: str OR list of str OR list of 2-tuple of str
       str OR list of str:
         The name(s) of the CAVE table(s) to query for annotations. Annotations
         will be pulled from the column named 'tag', so they must contain a
         column with that name.
       list of 2-tuple of str:
@@ -156,18 +160,25 @@
     """
     if isinstance(tags, str):
         tags = [tags]
     if exclude_tags is None:
         exclude_tags = []
     if isinstance(exclude_tags, str):
         exclude_tags = [exclude_tags]
-    if not return_as in ['list', 'url']:
+    if return_as not in ['list', 'url']:
         raise ValueError('return_as must be either "list" or "url"')
+    # Parse 'and'
+    tags = [tag for string in tags for tag in
+            re.split(re.compile(' and ', re.IGNORECASE), string) if tag]
+    exclude_tags = [tag for string in exclude_tags for tag in
+                    re.split(re.compile(' and ', re.IGNORECASE), string) if tag]
+    # Parse 'not'
     exclude_tags = exclude_tags + [tag[4:] for tag in tags if tag.lower().startswith('not ')]
     tags = [tag for tag in tags if not tag.lower().startswith('not ')]
+
     annos = all_annotations(source_tables=source_tables,
                             timestamp=timestamp,
                             group_by_segid=False)
     is_invalid = [tag not in annos.tag.unique() for tag in tags]
     if any(is_invalid):
         raise KeyError('Check your spelling – the following tags are not'
                        ' present at all in the annotation tables:'
@@ -241,24 +252,34 @@
         timestamp = client.materialize.get_timestamp()
 
     source_tables = _format_annotation_sources(source_tables)
 
     annos = []
     for table_name, column_name in source_tables:
         table = client.materialize.live_live_query(table_name, timestamp)
+        table.sort_values(by='created', inplace=True)
         table['source_table'] = table_name
         table['created'] = table['created'].apply(datetime.date)
         if 'user_id' not in table.columns:
             table['user_id'] = None
         if column_name != 'tag2':
             if 'tag2' not in table.columns:
                 table['tag2'] = None
             table.rename(columns={column_name: 'tag'}, inplace=True)
         else:
             table['tag'] = table['tag2']
+        if (table['tag'] == 't').any():
+            if not (table['tag'] == 't').all():
+                raise ValueError(f'Column "{column_name}" in table "{table_name}"'
+                                 ' contains "t" and other values. This is unexpected.')
+            # For boolean columns, use the table name as the tag
+            table['tag'] = table_name.replace('_', ' ')
+            # Only include the table name as a tag once for each neuron
+            table.drop_duplicates(subset=['pt_root_id'], keep='last', inplace=True)
+
         annos.append(table[['pt_root_id', 'tag', 'tag2', 'pt_position',
                             'user_id', 'source_table', 'created']])
 
     annos = pd.concat(annos).sort_values(by='created').reset_index(drop=True)
     if group_by_segid:
         annos = annos.groupby('pt_root_id')['tag'].apply(list)
     return annos
@@ -332,25 +353,34 @@
 
     # Fast mode: use filter_in_dict to request only the annotations we want from the server
     tables = []
     for table_name, column_name in source_tables:
         table = client.materialize.live_live_query(
             table_name, timestamp, filter_in_dict={table_name: {'pt_root_id': segids}})
         table['source_table'] = table_name
+        table.sort_values(by='created', inplace=True)
         if 'user_id' not in table.columns:
             table['user_id'] = None
         if column_name != 'tag2':
             if 'tag2' not in table.columns:
                 table['tag2'] = None
             table.rename(columns={column_name: 'tag'}, inplace=True)
         else:
             table['tag'] = table['tag2']
+        if (table['tag'] == 't').any():
+            if not (table['tag'] == 't').all():
+                raise ValueError(f'Column "{column_name}" in table "{table_name}"'
+                                 ' contains "t" and other values. This is unexpected.')
+            # For boolean columns, use the table name as the tag
+            table['tag'] = table_name.replace('_', ' ')
+            # Only include the table name as a tag once
+            table = table[-1:]
         tables.append(table[['pt_root_id', 'tag', 'tag2', 'pt_position',
                             'user_id', 'source_table', 'created']])
-    table = pd.concat(tables).sort_values(by='created').reset_index(drop=True)
+    table = pd.concat(tables).reset_index(drop=True)
 
     if return_details:
         return table
     return [[anno for anno in table.loc[table.pt_root_id == s, 'tag']] for s in segids]
 
 
 def _format_annotation_sources(source_tables):
@@ -444,17 +474,17 @@
     Order is preserved - the segID corresponding to the Nth point in
     the argument will be the Nth value in the returned array.
     """
     if timestamp == 'now':
         # cv.get_roots interprets timestamp=None as requesting the latest root
         timestamp = None
 
-    #print('WARNING: The supervoxel ID lookup service is not set up yet,'
-    #      ' so the slower cloudvolume lookup will be used.')
-    #return segid_from_pt_cv(points, timestamp=timestamp, **kwargs)
+    print('WARNING: The supervoxel ID lookup service is not set up yet,'
+          ' so the slower cloudvolume lookup will be used.')
+    return segid_from_pt_cv(points, timestamp=timestamp, **kwargs)
 
     svids = svid_from_pt(points, service_url=service_url)
 
     if 'cv' in kwargs:
         cv = kwargs['cv']
     else:
         cv = auth.get_cloudvolume()
@@ -781,27 +811,34 @@
     if not all(client.chunkedgraph.is_latest_roots(segids, timestamp=timestamp)):
         raise KeyError('A given ID(s) is not valid at the given timestamp.'
                        ' Use updated IDs or provide the timestamp where'
                        ' the ID(s) is valid.')
 
     if table in [None, 'default_soma_table']:
         table = client.info.get_datastack_info()['soma_table']
-        select_columns = None  # Feature not currently supported on reference tables
+        joins = [[table, 'id', 'somas_dec2022', 'id']]
     elif table in ['all', 'somas']:
         table = 'somas_dec2022'
+        joins = None
     elif table in ['neurons', 'neuron']:
         table = 'neuron_somas_dec2022'
-        select_columns = None  # Feature not currently supported on reference tables
+        joins = [[table, 'id', 'somas_dec2022', 'id']]
     elif table == 'glia':
         table = 'glia_somas_dec2022'
-        select_columns = None  # Feature not currently supported on reference tables
-    somas = client.materialize.query_table(table,
-                                           select_columns=select_columns,
-                                           timestamp=timestamp)
-    return somas.loc[somas.pt_root_id.isin(segids)]
+        joins = [[table, 'id', 'somas_dec2022', 'id']]
+    else:
+        raise ValueError(f'Unknown table name {table}. See docstring for options.')
+    somas = client.materialize.live_live_query(
+        table,
+        joins=joins,
+        timestamp=timestamp,
+        filter_in_dict={'somas_dec2022': {'pt_root_id': segids}}
+    )
+    somas.rename(columns={'idx': 'id'}, inplace=True)
+    return somas[select_columns]
 # --- END KEY ATTRIBUTES SECTION --- #
 
 
 # The code below implements a slower version of segid_from_pt that
 # you should never need to run as long as the service is operational. If the
 # service goes down, try using segid_from_pt_cv instead
 class GSPointLoader(object):
```

### Comparing `banc-0.3.0/banc/ngl_info.py` & `banc-0.4.0/banc/ngl_info.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,45 +25,50 @@
 syn = {'name': 'postsynapses',
        'path': '<not available>'}
 
 # The soma_table's flat_segmentation_source is the un-_verified layer
 #nuclei = {'name': 'nuclei_TODO-DATE',
 #          'path': client.annotation.get_table_metadata(info['soma_table'])['flat_segmentation_source']
 # so instead hardcode the _verified layer:
-nuclei = {'name': 'nuclei (verified)',
-          'path': '<not available>'}
+nuclei = {'name': 'nuclei_v1',
+          'path': 'precomputed://gs://lee-lab_brain-and-nerve-cord-fly-connectome/nuclei/seg_v1'}
 
 view_options = dict(
     position=[113200, 106900, 3100],
-    zoom_3d=6700,
+    zoom_3d=260000,
     layout='xy-3d'
 )
-zoom_2d = 12
-
-
-outlines_layer = {'type': 'segmentation', 'source': {'url': 'precomputed://gs://zetta_lee_fly_cns_001_kisuk/final/v2/volume_meshes', 'transform': {'matrix': [[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 0.9462, 0]], 'outputDimensions': {'x': [4e-9, 'm'], 'y': [4e-9, 'm'], 'z': [4.5e-8, 'm']}}, 'subsources': {'mesh': True}, 'enableDefaultSubsources': False}, 'tab': 'segments', 'meshSilhouetteRendering': 2, 'segments': ['1'], 'segmentDefaultColor': '#2a7fff', 'name': 'region outlines'}
+zoom_2d = 16
 
+outlines_layer = {'type': 'segmentation', 'source': {'url': 'precomputed://gs://lee-lab_brain-and-nerve-cord-fly-connectome/volume_meshes', 'subsources': {'mesh': True, 'bounds': True}, 'enableDefaultSubsources': False}, 'tab': 'segments', 'meshSilhouetteRendering': 2, 'segments': ['1'], 'segmentDefaultColor': '#2a7fff', 'name': 'region outlines'}
 
 
 def final_json_tweaks(state):
     """
     Apply some final changes to the neuroglancer state that I didn't take the
     time to figure out how to do through nglui, by directly modifying the
     json/dict representation of the state.
     """
     for layer in state['layers']:
         if layer['name'] == seg['name']:
             layer['selectedAlpha'] = 0.4
+            layer['tab'] = 'segments'
+            layer['toolBindings'] = {
+                "M": "grapheneMergeSegments",
+                "C": "grapheneMulticutSegments",
+                "F": "grapheneFindPath"
+            }
         if layer['name'] == nuclei['name']:
-            #layer['visible'] = False
+            layer['visible'] = False
             layer['ignoreSegmentInteractions'] = True
             layer['selectedAlpha'] = 0.8
         if layer['name'] == syn['name']:
             layer['visible'] = False
             layer['shader'] = 'void main() { emitRGBA(vec4(1, 0, 1, toNormalized(getDataValue()))); }'
 
     state['crossSectionScale'] = zoom_2d
     state['crossSectionOrientation'] = [0, 1, 0, 0]
+    state['projectionOrientation'] = [0, 1, 0, 0]
     state.update({
-        'gpuMemoryLimit': 4_000_000_000,
-        'systemMemoryLimit': 4_000_000_000,
+        'gpuMemoryLimit': 6_000_000_000,
+        'systemMemoryLimit': 8_000_000_000,
     })
```

### Comparing `banc-0.3.0/banc/publish.py` & `banc-0.4.0/banc/publish.py`

 * *Files identical despite different names*

### Comparing `banc-0.3.0/banc/render_neurons.py` & `banc-0.4.0/banc/render_neurons.py`

 * *Files identical despite different names*

### Comparing `banc-0.3.0/banc/skeletonize.py` & `banc-0.4.0/banc/skeletonize.py`

 * *Files identical despite different names*

### Comparing `banc-0.3.0/banc/statebuilder.py` & `banc-0.4.0/banc/statebuilder.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 try:
     from trimesh import exchange
 except ImportError:
     from trimesh import io as exchange
 import pymaid
 from cloudvolume import CloudVolume
 from cloudvolume.frontends.precomputed import CloudVolumePrecomputed
-from nglui.statebuilder import *
+from nglui.statebuilder import (StateBuilder, ChainedStateBuilder,
+                                ImageLayerConfig, SegmentationLayerConfig,
+                                AnnotationLayerConfig, PointMapper, SphereMapper)
 
 from . import auth, lookup
 from .transforms import realignment
 
 
 def render_scene(neurons=None,
                  annotations=None,
@@ -119,16 +121,17 @@
 
     if annotation_units not in ['nm', 'nanometer', 'nanometers', 'vox', 'voxel', 'voxels']:
         raise ValueError(f"annotation_units must be 'nm' or 'voxel' but was {annotation_units}")
 
     # Build a DataFrame containing rootIDs starting from whatever type is given
     if neurons is None:
         # None -> np.array
-        # Default to showing the 'homepage' FANC neuron
-        neurons = np.array([[48848, 114737, 2690]])
+        # By default show two neck motor neurons
+        neurons = np.array([[110000, 108000, 3100],
+                            [110000, 108800, 3100]])
     elif isinstance(neurons, (int, np.integer)):
         # int -> list
         neurons = [neurons]
     elif isinstance(neurons, str):
         # str -> DataFrame
         neurons = client.materialize.query_table(neurons, materialization_version=materialization_version)
 
@@ -143,15 +146,15 @@
             # Otherwise the series must contain root IDs
             neurons = neurons.to_frame(name='pt_root_id')
     if isinstance(neurons, np.ndarray):
         # np.array -> list
         if np.any(neurons < 10000000000000000):
             # If array contains point coordinates instead of rootIDs, lookup rootIDs
             neurons = lookup.segid_from_pt(neurons)
-        neurons = list(neurons)
+        neurons = list(neurons) if isinstance(neurons, np.ndarray) else [neurons]
     if isinstance(neurons, list):
         # list -> pd.DataFrame
         neurons = pd.DataFrame({'pt_root_id': neurons})
 
     if not isinstance(neurons, pd.DataFrame):
         raise TypeError('Could not determine how to handle neurons argument,'
                         ' which is now a {}'.format(type(neurons)))
@@ -187,17 +190,20 @@
         source=ngl_info.seg['path'],
         selected_ids_column='pt_root_id',
         color_column=color_column,
         fixed_ids=None,
         active=True
     )
 
-    StateBuilderDefaultSettings = lambda layers : StateBuilder(layers=layers,
-                                                               resolution=ngl_info.voxel_size,
-                                                               view_kws=ngl_info.view_options)
+    def StateBuilderDefaultSettings(layers):
+        return StateBuilder(
+            layers=layers,
+            resolution=ngl_info.voxel_size,
+            view_kws=ngl_info.view_options
+        )
 
     # Additional layer(s)
     additional_states = []
     additional_data = []
     if annotations is not None:
         if annotation_units in ['nm', 'nanometer', 'nanometers']:
             annotation_layer_resolution = (1, 1, 1)
@@ -273,26 +279,27 @@
         additional_states.append(StateBuilderDefaultSettings([nuclei_config]))
     if synapses_layer:
         synapses_config = ImageLayerConfig(name=ngl_info.syn['name'],
                                            source=ngl_info.syn['path'])
         additional_states.append(StateBuilder([synapses_config]))
         additional_data.append(None)
 
-
     # Build a state with the requested layers
     standard_state = StateBuilderDefaultSettings([img_config, seg_config])
     chained_sb = ChainedStateBuilder([standard_state] + additional_states)
 
     # Turn state into a dict, then add some last settings manually
-    state = chained_sb.render_state([neurons] + additional_data, return_as='dict')
+    state = chained_sb.render_state([neurons] + additional_data,
+                                    return_as='dict',
+                                    target_site='cave-explorer')
     if outlines_layer:
         state['layers'].insert(2, ngl_info.outlines_layer)
     ngl_info.final_json_tweaks(state)
     state.update(misc_settings)
 
     if return_as == 'json':
         return state
     elif return_as == 'url':
         json_id = client.state.upload_state_json(state)
-        return client.state.build_neuroglancer_url(json_id, ngl_info.ngl_app_url)
+        return client.state.build_neuroglancer_url(json_id, ngl_info.ngl_app_url, 'cave-explorer')
     else:
         raise ValueError('"return_as" must be "json" or "url" but was {}'.format(return_as))
```

### Comparing `banc-0.3.0/banc/statemanager.py` & `banc-0.4.0/banc/statemanager.py`

 * *Files identical despite different names*

### Comparing `banc-0.3.0/banc/synaptic_links.py` & `banc-0.4.0/banc/synaptic_links.py`

 * *Files identical despite different names*

### Comparing `banc-0.3.0/banc/template_spaces.py` & `banc-0.4.0/banc/template_spaces.py`

 * *Files identical despite different names*

### Comparing `banc-0.3.0/banc/transforms/realignment.py` & `banc-0.4.0/banc/transforms/realignment.py`

 * *Files identical despite different names*

### Comparing `banc-0.3.0/banc/transforms/template_alignment.py` & `banc-0.4.0/banc/transforms/template_alignment.py`

 * *Files identical despite different names*

### Comparing `banc-0.3.0/banc/upload.py` & `banc-0.4.0/banc/upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,102 +118,128 @@
         if cell_type == 'brain glia':
             try_annotate_neuron(segid, ('primary class', 'glia'), user_id)
         if cell_type == 'VNC glia':
             try_annotate_neuron(segid, ('primary class', 'glia'), user_id)
 
 
 def annotate_neuron(neuron: 'segID (int) or point (xyz)',
-                    annotation: str or tuple[str, str],
+                    annotation: str or tuple[str, str] or bool,
                     user_id: int,
                     table_name='cell_info',
                     convert_given_point_to_anchor_point=True,
-                    resolve_duplicate_anchor_points=False) -> dict:
+                    resolve_duplicate_anchor_points=False,
+                    select_nth_anchor_point=0) -> dict:
     """
     Upload information about a neuron to a CAVE table.
 
     This function will first check that `annotation` is a valid
     annotation for the given table, according to the rules described at
-    https://github.com/htem/FANC_auto_recon/wiki/Neuron-annotations#neuron_information
+    https://github.com/htem/FANC_auto_recon/wiki/Neuron-annotations
     If it is, the annotation will be posted to the table.
 
     This function is designed for use with tables with one of these schemas:
     - "bound_tag_user", in which case `annotation` should be a single annotation
     - "bound_double_tag_user", in which case `annotation` should be a pair of
       annotations, either as a colon-separated string formatted like
       "annotation_class: annotation", or as a 2-tuple of strings in the order
       (annotation_class, annotation).
+    - "proofreading_boolstatus_user", in which case `annotation` should
+      be True or False.
 
     Arguments
     ---------
     neuron: int OR 3-length iterable of ints/floats
         Segment ID or point coordinate of a neuron to upload information about
 
-    annotation: str OR 2-tuple of (str, str)
+    annotation: str OR 2-tuple of (str, str) OR bool
         Annotation to upload, or a pair of annotations if trying to upload to a
         table with two tag columns. See the docstring of
         `fanc.annotations.parse_annotation_pair()` for options on how to format
         an annotation pair.
 
     user_id: int
         The CAVE user ID number to associate with this annotation
 
     table_name: str
         Name of the CAVE table to upload information to. Only works
-        with tables of schema "bound_tag_user" or "bound_double_tag_user".
+        with tables of schema "bound_tag_user", "bound_double_tag_user",
+        or "proofreading_boolstatus_user".
 
     convert_given_point_to_anchor_point: bool
         Only matters if `neuron` is a point (not a segment ID).
         If False, the given point will just be used directly as the
         annotation's point. If True, the point used for the annotation will
         instead be the anchor point (see `lookup.anchor_point()`) of the
         segment corresponding to the given point.
 
     resolve_duplicate_anchor_points: bool or int
         This argument is passed to `lookup.anchor_point`, see its
         docstring for details.
 
+    select_nth_anchor_point: int
+        This argument is passed to `lookup.anchor_point`, see its
+        docstring for details.
+
     Returns
     -------
     list: Response from server containing information about the
           success or failure of the upload. If successful, the list
           contains the ID of the new annotation.
     """
     client = auth.get_caveclient()
     if isinstance(neuron, (int, np.integer)):
         if not client.chunkedgraph.is_latest_roots(int(neuron)):
             raise ValueError(f'{neuron} is not a current segment ID.')
         segid = neuron
-        point = lookup.anchor_point(neuron, resolve_duplicates=resolve_duplicate_anchor_points)
+        point = lookup.anchor_point(neuron,
+                                    resolve_duplicates=resolve_duplicate_anchor_points,
+                                    select_nth_duplicate=select_nth_anchor_point)
     else:
         try:
             iter(neuron)
             segid = lookup.segid_from_pt(neuron)
             if segid == 0:
                 raise ValueError(f'Point {neuron} is a location with no segmentation.')
             if convert_given_point_to_anchor_point:
-                point = lookup.anchor_point(segid, resolve_duplicates=resolve_duplicate_anchor_points)
+                point = lookup.anchor_point(segid,
+                                            resolve_duplicates=resolve_duplicate_anchor_points,
+                                            select_nth_duplicate=select_nth_anchor_point)
                 print(f'Found segID {segid} with anchor point {point}.')
             else:
                 point = np.array(neuron)
         except TypeError:
             raise TypeError('First argument must be a segID or a point coordinate.')
     if not isinstance(user_id, (int, np.integer)):
         raise TypeError(f'user_id must be an integer but got "{user_id}".')
 
     stage = client.annotation.stage_annotations(table_name)
-    if not annotations.is_allowed_to_post(segid, annotation,
-                                          table_name=table_name,
-                                          raise_errors=True):
+    try:
+        allowed_to_post = annotations.is_allowed_to_post(segid, annotation,
+                                                         table_name=table_name,
+                                                         raise_errors=True)
+    except ValueError as e:
+        if not e.args or not e.args[0].startswith('No annotation rules found for table'):
+            raise e
+        allowed_to_post = True
+    if not allowed_to_post:
         raise ValueError(f'"{annotation}" is not allowed to be posted to'
                          f' segment {segid} in table "{table_name}".')
 
     if 'tag2' in stage.fields:
         annotation = annotations.parse_annotation_pair(annotation)
 
-    if isinstance(annotation, tuple):
+    if 'tag' not in stage.fields:
+        if 'valid_id' in stage.fields and 'proofread' in stage.fields:
+            stage.add(pt_position=point,
+                      valid_id=int(segid),
+                      proofread=annotation,
+                      user_id=user_id)
+        else:
+            raise ValueError(f'Table "{table_name}" is not a supported schema.')
+    elif isinstance(annotation, tuple):
         assert len(annotation) == 2
         stage.add(pt_position=point,
                   tag=annotation[1],
                   tag2=annotation[0],
                   user_id=user_id)
     elif isinstance(annotation, str):
         stage.add(pt_position=point,
@@ -258,28 +284,35 @@
 
     if isinstance(annotation_sources, str):
         annotation_sources = [(annotation_sources, 'tag')]
     if not isinstance(annotation_sources, list):
         raise TypeError('annotation_sources is an unexpected type. See docstring.')
 
     for table_name, annotation_column in annotation_sources:
+        if annotation.replace(' ', '_') == table_name:
+            anno_query = 't'
+            anno_returned = True
+        else:
+            anno_query = annotation
+            anno_returned = annotation
+
         annos = client.materialize.live_live_query(
             table_name,
             datetime.now(timezone.utc),
-            filter_equal_dict={table_name: {annotation_column: annotation,
+            filter_equal_dict={table_name: {annotation_column: anno_query,
                                             'pt_root_id': segid}}
         )
-        if not 'user_id' in annos.columns:
+        if 'user_id' not in annos.columns:
             annos['user_id'] = None
-        matches = annos.loc[annos['user_id'] == user_id]
         for i, match in annos.loc[annos['user_id'] == user_id].iterrows():
             anno_raw = client.annotation.get_annotation(table_name, match['id'])[0]
             assert anno_raw['user_id'] == user_id
             assert lookup.segid_from_pt(anno_raw['pt_position']) == segid
-            assert anno_raw['tag'] == annotation
+            assert anno_returned in [anno_raw.get('proofread', -1),
+                                     anno_raw.get('tag', -1)]
             client.annotation.delete_annotation(table_name, match['id'])
             return (table_name,
                     match['id'],
                     client.annotation.get_annotation(table_name, match['id'])[0])
 
         for i, nonmatch in annos.loc[annos['user_id'] != user_id].iterrows():
             if nonmatch['user_id'] is None:
```

### Comparing `banc-0.3.0/banc/visualize.py` & `banc-0.4.0/banc/visualize.py`

 * *Files identical despite different names*

### Comparing `banc-0.3.0/banc.egg-info/PKG-INFO` & `banc-0.4.0/banc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: banc
-Version: 0.3.0
+Version: 0.4.0
 Summary: Tools for the GridTape-TEM dataset of an adult female fly's Brain And Nerve Cord
 Home-page: https://github.com/jasper-tms/the-BANC-fly-connectome
 Author: Jasper Phelps
 Author-email: jasper.s.phelps@gmail.com
 License: UNKNOWN
 Description: # The Brain And Nerve Cord fly connectome
```

### Comparing `banc-0.3.0/banc.egg-info/SOURCES.txt` & `banc-0.4.0/banc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `banc-0.3.0/setup.py` & `banc-0.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open('requirements.txt', 'r') as f:
     requirements = f.read().splitlines()
     requirements = [l for l in requirements if not l.startswith('#')]
 
 setuptools.setup(
     name='banc',
-    version='0.3.0',
+    version='0.4.0',
     author='Jasper Phelps',
     author_email='jasper.s.phelps@gmail.com',
     description="Tools for the GridTape-TEM dataset of an adult female"
                 " fly's Brain And Nerve Cord",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/jasper-tms/the-BANC-fly-connectome',
```

