# Comparing `tmp/docprompt-0.2.6.tar.gz` & `tmp/docprompt-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docprompt-0.2.6.tar", max compression
+gzip compressed data, was "docprompt-0.2.7.tar", max compression
```

## Comparing `docprompt-0.2.6.tar` & `docprompt-0.2.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      585 2023-10-19 02:11:11.194822 docprompt-0.2.6/LICENSE
--rw-r--r--   0        0        0     4917 2024-03-19 03:22:18.145677 docprompt-0.2.6/README.md
--rw-r--r--   0        0        0      593 2024-03-21 01:44:38.876965 docprompt-0.2.6/docprompt/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 16:11:05.761315 docprompt-0.2.6/docprompt/_exec/__init__.py
--rw-r--r--   0        0        0     2395 2024-03-19 02:54:19.707704 docprompt-0.2.6/docprompt/_exec/ghostscript.py
--rw-r--r--   0        0        0        0 2024-03-18 23:40:35.967506 docprompt-0.2.6/docprompt/provenance/__init__.py
--rw-r--r--   0        0        0     9850 2024-03-19 01:27:56.655646 docprompt-0.2.6/docprompt/provenance/search.py
--rw-r--r--   0        0        0     1357 2024-03-19 01:25:52.543395 docprompt-0.2.6/docprompt/provenance/source.py
--rw-r--r--   0        0        0     6054 2024-03-19 01:25:52.543395 docprompt-0.2.6/docprompt/provenance/util.py
--rw-r--r--   0        0        0        0 2024-01-07 23:02:33.076362 docprompt-0.2.6/docprompt/schema/__init__.py
--rw-r--r--   0        0        0     9570 2024-04-13 03:18:18.262506 docprompt-0.2.6/docprompt/schema/document.py
--rw-r--r--   0        0        0     6649 2024-04-13 03:18:18.370507 docprompt-0.2.6/docprompt/schema/layout.py
--rw-r--r--   0        0        0     3764 2024-04-05 21:39:58.248888 docprompt-0.2.6/docprompt/schema/pipeline.py
--rw-r--r--   0        0        0        0 2024-03-12 20:38:52.149979 docprompt-0.2.6/docprompt/tasks/__init__.py
--rw-r--r--   0        0        0     5103 2024-04-05 21:43:53.078902 docprompt-0.2.6/docprompt/tasks/base.py
--rw-r--r--   0        0        0        0 2024-03-12 20:43:10.168189 docprompt-0.2.6/docprompt/tasks/classification/__init__.py
--rw-r--r--   0        0        0     2522 2024-04-05 21:40:07.216964 docprompt-0.2.6/docprompt/tasks/message.py
--rw-r--r--   0        0        0        0 2024-03-14 22:11:01.166853 docprompt-0.2.6/docprompt/tasks/ocr/__init__.py
--rw-r--r--   0        0        0    18558 2024-04-13 03:18:18.370507 docprompt-0.2.6/docprompt/tasks/ocr/gcp.py
--rw-r--r--   0        0        0     1170 2024-04-05 21:40:16.917047 docprompt-0.2.6/docprompt/tasks/ocr/result.py
--rw-r--r--   0        0        0        0 2024-03-17 06:03:50.676445 docprompt-0.2.6/docprompt/tasks/table_extraction/__init__.py
--rw-r--r--   0        0        0      746 2024-04-05 21:43:47.746856 docprompt-0.2.6/docprompt/tasks/table_extraction/base.py
--rw-r--r--   0        0        0        0 2024-03-17 06:15:55.636068 docprompt-0.2.6/docprompt/tasks/table_extraction/providers/__init__.py
--rw-r--r--   0        0        0     3420 2024-04-05 21:53:59.072160 docprompt-0.2.6/docprompt/tasks/table_extraction/providers/claude.py
--rw-r--r--   0        0        0      783 2024-04-05 21:40:26.277127 docprompt-0.2.6/docprompt/tasks/table_extraction/result.py
--rw-r--r--   0        0        0      351 2024-03-14 21:45:48.927780 docprompt-0.2.6/docprompt/utils/__init__.py
--rw-r--r--   0        0        0      421 2023-10-19 04:28:21.331934 docprompt-0.2.6/docprompt/utils/compressor.py
--rw-r--r--   0        0        0     4915 2024-04-05 21:45:37.323801 docprompt-0.2.6/docprompt/utils/date_extraction.py
--rw-r--r--   0        0        0        0 2024-03-18 15:46:16.978297 docprompt-0.2.6/docprompt/utils/raster.py
--rw-r--r--   0        0        0     4015 2024-04-13 03:01:14.714377 docprompt-0.2.6/docprompt/utils/splitter.py
--rw-r--r--   0        0        0     3994 2024-04-05 21:52:56.007611 docprompt-0.2.6/docprompt/utils/util.py
--rw-r--r--   0        0        0     4131 2024-04-13 03:18:31.630612 docprompt-0.2.6/pyproject.toml
--rw-r--r--   0        0        0       39 2023-10-19 02:11:11.222822 docprompt-0.2.6/tests/__init__.py
--rw-r--r--   0        0        0   123638 2024-03-18 16:06:46.485527 docprompt-0.2.6/tests/fixtures/1.pdf
--rw-r--r--   0        0        0  2788655 2024-03-19 01:25:52.543395 docprompt-0.2.6/tests/fixtures/1_ocr.json
--rw-r--r--   0        0        0      202 2024-03-19 01:25:52.543395 docprompt-0.2.6/tests/fixtures.py
--rw-r--r--   0        0        0      830 2024-04-05 21:43:39.530785 docprompt-0.2.6/tests/test_date_extraction.py
--rw-r--r--   0        0        0     2103 2024-04-09 01:42:25.113812 docprompt-0.2.6/tests/test_document.py
--rw-r--r--   0        0        0     1361 2024-04-13 03:17:35.662168 docprompt-0.2.6/tests/test_layout_models.py
--rw-r--r--   0        0        0     1227 2024-04-09 01:36:21.595068 docprompt-0.2.6/tests/test_search.py
--rw-r--r--   0        0        0      878 2024-04-10 19:57:12.041828 docprompt-0.2.6/tests/test_threadpool.py
--rw-r--r--   0        0        0     1003 2024-03-19 01:25:52.547395 docprompt-0.2.6/tests/util.py
--rw-r--r--   0        0        0     7675 1970-01-01 00:00:00.000000 docprompt-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      585 2023-10-19 02:11:11.194822 docprompt-0.2.7/LICENSE
+-rw-r--r--   0        0        0     4917 2024-03-19 03:22:18.145677 docprompt-0.2.7/README.md
+-rw-r--r--   0        0        0      593 2024-03-21 01:44:38.876965 docprompt-0.2.7/docprompt/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-18 16:11:05.761315 docprompt-0.2.7/docprompt/_exec/__init__.py
+-rw-r--r--   0        0        0     2395 2024-03-19 02:54:19.707704 docprompt-0.2.7/docprompt/_exec/ghostscript.py
+-rw-r--r--   0        0        0        0 2024-03-18 23:40:35.967506 docprompt-0.2.7/docprompt/provenance/__init__.py
+-rw-r--r--   0        0        0     9850 2024-03-19 01:27:56.655646 docprompt-0.2.7/docprompt/provenance/search.py
+-rw-r--r--   0        0        0     1357 2024-03-19 01:25:52.543395 docprompt-0.2.7/docprompt/provenance/source.py
+-rw-r--r--   0        0        0     6054 2024-03-19 01:25:52.543395 docprompt-0.2.7/docprompt/provenance/util.py
+-rw-r--r--   0        0        0        0 2024-01-07 23:02:33.076362 docprompt-0.2.7/docprompt/schema/__init__.py
+-rw-r--r--   0        0        0    12278 2024-04-14 04:46:35.191268 docprompt-0.2.7/docprompt/schema/document.py
+-rw-r--r--   0        0        0     6649 2024-04-13 03:18:18.370507 docprompt-0.2.7/docprompt/schema/layout.py
+-rw-r--r--   0        0        0     3764 2024-04-05 21:39:58.248888 docprompt-0.2.7/docprompt/schema/pipeline.py
+-rw-r--r--   0        0        0        0 2024-03-12 20:38:52.149979 docprompt-0.2.7/docprompt/tasks/__init__.py
+-rw-r--r--   0        0        0     5103 2024-04-05 21:43:53.078902 docprompt-0.2.7/docprompt/tasks/base.py
+-rw-r--r--   0        0        0        0 2024-03-12 20:43:10.168189 docprompt-0.2.7/docprompt/tasks/classification/__init__.py
+-rw-r--r--   0        0        0     2522 2024-04-05 21:40:07.216964 docprompt-0.2.7/docprompt/tasks/message.py
+-rw-r--r--   0        0        0        0 2024-03-14 22:11:01.166853 docprompt-0.2.7/docprompt/tasks/ocr/__init__.py
+-rw-r--r--   0        0        0    18558 2024-04-13 03:18:18.370507 docprompt-0.2.7/docprompt/tasks/ocr/gcp.py
+-rw-r--r--   0        0        0     1170 2024-04-05 21:40:16.917047 docprompt-0.2.7/docprompt/tasks/ocr/result.py
+-rw-r--r--   0        0        0        0 2024-03-17 06:03:50.676445 docprompt-0.2.7/docprompt/tasks/table_extraction/__init__.py
+-rw-r--r--   0        0        0      746 2024-04-05 21:43:47.746856 docprompt-0.2.7/docprompt/tasks/table_extraction/base.py
+-rw-r--r--   0        0        0        0 2024-03-17 06:15:55.636068 docprompt-0.2.7/docprompt/tasks/table_extraction/providers/__init__.py
+-rw-r--r--   0        0        0     3420 2024-04-05 21:53:59.072160 docprompt-0.2.7/docprompt/tasks/table_extraction/providers/claude.py
+-rw-r--r--   0        0        0      783 2024-04-05 21:40:26.277127 docprompt-0.2.7/docprompt/tasks/table_extraction/result.py
+-rw-r--r--   0        0        0      351 2024-03-14 21:45:48.927780 docprompt-0.2.7/docprompt/utils/__init__.py
+-rw-r--r--   0        0        0      421 2023-10-19 04:28:21.331934 docprompt-0.2.7/docprompt/utils/compressor.py
+-rw-r--r--   0        0        0     4915 2024-04-05 21:45:37.323801 docprompt-0.2.7/docprompt/utils/date_extraction.py
+-rw-r--r--   0        0        0        0 2024-03-18 15:46:16.978297 docprompt-0.2.7/docprompt/utils/raster.py
+-rw-r--r--   0        0        0     4015 2024-04-13 03:01:14.714377 docprompt-0.2.7/docprompt/utils/splitter.py
+-rw-r--r--   0        0        0     3994 2024-04-05 21:52:56.007611 docprompt-0.2.7/docprompt/utils/util.py
+-rw-r--r--   0        0        0     4131 2024-04-14 04:48:32.080147 docprompt-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-10-19 02:11:11.222822 docprompt-0.2.7/tests/__init__.py
+-rw-r--r--   0        0        0   123638 2024-03-18 16:06:46.485527 docprompt-0.2.7/tests/fixtures/1.pdf
+-rw-r--r--   0        0        0  2788655 2024-03-19 01:25:52.543395 docprompt-0.2.7/tests/fixtures/1_ocr.json
+-rw-r--r--   0        0        0      202 2024-03-19 01:25:52.543395 docprompt-0.2.7/tests/fixtures.py
+-rw-r--r--   0        0        0      830 2024-04-05 21:43:39.530785 docprompt-0.2.7/tests/test_date_extraction.py
+-rw-r--r--   0        0        0     3463 2024-04-14 04:46:35.191268 docprompt-0.2.7/tests/test_document.py
+-rw-r--r--   0        0        0     1361 2024-04-13 03:17:35.662168 docprompt-0.2.7/tests/test_layout_models.py
+-rw-r--r--   0        0        0     1227 2024-04-09 01:36:21.595068 docprompt-0.2.7/tests/test_search.py
+-rw-r--r--   0        0        0      878 2024-04-10 19:57:12.041828 docprompt-0.2.7/tests/test_threadpool.py
+-rw-r--r--   0        0        0     1003 2024-03-19 01:25:52.547395 docprompt-0.2.7/tests/util.py
+-rw-r--r--   0        0        0     7675 1970-01-01 00:00:00.000000 docprompt-0.2.7/PKG-INFO
```

### Comparing `docprompt-0.2.6/LICENSE` & `docprompt-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.6/README.md` & `docprompt-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.6/docprompt/__init__.py` & `docprompt-0.2.7/docprompt/__init__.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.6/docprompt/_exec/ghostscript.py` & `docprompt-0.2.7/docprompt/_exec/ghostscript.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.6/docprompt/provenance/search.py` & `docprompt-0.2.7/docprompt/provenance/search.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.6/docprompt/provenance/source.py` & `docprompt-0.2.7/docprompt/provenance/source.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.6/docprompt/provenance/util.py` & `docprompt-0.2.7/docprompt/provenance/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.6/docprompt/schema/document.py` & `docprompt-0.2.7/docprompt/schema/document.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,35 +3,40 @@
 import tempfile
 from contextlib import contextmanager
 from datetime import datetime
 from functools import cached_property
 from io import BytesIO
 from os import PathLike
 from pathlib import Path
