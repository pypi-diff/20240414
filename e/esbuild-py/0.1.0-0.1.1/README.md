# Comparing `tmp/esbuild_py-0.1.0.tar.gz` & `tmp/esbuild_py-0.1.1-cp312-cp312-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esbuild_py-0.1.0.tar", last modified: Sat Apr 13 19:52:23 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

