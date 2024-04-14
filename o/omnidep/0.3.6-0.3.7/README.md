# Comparing `tmp/omnidep-0.3.6.tar.gz` & `tmp/omnidep-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnidep-0.3.6.tar", max compression
+gzip compressed data, was "omnidep-0.3.7.tar", max compression
```

## Comparing `omnidep-0.3.6.tar` & `omnidep-0.3.7.tar`

### file list

```diff
@@ -1,47 +1,60 @@
--rw-r--r--   0        0        0     1069 2022-06-11 17:48:28.000000 omnidep-0.3.6/LICENSE
--rw-r--r--   0        0        0        0 2022-06-11 16:57:02.840000 omnidep-0.3.6/omnidep/__init__.py
--rw-r--r--   0        0        0       90 2023-05-14 16:28:24.000000 omnidep-0.3.6/omnidep/__main__.py
--rw-r--r--   0        0        0     4921 2023-05-13 16:25:24.000000 omnidep-0.3.6/omnidep/command.py
--rw-r--r--   0        0        0     3715 2023-11-19 16:07:54.000000 omnidep-0.3.6/omnidep/errors.py
--rw-r--r--   0        0        0     2142 2023-05-14 15:03:32.000000 omnidep-0.3.6/omnidep/imports.py
--rw-r--r--   0        0        0     1406 2023-05-13 16:25:26.000000 omnidep-0.3.6/omnidep/main.py
--rw-r--r--   0        0        0     3218 2023-07-09 14:48:00.000000 omnidep-0.3.6/omnidep/packages.py
--rw-r--r--   0        0        0     7742 2023-07-09 14:53:40.000000 omnidep-0.3.6/omnidep/project.py
--rw-r--r--   0        0        0        0 2022-11-28 18:05:02.570000 omnidep-0.3.6/omnidep/tst/__init__.py
--rw-r--r--   0        0        0    10260 2023-07-09 14:44:48.000000 omnidep-0.3.6/omnidep/tst/errors_test.py
--rw-r--r--   0        0        0     1504 2022-06-12 12:45:12.000000 omnidep-0.3.6/omnidep/tst/imports_test.py
--rw-r--r--   0        0        0     2602 2022-06-11 17:48:28.000000 omnidep-0.3.6/omnidep/tst/packages_test.py
--rw-r--r--   0        0        0     2636 2023-05-14 15:03:34.000000 omnidep-0.3.6/omnidep/tst/project_test.py
--rw-r--r--   0        0        0      314 2022-10-07 14:23:06.000000 omnidep-0.3.6/omnidep/tst/test_cases/case_insensitive_sorted/pyproject.toml
--rw-r--r--   0        0        0      314 2022-10-07 14:23:06.000000 omnidep-0.3.6/omnidep/tst/test_cases/case_sensitive_sorted/pyproject.toml
--rw-r--r--   0        0        0      273 2023-05-14 15:03:34.000000 omnidep-0.3.6/omnidep/tst/test_cases/dependency_in_test_code/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-08 13:11:17.810000 omnidep-0.3.6/omnidep/tst/test_cases/dependency_in_test_code/tests/__init__.py
--rw-r--r--   0        0        0      398 2023-05-14 15:03:34.000000 omnidep-0.3.6/omnidep/tst/test_cases/dependency_in_test_code/tests/test_code.py
--rw-r--r--   0        0        0      291 2022-11-29 18:45:06.000000 omnidep-0.3.6/omnidep/tst/test_cases/dev_dependencies_new/pyproject.toml
--rw-r--r--   0        0        0      285 2022-11-29 18:45:06.000000 omnidep-0.3.6/omnidep/tst/test_cases/dev_dependencies_old/pyproject.toml
--rw-r--r--   0        0        0     2266 2022-06-11 17:48:28.000000 omnidep-0.3.6/omnidep/tst/test_cases/every_import.py~
--rw-r--r--   0        0        0        0 2023-05-14 15:03:33.360000 omnidep-0.3.6/omnidep/tst/test_cases/failed_import/failed_import/__init__.py
--rw-r--r--   0        0        0      157 2023-05-14 15:03:34.000000 omnidep-0.3.6/omnidep/tst/test_cases/failed_import/failed_import/code.py
--rw-r--r--   0        0        0      218 2023-05-14 15:03:34.000000 omnidep-0.3.6/omnidep/tst/test_cases/failed_import/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 15:03:34.950000 omnidep-0.3.6/omnidep/tst/test_cases/failed_import_but_ignored/failed_import/__init__.py
--rw-r--r--   0        0        0      157 2023-05-14 15:03:36.000000 omnidep-0.3.6/omnidep/tst/test_cases/failed_import_but_ignored/failed_import/code.py
--rw-r--r--   0        0        0      270 2023-05-14 15:03:36.000000 omnidep-0.3.6/omnidep/tst/test_cases/failed_import_but_ignored/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 15:03:35.090000 omnidep-0.3.6/omnidep/tst/test_cases/namespace_none_declared/namespace_code/__init__.py
--rw-r--r--   0        0        0      170 2023-05-14 15:03:36.000000 omnidep-0.3.6/omnidep/tst/test_cases/namespace_none_declared/namespace_code/code.py
--rw-r--r--   0        0        0      219 2023-05-14 15:03:36.000000 omnidep-0.3.6/omnidep/tst/test_cases/namespace_none_declared/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 15:03:35.180000 omnidep-0.3.6/omnidep/tst/test_cases/namespace_one_declared/namespace_code/__init__.py
--rw-r--r--   0        0        0      170 2023-05-14 15:03:36.000000 omnidep-0.3.6/omnidep/tst/test_cases/namespace_one_declared/namespace_code/code.py
--rw-r--r--   0        0        0      244 2023-05-14 15:03:36.000000 omnidep-0.3.6/omnidep/tst/test_cases/namespace_one_declared/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 15:03:35.290000 omnidep-0.3.6/omnidep/tst/test_cases/namespace_three_declared/namespace_code/__init__.py
--rw-r--r--   0        0        0      170 2023-05-14 15:03:36.000000 omnidep-0.3.6/omnidep/tst/test_cases/namespace_three_declared/namespace_code/code.py
--rw-r--r--   0        0        0      309 2023-05-14 15:03:36.000000 omnidep-0.3.6/omnidep/tst/test_cases/namespace_three_declared/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 15:03:35.320000 omnidep-0.3.6/omnidep/tst/test_cases/parent_child_configured/parent_child/__init__.py
--rw-r--r--   0        0        0      237 2023-05-14 15:03:36.000000 omnidep-0.3.6/omnidep/tst/test_cases/parent_child_configured/parent_child/code.py
--rw-r--r--   0        0        0      298 2023-05-14 15:03:36.000000 omnidep-0.3.6/omnidep/tst/test_cases/parent_child_configured/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 15:03:35.390000 omnidep-0.3.6/omnidep/tst/test_cases/parent_child_misconfigured/parent_child/__init__.py
--rw-r--r--   0        0        0      237 2023-05-14 15:03:36.000000 omnidep-0.3.6/omnidep/tst/test_cases/parent_child_misconfigured/parent_child/code.py
--rw-r--r--   0        0        0      367 2023-05-14 15:03:36.000000 omnidep-0.3.6/omnidep/tst/test_cases/parent_child_misconfigured/pyproject.toml
--rw-r--r--   0        0        0      293 2022-10-07 14:23:06.000000 omnidep-0.3.6/omnidep/tst/test_cases/unsorted/pyproject.toml
--rw-r--r--   0        0        0     3151 2023-11-19 16:07:54.000000 omnidep-0.3.6/pyproject.toml
--rw-r--r--   0        0        0    13966 2023-11-19 16:07:54.000000 omnidep-0.3.6/README.rst
--rw-r--r--   0        0        0    14966 1970-01-01 00:00:00.000000 omnidep-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-06-11 17:48:28.000000 omnidep-0.3.7/LICENSE
+-rw-r--r--   0        0        0        0 2022-06-11 16:57:02.840000 omnidep-0.3.7/omnidep/__init__.py
+-rw-r--r--   0        0        0       90 2023-05-14 16:28:24.000000 omnidep-0.3.7/omnidep/__main__.py
+-rw-r--r--   0        0        0     4921 2023-05-13 16:25:24.000000 omnidep-0.3.7/omnidep/command.py
+-rw-r--r--   0        0        0     3715 2024-04-14 14:45:16.000000 omnidep-0.3.7/omnidep/errors.py
+-rw-r--r--   0        0        0     2551 2024-04-14 15:15:24.000000 omnidep-0.3.7/omnidep/imports.py
+-rw-r--r--   0        0        0     1406 2023-05-13 16:25:26.000000 omnidep-0.3.7/omnidep/main.py
+-rw-r--r--   0        0        0     3218 2024-04-14 14:45:16.000000 omnidep-0.3.7/omnidep/packages.py
+-rw-r--r--   0        0        0     7742 2024-04-13 13:25:58.000000 omnidep-0.3.7/omnidep/project.py
+-rw-r--r--   0        0        0        0 2022-11-28 18:05:02.570000 omnidep-0.3.7/omnidep/tst/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-14 15:12:44.000000 omnidep-0.3.7/omnidep/tst/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    31562 2024-04-14 15:12:44.000000 omnidep-0.3.7/omnidep/tst/__pycache__/errors_test.cpython-38-pytest-7.4.4.pyc
+-rw-r--r--   0        0        0     8643 2024-04-14 15:12:44.000000 omnidep-0.3.7/omnidep/tst/__pycache__/imports_test.cpython-38-pytest-7.4.4.pyc
+-rw-r--r--   0        0        0     6957 2024-04-14 15:12:44.000000 omnidep-0.3.7/omnidep/tst/__pycache__/packages_test.cpython-38-pytest-7.4.4.pyc
+-rw-r--r--   0        0        0     6215 2024-04-14 15:12:44.000000 omnidep-0.3.7/omnidep/tst/__pycache__/project_test.cpython-38-pytest-7.4.4.pyc
+-rw-r--r--   0        0        0    10260 2023-07-09 14:44:48.000000 omnidep-0.3.7/omnidep/tst/errors_test.py
+-rw-r--r--   0        0        0     2688 2024-04-14 14:45:38.000000 omnidep-0.3.7/omnidep/tst/imports_test.py
+-rw-r--r--   0        0        0     2602 2022-06-11 17:48:28.000000 omnidep-0.3.7/omnidep/tst/packages_test.py
+-rw-r--r--   0        0        0     2774 2024-04-14 14:45:38.000000 omnidep-0.3.7/omnidep/tst/project_test.py
+-rw-r--r--   0        0        0      314 2022-10-07 14:23:06.000000 omnidep-0.3.7/omnidep/tst/test_cases/case_insensitive_sorted/pyproject.toml
+-rw-r--r--   0        0        0      314 2022-10-07 14:23:06.000000 omnidep-0.3.7/omnidep/tst/test_cases/case_sensitive_sorted/pyproject.toml
+-rw-r--r--   0        0        0      273 2023-05-14 15:03:34.000000 omnidep-0.3.7/omnidep/tst/test_cases/dependency_in_test_code/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-08 13:11:17.810000 omnidep-0.3.7/omnidep/tst/test_cases/dependency_in_test_code/tests/__init__.py
+-rw-r--r--   0        0        0      181 2024-04-14 15:12:44.000000 omnidep-0.3.7/omnidep/tst/test_cases/dependency_in_test_code/tests/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      349 2024-04-14 15:12:44.000000 omnidep-0.3.7/omnidep/tst/test_cases/dependency_in_test_code/tests/__pycache__/test_code.cpython-38-pytest-7.4.4.pyc
+-rw-r--r--   0        0        0      398 2023-05-14 15:03:34.000000 omnidep-0.3.7/omnidep/tst/test_cases/dependency_in_test_code/tests/test_code.py
+-rw-r--r--   0        0        0      291 2022-11-29 18:45:06.000000 omnidep-0.3.7/omnidep/tst/test_cases/dev_dependencies_new/pyproject.toml
+-rw-r--r--   0        0        0      285 2022-11-29 18:45:06.000000 omnidep-0.3.7/omnidep/tst/test_cases/dev_dependencies_old/pyproject.toml
+-rw-r--r--   0        0        0     2266 2022-06-11 17:48:28.000000 omnidep-0.3.7/omnidep/tst/test_cases/every_import.py~
+-rw-r--r--   0        0        0        0 2023-05-14 15:03:33.360000 omnidep-0.3.7/omnidep/tst/test_cases/failed_import/failed_import/__init__.py
+-rw-r--r--   0        0        0      157 2024-04-14 14:45:16.000000 omnidep-0.3.7/omnidep/tst/test_cases/failed_import/failed_import/code.py
+-rw-r--r--   0        0        0      218 2023-05-14 15:03:34.000000 omnidep-0.3.7/omnidep/tst/test_cases/failed_import/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-14 15:03:34.950000 omnidep-0.3.7/omnidep/tst/test_cases/failed_import_but_ignored/failed_import/__init__.py
+-rw-r--r--   0        0        0      157 2024-04-14 14:45:16.000000 omnidep-0.3.7/omnidep/tst/test_cases/failed_import_but_ignored/failed_import/code.py
+-rw-r--r--   0        0        0      270 2023-05-14 15:03:36.000000 omnidep-0.3.7/omnidep/tst/test_cases/failed_import_but_ignored/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-14 15:03:35.090000 omnidep-0.3.7/omnidep/tst/test_cases/namespace_none_declared/namespace_code/__init__.py
+-rw-r--r--   0        0        0      170 2023-05-14 15:03:36.000000 omnidep-0.3.7/omnidep/tst/test_cases/namespace_none_declared/namespace_code/code.py
+-rw-r--r--   0        0        0      219 2023-05-14 15:03:36.000000 omnidep-0.3.7/omnidep/tst/test_cases/namespace_none_declared/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-14 15:03:35.180000 omnidep-0.3.7/omnidep/tst/test_cases/namespace_one_declared/namespace_code/__init__.py
+-rw-r--r--   0        0        0      170 2023-05-14 15:03:36.000000 omnidep-0.3.7/omnidep/tst/test_cases/namespace_one_declared/namespace_code/code.py
+-rw-r--r--   0        0        0      244 2023-05-14 15:03:36.000000 omnidep-0.3.7/omnidep/tst/test_cases/namespace_one_declared/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-14 15:03:35.290000 omnidep-0.3.7/omnidep/tst/test_cases/namespace_three_declared/namespace_code/__init__.py
+-rw-r--r--   0        0        0      170 2023-05-14 15:03:36.000000 omnidep-0.3.7/omnidep/tst/test_cases/namespace_three_declared/namespace_code/code.py
+-rw-r--r--   0        0        0      309 2023-05-14 15:03:36.000000 omnidep-0.3.7/omnidep/tst/test_cases/namespace_three_declared/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-14 15:03:35.320000 omnidep-0.3.7/omnidep/tst/test_cases/parent_child_configured/parent_child/__init__.py
+-rw-r--r--   0        0        0      237 2024-04-14 14:45:16.000000 omnidep-0.3.7/omnidep/tst/test_cases/parent_child_configured/parent_child/code.py
+-rw-r--r--   0        0        0      298 2023-05-14 15:03:36.000000 omnidep-0.3.7/omnidep/tst/test_cases/parent_child_configured/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-14 15:03:35.390000 omnidep-0.3.7/omnidep/tst/test_cases/parent_child_misconfigured/parent_child/__init__.py
+-rw-r--r--   0        0        0      237 2024-04-14 14:45:16.000000 omnidep-0.3.7/omnidep/tst/test_cases/parent_child_misconfigured/parent_child/code.py
+-rw-r--r--   0        0        0      367 2023-05-14 15:03:36.000000 omnidep-0.3.7/omnidep/tst/test_cases/parent_child_misconfigured/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-14 14:48:32.620000 omnidep-0.3.7/omnidep/tst/test_cases/test_filter_hit/filter_code/__init__.py
+-rw-r--r--   0        0        0      137 2024-04-14 14:45:38.000000 omnidep-0.3.7/omnidep/tst/test_cases/test_filter_hit/filter_code/tst_code.py
+-rw-r--r--   0        0        0      330 2024-04-14 14:45:38.000000 omnidep-0.3.7/omnidep/tst/test_cases/test_filter_hit/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-14 14:48:28.050000 omnidep-0.3.7/omnidep/tst/test_cases/test_filter_missed/filter_code/__init__.py
+-rw-r--r--   0        0        0      137 2024-04-14 14:45:38.000000 omnidep-0.3.7/omnidep/tst/test_cases/test_filter_missed/filter_code/tst_code.py
+-rw-r--r--   0        0        0      334 2024-04-14 14:45:38.000000 omnidep-0.3.7/omnidep/tst/test_cases/test_filter_missed/pyproject.toml
+-rw-r--r--   0        0        0      293 2022-10-07 14:23:06.000000 omnidep-0.3.7/omnidep/tst/test_cases/unsorted/pyproject.toml
+-rw-r--r--   0        0        0     3151 2024-04-14 15:08:30.000000 omnidep-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0    14821 2024-04-14 15:25:16.000000 omnidep-0.3.7/README.rst
+-rw-r--r--   0        0        0    15821 1970-01-01 00:00:00.000000 omnidep-0.3.7/PKG-INFO
```

### Comparing `omnidep-0.3.6/LICENSE` & `omnidep-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `omnidep-0.3.6/omnidep/command.py` & `omnidep-0.3.7/omnidep/command.py`

 * *Files identical despite different names*

