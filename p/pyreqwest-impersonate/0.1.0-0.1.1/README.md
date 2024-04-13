# Comparing `tmp/pyreqwest_impersonate-0.1.0.tar.gz` & `tmp/pyreqwest_impersonate-0.1.1.tar.gz`

## Comparing `pyreqwest_impersonate-0.1.0.tar` & `pyreqwest_impersonate-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.1.0/Cargo.toml
--rw-r--r--   0     1001      127     4802 2024-04-12 20:50:44.000000 pyreqwest_impersonate-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-04-12 20:50:44.000000 pyreqwest_impersonate-0.1.0/.gitignore
--rw-r--r--   0     1001      127     1850 2024-04-12 20:50:44.000000 pyreqwest_impersonate-0.1.0/README.md
--rw-r--r--   0     1001      127     5116 2024-04-12 20:50:44.000000 pyreqwest_impersonate-0.1.0/src/lib.rs
--rw-r--r--   0     1001      127      341 2024-04-12 20:50:44.000000 pyreqwest_impersonate-0.1.0/tests/test_client.py
--rw-r--r--   0     1001      127    40959 2024-04-12 20:50:44.000000 pyreqwest_impersonate-0.1.0/Cargo.lock
--rw-r--r--   0     1001      127     1073 2024-04-12 20:50:44.000000 pyreqwest_impersonate-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2858 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      127     5305 2024-04-13 00:04:30.000000 pyreqwest_impersonate-0.1.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-04-13 00:04:30.000000 pyreqwest_impersonate-0.1.1/.gitignore
+-rw-r--r--   0     1001      127     1850 2024-04-13 00:04:30.000000 pyreqwest_impersonate-0.1.1/README.md
+-rw-r--r--   0     1001      127     5116 2024-04-13 00:04:30.000000 pyreqwest_impersonate-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      127      341 2024-04-13 00:04:30.000000 pyreqwest_impersonate-0.1.1/tests/test_client.py
+-rw-r--r--   0     1001      127    40959 2024-04-13 00:04:30.000000 pyreqwest_impersonate-0.1.1/Cargo.lock
+-rw-r--r--   0     1001      127     1073 2024-04-13 00:04:30.000000 pyreqwest_impersonate-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2858 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.1.1/PKG-INFO
```

### Comparing `pyreqwest_impersonate-0.1.0/Cargo.toml` & `pyreqwest_impersonate-0.1.1/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pyreqwest_impersonate"
-version = "0.1.0"
+version = "0.1.1"
 edition = "2021"
 description = "HTTP requests with impersonating web browsers. Impersonate browsers headers, `TLS/JA3` and `HTTP/2` fingerprints."
 authors = ["deedy5"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
```

### Comparing `pyreqwest_impersonate-0.1.0/.github/workflows/CI.yml` & `pyreqwest_impersonate-0.1.1/.github/workflows/CI.yml`

 * *Files 5% similar despite different names*

```diff
@@ -15,65 +15,81 @@
   pull_request:
   workflow_dispatch:
 
 permissions:
   contents: read
 
 jobs:
-  linux:
+  linux_x86_64:
     runs-on: ${{ matrix.platform.runner }}
     strategy:
       matrix:
         platform:
           - runner: ubuntu-latest
             target: x86_64
+        python-version: ['3.8', '3.9', '3.10', '3.11', '3.12']
+    steps:
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
+        with:
+          python-version: ${{ matrix.python-version }}
+      - name: Build wheels
+        uses: PyO3/maturin-action@v1
+        with:
+          target: ${{ matrix.platform.target }}
+          args: --release --out dist --zig -i python${{ matrix.python-version }}
+          sccache: 'true'
+          manylinux: auto
+      - name: Upload wheels
+        uses: actions/upload-artifact@v4
+        with:
+          name: wheels-linux-${{ matrix.platform.target }}-python${{ matrix.python-version }}
+          path: dist
+      - name: pytest
+        shell: bash
+        run: |
+          set -e
+          pip install pyreqwest_impersonate --find-links dist --force-reinstall
+          pip install pytest
+          pytest
+
+  linux_aarch64:
+    runs-on: ${{ matrix.platform.runner }}
+    strategy:
+      matrix:
+        platform:
           - runner: ubuntu-latest
             target: aarch64
+        python-version: ['3.10']
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
-          python-version: '3.10'
+          python-version: ${{ matrix.python-version }}
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.platform.target }}
-          args: --release --out dist --find-interpreter --zig
+          args: --release --out dist --zig --find-interpreter
           sccache: 'true'
           manylinux: auto
         env:
           CFLAGS_aarch64_unknown_linux_gnu: "-D__ARM_ARCH=8"
       - name: Upload wheels
         uses: actions/upload-artifact@v4
         with:
