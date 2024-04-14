# Comparing `tmp/vitriolic-3.3.6.tar.gz` & `tmp/vitriolic-3.3.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vitriolic-3.3.6.tar", last modified: Fri Feb  9 07:04:34 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

