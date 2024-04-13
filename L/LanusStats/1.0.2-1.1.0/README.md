# Comparing `tmp/LanusStats-1.0.2.tar.gz` & `tmp/LanusStats-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LanusStats-1.0.2.tar", last modified: Sun Apr  7 21:19:37 2024, max compression
+gzip compressed data, was "LanusStats-1.1.0.tar", last modified: Sat Apr 13 23:21:00 2024, max compression
```

## Comparing `LanusStats-1.0.2.tar` & `LanusStats-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 21:19:37.696142 LanusStats-1.0.2/
-drwxrwxrwx   0        0        0        0 2024-04-07 21:19:37.673043 LanusStats-1.0.2/LanusStats/
--rw-rw-rw-   0        0        0      222 2024-04-07 03:06:19.000000 LanusStats-1.0.2/LanusStats/__init__.py
--rw-rw-rw-   0        0        0     1759 2024-04-04 03:40:59.000000 LanusStats-1.0.2/LanusStats/exceptions.py
--rw-rw-rw-   0        0        0    14779 2024-04-07 03:01:27.000000 LanusStats-1.0.2/LanusStats/fbref.py
--rw-rw-rw-   0        0        0    11325 2024-04-07 03:01:27.000000 LanusStats-1.0.2/LanusStats/fotmob.py
--rw-rw-rw-   0        0        0    16568 2024-04-07 03:01:27.000000 LanusStats-1.0.2/LanusStats/functions.py
--rw-rw-rw-   0        0        0    19078 2024-04-07 21:18:09.000000 LanusStats-1.0.2/LanusStats/sofascore.py
--rw-rw-rw-   0        0        0     6439 2024-04-07 03:01:27.000000 LanusStats-1.0.2/LanusStats/threesixfivescores.py
--rw-rw-rw-   0        0        0     8640 2024-04-07 03:10:29.000000 LanusStats-1.0.2/LanusStats/visualizations.py
-drwxrwxrwx   0        0        0        0 2024-04-07 21:19:37.691513 LanusStats-1.0.2/LanusStats.egg-info/
--rw-rw-rw-   0        0        0     4858 2024-04-07 21:19:37.000000 LanusStats-1.0.2/LanusStats.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      386 2024-04-07 21:19:37.000000 LanusStats-1.0.2/LanusStats.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 21:19:37.000000 LanusStats-1.0.2/LanusStats.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-07 21:19:37.000000 LanusStats-1.0.2/LanusStats.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-07 21:19:37.000000 LanusStats-1.0.2/LanusStats.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4858 2024-04-07 21:19:37.695137 LanusStats-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4476 2024-04-07 16:05:01.000000 LanusStats-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 21:19:37.697139 LanusStats-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1012 2024-04-07 21:18:52.000000 LanusStats-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 23:21:00.414178 LanusStats-1.1.0/
+drwxrwxrwx   0        0        0        0 2024-04-13 23:21:00.394147 LanusStats-1.1.0/LanusStats/
+-rw-rw-rw-   0        0        0      222 2024-04-07 03:06:19.000000 LanusStats-1.1.0/LanusStats/__init__.py
+-rw-rw-rw-   0        0        0      234 2024-04-13 23:20:47.000000 LanusStats-1.1.0/LanusStats/config.py
+-rw-rw-rw-   0        0        0     1759 2024-04-04 03:40:59.000000 LanusStats-1.1.0/LanusStats/exceptions.py
+-rw-rw-rw-   0        0        0    14779 2024-04-07 03:01:27.000000 LanusStats-1.1.0/LanusStats/fbref.py
+-rw-rw-rw-   0        0        0    11508 2024-04-13 23:20:47.000000 LanusStats-1.1.0/LanusStats/fotmob.py
+-rw-rw-rw-   0        0        0    16566 2024-04-13 23:20:47.000000 LanusStats-1.1.0/LanusStats/functions.py
+-rw-rw-rw-   0        0        0      303 2024-04-13 23:20:47.000000 LanusStats-1.1.0/LanusStats/sofascore.py
+-rw-rw-rw-   0        0        0     6605 2024-04-13 23:20:47.000000 LanusStats-1.1.0/LanusStats/threesixfivescores.py
+-rw-rw-rw-   0        0        0     8640 2024-04-07 03:10:29.000000 LanusStats-1.1.0/LanusStats/visualizations.py
+drwxrwxrwx   0        0        0        0 2024-04-13 23:21:00.409850 LanusStats-1.1.0/LanusStats.egg-info/
+-rw-rw-rw-   0        0        0     4858 2024-04-13 23:20:59.000000 LanusStats-1.1.0/LanusStats.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      407 2024-04-13 23:21:00.000000 LanusStats-1.1.0/LanusStats.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 23:20:59.000000 LanusStats-1.1.0/LanusStats.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-04-13 23:20:59.000000 LanusStats-1.1.0/LanusStats.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-13 23:20:59.000000 LanusStats-1.1.0/LanusStats.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4858 2024-04-13 23:21:00.412848 LanusStats-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4476 2024-04-07 16:05:01.000000 LanusStats-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-13 23:21:00.415053 LanusStats-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1012 2024-04-13 23:20:47.000000 LanusStats-1.1.0/setup.py
```

### Comparing `LanusStats-1.0.2/LanusStats/exceptions.py` & `LanusStats-1.1.0/LanusStats/exceptions.py`

 * *Files identical despite different names*

### Comparing `LanusStats-1.0.2/LanusStats/fbref.py` & `LanusStats-1.1.0/LanusStats/fbref.py`

 * *Files identical despite different names*

### Comparing `LanusStats-1.0.2/LanusStats/fotmob.py` & `LanusStats-1.1.0/LanusStats/fotmob.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import requests
 import pandas as pd
 import json
