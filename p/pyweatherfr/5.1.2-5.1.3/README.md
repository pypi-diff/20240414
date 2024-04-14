# Comparing `tmp/pyweatherfr-5.1.2.tar.gz` & `tmp/pyweatherfr-5.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweatherfr-5.1.2.tar", last modified: Sun Apr 14 11:22:20 2024, max compression
+gzip compressed data, was "pyweatherfr-5.1.3.tar", last modified: Sun Apr 14 11:44:36 2024, max compression
```

## Comparing `pyweatherfr-5.1.2.tar` & `pyweatherfr-5.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:22:20.384011 pyweatherfr-5.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-14 11:21:37.000000 pyweatherfr-5.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-14 11:22:20.384011 pyweatherfr-5.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-14 11:21:37.000000 pyweatherfr-5.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-14 11:21:37.000000 pyweatherfr-5.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:22:20.384011 pyweatherfr-5.1.2/pyweatherfr/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-14 11:21:37.000000 pyweatherfr-5.1.2/pyweatherfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-04-14 11:21:37.000000 pyweatherfr-5.1.2/pyweatherfr/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    43357 2024-04-14 11:21:37.000000 pyweatherfr-5.1.2/pyweatherfr/pyweatherfr.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-14 11:21:37.000000 pyweatherfr-5.1.2/pyweatherfr/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:22:20.384011 pyweatherfr-5.1.2/pyweatherfr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-14 11:22:20.000000 pyweatherfr-5.1.2/pyweatherfr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-14 11:22:20.000000 pyweatherfr-5.1.2/pyweatherfr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 11:22:20.000000 pyweatherfr-5.1.2/pyweatherfr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-14 11:22:20.000000 pyweatherfr-5.1.2/pyweatherfr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 11:21:46.000000 pyweatherfr-5.1.2/pyweatherfr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-14 11:22:20.000000 pyweatherfr-5.1.2/pyweatherfr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-14 11:22:20.000000 pyweatherfr-5.1.2/pyweatherfr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 11:22:20.384011 pyweatherfr-5.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-14 11:21:37.000000 pyweatherfr-5.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:44:36.887249 pyweatherfr-5.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-14 11:43:59.000000 pyweatherfr-5.1.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-14 11:44:36.887249 pyweatherfr-5.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-14 11:43:59.000000 pyweatherfr-5.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-14 11:43:59.000000 pyweatherfr-5.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:44:36.887249 pyweatherfr-5.1.3/pyweatherfr/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-14 11:43:59.000000 pyweatherfr-5.1.3/pyweatherfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-04-14 11:43:59.000000 pyweatherfr-5.1.3/pyweatherfr/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41381 2024-04-14 11:43:59.000000 pyweatherfr-5.1.3/pyweatherfr/pyweatherfr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-14 11:43:59.000000 pyweatherfr-5.1.3/pyweatherfr/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:44:36.887249 pyweatherfr-5.1.3/pyweatherfr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-14 11:44:36.000000 pyweatherfr-5.1.3/pyweatherfr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-14 11:44:36.000000 pyweatherfr-5.1.3/pyweatherfr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 11:44:36.000000 pyweatherfr-5.1.3/pyweatherfr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-14 11:44:36.000000 pyweatherfr-5.1.3/pyweatherfr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 11:44:03.000000 pyweatherfr-5.1.3/pyweatherfr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-14 11:44:36.000000 pyweatherfr-5.1.3/pyweatherfr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-14 11:44:36.000000 pyweatherfr-5.1.3/pyweatherfr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 11:44:36.887249 pyweatherfr-5.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-14 11:43:59.000000 pyweatherfr-5.1.3/setup.py
```

### Comparing `pyweatherfr-5.1.2/LICENSE.txt` & `pyweatherfr-5.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.1.2/PKG-INFO` & `pyweatherfr-5.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 5.1.2
+Version: 5.1.3
 Summary: pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-5.1.2/README.md` & `pyweatherfr-5.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.1.2/pyweatherfr/args.py` & `pyweatherfr-5.1.3/pyweatherfr/args.py`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.1.2/pyweatherfr/pyweatherfr.py` & `pyweatherfr-5.1.3/pyweatherfr/pyweatherfr.py`

 * *Files 7% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     )
     pathlib.Path(ze_path).mkdir(parents=True, exist_ok=True)
     return ze_path
 
 
 def diff_jour(long,lat):
     tz=timezonefinder.TimezoneFinder().timezone_at(lng=float(long), lat=float(lat))
