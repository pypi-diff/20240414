# Comparing `tmp/pdfnaut-0.1.0.tar.gz` & `tmp/pdfnaut-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfnaut-0.1.0.tar", last modified: Sat Mar 30 04:27:28 2024, max compression
+gzip compressed data, was "pdfnaut-0.1.1.tar", last modified: Sun Apr 14 17:48:21 2024, max compression
```

## Comparing `pdfnaut-0.1.0.tar` & `pdfnaut-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 04:27:28.259699 pdfnaut-0.1.0/
--rw-rw-rw-   0        0        0    10315 2024-01-02 18:49:05.000000 pdfnaut-0.1.0/LICENSE
--rw-rw-rw-   0        0        0    14394 2024-03-30 04:27:28.254712 pdfnaut-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1550 2024-03-27 23:44:11.000000 pdfnaut-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-30 04:27:28.135389 pdfnaut-0.1.0/pdfnaut/
--rw-rw-rw-   0        0        0      320 2024-03-30 04:23:13.000000 pdfnaut-0.1.0/pdfnaut/__init__.py
--rw-rw-rw-   0        0        0      338 2024-03-24 03:14:43.000000 pdfnaut-0.1.0/pdfnaut/exceptions.py
--rw-rw-rw-   0        0        0     6429 2024-03-30 00:18:33.000000 pdfnaut-0.1.0/pdfnaut/filters.py
-drwxrwxrwx   0        0        0        0 2024-03-30 04:27:28.209838 pdfnaut-0.1.0/pdfnaut/objects/
--rw-rw-rw-   0        0        0      551 2024-03-29 21:44:31.000000 pdfnaut-0.1.0/pdfnaut/objects/__init__.py
--rw-rw-rw-   0        0        0     1632 2024-03-30 00:16:33.000000 pdfnaut-0.1.0/pdfnaut/objects/base.py
--rw-rw-rw-   0        0        0     1638 2024-03-30 00:18:21.000000 pdfnaut-0.1.0/pdfnaut/objects/stream.py
--rw-rw-rw-   0        0        0     1471 2024-03-30 00:48:56.000000 pdfnaut-0.1.0/pdfnaut/objects/xref.py
-drwxrwxrwx   0        0        0        0 2024-03-30 04:27:28.226405 pdfnaut-0.1.0/pdfnaut/parsers/
--rw-rw-rw-   0        0        0      105 2024-03-29 21:48:59.000000 pdfnaut-0.1.0/pdfnaut/parsers/__init__.py
--rw-rw-rw-   0        0        0    20925 2024-03-29 01:45:16.000000 pdfnaut-0.1.0/pdfnaut/parsers/pdf.py
--rw-rw-rw-   0        0        0    12465 2024-03-30 01:41:53.000000 pdfnaut-0.1.0/pdfnaut/parsers/simple.py
--rw-rw-rw-   0        0        0        0 2023-12-28 16:38:46.000000 pdfnaut-0.1.0/pdfnaut/py.typed
--rw-rw-rw-   0        0        0     9191 2024-03-30 03:48:10.000000 pdfnaut-0.1.0/pdfnaut/security_handler.py
--rw-rw-rw-   0        0        0     9646 2024-03-30 03:45:06.000000 pdfnaut-0.1.0/pdfnaut/serializer.py
-drwxrwxrwx   0        0        0        0 2024-03-30 04:27:28.250192 pdfnaut-0.1.0/pdfnaut.egg-info/
--rw-rw-rw-   0        0        0    14394 2024-03-30 04:27:27.000000 pdfnaut-0.1.0/pdfnaut.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      600 2024-03-30 04:27:28.000000 pdfnaut-0.1.0/pdfnaut.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 04:27:27.000000 pdfnaut-0.1.0/pdfnaut.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2024-03-30 04:27:27.000000 pdfnaut-0.1.0/pdfnaut.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-30 04:27:27.000000 pdfnaut-0.1.0/pdfnaut.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1196 2024-03-17 18:27:25.000000 pdfnaut-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-30 04:27:28.259699 pdfnaut-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-30 04:27:28.244580 pdfnaut-0.1.0/tests/
--rw-rw-rw-   0        0        0     1857 2024-03-27 21:59:14.000000 pdfnaut-0.1.0/tests/test_encryption.py
--rw-rw-rw-   0        0        0     3624 2024-03-27 21:50:34.000000 pdfnaut-0.1.0/tests/test_object_parsing.py
--rw-rw-rw-   0        0        0     2709 2024-03-27 21:47:19.000000 pdfnaut-0.1.0/tests/test_parsing_files.py
--rw-rw-rw-   0        0        0     3719 2024-03-27 21:43:26.000000 pdfnaut-0.1.0/tests/test_serializer.py
+drwxrwxrwx   0        0        0        0 2024-04-14 17:48:21.399553 pdfnaut-0.1.1/
+-rw-rw-rw-   0        0        0    10315 2024-01-02 18:49:05.000000 pdfnaut-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0    14726 2024-04-14 17:48:21.396545 pdfnaut-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1880 2024-04-03 04:18:41.000000 pdfnaut-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 17:48:21.250544 pdfnaut-0.1.1/pdfnaut/
+-rw-rw-rw-   0        0        0      320 2024-04-14 17:40:50.000000 pdfnaut-0.1.1/pdfnaut/__init__.py
+-rw-rw-rw-   0        0        0      338 2024-03-24 03:14:43.000000 pdfnaut-0.1.1/pdfnaut/exceptions.py
+-rw-rw-rw-   0        0        0     6429 2024-03-30 00:18:33.000000 pdfnaut-0.1.1/pdfnaut/filters.py
+drwxrwxrwx   0        0        0        0 2024-04-14 17:48:21.339550 pdfnaut-0.1.1/pdfnaut/objects/
+-rw-rw-rw-   0        0        0      551 2024-03-29 21:44:31.000000 pdfnaut-0.1.1/pdfnaut/objects/__init__.py
+-rw-rw-rw-   0        0        0     1632 2024-03-30 00:16:33.000000 pdfnaut-0.1.1/pdfnaut/objects/base.py
+-rw-rw-rw-   0        0        0     1638 2024-03-30 00:18:21.000000 pdfnaut-0.1.1/pdfnaut/objects/stream.py
+-rw-rw-rw-   0        0        0     1471 2024-03-30 00:48:56.000000 pdfnaut-0.1.1/pdfnaut/objects/xref.py
+drwxrwxrwx   0        0        0        0 2024-04-14 17:48:21.358544 pdfnaut-0.1.1/pdfnaut/parsers/
+-rw-rw-rw-   0        0        0      105 2024-03-29 21:48:59.000000 pdfnaut-0.1.1/pdfnaut/parsers/__init__.py
+-rw-rw-rw-   0        0        0    21355 2024-04-12 03:48:21.000000 pdfnaut-0.1.1/pdfnaut/parsers/pdf.py
+-rw-rw-rw-   0        0        0    12503 2024-04-12 02:41:06.000000 pdfnaut-0.1.1/pdfnaut/parsers/simple.py
+-rw-rw-rw-   0        0        0        0 2023-12-28 16:38:46.000000 pdfnaut-0.1.1/pdfnaut/py.typed
+-rw-rw-rw-   0        0        0     9191 2024-03-30 03:48:10.000000 pdfnaut-0.1.1/pdfnaut/security_handler.py
+-rw-rw-rw-   0        0        0     9684 2024-03-30 15:58:40.000000 pdfnaut-0.1.1/pdfnaut/serializer.py
+drwxrwxrwx   0        0        0        0 2024-04-14 17:48:21.384545 pdfnaut-0.1.1/pdfnaut.egg-info/
+-rw-rw-rw-   0        0        0    14726 2024-04-14 17:48:21.000000 pdfnaut-0.1.1/pdfnaut.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      600 2024-04-14 17:48:21.000000 pdfnaut-0.1.1/pdfnaut.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 17:48:21.000000 pdfnaut-0.1.1/pdfnaut.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2024-04-14 17:48:21.000000 pdfnaut-0.1.1/pdfnaut.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-14 17:48:21.000000 pdfnaut-0.1.1/pdfnaut.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1198 2024-04-14 17:40:42.000000 pdfnaut-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-14 17:48:21.400546 pdfnaut-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-14 17:48:21.377548 pdfnaut-0.1.1/tests/
+-rw-rw-rw-   0        0        0     1857 2024-03-27 21:59:14.000000 pdfnaut-0.1.1/tests/test_encryption.py
+-rw-rw-rw-   0        0        0     3726 2024-04-12 02:42:40.000000 pdfnaut-0.1.1/tests/test_object_parsing.py
+-rw-rw-rw-   0        0        0     2673 2024-04-11 22:31:30.000000 pdfnaut-0.1.1/tests/test_parsing_files.py
+-rw-rw-rw-   0        0        0     3719 2024-03-27 21:43:26.000000 pdfnaut-0.1.1/tests/test_serializer.py
```

### Comparing `pdfnaut-0.1.0/LICENSE` & `pdfnaut-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfnaut-0.1.0/PKG-INFO` & `pdfnaut-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pdfnaut
-Version: 0.1.0
-Summary: Parse PDFs with ease
+Version: 0.1.1
+Summary: Explore PDFs with ease
 Author: Angel Carias
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -200,14 +200,19 @@
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: sphinx-design; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 
 # pdfnaut
 
