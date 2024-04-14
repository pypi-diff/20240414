# Comparing `tmp/esbuild_py-0.1.1.tar.gz` & `tmp/esbuild_py-0.1.2-pp39-pypy39_pp73-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esbuild_py-0.1.1.tar", last modified: Sun Apr 14 19:04:25 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

