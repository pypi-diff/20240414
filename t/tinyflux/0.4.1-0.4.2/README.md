# Comparing `tmp/tinyflux-0.4.1.tar.gz` & `tmp/tinyflux-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyflux-0.4.1.tar", last modified: Mon Sep 25 20:37:39 2023, max compression
+gzip compressed data, was "tinyflux-0.4.2.tar", last modified: Sat Apr 13 23:32:48 2024, max compression
```

## Comparing `tinyflux-0.4.1.tar` & `tinyflux-0.4.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 20:37:39.945076 tinyflux-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-09-25 20:37:29.000000 tinyflux-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-09-25 20:37:29.000000 tinyflux-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8325 2023-09-25 20:37:39.945076 tinyflux-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6900 2023-09-25 20:37:29.000000 tinyflux-0.4.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-09-25 20:37:29.000000 tinyflux-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2023-09-25 20:37:39.945076 tinyflux-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 20:37:39.941076 tinyflux-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2023-09-25 20:37:29.000000 tinyflux-0.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2023-09-25 20:37:29.000000 tinyflux-0.4.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13758 2023-09-25 20:37:29.000000 tinyflux-0.4.1/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    25122 2023-09-25 20:37:29.000000 tinyflux-0.4.1/tests/test_measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)    11192 2023-09-25 20:37:29.000000 tinyflux-0.4.1/tests/test_point.py
--rw-r--r--   0 runner    (1001) docker     (127)    26679 2023-09-25 20:37:29.000000 tinyflux-0.4.1/tests/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)    19418 2023-09-25 20:37:29.000000 tinyflux-0.4.1/tests/test_storages.py
--rw-r--r--   0 runner    (1001) docker     (127)    35552 2023-09-25 20:37:29.000000 tinyflux-0.4.1/tests/test_tinyflux.py
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2023-09-25 20:37:29.000000 tinyflux-0.4.1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 20:37:39.945076 tinyflux-0.4.1/tinyflux/
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2023-09-25 20:37:29.000000 tinyflux-0.4.1/tinyflux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50550 2023-09-25 20:37:29.000000 tinyflux-0.4.1/tinyflux/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    28450 2023-09-25 20:37:29.000000 tinyflux-0.4.1/tinyflux/index.py
--rw-r--r--   0 runner    (1001) docker     (127)    11618 2023-09-25 20:37:29.000000 tinyflux-0.4.1/tinyflux/measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)    11548 2023-09-25 20:37:29.000000 tinyflux-0.4.1/tinyflux/point.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-25 20:37:29.000000 tinyflux-0.4.1/tinyflux/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    26609 2023-09-25 20:37:29.000000 tinyflux-0.4.1/tinyflux/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)    15958 2023-09-25 20:37:29.000000 tinyflux-0.4.1/tinyflux/storages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2023-09-25 20:37:29.000000 tinyflux-0.4.1/tinyflux/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 20:37:39.945076 tinyflux-0.4.1/tinyflux.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8325 2023-09-25 20:37:39.000000 tinyflux-0.4.1/tinyflux.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      564 2023-09-25 20:37:39.000000 tinyflux-0.4.1/tinyflux.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 20:37:39.000000 tinyflux-0.4.1/tinyflux.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-09-25 20:37:39.000000 tinyflux-0.4.1/tinyflux.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-09-25 20:37:32.000000 tinyflux-0.4.1/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:32:48.214458 tinyflux-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-13 23:32:40.000000 tinyflux-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-13 23:32:40.000000 tinyflux-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-04-13 23:32:48.214458 tinyflux-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-04-13 23:32:40.000000 tinyflux-0.4.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-13 23:32:40.000000 tinyflux-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-13 23:32:48.214458 tinyflux-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:32:48.210458 tinyflux-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-13 23:32:40.000000 tinyflux-0.4.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-13 23:32:40.000000 tinyflux-0.4.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13761 2024-04-13 23:32:40.000000 tinyflux-0.4.2/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25125 2024-04-13 23:32:40.000000 tinyflux-0.4.2/tests/test_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-04-13 23:32:40.000000 tinyflux-0.4.2/tests/test_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26680 2024-04-13 23:32:40.000000 tinyflux-0.4.2/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19424 2024-04-13 23:32:40.000000 tinyflux-0.4.2/tests/test_storages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35554 2024-04-13 23:32:40.000000 tinyflux-0.4.2/tests/test_tinyflux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-13 23:32:40.000000 tinyflux-0.4.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:32:48.210458 tinyflux-0.4.2/tinyflux/
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-13 23:32:40.000000 tinyflux-0.4.2/tinyflux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50551 2024-04-13 23:32:40.000000 tinyflux-0.4.2/tinyflux/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28446 2024-04-13 23:32:40.000000 tinyflux-0.4.2/tinyflux/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11619 2024-04-13 23:32:40.000000 tinyflux-0.4.2/tinyflux/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11547 2024-04-13 23:32:40.000000 tinyflux-0.4.2/tinyflux/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 23:32:40.000000 tinyflux-0.4.2/tinyflux/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    26616 2024-04-13 23:32:40.000000 tinyflux-0.4.2/tinyflux/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15961 2024-04-13 23:32:40.000000 tinyflux-0.4.2/tinyflux/storages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-13 23:32:40.000000 tinyflux-0.4.2/tinyflux/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-13 23:32:40.000000 tinyflux-0.4.2/tinyflux/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:32:48.214458 tinyflux-0.4.2/tinyflux.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-04-13 23:32:48.000000 tinyflux-0.4.2/tinyflux.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-13 23:32:48.000000 tinyflux-0.4.2/tinyflux.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 23:32:48.000000 tinyflux-0.4.2/tinyflux.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 23:32:48.000000 tinyflux-0.4.2/tinyflux.egg-info/top_level.txt
```

### Comparing `tinyflux-0.4.1/LICENSE` & `tinyflux-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyflux-0.4.1/PKG-INFO` & `tinyflux-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyflux
-Version: 0.4.1
+Version: 0.4.2
 Summary: The Tiny Time-Series Database Optimized for Your Happiness
 Home-page: https://github.com/citrusvanilla/tinyflux
 Author: Justin Fung
 Author-email: justincaseyfung@gmail.com
 Project-URL: Documentation, https://tinyflux.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -35,15 +35,15 @@
     :width: 500px
    
 .. image:: https://github.com/citrusvanilla/tinyflux/blob/master/artwork/tinyfluxdb-dark.png?raw=true#gh-light-mode-only
     :width: 500px
 
 TinyFlux is the tiny time series database optimized for your happiness :)
 
