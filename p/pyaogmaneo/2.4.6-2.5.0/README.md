# Comparing `tmp/pyaogmaneo-2.4.6.tar.gz` & `tmp/pyaogmaneo-2.5.0-cp312-cp312-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaogmaneo-2.4.6.tar", last modified: Thu Apr 11 18:48:56 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

