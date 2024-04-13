# Comparing `tmp/onnx-graphsurgeon-0.0.1.dev5.tar.gz` & `tmp/onnx_graphsurgeon-0.5.2-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/onnx-graphsurgeon-0.0.1.dev5.tar", last modified: Fri Apr 23 23:30:39 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

