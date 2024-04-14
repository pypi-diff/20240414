# Comparing `tmp/ortfodb-0.3.2.tar.gz` & `tmp/ortfodb-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ortfodb-0.3.2.tar", max compression
+gzip compressed data, was "ortfodb-1.0.0.tar", max compression
```

## Comparing `ortfodb-0.3.2.tar` & `ortfodb-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      209 2024-04-12 21:43:37.285597 ortfodb-0.3.2/README.md
--rw-r--r--   0        0        0      434 2024-04-12 21:42:27.066289 ortfodb-0.3.2/ortfodb/__init__.py
--rw-r--r--   0        0        0     6923 2024-04-12 22:45:43.206325 ortfodb-0.3.2/ortfodb/configuration.py
--rw-r--r--   0        0        0    14616 2024-04-12 22:45:44.073024 ortfodb-0.3.2/ortfodb/database.py
--rw-r--r--   0        0        0     2791 2024-04-12 22:45:44.903055 ortfodb-0.3.2/ortfodb/tags.py
--rw-r--r--   0        0        0     2311 2024-04-12 22:45:45.693084 ortfodb-0.3.2/ortfodb/technologies.py
--rw-r--r--   0        0        0      301 2024-04-12 22:45:46.336441 ortfodb-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 ortfodb-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      209 2024-04-12 21:43:37.285597 ortfodb-1.0.0/README.md
+-rw-r--r--   0        0        0      434 2024-04-12 21:42:27.066289 ortfodb-1.0.0/ortfodb/__init__.py
+-rw-r--r--   0        0        0     7128 2024-04-13 16:57:38.069979 ortfodb-1.0.0/ortfodb/configuration.py
+-rw-r--r--   0        0        0    14616 2024-04-13 16:57:38.953345 ortfodb-1.0.0/ortfodb/database.py
+-rw-r--r--   0        0        0     2791 2024-04-13 16:57:39.766708 ortfodb-1.0.0/ortfodb/tags.py
+-rw-r--r--   0        0        0     2311 2024-04-13 16:57:40.596738 ortfodb-1.0.0/ortfodb/technologies.py
+-rw-r--r--   0        0        0      301 2024-04-13 16:57:41.243429 ortfodb-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 ortfodb-1.0.0/PKG-INFO
```

### Comparing `ortfodb-0.3.2/ortfodb/configuration.py` & `ortfodb-1.0.0/ortfodb/configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -163,48 +163,52 @@
 
 class Configuration:
     build_metadata_file: str
     extract_colors: ExtractColors
     make_gifs: MakeGifs
     make_thumbnails: MakeThumbnails
     media: Media
+    projects_at: str
     scattered_mode_folder: str
     tags: Tags
     technologies: Technologies
 
-    def __init__(self, build_metadata_file: str, extract_colors: ExtractColors, make_gifs: MakeGifs, make_thumbnails: MakeThumbnails, media: Media, scattered_mode_folder: str, tags: Tags, technologies: Technologies) -> None:
+    def __init__(self, build_metadata_file: str, extract_colors: ExtractColors, make_gifs: MakeGifs, make_thumbnails: MakeThumbnails, media: Media, projects_at: str, scattered_mode_folder: str, tags: Tags, technologies: Technologies) -> None:
         self.build_metadata_file = build_metadata_file
         self.extract_colors = extract_colors
         self.make_gifs = make_gifs
         self.make_thumbnails = make_thumbnails
         self.media = media
+        self.projects_at = projects_at
         self.scattered_mode_folder = scattered_mode_folder
         self.tags = tags
         self.technologies = technologies
 
     @staticmethod
     def from_dict(obj: Any) -> 'Configuration':
         assert isinstance(obj, dict)
         build_metadata_file = from_str(obj.get("build metadata file"))
         extract_colors = ExtractColors.from_dict(obj.get("extract colors"))
         make_gifs = MakeGifs.from_dict(obj.get("make gifs"))
         make_thumbnails = MakeThumbnails.from_dict(obj.get("make thumbnails"))
         media = Media.from_dict(obj.get("media"))
+        projects_at = from_str(obj.get("projects at"))
         scattered_mode_folder = from_str(obj.get("scattered mode folder"))
         tags = Tags.from_dict(obj.get("tags"))
         technologies = Technologies.from_dict(obj.get("technologies"))
-        return Configuration(build_metadata_file, extract_colors, make_gifs, make_thumbnails, media, scattered_mode_folder, tags, technologies)
+        return Configuration(build_metadata_file, extract_colors, make_gifs, make_thumbnails, media, projects_at, scattered_mode_folder, tags, technologies)
 
     def to_dict(self) -> dict:
         result: dict = {}
         result["build metadata file"] = from_str(self.build_metadata_file)
         result["extract colors"] = to_class(ExtractColors, self.extract_colors)
         result["make gifs"] = to_class(MakeGifs, self.make_gifs)
         result["make thumbnails"] = to_class(MakeThumbnails, self.make_thumbnails)
         result["media"] = to_class(Media, self.media)
+        result["projects at"] = from_str(self.projects_at)
         result["scattered mode folder"] = from_str(self.scattered_mode_folder)
         result["tags"] = to_class(Tags, self.tags)
         result["technologies"] = to_class(Technologies, self.technologies)
         return result
 
 
 def configuration_from_dict(s: Any) -> Configuration:
```

### Comparing `ortfodb-0.3.2/ortfodb/database.py` & `ortfodb-1.0.0/ortfodb/database.py`

 * *Files identical despite different names*

### Comparing `ortfodb-0.3.2/ortfodb/tags.py` & `ortfodb-1.0.0/ortfodb/tags.py`

 * *Files identical despite different names*

### Comparing `ortfodb-0.3.2/ortfodb/technologies.py` & `ortfodb-1.0.0/ortfodb/technologies.py`

 * *Files identical despite different names*

### Comparing `ortfodb-0.3.2/PKG-INFO` & `ortfodb-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ortfodb
-Version: 0.3.2
+Version: 1.0.0
 Summary: ortfodb client library
 License: MIT
 Author: Ewen Le Bihan
 Author-email: hey@ewen.works
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