-from .functions import get_possible_leagues_for_page
+import matplotlib.pyplot as plt
 import time
+from .functions import get_possible_leagues_for_page
 from .exceptions import InvalidStat, MatchDoesntHaveInfo
-import matplotlib.pyplot as plt
+from .config import headers
 
 class FotMob:
     
     def __init__(self):
         self.player_possible_stats = ['goals',
             'goal_assist',
             '_goals_and_goal_assist',
@@ -82,15 +83,16 @@
 
         Returns:
             table_df: DataFrame with the table/s. 
         """
         leagues = get_possible_leagues_for_page(league, season, 'Fotmob')
         league_id = leagues[league]['id']
         season_string = season.replace('/', '%2F')
-        response = requests.get(f'https://www.fotmob.com/api/leagues?id={league_id}&ccode3=ARG&season={season_string}')
+        response = requests.get(f'https://www.fotmob.com/api/leagues?id={league_id}&ccode3=ARG&season={season_string}', headers=headers)
+        time.sleep(3)
         try:
             tables = response.json()['table'][0]['data']['table']
             table = tables[table]
             table_df = pd.DataFrame(table)
         except KeyError:
             tables = response.json()['table'][0]['data']['tables']
             table_df = tables
@@ -102,15 +104,16 @@
 
         Args:
             match_id (str): id of a certain match, could be found in the URL
 
         Returns:
             response: json with the response.
         """
-        response = requests.get(f'https://www.fotmob.com/api/matchDetails?matchId={match_id}')
+        response = requests.get(f'https://www.fotmob.com/api/matchDetails?matchId={match_id}', headers=headers)
+        time.sleep(3)
         return response
     
     def get_players_stats_season(self, league, season, stat):
         """Get players for a certain season and league stats. Possible stats are player_possible_stats.
 
         Args:
             league (str): Possible leagues in get_available_leagues("Fotmob")
@@ -125,16 +128,16 @@
         """
         print(f'Possible values for stat parameter: {self.player_possible_stats}')
         if stat not in self.player_possible_stats:
             raise InvalidStat(stat, self.player_possible_stats)
         leagues = get_possible_leagues_for_page(league, season, 'Fotmob')
         league_id = leagues[league]['id']
         season_id = leagues[league]['seasons'][season]
-        response = requests.get(f'https://www.fotmob.com/api/leagueseasondeepstats?id={league_id}&season={season_id}&type=players&stat={stat}')
-        time.sleep(1)
+        response = requests.get(f'https://www.fotmob.com/api/leagueseasondeepstats?id={league_id}&season={season_id}&type=players&stat={stat}', headers=headers)
+        time.sleep(3)
         df_1 = pd.DataFrame(response.json()['statsData'])
         df_2 = pd.DataFrame(response.json()['statsData']).statValue.apply(pd.Series)
         df = pd.concat([df_1, df_2], axis=1)
         return df
     
     def get_teams_stats_season(self, league, season, stat):
         """Get teams for a certain season and league stats. Possible stats are team_possible_stats.
@@ -152,16 +155,16 @@
         """
         print(f'Possible values for stat parameter: {self.team_possible_stats}')
         if stat not in self.team_possible_stats:
             raise InvalidStat(stat, self.team_possible_stats)
         leagues = get_possible_leagues_for_page(league, season, 'Fotmob')
         league_id = leagues[league]['id']
         season_id = leagues[league]['seasons'][season]
-        response = requests.get(f'https://www.fotmob.com/api/leagueseasondeepstats?id={league_id}&season={season_id}&type=teams&stat={stat}')
-        time.sleep(1)
+        response = requests.get(f'https://www.fotmob.com/api/leagueseasondeepstats?id={league_id}&season={season_id}&type=teams&stat={stat}', headers=headers)
+        time.sleep(3)
         df_1 = pd.DataFrame(response.json()['statsData'])
         df_2 = pd.DataFrame(response.json()['statsData']).statValue.apply(pd.Series)
         df = pd.concat([df_1, df_2], axis=1)
         return df
 
     def get_match_shotmap(self, match_id):
         """Scrape a match shotmap, if it has one.
@@ -244,10 +247,11 @@
 
         Returns:
             shotmap: DataFrame with the data for all the shots shown in the FotMob UI.
         """
         leagues = get_possible_leagues_for_page(league, season, 'Fotmob')
         league_id = leagues[league]['id']
         season_string = season.replace('/', '%2F')
-        response = requests.get(f'https://www.fotmob.com/api/playerStats?playerId={player_id}&seasonId={season_string}-{league_id}')
+        response = requests.get(f'https://www.fotmob.com/api/playerStats?playerId={player_id}&seasonId={season_string}-{league_id}', headers=headers)
+        time.sleep(3)
         shotmap = pd.DataFrame(response.json()['shotmap'])
         return shotmap
```

### Comparing `LanusStats-1.0.2/LanusStats/functions.py` & `LanusStats-1.1.0/LanusStats/functions.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -478,8 +478,8 @@
         page (str): Page inside the array of get_available_pagues()
         league (str): League inside the array of get_available_leagues(page)
 
     Returns:
         dict: League data with the seasons inside
     """
     league_data = get_possible_leagues('Argentina Copa de la Liga', '2023', 'Fotmob')[page][league]
-    return league_data
+    return league_data
```

### Comparing `LanusStats-1.0.2/LanusStats/threesixfivescores.py` & `LanusStats-1.1.0/LanusStats/threesixfivescores.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import requests
 import json
 from PIL import Image
 import re
 from io import BytesIO
 from .functions import get_possible_leagues_for_page
 from .exceptions import MatchDoesntHaveInfo
+from .config import headers
+import time
 
 class ThreeSixFiveScores:
 
     def parse_dataframe(self, objeto):
         df = pd.DataFrame(objeto['rows'])
         df_1 = df['entity'].apply(pd.Series)
         df_2 = df['stats'].apply(pd.Series)[0].apply(pd.Series)
@@ -25,15 +27,16 @@
                           The page don't show stats from previous seasons.
 
         Returns:
             total_df: DataFrame with all the stats, values and players.
         """
         leagues = get_possible_leagues_for_page(league, None, '365Scores')
         league_id = leagues[league]['id']
-        response = requests.get(f'https://webws.365scores.com/web/stats/?appTypeId=5&langId=29&timezoneName=America/Buenos_Aires&userCountryId=382&competitions={league_id}&competitors=&withSeasons=true')
+        response = requests.get(f'https://webws.365scores.com/web/stats/?appTypeId=5&langId=29&timezoneName=America/Buenos_Aires&userCountryId=382&competitions={league_id}&competitors=&withSeasons=true', headers=headers)
+        time.sleep(3)
         stats = response.json()
         general_stats = stats['stats']
         total_df = pd.DataFrame()
         for i in range(len(general_stats)):
             objeto = general_stats[i]
             stats_df = self.parse_dataframe(objeto)
             total_df = pd.concat([total_df, stats_df])
@@ -63,15 +66,16 @@
             match_url (url): 365Scores match URL. Example: https://www.365scores.com/es-mx/football/match/copa-de-la-liga-profesional-7214/lanus-union-santa-fe-869-7206-7214#id=4033824
 
         Returns:
             match_data: Json with game data.
         """
         
         matchup_id, game_id = self.get_ids(match_url)
-        response = requests.get(f'https://webws.365scores.com/web/game/?appTypeId=5&langId=29&timezoneName=America/Buenos_Aires&userCountryId=382&gameId={game_id}&matchupId={matchup_id}&topBookmaker=14')
+        response = requests.get(f'https://webws.365scores.com/web/game/?appTypeId=5&langId=29&timezoneName=America/Buenos_Aires&userCountryId=382&gameId={game_id}&matchupId={matchup_id}&topBookmaker=14', headers=headers)
+        time.sleep(3)
         match_data = response.json()['game']
         return match_data
     
     def get_match_shotmap(self, match_url):
         """Scrape shotmap from the page as a DataFrame, if the match has it.
 
         Args:
@@ -142,12 +146,13 @@
         """
         match_data = self.get_match_data(match_url)
         players = match_data['homeCompetitor']['lineups']['members']
         df_players = pd.DataFrame(players)
         players_total = pd.DataFrame(match_data['members'])
         df_players = df_players.merge(players_total, on='id', how='left')
         try:
-            heatmap = requests.get(df_players[df_players['name'] == player].heatMap.iloc[0])
+            heatmap = requests.get(df_players[df_players['name'] == player].heatMap.iloc[0], headers=headers)
+            time.sleep(3)
         except AttributeError:
             raise MatchDoesntHaveInfo(match_url)
         heatmap_image = Image.open(BytesIO(heatmap.content))
         return heatmap_image
```

### Comparing `LanusStats-1.0.2/LanusStats/visualizations.py` & `LanusStats-1.1.0/LanusStats/visualizations.py`

 * *Files identical despite different names*

### Comparing `LanusStats-1.0.2/LanusStats.egg-info/PKG-INFO` & `LanusStats-1.1.0/LanusStats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LanusStats
-Version: 1.0.2
+Version: 1.1.0
 Summary: Python library for scraping football data and visualize it / Libreria de Python para scrapear data de fútbol y visualizarla
 Home-page: https://github.com/federicorabanos
 Author: Federico Rábanos
 Author-email: lanusstats@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `LanusStats-1.0.2/PKG-INFO` & `LanusStats-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LanusStats
-Version: 1.0.2
+Version: 1.1.0
 Summary: Python library for scraping football data and visualize it / Libreria de Python para scrapear data de fútbol y visualizarla
 Home-page: https://github.com/federicorabanos
 Author: Federico Rábanos
 Author-email: lanusstats@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `LanusStats-1.0.2/README.md` & `LanusStats-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `LanusStats-1.0.2/setup.py` & `LanusStats-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.0.2'
+VERSION = '1.1.0'
 PACKAGE_NAME = 'LanusStats'
 AUTHOR = 'Federico Rábanos'
 AUTHOR_EMAIL = 'lanusstats@gmail.com'
 URL = 'https://github.com/federicorabanos'
 
 LICENSE = 'MIT'
 DESCRIPTION = 'Python library for scraping football data and visualize it / Libreria de Python para scrapear data de fútbol y visualizarla'
```

