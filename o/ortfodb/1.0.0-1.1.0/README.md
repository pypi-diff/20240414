# Comparing `tmp/ortfodb-1.0.0.tar.gz` & `tmp/ortfodb-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ortfodb-1.0.0.tar", max compression
+gzip compressed data, was "ortfodb-1.1.0.tar", max compression
```

## Comparing `ortfodb-1.0.0.tar` & `ortfodb-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      209 2024-04-12 21:43:37.285597 ortfodb-1.0.0/README.md
--rw-r--r--   0        0        0      434 2024-04-12 21:42:27.066289 ortfodb-1.0.0/ortfodb/__init__.py
--rw-r--r--   0        0        0     7128 2024-04-13 16:57:38.069979 ortfodb-1.0.0/ortfodb/configuration.py
--rw-r--r--   0        0        0    14616 2024-04-13 16:57:38.953345 ortfodb-1.0.0/ortfodb/database.py
--rw-r--r--   0        0        0     2791 2024-04-13 16:57:39.766708 ortfodb-1.0.0/ortfodb/tags.py
--rw-r--r--   0        0        0     2311 2024-04-13 16:57:40.596738 ortfodb-1.0.0/ortfodb/technologies.py
--rw-r--r--   0        0        0      301 2024-04-13 16:57:41.243429 ortfodb-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 ortfodb-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      209 2024-04-12 21:43:37.285597 ortfodb-1.1.0/README.md
+-rw-r--r--   0        0        0      434 2024-04-12 21:42:27.066289 ortfodb-1.1.0/ortfodb/__init__.py
+-rw-r--r--   0        0        0     7927 2024-04-14 11:44:04.466338 ortfodb-1.1.0/ortfodb/configuration.py
+-rw-r--r--   0        0        0    14616 2024-04-14 11:44:05.373039 ortfodb-1.1.0/ortfodb/database.py
+-rw-r--r--   0        0        0     2791 2024-04-14 11:44:06.206403 ortfodb-1.1.0/ortfodb/tags.py
+-rw-r--r--   0        0        0     2311 2024-04-14 11:44:07.006433 ortfodb-1.1.0/ortfodb/technologies.py
+-rw-r--r--   0        0        0      301 2024-04-14 11:44:07.656458 ortfodb-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 ortfodb-1.1.0/PKG-INFO
```

### Comparing `ortfodb-1.0.0/ortfodb/configuration.py` & `ortfodb-1.1.0/ortfodb/configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Any, TypeVar, Callable, Type, cast
+from typing import List, Any, Dict, Optional, TypeVar, Callable, Type, cast
 
 
 T = TypeVar("T")
 
 
 def from_list(f: Callable[[Any], T], x: Any) -> List[T]:
     assert isinstance(x, list)
@@ -20,14 +20,33 @@
 
 
 def from_int(x: Any) -> int:
     assert isinstance(x, int) and not isinstance(x, bool)
     return x
 
 
+def from_dict(f: Callable[[Any], T], x: Any) -> Dict[str, T]:
+    assert isinstance(x, dict)
+    return { k: f(v) for (k, v) in x.items() }
+
+
+def from_none(x: Any) -> Any:
+    assert x is None
+    return x
+
+
+def from_union(fs, x):
+    for f in fs:
+        try:
+            return f(x)
+        except:
+            pass
+    assert False
+
+
 def to_class(c: Type[T], x: Any) -> dict:
     assert isinstance(x, c)
     return cast(Any, x).to_dict()
 
 
 class ExtractColors:
     default_files: List[str]
@@ -159,51 +178,56 @@
         result: dict = {}
         result["repository"] = from_str(self.repository)
         return result
 
 
 class Configuration:
     build_metadata_file: str
+    exporters: Optional[Dict[str, Dict[str, Any]]]
     extract_colors: ExtractColors
     make_gifs: MakeGifs
     make_thumbnails: MakeThumbnails
     media: Media
     projects_at: str
     scattered_mode_folder: str
     tags: Tags
     technologies: Technologies
 
