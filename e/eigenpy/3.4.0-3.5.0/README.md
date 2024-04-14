# Comparing `tmp/eigenpy-3.4.0.tar.gz` & `tmp/eigenpy-3.5.0-3-cp312-cp312-manylinux_2_28_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eigenpy-3.4.0.tar", last modified: Mon Feb 26 16:02:41 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

