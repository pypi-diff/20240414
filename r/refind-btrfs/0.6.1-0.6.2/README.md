# Comparing `tmp/refind-btrfs-0.6.1.tar.gz` & `tmp/refind_btrfs-0.6.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refind-btrfs-0.6.1.tar", last modified: Mon Nov 20 20:50:30 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

