# Comparing `tmp/sc_file-3.0.6.tar.gz` & `tmp/sc_file-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc_file-3.0.6.tar", max compression
+gzip compressed data, was "sc_file-3.0.7.tar", max compression
```

## Comparing `sc_file-3.0.6.tar` & `sc_file-3.0.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1083 2023-01-22 13:34:34.609366 sc_file-3.0.6/LICENSE
--rw-r--r--   0        0        0      607 2024-04-02 04:38:51.888155 sc_file-3.0.6/pyproject.toml
--rw-r--r--   0        0        0     5065 2024-04-02 04:37:30.352990 sc_file-3.0.6/README.md
--rw-r--r--   0        0        0      158 2024-03-20 03:27:16.310140 sc_file-3.0.6/scfile/__init__.py
--rw-r--r--   0        0        0     1485 2024-04-02 04:37:30.354990 sc_file-3.0.6/scfile/__main__.py
--rw-r--r--   0        0        0     1192 2024-03-20 03:27:16.311141 sc_file-3.0.6/scfile/consts.py
--rw-r--r--   0        0        0     1124 2024-03-20 03:27:16.312140 sc_file-3.0.6/scfile/enums.py
--rw-r--r--   0        0        0      427 2024-03-20 03:27:16.312140 sc_file-3.0.6/scfile/exceptions/__init__.py
--rw-r--r--   0        0        0       84 2024-03-20 03:27:16.312140 sc_file-3.0.6/scfile/exceptions/base.py
--rw-r--r--   0        0        0     1408 2024-03-20 03:27:16.313140 sc_file-3.0.6/scfile/exceptions/basic.py
--rw-r--r--   0        0        0      641 2024-03-20 03:27:16.313140 sc_file-3.0.6/scfile/exceptions/decode.py
--rw-r--r--   0        0        0     1409 2024-03-20 03:27:16.313140 sc_file-3.0.6/scfile/exceptions/mcsa.py
--rw-r--r--   0        0        0      866 2024-03-20 03:27:16.314140 sc_file-3.0.6/scfile/exceptions/ol.py
--rw-r--r--   0        0        0        2 2024-03-20 03:27:16.314140 sc_file-3.0.6/scfile/file/__init__.py
--rw-r--r--   0        0        0      780 2024-03-20 03:27:16.314140 sc_file-3.0.6/scfile/file/base.py
--rw-r--r--   0        0        0      394 2024-03-25 13:19:34.701976 sc_file-3.0.6/scfile/file/data.py
--rw-r--r--   0        0        0     2162 2024-03-20 03:27:16.315140 sc_file-3.0.6/scfile/file/dds/encoder.py
--rw-r--r--   0        0        0     1124 2024-03-20 03:27:16.315140 sc_file-3.0.6/scfile/file/dds/structure.py
--rw-r--r--   0        0        0     3185 2024-03-26 21:28:59.417991 sc_file-3.0.6/scfile/file/decoder.py
--rw-r--r--   0        0        0     1840 2024-03-26 21:28:59.418992 sc_file-3.0.6/scfile/file/encoder.py
--rw-r--r--   0        0        0     7329 2024-04-02 04:05:44.388714 sc_file-3.0.6/scfile/file/mcsa/decoder.py
--rw-r--r--   0        0        0      682 2024-03-26 21:28:59.419991 sc_file-3.0.6/scfile/file/mcsa/flags.py
--rw-r--r--   0        0        0      153 2024-03-20 03:27:16.317139 sc_file-3.0.6/scfile/file/mcsa/versions.py
--rw-r--r--   0        0        0      611 2024-03-20 03:27:16.317139 sc_file-3.0.6/scfile/file/mic/decoder.py
--rw-r--r--   0        0        0     2284 2024-03-26 21:28:59.419991 sc_file-3.0.6/scfile/file/obj/encoder.py
--rw-r--r--   0        0        0      694 2024-03-20 03:27:16.318139 sc_file-3.0.6/scfile/file/ol/converter/base.py
--rw-r--r--   0        0        0      189 2024-03-20 03:27:16.318139 sc_file-3.0.6/scfile/file/ol/converter/bgra8.py
--rw-r--r--   0        0        0      244 2024-03-20 03:27:16.318139 sc_file-3.0.6/scfile/file/ol/converter/rgba32f.py
--rw-r--r--   0        0        0     3864 2024-03-26 21:28:59.419991 sc_file-3.0.6/scfile/file/ol/decoder.py
--rw-r--r--   0        0        0      144 2024-03-20 03:27:16.319140 sc_file-3.0.6/scfile/file/ol/formats.py
--rw-r--r--   0        0        0      295 2024-03-20 03:27:16.319140 sc_file-3.0.6/scfile/file/png/encoder.py
--rw-r--r--   0        0        0        0 2024-03-20 03:27:16.319140 sc_file-3.0.6/scfile/io/__init__.py
--rw-r--r--   0        0        0     1568 2024-03-20 03:27:16.320140 sc_file-3.0.6/scfile/io/base.py
--rw-r--r--   0        0        0      261 2024-03-20 03:27:16.320140 sc_file-3.0.6/scfile/io/binary.py
--rw-r--r--   0        0        0      610 2024-03-20 03:27:16.320140 sc_file-3.0.6/scfile/io/mcsa.py
--rw-r--r--   0        0        0      405 2024-03-20 03:27:16.321141 sc_file-3.0.6/scfile/io/ol.py
--rw-r--r--   0        0        0      122 2024-03-26 21:28:59.420991 sc_file-3.0.6/scfile/types.py
--rw-r--r--   0        0        0     3341 2024-03-20 03:27:16.322141 sc_file-3.0.6/scfile/utils/convert.py
--rw-r--r--   0        0        0     3027 2024-04-02 04:40:15.093571 sc_file-3.0.6/scfile/utils/model.py
--rw-r--r--   0        0        0     6088 1970-01-01 00:00:00.000000 sc_file-3.0.6/setup.py
--rw-r--r--   0        0        0     5384 1970-01-01 00:00:00.000000 sc_file-3.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-01-22 13:34:34.609366 sc_file-3.0.7/LICENSE
+-rw-r--r--   0        0        0      795 2024-04-14 13:22:14.053758 sc_file-3.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5020 2024-04-14 13:16:37.213662 sc_file-3.0.7/README.md
+-rw-r--r--   0        0        0      158 2024-03-20 03:27:16.310140 sc_file-3.0.7/scfile/__init__.py
+-rw-r--r--   0        0        0     1485 2024-04-14 13:10:00.131909 sc_file-3.0.7/scfile/__main__.py
+-rw-r--r--   0        0        0     1192 2024-03-20 03:27:16.311141 sc_file-3.0.7/scfile/consts.py
+-rw-r--r--   0        0        0     1124 2024-03-20 03:27:16.312140 sc_file-3.0.7/scfile/enums.py
+-rw-r--r--   0        0        0      427 2024-03-20 03:27:16.312140 sc_file-3.0.7/scfile/exceptions/__init__.py
+-rw-r--r--   0        0        0       84 2024-03-20 03:27:16.312140 sc_file-3.0.7/scfile/exceptions/base.py
+-rw-r--r--   0        0        0     1408 2024-03-20 03:27:16.313140 sc_file-3.0.7/scfile/exceptions/basic.py
+-rw-r--r--   0        0        0      641 2024-03-20 03:27:16.313140 sc_file-3.0.7/scfile/exceptions/decode.py
+-rw-r--r--   0        0        0     1409 2024-03-20 03:27:16.313140 sc_file-3.0.7/scfile/exceptions/mcsa.py
+-rw-r--r--   0        0        0      866 2024-03-20 03:27:16.314140 sc_file-3.0.7/scfile/exceptions/ol.py
+-rw-r--r--   0        0        0        2 2024-03-20 03:27:16.314140 sc_file-3.0.7/scfile/file/__init__.py
+-rw-r--r--   0        0        0      780 2024-03-20 03:27:16.314140 sc_file-3.0.7/scfile/file/base.py
+-rw-r--r--   0        0        0      394 2024-03-25 13:19:34.701976 sc_file-3.0.7/scfile/file/data.py
+-rw-r--r--   0        0        0     2162 2024-03-20 03:27:16.315140 sc_file-3.0.7/scfile/file/dds/encoder.py
+-rw-r--r--   0        0        0     1124 2024-03-20 03:27:16.315140 sc_file-3.0.7/scfile/file/dds/structure.py
+-rw-r--r--   0        0        0     3185 2024-03-26 21:28:59.417991 sc_file-3.0.7/scfile/file/decoder.py
+-rw-r--r--   0        0        0     1840 2024-03-26 21:28:59.418992 sc_file-3.0.7/scfile/file/encoder.py
+-rw-r--r--   0        0        0     7342 2024-04-14 13:11:08.724324 sc_file-3.0.7/scfile/file/mcsa/decoder.py
+-rw-r--r--   0        0        0      682 2024-03-26 21:28:59.419991 sc_file-3.0.7/scfile/file/mcsa/flags.py
+-rw-r--r--   0        0        0      153 2024-03-20 03:27:16.317139 sc_file-3.0.7/scfile/file/mcsa/versions.py
+-rw-r--r--   0        0        0      611 2024-03-20 03:27:16.317139 sc_file-3.0.7/scfile/file/mic/decoder.py
+-rw-r--r--   0        0        0     2284 2024-03-26 21:28:59.419991 sc_file-3.0.7/scfile/file/obj/encoder.py
+-rw-r--r--   0        0        0      694 2024-03-20 03:27:16.318139 sc_file-3.0.7/scfile/file/ol/converter/base.py
+-rw-r--r--   0        0        0      189 2024-03-20 03:27:16.318139 sc_file-3.0.7/scfile/file/ol/converter/bgra8.py
+-rw-r--r--   0        0        0      244 2024-03-20 03:27:16.318139 sc_file-3.0.7/scfile/file/ol/converter/rgba32f.py
+-rw-r--r--   0        0        0     3864 2024-03-26 21:28:59.419991 sc_file-3.0.7/scfile/file/ol/decoder.py
+-rw-r--r--   0        0        0      144 2024-03-20 03:27:16.319140 sc_file-3.0.7/scfile/file/ol/formats.py
+-rw-r--r--   0        0        0      295 2024-03-20 03:27:16.319140 sc_file-3.0.7/scfile/file/png/encoder.py
+-rw-r--r--   0        0        0        0 2024-03-20 03:27:16.319140 sc_file-3.0.7/scfile/io/__init__.py
+-rw-r--r--   0        0        0     1568 2024-03-20 03:27:16.320140 sc_file-3.0.7/scfile/io/base.py
+-rw-r--r--   0        0        0      261 2024-03-20 03:27:16.320140 sc_file-3.0.7/scfile/io/binary.py
+-rw-r--r--   0        0        0      610 2024-03-20 03:27:16.320140 sc_file-3.0.7/scfile/io/mcsa.py
+-rw-r--r--   0        0        0      405 2024-03-20 03:27:16.321141 sc_file-3.0.7/scfile/io/ol.py
+-rw-r--r--   0        0        0      122 2024-03-26 21:28:59.420991 sc_file-3.0.7/scfile/types.py
+-rw-r--r--   0        0        0     3341 2024-03-20 03:27:16.322141 sc_file-3.0.7/scfile/utils/convert.py
+-rw-r--r--   0        0        0     3027 2024-04-02 04:43:06.633771 sc_file-3.0.7/scfile/utils/model.py
+-rw-r--r--   0        0        0     6071 1970-01-01 00:00:00.000000 sc_file-3.0.7/setup.py
+-rw-r--r--   0        0        0     5535 1970-01-01 00:00:00.000000 sc_file-3.0.7/PKG-INFO
```

### Comparing `sc_file-3.0.6/LICENSE` & `sc_file-3.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.6/pyproject.toml` & `sc_file-3.0.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 [tool.poetry]
 name = "sc-file"
