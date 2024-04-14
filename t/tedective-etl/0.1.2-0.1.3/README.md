# Comparing `tmp/tedective_etl-0.1.2.tar.gz` & `tmp/tedective_etl-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tedective_etl-0.1.2.tar", max compression
+gzip compressed data, was "tedective_etl-0.1.3.tar", max compression
```

## Comparing `tedective_etl-0.1.2.tar` & `tedective_etl-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     3779 2024-04-11 14:10:08.207308 tedective_etl-0.1.2/README.md
--rw-r--r--   0        0        0     1175 2024-04-11 21:51:51.847643 tedective_etl-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-05 14:40:09.538488 tedective_etl-0.1.2/tedective_etl/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 10:14:51.437671 tedective_etl-0.1.2/tedective_etl/currency/__init__.py
--rw-r--r--   0        0        0        1 2024-04-11 13:17:38.965153 tedective_etl-0.1.2/tedective_etl/currency/rates.json
--rw-r--r--   0        0        0     1096 2024-04-11 13:15:59.170324 tedective_etl-0.1.2/tedective_etl/currency/update.py
--rw-r--r--   0        0        0     5632 2024-04-11 13:17:43.785095 tedective_etl-0.1.2/tedective_etl/dedupe.py
--rw-r--r--   0        0        0    14149 2024-04-11 13:17:47.029057 tedective_etl-0.1.2/tedective_etl/graph.py
--rw-r--r--   0        0        0    18394 2024-04-11 13:17:50.581014 tedective_etl-0.1.2/tedective_etl/main.py
--rw-r--r--   0        0        0    52887 2024-04-11 13:17:55.408956 tedective_etl-0.1.2/tedective_etl/schema/ocds.py
--rw-r--r--   0        0        0     4469 2024-04-11 13:18:33.060502 tedective_etl-0.1.2/tedective_etl/search.py
--rw-r--r--   0        0        0       62 2024-04-11 13:18:01.080888 tedective_etl-0.1.2/tedective_etl/server.py
--rw-r--r--   0        0        0        0 2024-04-05 14:40:09.542488 tedective_etl-0.1.2/tedective_etl/ted_to_ocds/__init__.py
--rw-r--r--   0        0        0     7781 2024-04-11 13:18:10.044780 tedective_etl-0.1.2/tedective_etl/ted_to_ocds/extractors.py
--rw-r--r--   0        0        0     6292 2024-04-11 13:18:12.740748 tedective_etl-0.1.2/tedective_etl/ted_to_ocds/process.py
--rw-r--r--   0        0        0      178 2024-04-11 13:18:17.776687 tedective_etl-0.1.2/tedective_etl/ted_to_ocds/trackers.py
--rw-r--r--   0        0        0    15886 2024-04-11 13:18:20.804650 tedective_etl-0.1.2/tedective_etl/ted_to_ocds/transform.py
--rw-r--r--   0        0        0     3518 2024-04-11 13:18:24.264608 tedective_etl-0.1.2/tedective_etl/utils.py
--rw-r--r--   0        0        0     5168 1970-01-01 00:00:00.000000 tedective_etl-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     7862 2024-04-13 17:06:49.262786 tedective_etl-0.1.3/README.md
+-rw-r--r--   0        0        0     1205 2024-04-14 09:19:15.100604 tedective_etl-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-15 09:05:10.619627 tedective_etl-0.1.3/tedective_etl/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-17 09:28:40.838132 tedective_etl-0.1.3/tedective_etl/currency/__init__.py
+-rw-r--r--   0        0        0        1 2024-04-13 17:06:49.263786 tedective_etl-0.1.3/tedective_etl/currency/rates.json
+-rw-r--r--   0        0        0     1096 2024-04-13 17:06:49.263786 tedective_etl-0.1.3/tedective_etl/currency/update.py
+-rw-r--r--   0        0        0     5632 2024-04-13 17:06:49.263786 tedective_etl-0.1.3/tedective_etl/dedupe.py
+-rw-r--r--   0        0        0    14149 2024-04-13 17:06:49.264786 tedective_etl-0.1.3/tedective_etl/graph.py
+-rw-r--r--   0        0        0    18394 2024-04-13 17:06:49.264786 tedective_etl-0.1.3/tedective_etl/main.py
+-rw-r--r--   0        0        0    52887 2024-04-13 17:06:49.264786 tedective_etl-0.1.3/tedective_etl/schema/ocds.py
+-rw-r--r--   0        0        0     4469 2024-02-11 16:34:23.573967 tedective_etl-0.1.3/tedective_etl/search.py
+-rw-r--r--   0        0        0       62 2024-02-13 19:06:47.041698 tedective_etl-0.1.3/tedective_etl/server.py
+-rw-r--r--   0        0        0        0 2023-08-14 14:58:10.049645 tedective_etl-0.1.3/tedective_etl/ted_to_ocds/__init__.py
+-rw-r--r--   0        0        0     7919 2024-04-14 07:34:51.958753 tedective_etl-0.1.3/tedective_etl/ted_to_ocds/extractors.py
+-rw-r--r--   0        0        0     6292 2024-04-13 17:06:43.017835 tedective_etl-0.1.3/tedective_etl/ted_to_ocds/process.py
+-rw-r--r--   0        0        0      178 2023-08-16 14:17:01.977527 tedective_etl-0.1.3/tedective_etl/ted_to_ocds/trackers.py
+-rw-r--r--   0        0        0    15886 2024-04-13 17:06:49.264786 tedective_etl-0.1.3/tedective_etl/ted_to_ocds/transform.py
+-rw-r--r--   0        0        0     3518 2024-04-13 17:06:49.264786 tedective_etl-0.1.3/tedective_etl/utils.py
+-rw-r--r--   0        0        0     9251 1970-01-01 00:00:00.000000 tedective_etl-0.1.3/PKG-INFO
```

### Comparing `tedective_etl-0.1.2/pyproject.toml` & `tedective_etl-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "tedective-etl"
-version = "0.1.2"
+version = "0.1.3"
 description = "The XML-to-OCDS parser for the TEDective project based on lxml"
 authors = ["Free Software Foundation Europe e.V. <tedective@fsfe.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "tedective_etl"}]
+exclude = [".devenv/profile"]
 
 [tool.poetry.urls]
 "Homepage" = "https://tedective.org"
 "Repository" = "https://git.fsfe.org/TEDective/etl"
 "Documentation" = "https://docs.tedective.org"
 
 [tool.poetry.scripts]
```

### Comparing `tedective_etl-0.1.2/tedective_etl/currency/update.py` & `tedective_etl-0.1.3/tedective_etl/currency/update.py`

 * *Files identical despite different names*

### Comparing `tedective_etl-0.1.2/tedective_etl/dedupe.py` & `tedective_etl-0.1.3/tedective_etl/dedupe.py`

 * *Files identical despite different names*

### Comparing `tedective_etl-0.1.2/tedective_etl/graph.py` & `tedective_etl-0.1.3/tedective_etl/graph.py`

 * *Files identical despite different names*

### Comparing `tedective_etl-0.1.2/tedective_etl/main.py` & `tedective_etl-0.1.3/tedective_etl/main.py`

 * *Files identical despite different names*

### Comparing `tedective_etl-0.1.2/tedective_etl/schema/ocds.py` & `tedective_etl-0.1.3/tedective_etl/schema/ocds.py`

 * *Files identical despite different names*

### Comparing `tedective_etl-0.1.2/tedective_etl/search.py` & `tedective_etl-0.1.3/tedective_etl/search.py`

 * *Files identical despite different names*

### Comparing `tedective_etl-0.1.2/tedective_etl/ted_to_ocds/extractors.py` & `tedective_etl-0.1.3/tedective_etl/ted_to_ocds/extractors.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 from typing import Dict, Optional
 
 import ftfy
 import phonenumbers
-from _decimal import Decimal
+from _decimal import Decimal, InvalidOperation
 from lxml import etree
 
 from tedective_etl.schema import ocds
 from tedective_etl.utils import clean, convert_to_euro
 
 
 def extract_title(
@@ -189,29 +189,35 @@
 
 
 def _extract_value(elem: etree._Element, path: str, date) -> Optional[ocds.Value]:
     amount = extract_text(elem, path)
     currency = extract_attribute(elem, path, "CURRENCY")
     amountEur = None
     if amount is not None:
+        amount = amount.strip()
         if currency != "EUR":
             amountEur = convert_to_euro(amount=amount, currency=currency, date=date)
         else:
-            # amount = float(Decimal(amount))
             amountEur = amount
+        try:
+            amount = float(Decimal(amount))
+        except (ValueError, InvalidOperation):
+            return None
         return ocds.Value(
             amount=float(Decimal(amount)),
             currency=ocds.Currency[currency],
             amountEur=amountEur,
         )
     else:
         return None
 
 
-def extract_value(elem: etree._Element, ocds_object: str, date: str = None) -> Optional[ocds.Value]:
+def extract_value(
+    elem: etree._Element, ocds_object: str, date: str = None
+) -> Optional[ocds.Value]:
     # TODO Update currency conversion without re-ingesting all the data
 
     if ocds_object == "tender":
         tender_value_paths = [
             ".//OBJECT_CONTRACT/VAL_ESTIMATED_TOTAL",
         ]
```

### Comparing `tedective_etl-0.1.2/tedective_etl/ted_to_ocds/process.py` & `tedective_etl-0.1.3/tedective_etl/ted_to_ocds/process.py`

 * *Files identical despite different names*

### Comparing `tedective_etl-0.1.2/tedective_etl/ted_to_ocds/transform.py` & `tedective_etl-0.1.3/tedective_etl/ted_to_ocds/transform.py`

 * *Files identical despite different names*

### Comparing `tedective_etl-0.1.2/tedective_etl/utils.py` & `tedective_etl-0.1.3/tedective_etl/utils.py`

 * *Files identical despite different names*

