# Comparing `tmp/openmindat-0.0.3.tar.gz` & `tmp/openmindat-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmindat-0.0.3.tar", last modified: Fri Apr 12 00:57:44 2024, max compression
+gzip compressed data, was "openmindat-0.0.4.tar", last modified: Sun Apr 14 17:33:07 2024, max compression
```

## Comparing `openmindat-0.0.3.tar` & `openmindat-0.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 blc        (501) staff       (20)        0 2024-04-12 00:57:44.107414 openmindat-0.0.3/
--rw-r--r--   0 blc        (501) staff       (20)    11357 2023-09-28 23:58:40.000000 openmindat-0.0.3/LICENSE
--rw-r--r--   0 blc        (501) staff       (20)      136 2024-04-09 06:30:41.000000 openmindat-0.0.3/MANIFEST.in
--rw-r--r--   0 blc        (501) staff       (20)     4911 2024-04-12 00:57:44.107139 openmindat-0.0.3/PKG-INFO
--rw-r--r--   0 blc        (501) staff       (20)     4375 2024-04-12 00:56:04.000000 openmindat-0.0.3/README.md
-drwxr-xr-x   0 blc        (501) staff       (20)        0 2024-04-12 00:57:44.104996 openmindat-0.0.3/openmindat/
--rw-r--r--   0 blc        (501) staff       (20)     4506 2024-04-09 03:16:57.000000 openmindat-0.0.3/openmindat/__init__.py
--rw-r--r--   0 blc        (501) staff       (20)     8088 2024-04-12 00:35:16.000000 openmindat-0.0.3/openmindat/countries.py
--rw-r--r--   0 blc        (501) staff       (20)     5384 2024-04-09 03:16:57.000000 openmindat-0.0.3/openmindat/dana8.py
--rw-r--r--   0 blc        (501) staff       (20)    46983 2024-04-12 00:27:42.000000 openmindat-0.0.3/openmindat/geomaterials.py
--rw-r--r--   0 blc        (501) staff       (20)     3810 2024-04-09 03:16:57.000000 openmindat-0.0.3/openmindat/geomaterials_search.py
--rw-r--r--   0 blc        (501) staff       (20)    16008 2024-04-09 03:16:57.000000 openmindat-0.0.3/openmindat/localities.py
--rw-r--r--   0 blc        (501) staff       (20)     8328 2024-04-09 03:16:57.000000 openmindat-0.0.3/openmindat/localities_age.py
--rw-r--r--   0 blc        (501) staff       (20)     8369 2024-04-09 03:16:57.000000 openmindat-0.0.3/openmindat/localities_status.py
--rw-r--r--   0 blc        (501) staff       (20)     8330 2024-04-09 03:16:57.000000 openmindat-0.0.3/openmindat/localities_type.py
--rw-r--r--   0 blc        (501) staff       (20)     4465 2024-04-09 03:16:57.000000 openmindat-0.0.3/openmindat/locgeoregion2.py
--rw-r--r--   0 blc        (501) staff       (20)     3873 2024-04-09 03:16:57.000000 openmindat-0.0.3/openmindat/locobject.py
--rw-r--r--   0 blc        (501) staff       (20)    11800 2024-04-12 00:35:16.000000 openmindat-0.0.3/openmindat/mindat_api.py
--rw-r--r--   0 blc        (501) staff       (20)    13419 2024-04-12 00:36:48.000000 openmindat-0.0.3/openmindat/minerals_ima.py
--rw-r--r--   0 blc        (501) staff       (20)     5848 2024-04-09 03:16:57.000000 openmindat-0.0.3/openmindat/nickel_strunz.py
--rw-r--r--   0 blc        (501) staff       (20)     3126 2024-04-09 03:16:57.000000 openmindat-0.0.3/openmindat/photo_count.py
-drwxr-xr-x   0 blc        (501) staff       (20)        0 2024-04-12 00:57:44.106683 openmindat-0.0.3/openmindat.egg-info/
--rw-r--r--   0 blc        (501) staff       (20)     4911 2024-04-12 00:57:44.000000 openmindat-0.0.3/openmindat.egg-info/PKG-INFO
--rw-r--r--   0 blc        (501) staff       (20)      642 2024-04-12 00:57:44.000000 openmindat-0.0.3/openmindat.egg-info/SOURCES.txt
--rw-r--r--   0 blc        (501) staff       (20)        1 2024-04-12 00:57:44.000000 openmindat-0.0.3/openmindat.egg-info/dependency_links.txt
--rw-r--r--   0 blc        (501) staff       (20)        1 2024-03-09 23:51:57.000000 openmindat-0.0.3/openmindat.egg-info/not-zip-safe
--rw-r--r--   0 blc        (501) staff       (20)       16 2024-04-12 00:57:44.000000 openmindat-0.0.3/openmindat.egg-info/requires.txt
--rw-r--r--   0 blc        (501) staff       (20)       11 2024-04-12 00:57:44.000000 openmindat-0.0.3/openmindat.egg-info/top_level.txt
--rw-r--r--   0 blc        (501) staff       (20)       38 2024-04-12 00:57:44.107507 openmindat-0.0.3/setup.cfg
--rw-r--r--   0 blc        (501) staff       (20)     1058 2024-04-12 00:52:52.000000 openmindat-0.0.3/setup.py
+drwxr-xr-x   0 blc        (501) staff       (20)        0 2024-04-14 17:33:07.599038 openmindat-0.0.4/
+-rw-r--r--   0 blc        (501) staff       (20)    11357 2023-09-28 23:58:40.000000 openmindat-0.0.4/LICENSE
+-rw-r--r--   0 blc        (501) staff       (20)      136 2024-04-09 06:30:41.000000 openmindat-0.0.4/MANIFEST.in
+-rw-r--r--   0 blc        (501) staff       (20)     5833 2024-04-14 17:33:07.598785 openmindat-0.0.4/PKG-INFO
+-rw-r--r--   0 blc        (501) staff       (20)     5319 2024-04-14 17:31:34.000000 openmindat-0.0.4/README.md
+drwxr-xr-x   0 blc        (501) staff       (20)        0 2024-04-14 17:33:07.597243 openmindat-0.0.4/openmindat/
+-rw-r--r--   0 blc        (501) staff       (20)     6064 2024-04-14 17:11:41.000000 openmindat-0.0.4/openmindat/__init__.py
+-rw-r--r--   0 blc        (501) staff       (20)     8140 2024-04-14 17:11:41.000000 openmindat-0.0.4/openmindat/countries.py
+-rw-r--r--   0 blc        (501) staff       (20)     5358 2024-04-14 17:11:41.000000 openmindat-0.0.4/openmindat/dana8.py
+-rw-r--r--   0 blc        (501) staff       (20)    46900 2024-04-14 17:11:41.000000 openmindat-0.0.4/openmindat/geomaterials.py
+-rw-r--r--   0 blc        (501) staff       (20)     3785 2024-04-14 17:11:41.000000 openmindat-0.0.4/openmindat/geomaterials_search.py
+-rw-r--r--   0 blc        (501) staff       (20)    20215 2024-04-14 17:11:41.000000 openmindat-0.0.4/openmindat/localities.py
+-rw-r--r--   0 blc        (501) staff       (20)     8285 2024-04-14 17:11:41.000000 openmindat-0.0.4/openmindat/localities_age.py
+-rw-r--r--   0 blc        (501) staff       (20)     8335 2024-04-14 17:11:41.000000 openmindat-0.0.4/openmindat/localities_status.py
+-rw-r--r--   0 blc        (501) staff       (20)     8296 2024-04-14 17:11:41.000000 openmindat-0.0.4/openmindat/localities_type.py
+-rw-r--r--   0 blc        (501) staff       (20)     4447 2024-04-14 17:11:41.000000 openmindat-0.0.4/openmindat/locgeoregion2.py
+-rw-r--r--   0 blc        (501) staff       (20)     3848 2024-04-14 17:11:41.000000 openmindat-0.0.4/openmindat/locobject.py
+-rw-r--r--   0 blc        (501) staff       (20)    11800 2024-04-12 00:35:16.000000 openmindat-0.0.4/openmindat/mindat_api.py
+-rw-r--r--   0 blc        (501) staff       (20)    13369 2024-04-14 17:11:41.000000 openmindat-0.0.4/openmindat/minerals_ima.py
+-rw-r--r--   0 blc        (501) staff       (20)     5839 2024-04-14 17:11:41.000000 openmindat-0.0.4/openmindat/nickel_strunz.py
+-rw-r--r--   0 blc        (501) staff       (20)     3101 2024-04-14 17:11:41.000000 openmindat-0.0.4/openmindat/photo_count.py
+drwxr-xr-x   0 blc        (501) staff       (20)        0 2024-04-14 17:33:07.598486 openmindat-0.0.4/openmindat.egg-info/
+-rw-r--r--   0 blc        (501) staff       (20)     5833 2024-04-14 17:33:07.000000 openmindat-0.0.4/openmindat.egg-info/PKG-INFO
+-rw-r--r--   0 blc        (501) staff       (20)      642 2024-04-14 17:33:07.000000 openmindat-0.0.4/openmindat.egg-info/SOURCES.txt
+-rw-r--r--   0 blc        (501) staff       (20)        1 2024-04-14 17:33:07.000000 openmindat-0.0.4/openmindat.egg-info/dependency_links.txt
+-rw-r--r--   0 blc        (501) staff       (20)        1 2024-03-09 23:51:57.000000 openmindat-0.0.4/openmindat.egg-info/not-zip-safe
+-rw-r--r--   0 blc        (501) staff       (20)       16 2024-04-14 17:33:07.000000 openmindat-0.0.4/openmindat.egg-info/requires.txt
+-rw-r--r--   0 blc        (501) staff       (20)       11 2024-04-14 17:33:07.000000 openmindat-0.0.4/openmindat.egg-info/top_level.txt
+-rw-r--r--   0 blc        (501) staff       (20)       38 2024-04-14 17:33:07.599099 openmindat-0.0.4/setup.cfg
+-rw-r--r--   0 blc        (501) staff       (20)     1058 2024-04-14 17:12:58.000000 openmindat-0.0.4/setup.py
```

### Comparing `openmindat-0.0.3/LICENSE` & `openmindat-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openmindat-0.0.3/PKG-INFO` & `openmindat-0.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmindat
-Version: 0.0.3
+Version: 0.0.4
 Summary: An alpha version for OpenMindat package
 Home-page: https://github.com/ChuBL/OpenMindat
 Author: Jiyin Zhang
 Author-email: jiyinz@uidaho.edu
 License: Apache Software License
 Keywords: mindat openmindat mineral data python api
 Classifier: Development Status :: 3 - Alpha