-version = "3.0.6"
+version = "3.0.7"
 description = "Utility & Library for decoding stalcraft assets"
 authors = ["onejeuu <bloodtrail@beber1k.ru>"]
+
 license = "MIT"
 readme = "README.md"
+
+homepage = "https://github.com/onejeuu/sc-file"
+repository = "https://github.com/onejeuu/sc-file"
+documentation = "https://github.com/onejeuu/sc-file/?tab=readme-ov-file#usage-1"
+
 packages = [{ include = "scfile" }]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
 lz4 = "^4.3.2"
 click = "^8.1.7"
 quicktex = "^0.2.0"
```

### Comparing `sc_file-3.0.6/README.md` & `sc_file-3.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # SC FILE
 
 Utility and Library for decoding and converting stalcraft assets files, such as models and textures into well-known formats.
 
-You can use executable from [Releases](https://github.com/onejeuu/sc-file/releases) page.
+Designed for artworks creation and the like.
 
-> [!IMPORTANT]
-> This utility is designed for artworks and etc \
-> There is not and will not be any encoding back into game formats
+> [!NOTE]
+> There is not and will not be encoding back into game formats.
 
 > [!WARNING]
-> Do not use game assets directly \
-> You can get banned for any changes in game client
+> Do not use game assets directly. \
+> Any changes in game client can be detected.
+
+You can use executable program from [Releases](https://github.com/onejeuu/sc-file/releases) page.
 
 # 📁 Formats
 
 | Type    | Source format | Output format |
 | ------- | ------------- | ------------- |
 | Model   | .mcsa         | .obj          |
 | Texture | .ol           | .dds          |
@@ -33,63 +34,63 @@
 From bash:
 
 ```bash
 scfile [FILES]... [OPTIONS]
 ```
 
 > [!TIP]
-> You can just drag and drop one or multiple files onto `scfile.exe`
+> You can just drag and drop one or multiple files onto `scfile.exe`.
 
 ## Arguments
 
 - `FILES`: **List of file paths to be converted**. Multiple files should be separated by **spaces**. Accepts both full and relative paths. **Does not accept directory**.
 
 ## Options
 
-- `-O`, `--output`: **One path to output file or directory**. Can be specified multiple times for different output files or directories. If not specified, file will be saved in the same directory with a new suffix. You can specify multiple `FILES` and a single `--output` directory.
+- `-O`, `--output`: **One path to output file or directory**. Can be specified multiple times for different output files or directories. If not specified, file will be saved in same directory with a new suffix. You can specify multiple `FILES` and a single `--output` directory.
 
 ## Examples
 
 1. Convert a single file:
 
    ```bash
    scfile file.mcsa
    ```
 
-   _Will be saved in the same directory with a new suffix._
+   _Will be saved in same directory with a new suffix._
 
-1. Convert a single file with a specified path or name:
+2. Convert a single file with a specified path or name:
 
    ```bash
    scfile file.mcsa --output path/to/file.obj
    ```
 
-1. Convert multiple files to a specified directory:
+3. Convert multiple files to a specified directory:
 
    ```bash
    scfile file1.mcsa file2.mcsa --output path/to/dir
    ```
 
-1. Convert multiple files with explicitly specified output files:
+4. Convert multiple files with explicitly specified output files:
 
    ```bash
    scfile file1.mcsa file2.mcsa -O 1.obj -O 2.obj
    ```
 
-   _If the count of `FILES` and `--output` is different, as many files as possible will be converted._
+   _If count of `FILES` and `--output` is different, as many files as possible will be converted._
 
-1. Convert all `.mcsa` files in the current directory:
+5. Convert all `.mcsa` files in current directory:
 
    ```bash
    scfile *.mcsa
    ```
 
    _In this case, `--output` accepts only a directory. Subdirectories are not included._
 
-1. Convert all `.mcsa` files with subdirectories to a specified directory:
+6. Convert all `.mcsa` files with subdirectories to a specified directory:
 
    ```bash
    scfile **/*.mcsa -O path/to/dir
    ```
 
    _In this case, `--output` accepts only a directory. With `--output` specified, directory structure is not duplicated._
 
@@ -202,18 +203,18 @@
         obj.save_as("model_1.obj")
         obj.save_as("model_2.obj")
 ```
 
 # 🛠️ Build
 
 > [!IMPORTANT]
-> You will need [poetry](https://python-poetry.org) to do compilation
+> You will need [poetry](https://python-poetry.org) to do compilation.
 
 > [!TIP]
-> Before proceeding, it's recommended to create virtual environment
+> Recommended to create virtual environment.
 >
 > ```bash
 > poetry shell
 > ```
 
 Then install dependencies:
```

### Comparing `sc_file-3.0.6/scfile/__main__.py` & `sc_file-3.0.7/scfile/__main__.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.6/scfile/consts.py` & `sc_file-3.0.7/scfile/consts.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.6/scfile/enums.py` & `sc_file-3.0.7/scfile/enums.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.6/scfile/exceptions/basic.py` & `sc_file-3.0.7/scfile/exceptions/basic.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.6/scfile/exceptions/decode.py` & `sc_file-3.0.7/scfile/exceptions/decode.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.6/scfile/exceptions/mcsa.py` & `sc_file-3.0.7/scfile/exceptions/mcsa.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.6/scfile/exceptions/ol.py` & `sc_file-3.0.7/scfile/exceptions/ol.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.6/scfile/file/base.py` & `sc_file-3.0.7/scfile/file/base.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.6/scfile/file/dds/encoder.py` & `sc_file-3.0.7/scfile/file/dds/encoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.6/scfile/file/dds/structure.py` & `sc_file-3.0.7/scfile/file/dds/structure.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.6/scfile/file/decoder.py` & `sc_file-3.0.7/scfile/file/decoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.6/scfile/file/encoder.py` & `sc_file-3.0.7/scfile/file/encoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.6/scfile/file/mcsa/decoder.py` & `sc_file-3.0.7/scfile/file/mcsa/decoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,21 +50,20 @@
         self.version = self.f.readb(F.F32)
 
         if self.version not in SUPPORTED_VERSIONS:
             raise exc.McsaUnsupportedVersion(self.path, self.version)
 
     def _parse_flags(self):
         self.flags = McsaFlags()
+        self.flags_count = VERSION_FLAGS.get(self.version)
 
-        flags_count = VERSION_FLAGS.get(self.version)
-
-        if not flags_count:
+        if not self.flags_count:
             raise exc.McsaUnsupportedVersion(self.path, self.version)
 
-        for index in range(flags_count):
+        for index in range(self.flags_count):
             self.flags[index] = self.f.readb(F.BOOL)
 
         self.model.flags.texture = self.flags[Flag.TEXTURE]
         self.model.flags.normals = self.flags[Flag.NORMALS]
 
     def _parse_scales(self):
         self.model.scale.position = self.f.readb(F.F32)
```

### Comparing `sc_file-3.0.6/scfile/file/mcsa/flags.py` & `sc_file-3.0.7/scfile/file/mcsa/flags.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.6/scfile/file/mic/decoder.py` & `sc_file-3.0.7/scfile/file/mic/decoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.6/scfile/file/obj/encoder.py` & `sc_file-3.0.7/scfile/file/obj/encoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.6/scfile/file/ol/converter/base.py` & `sc_file-3.0.7/scfile/file/ol/converter/base.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.6/scfile/file/ol/decoder.py` & `sc_file-3.0.7/scfile/file/ol/decoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.6/scfile/io/base.py` & `sc_file-3.0.7/scfile/io/base.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.6/scfile/io/mcsa.py` & `sc_file-3.0.7/scfile/io/mcsa.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.6/scfile/utils/convert.py` & `sc_file-3.0.7/scfile/utils/convert.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.6/scfile/utils/model.py` & `sc_file-3.0.7/scfile/utils/model.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.6/setup.py` & `sc_file-3.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,22 +25,22 @@
  'quicktex>=0.2.0,<0.3.0']
 
 entry_points = \
 {'console_scripts': ['build = build:build']}
 
 setup_kwargs = {
     'name': 'sc-file',
-    'version': '3.0.6',
+    'version': '3.0.7',
     'description': 'Utility & Library for decoding stalcraft assets',
-    'long_description': '# SC FILE\n\nUtility and Library for decoding and converting stalcraft assets files, such as models and textures into well-known formats.\n\nYou can use executable from [Releases](https://github.com/onejeuu/sc-file/releases) page.\n\n> [!IMPORTANT]\n> This utility is designed for artworks and etc \\\n> There is not and will not be any encoding back into game formats\n\n> [!WARNING]\n> Do not use game assets directly \\\n> You can get banned for any changes in game client\n\n# 📁 Formats\n\n| Type    | Source format | Output format |\n| ------- | ------------- | ------------- |\n| Model   | .mcsa         | .obj          |\n| Texture | .ol           | .dds          |\n| Image   | .mic          | .png          |\n\nModel versions supported: 7.0, 8.0, 10.0\n\nTexture formats supported: DXT1, DXT3, DXT5, RGBA8, BGRA8, RGBA32F, DXN_XY\n\nTexture formats unsupported: Cubemaps (hdri, sky)\n\n# 💻 CLI Utility\n\n## Usage\n\nFrom bash:\n\n```bash\nscfile [FILES]... [OPTIONS]\n```\n\n> [!TIP]\n> You can just drag and drop one or multiple files onto `scfile.exe`\n\n## Arguments\n\n- `FILES`: **List of file paths to be converted**. Multiple files should be separated by **spaces**. Accepts both full and relative paths. **Does not accept directory**.\n\n## Options\n\n- `-O`, `--output`: **One path to output file or directory**. Can be specified multiple times for different output files or directories. If not specified, file will be saved in the same directory with a new suffix. You can specify multiple `FILES` and a single `--output` directory.\n\n## Examples\n\n1. Convert a single file:\n\n   ```bash\n   scfile file.mcsa\n   ```\n\n   _Will be saved in the same directory with a new suffix._\n\n1. Convert a single file with a specified path or name:\n\n   ```bash\n   scfile file.mcsa --output path/to/file.obj\n   ```\n\n1. Convert multiple files to a specified directory:\n\n   ```bash\n   scfile file1.mcsa file2.mcsa --output path/to/dir\n   ```\n\n1. Convert multiple files with explicitly specified output files:\n\n   ```bash\n   scfile file1.mcsa file2.mcsa -O 1.obj -O 2.obj\n   ```\n\n   _If the count of `FILES` and `--output` is different, as many files as possible will be converted._\n\n1. Convert all `.mcsa` files in the current directory:\n\n   ```bash\n   scfile *.mcsa\n   ```\n\n   _In this case, `--output` accepts only a directory. Subdirectories are not included._\n\n1. Convert all `.mcsa` files with subdirectories to a specified directory:\n\n   ```bash\n   scfile **/*.mcsa -O path/to/dir\n   ```\n\n   _In this case, `--output` accepts only a directory. With `--output` specified, directory structure is not duplicated._\n\n# 📚 Library\n\n## Install\n\n### Pip\n\n```bash\npip install sc-file -U\n```\n\n### Manual\n\n```bash\ngit clone git@github.com:onejeuu/sc-file.git\n```\n\n```bash\ncd sc-file\n```\n\n```bash\npoetry install\n```\n\n## Usage\n\n### Simple\n\n```python\nfrom scfile import convert\n\n# Output path is optional.\n# Defaults to source path with new suffix.\nconvert.mcsa_to_obj("path/to/model.mcsa", "path/to/model.obj")\nconvert.ol_to_dds("path/to/texture.ol", "path/to/texture.dds")\nconvert.mic_to_png("path/to/image.mic", "path/to/image.png")\n\n# Or determinate it automatically\nconvert.auto("path/to/model.mcsa")\n```\n\n### Advanced\n\nDefault\n\n```python\nfrom scfile.file.data import ModelData\nfrom scfile.file.mcsa.decoder import McsaDecoder\nfrom scfile.file.obj.encoder import ObjEncoder\n\nmcsa = McsaDecoder("model.mcsa")\ndata: ModelData = mcsa.decode()\nmcsa.close() # ? Necessary to close\n\nobj = ObjEncoder(data)\nobj.encode().save("model.obj") # ? Encoder closes after saving\n```\n\nUse encoded content bytes\n\n```python\nobj = ObjEncoder(data)\nobj.encode()\n\nwith open("model.obj", "wb") as fp:\n    fp.write(obj.content)\n\nobj.close() # ? Necessary to close\n```\n\nUse convert methods\n\n```python\nmcsa = McsaDecoder("model.mcsa")\nmcsa.convert_to(ObjEncoder).save("model.obj")\nmcsa.close() # ? Necessary to close\n```\n\n```python\nmcsa = McsaDecoder("model.mcsa")\nmcsa.to_obj().save("model.obj")\nmcsa.close() # ? Necessary to close\n```\n\nUse context manager\n\n```python\nwith McsaDecoder("model.mcsa") as mcsa:\n    data: ModelData = mcsa.decode()\n\nwith ObjEncoder(data) as obj:\n    obj.encode().save("model.obj")\n```\n\nUse context manager + convert methods\n\n```python\nwith McsaDecoder("model.mcsa") as mcsa:\n    mcsa.to_obj().save("model.obj")\n```\n\nSave multiple copies\n\n```python\nwith McsaDecoder("model.mcsa") as mcsa:\n    with mcsa.to_obj() as obj:\n        obj.save_as("model_1.obj")\n        obj.save_as("model_2.obj")\n```\n\n# 🛠️ Build\n\n> [!IMPORTANT]\n> You will need [poetry](https://python-poetry.org) to do compilation\n\n> [!TIP]\n> Before proceeding, it\'s recommended to create virtual environment\n>\n> ```bash\n> poetry shell\n> ```\n\nThen install dependencies:\n\n```bash\npoetry install\n```\n\nAnd run script to compile:\n\n```bash\npoetry run build\n```\n\nExecutable file will be created in `/dist` directory.\n',
+    'long_description': '# SC FILE\n\nUtility and Library for decoding and converting stalcraft assets files, such as models and textures into well-known formats.\n\nDesigned for artworks creation and the like.\n\n> [!NOTE]\n> There is not and will not be encoding back into game formats.\n\n> [!WARNING]\n> Do not use game assets directly. \\\n> Any changes in game client can be detected.\n\nYou can use executable program from [Releases](https://github.com/onejeuu/sc-file/releases) page.\n\n# 📁 Formats\n\n| Type    | Source format | Output format |\n| ------- | ------------- | ------------- |\n| Model   | .mcsa         | .obj          |\n| Texture | .ol           | .dds          |\n| Image   | .mic          | .png          |\n\nModel versions supported: 7.0, 8.0, 10.0\n\nTexture formats supported: DXT1, DXT3, DXT5, RGBA8, BGRA8, RGBA32F, DXN_XY\n\nTexture formats unsupported: Cubemaps (hdri, sky)\n\n# 💻 CLI Utility\n\n## Usage\n\nFrom bash:\n\n```bash\nscfile [FILES]... [OPTIONS]\n```\n\n> [!TIP]\n> You can just drag and drop one or multiple files onto `scfile.exe`.\n\n## Arguments\n\n- `FILES`: **List of file paths to be converted**. Multiple files should be separated by **spaces**. Accepts both full and relative paths. **Does not accept directory**.\n\n## Options\n\n- `-O`, `--output`: **One path to output file or directory**. Can be specified multiple times for different output files or directories. If not specified, file will be saved in same directory with a new suffix. You can specify multiple `FILES` and a single `--output` directory.\n\n## Examples\n\n1. Convert a single file:\n\n   ```bash\n   scfile file.mcsa\n   ```\n\n   _Will be saved in same directory with a new suffix._\n\n2. Convert a single file with a specified path or name:\n\n   ```bash\n   scfile file.mcsa --output path/to/file.obj\n   ```\n\n3. Convert multiple files to a specified directory:\n\n   ```bash\n   scfile file1.mcsa file2.mcsa --output path/to/dir\n   ```\n\n4. Convert multiple files with explicitly specified output files:\n\n   ```bash\n   scfile file1.mcsa file2.mcsa -O 1.obj -O 2.obj\n   ```\n\n   _If count of `FILES` and `--output` is different, as many files as possible will be converted._\n\n5. Convert all `.mcsa` files in current directory:\n\n   ```bash\n   scfile *.mcsa\n   ```\n\n   _In this case, `--output` accepts only a directory. Subdirectories are not included._\n\n6. Convert all `.mcsa` files with subdirectories to a specified directory:\n\n   ```bash\n   scfile **/*.mcsa -O path/to/dir\n   ```\n\n   _In this case, `--output` accepts only a directory. With `--output` specified, directory structure is not duplicated._\n\n# 📚 Library\n\n## Install\n\n### Pip\n\n```bash\npip install sc-file -U\n```\n\n### Manual\n\n```bash\ngit clone git@github.com:onejeuu/sc-file.git\n```\n\n```bash\ncd sc-file\n```\n\n```bash\npoetry install\n```\n\n## Usage\n\n### Simple\n\n```python\nfrom scfile import convert\n\n# Output path is optional.\n# Defaults to source path with new suffix.\nconvert.mcsa_to_obj("path/to/model.mcsa", "path/to/model.obj")\nconvert.ol_to_dds("path/to/texture.ol", "path/to/texture.dds")\nconvert.mic_to_png("path/to/image.mic", "path/to/image.png")\n\n# Or determinate it automatically\nconvert.auto("path/to/model.mcsa")\n```\n\n### Advanced\n\nDefault\n\n```python\nfrom scfile.file.data import ModelData\nfrom scfile.file.mcsa.decoder import McsaDecoder\nfrom scfile.file.obj.encoder import ObjEncoder\n\nmcsa = McsaDecoder("model.mcsa")\ndata: ModelData = mcsa.decode()\nmcsa.close() # ? Necessary to close\n\nobj = ObjEncoder(data)\nobj.encode().save("model.obj") # ? Encoder closes after saving\n```\n\nUse encoded content bytes\n\n```python\nobj = ObjEncoder(data)\nobj.encode()\n\nwith open("model.obj", "wb") as fp:\n    fp.write(obj.content)\n\nobj.close() # ? Necessary to close\n```\n\nUse convert methods\n\n```python\nmcsa = McsaDecoder("model.mcsa")\nmcsa.convert_to(ObjEncoder).save("model.obj")\nmcsa.close() # ? Necessary to close\n```\n\n```python\nmcsa = McsaDecoder("model.mcsa")\nmcsa.to_obj().save("model.obj")\nmcsa.close() # ? Necessary to close\n```\n\nUse context manager\n\n```python\nwith McsaDecoder("model.mcsa") as mcsa:\n    data: ModelData = mcsa.decode()\n\nwith ObjEncoder(data) as obj:\n    obj.encode().save("model.obj")\n```\n\nUse context manager + convert methods\n\n```python\nwith McsaDecoder("model.mcsa") as mcsa:\n    mcsa.to_obj().save("model.obj")\n```\n\nSave multiple copies\n\n```python\nwith McsaDecoder("model.mcsa") as mcsa:\n    with mcsa.to_obj() as obj:\n        obj.save_as("model_1.obj")\n        obj.save_as("model_2.obj")\n```\n\n# 🛠️ Build\n\n> [!IMPORTANT]\n> You will need [poetry](https://python-poetry.org) to do compilation.\n\n> [!TIP]\n> Recommended to create virtual environment.\n>\n> ```bash\n> poetry shell\n> ```\n\nThen install dependencies:\n\n```bash\npoetry install\n```\n\nAnd run script to compile:\n\n```bash\npoetry run build\n```\n\nExecutable file will be created in `/dist` directory.\n',
     'author': 'onejeuu',
     'author_email': 'bloodtrail@beber1k.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://github.com/onejeuu/sc-file',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.11,<3.13',
 }
```

### Comparing `sc_file-3.0.6/PKG-INFO` & `sc_file-3.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 Metadata-Version: 2.1
 Name: sc-file
-Version: 3.0.6
+Version: 3.0.7
 Summary: Utility & Library for decoding stalcraft assets
+Home-page: https://github.com/onejeuu/sc-file
 License: MIT
 Author: onejeuu
 Author-email: bloodtrail@beber1k.ru
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: lz4 (>=4.3.2,<5.0.0)
 Requires-Dist: numpy (>=1.26.3,<2.0.0)
 Requires-Dist: quicktex (>=0.2.0,<0.3.0)
+Project-URL: Documentation, https://github.com/onejeuu/sc-file/?tab=readme-ov-file#usage-1
+Project-URL: Repository, https://github.com/onejeuu/sc-file
 Description-Content-Type: text/markdown
 
 # SC FILE
 
 Utility and Library for decoding and converting stalcraft assets files, such as models and textures into well-known formats.
 
-You can use executable from [Releases](https://github.com/onejeuu/sc-file/releases) page.
+Designed for artworks creation and the like.
 
-> [!IMPORTANT]
-> This utility is designed for artworks and etc \
-> There is not and will not be any encoding back into game formats
+> [!NOTE]
+> There is not and will not be encoding back into game formats.
 
 > [!WARNING]
-> Do not use game assets directly \
-> You can get banned for any changes in game client
+> Do not use game assets directly. \
+> Any changes in game client can be detected.
+
+You can use executable program from [Releases](https://github.com/onejeuu/sc-file/releases) page.
 
 # 📁 Formats
 
 | Type    | Source format | Output format |
 | ------- | ------------- | ------------- |
 | Model   | .mcsa         | .obj          |
 | Texture | .ol           | .dds          |
@@ -50,63 +54,63 @@
 From bash:
 
 ```bash
 scfile [FILES]... [OPTIONS]
 ```
 
 > [!TIP]
-> You can just drag and drop one or multiple files onto `scfile.exe`
+> You can just drag and drop one or multiple files onto `scfile.exe`.
 
 ## Arguments
 
 - `FILES`: **List of file paths to be converted**. Multiple files should be separated by **spaces**. Accepts both full and relative paths. **Does not accept directory**.
 
 ## Options
 
-- `-O`, `--output`: **One path to output file or directory**. Can be specified multiple times for different output files or directories. If not specified, file will be saved in the same directory with a new suffix. You can specify multiple `FILES` and a single `--output` directory.
+- `-O`, `--output`: **One path to output file or directory**. Can be specified multiple times for different output files or directories. If not specified, file will be saved in same directory with a new suffix. You can specify multiple `FILES` and a single `--output` directory.
 
 ## Examples
 
 1. Convert a single file:
 
    ```bash
    scfile file.mcsa
    ```
 
-   _Will be saved in the same directory with a new suffix._
+   _Will be saved in same directory with a new suffix._
 
-1. Convert a single file with a specified path or name:
+2. Convert a single file with a specified path or name:
 
    ```bash
    scfile file.mcsa --output path/to/file.obj
    ```
 
-1. Convert multiple files to a specified directory:
+3. Convert multiple files to a specified directory:
 
    ```bash
    scfile file1.mcsa file2.mcsa --output path/to/dir
    ```
 
-1. Convert multiple files with explicitly specified output files:
+4. Convert multiple files with explicitly specified output files:
 
    ```bash
    scfile file1.mcsa file2.mcsa -O 1.obj -O 2.obj
    ```
 
-   _If the count of `FILES` and `--output` is different, as many files as possible will be converted._
+   _If count of `FILES` and `--output` is different, as many files as possible will be converted._
 
-1. Convert all `.mcsa` files in the current directory:
+5. Convert all `.mcsa` files in current directory:
 
    ```bash
    scfile *.mcsa
    ```
 
    _In this case, `--output` accepts only a directory. Subdirectories are not included._
 
-1. Convert all `.mcsa` files with subdirectories to a specified directory:
+6. Convert all `.mcsa` files with subdirectories to a specified directory:
 
    ```bash
    scfile **/*.mcsa -O path/to/dir
    ```
 
    _In this case, `--output` accepts only a directory. With `--output` specified, directory structure is not duplicated._
 
@@ -219,18 +223,18 @@
         obj.save_as("model_1.obj")
         obj.save_as("model_2.obj")
 ```
 
 # 🛠️ Build
 
 > [!IMPORTANT]
-> You will need [poetry](https://python-poetry.org) to do compilation
+> You will need [poetry](https://python-poetry.org) to do compilation.
 
 > [!TIP]
-> Before proceeding, it's recommended to create virtual environment
+> Recommended to create virtual environment.
 >
 > ```bash
 > poetry shell
 > ```
 
 Then install dependencies:
```

