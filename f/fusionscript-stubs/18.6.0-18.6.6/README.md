# Comparing `tmp/fusionscript-stubs-18.6.0.tar.gz` & `tmp/fusionscript_stubs-18.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusionscript-stubs-18.6.0.tar", last modified: Fri Nov  3 13:50:54 2023, max compression
+gzip compressed data, was "fusionscript_stubs-18.6.6.tar", last modified: Sun Apr 14 12:48:09 2024, max compression
```

## Comparing `fusionscript-stubs-18.6.0.tar` & `fusionscript_stubs-18.6.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-11-03 13:50:54.685511 fusionscript-stubs-18.6.0/
--rw-rw-rw-   0        0        0     1079 2023-06-18 12:26:33.000000 fusionscript-stubs-18.6.0/LICENSE.md
--rw-rw-rw-   0        0        0     1628 2023-11-03 13:50:54.683515 fusionscript-stubs-18.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     1330 2023-11-03 13:32:10.000000 fusionscript-stubs-18.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-11-03 13:50:54.673523 fusionscript-stubs-18.6.0/fusionscript-stubs/
--rw-rw-rw-   0        0        0     5259 2023-06-23 08:48:38.000000 fusionscript-stubs-18.6.0/fusionscript-stubs/__init__.pyi
--rw-rw-rw-   0        0        0    86227 2023-11-03 13:31:06.000000 fusionscript-stubs-18.6.0/fusionscript-stubs/fusionscript.pyi
-drwxrwxrwx   0        0        0        0 2023-11-03 13:50:54.681520 fusionscript-stubs-18.6.0/fusionscript_stubs.egg-info/
--rw-rw-rw-   0        0        0     1628 2023-11-03 13:50:54.000000 fusionscript-stubs-18.6.0/fusionscript_stubs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-11-03 13:50:54.000000 fusionscript-stubs-18.6.0/fusionscript_stubs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-03 13:50:54.000000 fusionscript-stubs-18.6.0/fusionscript_stubs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-11-03 13:50:54.000000 fusionscript-stubs-18.6.0/fusionscript_stubs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-03 13:50:54.686505 fusionscript-stubs-18.6.0/setup.cfg
--rw-rw-rw-   0        0        0      557 2023-11-03 13:31:42.000000 fusionscript-stubs-18.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 12:48:09.185391 fusionscript_stubs-18.6.6/
+-rw-rw-rw-   0        0        0     1079 2023-06-18 12:26:34.000000 fusionscript_stubs-18.6.6/LICENSE.md
+-rw-rw-rw-   0        0        0     1634 2024-04-14 12:48:09.183992 fusionscript_stubs-18.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1336 2024-04-14 10:09:40.000000 fusionscript_stubs-18.6.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 12:48:09.180166 fusionscript_stubs-18.6.6/fusionscript-stubs/
+-rw-rw-rw-   0        0        0     5361 2024-04-14 08:57:27.000000 fusionscript_stubs-18.6.6/fusionscript-stubs/__init__.pyi
+-rw-rw-rw-   0        0        0    94837 2024-04-14 10:05:31.000000 fusionscript_stubs-18.6.6/fusionscript-stubs/fusionscript.pyi
+drwxrwxrwx   0        0        0        0 2024-04-14 12:48:09.183992 fusionscript_stubs-18.6.6/fusionscript_stubs.egg-info/
+-rw-rw-rw-   0        0        0     1634 2024-04-14 12:48:09.000000 fusionscript_stubs-18.6.6/fusionscript_stubs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-04-14 12:48:09.000000 fusionscript_stubs-18.6.6/fusionscript_stubs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 12:48:09.000000 fusionscript_stubs-18.6.6/fusionscript_stubs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-14 12:48:09.000000 fusionscript_stubs-18.6.6/fusionscript_stubs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 12:48:09.185897 fusionscript_stubs-18.6.6/setup.cfg
+-rw-rw-rw-   0        0        0      553 2024-04-14 10:08:35.000000 fusionscript_stubs-18.6.6/setup.py
```

### Comparing `fusionscript-stubs-18.6.0/LICENSE.md` & `fusionscript_stubs-18.6.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fusionscript-stubs-18.6.0/PKG-INFO` & `fusionscript_stubs-18.6.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusionscript-stubs
-Version: 18.6.0
+Version: 18.6.6
 Summary: DaVinci Resolve Python API stubs
 Home-page: https://github.com/czukowski/fusionscript-stubs
 Author: Korney Czukowski
 Author-email: carbofos@seznam.cz
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
@@ -47,13 +47,13 @@
 Happy scripting!
 
 Patches are welcome to fix any errors in the stubs!
 
 About versioning
 ----------------
 