### Comparing `omnidep-0.3.6/omnidep/errors.py` & `omnidep-0.3.7/omnidep/errors.py`

 * *Files identical despite different names*

### Comparing `omnidep-0.3.6/omnidep/imports.py` & `omnidep-0.3.7/omnidep/imports.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,17 +25,28 @@
             to_process.extend(node)
         elif isinstance(node, ast.AST):
             to_process.extend(getattr(node, name) for name in node._fields)
         elif not isinstance(node, basic_types):
             raise NotImplementedError(f"unhandled {type(node)} {node!r}")
 
 def find_source_files(path: Path) -> Iterable[Path]:
-    if path.is_file() and path.suffix == '.py':
-        return [path]
-    return path.glob('**/*.py')
+    if '*' not in path.name and path.parent.name != '**':
+        if path.is_file() and path.suffix == '.py':
+            return [path]
+        if path.is_dir():
+            return path.rglob('*.py')
+        # Doesn't exist, and not a glob, so no matches
+        return []
+    pattern = path.name
+    parent = path.parent
+    if parent.name == '**':
+        matches = parent.parent.rglob(pattern)
+    else:
+        matches = parent.glob(pattern)
+    return [match for match in matches if match.suffix == '.py']
 
 def iter_modules(path: Path) -> Iterable[str]:
     for file in find_source_files(path):
         with file.open(encoding='utf8') as infile:
             # print(file)
             tree = ast.parse(infile.read())
             yield from iter_import_names(tree)
