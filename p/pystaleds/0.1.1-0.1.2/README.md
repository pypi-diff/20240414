# Comparing `tmp/pystaleds-0.1.1.tar.gz` & `tmp/pystaleds-0.1.2.tar.gz`

## Comparing `pystaleds-0.1.1.tar` & `pystaleds-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 pystaleds-0.1.1/Cargo.toml
--rw-r--r--   0     1001      127     3526 2024-04-14 19:06:13.000000 pystaleds-0.1.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      127     1391 2024-04-14 19:06:13.000000 pystaleds-0.1.1/.github/workflows/linting.yml
--rw-r--r--   0     1001      127     2437 2024-04-14 19:06:13.000000 pystaleds-0.1.1/.github/workflows/tests.yml
--rw-r--r--   0     1001      127      686 2024-04-14 19:06:13.000000 pystaleds-0.1.1/.gitignore
--rw-r--r--   0     1001      127    25979 2024-04-14 19:06:13.000000 pystaleds-0.1.1/Cargo.lock
--rw-r--r--   0     1001      127     1062 2024-04-14 19:06:13.000000 pystaleds-0.1.1/LICENSE
--rw-r--r--   0     1001      127      564 2024-04-14 19:06:13.000000 pystaleds-0.1.1/README.md
--rw-r--r--   0     1001      127     2338 2024-04-14 19:06:13.000000 pystaleds-0.1.1/src/ast_parsing.rs
--rw-r--r--   0     1001      127      324 2024-04-14 19:06:13.000000 pystaleds-0.1.1/src/debug.rs
--rw-r--r--   0     1001      127       65 2024-04-14 19:06:13.000000 pystaleds-0.1.1/src/lib.rs
--rw-r--r--   0     1001      127     5653 2024-04-14 19:06:13.000000 pystaleds-0.1.1/src/main.rs
--rw-r--r--   0     1001      127     4083 2024-04-14 19:06:13.000000 pystaleds-0.1.1/src/parsing.rs
--rw-r--r--   0     1001      127    21488 2024-04-14 19:06:13.000000 pystaleds-0.1.1/src/rules_checking.rs
--rw-r--r--   0     1001      127      188 2024-04-14 19:06:13.000000 pystaleds-0.1.1/test.py
--rw-r--r--   0     1001      127      335 2024-04-14 19:06:13.000000 pystaleds-0.1.1/test_folder/test.py
--rw-r--r--   0     1001      127      152 2024-04-14 19:06:13.000000 pystaleds-0.1.1/test_folder/test_cp.py
--rw-r--r--   0     1001      127      857 2024-04-14 19:06:13.000000 pystaleds-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 pystaleds-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 pystaleds-0.1.2/Cargo.toml
+-rw-r--r--   0     1001      127     3526 2024-04-14 20:31:18.000000 pystaleds-0.1.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127     1391 2024-04-14 20:31:18.000000 pystaleds-0.1.2/.github/workflows/linting.yml
+-rw-r--r--   0     1001      127     2437 2024-04-14 20:31:18.000000 pystaleds-0.1.2/.github/workflows/tests.yml
+-rw-r--r--   0     1001      127      686 2024-04-14 20:31:18.000000 pystaleds-0.1.2/.gitignore
+-rw-r--r--   0     1001      127    25979 2024-04-14 20:31:18.000000 pystaleds-0.1.2/Cargo.lock
+-rw-r--r--   0     1001      127     1062 2024-04-14 20:31:18.000000 pystaleds-0.1.2/LICENSE
+-rw-r--r--   0     1001      127     5339 2024-04-14 20:31:18.000000 pystaleds-0.1.2/README.md
+-rw-r--r--   0     1001      127     2338 2024-04-14 20:31:18.000000 pystaleds-0.1.2/src/ast_parsing.rs
+-rw-r--r--   0     1001      127      324 2024-04-14 20:31:18.000000 pystaleds-0.1.2/src/debug.rs
+-rw-r--r--   0     1001      127       65 2024-04-14 20:31:18.000000 pystaleds-0.1.2/src/lib.rs
+-rw-r--r--   0     1001      127     5652 2024-04-14 20:31:18.000000 pystaleds-0.1.2/src/main.rs
+-rw-r--r--   0     1001      127     4083 2024-04-14 20:31:18.000000 pystaleds-0.1.2/src/parsing.rs
+-rw-r--r--   0     1001      127    21488 2024-04-14 20:31:18.000000 pystaleds-0.1.2/src/rules_checking.rs
+-rw-r--r--   0     1001      127      188 2024-04-14 20:31:18.000000 pystaleds-0.1.2/test.py
+-rw-r--r--   0     1001      127      335 2024-04-14 20:31:18.000000 pystaleds-0.1.2/test_folder/test.py
+-rw-r--r--   0     1001      127      152 2024-04-14 20:31:18.000000 pystaleds-0.1.2/test_folder/test_cp.py
+-rw-r--r--   0     1001      127      857 2024-04-14 20:31:18.000000 pystaleds-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6036 1970-01-01 00:00:00.000000 pystaleds-0.1.2/PKG-INFO
```

### Comparing `pystaleds-0.1.1/Cargo.toml` & `pystaleds-0.1.2/Cargo.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pystaleds"
-version = "0.1.1"
+version = "0.1.2"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pystaleds"
 crate-type = ["lib"]
```

### Comparing `pystaleds-0.1.1/.github/workflows/CI.yml` & `pystaleds-0.1.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pystaleds-0.1.1/.github/workflows/linting.yml` & `pystaleds-0.1.2/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pystaleds-0.1.1/.github/workflows/tests.yml` & `pystaleds-0.1.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `pystaleds-0.1.1/.gitignore` & `pystaleds-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pystaleds-0.1.1/Cargo.lock` & `pystaleds-0.1.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -405,15 +405,15 @@
  "pyo3-build-config",
  "quote",
  "syn 2.0.58",
 ]
 
 [[package]]
 name = "pystaleds"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "anyhow",
  "cc",
  "clap",
  "glob",
  "pyo3",
  "rayon",
```

### Comparing `pystaleds-0.1.1/LICENSE` & `pystaleds-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pystaleds-0.1.1/src/ast_parsing.rs` & `pystaleds-0.1.2/src/ast_parsing.rs`

 * *Files identical despite different names*

### Comparing `pystaleds-0.1.1/src/main.rs` & `pystaleds-0.1.2/src/main.rs`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 #[derive(Parser)]
 #[command(version, about, long_about=None)]
 struct Args {
     path: String,
 
     #[arg(long, default_value_t = false, alias = "ah")]
-    /// Will ignore hidden files.
+    /// Will allow hidden files.
     allow_hidden: bool,
 
     #[arg(long, default_value_t = false, alias = "be")]
     /// Will consider that an "Args" section breaks on an empty line.
     break_on_empty_line: bool,
 
     #[arg(long, default_value_t = false, alias = "nd")]
```

### Comparing `pystaleds-0.1.1/src/parsing.rs` & `pystaleds-0.1.2/src/parsing.rs`

 * *Files identical despite different names*

### Comparing `pystaleds-0.1.1/src/rules_checking.rs` & `pystaleds-0.1.2/src/rules_checking.rs`

 * *Files identical despite different names*

### Comparing `pystaleds-0.1.1/pyproject.toml` & `pystaleds-0.1.2/pyproject.toml`

 * *Files identical despite different names*