-The stubs package major and minor version numbers (eg. 18.6) indicate compatibility 
-with the corresponding DaVinci Resolve version and is based on the documentaton 
+The stubs package major and minor version numbers (e.g. 18.6) indicate compatibility 
+with the corresponding DaVinci Resolve version and is based on the documentation 
 (scripting README.txt) shipped with that version. The patch version number is incremental
 and does not correspond to DaVinci Resolve releases.
 
-The current stubs are based on the documentation marked as "Updated as of 18 July 2023". 
+The current stubs are based on the documentation marked as "Updated as of 18 December 2023".
```

### Comparing `fusionscript-stubs-18.6.0/README.md` & `fusionscript_stubs-18.6.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,13 +37,13 @@
 Happy scripting!
 
 Patches are welcome to fix any errors in the stubs!
 
 About versioning
 ----------------
 
-The stubs package major and minor version numbers (eg. 18.6) indicate compatibility 
-with the corresponding DaVinci Resolve version and is based on the documentaton 
+The stubs package major and minor version numbers (e.g. 18.6) indicate compatibility 
+with the corresponding DaVinci Resolve version and is based on the documentation 
 (scripting README.txt) shipped with that version. The patch version number is incremental
 and does not correspond to DaVinci Resolve releases.
 
-The current stubs are based on the documentation marked as "Updated as of 18 July 2023". 
+The current stubs are based on the documentation marked as "Updated as of 18 December 2023".
```

### Comparing `fusionscript-stubs-18.6.0/fusionscript-stubs/__init__.pyi` & `fusionscript_stubs-18.6.6/fusionscript-stubs/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,17 @@
     UniqueFilenameStyle as UniqueFilenameStyle,
     VersionType as VersionType,
 )
 
 
 # Typed dicts
 from .fusionscript import (
+    AutoCaptionSettings as AutoCaptionSettings,
     CDLMap as CDLMap,
+    CloudProjectsSettings as CloudProjectsSettings,
     DbInfo as DbInfo,
     FloatingWindowParams as FloatingWindowParams,
     ImportClipInfo as ImportClipInfo,
     Marker as Marker,
     MediaPoolClipInfo as MediaPoolClipInfo,
     Preset as Preset,
     RenderPreset as RenderPreset,
```

### Comparing `fusionscript-stubs-18.6.0/fusionscript-stubs/fusionscript.pyi` & `fusionscript_stubs-18.6.6/fusionscript-stubs/fusionscript.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,18 @@
-from typing import Any, Final, List, NotRequired, Optional, TypedDict
+from typing import Annotated, Any, Final, List, NotRequired, Optional, TypedDict
 from typing import overload
 from typing_extensions import Literal
+from dataclasses import dataclass
 from deprecated import deprecated
 
+@dataclass
+class ValueRange:
+    min: int
+    max: int
+
 
 ColorSet1 = Literal['Orange', 'Apricot', 'Yellow', 'Lime', 'Olive', 'Green', 'Teal', 'Navy', 'Blue', 'Purple', 'Violet', 'Pink', 'Tan', 'Beige', 'Brown', 'Chocolate']
 ColorSet2 = Literal['Blue', 'Cyan', 'Green', 'Yellow', 'Red', 'Pink', 'Purple', 'Fuchsia', 'Rose', 'Lavender', 'Sky', 'Mint', 'Lemon', 'Sand', 'Cocoa', 'Cream']
 
 ClipColor = ColorSet1
 FlagColor = ColorSet2
 MarkerColor = ColorSet2
@@ -65,14 +71,45 @@
 
 UniqueFilenameStyle = Literal[0, 1]
 """ 0 - Prefix, 1 - Suffix """
 
 VersionType = Literal[0, 1]
 """ 0 - Local, 1 - Remote """
 
+AutoCaptionSettings = TypedDict('AutoCaptionSettings', {
+    Resolve.SUBTITLE_LANGUAGE: Literal[Resolve.AUTO_CAPTION_AUTO, \
+                                       Resolve.AUTO_CAPTION_DANISH, \
+                                       Resolve.AUTO_CAPTION_DUTCH, \
+                                       Resolve.AUTO_CAPTION_ENGLISH, \
+                                       Resolve.AUTO_CAPTION_FRENCH, \
+                                       Resolve.AUTO_CAPTION_GERMAN, \
+                                       Resolve.AUTO_CAPTION_ITALIAN, \
+                                       Resolve.AUTO_CAPTION_JAPANESE, \
+                                       Resolve.AUTO_CAPTION_KOREAN, \
+                                       Resolve.AUTO_CAPTION_MANDARIN_SIMPLIFIED, \
+                                       Resolve.AUTO_CAPTION_MANDARIN_TRADITIONAL, \
+                                       Resolve.AUTO_CAPTION_NORWEGIAN, \
+                                       Resolve.AUTO_CAPTION_PORTUGUESE, \
+                                       Resolve.AUTO_CAPTION_RUSSIAN, \
+                                       Resolve.AUTO_CAPTION_SPANISH, \
+                                       Resolve.AUTO_CAPTION_SWEDISH],
+    Resolve.SUBTITLE_CAPTION_PRESET: Resolve.AUTO_CAPTION_SUBTITLE_DEFAULT | Resolve.AUTO_CAPTION_TELETEXT | Resolve.AUTO_CAPTION_NETFLIX,
+    Resolve.SUBTITLE_CHARS_PER_LINE: Annotated[int, ValueRange(1, 60)],
+    Resolve.SUBTITLE_LINE_BREAK: Literal[Resolve.AUTO_CAPTION_LINE_SINGLE, Resolve.AUTO_CAPTION_LINE_DOUBLE],
+    Resolve.SUBTITLE_GAP: Annotated[int, ValueRange(0, 10)],
+})
+
+CloudProjectsSettings = TypedDict('CloudProjectsSettings', {
+    Resolve.CLOUD_SETTING_PROJECT_NAME: str,
+    Resolve.CLOUD_SETTING_PROJECT_MEDIA_PATH: str,
+    Resolve.CLOUD_SETTING_IS_COLLAB: bool,
+    Resolve.CLOUD_SETTING_SYNC_MODE: Literal[Resolve.CLOUD_SYNC_NONE, Resolve.CLOUD_SYNC_PROXY_ONLY, Resolve.CLOUD_SYNC_PROXY_AND_ORIG],
+    Resolve.CLOUD_SETTING_IS_CAMERA_ACCESS: bool,
+})
+
 
 class CDLMap(TypedDict):
     """ Keys of map are: "NodeIndex", "Slope", "Offset", "Power", "Saturation", where 1 <= NodeIndex <= total number of nodes. """
     NodeIndex: int
     Slope: str
     Offset: str
     Power: str
@@ -349,14 +386,32 @@
     """
     List and Dict Data Structures
     -----------------------------
     Beside primitive data types, Resolve's Python API mainly uses list and dict data structures. Lists are denoted by [ ... ] and dicts are denoted by { ... } above.
     As Lua does not support list and dict data structures, the Lua API implements "list" as a table with indices, e.g. { [1] = listValue1, [2] = listValue2, ... }.
     Similarly the Lua API implements "dict" as a table with the dictionary key as first element, e.g. { [dictKey1] = dictValue1, [dictKey2] = dictValue2, ... }.
 
+    Cloud Projects Settings
+    --------------------------------------
+    This section covers additional notes for the functions "ProjectManager:CreateCloudProject," "ProjectManager:ImportCloudProject," and "ProjectManager:RestoreCloudProject"
+
+    All three functions take in a {cloudSettings} dict, that have the following keys:
+    * resolve.CLOUD_SETTING_PROJECT_NAME: String, ["" by default]
+    * resolve.CLOUD_SETTING_PROJECT_MEDIA_PATH: String, ["" by default]
+    * resolve.CLOUD_SETTING_IS_COLLAB: Bool, [False by default]
+    * resolve.CLOUD_SETTING_SYNC_MODE: syncMode (see below), [resolve.CLOUD_SYNC_PROXY_ONLY by default]
+    * resolve.CLOUD_SETTING_IS_CAMERA_ACCESS: Bool [False by default]
+
+    Where syncMode is one of the following values:
+    * resolve.CLOUD_SYNC_NONE,
+    * resolve.CLOUD_SYNC_PROXY_ONLY,
+    * resolve.CLOUD_SYNC_PROXY_AND_ORIG
+
+    All three "ProjectManager:CreateCloudProject," "ProjectManager:ImportCloudProject," and "ProjectManager:RestoreCloudProject" require resolve.PROJECT_MEDIA_PATH to be defined. "ProjectManager:CreateCloudProject" also requires resolve.PROJECT_NAME to be defined.
+
     Looking up Project and Clip properties
     --------------------------------------
     This section covers additional notes for the functions "Project:GetSetting", "Project:SetSetting", "Timeline:GetSetting", "Timeline:SetSetting", "MediaPoolItem:GetClipProperty" and
     "MediaPoolItem:SetClipProperty". These functions are used to get and set properties otherwise available to the user through the Project Settings and the Clip Attributes dialogs.
 
     The functions follow a key-value pair format, where each property is identified by a key (the settingName or propertyName parameter) and possesses a value (typically a text value). Keys and values are
     designed to be easily correlated with parameter names and values in the Resolve UI. Explicitly enumerated values for some parameters are listed below.
@@ -388,14 +443,58 @@
     The following Clip properties have specifically enumerated values:
     "Super Scale" - the property value is an enumerated integer between 1 and 4 with these meanings: 1=no scaling, and 2, 3 and 4 represent the Super Scale multipliers 2x, 3x and 4x.
                     for super scale multiplier '2x Enhanced', exactly 4 arguments must be passed as outlined below. If less than 4 arguments are passed, it will default to 2x.
     Affects:
     • x = MediaPoolItem:GetClipProperty('Super Scale') and MediaPoolItem:SetClipProperty('Super Scale', x)
     • for '2x Enhanced' --> MediaPoolItem:SetClipProperty('Super Scale', 2, sharpnessValue, noiseReductionValue), where sharpnessValue is a float in the range [0.0, 1.0] and noiseReductionValue is a float in the range [0.0, 1.0]
 
+    Auto Caption Settings
+    ----------------------
+    This section covers the supported settings for the method Timeline.CreateSubtitlesFromAudio({autoCaptionSettings})
+
+    The parameter setting is a dictionary containing the following keys:
+    * resolve.SUBTITLE_LANGUAGE: languageID (see below), [resolve.AUTO_CAPTION_AUTO by default]
+    * resolve.SUBTITLE_CAPTION_PRESET: presetType (see below), [resolve.AUTO_CAPTION_SUBTITLE_DEFAULT by default]
+    * resolve.SUBTITLE_CHARS_PER_LINE: Number between 1 and 60 inclusive [42 by default]
+    * resolve.SUBTITLE_LINE_BREAK: lineBreakType (see below), [resolve.AUTO_CAPTION_LINE_SINGLE by default]
+    * resolve.SUBTITLE_GAP: Number between 0 and 10 inclusive [0 by default]
+
+    Note that the default values for some keys may change based on values defined for other keys, as per the UI.
+    For example, if the following dictionary is supplied,
+        CreateSubtitlesFromAudio( { resolve.SUBTITLE_LANGUAGE = resolve.AUTO_CAPTION_KOREAN,
+                                    resolve.SUBTITLE_CAPTION_PRESET = resolve.AUTO_CAPTION_NETFLIX } )
+    the default value for resolve.SUBTITLE_CHARS_PER_LINE will be 16 instead of 42
+
+    languageIDs:
+    * resolve.AUTO_CAPTION_AUTO
+    * resolve.AUTO_CAPTION_DANISH
+    * resolve.AUTO_CAPTION_DUTCH
+    * resolve.AUTO_CAPTION_ENGLISH
+    * resolve.AUTO_CAPTION_FRENCH
+    * resolve.AUTO_CAPTION_GERMAN
+    * resolve.AUTO_CAPTION_ITALIAN
+    * resolve.AUTO_CAPTION_JAPANESE
+    * resolve.AUTO_CAPTION_KOREAN
+    * resolve.AUTO_CAPTION_MANDARIN_SIMPLIFIED
+    * resolve.AUTO_CAPTION_MANDARIN_TRADITIONAL
+    * resolve.AUTO_CAPTION_NORWEGIAN
+    * resolve.AUTO_CAPTION_PORTUGUESE
+    * resolve.AUTO_CAPTION_RUSSIAN
+    * resolve.AUTO_CAPTION_SPANISH
+    * resolve.AUTO_CAPTION_SWEDISH
+
+    presetTypes:
+    * resolve.AUTO_CAPTION_SUBTITLE_DEFAULT
+    * resolve.AUTO_CAPTION_TELETEXT
+    * resolve.AUTO_CAPTION_NETFLIX
+
+    lineBreakTypes:
+    * resolve.AUTO_CAPTION_LINE_SINGLE
+    * resolve.AUTO_CAPTION_LINE_DOUBLE
+
 
     Looking up Render Settings
     --------------------------
     This section covers the supported settings for the method SetRenderSettings({settings})
 
     The parameter setting is a dictionary containing the following keys:
         - "SelectAllFrames": Bool (when set True, the settings MarkIn and MarkOut are ignored)
@@ -570,14 +669,48 @@
 
     The arguments can be passed as a key and value pair or they can be grouped together into a dictionary (for python) or table (for lua) and passed
     as a single argument.
 
     Getting the values for the keys that uses constants will return the number which is in the constant
     """
 
+    AUTO_CAPTION_AUTO: Final
+    AUTO_CAPTION_DANISH: Final
+    AUTO_CAPTION_DUTCH: Final
+    AUTO_CAPTION_ENGLISH: Final
+    AUTO_CAPTION_FRENCH: Final
+    AUTO_CAPTION_GERMAN: Final
+    AUTO_CAPTION_ITALIAN: Final
+    AUTO_CAPTION_JAPANESE: Final
+    AUTO_CAPTION_KOREAN: Final
+    AUTO_CAPTION_MANDARIN_SIMPLIFIED: Final
+    AUTO_CAPTION_MANDARIN_TRADITIONAL: Final
+    AUTO_CAPTION_NORWEGIAN: Final
+    AUTO_CAPTION_PORTUGUESE: Final
+    AUTO_CAPTION_RUSSIAN: Final
+    AUTO_CAPTION_SPANISH: Final
+    AUTO_CAPTION_SWEDISH: Final
+
+    AUTO_CAPTION_SUBTITLE_DEFAULT: Final
+    AUTO_CAPTION_TELETEXT: Final
+    AUTO_CAPTION_NETFLIX: Final
+
+    AUTO_CAPTION_LINE_SINGLE: Final
+    AUTO_CAPTION_LINE_DOUBLE: Final
+
+    CLOUD_SETTING_PROJECT_NAME: Final
+    CLOUD_SETTING_PROJECT_MEDIA_PATH: Final
+    CLOUD_SETTING_IS_COLLAB: Final
+    CLOUD_SETTING_SYNC_MODE: Final
+    CLOUD_SETTING_IS_CAMERA_ACCESS: Final
+
+    CLOUD_SYNC_NONE: Final
+    CLOUD_SYNC_PROXY_ONLY: Final
+    CLOUD_SYNC_PROXY_AND_ORIG: Final
+
     EXPORT_AAF: Final
     EXPORT_DRT: Final
     EXPORT_EDL: Final
     EXPORT_FCP_7_XML: Final
     EXPORT_FCPXML_1_8: Final
     EXPORT_FCPXML_1_9: Final
     EXPORT_FCPXML_1_10: Final
@@ -593,14 +726,20 @@
     EXPORT_NONE: Final
     EXPORT_AAF_NEW: Final
     EXPORT_AAF_EXISTING: Final
     EXPORT_CDL: Final
     EXPORT_SDL: Final
     EXPORT_MISSING_CLIPS: Final
 
+    SUBTITLE_LANGUAGE: Final
+    SUBTITLE_CAPTION_PRESET: Final
+    SUBTITLE_CHARS_PER_LINE: Final
+    SUBTITLE_LINE_BREAK: Final
+    SUBTITLE_GAP: Final
+
     def Fusion(self) -> Fusion:
         """ Returns the Fusion object. Starting point for Fusion scripts. """
         ...
 
     def GetMediaStorage(self) -> MediaStorage:
         """ Returns the media storage object to query and act on media locations. """
         ...
@@ -783,14 +922,37 @@
         """ Returns a list of dictionary items (with keys 'DbType', 'DbName' and optional 'IpAddress') corresponding to all the databases added to Resolve """
         ...
 
     def SetCurrentDatabase(self, dbInfo: DbInfo) -> bool:
         """ Switches current database connection to the database specified by the keys below, and closes any open project. """
         ...
 
+    def CreateCloudProject(self, cloudSettings: CloudProjectsSettings) -> Project:
+        """
+        Creates and returns a cloud project.
+        '{cloudSettings}': Check 'Cloud Projects Settings' subsection below for more information.
+        """
+        ...
+
+    def ImportCloudProject(self, filePath: str, cloudSettings: CloudProjectsSettings) -> bool:
+        """
+        Returns True if import cloud project is successful; False otherwise
+        'filePath': String; filePath of file to import
+        '{cloudSettings}': Check 'Cloud Projects Settings' subsection below for more information.
+        """
+        ...
+
+    def RestoreCloudProject(self, folderPath: str, cloudSettings: CloudProjectsSettings) -> bool:
+        """
+        Returns True if restore cloud project is successful; False otherwise
+        'folderPath': String; path of folder to restore
+        '{cloudSettings}': Check 'Cloud Projects Settings' subsection below for more information.
+        """
+        ...
+
 
 class Project:
 
     def GetMediaPool(self) -> MediaPool:
         """ Returns the Media Pool object. """
         ...
 
@@ -1200,15 +1362,15 @@
     @overload
     def CreateTimelineFromClips(self, name: str, clipInfo: List[MediaPoolClipInfo]) -> Timeline:
         """ Creates new timeline with specified name, appending the list of clipInfos specified as a dict of "mediaPoolItem", "startFrame" (int), "endFrame" (int), "recordFrame" (int). """
         ...
 
     def ImportTimelineFromFile(self, filePath: str, importOptions: TimelineImportOptions) -> Timeline:
         """
-        Creates timeline based on parameters within given file (AAF/EDL/XML/FCPXML/DRT/ADL) and optional importOptions dict, with support for the keys:
+        Creates timeline based on parameters within given file (AAF/EDL/XML/FCPXML/DRT/ADL/OTIO) and optional importOptions dict, with support for the keys:
         "timelineName": string, specifies the name of the timeline to be created. Not valid for DRT import
         "importSourceClips": Bool, specifies whether source clips should be imported, True by default. Not valid for DRT import
         "sourceClipsPath": string, specifies a filesystem path to search for source clips if the media is inaccessible in their original path and if "importSourceClips" is True
         "sourceClipsFolders": List of Media Pool folder objects to search for source clips if the media is not present in current folder and if "importSourceClips" is False. Not valid for DRT import
         "interlaceProcessing": Bool, specifies whether to enable interlace processing on the imported timeline being created. valid only for AAF import
         """
         ...
@@ -1292,14 +1454,18 @@
         """
         ...
     
     def GetUniqueId(self) -> str:
         """ Returns a unique ID for the media pool """
         ...
 
+    def CreateStereoClip(str, LeftMediaPoolItem: MediaPoolItem, RightMediaPoolItem: MediaPoolItem) -> MediaPoolItem:
+        """ Takes in two existing media pool items and creates a new 3D stereoscopic media pool entry replacing the input media in the media pool. """
+        ...
+
 
 class Folder:
 
     def GetClipList(self) -> List[MediaPoolItem]:
         """ Returns a list of clips (items) within the folder. """
         ...
 
@@ -1335,14 +1501,22 @@
         """ Returns a unique ID for the media pool folder """
         ...
 
     def Export(self, filePath: str) -> bool:
         """ Returns true if export of DRB folder to filePath is successful, false otherwise """
         ...
 
+    def TranscribeAudio(self) -> bool:
+        """ Transcribes audio of the MediaPoolItems within the folder and nested folders. Returns True if successful; False otherwise """
+        ...
+
+    def ClearTranscription(self) -> bool:
+        """ Clears audio transcription of the MediaPoolItems within the folder and nested folders. Returns True if successful; False otherwise. """
+        ...
+
 
 class MediaPoolItem:
 
     def GetName(self) -> str:
         """ Returns the clip name. """
         ...
 
@@ -1722,22 +1896,30 @@
         """
         ...
 
     def GetUniqueId(self) -> str:
         """ Returns a unique ID for the timeline """
         ...
 
-    def CreateSubtitlesFromAudio(self) -> bool:
-        """ Creates subtitles from audio for the timeline. Returns True on success, False otherwise. """
+    def CreateSubtitlesFromAudio(self, autoCaptionSettings: Optional[AutoCaptionSettings]) -> bool:
+        """
+        Creates subtitles from audio for the timeline.
+        Takes in optional dictionary {autoCaptionSettings}. Check 'Auto Caption Settings' subsection below for more information.
+        Returns True on success, False otherwise.
+        """
         ...
 
     def DetectSceneCuts(self) -> bool:
         """ Detects and makes scene cuts along the timeline. Returns True if successful, False otherwise. """
         ...
 
+    def ConvertTimelineToStereo(self) -> bool:
+        """ Converts timeline to stereo. Returns True if successful; False otherwise. """
+        ...
+
 
 class TimelineItem:
 
     def GetName(self) -> str:
         """ Returns the item name. """
         ...
```

### Comparing `fusionscript-stubs-18.6.0/fusionscript_stubs.egg-info/PKG-INFO` & `fusionscript_stubs-18.6.6/fusionscript_stubs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusionscript-stubs
-Version: 18.6.0
+Version: 18.6.6
 Summary: DaVinci Resolve Python API stubs
 Home-page: https://github.com/czukowski/fusionscript-stubs
 Author: Korney Czukowski
 Author-email: carbofos@seznam.cz
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
@@ -47,13 +47,13 @@
 Happy scripting!
 
 Patches are welcome to fix any errors in the stubs!
 
 About versioning
 ----------------
 
-The stubs package major and minor version numbers (eg. 18.6) indicate compatibility 
-with the corresponding DaVinci Resolve version and is based on the documentaton 
+The stubs package major and minor version numbers (e.g. 18.6) indicate compatibility 
+with the corresponding DaVinci Resolve version and is based on the documentation 
 (scripting README.txt) shipped with that version. The patch version number is incremental
 and does not correspond to DaVinci Resolve releases.
 
-The current stubs are based on the documentation marked as "Updated as of 18 July 2023". 
+The current stubs are based on the documentation marked as "Updated as of 18 December 2023".
```

### Comparing `fusionscript-stubs-18.6.0/setup.py` & `fusionscript_stubs-18.6.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from distutils.core import setup
+from setuptools import setup
 from pathlib import Path
 
 
 setup(
     name="fusionscript-stubs",
     url="https://github.com/czukowski/fusionscript-stubs",
     description="DaVinci Resolve Python API stubs",
     long_description=(Path(__file__).parent / "README.md").read_text(),
     long_description_content_type='text/markdown',
     author="Korney Czukowski",
     author_email="carbofos@seznam.cz",
-    version="18.6.0",
+    version="18.6.6",
     package_data={"fusionscript-stubs": ['fusionscript.pyi', '__init__.pyi']},
     packages=["fusionscript-stubs"]
 )
```