+[![Documentation Status](https://readthedocs.org/projects/pdfnaut/badge/?version=latest)](https://pdfnaut.readthedocs.io/en/latest/?badge=latest)
+![PyPI - License](https://img.shields.io/pypi/l/pdfnaut)
+![PyPI - Downloads](https://img.shields.io/pypi/dw/pdfnaut)
+![PyPI - Version](https://img.shields.io/pypi/v/pdfnaut)
+
 > [!Warning]
 > pdfnaut is currently in an early stage of development and has only been tested with a small set of compliant documents. Expect bugs or issues.
 
 pdfnaut is a Python library for parsing PDF 1.7 files.
 
 pdfnaut provides a low-level interface for reading and writing PDF objects as defined in the [PDF 1.7 specification](https://opensource.adobe.com/dc-acrobat-sdk-docs/pdfstandards/PDF32000_2008.pdf). pdfnaut currently does not attempt to deviate from the specification. There's no guarantee that valid documents not fully conforming to the standard will be processed correctly.
 
@@ -221,15 +226,15 @@
     # Get the pages object from the trailer
     root = pdf.resolve_reference(pdf.trailer["Root"])
     pages = pdf.resolve_reference(root["Pages"])
     
     # Get the first page contents
     first_page = pdf.resolve_reference(pages["Kids"][0])
     first_page_stream = pdf.resolve_reference(first_page["Contents"])
-    print(first_page_stream.contents)
+    print(first_page_stream.decompress())
 ```
 
 ## Coverage
 
 The following tracks coverage of certain portions of the PDF standard.
 
 - Compression filters: **Supported** (only FlateDecode, ASCII85Decode, and ASCIIHexDecode for now)
```

### Comparing `pdfnaut-0.1.0/README.md` & `pdfnaut-0.1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # pdfnaut
 
+[![Documentation Status](https://readthedocs.org/projects/pdfnaut/badge/?version=latest)](https://pdfnaut.readthedocs.io/en/latest/?badge=latest)
+![PyPI - License](https://img.shields.io/pypi/l/pdfnaut)
+![PyPI - Downloads](https://img.shields.io/pypi/dw/pdfnaut)
+![PyPI - Version](https://img.shields.io/pypi/v/pdfnaut)
+
 > [!Warning]
 > pdfnaut is currently in an early stage of development and has only been tested with a small set of compliant documents. Expect bugs or issues.
 
 pdfnaut is a Python library for parsing PDF 1.7 files.
 
 pdfnaut provides a low-level interface for reading and writing PDF objects as defined in the [PDF 1.7 specification](https://opensource.adobe.com/dc-acrobat-sdk-docs/pdfstandards/PDF32000_2008.pdf). pdfnaut currently does not attempt to deviate from the specification. There's no guarantee that valid documents not fully conforming to the standard will be processed correctly.
 
@@ -17,15 +22,15 @@
     # Get the pages object from the trailer
     root = pdf.resolve_reference(pdf.trailer["Root"])
     pages = pdf.resolve_reference(root["Pages"])
     
     # Get the first page contents
     first_page = pdf.resolve_reference(pages["Kids"][0])
     first_page_stream = pdf.resolve_reference(first_page["Contents"])
-    print(first_page_stream.contents)
+    print(first_page_stream.decompress())
 ```
 
 ## Coverage
 
 The following tracks coverage of certain portions of the PDF standard.
 
 - Compression filters: **Supported** (only FlateDecode, ASCII85Decode, and ASCIIHexDecode for now)
```

### Comparing `pdfnaut-0.1.0/pdfnaut/filters.py` & `pdfnaut-0.1.1/pdfnaut/filters.py`

 * *Files identical despite different names*

### Comparing `pdfnaut-0.1.0/pdfnaut/objects/__init__.py` & `pdfnaut-0.1.1/pdfnaut/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfnaut-0.1.0/pdfnaut/objects/base.py` & `pdfnaut-0.1.1/pdfnaut/objects/base.py`

 * *Files identical despite different names*

### Comparing `pdfnaut-0.1.0/pdfnaut/objects/stream.py` & `pdfnaut-0.1.1/pdfnaut/objects/stream.py`

 * *Files identical despite different names*

### Comparing `pdfnaut-0.1.0/pdfnaut/objects/xref.py` & `pdfnaut-0.1.1/pdfnaut/objects/xref.py`

 * *Files identical despite different names*

### Comparing `pdfnaut-0.1.0/pdfnaut/parsers/pdf.py` & `pdfnaut-0.1.1/pdfnaut/parsers/pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,27 +26,27 @@
 
 
 class PdfParser:
     """A parser that can completely parse a PDF document.
     
     It consumes the PDF's cross-reference tables and trailers. It merges the tables
     into a single one and provides an interface to individually parse each indirect 
-    object using :class:`PdfTokenizer`."""
+    object using :class:`~pdfnaut.parsers.simple.PdfTokenizer`."""
 
     def __init__(self, data: bytes) -> None:
         self._tokenizer = PdfTokenizer(data)
-        self._trailers: list[dict[str, Any]] = []
 
-        self.update_xrefs: list[PdfXRefTable] = []
-        """A list of all XRef tables in the document (the most recent first)"""
+        self.updates: list[tuple[PdfXRefTable, dict[str, Any]]] = []
+        """A list of all incremental updates present in the document. The items are two-element 
+        tuples: first, the XRef table; second, the trailer. (most recent/last update first)"""
 
         self.trailer: dict[str, Any] = {}
         """The most recent trailer in the PDF document.
         
-        For details on the contents of the trailer, see § 7.5.5 File Trailer of the PDF spec.
+        For details on the contents of the trailer, see ``§ 7.5.5 File Trailer`` in the PDF spec.
         """
 
         self.xref: dict[tuple[int, int], PdfXRefEntry] = {}
         """A cross-reference mapping combining the entries of all XRef tables present 
         in the document.
         
         The key is a tuple of two integers: object number and generation number. 
@@ -57,15 +57,15 @@
         """The document's PDF version as seen in the header.
         
         To retrieve the PDF's version properly, access the Version entry part of the 
         document catalog. If not present, you can reliably depend on the header.
         """
 
         self.security_handler = None
-        """The document's standard security handler if any, as specified in the Encrypt 
+        """The document's standard security handler, if any, as specified in the Encrypt 
         dictionary of the PDF trailer.
 
         This field being set indicates that a supported security handler was used for
         encryption. If not set, the parser will not attempt to decrypt this document.
         """
 
         self._encryption_key = None
@@ -89,25 +89,24 @@
         if start_xref is None:
             start_xref = self.lookup_xref_start()
 
         # Move to the offset where the XRef and trailer are
         self._tokenizer.position = start_xref
         xref, trailer = self.parse_xref_and_trailer()
 
-        self.update_xrefs.append(xref)
-        self._trailers.append(trailer)
+        self.updates.append((xref, trailer))
 
         if "Prev" in trailer:
             # More XRefs were found. Recurse!
             self._tokenizer.position = 0
             self.parse(trailer["Prev"])
         else:
             # That's it. Merge them together.
             self.xref = self.get_merged_xrefs()
-            self.trailer = self._trailers[0]
+            self.trailer = self.updates[0][1]
 
         # Is the document encrypted with a standard security handler?
         if "Encrypt" in self.trailer:
             encryption = cast("dict[str, Any]", 
                 self.resolve_reference(_E) if isinstance((_E := self.trailer["Encrypt"]), PdfIndirectRef) else _E)
             
             if encryption["Filter"].value == b"Standard":
@@ -118,31 +117,39 @@
         header = self._tokenizer.parse_comment()
         mat = re.match(rb"PDF-(?P<major>\d+).(?P<minor>\d+)", header.value)
         if mat:
             return f"{mat.group('major').decode()}.{mat.group('minor').decode()}"
 
         raise PdfParseError("Expected PDF header at start of file.")
     
+    def build_xref_map(self, xref: PdfXRefTable) -> dict[tuple[int, int], PdfXRefEntry]:
+        """Creates a dictionary mapping references to XRef entries in the document."""
+        entry_map: dict[tuple[int, int], PdfXRefEntry] = {}
+
+        for section in xref.sections:
+            for idx, entry in enumerate(section.entries, section.first_obj_number):
+                if isinstance(entry, FreeXRefEntry):
+                    gen = entry.gen_if_used_again
+                elif isinstance(entry, InUseXRefEntry):
+                    gen = entry.generation
+                else:
+                    gen = 0 # compressed entries
+
+                entry_map[(idx, gen)] = entry
+
+        return entry_map
+
     def get_merged_xrefs(self) -> dict[tuple[int, int], PdfXRefEntry]:
         """Combines all update XRef tables in the document into a cross-reference mapping
         that includes all entries."""
         entry_map: dict[tuple[int, int], PdfXRefEntry] = {}
 
-        # from least recent
-        for xref in self.update_xrefs[::-1]:
-            for section in xref.sections:
-                for idx, entry in enumerate(section.entries, section.first_obj_number):
-                    if isinstance(entry, FreeXRefEntry):
-                        gen = entry.gen_if_used_again
-                    elif isinstance(entry, InUseXRefEntry):
-                        gen = entry.generation
-                    else:
-                        gen = 0 # compressed entries
-                    
-                    entry_map[(idx, gen)] = entry
+        # from least recent to most recent
+        for xref, _ in self.updates[::-1]:    
+            entry_map.update(self.build_xref_map(xref))        
 
         return entry_map
 
     def lookup_xref_start(self) -> int:
         """Scans through the PDF until it finds the XRef offset then returns it"""
         contents = bytearray()
 
@@ -195,15 +202,15 @@
         return trailer
 
     def parse_simple_xref(self) -> PdfXRefTable:
         """Parses a standard, uncompressed XRef table of the format described in 
         ``§ 7.5.4 Cross-Reference Table`` in the PDF spec.
 
         If ``startxref`` points to an XRef object, :meth:`.parse_compressed_xref`
-        is called instead.
+        should be called instead.
         """
         self._tokenizer.advance(4)
         self._tokenizer.advance_whitespace()
 
         table = PdfXRefTable([])
 
         while not self._tokenizer.at_end():
@@ -276,15 +283,15 @@
                     section.entries.append(CompressedXRefEntry(objstm_number=second, 
                                                                index_within=third))
 
             table.sections.append(section)
 
         return table, xref_stream.details
 
-    def parse_indirect_object(self, xref_entry: InUseXRefEntry) -> PdfObject | PdfStream | None:
+    def parse_indirect_object(self, xref_entry: InUseXRefEntry) -> PdfObject | PdfStream:
         """Parses an indirect object not within an object stream, or basically, an object 
         that is directly referred to by an ``xref_entry``"""
         self._tokenizer.position = xref_entry.offset
         self._tokenizer.advance_whitespace()
         mat = re.match(rb"(?P<num>\d+)\s+(?P<gen>\d+)\s+obj", 
                        self._tokenizer.current_to_eol)
         if not mat:
@@ -311,15 +318,15 @@
             tok = cast("dict[str, Any]", tok)
             length = tok["Length"]
             if isinstance(length, PdfIndirectRef):
                 _current = self._tokenizer.position
                 length = self.resolve_reference(length)
                 self._tokenizer.position = _current 
             if not isinstance(length, int):
-                raise PdfParseError(f"\\Length entry of stream extent not an integer")
+                raise PdfParseError("\\Length entry of stream extent not an integer")
 
             stream = PdfStream(tok, self.parse_stream(xref_entry, length))
             if indirect_ref is None:
                 return stream
             return self._get_decrypted(stream, indirect_ref)
 
         return self._get_decrypted(tok, indirect_ref) # type: ignore
@@ -383,16 +390,16 @@
         self._tokenizer.advance(len(contents))
 
         # Same check as earlier
         pos, eol = self._tokenizer.next_eol()
         if pos == self._tokenizer.position and eol != "\r":
             self._tokenizer.advance(len(eol))
 
-        # Get the offset of the next XRef entry directly following the current one
         if self.xref:
+            # As a bounds check, we get the offset of the entry directly following the current one.
             index_after = list(self.xref.values()).index(xref_entry)
             next_entry_hold = filter(
                 lambda e: isinstance(e, InUseXRefEntry) and e.offset > xref_entry.offset, 
                 list(self.xref.values())[index_after + 1:]
             )
         else:
             # The stream being parsed is (most likely) part of an XRef object
@@ -409,26 +416,25 @@
         self._tokenizer.advance_whitespace()
         # Have we not reached the end?
         if not self._tokenizer.advance_if_next(b"endstream"):
             raise PdfParseError("\\Length key in stream extent does not match end of stream.")
         
         return contents
 
-    def resolve_reference(self, reference: PdfIndirectRef | tuple[int, int]):
+    def resolve_reference(self, reference: PdfIndirectRef | tuple[int, int]) -> PdfObject | PdfStream | PdfNull:
         """Resolves a reference into the indirect object it points to.
         
         Arguments:
-            reference (int | :class:`PdfIndirectRef`): 
+            reference (:class:`.PdfIndirectRef` | tuple[int, int]): 
                 An indirect reference object or a tuple of two integers representing, 
                 in order, the object number and the generation number.
-
+  
         Returns:
-            A PDF object if the reference was found, otherwise :class:`PdfNull`.
+            A PDF object if the reference was found, otherwise :class:`.PdfNull`.
         """
-        
         if isinstance(reference, tuple):
             root_entry = self.xref.get(reference)
         else:
             root_entry = self.xref.get((reference.object_number, reference.generation))
         
         if root_entry is None:
             return PdfNull()
```

### Comparing `pdfnaut-0.1.0/pdfnaut/parsers/simple.py` & `pdfnaut-0.1.1/pdfnaut/parsers/simple.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from __future__ import annotations
 
 import re
 from typing import Any
 
-from ..objects.base import (
-    PdfHexString, PdfName, PdfNull, PdfComment, 
-    PdfIndirectRef, PdfObject, PdfOperator
-)
+from ..objects.base import (PdfHexString, PdfName, PdfNull, PdfComment, 
+                            PdfIndirectRef, PdfObject, PdfOperator)
 
 # as defined in § 7.2.2 Character Set, Table 1 & Table 2
 DELIMITERS = b"()<>[]{}/%"
 WHITESPACE = b"\x00\t\n\x0c\r "
 
 # as defined in § 7.3.4.2 Literal Strings, Table 3
 STRING_ESCAPE = {
@@ -78,15 +76,15 @@
         if self.current + self.peek(len(keyword) - 1) == keyword:
             self.advance(len(keyword))
             return True
         return False
     
     def advance_whitespace(self) -> None:
         """Advances through PDF whitespace."""
-        while self.current in WHITESPACE:
+        while self.current in WHITESPACE and not self.at_end():
             self.advance()
 
     def next_eol(self) -> tuple[int, str]:
         """Returns a tuple containing the position where the next End-Of-Line 
         Marker occurs along with the EOL marker itself. If none is found, ``(-1, "")``
         is returned.
```

### Comparing `pdfnaut-0.1.0/pdfnaut/security_handler.py` & `pdfnaut-0.1.1/pdfnaut/security_handler.py`

 * *Files identical despite different names*

### Comparing `pdfnaut-0.1.0/pdfnaut/serializer.py` & `pdfnaut-0.1.1/pdfnaut/serializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Literal, Any
 from collections import defaultdict
 
 from .objects.stream import PdfStream
 from .objects.xref import PdfXRefSubsection, PdfXRefTable, FreeXRefEntry, InUseXRefEntry
 from .objects.base import (PdfComment, PdfIndirectRef, PdfObject, PdfNull, PdfName,
                            PdfHexString)
```

### Comparing `pdfnaut-0.1.0/pdfnaut.egg-info/PKG-INFO` & `pdfnaut-0.1.1/pdfnaut.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pdfnaut
-Version: 0.1.0
-Summary: Parse PDFs with ease
+Version: 0.1.1
+Summary: Explore PDFs with ease
 Author: Angel Carias
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -200,14 +200,19 @@
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: sphinx-design; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 
 # pdfnaut
 
+[![Documentation Status](https://readthedocs.org/projects/pdfnaut/badge/?version=latest)](https://pdfnaut.readthedocs.io/en/latest/?badge=latest)
+![PyPI - License](https://img.shields.io/pypi/l/pdfnaut)
+![PyPI - Downloads](https://img.shields.io/pypi/dw/pdfnaut)
+![PyPI - Version](https://img.shields.io/pypi/v/pdfnaut)
+
 > [!Warning]
 > pdfnaut is currently in an early stage of development and has only been tested with a small set of compliant documents. Expect bugs or issues.
 
 pdfnaut is a Python library for parsing PDF 1.7 files.
 
 pdfnaut provides a low-level interface for reading and writing PDF objects as defined in the [PDF 1.7 specification](https://opensource.adobe.com/dc-acrobat-sdk-docs/pdfstandards/PDF32000_2008.pdf). pdfnaut currently does not attempt to deviate from the specification. There's no guarantee that valid documents not fully conforming to the standard will be processed correctly.
 
@@ -221,15 +226,15 @@
     # Get the pages object from the trailer
     root = pdf.resolve_reference(pdf.trailer["Root"])
     pages = pdf.resolve_reference(root["Pages"])
     
     # Get the first page contents
     first_page = pdf.resolve_reference(pages["Kids"][0])
     first_page_stream = pdf.resolve_reference(first_page["Contents"])
-    print(first_page_stream.contents)
+    print(first_page_stream.decompress())
 ```
 
 ## Coverage
 
 The following tracks coverage of certain portions of the PDF standard.
 
 - Compression filters: **Supported** (only FlateDecode, ASCII85Decode, and ASCIIHexDecode for now)
```

### Comparing `pdfnaut-0.1.0/pdfnaut.egg-info/SOURCES.txt` & `pdfnaut-0.1.1/pdfnaut.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdfnaut-0.1.0/pyproject.toml` & `pdfnaut-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "pdfnaut"
-version = "0.1.0"
-description = "Parse PDFs with ease"
+version = "0.1.1"
+description = "Explore PDFs with ease"
 authors = [
     { name = "Angel Carias" }
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pdfnaut-0.1.0/tests/test_encryption.py` & `pdfnaut-0.1.1/tests/test_encryption.py`

 * *Files identical despite different names*

### Comparing `pdfnaut-0.1.0/tests/test_object_parsing.py` & `pdfnaut-0.1.1/tests/test_object_parsing.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,92 +5,96 @@
 from typing import cast
 
 from pdfnaut.parsers import PdfTokenizer
 from pdfnaut.objects import PdfName, PdfIndirectRef, PdfHexString, PdfNull, PdfComment
 
 
 def test_null_and_boolean() -> None:
-    parser = PdfTokenizer(b"null true false")
-    tokens = list(parser)
+    lexer = PdfTokenizer(b"null true false")
+    tokens = list(lexer)
 
     assert isinstance(tokens[0], PdfNull)
     assert tokens[1] is True and tokens[2] is False
 
 
 def test_numeric() -> None:
-    parser = PdfTokenizer(b"-1 +25 46 -32.591 +52.871 3.1451")
-    tokens = list(parser)
+    lexer = PdfTokenizer(b"-1 +25 46 -32.591 +52.871 3.1451")
+    tokens = list(lexer)
 
     assert tokens == [-1, 25, 46, -32.591, 52.871, 3.1451]
 
 
 def test_name_object() -> None:
-    parser = PdfTokenizer(b"/Type /SomeR@ndomK*y /Lime#20Green / /F#23")
-    tokens = list(parser)
+    lexer = PdfTokenizer(b"/Type /SomeR@ndomK*y /Lime#20Green / /F#23")
+    tokens = list(lexer)
     assert tokens == [PdfName(b"Type"), PdfName(b"SomeR@ndomK*y"), PdfName(b"Lime Green"), 
                       PdfName(b""), PdfName(b"F#")]
 
 
 def test_literal_string() -> None:
     # Basic string
-    parser = PdfTokenizer(b"(The quick brown fox jumps over the lazy dog.)")
-    assert parser.next_token() == b"The quick brown fox jumps over the lazy dog."
+    lexer = PdfTokenizer(b"(The quick brown fox jumps over the lazy dog.)")
+    assert lexer.next_token() == b"The quick brown fox jumps over the lazy dog."
 
     # String with nested parentheses
-    parser = PdfTokenizer(b"(This is a string with a (few) nested ((parentheses)))")
-    assert parser.next_token() == b"This is a string with a (few) nested ((parentheses))"
+    lexer = PdfTokenizer(b"(This is a string with a (few) nested ((parentheses)))")
+    assert lexer.next_token() == b"This is a string with a (few) nested ((parentheses))"
 
     # String continued in next line
-    parser = PdfTokenizer(b"(This is a string that is \r\n"
+    lexer = PdfTokenizer(b"(This is a string that is \r\n"
                                 b"continued on the next line)")
-    assert parser.next_token() == b"This is a string that is \r\ncontinued on the next line"
+    assert lexer.next_token() == b"This is a string that is \r\ncontinued on the next line"
 
     # String ending with a \ at the EOL and followed next line
-    parser = PdfTokenizer(b"(This is a string \\\r\nwith no newlines.)")
-    assert parser.next_token() == b"This is a string with no newlines."
+    lexer = PdfTokenizer(b"(This is a string \\\r\nwith no newlines.)")
+    assert lexer.next_token() == b"This is a string with no newlines."
 
     # String with escape characters
-    parser = PdfTokenizer(b"(This is a string with a \\t tab character and a \\053 plus.))")
-    assert parser.next_token() == b"This is a string with a \t tab character and a + plus."
+    lexer = PdfTokenizer(b"(This is a string with a \\t tab character and a \\053 plus.))")
+    assert lexer.next_token() == b"This is a string with a \t tab character and a + plus."
 
 
 def test_hex_string() -> None:
-    parser = PdfTokenizer(b"<A5B2FF><6868ADE>")
-    tokens = cast("list[PdfHexString]", list(parser))
+    lexer = PdfTokenizer(b"<A5B2FF><6868ADE>")
+    tokens = cast("list[PdfHexString]", list(lexer))
 
     assert tokens[0].raw == b"A5B2FF" and tokens[1].raw == b"6868ADE0" 
 
 
 def test_dictionary() -> None:
-    parser = PdfTokenizer(b"""<< /Type /Catalog /Metadata 2 0 R /Pages 3 0 R >>""")
-    assert parser.next_token() == { 
+    lexer = PdfTokenizer(b"""<< /Type /Catalog /Metadata 2 0 R /Pages 3 0 R >>""")
+    assert lexer.next_token() == { 
         "Type": PdfName(b"Catalog"), 
         "Metadata": PdfIndirectRef(2, 0), 
         "Pages": PdfIndirectRef(3, 0) 
     }
 
 
 def test_comment() -> None:
     # This also counts as an EOL test
-    parser = PdfTokenizer(b"% This is a comment\r\n"
+    lexer = PdfTokenizer(b"% This is a comment\r\n"
                                 b"12 % This is another comment\r"
                                 b"25\n")
-    assert isinstance(com := next(parser), PdfComment) \
+    assert isinstance(com := next(lexer), PdfComment) \
         and com.value == b" This is a comment"
-    assert next(parser) == 12
-    assert isinstance(com := next(parser), PdfComment) and \
+    assert next(lexer) == 12
+    assert isinstance(com := next(lexer), PdfComment) and \
         com.value == b" This is another comment"
-    assert next(parser) == 25
+    assert next(lexer) == 25
 
-    parser = PdfTokenizer(b"% This is a comment ending with \\r\r")
-    assert isinstance(com := parser.next_token(), PdfComment) \
+    lexer = PdfTokenizer(b"% This is a comment ending with \\r\r")
+    assert isinstance(com := lexer.next_token(), PdfComment) \
         and com.value == b" This is a comment ending with \\r"
 
 
 def test_array() -> None:
     # Simple array
-    parser = PdfTokenizer(b"[45 <</Size 40>> (42)]") 
-    assert parser.next_token() == [45, {"Size": 40}, b"42"]
+    lexer = PdfTokenizer(b"[45 <</Size 40>> (42)]") 
+    assert lexer.next_token() == [45, {"Size": 40}, b"42"]
     
     # Nested array
-    parser = PdfTokenizer(b"[/XYZ [45 32 76] /Great]")
-    assert parser.next_token() == [PdfName(b"XYZ"), [45, 32, 76], PdfName(b"Great")]
+    lexer = PdfTokenizer(b"[/XYZ [45 32 76] /Great]")
+    assert lexer.next_token() == [PdfName(b"XYZ"), [45, 32, 76], PdfName(b"Great")]
+
+def test_indirect_reference() -> None:
+    lexer = PdfTokenizer(b"2 0 R")
+    assert lexer.next_token() == PdfIndirectRef(2, 0)
```

### Comparing `pdfnaut-0.1.0/tests/test_parsing_files.py` & `pdfnaut-0.1.1/tests/test_parsing_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 def test_pdf_with_incremental() -> None:
     """Tests whether an incremental PDF is parsed correctly. Basically, whether the 
     correct trailer is provided and whether the XRefs are merged."""
     with open("tests/docs/pdf2-incremental.pdf", "rb") as data:
         parser = PdfParser(data.read())
         parser.parse()
         
-        assert len(parser.update_xrefs) == 2 and len(parser._trailers) == 2
+        assert len(parser.updates) == 2
         assert parser.trailer["Size"] == len(parser.xref)
 
 
 def test_pdf_with_xref_stream() -> None:
     """Tests a PDF document with a compressed XRef stream"""
     with open("tests/docs/compressed-xref.pdf", "rb") as data:
         parser = PdfParser(data.read())
```

### Comparing `pdfnaut-0.1.0/tests/test_serializer.py` & `pdfnaut-0.1.1/tests/test_serializer.py`

 * *Files identical despite different names*

