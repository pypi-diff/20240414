# Comparing `tmp/ytmdl-2023.7.27.tar.gz` & `tmp/ytmdl-2024.4.14-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytmdl-2023.7.27.tar", last modified: Sun Aug 27 09:29:09 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