-          name: wheels-linux-${{ matrix.platform.target }}
+          name: wheels-linux-${{ matrix.platform.target }}-python${{ matrix.python-version }}
           path: dist
       - name: pytest
-        if: ${{ startsWith(matrix.platform.target, 'x86_64') }}
         shell: bash
         run: |
           set -e
           pip install pyreqwest_impersonate --find-links dist --force-reinstall
           pip install pytest
           pytest
-      - name: pytest
-        if: ${{ !startsWith(matrix.platform.target, 'x86') && matrix.platform.target != 'ppc64' }}
-        uses: uraimo/run-on-arch-action@v2.5.0
-        with:
-          arch: ${{ matrix.platform.target }}
-          distro: ubuntu22.04
-          githubToken: ${{ github.token }}
-          install: |
-            apt-get update
-            apt-get install -y --no-install-recommends python3 python3-pip
-            pip3 install -U pip pytest
-          run: |
-            set -e
-            pip3 install pyreqwest_impersonate --find-links dist --force-reinstall
-            pytest
 
   windows:
     runs-on: ${{ matrix.platform.runner }}
     strategy:
       matrix:
         platform:
           - runner: windows-latest
@@ -91,15 +107,15 @@
         with:
           target: ${{ matrix.platform.target }}
           args: --release --out dist --find-interpreter
           sccache: 'true'
       - name: Upload wheels
         uses: actions/upload-artifact@v4
         with:
-          name: wheels-windows-${{ matrix.platform.target }}
+          name: wheels-windows-${{ matrix.platform.target }}-python${{ matrix.python-version }}
           path: dist
       - name: pytest
         if: ${{ !startsWith(matrix.platform.target, 'aarch64') }}
         shell: bash
         run: |
           set -e
           pip install pyreqwest_impersonate --find-links dist --force-reinstall
@@ -125,15 +141,15 @@
         with:
           target: ${{ matrix.platform.target }}
           args: --release --out dist --find-interpreter
           sccache: 'true'
       - name: Upload wheels
         uses: actions/upload-artifact@v4
         with:
-          name: wheels-macos-${{ matrix.platform.target }}
+          name: wheels-macos-${{ matrix.platform.target }}-python${{ matrix.python-version }}
           path: dist
       - name: pytest
         if: ${{ !startsWith(matrix.platform.target, 'aarch64') }}
         shell: bash
         run: |
           set -e
           pip install pyreqwest_impersonate --find-links dist --force-reinstall
@@ -155,15 +171,15 @@
           name: wheels-sdist
           path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
     if: "startsWith(github.ref, 'refs/tags/')"
-    needs: [linux, windows, macos, sdist]
+    needs: [linux_x86_64, linux_aarch64, windows, macos, sdist]
     steps:
       - uses: actions/download-artifact@v4
       - name: Publish to PyPI
         uses: PyO3/maturin-action@v1
         env:
           MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
         with:
```

### Comparing `pyreqwest_impersonate-0.1.0/.gitignore` & `pyreqwest_impersonate-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.1.0/README.md` & `pyreqwest_impersonate-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.1.0/src/lib.rs` & `pyreqwest_impersonate-0.1.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.1.0/Cargo.lock` & `pyreqwest_impersonate-0.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -899,15 +899,15 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyreqwest_impersonate"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "pyo3",
  "reqwest-impersonate",
 ]
 
 [[package]]
 name = "quote"
```

### Comparing `pyreqwest_impersonate-0.1.0/pyproject.toml` & `pyreqwest_impersonate-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.1.0/PKG-INFO` & `pyreqwest_impersonate-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyreqwest_impersonate
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

