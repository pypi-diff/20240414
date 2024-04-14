# Comparing `tmp/akatsuki_pp_py-1.0.0.tar.gz` & `tmp/akatsuki_pp_py-1.0.1.tar.gz`

## Comparing `akatsuki_pp_py-1.0.0.tar` & `akatsuki_pp_py-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 akatsuki_pp_py-1.0.0/Cargo.toml
--rw-r--r--   0      501       20     3861 2023-11-16 20:40:42.000000 akatsuki_pp_py-1.0.0/.github/workflows/publish.yml
--rw-r--r--   0      501       20      686 2023-11-16 20:40:42.000000 akatsuki_pp_py-1.0.0/.gitignore
--rw-r--r--   0      501       20     2445 2023-11-16 20:40:42.000000 akatsuki_pp_py-1.0.0/CHANGELOG.md
--rw-r--r--   0      501       20     1060 2023-11-16 20:40:42.000000 akatsuki_pp_py-1.0.0/LICENSE
--rw-r--r--   0      501       20     4186 2023-11-16 20:40:42.000000 akatsuki_pp_py-1.0.0/README.md
--rw-r--r--   0      501       20    13156 2023-11-16 20:40:42.000000 akatsuki_pp_py-1.0.0/akatsuki_pp_py.pyi
--rw-r--r--   0      501       20      915 2023-11-16 20:40:42.000000 akatsuki_pp_py-1.0.0/pyproject.toml
--rw-r--r--   0      501       20     4462 2023-11-16 20:40:42.000000 akatsuki_pp_py-1.0.0/src/beatmap.rs
--rw-r--r--   0      501       20    10276 2023-11-16 20:40:42.000000 akatsuki_pp_py-1.0.0/src/calculator.rs
--rw-r--r--   0      501       20     6821 2023-11-16 20:40:42.000000 akatsuki_pp_py-1.0.0/src/diff_attrs.rs
--rw-r--r--   0      501       20      632 2023-11-16 20:40:42.000000 akatsuki_pp_py-1.0.0/src/error.rs
--rw-r--r--   0      501       20      930 2023-11-16 20:40:42.000000 akatsuki_pp_py-1.0.0/src/lib.rs
--rw-r--r--   0      501       20     2338 2023-11-16 20:40:42.000000 akatsuki_pp_py-1.0.0/src/map_attrs.rs
--rw-r--r--   0      501       20     4495 2023-11-16 20:40:42.000000 akatsuki_pp_py-1.0.0/src/perf_attrs.rs
--rw-r--r--   0      501       20     4695 2023-11-16 20:40:42.000000 akatsuki_pp_py-1.0.0/src/strains.rs
--rw-r--r--   0      501       20     7634 2023-11-16 20:40:42.000000 akatsuki_pp_py-1.0.0/Cargo.lock
--rw-r--r--   0        0        0     4981 1970-01-01 00:00:00.000000 akatsuki_pp_py-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 akatsuki_pp_py-1.0.1/Cargo.toml
+-rw-r--r--   0      501       20     3861 2024-04-14 13:47:22.000000 akatsuki_pp_py-1.0.1/.github/workflows/publish.yml
+-rw-r--r--   0      501       20      686 2024-04-14 13:47:22.000000 akatsuki_pp_py-1.0.1/.gitignore
+-rw-r--r--   0      501       20     2445 2024-04-14 13:47:22.000000 akatsuki_pp_py-1.0.1/CHANGELOG.md
+-rw-r--r--   0      501       20     1060 2024-04-14 13:47:22.000000 akatsuki_pp_py-1.0.1/LICENSE
+-rw-r--r--   0      501       20     4186 2024-04-14 13:47:22.000000 akatsuki_pp_py-1.0.1/README.md
+-rw-r--r--   0      501       20    13156 2024-04-14 13:47:22.000000 akatsuki_pp_py-1.0.1/akatsuki_pp_py.pyi
+-rw-r--r--   0      501       20      915 2024-04-14 13:47:22.000000 akatsuki_pp_py-1.0.1/pyproject.toml
+-rw-r--r--   0      501       20     4462 2024-04-14 13:47:22.000000 akatsuki_pp_py-1.0.1/src/beatmap.rs
+-rw-r--r--   0      501       20    10276 2024-04-14 13:47:22.000000 akatsuki_pp_py-1.0.1/src/calculator.rs
+-rw-r--r--   0      501       20     6821 2024-04-14 13:47:22.000000 akatsuki_pp_py-1.0.1/src/diff_attrs.rs
+-rw-r--r--   0      501       20      632 2024-04-14 13:47:22.000000 akatsuki_pp_py-1.0.1/src/error.rs
+-rw-r--r--   0      501       20      930 2024-04-14 13:47:22.000000 akatsuki_pp_py-1.0.1/src/lib.rs
+-rw-r--r--   0      501       20     2338 2024-04-14 13:47:22.000000 akatsuki_pp_py-1.0.1/src/map_attrs.rs
+-rw-r--r--   0      501       20     4495 2024-04-14 13:47:22.000000 akatsuki_pp_py-1.0.1/src/perf_attrs.rs
+-rw-r--r--   0      501       20     4695 2024-04-14 13:47:22.000000 akatsuki_pp_py-1.0.1/src/strains.rs
+-rw-r--r--   0      501       20     7634 2024-04-14 13:47:22.000000 akatsuki_pp_py-1.0.1/Cargo.lock
+-rw-r--r--   0        0        0     4981 1970-01-01 00:00:00.000000 akatsuki_pp_py-1.0.1/PKG-INFO
```

### Comparing `akatsuki_pp_py-1.0.0/Cargo.toml` & `akatsuki_pp_py-1.0.1/Cargo.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [package]
 name = "akatsuki-pp-py"
