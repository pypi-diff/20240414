# Comparing `tmp/invest_guard-0.1.14.tar.gz` & `tmp/invest_guard-0.1.15-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invest_guard-0.1.14.tar", last modified: Sun Apr 14 01:23:02 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