-    if not compute_args().date == None:
+    if not compute_args().date is None:
         if not est_format_date(compute_args().date):
             print(my_colored("erreur : format date invalide, format attendu yyyy-mm-dd", "red"))
             exit(1)
         diff = (pytz.timezone(tz).localize(datetime.datetime.strptime(compute_args().date, "%Y-%m-%d")) - datetime.datetime.now(tz=pytz.timezone(tz))).days +1
         print_debug(str(diff) + " jours")
         if diff>=15:
             print(my_colored("erreur : date invalide (limitée à +15 jour de la date actuelle)", "red"))
@@ -132,23 +132,23 @@
     if compute_args().pc:
         tz=str(tzlocal.get_localzone())
     if compute_args().utc:
         tz=str(pytz.utc)              
     print_debug(tz)
     if compute_args().now:
         previsions_courantes(ville, dpt, lat, long,tz)
-    elif not compute_args().date == None:
+    elif not compute_args().date is None:
         previsions_detaillees(ville, dpt, lat, long,tz)        
     elif compute_args().jour is None:
         previsions_generiques(ville, dpt, lat, long,tz)
     else:
         previsions_detaillees(ville, dpt, lat, long,tz)
     if not compute_args().town and not compute_args().gps:   
         print(my_colored("warning : si vous utilisez un proxy ou un VPN, la localisation peut être incorrecte", "yellow"))
-    if country ==None:
+    if country is None:
         print(my_colored("warning : ville potentiellement hors de France, les prévisions et données peuvent être moins précises", "yellow"))
     elif  country!="France":
         print(my_colored("warning : ville hors de France, les prévisions et données peuvent être moins précises", "yellow"))
 
 
 def previsions_detaillees(ville, dpt, lat, long, tz):
 
@@ -359,15 +359,15 @@
     if (
             direction_vent_degres <= 360 - 22.5 - 270
             and direction_vent_degres > 360 - 22.5 - 315
         ):
         direction = "NE "
         if not compute_args().nocolor:
             direction=direction+FLECHE_NE
-    return ""
+    return direction
 
 
 def traduction(current_weather_code,jour):
     if (
         current_weather_code == 0
         or current_weather_code == 1
         or current_weather_code == 2
@@ -664,25 +664,23 @@
         if (ville is None or ville == "") and (dpt is None or dpt == ""):
             print_debug("pas de data pour ville/dpt/cp")
         elif dpt is None or dpt == "":
             data.append([ville])
         else:    
             data.append([ville + " (" + dpt + ")"])
         data.append([f"lat.:  {float(lat):.4f}° / long.: {float(long):.4f}° / alt.: {float(alt):.0f}m "])
-        #data.append([datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")])
         data.append([recap])
     else:
         if (ville is None or ville == "") and (dpt is None or dpt == ""):
             print_debug("pas de data pour ville/dpt/cp")
         elif dpt is None or dpt == "":
             data.append([HOME, ville])
         else:    
             data.append([HOME, ville + " (" + dpt + ")"])
         data.append([BOUSSOLE, f"lat.:  {float(lat):.4f}°  / long.: {float(long):.4f}° / alt.: {float(alt):.0f}m "])
-        #data.append([CLOCK, datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")])
         data.append([PC,recap])
     if compute_args().condensate:
         table = columnar.columnar(data, no_borders=True, wrap_max=0)
     else:
         table = columnar.columnar(data, no_borders=False, wrap_max=0)
 
     print(table)
@@ -719,25 +717,22 @@
             "recherche de la localisation depuis https://geolocation-db.com/json"
         )
         resultat= url.read().decode()
         print_debug(resultat)
         data = json.loads(resultat)
         print_debug(str(json.dumps(data, indent=4,ensure_ascii=False)))
         ville = data["city"]
-        if ville ==None:
+        if ville is None:
             ville=""
         lat = str(data["latitude"])
         long = str(data["longitude"])
         dpt = str(data["state"])
-        if dpt ==None:
+        if dpt is None:
             dpt=""
         country = str(data["country_name"])
