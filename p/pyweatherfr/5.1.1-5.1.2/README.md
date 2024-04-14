# Comparing `tmp/pyweatherfr-5.1.1.tar.gz` & `tmp/pyweatherfr-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweatherfr-5.1.1.tar", last modified: Sun Apr 14 08:22:31 2024, max compression
+gzip compressed data, was "pyweatherfr-5.1.2.tar", last modified: Sun Apr 14 11:22:20 2024, max compression
```

## Comparing `pyweatherfr-5.1.1.tar` & `pyweatherfr-5.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:22:31.887678 pyweatherfr-5.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-14 08:21:41.000000 pyweatherfr-5.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-14 08:22:31.887678 pyweatherfr-5.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-14 08:21:41.000000 pyweatherfr-5.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-14 08:21:41.000000 pyweatherfr-5.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:22:31.883678 pyweatherfr-5.1.1/pyweatherfr/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-14 08:21:41.000000 pyweatherfr-5.1.1/pyweatherfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-04-14 08:21:41.000000 pyweatherfr-5.1.1/pyweatherfr/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    42195 2024-04-14 08:21:41.000000 pyweatherfr-5.1.1/pyweatherfr/pyweatherfr.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-14 08:21:41.000000 pyweatherfr-5.1.1/pyweatherfr/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:22:31.887678 pyweatherfr-5.1.1/pyweatherfr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-14 08:22:31.000000 pyweatherfr-5.1.1/pyweatherfr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-14 08:22:31.000000 pyweatherfr-5.1.1/pyweatherfr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 08:22:31.000000 pyweatherfr-5.1.1/pyweatherfr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-14 08:22:31.000000 pyweatherfr-5.1.1/pyweatherfr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 08:21:53.000000 pyweatherfr-5.1.1/pyweatherfr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-14 08:22:31.000000 pyweatherfr-5.1.1/pyweatherfr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-14 08:22:31.000000 pyweatherfr-5.1.1/pyweatherfr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 08:22:31.887678 pyweatherfr-5.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-14 08:21:41.000000 pyweatherfr-5.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:22:20.384011 pyweatherfr-5.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-14 11:21:37.000000 pyweatherfr-5.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-14 11:22:20.384011 pyweatherfr-5.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-14 11:21:37.000000 pyweatherfr-5.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-14 11:21:37.000000 pyweatherfr-5.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:22:20.384011 pyweatherfr-5.1.2/pyweatherfr/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-14 11:21:37.000000 pyweatherfr-5.1.2/pyweatherfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-04-14 11:21:37.000000 pyweatherfr-5.1.2/pyweatherfr/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43357 2024-04-14 11:21:37.000000 pyweatherfr-5.1.2/pyweatherfr/pyweatherfr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-14 11:21:37.000000 pyweatherfr-5.1.2/pyweatherfr/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:22:20.384011 pyweatherfr-5.1.2/pyweatherfr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-14 11:22:20.000000 pyweatherfr-5.1.2/pyweatherfr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-14 11:22:20.000000 pyweatherfr-5.1.2/pyweatherfr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 11:22:20.000000 pyweatherfr-5.1.2/pyweatherfr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-14 11:22:20.000000 pyweatherfr-5.1.2/pyweatherfr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 11:21:46.000000 pyweatherfr-5.1.2/pyweatherfr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-14 11:22:20.000000 pyweatherfr-5.1.2/pyweatherfr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-14 11:22:20.000000 pyweatherfr-5.1.2/pyweatherfr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 11:22:20.384011 pyweatherfr-5.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-14 11:21:37.000000 pyweatherfr-5.1.2/setup.py
```

### Comparing `pyweatherfr-5.1.1/LICENSE.txt` & `pyweatherfr-5.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.1.1/PKG-INFO` & `pyweatherfr-5.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 5.1.1
+Version: 5.1.2
 Summary: pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-5.1.1/README.md` & `pyweatherfr-5.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.1.1/pyweatherfr/args.py` & `pyweatherfr-5.1.2/pyweatherfr/args.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,21 @@
 pygitscrum argparse gestion
 """
 
 import argparse
 import sys
 
 
+# Fonction de validation pour s'assurer que l'argument est un nombre positif
+def positive_integer(value):
+    ivalue = int(value)
+    if ivalue <= 0:
+        raise argparse.ArgumentTypeError("%s n'est pas un nombre entier strictement positif" % value)
+    return ivalue
+
 class CustomHelpFormatter(argparse.HelpFormatter):
     def _format_action_invocation(self, action):
         if not action.option_strings or action.nargs == 0:
             return super()._format_action_invocation(action)
         default = self._get_default_metavar_for_optional(action)
         args_string = self._format_args(action, default)
         return ", ".join(action.option_strings) + " " + args_string
@@ -56,18 +63,16 @@
     )
     my_2group.add_argument(
         "-j",
         "--jour",
         metavar="JOUR",
         action="store",
         type=int,
-        default=1000,
         nargs='?',
         const=0,        
-        choices=range(-101, 4),
         help="affichage des données météo détaillées pour [JOUR] (0 pour le jour actuel, 1 pour le J+1, ..., -1 pour J-1, ...) plutôt que les données génériques",
     )
     my_2group.add_argument(
         "-d",
         "--date",
         metavar="DATE",
         action="store",
@@ -75,18 +80,17 @@
         help="affichage des données météo détaillées pour [DAY] au format yyyy-mm-dd, plutôt que les données génériques",
     )    
     my_2group.add_argument(
         "-p",
         "--past",
         metavar="JOUR PASSE",
         action="store",
-        type=int,
+        type=positive_integer,
         default=0,
-        choices=range(1, 101),
-        help="affichage des données météo génériques depuis [JOUR PASSE] (10 pour J-10 à J-1, ...), compris entre 1 et 100, plutôt que les données génériques",
+        help="affichage des données météo génériques depuis [JOUR PASSE] (10 pour J-10 à J-1, ...), plutôt que les données génériques",
     )         
     my_group.add_argument(
         "-g",
         "--gps",
         metavar=("LATITUDE", "LONGITUDE"),
         action="store",
         nargs=2,
```

### Comparing `pyweatherfr-5.1.1/pyweatherfr/pyweatherfr.py` & `pyweatherfr-5.1.2/pyweatherfr/pyweatherfr.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import termcolor
 import pathlib
 import retry_requests
 import geopy
 import timezonefinder
 import pytz
 import tzlocal
+import numpy
 
 
 DOSSIER_CONFIG_PYWEATHER = "pyweatherfr"
 
 SUN = "\U0001F31E"
 MI_SUN = "\U0001F324"
 CLOUD = "\U0001F325"
@@ -57,22 +58,23 @@
 FLECHE_S = "\U00002B06"
 FLECHE_SE = "\U00002196"
 FLECHE_E = "\U00002B05"
 FLECHE_NE = "\U00002199"
 ELEPHANT = "\U0001F418"
 PLUME = "\U0001FAB6"
 PC ="\U0001f4bb"
+LUNETTES= "\U0001F60E"
 WARNING_WARM=30
 WARNING_FROID=0
 WARNING_SNOW=0.1
 WARNING_RAIN=0.1
 WARNING_WIND=30
 WARNING_WIND_GUST=50
 WARNING_HP=1030
-WARNING_BP=990
+WARNING_BP=995
 WARNING_HUMIDITY=90
 
 def get_user_config_directory_pyweather():
     if os.name == "nt":
         appdata = os.getenv("LOCALAPPDATA")
         if appdata:
             ze_path = os.path.join(appdata, DOSSIER_CONFIG_PYWEATHER, "")
@@ -101,16 +103,16 @@
     tz=timezonefinder.TimezoneFinder().timezone_at(lng=float(long), lat=float(lat))
     if not compute_args().date == None:
         if not est_format_date(compute_args().date):
             print(my_colored("erreur : format date invalide, format attendu yyyy-mm-dd", "red"))
             exit(1)
         diff = (pytz.timezone(tz).localize(datetime.datetime.strptime(compute_args().date, "%Y-%m-%d")) - datetime.datetime.now(tz=pytz.timezone(tz))).days +1
         print_debug(str(diff) + " jours")
-        if diff>=4 or diff<-100:
-            print(my_colored("erreur : date invalide (-100 à +4 jour de la date actuelle)", "red"))
+        if diff>=15:
+            print(my_colored("erreur : date invalide (limitée à +15 jour de la date actuelle)", "red"))
             exit(1)
         return diff     
     return compute_args().jour
 
 def est_format_date(chaine):
     try:
         datetime.datetime.strptime(chaine, '%Y-%m-%d')
@@ -132,23 +134,24 @@
     if compute_args().utc:
         tz=str(pytz.utc)              
     print_debug(tz)
     if compute_args().now:
         previsions_courantes(ville, dpt, lat, long,tz)
     elif not compute_args().date == None:
         previsions_detaillees(ville, dpt, lat, long,tz)        
-    elif diff_jour(long,lat) == 1000:
+    elif compute_args().jour is None:
         previsions_generiques(ville, dpt, lat, long,tz)
     else:
         previsions_detaillees(ville, dpt, lat, long,tz)
+    if not compute_args().town and not compute_args().gps:   
+        print(my_colored("warning : si vous utilisez un proxy ou un VPN, la localisation peut être incorrecte", "yellow"))
     if country ==None:
         print(my_colored("warning : ville potentiellement hors de France, les prévisions et données peuvent être moins précises", "yellow"))
     elif  country!="France":
         print(my_colored("warning : ville hors de France, les prévisions et données peuvent être moins précises", "yellow"))
-   
 
 
 def previsions_detaillees(ville, dpt, lat, long, tz):
 
 
     
     (
@@ -178,14 +181,17 @@
     if diff_jour(long,lat)<0:
         recap ="Données détaillées pour le " + (datetime.datetime.now(tz=pytz.timezone(tz)) + datetime.timedelta(days=diff_jour(long,lat))).strftime(
                 "%Y-%m-%d")        
     print_generic_data_town(ville, dpt, lat, long, alt, recap)
     data = []
     new_var = diff_jour(long,lat)
     for h in range(0, 24):
+        if numpy.isnan(hourly_temperature_2m[h]):
+            print(my_colored("warning : pas de données pour ce jour", "yellow"))
+            exit(1)
         warning = ""
         if (
             (datetime.datetime.now(tz=pytz.timezone(tz)) + datetime.timedelta(days=new_var)).strftime(
             "%Y-%m-%d") == datetime.datetime.now(tz=pytz.timezone(tz)).strftime("%Y-%m-%d")
             and 0 < h - int(datetime.datetime.now(tz=pytz.timezone(tz)).strftime("%H")) <= 1
         ):
             warning = warning + " " + CLOCK
@@ -215,15 +221,17 @@
         if surface_pressure[h] >= WARNING_HP:
             warning = warning + " " + ELEPHANT
         if surface_pressure[h] <= WARNING_BP:
             warning = warning + " " + PLUME
         weather, emojiweather = traduction(current_weather_code[h],isday[h])
         humidity = f"{relative_humidity_2m[h]:.0f}%"
         duree_soleil = f"{sunshine_duration[h]/60:.0f}'"
-        rayonnement = f" {shortwave_radiation[h]:.0f}W/m"        
+        rayonnement = f" {shortwave_radiation[h]:.0f}W/m\u00B2" 
+        if shortwave_radiation[h]>1000:
+            warning = warning + " " + LUNETTES   
         if compute_args().nocolor:
             data.append(
                 [
                     datetime.datetime.strftime(
                         datetime.datetime.now(tz=pytz.timezone(tz)).replace(
                             hour=0, minute=0, second=0, microsecond=0
                         )
@@ -351,15 +359,15 @@
     if (
             direction_vent_degres <= 360 - 22.5 - 270
             and direction_vent_degres > 360 - 22.5 - 315
         ):
         direction = "NE "
         if not compute_args().nocolor:
             direction=direction+FLECHE_NE
-    return direction
+    return ""
 
 
 def traduction(current_weather_code,jour):
     if (
         current_weather_code == 0
         or current_weather_code == 1
         or current_weather_code == 2
@@ -383,15 +391,15 @@
         return ["bruine", RAIN]
     if current_weather_code >= 60 and current_weather_code <= 69:
         return ["pluie", RAIN]
     if current_weather_code >= 70 and current_weather_code <= 79:
         return ["neige", SNOW]
     if current_weather_code >= 80 and current_weather_code <= 99:
         return ["averse / orage", ORAGE_PLUIE]
-
+    return ["", ""]
 
 def previsions_courantes(ville, dpt, lat, long, tz):
     
 
     (
         current_temperature_2m,
         current_apparent_temperature,
@@ -434,15 +442,15 @@
         data.append(
             [
                 "vent",
                 f"{current_wind_speed_10m:.1f}km/h ({current_wind_gusts_10m:.1f}km/h) - "
                 + direction,
             ]
         )
-        data.append(["rayonnement", f"{w_soleil:.0f}W/m"])
+        data.append(["rayonnement", f"{w_soleil:.0f}W/m\u00B2"])
         data.append(["temps", current_weather])
 
     else:
         if current_temperature_2m >= WARNING_WARM or current_apparent_temperature >= WARNING_WARM:
             data.append(
                 [
                     "température (ressentie)",
@@ -488,15 +496,18 @@
                 [
                     "vent",
                     f"{current_wind_speed_10m:.1f}km/h ({current_wind_gusts_10m:.1f}km/h) - "
                     + direction,
                     "",
                 ]
             )
-        data.append(["rayonnement", f"{w_soleil:.0f}W/m",""])    
+        if w_soleil>1000:
+            data.append(["rayonnement", f"{w_soleil:.0f}W/m\u00B2",LUNETTES]) 
+        else:      
+            data.append(["rayonnement", f"{w_soleil:.0f}W/m\u00B2",""]) 
         data.append(["temps", emojiweather + " " + current_weather, ""])
     if compute_args().condensate:
         table = columnar.columnar(data, no_borders=True, wrap_max=0)
     else:
         print("")
         table = columnar.columnar(data, no_borders=False, wrap_max=0)
     print(table)
@@ -533,117 +544,121 @@
     else:
         recap = recap + " (loc.)"  
     print_generic_data_town(ville, dpt, lat, long, alt, recap)
     data = []
     fin = 3
     if compute_args().past!=0:
         fin=-1
+    tronque=False    
     for i in range(0,len(daily_precipitation_sum)):
-        warning = ""
-        pluie = f"{daily_precipitation_sum[i]:.1f}mm"
-        if snowfall[i] >= WARNING_SNOW:
-            warning = warning + " " + SNOW
-        elif daily_precipitation_sum[i] >= WARNING_RAIN:
-            warning = warning + " " + RAIN
-        temp = f"{daily_temperature_2m_min[i]:.1f}°C ({daily_apparent_temperature_min[i]:.1f}°C) -> {daily_temperature_2m_max[i]:.1f}°C ({daily_apparent_temperature_max[i]:.1f}°C)"
-        if (
-            daily_temperature_2m_min[i] <= WARNING_FROID
-            or daily_apparent_temperature_min[i] <= WARNING_FROID
-            or daily_temperature_2m_max[i] <= WARNING_FROID
-            or daily_apparent_temperature_max[i] <= WARNING_FROID
-        ):
-            warning = warning + " " + COLD
-        if (
-            daily_temperature_2m_min[i] >= WARNING_WARM
-            or daily_apparent_temperature_min[i] >= WARNING_WARM
-            or daily_temperature_2m_max[i] >= WARNING_WARM
-            or daily_apparent_temperature_max[i] >= WARNING_WARM
-        ):
-            warning = warning + " " + WARM
-        weather, emojiweather = traduction(weather_code[i],1)
-
-        vent = f"{daily_wind_speed_10m_max[i]:.1f}km/h ({daily_wind_gusts_10m_max[i]:.1f}km/h)"
-        direction=calculer_direction(daily_wind_direction_10m_dominant[i])
-
-
-        vent = vent
-        if daily_wind_speed_10m_max[i] >= WARNING_WIND or daily_wind_gusts_10m_max[i] >= WARNING_WIND_GUST:
-            warning = warning + " " + WIND
-        duree_pluie = f"{precipitation_hours[i]:.0f}h"
-        duree_soleil = f"{sunshine_duration[i]/3600:.1f}h"
-        if compute_args().nocolor:
-            data.append(
-                [
-                    datetime.datetime.strftime(
-                        datetime.datetime.now(tz=pytz.timezone(tz)).replace(
-                            hour=0, minute=0, second=0, microsecond=0
-                        )
-                        + datetime.timedelta(hours=24 * i),
-                        "%Y-%m-%d",
-                    ),
-                    weather,
-                    temp,
-                    pluie,
-                    vent,
-                    direction,
-                    duree_pluie,
-                    duree_soleil
+        if not numpy.isnan(daily_precipitation_sum[i]):
+            warning = ""
+            pluie = f"{daily_precipitation_sum[i]:.1f}mm"
+            if snowfall[i] >= WARNING_SNOW:
+                warning = warning + " " + SNOW
+            elif daily_precipitation_sum[i] >= WARNING_RAIN:
+                warning = warning + " " + RAIN
+            temp = f"{daily_temperature_2m_min[i]:.1f}°C ({daily_apparent_temperature_min[i]:.1f}°C) -> {daily_temperature_2m_max[i]:.1f}°C ({daily_apparent_temperature_max[i]:.1f}°C)"
+            if (
+                daily_temperature_2m_min[i] <= WARNING_FROID
+                or daily_apparent_temperature_min[i] <= WARNING_FROID
+                or daily_temperature_2m_max[i] <= WARNING_FROID
+                or daily_apparent_temperature_max[i] <= WARNING_FROID
+            ):
+                warning = warning + " " + COLD
+            if (
+                daily_temperature_2m_min[i] >= WARNING_WARM
+                or daily_apparent_temperature_min[i] >= WARNING_WARM
+                or daily_temperature_2m_max[i] >= WARNING_WARM
+                or daily_apparent_temperature_max[i] >= WARNING_WARM
+            ):
+                warning = warning + " " + WARM
+            weather, emojiweather = traduction(weather_code[i],1)
+
+            vent = f"{daily_wind_speed_10m_max[i]:.1f}km/h ({daily_wind_gusts_10m_max[i]:.1f}km/h)"
+            direction=calculer_direction(daily_wind_direction_10m_dominant[i])
+
+
+            vent = vent
+            if daily_wind_speed_10m_max[i] >= WARNING_WIND or daily_wind_gusts_10m_max[i] >= WARNING_WIND_GUST:
+                warning = warning + " " + WIND
+            duree_pluie = f"{precipitation_hours[i]:.0f}h"
+            duree_soleil = f"{sunshine_duration[i]/3600:.1f}h"
+            if compute_args().nocolor:
+                data.append(
+                    [
+                        datetime.datetime.strftime(
+                            datetime.datetime.now(tz=pytz.timezone(tz)).replace(
+                                hour=0, minute=0, second=0, microsecond=0
+                            )
+                            + datetime.timedelta(hours=24 * i),
+                            "%Y-%m-%d",
+                        ),
+                        weather,
+                        temp,
+                        pluie,
+                        vent,
+                        direction,
+                        duree_pluie,
+                        duree_soleil
+                    ]
+                )
+                headers = [
+                    "date",
+                    "temps",
+                    "température (ressentie)",
+                    "précipitations",
+                    "vent (rafales)",
+                    "direction",
+                    "durée pluie",
+                    "durée soleil"
                 ]
-            )
-            headers = [
-                "date",
-                "temps",
-                "température (ressentie)",
-                "précipitations",
-                "vent (rafales)",
-                "direction",
-                "durée pluie",
-                "durée soleil"
-            ]
-        else:
-            data.append(
-                [
-                    datetime.datetime.strftime(
-                        datetime.datetime.now(tz=pytz.timezone(tz)).replace(
-                            hour=0, minute=0, second=0, microsecond=0
-                        )
-                        + datetime.timedelta(hours=24 * i)
-                        + datetime.timedelta(days=-1*compute_args().past),
-                        "%Y-%m-%d",
-                    ),
-                    emojiweather + " " + weather,
-                    temp,
-                    pluie,
-                    vent,
-                    direction,
-                    duree_pluie,
-                    duree_soleil,
-                    warning,
+            else:
+                data.append(
+                    [
+                        datetime.datetime.strftime(
+                            datetime.datetime.now(tz=pytz.timezone(tz)).replace(
+                                hour=0, minute=0, second=0, microsecond=0
+                            )
+                            + datetime.timedelta(hours=24 * i)
+                            + datetime.timedelta(days=-1*compute_args().past),
+                            "%Y-%m-%d",
+                        ),
+                        emojiweather + " " + weather,
+                        temp,
+                        pluie,
+                        vent,
+                        direction,
+                        duree_pluie,
+                        duree_soleil,
+                        warning,
+                    ]
+                )
+                headers = [
+                    "date",
+                    "temps",
+                    "température (ressentie)",
+                    "précipitations",
+                    "vent (rafales)",
+                    "direction vent",
+                    "durée pluie",
+                    "durée soleil",
+                    "warning",
                 ]
-            )
-            headers = [
-                "date",
-                "temps",
-                "température (ressentie)",
-                "précipitations",
-                "vent (rafales)",
-                "direction vent",
-                "durée pluie",
-                "durée soleil",
-                "warning",
-            ]
-
+        else:
+            tronque=True
     if data != []:
         if compute_args().condensate:
             table = columnar.columnar(data, headers, no_borders=True, wrap_max=0)
         else:
             print("")
             table = columnar.columnar(data, headers, no_borders=False, wrap_max=0)
         print(table)
-
+    if tronque:
+        print(my_colored("warning : données tronquées", "yellow"))
 
 def print_generic_data_town(ville, dpt, lat, long, alt, recap):
     print("")
 
     data = []
     if compute_args().nocolor:
         if (ville is None or ville == "") and (dpt is None or dpt == ""):
```

### Comparing `pyweatherfr-5.1.1/pyweatherfr.egg-info/PKG-INFO` & `pyweatherfr-5.1.2/pyweatherfr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 5.1.1
+Version: 5.1.2
 Summary: pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-5.1.1/setup.py` & `pyweatherfr-5.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="pyweatherfr",
-    version="5.1.1",
+    version="5.1.2",
     description="pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)",
     long_description="The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme",
     url="https://github.com/thib1984/pyweatherfr",
     author="thib1984",
     author_email="thibault.garcon@gmail.com",
     license="MIT",
     packages=["pyweatherfr"],
```