@@ -20,16 +20,14 @@
 
 This is a test version of the OpenMindat Python package, designed to facilitate querying and retrieving data on minerals and geomaterials from the Mindat API. It provides classes for detailed queries based on various attributes like IMA status, keywords, and specific geomaterial properties.
 
 GitHub Repository: [OpenMindat Python Package](https://github.com/ChuBL/OpenMindat)
 
 ## Get Started
 
-> If you do not have a Mindat API key, please refer to [How to Get My Mindat API Key or Token?](https://www.mindat.org/a/how_to_get_my_mindat_api_key)
-
 ### Install via Pip
 
 ```console
 foo@bar:~$ pip install openmindat
 ```
 
 ### Import the Package in Python
@@ -44,19 +42,24 @@
 
 ```python
 import os
 
 os.environ["MINDAT_API_KEY"] = 'Your_Mindat_API_Key'
 ```
 
-You can also set the API key by following the instructions when using the following queries.
+> If you do not have a Mindat API key, please refer to [How to Get My Mindat API Key or Token?](https://www.mindat.org/a/how_to_get_my_mindat_api_key)
+
+You can also set the API key by following the general queries.
 
 ### 1. Perform Detailed Queries on Geomaterials
 
+:exclamation: Temporarily Outage, see https://github.com/ChuBL/OpenMindat/issues/12
+
 ```python
+# Temporarily Outage, see https://github.com/ChuBL/OpenMindat/issues/12
 from openmindat import GeomaterialRetriever
 
 gr = GeomaterialRetriever()
 gr.density_min(2.0).density_max(5.0).crystal_system("Hexagonal")
 gr.elements_exc("Au,Ag")
 gr.saveto("./mindat_data")
 ```
@@ -74,25 +77,37 @@
 ### 3. Search Geomaterials Using Keywords
 
 ```python
 from openmindat import GeomaterialSearchRetriever
 
 gsr = GeomaterialSearchRetriever()
 gsr.geomaterials_search("quartz, green, hexagonal")
-gsr.save('my_filename')
+gsr.save("filename")
+
+# Alternatively, you can get the list object directly:
+gsr = GeomaterialSearchRetriever()
+gsr.geomaterials_search("ruby, red, hexagonal")
+print(gsr.get_list())
 ```
 
 ### 4. Retrieve Localities
 
+:exclamation: Some country names, e.g., United States and United Kingdom, are not working due to server-side problems, which will be fixed in the future.
+
 ```python
 from openmindat import LocalitiesRetriever
 
 lr = LocalitiesRetriever()
 lr.country("France").txt("mine")
 lr.save()
+
+# Alternatively, you can get the list object directly:
+lr = LocalitiesRetriever()
+lr.country("Canada").description("mine")
+print(lr.get_list())
 ```
 
 ### 5. Retrieve Type Localities for IMA-Approved Mineral Species
 
 ```python
 from openmindat import GeomaterialRetriever
 
@@ -163,16 +178,23 @@
         <img src="https://github.com/ChuBL/OpenMindat/blob/main/Logo/NSF_Official_logo_Low_Res.png?raw=true"  width="10%">
 </p>
 
 - This work is supported by NSF, Award #2126315.
 
 ## Updating Logs
 
+### 0.0.4
+**Released:** Apr 14, 2024
+
+- Tentative issue: Data queries involving multiple pages might return an `Internal Server Error` due to server-end issues. [Related GitHub issue](https://github.com/ChuBL/OpenMindat/issues/12)
+- Added support to getting list objects of obtained data in addition to saving it to local directories.
+
 ### 0.0.3
 **Released:** Apr 11, 2024
+
 - Tentative issue: Data queries involving multiple pages might return an `Internal Server Error` due to server-end issues. 
 - Now supporting more Mindat endpoints. Not fully tested. Feedback is welcome.
 - Revised API key obtaining workflow.
 
 ### 0.0.1
 **Released:** Dec 14, 2023
```

### Comparing `openmindat-0.0.3/README.md` & `openmindat-0.0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 
 This is a test version of the OpenMindat Python package, designed to facilitate querying and retrieving data on minerals and geomaterials from the Mindat API. It provides classes for detailed queries based on various attributes like IMA status, keywords, and specific geomaterial properties.
 
 GitHub Repository: [OpenMindat Python Package](https://github.com/ChuBL/OpenMindat)
 
 ## Get Started
 
-> If you do not have a Mindat API key, please refer to [How to Get My Mindat API Key or Token?](https://www.mindat.org/a/how_to_get_my_mindat_api_key)
-
 ### Install via Pip
 
 ```console
 foo@bar:~$ pip install openmindat
 ```
 
 ### Import the Package in Python
@@ -26,19 +24,24 @@
 
 ```python
 import os
 
 os.environ["MINDAT_API_KEY"] = 'Your_Mindat_API_Key'
 ```
 
-You can also set the API key by following the instructions when using the following queries.
+> If you do not have a Mindat API key, please refer to [How to Get My Mindat API Key or Token?](https://www.mindat.org/a/how_to_get_my_mindat_api_key)
+
+You can also set the API key by following the general queries.
 
 ### 1. Perform Detailed Queries on Geomaterials
 
+:exclamation: Temporarily Outage, see https://github.com/ChuBL/OpenMindat/issues/12
+
 ```python
+# Temporarily Outage, see https://github.com/ChuBL/OpenMindat/issues/12
 from openmindat import GeomaterialRetriever
 
 gr = GeomaterialRetriever()
 gr.density_min(2.0).density_max(5.0).crystal_system("Hexagonal")
 gr.elements_exc("Au,Ag")
 gr.saveto("./mindat_data")
 ```
@@ -56,25 +59,37 @@
 ### 3. Search Geomaterials Using Keywords
 
 ```python
 from openmindat import GeomaterialSearchRetriever
 
 gsr = GeomaterialSearchRetriever()
 gsr.geomaterials_search("quartz, green, hexagonal")
-gsr.save('my_filename')
+gsr.save("filename")
+
+# Alternatively, you can get the list object directly:
+gsr = GeomaterialSearchRetriever()
+gsr.geomaterials_search("ruby, red, hexagonal")
+print(gsr.get_list())
 ```
 
 ### 4. Retrieve Localities
 
+:exclamation: Some country names, e.g., United States and United Kingdom, are not working due to server-side problems, which will be fixed in the future.
+
 ```python
 from openmindat import LocalitiesRetriever
 
 lr = LocalitiesRetriever()
 lr.country("France").txt("mine")
 lr.save()
+
+# Alternatively, you can get the list object directly:
+lr = LocalitiesRetriever()
+lr.country("Canada").description("mine")
+print(lr.get_list())
 ```
 
 ### 5. Retrieve Type Localities for IMA-Approved Mineral Species
 
 ```python
 from openmindat import GeomaterialRetriever
 
@@ -145,16 +160,23 @@
         <img src="https://github.com/ChuBL/OpenMindat/blob/main/Logo/NSF_Official_logo_Low_Res.png?raw=true"  width="10%">
 </p>
 
 - This work is supported by NSF, Award #2126315.
 
 ## Updating Logs
 
+### 0.0.4
+**Released:** Apr 14, 2024
+
+- Tentative issue: Data queries involving multiple pages might return an `Internal Server Error` due to server-end issues. [Related GitHub issue](https://github.com/ChuBL/OpenMindat/issues/12)
+- Added support to getting list objects of obtained data in addition to saving it to local directories.
+
 ### 0.0.3
 **Released:** Apr 11, 2024
+
 - Tentative issue: Data queries involving multiple pages might return an `Internal Server Error` due to server-end issues. 
 - Now supporting more Mindat endpoints. Not fully tested. Feedback is welcome.
 - Revised API key obtaining workflow.
 
 ### 0.0.1
 **Released:** Dec 14, 2023
```

### Comparing `openmindat-0.0.3/openmindat/__init__.py` & `openmindat-0.0.4/openmindat/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,34 @@
 """
 This module provides a suite of tools for querying mineral and geomaterial data from the Mindat API.
 These classes offer flexible query parameters, method chaining, and functionality to save query results to a specified location.
 
 Attributes:
     MineralsIMARetriever (class): A class for querying mineral data based on IMA status and other parameters.
+    MineralIdRetriever (class): A class for querying mineral IMA data based on id.
     GeomaterialSearchRetriever (class): A class for searching geomaterials using specific keywords.
     GeomaterialRetriever (class): A class for performing detailed queries on geomaterials.
+    GeomaterialIdRetriever (class): A class for querying geomaterials based on id.
+    GeomaterialDictRetriever (class): A class for displaying a dictionary of values for a field.
+    LocalitiesRetriever (class): A class for performing detailed queries based on localities.
+    LocalitiesIdRetriever (class): A class for finding locality data based on id.
+    LocalitiesAgeRetriever (class): A class for querying locality age data.
+    LocalitiesAgeIdRetriever (class): A class for querying locality age based on id.
+    LocalitiesStatusRetriever (class): A class for querying locality status data.
+    LocalitiesStatusIdRetriever (class): A class for querying locality status based on id.
+    LocalitiesTypeRetriever (class): A class for querying locality type data.
+    LocalitiesTypeIdRetriever (class): A class for querying locality type based on id.
+    GeoRegionRetriever (class): A class for querying locality georegion data.
+    LocObjectRetriever (class): A class for querying locality object data based on id.
+    CountriesListRetriever (class): A class for querying country data from OpenMindat.
+    CountriesIdRetriever (class): A class for querying country data based on id.
+    DanaRetriever (class): A class for querying dana-8 group and subgroup data. 
+    StrunzRetriever (class): A class for querying different types of nickel-strunz-10 data.
+    PhotoCountRetriever(class): A class to facilitate the retrieval of photo count data from the Mindat API.
+    
 
 Todo:
     * Expand the module with additional classes and functions as needed.
     * Implement additional filters and query options for enhanced data retrieval.
 
 Note:
     Ensure that the Mindat API is accessible and properly configured before using these classes.
```

### Comparing `openmindat-0.0.3/openmindat/countries.py` & `openmindat-0.0.4/openmindat/countries.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,20 +142,25 @@
         print("Retrieving countries. This may take a while... ")
        
         params = self._params
         end_point = self.end_point
         
         ma = mindat_api.MindatApi()        
         #clears params for next get statement     
-        self._init_params()
 
         if "page" in params:
-            return [ma.get_mindat_dict(params, end_point)]
+            results = [ma.get_mindat_dict(params, end_point)]
         else:
-            return ma.get_mindat_list_object(params, end_point)
+            results = ma.get_mindat_list_object(params, end_point)
+        
+        
+        self._init_params()
+        return results
+            
+            
         
 
 class CountriesIdRetriever:
     """
     A class to facilitate the retrieval of country data from the Mindat API using an id.
     For more information visit: https://api.mindat.org/schema/redoc/#tag/countries/operation/countries_retrieve
 
@@ -267,18 +272,18 @@
             >>> france = cidr.id(2).get_liat()
 
         '''
         
         print("Retrieving countries. This may take a while... ")
        
         params = self._params
-        end_point = self.end_point
-        
-        #clears params for next get statement     
-        self._init_params()
+        end_point = self.end_point    
         
         ma = mindat_api.MindatApi()
-        return [ma.get_mindat_dict(params, end_point)]
+        results = [ma.get_mindat_dict(params, end_point)]
+        
+        self._init_params()
+        return results
 
 if __name__ == '__main__':
     cidr = CountriesIdRetriever()
     cidr.id(2).save()
```

### Comparing `openmindat-0.0.3/openmindat/dana8.py` & `openmindat-0.0.4/openmindat/dana8.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,21 +181,21 @@
         
         print("Retrieving dana-8. This may take a while... ")
        
         params = self._params        
         
         if self.sub_endpoint != '':
             end_point = '/'.join(['dana-8', self.sub_endpoint])
-            
-        #clears params for next get statement     
-        self._init_params()
         
         ma = mindat_api.MindatApi()
         if self.sub_endpoint.isnumeric():
-            return [ma.get_mindat_dict(params, end_point)]
+            results = [ma.get_mindat_dict(params, end_point)]
         else:
-            return ma.get_mindat_list_object(params, end_point)
+            results = ma.get_mindat_list_object(params, end_point)
+        
+        self._init_params()
+        return results
 
 
 if __name__ == '__main__':
     dr = DanaRetriever()
     dr.groups().save()
```

### Comparing `openmindat-0.0.3/openmindat/geomaterials.py` & `openmindat-0.0.4/openmindat/geomaterials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1310,19 +1310,19 @@
         '''
         
         print("Retrieving geomaterials. This may take a while... ")
        
         params = self._params
         end_point = self.end_point
         
-        #clears params for next get statement     
-        self._init_params()
-        
         ma = mindat_api.MindatApi()
-        return ma.get_mindat_list_object(params, end_point)
+        results = ma.get_mindat_list_object(params, end_point)
+        
+        self._init_params()
+        return results
 
 
 class GeomaterialIdRetriever:
     """
     This module provides the GeomaterialIdRetriever class for returning geomaterial by id
     For more information visit: https://api.mindat.org/schema/redoc/#tag/geomaterials/operation/geomaterials_retrieve
 
@@ -1428,32 +1428,32 @@
         self.saveto('', file_name)
         
     def get_list(self):
         '''
         Executes the query to retrieve geomaterial with a corresponding id and returns a dictionary.
 
         Returns:
-            List of DIctionaries.
+            List of Dictionaries.
 
         Example:
             >>> gir = GeomaterialIdRetriever()
             >>> geo5 = gir.id(5).get_list()
 
         '''
         
         print("Retrieving geomaterials. This may take a while... ")
        
         params = self._params
         end_point = '/'.join([self.end_point, self.sub_endpoint])
         
-        #clears params for next get statement     
-        self._init_params()
-        
         ma = mindat_api.MindatApi()
-        return [ma.get_mindat_dict(params, end_point)]
+        results = [ma.get_mindat_dict(params, end_point)]
+        
+        self._init_params()
+        return results
         
         
         
         #NOT YET WORKING, check in to see if it returns list vs item
 class GeomaterialDictRetriever:
     """
     This module provides the GeomaterialDictRetriever class for returning geomaterial Dictionaries
@@ -1538,20 +1538,20 @@
 
         '''
         
         print("Retrieving geomaterials. This may take a while... ")
        
         params = self._params
         end_point = self.end_point
+
+        ma = mindat_api.MindatApi()
+        results = [ma.get_mindat_dict(params, end_point)]
         
-        #clears params for next get statement     
         self._init_params()
-        
-        ma = mindat_api.MindatApi()
-        return [ma.get_mindat_dict(params, end_point)]
+        return results
         
 
 if __name__ == '__main__':
     gr = GeomaterialRetriever()
     # gr.cleavagetype('Distinct/Good').colour('blue').crystal_system(["Amorphous", "Hexagonal"]).save()
     gr.id__in("3337, 114").save()
     # print(gr.density_max('9').density_min(8).ordering('-name')._params)
```

### Comparing `openmindat-0.0.3/openmindat/geomaterials_search.py` & `openmindat-0.0.4/openmindat/geomaterials_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,17 +95,17 @@
         '''
         
         print("Retrieving geomaterial search. This may take a while... ")
        
         params = self._params
         end_point = self.end_point
         
-        #clears params for next get statement     
-        self._init_params()
-        
         ma = mindat_api.MindatApi()
-        return [ma.get_mindat_dict(params, end_point)]
+        results = [ma.get_mindat_dict(params, end_point)]
+        
+        self._init_params()
+        return results
 
 
 if __name__ == '__main__':
     gsr = GeomaterialSearchRetriever()
     gsr.geomaterials_search("quartz, green, hexagonal").save()
```

### Comparing `openmindat-0.0.3/openmindat/localities.py` & `openmindat-0.0.4/openmindat/localities.py`

 * *Files 23% similar despite different names*

```diff
@@ -55,17 +55,57 @@
             self: The LocalitiesRetriever object.
 
         Example:
             >>> lr = LocalitiesRetriever()
             >>> lr.country("United States")
             >>> lr.saveto()
         '''
-        self._params.update({
-            'country': COUNTRY_STR
-        })
+        valid_options = ["Afghanistan","Albania", "Algeria", "American Samoa", "Andorra", "Angola", "Anguilla", "Antigua and Barbuda",
+                         "Argentina", "Armenia", "Aruba", "Ashmore and Cartier Islands", "Australia", "Austria", "Azerbaijan", "Bahamas",
+                         "Bahrain", "Bangladesh", "Barbados", "Belarus", "Belgium", "Belize", "Benin", "Bermuda", "Bhutan",
+                         "Bolivia", "Bosnia And Herzegovina", "Botswana", "Bouvet Island", "Brazil", "British Indian Ocean Territories",
+                         "British Solomon Islands", "British Virgin Islands", "Brunei", "Bulgaria", "Burkina Faso", "Burundi", "Cambodia",
+                         "Cameroon", "Canada", "Cape Verde", "Cayman Islands", "Central African Republic", "Chad", "Chile", "China",
+                         "Christmas Island", "Cocos Islands", "Colombia", "Comoro Islands", "Cook Islands", "Costa Rica", "Croatia",
+                         "Cuba", "Cyprus", "Czech Republic", "Democratic Republic of the Congo", "Denmark", "Djibouti", "Dominica",
+                         "Dominican Republic", "East Timor", "Ecuador", "Egypt", "El Salvador", "Equatorial Guinea", "Estonia",
+                         "Ethiopia", "Faeroe Islands", "Falkland Islands", "Federated States of Micronesia", "Fiji", "Finland",
+                         "France", "French Guiana", "French Polynesia", "Gabon", "Gambia", "Georgia", "Germany", "Ghana", "Gibraltar",
+                         "Greece", "Greenland", "Grenada", "Guadeloupe", "Guam", "Guatemala", "Guernsey", "Guinea", "Guinea-Bissau",
+                         "Guyana", "Haiti", "Honduras", "Hong Kong", "Hungary", "Iceland", "India", "Indonesia", "Iran", "Iraq",
+                         "Ireland", "Isle of Man", "Israel", "Italy", "Ivory Coast (Côte d'Ivoire)", "Jamaica", "Japan", "Jersey",
+                         "Jordan", "Kazakhstan", "Kenya", "Kiribati", "Kosovo", "Kuwait", "Kyrgyzstan", "Laos", "Latvia", "Lebanon",
+                         "Lesotho", "Liberia", "Libya", "Liechtenstein", "Lithuania", "Luxembourg", "Macao", "Madagascar", "Malawi",
+                         "Malaysia", "Maldives", "Mali", "Malta", "Martinique", "Mauritania", "Mauritius", "Mexico", "Moldova",
+                         "Monaco", "Mongolia", "Montenegro", "Montserrat", "Morocco", "Mozambique", "Myanmar", "Namibia", "Nauru",
+                         "Nepal", "Netherlands", "Netherlands Antilles", "New Caledonia", "New Zealand", "Nicaragua", "Niger",
+                         "Nigeria", "North Korea", "Norway", "Oman", "Pakistan", "Panama", "Papua New Guinea", "Paraguay", "Peru",
+                         "Philippines", "Poland", "Portugal", "Puerto Rico", "Qatar", "Republic of Congo (Brazzaville)",
+                         "Republic of Macedonia", "Reunion Island", "Romania", "Russia", "Rwanda", "Saint Helena", "Saint Lucia",
+                         "Saint Vincent and the Grenadines", "San Marino", "Sao Tome And Principe", "Saudi Arabia", "Senegal",
+                         "Serbia", "Seychelles", "Sierra Leone", "Singapore", "Slovakia", "Slovenia", "Solomon Islands", "Somalia",
+                         "South Africa", "South Korea", "Spain", "Sri Lanka", "St Christopher-Nevis Islands", "Sudan", "Suriname",
+                         "Swaziland", "Sweden", "Switzerland", "Syria", "Taiwan", "Tajikistan", "Tanzania", "Thailand", "Togo",
+                         "Tonga", "Trinidad And Tobago", "Tunisia", "Turkey", "Turkmenistan", "Turks And Caicos Islands", "Tuvalu",
+                         "U.S. Virgin Islands", "Uganda", "Ukraine", "United Arab Emirates", "United Kingdom", "United States",
+                         "Uruguay", "Uzbekistan", "Vanuatu (Republic of Vanuatu; New Hebrides) ", "Venezuela", "Vietnam",
+                         "Western Sahara", "Western Samoa", "Yemen", "Zambia", "Zimbabwe"]
+        
+        if COUNTRY_STR is not None:
+            if isinstance(COUNTRY_STR, str):
+                country = COUNTRY_STR  
+            else:
+                raise TypeError("Country must be a string")
+
+            if country not in valid_options:
+                raise ValueError(f"Invalid country: {country}. Valid options are: {', '.join(valid_options)}")
+
+            self._params.update({
+                'country': country
+            })  
 
         return self
     
     def cursor(self, CURSOR_STR):
         '''
         Sets the pagination cursor value for the query.
 
@@ -394,19 +434,19 @@
         '''
         
         print("Retrieving localities. This may take a while... ")
        
         params = self._params
         end_point = self.end_point
         
-        #clears params for next get statement     
-        self._init_params()
-        
         ma = mindat_api.MindatApi()
-        return ma.get_mindat_list_object(params, end_point)
+        results = ma.get_mindat_list_object(params, end_point)
+        
+        self._init_params()
+        return results
         
         
 class LocalitiesIdRetriever:
     """
     This module provides the LocalitiesIdRetriever class for returning localities by id
     For more information visit: https://api.mindat.org/schema/redoc/#tag/localities/operation/localities_retrieve
 
@@ -517,16 +557,16 @@
         '''
         
         print("Retrieving localities. This may take a while... ")
        
         params = self._params
         end_point = '/'.join([self.end_point, self.sub_endpoint])
         
-        #clears params for next get statement     
-        self._init_params()
-        
         ma = mindat_api.MindatApi()
-        return [ma.get_mindat_dict(params, end_point)]
+        results = [ma.get_mindat_dict(params, end_point)]
+        
+        self._init_params()
+        return results
 
 if __name__ == '__main__':
     lr = LocalitiesRetriever()
     lr.country("UK").save()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openmindat-0.0.3/openmindat/localities_age.py` & `openmindat-0.0.4/openmindat/localities_age.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,21 +142,21 @@
         print("Retrieving localities search. This may take a while... ")
        
         params = self._params
         end_point = self.end_point
         
         ma = mindat_api.MindatApi()
         
-        #clears params for next get statement     
-        self._init_params()
-        
         if "page" in params:
-            return [ma.get_mindat_dict(params, end_point)]
+            results = [ma.get_mindat_dict(params, end_point)]
         else:
-            return ma.get_mindat_list_object(params, end_point)
+            results = ma.get_mindat_list_object(params, end_point)
+            
+        self._init_params()
+        return results
         
         
 class LocalitiesAgeIdRetriever:
     """
     A class to facilitate the retrieval of locality data from the Mindat API filtered by id.
     For more information visit: https://api.mindat.org/schema/redoc/#tag/locality_age/operation/locality_age_retrieve
 
@@ -272,16 +272,16 @@
         '''
         
         print("Retrieving localities. This may take a while... ")
        
         params = self._params
         end_point = '/'.join([self.end_point, self.sub_endpoint])
         
-        #clears params for next get statement     
-        self._init_params()
-        
         ma = mindat_api.MindatApi()
-        return [ma.get_mindat_dict(params, end_point)]
+        results = [ma.get_mindat_dict(params, end_point)]
+        
+        self._init_params()
+        return results
 
 if __name__ == '__main__':
     lair = LocalitiesAgeIdRetriever()
     lair.id(2).save()
```

### Comparing `openmindat-0.0.3/openmindat/localities_status.py` & `openmindat-0.0.4/openmindat/localities_status.py`

 * *Files 6% similar despite different names*

```diff
@@ -141,21 +141,22 @@
         
         print("Retrieving localities search. This may take a while... ")
        
         params = self._params
         end_point = self.end_point
         
         ma = mindat_api.MindatApi()
-        #clears params for next get statement     
-        self._init_params()
         
         if "page" in params:
-            return [ma.get_mindat_dict(params, end_point)]
+            results = [ma.get_mindat_dict(params, end_point)]
         else:
-            return ma.get_mindat_list_object(params, end_point)
+            results = ma.get_mindat_list_object(params, end_point)
+            
+        self._init_params()
+        return results
         
         
 class LocalitiesStatusIdRetriever:
     """
     A class to facilitate the retrieval of locality data from the Mindat API filtered by id.
     For more information visit: https://api.mindat.org/schema/redoc/#tag/locality_status/operation/locality_status_retrieve
 
@@ -270,16 +271,16 @@
         '''
         
         print("Retrieving localities. This may take a while... ")
        
         params = self._params
         end_point = '/'.join([self.end_point, self.sub_endpoint])
         
-        #clears params for next get statement     
-        self._init_params()
-        
         ma = mindat_api.MindatApi()
-        return [ma.get_mindat_dict(params, end_point)]
+        results = [ma.get_mindat_dict(params, end_point)]
+        
+        self._init_params()
+        return results
 
 if __name__ == '__main__':
     lsir = LocalitiesStatusIdRetriever()
     lsir.id(2).save()
```

### Comparing `openmindat-0.0.3/openmindat/localities_type.py` & `openmindat-0.0.4/openmindat/localities_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,21 +140,22 @@
         
         print("Retrieving localities search. This may take a while... ")
        
         params = self._params
         end_point = self.end_point
         
         ma = mindat_api.MindatApi()
-        #clears params for next get statement     
-        self._init_params()
         
         if "page" in params:
-            return [ma.get_mindat_dict(params, end_point)]
+            results = [ma.get_mindat_dict(params, end_point)]
         else:
-            return ma.get_mindat_list_object(params, end_point)
+            results = ma.get_mindat_list_object(params, end_point)
+            
+        self._init_params()
+        return results
         
         
 class LocalitiesTypeIdRetriever:
     """
     A class to facilitate the retrieval of locality data from the Mindat API filtered by id.
     For more information visit: https://api.mindat.org/schema/redoc/#tag/locality_type/operation/locality_type_retrieve
 
@@ -269,16 +270,16 @@
         '''
         
         print("Retrieving localities. This may take a while... ")
        
         params = self._params
         end_point = '/'.join([self.end_point, self.sub_endpoint])
         
-        #clears params for next get statement     
-        self._init_params()
-        
         ma = mindat_api.MindatApi()
-        return [ma.get_mindat_dict(params, end_point)]
+        results = [ma.get_mindat_dict(params, end_point)]
+        
+        self._init_params()
+        return results
 
 if __name__ == '__main__':
     ltir = LocalitiesTypeIdRetriever()
     ltir.id(2).save()
```

### Comparing `openmindat-0.0.3/openmindat/locgeoregion2.py` & `openmindat-0.0.4/openmindat/locgeoregion2.py`

 * *Files 5% similar despite different names*

```diff
@@ -141,19 +141,19 @@
         print("Retrieving local geoRegion search. This may take a while... ")
        
         params = self._params
         end_point = self.end_point
         
         ma = mindat_api.MindatApi()
         
-        #clears params for next get statement     
-        self._init_params()
-        
         if "page" in params:
-            return [ma.get_mindat_dict(params, end_point)]
+            results = [ma.get_mindat_dict(params, end_point)]
         else:
-            return ma.get_mindat_list_object(params, end_point)
+            results = ma.get_mindat_list_object(params, end_point)
+            
+        self._init_params()
+        return results
             
             
 if __name__ == '__main__':
     grr = GeoRegionRetriever()
     grr.page(1).save()
```

### Comparing `openmindat-0.0.3/openmindat/locobject.py` & `openmindat-0.0.4/openmindat/locobject.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,16 +118,16 @@
         '''
         
         print("Retrieving locObject. This may take a while... ")
        
         params = self._params
         end_point = '/'.join([self.end_point, self.sub_endpoint])
         
-        #clears params for next get statement     
-        self._init_params()
-        
         ma = mindat_api.MindatApi()
-        return [ma.get_mindat_dict(params, end_point)]
+        results = [ma.get_mindat_dict(params, end_point)]
+        
+        self._init_params()
+        return results
 
 if __name__ == '__main__':
     lor = LocobjectRetriever()
     lor.id(2).save()
```

### Comparing `openmindat-0.0.3/openmindat/mindat_api.py` & `openmindat-0.0.4/openmindat/mindat_api.py`

 * *Files identical despite different names*

### Comparing `openmindat-0.0.3/openmindat/minerals_ima.py` & `openmindat-0.0.4/openmindat/minerals_ima.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,19 +314,19 @@
         '''
         
         print("Retrieving minerals. This may take a while... ")
        
         params = self._params
         end_point = self.end_point
         
-        #clears params for next get statement     
-        self._init_params()
-        
         ma = mindat_api.MindatApi()
-        return ma.get_mindat_list_object(params, end_point)
+        results = ma.get_mindat_list_object(params, end_point)
+        
+        self._init_params()
+        return results
         
         
 class MineralsIdRetriever:
     """
     This module provides the MineralsIdRetriever class for returning Minerals by id
     For more information visit: https://api.mindat.org/schema/redoc/#tag/minerals_ima/operation/minerals_ima_retrieve
 
@@ -437,17 +437,17 @@
         '''
         
         print("Retrieving minerals. This may take a while... ")
        
         params = self._params
         end_point = '/'.join([self.end_point, self.sub_endpoint])
         
-        #clears params for next get statement     
-        self._init_params()
-        
         ma = mindat_api.MindatApi()
-        return [ma.get_mindat_dict(params, end_point)]
+        results = [ma.get_mindat_dict(params, end_point)]
+        
+        self._init_params()
+        return results
 
 
 if __name__ == '__main__':
     mir = MineralsIMARetriever()
     mir.ima('1').saveto()
```

### Comparing `openmindat-0.0.3/openmindat/nickel_strunz.py` & `openmindat-0.0.4/openmindat/nickel_strunz.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,19 +196,20 @@
         
         print("Retrieving nickel-strunz. This may take a while... ")
        
         params = self._params
         end_point = '/'.join([self.end_point, self.sub_endpoint])
         
         ma = mindat_api.MindatApi()
-        #clears params for next get statement     
-        self._init_params()
         
         if "classes" in self.sub_endpoint:
-            return [ma.get_mindat_dict(params, end_point)]
+            results = [ma.get_mindat_dict(params, end_point)]
         else:
-            return ma.get_mindat_list_object(params, end_point)
+            results = ma.get_mindat_list_object(params, end_point)
+            
+        self._init_params()
+        return results
 
 
 if __name__ == '__main__':
     sr = StrunzRetriever()
     sr.classes().save()
```

### Comparing `openmindat-0.0.3/openmindat/photo_count.py` & `openmindat-0.0.4/openmindat/photo_count.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,16 +88,16 @@
         '''
         
         print("Retrieving photo count. This may take a while... ")
        
         params = self._params
         end_point = self.end_point
         
-        #clears params for next get statement     
-        self._init_params()
-        
         ma = mindat_api.MindatApi()
-        return [ma.get_mindat_dict(params, end_point)]
+        results = [ma.get_mindat_dict(params, end_point)]
+        
+        self._init_params()
+        return results
 
 if __name__ == '__main__':
     pcr = PhotoCountRetriever()
     pcr.save()
```

### Comparing `openmindat-0.0.3/openmindat.egg-info/PKG-INFO` & `openmindat-0.0.4/openmindat.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmindat
-Version: 0.0.3
+Version: 0.0.4
 Summary: An alpha version for OpenMindat package
 Home-page: https://github.com/ChuBL/OpenMindat
 Author: Jiyin Zhang
 Author-email: jiyinz@uidaho.edu
 License: Apache Software License
 Keywords: mindat openmindat mineral data python api
 Classifier: Development Status :: 3 - Alpha
@@ -20,16 +20,14 @@
 
 This is a test version of the OpenMindat Python package, designed to facilitate querying and retrieving data on minerals and geomaterials from the Mindat API. It provides classes for detailed queries based on various attributes like IMA status, keywords, and specific geomaterial properties.
 
 GitHub Repository: [OpenMindat Python Package](https://github.com/ChuBL/OpenMindat)
 
 ## Get Started
 
-> If you do not have a Mindat API key, please refer to [How to Get My Mindat API Key or Token?](https://www.mindat.org/a/how_to_get_my_mindat_api_key)
-
 ### Install via Pip
 
 ```console
 foo@bar:~$ pip install openmindat
 ```
 
 ### Import the Package in Python
@@ -44,19 +42,24 @@
 
 ```python
 import os
 
 os.environ["MINDAT_API_KEY"] = 'Your_Mindat_API_Key'
 ```
 
-You can also set the API key by following the instructions when using the following queries.
+> If you do not have a Mindat API key, please refer to [How to Get My Mindat API Key or Token?](https://www.mindat.org/a/how_to_get_my_mindat_api_key)
+
+You can also set the API key by following the general queries.
 
 ### 1. Perform Detailed Queries on Geomaterials
 
+:exclamation: Temporarily Outage, see https://github.com/ChuBL/OpenMindat/issues/12
+
 ```python
+# Temporarily Outage, see https://github.com/ChuBL/OpenMindat/issues/12
 from openmindat import GeomaterialRetriever
 
 gr = GeomaterialRetriever()
 gr.density_min(2.0).density_max(5.0).crystal_system("Hexagonal")
 gr.elements_exc("Au,Ag")
 gr.saveto("./mindat_data")
 ```
@@ -74,25 +77,37 @@
 ### 3. Search Geomaterials Using Keywords
 
 ```python
 from openmindat import GeomaterialSearchRetriever
 
 gsr = GeomaterialSearchRetriever()
 gsr.geomaterials_search("quartz, green, hexagonal")
-gsr.save('my_filename')
+gsr.save("filename")
+
+# Alternatively, you can get the list object directly:
+gsr = GeomaterialSearchRetriever()
+gsr.geomaterials_search("ruby, red, hexagonal")
+print(gsr.get_list())
 ```
 
 ### 4. Retrieve Localities
 
+:exclamation: Some country names, e.g., United States and United Kingdom, are not working due to server-side problems, which will be fixed in the future.
+
 ```python
 from openmindat import LocalitiesRetriever
 
 lr = LocalitiesRetriever()
 lr.country("France").txt("mine")
 lr.save()
+
+# Alternatively, you can get the list object directly:
+lr = LocalitiesRetriever()
+lr.country("Canada").description("mine")
+print(lr.get_list())
 ```
 
 ### 5. Retrieve Type Localities for IMA-Approved Mineral Species
 
 ```python
 from openmindat import GeomaterialRetriever
 
@@ -163,16 +178,23 @@
         <img src="https://github.com/ChuBL/OpenMindat/blob/main/Logo/NSF_Official_logo_Low_Res.png?raw=true"  width="10%">
 </p>
 
 - This work is supported by NSF, Award #2126315.
 
 ## Updating Logs
 
+### 0.0.4
+**Released:** Apr 14, 2024
+
+- Tentative issue: Data queries involving multiple pages might return an `Internal Server Error` due to server-end issues. [Related GitHub issue](https://github.com/ChuBL/OpenMindat/issues/12)
+- Added support to getting list objects of obtained data in addition to saving it to local directories.
+
 ### 0.0.3
 **Released:** Apr 11, 2024
+
 - Tentative issue: Data queries involving multiple pages might return an `Internal Server Error` due to server-end issues. 
 - Now supporting more Mindat endpoints. Not fully tested. Feedback is welcome.
 - Revised API key obtaining workflow.
 
 ### 0.0.1
 **Released:** Dec 14, 2023
```

### Comparing `openmindat-0.0.3/openmindat.egg-info/SOURCES.txt` & `openmindat-0.0.4/openmindat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openmindat-0.0.3/setup.py` & `openmindat-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 setup(name='openmindat',
-      version='0.0.3',
+      version='0.0.4',
       description='An alpha version for OpenMindat package',
       long_description=open('README.md').read(),
       long_description_content_type='text/markdown',
       classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: Apache Software License',
         "Programming Language :: Python :: 3",
```