-version = "1.0.0"
+version = "1.0.1"
 description = "osu! difficulty and pp calculation for all modes"
 authors = ["Max Ohn <ohn.m@hotmail.de>", "tsunyoku <tsunyoku@gmail.com>"]
 license = "MIT"
 edition = "2021"
 
 [lib]
 name = "akatsuki_pp_py"
 crate-type = ["cdylib"]
 
 [dependencies]
 pyo3 = { version = "0.17", features = ["extension-module", "macros"] }
-akatsuki-pp = { git = "https://github.com/osuAkatsuki/akatsuki-pp-rs", rev = "a8b4eaffb2274d2e86ff042b7327286e13b6488d" }
+akatsuki-pp = { git = "https://github.com/osuAkatsuki/akatsuki-pp-rs", rev = "5c97207f25cf9fd07252dca1ba68d785e2147ce1" }
 
 [profile.release]
 lto = "fat"
 codegen-units = 1
 strip = "debuginfo"
```

### Comparing `akatsuki_pp_py-1.0.0/.github/workflows/publish.yml` & `akatsuki_pp_py-1.0.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `akatsuki_pp_py-1.0.0/.gitignore` & `akatsuki_pp_py-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `akatsuki_pp_py-1.0.0/CHANGELOG.md` & `akatsuki_pp_py-1.0.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `akatsuki_pp_py-1.0.0/LICENSE` & `akatsuki_pp_py-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `akatsuki_pp_py-1.0.0/README.md` & `akatsuki_pp_py-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `akatsuki_pp_py-1.0.0/akatsuki_pp_py.pyi` & `akatsuki_pp_py-1.0.1/akatsuki_pp_py.pyi`

 * *Files identical despite different names*

### Comparing `akatsuki_pp_py-1.0.0/pyproject.toml` & `akatsuki_pp_py-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "akatsuki-pp-py"
-version = "1.0.0"
+version = "1.0.1"
 requires-python = ">=3.7"
 description = "osu! difficulty and pp calculation for all modes"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `akatsuki_pp_py-1.0.0/src/beatmap.rs` & `akatsuki_pp_py-1.0.1/src/beatmap.rs`

 * *Files identical despite different names*

### Comparing `akatsuki_pp_py-1.0.0/src/calculator.rs` & `akatsuki_pp_py-1.0.1/src/calculator.rs`

 * *Files identical despite different names*

### Comparing `akatsuki_pp_py-1.0.0/src/diff_attrs.rs` & `akatsuki_pp_py-1.0.1/src/diff_attrs.rs`

 * *Files identical despite different names*

### Comparing `akatsuki_pp_py-1.0.0/src/error.rs` & `akatsuki_pp_py-1.0.1/src/error.rs`

 * *Files identical despite different names*

### Comparing `akatsuki_pp_py-1.0.0/src/lib.rs` & `akatsuki_pp_py-1.0.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `akatsuki_pp_py-1.0.0/src/map_attrs.rs` & `akatsuki_pp_py-1.0.1/src/map_attrs.rs`

 * *Files identical despite different names*

### Comparing `akatsuki_pp_py-1.0.0/src/perf_attrs.rs` & `akatsuki_pp_py-1.0.1/src/perf_attrs.rs`

 * *Files identical despite different names*

### Comparing `akatsuki_pp_py-1.0.0/src/strains.rs` & `akatsuki_pp_py-1.0.1/src/strains.rs`

 * *Files identical despite different names*

### Comparing `akatsuki_pp_py-1.0.0/Cargo.lock` & `akatsuki_pp_py-1.0.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "akatsuki-pp"
 version = "0.9.6"
-source = "git+https://github.com/osuAkatsuki/akatsuki-pp-rs?rev=a8b4eaffb2274d2e86ff042b7327286e13b6488d#a8b4eaffb2274d2e86ff042b7327286e13b6488d"
+source = "git+https://github.com/osuAkatsuki/akatsuki-pp-rs?rev=5c97207f25cf9fd07252dca1ba68d785e2147ce1#5c97207f25cf9fd07252dca1ba68d785e2147ce1"
 
 [[package]]
 name = "akatsuki-pp-py"
-version = "1.0.0"
+version = "1.0.1"
 dependencies = [
  "akatsuki-pp",
  "pyo3",
 ]
 
 [[package]]
 name = "autocfg"
```

### Comparing `akatsuki_pp_py-1.0.0/PKG-INFO` & `akatsuki_pp_py-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akatsuki-pp-py
-Version: 1.0.0
+Version: 1.0.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