-    def __init__(self, build_metadata_file: str, extract_colors: ExtractColors, make_gifs: MakeGifs, make_thumbnails: MakeThumbnails, media: Media, projects_at: str, scattered_mode_folder: str, tags: Tags, technologies: Technologies) -> None:
+    def __init__(self, build_metadata_file: str, exporters: Optional[Dict[str, Dict[str, Any]]], extract_colors: ExtractColors, make_gifs: MakeGifs, make_thumbnails: MakeThumbnails, media: Media, projects_at: str, scattered_mode_folder: str, tags: Tags, technologies: Technologies) -> None:
         self.build_metadata_file = build_metadata_file
+        self.exporters = exporters
         self.extract_colors = extract_colors
         self.make_gifs = make_gifs
         self.make_thumbnails = make_thumbnails
         self.media = media
         self.projects_at = projects_at
         self.scattered_mode_folder = scattered_mode_folder
         self.tags = tags
         self.technologies = technologies
 
     @staticmethod
     def from_dict(obj: Any) -> 'Configuration':
         assert isinstance(obj, dict)
         build_metadata_file = from_str(obj.get("build metadata file"))
+        exporters = from_union([lambda x: from_dict(lambda x: from_dict(lambda x: x, x), x), from_none], obj.get("exporters"))
         extract_colors = ExtractColors.from_dict(obj.get("extract colors"))
         make_gifs = MakeGifs.from_dict(obj.get("make gifs"))
         make_thumbnails = MakeThumbnails.from_dict(obj.get("make thumbnails"))
         media = Media.from_dict(obj.get("media"))
         projects_at = from_str(obj.get("projects at"))
         scattered_mode_folder = from_str(obj.get("scattered mode folder"))
         tags = Tags.from_dict(obj.get("tags"))
         technologies = Technologies.from_dict(obj.get("technologies"))
-        return Configuration(build_metadata_file, extract_colors, make_gifs, make_thumbnails, media, projects_at, scattered_mode_folder, tags, technologies)
+        return Configuration(build_metadata_file, exporters, extract_colors, make_gifs, make_thumbnails, media, projects_at, scattered_mode_folder, tags, technologies)
 
     def to_dict(self) -> dict:
         result: dict = {}
         result["build metadata file"] = from_str(self.build_metadata_file)
+        if self.exporters is not None:
+            result["exporters"] = from_union([lambda x: from_dict(lambda x: from_dict(lambda x: x, x), x), from_none], self.exporters)
         result["extract colors"] = to_class(ExtractColors, self.extract_colors)
         result["make gifs"] = to_class(MakeGifs, self.make_gifs)
         result["make thumbnails"] = to_class(MakeThumbnails, self.make_thumbnails)
         result["media"] = to_class(Media, self.media)
         result["projects at"] = from_str(self.projects_at)
         result["scattered mode folder"] = from_str(self.scattered_mode_folder)
         result["tags"] = to_class(Tags, self.tags)
```

### Comparing `ortfodb-1.0.0/ortfodb/database.py` & `ortfodb-1.1.0/ortfodb/database.py`

 * *Files identical despite different names*

### Comparing `ortfodb-1.0.0/ortfodb/tags.py` & `ortfodb-1.1.0/ortfodb/tags.py`

 * *Files identical despite different names*

### Comparing `ortfodb-1.0.0/ortfodb/technologies.py` & `ortfodb-1.1.0/ortfodb/technologies.py`

 * *Files identical despite different names*

### Comparing `ortfodb-1.0.0/PKG-INFO` & `ortfodb-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ortfodb
-Version: 1.0.0
+Version: 1.1.0
 Summary: ortfodb client library
 License: MIT
 Author: Ewen Le Bihan
 Author-email: hey@ewen.works
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

