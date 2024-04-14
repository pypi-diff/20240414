# Comparing `tmp/pyweatherfr-5.0.0.tar.gz` & `tmp/pyweatherfr-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweatherfr-5.0.0.tar", last modified: Sat Apr 13 16:49:16 2024, max compression
+gzip compressed data, was "pyweatherfr-5.0.2.tar", last modified: Sat Apr 13 20:10:38 2024, max compression
```

## Comparing `pyweatherfr-5.0.0.tar` & `pyweatherfr-5.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:49:16.579111 pyweatherfr-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-13 16:48:41.000000 pyweatherfr-5.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-13 16:49:16.579111 pyweatherfr-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-13 16:48:41.000000 pyweatherfr-5.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-13 16:48:41.000000 pyweatherfr-5.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:49:16.575111 pyweatherfr-5.0.0/pyweatherfr/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-13 16:48:41.000000 pyweatherfr-5.0.0/pyweatherfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-13 16:48:41.000000 pyweatherfr-5.0.0/pyweatherfr/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    37788 2024-04-13 16:48:41.000000 pyweatherfr-5.0.0/pyweatherfr/pyweatherfr.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-13 16:48:41.000000 pyweatherfr-5.0.0/pyweatherfr/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:49:16.579111 pyweatherfr-5.0.0/pyweatherfr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-13 16:49:16.000000 pyweatherfr-5.0.0/pyweatherfr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-13 16:49:16.000000 pyweatherfr-5.0.0/pyweatherfr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 16:49:16.000000 pyweatherfr-5.0.0/pyweatherfr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-13 16:49:16.000000 pyweatherfr-5.0.0/pyweatherfr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 16:48:46.000000 pyweatherfr-5.0.0/pyweatherfr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-13 16:49:16.000000 pyweatherfr-5.0.0/pyweatherfr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 16:49:16.000000 pyweatherfr-5.0.0/pyweatherfr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 16:49:16.579111 pyweatherfr-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-13 16:48:41.000000 pyweatherfr-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 20:10:38.696352 pyweatherfr-5.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-13 20:10:02.000000 pyweatherfr-5.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-13 20:10:38.696352 pyweatherfr-5.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-13 20:10:02.000000 pyweatherfr-5.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-13 20:10:02.000000 pyweatherfr-5.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 20:10:38.696352 pyweatherfr-5.0.2/pyweatherfr/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-13 20:10:02.000000 pyweatherfr-5.0.2/pyweatherfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-13 20:10:02.000000 pyweatherfr-5.0.2/pyweatherfr/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40595 2024-04-13 20:10:02.000000 pyweatherfr-5.0.2/pyweatherfr/pyweatherfr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-13 20:10:02.000000 pyweatherfr-5.0.2/pyweatherfr/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 20:10:38.696352 pyweatherfr-5.0.2/pyweatherfr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-13 20:10:38.000000 pyweatherfr-5.0.2/pyweatherfr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-13 20:10:38.000000 pyweatherfr-5.0.2/pyweatherfr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 20:10:38.000000 pyweatherfr-5.0.2/pyweatherfr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-13 20:10:38.000000 pyweatherfr-5.0.2/pyweatherfr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 20:10:06.000000 pyweatherfr-5.0.2/pyweatherfr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-13 20:10:38.000000 pyweatherfr-5.0.2/pyweatherfr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 20:10:38.000000 pyweatherfr-5.0.2/pyweatherfr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 20:10:38.696352 pyweatherfr-5.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-13 20:10:02.000000 pyweatherfr-5.0.2/setup.py
```

### Comparing `pyweatherfr-5.0.0/LICENSE.txt` & `pyweatherfr-5.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.0.0/PKG-INFO` & `pyweatherfr-5.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 5.0.0
+Version: 5.0.2
 Summary: pyweatherfr displays weather forecast for a given town in France
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-5.0.0/README.md` & `pyweatherfr-5.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.0.0/pyweatherfr/args.py` & `pyweatherfr-5.0.2/pyweatherfr/args.py`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.0.0/pyweatherfr/pyweatherfr.py` & `pyweatherfr-5.0.2/pyweatherfr/pyweatherfr.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,34 +117,36 @@
         return True
     except ValueError:
         return False
 
 def find():
 
     if compute_args().town:
-        ville, dpt, lat, long = obtain_city_data()
+        ville, dpt, lat, long,country = obtain_city_data()
     elif compute_args().gps:
-        ville, dpt, lat, long = obtain_city_data_from_gps()
+        ville, dpt, lat, long,country = obtain_city_data_from_gps()
     else:
-        ville, dpt, lat, long = obtain_city_data_from_ip()
+        ville, dpt, lat, long,country = obtain_city_data_from_ip()
     tz=timezonefinder.TimezoneFinder().timezone_at(lng=float(long), lat=float(lat))
     if compute_args().pc:
         tz=str(tzlocal.get_localzone())
     if compute_args().utc:
         tz=str(pytz.utc)              
     print_debug(tz)
     if compute_args().now:
         previsions_courantes(ville, dpt, lat, long,tz)
     elif not compute_args().date == None:
         previsions_detaillees(ville, dpt, lat, long,tz)        
     elif diff_jour(long,lat) == 1000:
         previsions_generiques(ville, dpt, lat, long,tz)
     else:
         previsions_detaillees(ville, dpt, lat, long,tz)
-
+    if country ==None or country!="France":
+        print(my_colored("warning : ville potentiellement hors de France, les prévisions et données peuvent être moins détailées", "yellow"))
+    
 
 
 def previsions_detaillees(ville, dpt, lat, long, tz):
 
 
     
     (
@@ -685,103 +687,150 @@
         )
         data = json.loads(url.read().decode())
         print_debug(str(json.dumps(data, indent=4,ensure_ascii=False)))
         ville = data["city"]
         lat = str(data["latitude"])
         long = str(data["longitude"])
         dpt = str(data["state"])
-        return ville, dpt, lat, long 
+        country = str(data["country_name"])
+        if country!="France" and compute_args().world == False:
+            print(my_colored("erreur : aucune ville trouvée. Si vous souhaitez rechercher une ville hors de France, ajoutez --world", "red"))
+            exit(1)
+        return ville, dpt, lat, long, country
 
 
 
 
 def obtain_city_data_from_gps():
     print_debug(
         "COORDONNEES_GPS :"
         + "latitude="
         + str(compute_args().gps[0])
         + " longitude="
         + str(compute_args().gps[1])
     )
-    return "", "", str(compute_args().gps[0]), str(compute_args().gps[1])
+    geolocator = geopy.geocoders.Nominatim(user_agent="my_geocoder")
+    location = geolocator.reverse(compute_args().gps[0] +", " + compute_args().gps[1],addressdetails=True,language="fr")
+    if location == None:
+        print(my_colored("erreur : aucune ville trouvée.", "red"))
+        exit(1)
+    ville = None
+    if ville == None or (location.raw.get("address").get("village") != None):
+        ville = location.raw.get("address").get("village")
+    if ville == None or (location.raw.get("address").get("municipality") != None):
+        ville = location.raw.get("address").get("municipality")
+    if ville == None or (location.raw.get("address").get("town") != None):
+        ville = location.raw.get("address").get("town")               
+    if ville == None or (location.raw.get("address").get("city") != None):
+        ville = location.raw.get("address").get("city")        
+    dpt = location.raw.get("address").get("county")
+    if dpt ==None:
+        dpt=location.raw.get("address").get("state")
+    if dpt ==None:
+        dpt= location.raw.get("address").get("postcode") 
+    if dpt ==None or location.raw.get("address").get("country")!="France":
+        dpt= location.raw.get("address").get("country")              
+    cp = location.raw.get("address").get("postcode")
+    country=location.raw.get("address").get("country") 
+    if country!="France" and compute_args().world == False:
+        print(my_colored("erreur : aucune ville trouvée. Si vous souhaitez rechercher une ville hors de France, ajoutez --world", "red"))
+        exit(1)    
+    if cp == None:
+        cp = ""
+    lat = location.raw.get("lat")
+    long = location.raw.get("lon")
+    print_debug(ville+"-"+dpt+"-"+lat+"-"+long+"-"+country)
+
+
+    return ville, dpt, lat, long, country
 
 
 def obtain_city_data():
 
     town = compute_args().town
     ctx = ssl.create_default_context(cafile=certifi.where())
     geopy.geocoders.options.default_ssl_context = ctx
     
     # Création d'un objet géocodeur Nominatim
     geolocator = geopy.geocoders.Nominatim(user_agent="my_geocoder")
     
     # Géocodage d'une adresse
     if compute_args().world:
-        locations = geolocator.geocode(town,exactly_one=False,addressdetails=True)
+        locations = geolocator.geocode(town,exactly_one=False,addressdetails=True,language="fr")
     else:
-        locations = geolocator.geocode(town + ", France",exactly_one=False,addressdetails=True)
+        locations = geolocator.geocode(town + ", France",exactly_one=False,addressdetails=True,language="fr")
     
     # Affichage des informations de localisation
     choix = []
     if locations == None:
-        print(my_colored("erreur : aucune ville trouvée", "red")) 
-        exit(1)    
+        if not compute_args().world:
+            print(my_colored("erreur : aucune ville trouvée. Si vous souhaitez rechercher une ville hors de France, ajoutez --world", "red"))
+        else:
+            print(my_colored("erreur : aucune ville trouvée", "red"))
+        exit(1)  
     for location in locations:
+        print_debug(json.dumps(location.raw, indent=4,ensure_ascii=False))
         if (location.raw.get("addresstype")=="postcode" or location.raw.get("addresstype")=="town" or location.raw.get("addresstype")=="city" or location.raw.get("addresstype")=="municipality" or location.raw.get("addresstype")=="village"):
-            print_debug(json.dumps(location.raw, indent=4,ensure_ascii=False))
+            
             ville = None
             if ville == None or (location.raw.get("address").get("village") != None and (clean_string(location.raw.get("address").get("village").lower())==clean_string(town.lower()) or (compute_args().world and location.raw.get("address").get("country")!="France"))):
                 ville = location.raw.get("address").get("village")
             if ville == None or (location.raw.get("address").get("municipality") != None and (clean_string(location.raw.get("address").get("municipality").lower())==clean_string(town.lower()) or (compute_args().world and location.raw.get("address").get("country")!="France"))):
                 ville = location.raw.get("address").get("municipality")
             if ville == None or (location.raw.get("address").get("town") != None and (clean_string(location.raw.get("address").get("town").lower())==clean_string(town.lower()) or (compute_args().world and location.raw.get("address").get("country")!="France"))):
                 ville = location.raw.get("address").get("town")               
             if ville == None or (location.raw.get("address").get("city") != None and (clean_string(location.raw.get("address").get("city").lower())==clean_string(town.lower()) or (compute_args().world and location.raw.get("address").get("country")!="France"))):
                 ville = location.raw.get("address").get("city")        
             dpt = location.raw.get("address").get("county")
             if dpt ==None:
                 dpt=location.raw.get("address").get("state")
             if dpt ==None:
                 dpt= location.raw.get("address").get("postcode") 
-            if dpt ==None or compute_args().world:
+            if dpt ==None or location.raw.get("address").get("country")!="France":
                 dpt= location.raw.get("address").get("country")              
             cp = location.raw.get("address").get("postcode")
+            country = location.raw.get("address").get("country")
             if cp == None:
                 cp = ""
             lat = location.raw.get("lat")
             long = location.raw.get("lon")
-            print_debug(ville+"-"+dpt+"-"+lat+"-"+long)
+            print_debug(ville+"-"+dpt+"-"+lat+"-"+long+"-"+country)
             if (clean_string(ville.lower()) == clean_string(town.lower()) or cp.lower() == town.lower() or (compute_args().world and location.raw.get("address").get("country")!="France")): 
                 if ville+"-"+dpt not in [item[0] for item in choix]:  # Vérifier si ville+"-"+dpt n'est pas déjà présent dans choix
-                    choix.append([ville+"-"+dpt, ville, dpt, lat, long])
+                    choix.append([ville+"-"+dpt, ville, dpt, country,lat, long])
     if len(choix)==1:
         choice = choix[0]
         ville = choice[1]
         dpt = choice[2]
-        lat = choice[3]
-        long = choice[4]
-        return ville, dpt, lat, long    
+        country = choice[3]
+        lat = choice[4]
+        long = choice[5]
+        return ville, dpt, lat, long, country    
     if len(choix)==0:
-        print(my_colored("erreur : aucune ville trouvée", "red")) 
+        if not compute_args().world:
+            print(my_colored("erreur : aucune ville trouvée. Si vous souhaitez rechercher une ville hors de France, ajoutez --world", "red"))
+        else:
+            print(my_colored("erreur : aucune ville trouvée", "red"))
         exit(1)
     while True:    
         i=0    
         for choice in choix:
             i=i+1
             print("["+str(i)+"] " + choice[1] + " (" + choice[2]+ ")")
         toto = input("Quelle ville? ")
         if toto.isnumeric() and 1 <= int(toto) <= len(choix):
             break
         print(my_colored("erreur : choix incorrect", "red"))       
     choice = choix[int(toto)-1]
     ville = choice[1]
     dpt = choice[2]
-    lat = choice[3]
-    long = choice[4]
-    return ville, dpt, lat, long
+    country = choice[3]
+    lat = choice[4]
+    long = choice[5]
+    return ville, dpt, lat, long, country
 
 
 def my_colored(message, color):
     if compute_args().nocolor:
         return message
     return termcolor.colored(message, color)
```

### Comparing `pyweatherfr-5.0.0/pyweatherfr.egg-info/PKG-INFO` & `pyweatherfr-5.0.2/pyweatherfr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 5.0.0
+Version: 5.0.2
 Summary: pyweatherfr displays weather forecast for a given town in France
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-5.0.0/setup.py` & `pyweatherfr-5.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="pyweatherfr",
-    version="5.0.0",
+    version="5.0.2",
     description="pyweatherfr displays weather forecast for a given town in France",
     long_description="The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme",
     url="https://github.com/thib1984/pyweatherfr",
     author="thib1984",
     author_email="thibault.garcon@gmail.com",
     license="MIT",
     packages=["pyweatherfr"],
```