-from typing import Dict, Generator, Optional, Tuple, Union
+from typing import Dict, Generator, Literal, Optional, Tuple, Union
+from pydantic import Field
 
 import magic
 import pypdfium2 as pdfium
 from PIL import Image
 from pydantic import (
     BaseModel,
-    Field,
     PositiveInt,
     PrivateAttr,
     computed_field,
     field_serializer,
     field_validator,
 )
 
 from docprompt._exec.ghostscript import (
     compress_pdf_to_bytes,
 )
+import logging
 
 DEFAULT_DPI = 100
 
+ResizeModes = Literal["thumbnail", "resize"]
+
+logger = logging.getLogger(__name__)
+
 
 def get_page_render_size_from_bytes(
     file_bytes: bytes, page_number: int, dpi: int = DEFAULT_DPI
 ):
     """
     Returns the render size of a page in pixels
     """
@@ -46,46 +51,111 @@
 
     width = int(base_width * dpi / 72)
     height = int(base_height * dpi / 72)
 
     return width, height
 
 
+def resize_image_to_fize_size_limit(
+    image_bytes: bytes,
+    max_file_size_bytes: int,
+    *,
+    resize_mode: ResizeModes = "thumbnail",
+    resize_step_size: float = 0.1,
+):
+    """
+    Incrementally resizes an image until it is under a certain file size
+    """
+
+    if resize_step_size <= 0 or resize_step_size >= 0.5:
+        raise ValueError("resize_step_size must be between 0 and 0.5")
+
+    if len(image_bytes) < max_file_size_bytes:
+        return image_bytes
+
+    output_bytes = image_bytes
+    step_count = 0
+
+    while len(output_bytes) > max_file_size_bytes:
+        image = Image.open(BytesIO(output_bytes))
+
+        new_width = int(image.width * (1 - resize_step_size * step_count))
+        new_height = int(image.height * (1 - resize_step_size * step_count))
+
+        if new_width <= 200 or new_height <= 200:
+            logger.warning(
+                f"Image could not be resized to under {max_file_size_bytes} bytes. Reached {len(output_bytes)} bytes."
+            )
+            break
+
+        if resize_mode == "thumbnail":
+            image.thumbnail((new_width, new_height))
+        elif resize_mode == "resize":
+            image = image.resize((new_width, new_height))
+
+        buffer = BytesIO()
+
+        image.save(buffer, format="PNG", optimize=True)
+
+        output_bytes = buffer.getvalue()
+
+        step_count += 1
+
+    return output_bytes
+
+
 def process_raster_image(
     image_bytes: bytes,
     *,
     do_resize: bool = False,
     resize_width: Optional[int] = None,
     resize_height: Optional[int] = None,
+    resize_mode: ResizeModes = "thumbnail",
     do_convert: bool = True,
     image_covert_mode: str = "L",
     do_quantize: bool = True,
     quantize_color_count: int = 8,
+    max_file_size_bytes: Optional[int] = None,
 ):