-        #if country==None or country!="France":
-        #    print(my_colored("erreur : aucune ville trouvée. Si vous souhaitez rechercher une ville hors de France, ajoutez --world", "red"))
-        #    exit(1)
         return ville, dpt, lat, long, country
 
 
 
 
 def obtain_city_data_from_gps():
     print_debug(
@@ -748,120 +743,100 @@
         + str(compute_args().gps[1])
     )
     geolocator = geopy.geocoders.Nominatim(user_agent="my_geocoder")
     if compute_args().lang:
         location = geolocator.reverse(compute_args().gps[0] +", " + compute_args().gps[1],addressdetails=True)
     else:        
         location = geolocator.reverse(compute_args().gps[0] +", " + compute_args().gps[1],addressdetails=True,language="fr")
-    if location == None:
+    if location is None:
         print(my_colored("erreur : aucune ville trouvée.", "red"))
         exit(1)
     ville = None
-    if ville == None or (location.raw.get("address").get("village") != None):
+    if ville is None or (location.raw.get("address").get("village") is not None):
         ville = location.raw.get("address").get("village")
-    if ville == None or (location.raw.get("address").get("municipality") != None):
+    if ville is None or (location.raw.get("address").get("municipality") is not None):
         ville = location.raw.get("address").get("municipality")
-    if ville == None or (location.raw.get("address").get("town") != None):
+    if ville is None or (location.raw.get("address").get("town") is not None):
         ville = location.raw.get("address").get("town")               
-    if ville == None or (location.raw.get("address").get("city") != None):
+    if ville is None or (location.raw.get("address").get("city") is not None):
         ville = location.raw.get("address").get("city")        
     dpt = location.raw.get("address").get("county")
-    if dpt ==None:
+    if dpt is None:
         dpt=location.raw.get("address").get("state")
-    if dpt ==None:
+    if dpt is None:
         dpt= location.raw.get("address").get("postcode") 
-    if dpt ==None or location.raw.get("address").get("country")!="France":
+    if dpt is None or location.raw.get("address").get("country")!="France":
         dpt= location.raw.get("address").get("country")              
     cp = location.raw.get("address").get("postcode")
     country=location.raw.get("address").get("country") 
-    #if country!="France" and compute_args().world == False:
-    #    print(my_colored("erreur : aucune ville trouvée. Si vous souhaitez rechercher une ville hors de France, ajoutez --world", "red"))
-    #    exit(1)    
-    if cp == None:
+    if cp is None:
         cp = ""
     lat = location.raw.get("lat")
     long = location.raw.get("lon")
     print_debug(ville+"-"+dpt+"-"+lat+"-"+long+"-"+country)
 
 
     return ville, dpt, lat, long, country
 
 
 def obtain_city_data():
 
     town = compute_args().town
     ctx = ssl.create_default_context(cafile=certifi.where())
     geopy.geocoders.options.default_ssl_context = ctx
-    
-    # Création d'un objet géocodeur Nominatim
     geolocator = geopy.geocoders.Nominatim(user_agent="my_geocoder")
-    
-    # Géocodage d'une adresse
-    #if compute_args().world:
-    #    locations = geolocator.geocode(town,exactly_one=False,addressdetails=True,language="fr")
-    #else:
-    #    locations = geolocator.geocode(town + ", France",exactly_one=False,addressdetails=True,language="fr")
     if compute_args().lang:
         locations = geolocator.geocode(town,exactly_one=False,addressdetails=True)
     else:
         locations = geolocator.geocode(town,exactly_one=False,addressdetails=True,language="fr")    
-    # Affichage des informations de localisation
     choix = []
-    if locations == None:
-        #if not compute_args().world:
-        #    print(my_colored("erreur : aucune ville trouvée. Si vous souhaitez rechercher une ville hors de France, ajoutez --world", "red"))
-        #else:
-        #    print(my_colored("erreur : aucune ville trouvée", "red"))
+    if locations is None:
         print(my_colored("erreur : aucune ville trouvée", "red"))
         exit(1)  
     for location in locations:
         print_debug(json.dumps(location.raw, indent=4,ensure_ascii=False))
         if ((location.raw.get("addresstype")=="postcode" and location.raw.get("address").get("country")=="France") or location.raw.get("addresstype")=="town" or location.raw.get("addresstype")=="city" or location.raw.get("addresstype")=="municipality" or location.raw.get("addresstype")=="village"):
             
             ville = None
