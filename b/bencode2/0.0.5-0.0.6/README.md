# Comparing `tmp/bencode2-0.0.5.tar.gz` & `tmp/bencode2-0.0.6-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bencode2-0.0.5.tar", last modified: Sun Apr 14 07:57:18 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