```

### Comparing `omnidep-0.3.6/omnidep/main.py` & `omnidep-0.3.7/omnidep/main.py`

 * *Files identical despite different names*

### Comparing `omnidep-0.3.6/omnidep/packages.py` & `omnidep-0.3.7/omnidep/packages.py`

 * *Files identical despite different names*

### Comparing `omnidep-0.3.6/omnidep/project.py` & `omnidep-0.3.7/omnidep/project.py`

 * *Files identical despite different names*

### Comparing `omnidep-0.3.6/omnidep/tst/errors_test.py` & `omnidep-0.3.7/omnidep/tst/errors_test.py`

 * *Files identical despite different names*

### Comparing `omnidep-0.3.6/omnidep/tst/imports_test.py` & `omnidep-0.3.7/omnidep/tst/imports_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,15 +9,41 @@
 def test_find_source_files() -> None:
     results = list(imports.find_source_files(test_dir))
     assert Path(__file__) in results
     assert all(path.suffix == '.py' for path in results)
 
 def test_find_source_files_single() -> None:
     this_file = Path(__file__)
-    assert list(imports.find_source_files(this_file)) == [Path(this_file)]
+    # When full file name is specified, must find only that.
+    assert list(imports.find_source_files(this_file)) == [this_file]
+
+def test_find_source_files_glob_hits() -> None:
+    results = list(imports.find_source_files(test_dir/ '*.py'))
+    # When glob is specified, must find multiple files
+    assert Path(__file__) in results
+    assert len(results) > 1
+    assert all(path.suffix == '.py' for path in results)
+
+def test_find_source_files_glob_misses() -> None:
+    results = list(imports.find_source_files(test_dir/ '*errors*.py'))
+    # When restricted glob is specified, must find just the file that matches
+    assert Path(__file__) not in results
+    assert results == [test_dir / 'errors_test.py']
+
+def test_find_source_files_rglob() -> None:
+    results = list(imports.find_source_files(test_dir.parent/ '*.py'))
+    assert Path(__file__) not in results
+    results = list(imports.find_source_files(test_dir.parent/ '**/*.py'))
+    assert Path(__file__) in results
+
+def test_find_source_files_nonpy() -> None:
+    results = list(test_dir.parent.rglob('*'))
+    assert any(file.suffix != '.py' for file in results)
+    results = list(imports.find_source_files(test_dir.parent / '**/*'))
+    assert all(path.suffix == '.py' for path in results)
 
 def test_is_external() -> None:
     assert not imports.is_external('pathlib')
     assert not imports.is_external('__future__')
     assert imports.is_external('omnidep')
     assert imports.is_external('pytest')
     # Not strictly true, but for our purposes
