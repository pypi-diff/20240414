# Comparing `tmp/pyweatherfr-5.1.0.tar.gz` & `tmp/pyweatherfr-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweatherfr-5.1.0.tar", last modified: Sun Apr 14 07:17:13 2024, max compression
+gzip compressed data, was "pyweatherfr-5.1.1.tar", last modified: Sun Apr 14 08:22:31 2024, max compression
```

## Comparing `pyweatherfr-5.1.0.tar` & `pyweatherfr-5.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:17:12.997019 pyweatherfr-5.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-14 07:16:34.000000 pyweatherfr-5.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-14 07:17:12.997019 pyweatherfr-5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-14 07:16:34.000000 pyweatherfr-5.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-14 07:16:34.000000 pyweatherfr-5.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:17:12.993019 pyweatherfr-5.1.0/pyweatherfr/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-14 07:16:34.000000 pyweatherfr-5.1.0/pyweatherfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-04-14 07:16:34.000000 pyweatherfr-5.1.0/pyweatherfr/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    41338 2024-04-14 07:16:34.000000 pyweatherfr-5.1.0/pyweatherfr/pyweatherfr.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-14 07:16:34.000000 pyweatherfr-5.1.0/pyweatherfr/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:17:12.997019 pyweatherfr-5.1.0/pyweatherfr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-14 07:17:12.000000 pyweatherfr-5.1.0/pyweatherfr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-14 07:17:12.000000 pyweatherfr-5.1.0/pyweatherfr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 07:17:12.000000 pyweatherfr-5.1.0/pyweatherfr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-14 07:17:12.000000 pyweatherfr-5.1.0/pyweatherfr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 07:16:39.000000 pyweatherfr-5.1.0/pyweatherfr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-14 07:17:12.000000 pyweatherfr-5.1.0/pyweatherfr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-14 07:17:12.000000 pyweatherfr-5.1.0/pyweatherfr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 07:17:12.997019 pyweatherfr-5.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-14 07:16:34.000000 pyweatherfr-5.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:22:31.887678 pyweatherfr-5.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-14 08:21:41.000000 pyweatherfr-5.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-14 08:22:31.887678 pyweatherfr-5.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-14 08:21:41.000000 pyweatherfr-5.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-14 08:21:41.000000 pyweatherfr-5.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:22:31.883678 pyweatherfr-5.1.1/pyweatherfr/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-14 08:21:41.000000 pyweatherfr-5.1.1/pyweatherfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-04-14 08:21:41.000000 pyweatherfr-5.1.1/pyweatherfr/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42195 2024-04-14 08:21:41.000000 pyweatherfr-5.1.1/pyweatherfr/pyweatherfr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-14 08:21:41.000000 pyweatherfr-5.1.1/pyweatherfr/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:22:31.887678 pyweatherfr-5.1.1/pyweatherfr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-14 08:22:31.000000 pyweatherfr-5.1.1/pyweatherfr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-14 08:22:31.000000 pyweatherfr-5.1.1/pyweatherfr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 08:22:31.000000 pyweatherfr-5.1.1/pyweatherfr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-14 08:22:31.000000 pyweatherfr-5.1.1/pyweatherfr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 08:21:53.000000 pyweatherfr-5.1.1/pyweatherfr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-14 08:22:31.000000 pyweatherfr-5.1.1/pyweatherfr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-14 08:22:31.000000 pyweatherfr-5.1.1/pyweatherfr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 08:22:31.887678 pyweatherfr-5.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-14 08:21:41.000000 pyweatherfr-5.1.1/setup.py
```

### Comparing `pyweatherfr-5.1.0/LICENSE.txt` & `pyweatherfr-5.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.1.0/PKG-INFO` & `pyweatherfr-5.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 5.1.0
+Version: 5.1.1
 Summary: pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-5.1.0/README.md` & `pyweatherfr-5.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.1.0/pyweatherfr/args.py` & `pyweatherfr-5.1.1/pyweatherfr/args.py`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.1.0/pyweatherfr/pyweatherfr.py` & `pyweatherfr-5.1.1/pyweatherfr/pyweatherfr.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,22 +46,22 @@
 WARM = "\U0001F321"
 HOME = "\U0001F3E0"
 BOUSSOLE = "\U0001F9ED"
 CLOCK = "\U000023F0"
 THERMO = "\U0001F321"
 HUMIDITE = "\U0001F4A7"
 PLUIE = "\U0001F327"
-FLECHE_N = "\U0000FE0F"
-FLECHE_NW = "\U0000FE0F"
-FLECHE_W = "\U0000FE0F"
-FLECHE_SW = "\U0000FE0F"
-FLECHE_S = "\U0000FE0F"
-FLECHE_SE = "\U0000FE0F"
-FLECHE_E = "\U0000FE0F"
-FLECHE_NE = "\U0000FE0F"
+FLECHE_N = "\U00002B07"
+FLECHE_NO = "\U00002198"
+FLECHE_O = "\U000027A1"
+FLECHE_SO = "\U00002197"
+FLECHE_S = "\U00002B06"
+FLECHE_SE = "\U00002196"
+FLECHE_E = "\U00002B05"
+FLECHE_NE = "\U00002199"
 ELEPHANT = "\U0001F418"
 PLUME = "\U0001FAB6"
 PC ="\U0001f4bb"
 WARNING_WARM=30
 WARNING_FROID=0
 WARNING_SNOW=0.1
 WARNING_RAIN=0.1
@@ -299,50 +299,66 @@
         print(table)
 
 def calculer_direction(direction_vent_degres):
     if (
             direction_vent_degres <= 22.5
             or direction_vent_degres >= 360 - 22.5
         ):
-        direction = "N"
+        direction = "N  "
+        if not compute_args().nocolor:
+            direction=direction+FLECHE_N        
     if (
             direction_vent_degres <= 360 - 22.5
             and direction_vent_degres > 360 - 22.5 - 45
         ):
-        direction = "NO"
+        direction = "NO "
+        if not compute_args().nocolor:
+            direction=direction+FLECHE_NO        
     if (
             direction_vent_degres <= 360 - 22.5 - 45
             and direction_vent_degres > 360 - 22.5 - 90
         ):
-        direction = "O"
+        direction = "O  "
+        if not compute_args().nocolor:
+            direction=direction+FLECHE_O        
     if (
             direction_vent_degres <= 360 - 22.5 - 90
             and direction_vent_degres > 360 - 22.5 - 135
         ):
-        direction = "SO"
+        direction = "SO "
+        if not compute_args().nocolor:
+            direction=direction+FLECHE_SO        
     if (
             direction_vent_degres <= 360 - 22.5 - 135
             and direction_vent_degres > 360 - 22.5 - 180
         ):
-        direction = "S"
+        direction = "S  "
+        if not compute_args().nocolor:
+            direction=direction+FLECHE_S        
     if (
             direction_vent_degres <= 360 - 22.5 - 180
             and direction_vent_degres > 360 - 22.5 - 225
         ):
-        direction = "SE"
+        direction = "SE "
+        if not compute_args().nocolor:
+            direction=direction+FLECHE_SE        
     if (
             direction_vent_degres <= 360 - 22.5 - 225
             and direction_vent_degres > 360 - 22.5 - 270
         ):
-        direction = "E"
+        direction = "E  "
+        if not compute_args().nocolor:
+            direction=direction+FLECHE_E        
     if (
             direction_vent_degres <= 360 - 22.5 - 270
             and direction_vent_degres > 360 - 22.5 - 315
         ):
-        direction = "NE"
+        direction = "NE "
+        if not compute_args().nocolor:
+            direction=direction+FLECHE_NE
     return direction
 
 
 def traduction(current_weather_code,jour):
     if (
         current_weather_code == 0
         or current_weather_code == 1
@@ -683,20 +699,26 @@
 
 def obtain_city_data_from_ip():
 
     with urllib.request.urlopen("https://geolocation-db.com/json") as url:
         print_debug(
             "recherche de la localisation depuis https://geolocation-db.com/json"
         )
-        data = json.loads(url.read().decode())
+        resultat= url.read().decode()
+        print_debug(resultat)
+        data = json.loads(resultat)
         print_debug(str(json.dumps(data, indent=4,ensure_ascii=False)))
         ville = data["city"]
+        if ville ==None:
+            ville=""
         lat = str(data["latitude"])
         long = str(data["longitude"])
         dpt = str(data["state"])
+        if dpt ==None:
+            dpt=""
         country = str(data["country_name"])
         #if country==None or country!="France":
         #    print(my_colored("erreur : aucune ville trouvée. Si vous souhaitez rechercher une ville hors de France, ajoutez --world", "red"))
         #    exit(1)
         return ville, dpt, lat, long, country
```

### Comparing `pyweatherfr-5.1.0/pyweatherfr.egg-info/PKG-INFO` & `pyweatherfr-5.1.1/pyweatherfr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 5.1.0
+Version: 5.1.1
 Summary: pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-5.1.0/setup.py` & `pyweatherfr-5.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="pyweatherfr",
-    version="5.1.0",
+    version="5.1.1",
     description="pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)",
     long_description="The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme",
     url="https://github.com/thib1984/pyweatherfr",
     author="thib1984",
     author_email="thibault.garcon@gmail.com",
     license="MIT",
     packages=["pyweatherfr"],
```