-            if ville == None or (location.raw.get("address").get("village") != None and (clean_string(location.raw.get("address").get("village").lower())==clean_string(town.lower()))):# or (compute_args().world and location.raw.get("address").get("country")!="France"))):
+            if ville is None or (location.raw.get("address").get("village") is not None and (clean_string(location.raw.get("address").get("village").lower())==clean_string(town.lower()))):
                 ville = location.raw.get("address").get("village")
-            if ville == None or (location.raw.get("address").get("municipality") != None and (clean_string(location.raw.get("address").get("municipality").lower())==clean_string(town.lower()))):# or (compute_args().world and location.raw.get("address").get("country")!="France"))):
+            if ville is None or (location.raw.get("address").get("municipality") is not None and (clean_string(location.raw.get("address").get("municipality").lower())==clean_string(town.lower()))):
                 ville = location.raw.get("address").get("municipality")
-            if ville == None or (location.raw.get("address").get("town") != None and (clean_string(location.raw.get("address").get("town").lower())==clean_string(town.lower()))):# or (compute_args().world and location.raw.get("address").get("country")!="France"))):
+            if ville is None or (location.raw.get("address").get("town") is not None and (clean_string(location.raw.get("address").get("town").lower())==clean_string(town.lower()))):
                 ville = location.raw.get("address").get("town")               
-            if ville == None or (location.raw.get("address").get("city") != None and (clean_string(location.raw.get("address").get("city").lower())==clean_string(town.lower()))):# or (compute_args().world and location.raw.get("address").get("country")!="France"))):
+            if ville is None or (location.raw.get("address").get("city") is not None and (clean_string(location.raw.get("address").get("city").lower())==clean_string(town.lower()))):
                 ville = location.raw.get("address").get("city")        
             dpt = location.raw.get("address").get("county")
-            if dpt ==None:
+            if dpt is None:
                 dpt=location.raw.get("address").get("state")
-            if dpt ==None:
+            if dpt is None:
                 dpt= location.raw.get("address").get("postcode") 
-            if dpt ==None or location.raw.get("address").get("country")!="France":
+            if dpt is None or location.raw.get("address").get("country")!="France":
                 dpt= location.raw.get("address").get("country")
 
             country = location.raw.get("address").get("country")
             if country == "France":
                 cp = location.raw.get("address").get("postcode")
             else:
                 cp = ""
             lat = location.raw.get("lat")
             long = location.raw.get("lon")
             print_debug(ville+"-"+dpt+"-"+lat+"-"+long+"-"+country)
-            if (clean_string(ville.lower()) == clean_string(town.lower()) or cp.lower() == town.lower()):# or (compute_args().world and location.raw.get("address").get("country")!="France")): 
-                if ville+"-"+dpt not in [item[0] for item in choix]:  # Vérifier si ville+"-"+dpt n'est pas déjà présent dans choix
+            if (clean_string(ville.lower()) == clean_string(town.lower()) or cp.lower() == town.lower()):
+                if ville+"-"+dpt not in [item[0] for item in choix]:  
                     choix.append([ville+"-"+dpt, ville, dpt, country,lat, long])
     if len(choix)==1:
         choice = choix[0]
         ville = choice[1]
         dpt = choice[2]
         country = choice[3]
         lat = choice[4]
         long = choice[5]
         return ville, dpt, lat, long, country    
     if len(choix)==0:
-        #if not compute_args().world:
-        #    print(my_colored("erreur : aucune ville trouvée. Si vous souhaitez rechercher une ville hors de France, ajoutez --world", "red"))
-        #else:
-        #    print(my_colored("erreur : aucune ville trouvée", "red"))
         print(my_colored("erreur : aucune ville trouvée", "red"))
         exit(1)
     while True:    
         i=0    
         for choice in choix:
             i=i+1
             print("["+str(i)+"] " + choice[1] + " (" + choice[2]+ ")")
```

### Comparing `pyweatherfr-5.1.2/pyweatherfr.egg-info/PKG-INFO` & `pyweatherfr-5.1.3/pyweatherfr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 5.1.2
+Version: 5.1.3
 Summary: pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-5.1.2/setup.py` & `pyweatherfr-5.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="pyweatherfr",
-    version="5.1.2",
+    version="5.1.3",
     description="pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)",
     long_description="The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme",
     url="https://github.com/thib1984/pyweatherfr",
     author="thib1984",
     author_email="thibault.garcon@gmail.com",
     license="MIT",
     packages=["pyweatherfr"],
```

