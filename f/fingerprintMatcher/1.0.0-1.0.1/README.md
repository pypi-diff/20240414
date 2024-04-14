# Comparing `tmp/fingerprintMatcher-1.0.0.tar.gz` & `tmp/fingerprintMatcher-1.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fingerprintMatcher-1.0.0.tar", last modified: Sun Apr 14 11:22:58 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