-TinyFlux is a time series version of `TinyDB <https://tinydb.readthedocs.io/en/latest/index.html>`__ that is also written in Python and has no external dependencies.  It's a great companion for small analytics workflows and apps, as well as at-home IOT data stores.  TinyFlux has 100% coverage, tens of thousands of downloads, and no open issues.
+TinyFlux is a time series version of `TinyDB <https://tinydb.readthedocs.io/en/latest/index.html>`__ that is also written in Python and has no external dependencies.  It's a great companion for small analytics workflows and apps, as well as at-home IOT data stores.  TinyFlux has 100% test coverage, over 50,000 downloads, and no open issues.
 
 |Build Status| |Coverage| |Version| |Downloads|
 
 
 Quick Links
 ***********
```

### Comparing `tinyflux-0.4.1/README.rst` & `tinyflux-0.4.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     :width: 500px
    
 .. image:: https://github.com/citrusvanilla/tinyflux/blob/master/artwork/tinyfluxdb-dark.png?raw=true#gh-light-mode-only
     :width: 500px
 
 TinyFlux is the tiny time series database optimized for your happiness :)
 
-TinyFlux is a time series version of `TinyDB <https://tinydb.readthedocs.io/en/latest/index.html>`__ that is also written in Python and has no external dependencies.  It's a great companion for small analytics workflows and apps, as well as at-home IOT data stores.  TinyFlux has 100% coverage, tens of thousands of downloads, and no open issues.
+TinyFlux is a time series version of `TinyDB <https://tinydb.readthedocs.io/en/latest/index.html>`__ that is also written in Python and has no external dependencies.  It's a great companion for small analytics workflows and apps, as well as at-home IOT data stores.  TinyFlux has 100% test coverage, over 50,000 downloads, and no open issues.
 
 |Build Status| |Coverage| |Version| |Downloads|
 
 
 Quick Links
 ***********