```

### Comparing `omnidep-0.3.6/omnidep/tst/packages_test.py` & `omnidep-0.3.7/omnidep/tst/packages_test.py`

 * *Files identical despite different names*

### Comparing `omnidep-0.3.6/omnidep/tst/project_test.py` & `omnidep-0.3.7/omnidep/tst/project_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,16 @@
     (test_dir / 'test_cases/failed_import', [], [Violation.ODEP002], []),
     (test_dir / 'test_cases/failed_import_but_ignored', [], [], []),
     (test_dir / 'test_cases/namespace_none_declared', [], [Violation.ODEP004], []),
     (test_dir / 'test_cases/namespace_one_declared', [], [Violation.ODEP003], []),
     (test_dir / 'test_cases/namespace_three_declared', [], [], []),
     (test_dir / 'test_cases/parent_child_configured', [], [], []),
     (test_dir / 'test_cases/parent_child_misconfigured', [], [Violation.ODEP001], []),
+    (test_dir / 'test_cases/test_filter_missed', [], [Violation.ODEP001], []),
+    (test_dir / 'test_cases/test_filter_hit', [], [], []),
 ]
 
 def codes(warnings: Iterable[Warn]) -> Codes:
     return [warning.code for warning in warnings]
 
 @pytest.mark.parametrize('projdir,expected,main,dev', plain_project_files)
 def test_known_project_files(projdir: Path, expected: Codes, main: Codes, dev: Codes) -> None:
