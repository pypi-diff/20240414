# Comparing `tmp/chiasmodon-0.2.9.tar.gz` & `tmp/chiasmodon-1.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chiasmodon-0.2.9.tar", last modified: Sat Mar 23 21:45:53 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