-    if not do_resize and not do_quantize and not do_convert:
+    if not do_resize and not do_quantize and not do_convert and not max_file_size_bytes:
         return image_bytes
 
     image = Image.open(BytesIO(image_bytes))
 
     if do_resize:
         if resize_width is None or resize_height is None:
             raise ValueError("Must specify both resize_width and resize_height")
 
-        image = image.resize((resize_width, resize_height))
+        if resize_mode == "resize":
+            image = image.resize((resize_width, resize_height))
+        elif resize_mode == "thumbnail":
+            image.thumbnail((resize_width, resize_height))
+        else:
+            raise ValueError("Invalid resize_mode")
 
     if do_convert:
         image = image.convert(image_covert_mode)
 
     if do_quantize:
         image = image.quantize(colors=quantize_color_count)
 
     buffer = BytesIO()
     image.save(buffer, format="PNG", optimize=True)
 
-    return buffer.getvalue()
+    result = buffer.getvalue()
+
+    if max_file_size_bytes and len(result) > max_file_size_bytes:
+        result = resize_image_to_fize_size_limit(
+            result,
+            max_file_size_bytes,
+            resize_mode=resize_mode,
+            resize_step_size=0.1,
+        )
+
+    return result
 
 
 class PdfDocument(BaseModel):
     """
     Represents a PDF document
     """
 