```

### Comparing `omnidep-0.3.6/omnidep/tst/test_cases/every_import.py~` & `omnidep-0.3.7/omnidep/tst/test_cases/every_import.py~`

 * *Files identical despite different names*

### Comparing `omnidep-0.3.6/pyproject.toml` & `omnidep-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omnidep"
-version = "0.3.6"
+version = "0.3.7"
 description = "Linter to compare project dependencies against imports in source code"
 readme = "README.rst"
 authors = ["Steve Jessop <68118527+sjjessop@users.noreply.github.com>"]
 license = "MIT"
 homepage = "https://github.com/sjjessop/omnidep"
 packages = [{ include = "omnidep" }]
```

### Comparing `omnidep-0.3.6/README.rst` & `omnidep-0.3.7/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -149,14 +149,31 @@
 Since: 0.2.0
 
 Causes omnidep to treat all code in ``myproject.tests`` as test code, meaning
 that anything it imports can be provided either by your project's dependencies
 or by its dev-dependencies. Imports from code that is not test code must be
 provided by non-dev dependencies.
 
+Since 0.3.7
+
+You can use a glob pattern at the end (only) of each path, the same format as
+`Pathlib.glob <https://docs.python.org/3/library/pathlib.html#pathlib.Path.glob>`_
+Specifying ``myproject/tests/**/*.py`` is equivalent to just specifying the
+directory ``myproject/tests/``.
+
+You can give a tighter pattern for your test files, such as
+``myproject/**/*_tests.py``. In that case ``foo_tests.py`` is test code, and
+``foo.py`` is non-test code, wherever they appear under ``myproject``.
+
+You can also search non-recursively, such as ``myproject/tests/*.py``, in
+which case ``myproject/tests/foo/bar.py`` would be considered non-test code.
+
+Regardless of the pattern you specify, only .py files are ever analysed by
+omnidep. For example ``*.txt`` will match nothing.
+
 local-test-packages
 ^^^^^^^^^^^^^^^^^^^
 
 Example: ``local-test-packages = ["tests"]``
 
 Since: 0.2.0
 
@@ -340,14 +357,20 @@
 * If you know what you're doing, and users of your project will know how to
   supply the code that you're importing, then ignore the import with
   ``ignore-imports = ["X"]`` in your ``[tool.omnidep]`` config.
 
 Changelog
 =========
 
+0.3.7 (2024-04-14)
+------------------
+
+* Allow globs when specifying local paths.
+
+
 0.3.6
 -----
 
 * Add Python 3.12 to the test matrix, and to the trove classifiers.
 * Correction to the documentation for the ODEP001 error message
   (https://github.com/sjjessop/omnidep/issues/4)
```

### Comparing `omnidep-0.3.6/PKG-INFO` & `omnidep-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnidep
-Version: 0.3.6
+Version: 0.3.7
 Summary: Linter to compare project dependencies against imports in source code
 Home-page: https://github.com/sjjessop/omnidep
 License: MIT
 Author: Steve Jessop
 Author-email: 68118527+sjjessop@users.noreply.github.com
 Requires-Python: >=3.7.0
 Classifier: License :: OSI Approved :: MIT License
@@ -172,14 +172,31 @@
 Since: 0.2.0
 
 Causes omnidep to treat all code in ``myproject.tests`` as test code, meaning
 that anything it imports can be provided either by your project's dependencies
 or by its dev-dependencies. Imports from code that is not test code must be
 provided by non-dev dependencies.
 
+Since 0.3.7
+
+You can use a glob pattern at the end (only) of each path, the same format as
+`Pathlib.glob <https://docs.python.org/3/library/pathlib.html#pathlib.Path.glob>`_
+Specifying ``myproject/tests/**/*.py`` is equivalent to just specifying the
+directory ``myproject/tests/``.
+
+You can give a tighter pattern for your test files, such as
+``myproject/**/*_tests.py``. In that case ``foo_tests.py`` is test code, and
+``foo.py`` is non-test code, wherever they appear under ``myproject``.
+
+You can also search non-recursively, such as ``myproject/tests/*.py``, in
+which case ``myproject/tests/foo/bar.py`` would be considered non-test code.
+
+Regardless of the pattern you specify, only .py files are ever analysed by
+omnidep. For example ``*.txt`` will match nothing.
+
 local-test-packages
 ^^^^^^^^^^^^^^^^^^^
 
 Example: ``local-test-packages = ["tests"]``
 
 Since: 0.2.0
 
@@ -363,14 +380,20 @@
 * If you know what you're doing, and users of your project will know how to
   supply the code that you're importing, then ignore the import with
   ``ignore-imports = ["X"]`` in your ``[tool.omnidep]`` config.
 
 Changelog
 =========
 
+0.3.7 (2024-04-14)
+------------------
+
+* Allow globs when specifying local paths.
+
+
 0.3.6
 -----
 
 * Add Python 3.12 to the test matrix, and to the trove classifiers.
 * Correction to the documentation for the ODEP001 error message
   (https://github.com/sjjessop/omnidep/issues/4)
```