```

### Comparing `tinyflux-0.4.1/setup.cfg` & `tinyflux-0.4.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 	.git,
 	__pycache__,
 	docs/**
 extend-ignore = E203
 
 [metadata]
 name = tinyflux
-version = file: version.txt
+version = attr: tinyflux.version.__version__
 author = Justin Fung
 author_email = justincaseyfung@gmail.com
 description = The Tiny Time-Series Database Optimized for Your Happiness
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/citrusvanilla/tinyflux
 project_urls =
```

### Comparing `tinyflux-0.4.1/tests/conftest.py` & `tinyflux-0.4.2/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """PyTest configuration and test fixtures."""
+
 import pytest
 
 from tinyflux.storages import CSVStorage, MemoryStorage
 
 
 class CSVStorageWithCounters(CSVStorage):  # pragma: no cover
     """CSVStorage with some counters for read/write/append ops."""
```

### Comparing `tinyflux-0.4.1/tests/test_index.py` & `tinyflux-0.4.2/tests/test_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for tinyflux.index module."""
+
 from datetime import datetime, timezone, timedelta
 import pytest
 
 from tinyflux import Point, FieldQuery, TagQuery, MeasurementQuery, TimeQuery
 from tinyflux.index import Index
 
 
@@ -114,15 +115,15 @@
     assert index._timestamps == [t1.timestamp()]
 
     t2 = datetime.now(timezone.utc)
     index._insert_time(t2)
     assert index._timestamps == [t1.timestamp(), t2.timestamp()]
 
 
-def test_index_measuments_method():
+def test_index_measurements_method():
     """Test _insert_measurements helper of Index."""
     index = Index()
 
     index._insert_measurements(0, "_default")
     assert index._measurements == {"_default": [0]}
 
     index._insert_measurements(1, "cities")
@@ -377,15 +378,15 @@
     assert rst.items == {0, 1}
 
     # Field query. Note for Field Queries, a NOT operator means we have to
     # check every single item in the storage layer.
     rst = index.search(~fiel_q)
     assert rst.items == {0, 1}
 
-    # Compount NOT FieldQuery.
+    # Compound NOT FieldQuery.
     rst = index.search(~fiel_q & tags_q)
     assert rst.items == {0}
 
     # Time query.
     rst = index.search(~time_q)
     assert rst.items == {0}
```

### Comparing `tinyflux-0.4.1/tests/test_measurement.py` & `tinyflux-0.4.2/tests/test_measurement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Tests for the tinyflux.measurement module.
 
 Tests are generally organized by Measurement class method.
 """
+
 from datetime import datetime, timezone, timedelta
 import re
 from typing import Generator
 
 import pytest
 
 from tinyflux import Point
@@ -39,15 +40,15 @@
         assert isinstance(p, Point)
         assert p.measurement == m._name
 
     assert len(m.all()) == 1
 
 
 def test_len():
-    """Test __len__ of Measuremnt."""
+    """Test __len__ of Measurement."""
     db = TinyFlux(storage=MemoryStorage)
     m = db.measurement("a")
     assert len(m) == 0
 
     # Insert point.
     m.insert(Point())
     assert m.index.valid and len(m.index) == 1
@@ -464,15 +465,15 @@
     assert m1.insert(p1) == 1
     assert db.index.valid and not db.index.empty
     assert len(db.index) == 1
     assert len(db) == 1
     assert len(m1) == 1
     assert len(m2) == 0
 
-    # Insert in-order, into a different measurment.
+    # Insert in-order, into a different measurement.
     assert m2.insert(p2) == 1
     assert db.index.valid and not db.index.empty
     assert len(db.index) == 2
     assert len(db) == 2
     assert len(m1) == 1
     assert len(m2) == 1
```

### Comparing `tinyflux-0.4.1/tests/test_point.py` & `tinyflux-0.4.2/tests/test_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for the tinyflux.point module."""
+
 from datetime import datetime, timezone, timedelta
 import pytest
 from tinyflux.point import Point, validate_tags, validate_fields
 
 
 def test_repr():
     """Test the repr method of Point class."""
@@ -280,15 +281,15 @@
     assert p2 != p3
     assert p1 != {}
     assert p2 != {}
     assert p3 != {}
 
 
 def test_serialize_point():
-    """Test serializaiton of a Point object."""
+    """Test serialization of a Point object."""
     time_now = datetime.now(timezone.utc)
     time_now_str = time_now.replace(tzinfo=None).isoformat()
 
     p1 = Point(
         time=time_now,
         tags={"city": "nyc"},
         fields={"temp_f": 30.1},
```

### Comparing `tinyflux-0.4.1/tests/test_queries.py` & `tinyflux-0.4.2/tests/test_queries.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for the tinyflux.queries module."""
+
 import operator
 from datetime import datetime, timezone, timedelta
 from itertools import combinations
 
 import pytest
 
 from tinyflux import Point
@@ -71,15 +72,15 @@
     assert repr(c3) == rc3
     assert repr(c4) == rc4
     assert repr(c5) == rc5
     assert repr(c6) == rc6
 
 
 def test_no_path():
-    """Test absense of path for Tag and Field queries.
+    """Test absence of path for Tag and Field queries.
 
     TagQuery and FieldQuery should have paths.
     """
     for q in (TagQuery, FieldQuery):
         with pytest.raises(RuntimeError):
             _ = q() == "some_value"
 
@@ -222,15 +223,15 @@
 
 
 def test_lt():
     """Test simple less than comparison."""
     # Test for tag key "city".
     taq_q = TagQuery().city < "melbourne"
     assert taq_q(Point(tags={"city": "amsterdam"}))
-    assert not taq_q(Point(tags={"city": "zansibar"}))
+    assert not taq_q(Point(tags={"city": "zanzibar"}))
     assert not taq_q(Point())
     assert hash(taq_q)
 
     # Test for field key "temperature".
     field_q = FieldQuery().temperature < 70.0
     assert field_q(Point(fields={"temperature": 69.0}))
     assert not field_q(Point(fields={"temperature": 70.0}))
@@ -254,15 +255,15 @@
 
 
 def test_le():
     """Test simple less than or equal to comparison."""
     # Test for tag key "city".
     taq_q = TagQuery().city <= "melbourne"
     assert taq_q(Point(tags={"city": "melbourne"}))
-    assert not taq_q(Point(tags={"city": "zansibar"}))
+    assert not taq_q(Point(tags={"city": "zanzibar"}))
     assert not taq_q(Point())
     assert hash(taq_q)
 
     # Test for field key "temperature".
     field_q = FieldQuery().temperature <= 70.0
     assert field_q(Point(fields={"temperature": 70.0}))
     assert not field_q(Point(fields={"temperature": 71.0}))
@@ -285,15 +286,15 @@
     assert hash(time_q)
 
 
 def test_gt():
     """Test simple greater than comparison."""
     # Test for tag key "city".
     taq_q = TagQuery().city > "melbourne"
-    assert taq_q(Point(tags={"city": "zansibar"}))
+    assert taq_q(Point(tags={"city": "zanzibar"}))
     assert not taq_q(Point(tags={"city": "amsterdam"}))
     assert not taq_q(Point())
     assert hash(taq_q)
 
     # Test for field key "temperature".
     field_q = FieldQuery().temperature > 70.0
     assert field_q(Point(fields={"temperature": 71.0}))
```

### Comparing `tinyflux-0.4.1/tests/test_storages.py` & `tinyflux-0.4.2/tests/test_storages.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for the tinyflux.storages module."""
+
 import csv
 from datetime import datetime, timezone, timedelta
 import os
 import random
 import re
 import tempfile
 from typing import Any
@@ -98,15 +99,15 @@
 
     # Verify contents
     assert [p] == storage.read()
     storage.close()
 
 
 def test_csv_kwargs(tmpdir):
-    """Test kwargs propogation."""
+    """Test kwargs propagation."""
     dbfile = os.path.join(tmpdir, "test.csv")
 
     # Pass the 'delimiter' kwarg from csv module.
     db = TinyFlux(str(dbfile), delimiter="|")
 
     # Write contents.
     p1 = Point(
@@ -129,17 +130,17 @@
 
 
 def test_create_dirs():
     """Test creation of directories for DB path."""
     temp_dir = tempfile.gettempdir()
 
     while True:
-        dname = os.path.join(temp_dir, str(random.getrandbits(20)))
-        if not os.path.exists(dname):
-            dbdir = dname
+        dbname = os.path.join(temp_dir, str(random.getrandbits(20)))
+        if not os.path.exists(dbname):
+            dbdir = dbname
             dbfile = os.path.join(dbdir, "db.json")
             break
 
     with pytest.raises(IOError):
         CSVStorage(dbfile)
 
     CSVStorage(dbfile, create_dirs=True).close()
@@ -359,15 +360,15 @@
     storage = csv_storage_with_counters(path)
     assert storage.reindex_count == 0
 
     # Append a point.  No reads should be performed.
     storage.append([storage._serialize_point(p3)])
     assert storage.reindex_count == 0
 
-    # Read without reindexing.
+    # Read without re-indexing.
     assert storage.read() == [p2, p1, p3]
     assert storage.reindex_count == 0
     assert storage.write_count == 0
 
     storage.close()
 
     # Connect to empty CSV.
@@ -437,15 +438,15 @@
 
     # Insert a point from a previous time.
     storage.append([p3])
     assert storage.append_count == 3
     assert storage.reindex_count == 0
     assert storage.write_count == 0
 
-    # Read contents with reindexing.
+    # Read contents with re-indexing.
     storage.read()
     assert storage.append_count == 3
     assert storage.reindex_count == 0
     assert storage.write_count == 0
 
 
 def test_multiple_appends(
```

### Comparing `tinyflux-0.4.1/tests/test_tinyflux.py` & `tinyflux-0.4.2/tests/test_tinyflux.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Tests for the tinyflux.database module.
 
 Tests are generally organized by TinyFlux class method.
 """
+
 import csv
 from datetime import datetime, timezone, timedelta
 import os
 from pathlib import Path
 import re
 
 import pytest
@@ -621,15 +622,15 @@
 def test_measurement():
     """Test measurement method."""
     # Empty db.  No actual measurements, no Measurement references.
     db = TinyFlux(storage=MemoryStorage)
     assert not db._measurements
     assert not db.get_measurements()
 
-    # Create a reference to a measurment that does not exist.
+    # Create a reference to a measurement that does not exist.
     m = db.measurement("a")
     assert "a" in db._measurements
     assert not len(m)
     assert not db.get_measurements()
 
     # Add a point to the db.
     db.insert(Point())
```

### Comparing `tinyflux-0.4.1/tests/test_utils.py` & `tinyflux-0.4.2/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for tinyflux.utils module."""
+
 import pytest
 
 from tinyflux.utils import (
     freeze,
     FrozenDict,
     find_eq,
     find_ge,
@@ -31,15 +32,15 @@
         frozen[3].pop("a")
 
     with pytest.raises(TypeError):
         frozen[3].update({"a": 9})
 
 
 def test_frozen_dict_hash():
-    """Tesh the hash function on FrozenDict class."""
+    """Test the hash function on FrozenDict class."""
     my_frozen_set1 = FrozenDict({"city": "la", "state": "ca"})
     my_frozen_set2 = FrozenDict({"state": "ca", "city": "la"})
     my_frozen_set3 = FrozenDict({"temp": 70})
 
     assert hash(my_frozen_set1) == hash(my_frozen_set2)
     assert hash(my_frozen_set1) != hash(my_frozen_set3)
     assert hash(my_frozen_set2) != hash(my_frozen_set3)
```

### Comparing `tinyflux-0.4.1/tinyflux/__init__.py` & `tinyflux-0.4.2/tinyflux/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     ...     fields={"aqi": 112}
     ... )
     >>> db.insert(p)
     >>> q1 = TimeQuery() >= datetime.fromisoformat("2020-01-01T00:00:00-00:00")
     >>> q2 = FieldQuery().aqi > 100
     >>> hazardous_days_in_LA_2020 = db.search(q1 & q2)
 """
+
 from .database import TinyFlux
 from .point import Point
 from .queries import TagQuery, FieldQuery, MeasurementQuery, TimeQuery
 
 __all__ = [
     "TinyFlux",
     "Point",
```

### Comparing `tinyflux-0.4.1/tinyflux/database.py` & `tinyflux-0.4.2/tinyflux/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The main module of the TinyFlux package, containing the TinyFlux class."""
+
 import copy
 from datetime import datetime, timezone
 from functools import wraps
 from typing import (
     Any,
     Callable,
     Dict,
@@ -160,15 +161,15 @@
         efficient querying.
 
         Please note, this operation can take some time.  If you need to insert
         into TinyFlux immediately after initializing the DB, set
         'auto-index' to False.
 
         Args:
-            auto_index: Reindexing of data will be performed automatically.
+            auto_index: Re-indexing of data will be performed automatically.
             storage: Class of Storage instance.
         """
         self._auto_index = auto_index
 
         # Init storage.
         storage = kwargs.pop("storage", self.default_storage_class)
         self._storage = storage(*args, **kwargs)
@@ -209,15 +210,15 @@
         """Close the storage instance when leaving a context."""
         if self._open:
             self.close()
 
         return
 
     def __iter__(self) -> Iterator[Point]:
-        """Return an iterater for all Points in the storage layer."""
+        """Return an iterator for all Points in the storage layer."""
         for item in self._storage:
             yield self._storage._deserialize_storage_item(item)
 
     def __len__(self) -> int:
         """Get the number of Points in the storage layer."""
         # If the index is valid, check it.
         if self._auto_index and self._index.valid:
@@ -683,15 +684,15 @@
             measurement: An optional measurement to filter by.
             compact_key_prefixes: Use compact key prefixes in relevant storages.
 
         Returns:
             1 if success.
 
         Raises:
-            OSError if storage cannot be appendex to.
+            OSError if storage cannot be appended to.
             TypeError if point is not a Point instance.
         """
         return self._insert_helper([point], measurement, compact_key_prefixes)
 
     @append_op
     def insert_multiple(
         self,
@@ -706,15 +707,15 @@
             measurement: An optional measurement to insert Points into.
             compact_key_prefixes: Use compact key prefixes in relevant storages.
 
         Returns:
             The count of inserted points.
 
         Raises:
-            OSError if storage cannot be appendex to.
+            OSError if storage cannot be appended to.
             TypeError if point is not a Point instance.
         """
         return self._insert_helper(points, measurement, compact_key_prefixes)
 
     def measurement(self, name: str, **kwargs: Any) -> Measurement:
         """Return a reference to a measurement in this database.
 
@@ -892,15 +893,15 @@
         self,
         select_keys: Union[str, Iterable[str]],
         query: Query,
         measurement: Optional[str] = None,
     ) -> List[Union[Any, Tuple[Any, ...]]]:
         """Get specified attributes from Points specified by a query.
 
-        'select_keys' should be an iterable of attributres including 'time',
+        'select_keys' should be an iterable of attributes including 'time',
         'measurement', and tag keys and tag values.  Passing 'tags' or 'fields'
         in the 'select_keys' iterable will not retrieve all tag and/or field
         values.  Tag and field keys must be specified individually.
 
         Args:
             select_keys: A Point attribute or iterable of Point attributes.
             query: A Query.
```

### Comparing `tinyflux-0.4.1/tinyflux/index.py` & `tinyflux-0.4.2/tinyflux/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,46 +1,47 @@
-"""Defintion of the TinyFlux Index.
+"""Definition of the TinyFlux Index.
 
 Class descriptions for Index and IndexResult.  An Index acts like a singleton,
 and is initialized at creation time with the TinyFlux instance. It provides
 efficient in-memory data structures and getters for TinyFlux operations. An
 Index instance is not a part of the TinyFlux interface.
 
-An IndexResult returns the indicies of revelant TinyFlux queries for further
+An IndexResult returns the indices of relevant TinyFlux queries for further
 handling, usually as an input to a storage retrieval.
 """
+
 from datetime import datetime, timezone
 import operator
 from typing import Dict, Iterable, List, Optional, Set, Tuple, Union
 
 from tinyflux.queries import SimpleQuery, CompoundQuery, Query
 from .point import FieldSet, FieldValue, Point, TagSet
 from .utils import find_eq, find_lt, find_le, find_gt, find_ge
 
 
 class IndexResult:
-    """Returns indicies of TinyFlux queries that are handled by an Index.
+    """Returns indices of TinyFlux queries that are handled by an Index.
 
     IndexResults instances are generated by an Index.
 
-    Arritributes:
-        items: A set of indicies as ints.
+    Attributes:
+        items: A set of indices as ints.
 
     Usage:
         >>> IndexResult(items=set(), index_count=0)
     """
 
     _items: Set[int]
     _index_count: int
 
     def __init__(self, items: Set[int], index_count: int):
         """Init IndexResult.
 
         Args:
-            items: Matching items from a query as indicies.
+            items: Matching items from a query as indices.
             index_count: Number of items in the index..
         """
         self._items = items
         self._index_count = index_count
 
     @property
     def items(self) -> Set[int]:
```

### Comparing `tinyflux-0.4.1/tinyflux/measurement.py` & `tinyflux-0.4.2/tinyflux/measurement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-"""Defintion of TinyFlux measurement class.
+"""Definition of TinyFlux measurement class.
 
 The measurement class provides a convenient interface into a subset of
 data points with a common measurement name.  A measurement is analogous to a
 table in a traditional RDBMS.
 
 Usage:
     >>> db = TinyFlux(storage=MemoryStorage)
     >>> m = db.measurement("my_measurement")
 """
+
 from __future__ import annotations
 
 from datetime import datetime
 from typing import (
     Callable,
     Dict,
     Iterable,
@@ -294,15 +295,15 @@
     def select(
         self,
         keys: Union[str, Iterable[str]],
         query: Query,
     ) -> List[Tuple[Union[datetime, str, int, float, None]]]:
         """Get specified attributes from Points specified by a query.
 
-        'keys' should be an iterable of attributres including 'time',
+        'keys' should be an iterable of attributes including 'time',
         'measurement', and tag keys and tag values.  Passing 'tags' or 'fields'
         in the 'keys' iterable will not retrieve all tag and/or field values.
         Tag and field keys must be specified individually.
 
         Args:
             keys: An iterable of Point attributes.
             query: A Query.
```

### Comparing `tinyflux-0.4.1/tinyflux/point.py` & `tinyflux-0.4.2/tinyflux/point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-"""Defintion of the TinyFlux Point class.
+"""Definition of the TinyFlux Point class.
 
 A Point is the data type upon which TinyFlux manages.  It contains the time
 data and metadata for an individual observation.  Points are serialized and
-deserialized from Storage.  SimpleQuerys act upon individual Points.
+deserialized from Storage. SimpleQuery act upon individual Points.
 
 A Point is comprised of a timestamp, a measurement, fields, and tags.
 
 Fields contains string/numeric key-values, while tags contain
 string/string key-values.  This is enforced upon Point instantiation.
 
 Usage:
```

### Comparing `tinyflux-0.4.1/tinyflux/queries.py` & `tinyflux-0.4.2/tinyflux/queries.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-"""Defintion of TinyFlux Queries.
+"""Definition of TinyFlux Queries.
 
 A query contains logic in the form of a test and it acts upon a single Point
 when it is eventually evaluated.
 
 All Queries begin as subclass of BaseQuery, which is not itself callable. Logic
 for the query is handled by the Python data model of the BaseQuery class,
 resulting in the generation of a SimpleQuery, which is callable. SimpleQuery
 instances support logical AND, OR, and NOT operations, which result in the
 initialization of a new CompoundQuery object.
 
 Each SimpleQuery instance contains attributes that constitute the
-"deconstuction" of a query into several key parts (e.g. the operator, the
-right-hand side) so that the other consumers of queries, includng an Index, may
+"deconstruction" of a query into several key parts (e.g. the operator, the
+right-hand side) so that the other consumers of queries, including an Index, may
 use them for their own purposes.
 """
+
 from datetime import datetime
 import operator
 import re
 from typing import (
     Any,
     Callable,
     Mapping,
@@ -210,15 +211,15 @@
         """Initialize an SimpleQuery.
 
         Args:
             point_attr: The attribute of a Point relevant for this query.
             operator: The operator portion of a test.
             rhs: The value that a test should evaluated against.
             test: The combined logic as a callable.
-            path_resolver: A fetcher/translater for Point metadata that the
+            path_resolver: A fetcher/translator for Point metadata that the
                            query will be evaluated on.
             hashval: The hash value for the query.
         """
         self._point_attr = point_attr
         self._operator = operator
         self._rhs = rhs
         self._test = test
@@ -319,18 +320,18 @@
         """Return the ability to hash this query."""
         return self._hash is not None
 
 
 class BaseQuery:
     """A base class for the different TinyFlux query types.
 
-    A query type that explicity unifies the divergent interfaces of TimeQuery,
+    A query type that explicitly unifies the divergent interfaces of TimeQuery,
     MeasurementQuery, TagQuery, and FieldQuery.
 
-    A BaseQuery is not iteslf callable. When it is combined with test logic,
+    A BaseQuery is not itself callable. When it is combined with test logic,
     it generates a SimpleQuery, which is callable without exception.
 
     Usage:
         >>> from tinyflux import TagQuery, Point
         >>> p = Point(tags={"city": "LA"})
         >>> q1 = TagQuery()
         >>> isinstance(q1, tinyflux.queries.BaseQuery)
@@ -417,15 +418,15 @@
         """Generate a SimpleQuery and its components.
 
         A helper function for a BaseQuery instance.
 
         Args:
             operator: A Callable.
             rhs: A value to test against.
-            test_against_rhs: Whether the test should evaulate against RHS.
+            test_against_rhs: Whether the test should evaluate against RHS.
             hashval: The hash value for the query.
         """
         # Make sure this query has some keys if they are required.
         if self._path_required and not self._path:
             raise RuntimeError(
                 "Query has no path. Provide tag or field key to query."
             )
@@ -464,15 +465,15 @@
             self._point_attr == "_fields"
             and rhs
             and not isinstance(rhs, (int, float))
         ):
             raise TypeError("FieldQuery comparison value must be numeric.")
 
         def test(x: Any) -> bool:
-            """The test function from an operator and righthand side."""
+            """The test function from an operator and right-hand side."""
             if not test_against_rhs:
                 return operator(x, *args) if args else operator(x)
 
             # Wrap this in a try/except block.
             # Some operators do not work against None types.
             # They should evaluate to False.
             try:
@@ -651,15 +652,15 @@
 
         >>> def test_func(val):
         ...     return val == 42
         ...
         >>> FieldQuery()["my field"].test(test_func)
 
         Warning:
-            The test fuction provided needs to be deterministic (returning the
+            The test function provided needs to be deterministic (returning the
             same value when provided with the same arguments), otherwise this
             may mess up the query cache that :class:`~tinyflux.table.Table`
             implements.
 
         Args:
             func: The function to call, passing the value as the first arg.
             args: Additional arguments to pass to the test function.
```

### Comparing `tinyflux-0.4.1/tinyflux/storages.py` & `tinyflux-0.4.2/tinyflux/storages.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-"""Defintion of TinyFlux storages classes.
+"""Definition of TinyFlux storages classes.
 
 Storage defines an abstract base case using the built-in ABC of python. This
 class defines the requires abstract methods of read, write, and append, as well
 as getters and setters for attributes required to reindex the data.
 
 A storage object will manage data with a file handle, or in memory.
 
 A storage class is provided to the TinyFlux facade as an initial argument.  The
 TinyFlux instance will manage the lifecycle of the storage instance.
 
 Usage:
     >>> my_mem_db = TinyFlux(storage=MemoryStorage)
     >>> my_csv_db = TinyFlux('path/to/my.csv', storage=CSVStorage)
 """
+
 from abc import ABC, abstractmethod
 import csv
 from datetime import datetime
 import os
 from pathlib import Path
 import shutil
 from tempfile import NamedTemporaryFile
@@ -54,15 +55,15 @@
 
 class Storage(ABC):  # pragma: no cover
     """The abstract base class for all storage types for TinyFlux.
 
     Defines an extensible, static interface with required read/write ops and
     index-related getter/setters.
 
-    Custom storage classes should inheret like so:
+    Custom storage classes should inherit like so:
         >>> from tinyflux import Storage
         >>> class MyStorageClass(Storage):
                 ...
     """
 
     _initially_empty: bool
 
@@ -92,15 +93,15 @@
         ...
 
     @abstractmethod
     def append(self, points: List[Any], temporary: bool = False) -> None:
         """Append points to the store.
 
         Args:
-            points: A list of Point objets.
+            points: A list of Point objects.
             temporary: Whether or not to append to temporary storage.
         """
         ...
 
     def close(self) -> None:
         """Perform clean up ops."""
         ...
```

### Comparing `tinyflux-0.4.1/tinyflux/utils.py` & `tinyflux-0.4.2/tinyflux/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""Defintion of TinyFlux utils."""
+"""Definition of TinyFlux utils."""
+
 import bisect
 from typing import Any, List, Optional
 
 
 class FrozenDict(dict):
     """
     An immutable dictionary.
```

### Comparing `tinyflux-0.4.1/tinyflux.egg-info/PKG-INFO` & `tinyflux-0.4.2/tinyflux.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyflux
-Version: 0.4.1
+Version: 0.4.2
 Summary: The Tiny Time-Series Database Optimized for Your Happiness
 Home-page: https://github.com/citrusvanilla/tinyflux
 Author: Justin Fung
 Author-email: justincaseyfung@gmail.com
 Project-URL: Documentation, https://tinyflux.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -35,15 +35,15 @@
     :width: 500px
    
 .. image:: https://github.com/citrusvanilla/tinyflux/blob/master/artwork/tinyfluxdb-dark.png?raw=true#gh-light-mode-only
     :width: 500px
 
 TinyFlux is the tiny time series database optimized for your happiness :)
 
-TinyFlux is a time series version of `TinyDB <https://tinydb.readthedocs.io/en/latest/index.html>`__ that is also written in Python and has no external dependencies.  It's a great companion for small analytics workflows and apps, as well as at-home IOT data stores.  TinyFlux has 100% coverage, tens of thousands of downloads, and no open issues.
+TinyFlux is a time series version of `TinyDB <https://tinydb.readthedocs.io/en/latest/index.html>`__ that is also written in Python and has no external dependencies.  It's a great companion for small analytics workflows and apps, as well as at-home IOT data stores.  TinyFlux has 100% test coverage, over 50,000 downloads, and no open issues.
 
 |Build Status| |Coverage| |Version| |Downloads|
 
 
 Quick Links
 ***********
```

### Comparing `tinyflux-0.4.1/tinyflux.egg-info/SOURCES.txt` & `tinyflux-0.4.2/tinyflux.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
-version.txt
 tests/__init__.py
 tests/conftest.py
 tests/test_index.py
 tests/test_measurement.py
 tests/test_point.py
 tests/test_queries.py
 tests/test_storages.py
@@ -18,11 +17,12 @@
 tinyflux/index.py
 tinyflux/measurement.py
 tinyflux/point.py
 tinyflux/py.typed
 tinyflux/queries.py
 tinyflux/storages.py
 tinyflux/utils.py
+tinyflux/version.py
 tinyflux.egg-info/PKG-INFO
 tinyflux.egg-info/SOURCES.txt
 tinyflux.egg-info/dependency_links.txt
 tinyflux.egg-info/top_level.txt
```