@@ -190,22 +260,24 @@
 
     def rasterize_page(
         self,
         page_number: int,
         *,
         dpi: int = DEFAULT_DPI,
         downscale_size: Optional[Tuple[int, int]] = None,
+        resize_mode: ResizeModes = "thumbnail",
+        max_file_size_bytes: Optional[int] = None,
         use_cache: bool = True,
         do_convert: bool = False,
         image_covert_mode: str = "L",
         do_quantize: bool = False,
         quantize_color_count: int = 8,
     ) -> bytes:
         """
-        Rasterizes a page of the document using Ghostscript
+        Rasterizes a page of the document using Pdfium
         """
         generated_image = False
 
         if page_number < 0 or page_number > self.num_pages:
             raise ValueError(f"Page number must be between 0 and {self.num_pages}")
 
         if use_cache and self._raster_cache.get(dpi, {}).get(page_number):
@@ -229,39 +301,51 @@
             self._raster_cache[dpi][page_number] = rastered
 
         rastered = process_raster_image(
             rastered,
             do_resize=downscale_size is not None,
             resize_width=downscale_size[0] if downscale_size else None,
             resize_height=downscale_size[1] if downscale_size else None,
+            resize_mode=resize_mode,
             do_convert=do_convert,
             image_covert_mode=image_covert_mode,
             do_quantize=do_quantize,
             quantize_color_count=quantize_color_count,
+            max_file_size_bytes=max_file_size_bytes,
         )
 
         return rastered
 
     def rasterize_page_to_data_uri(
         self,
         page_number: int,
         *,
         dpi: int = DEFAULT_DPI,
         downscale_size: Optional[Tuple[int, int]] = None,
         use_cache: bool = True,
+        do_convert: bool = False,
+        image_covert_mode: str = "L",
+        do_quantize: bool = False,
+        quantize_color_count: int = 8,
+        max_image_file_size: Optional[int] = None,
     ) -> str:
         """
         Rasterizes a page of the document using Pdfium and returns a data URI, which can
         be embedded into HTML or passed to large language models
         """
         image_bytes = self.rasterize_page(
             page_number,
             dpi=dpi,
             downscale_size=downscale_size,
             use_cache=use_cache,
+            do_convert=do_convert,
+            image_covert_mode=image_covert_mode,
+            do_quantize=do_quantize,
+            quantize_color_count=quantize_color_count,
+            max_image_file_size=max_image_file_size,
         )
         return f"data:image/png;base64,{base64.b64encode(image_bytes).decode('utf-8')}"
 
     def rasterize_pdf(
         self,
         dpi: int = DEFAULT_DPI,
         use_cache: bool = True,
```

### Comparing `docprompt-0.2.6/docprompt/schema/layout.py` & `docprompt-0.2.7/docprompt/schema/layout.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.6/docprompt/schema/pipeline.py` & `docprompt-0.2.7/docprompt/schema/pipeline.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.6/docprompt/tasks/base.py` & `docprompt-0.2.7/docprompt/tasks/base.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.6/docprompt/tasks/message.py` & `docprompt-0.2.7/docprompt/tasks/message.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.6/docprompt/tasks/ocr/gcp.py` & `docprompt-0.2.7/docprompt/tasks/ocr/gcp.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.6/docprompt/tasks/ocr/result.py` & `docprompt-0.2.7/docprompt/tasks/ocr/result.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.6/docprompt/tasks/table_extraction/base.py` & `docprompt-0.2.7/docprompt/tasks/table_extraction/base.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.6/docprompt/tasks/table_extraction/providers/claude.py` & `docprompt-0.2.7/docprompt/tasks/table_extraction/providers/claude.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.6/docprompt/tasks/table_extraction/result.py` & `docprompt-0.2.7/docprompt/tasks/table_extraction/result.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.6/docprompt/utils/date_extraction.py` & `docprompt-0.2.7/docprompt/utils/date_extraction.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.6/docprompt/utils/splitter.py` & `docprompt-0.2.7/docprompt/utils/splitter.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.6/docprompt/utils/util.py` & `docprompt-0.2.7/docprompt/utils/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.6/pyproject.toml` & `docprompt-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "docprompt"
-version = "0.2.6"
+version = "0.2.7"
 homepage = "https://github.com/Page-Leaf/docprompt"
 description = "Documents and large language models."
 authors = ["Frankie Colson <frank@pageleaf.io>"]
 readme = "README.md"
 license =  "Apache-2.0"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `docprompt-0.2.6/tests/fixtures/1.pdf` & `docprompt-0.2.7/tests/fixtures/1.pdf`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.6/tests/fixtures/1_ocr.json` & `docprompt-0.2.7/tests/fixtures/1_ocr.json`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.6/tests/test_date_extraction.py` & `docprompt-0.2.7/tests/test_date_extraction.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.6/tests/test_document.py` & `docprompt-0.2.7/tests/test_document.py`

 * *Files 24% similar despite different names*

```diff
@@ -35,27 +35,74 @@
             image_covert_mode=convert_mode,
             do_quantize=True,
             quantize_color_count=quantize_color_count,
         )
         Image.open(io.BytesIO(img_bytes))
 
 
-def test_rasterize_resize():
+def test_rasterize_resize__regular():
     # Fow now just test PIL can open the image
     resize_width = 100
     resize_height = 100
 
     for fixture in PDF_FIXTURES:
         doc = load_document(fixture.get_full_path())
-        img_bytes = doc.rasterize_page(1, downscale_size=(resize_width, resize_height))
+        img_bytes = doc.rasterize_page(
+            1, downscale_size=(resize_width, resize_height), resize_mode="resize"
+        )
         result = Image.open(io.BytesIO(img_bytes))
 
         assert result.size == (resize_width, resize_height)
 
 
+def test_rasterize_resize__thumbnail():
+    # Fow now just test PIL can open the image
+    resize_width = 100
+    resize_height = 100
+
+    for fixture in PDF_FIXTURES:
+        doc = load_document(fixture.get_full_path())
+        img_bytes = doc.rasterize_page(
+            1, downscale_size=(resize_width, resize_height), resize_mode="thumbnail"
+        )
+        result = Image.open(io.BytesIO(img_bytes))
+
+        result_width, result_height = result.size
+
+        assert result_width == resize_width or result_height == resize_height
+
+
+def test_max_image_file_size():
+    for fixture in PDF_FIXTURES:
+        doc = load_document(fixture.get_full_path())
+
+        initial_img_bytes = doc.rasterize_page(1)
+
+        resize_bytes = doc.rasterize_page(
+            1, max_file_size_bytes=len(initial_img_bytes) - 10000
+        )
+
+        assert len(resize_bytes) < len(initial_img_bytes)
+
+
+def test_rasterize_with_optimizations():
+    max_image_size = 1024 * 1024 * 5
+
+    for fixture in PDF_FIXTURES:
+        doc = load_document(fixture.get_full_path())
+
+        no_optimize_img_bytes = doc.rasterize_page(1)
+
+        optimized = doc.rasterize_page(
+            1, do_convert=True, do_quantize=True, max_file_size_bytes=max_image_size
+        )
+
+        assert len(optimized) < len(no_optimize_img_bytes)
+
+
 def test_split():
     doc = load_document(PDF_FIXTURES[0].get_full_path())
 
     new_docs = doc.split(start=2)
 
     assert len(new_docs) == len(doc) - 2
```

### Comparing `docprompt-0.2.6/tests/test_layout_models.py` & `docprompt-0.2.7/tests/test_layout_models.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.6/tests/test_search.py` & `docprompt-0.2.7/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.6/tests/test_threadpool.py` & `docprompt-0.2.7/tests/test_threadpool.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.6/tests/util.py` & `docprompt-0.2.7/tests/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.6/PKG-INFO` & `docprompt-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docprompt
-Version: 0.2.6
+Version: 0.2.7
 Summary: Documents and large language models.
 Home-page: https://github.com/Page-Leaf/docprompt
 License: Apache-2.0
 Author: Frankie Colson
 Author-email: frank@pageleaf.io
 Requires-Python: >=3.8.1,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: docprompt Version: 0.2.6 Summary: Documents and
+Metadata-Version: 2.1 Name: docprompt Version: 0.2.7 Summary: Documents and
 large language models. Home-page: https://github.com/Page-Leaf/docprompt
 License: Apache-2.0 Author: Frankie Colson Author-email: frank@pageleaf.io
 Requires-Python: >=3.8.1,<3.13 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Natural Language :: English Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

