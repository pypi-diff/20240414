# Comparing `tmp/nokey-0.0.1.tar.gz` & `tmp/nokey-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nokey-0.0.1.tar", last modified: Thu Apr 11 00:08:55 2024, max compression
+gzip compressed data, was "nokey-0.1.0.tar", last modified: Sun Apr 14 00:33:39 2024, max compression
```

## Comparing `nokey-0.0.1.tar` & `nokey-0.1.0.tar`

### file list

```diff
@@ -1,49 +1,64 @@
-drwx------   0 root         (0) root         (0)        0 2024-04-11 00:08:55.947324 nokey-0.0.1/
--rw-------   0 root         (0) root         (0)     1068 2024-04-10 23:28:41.000000 nokey-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2501 2024-04-11 00:08:55.943324 nokey-0.0.1/PKG-INFO
--rw-------   0 root         (0) root         (0)     1980 2024-04-10 23:25:41.000000 nokey-0.0.1/README.md
-drwx------   0 root         (0) root         (0)        0 2024-04-11 00:08:55.803324 nokey-0.0.1/nokey/
--rw-rw----   0 root         (0) root         (0)        0 2024-04-10 00:28:19.000000 nokey-0.0.1/nokey/__init__.py
-drwx------   0 root         (0) root         (0)        0 2024-04-11 00:08:55.827324 nokey-0.0.1/nokey/animals/
--rw-rw----   0 root         (0) root         (0)        0 2024-04-10 00:28:20.000000 nokey-0.0.1/nokey/animals/__init__.py
--rw-rw----   0 root         (0) root         (0)     2615 2024-04-10 00:28:20.000000 nokey-0.0.1/nokey/animals/dog_api.py
-drwx------   0 root         (0) root         (0)        0 2024-04-11 00:08:55.835324 nokey-0.0.1/nokey/country_info/
--rw-rw----   0 root         (0) root         (0)        0 2024-04-10 00:28:19.000000 nokey-0.0.1/nokey/country_info/__init__.py
--rw-rw----   0 root         (0) root         (0)     4542 2024-04-10 22:46:06.000000 nokey-0.0.1/nokey/country_info/rest_country.py
-drwx------   0 root         (0) root         (0)        0 2024-04-11 00:08:55.847324 nokey-0.0.1/nokey/education/
--rw-rw----   0 root         (0) root         (0)        0 2024-04-10 00:28:20.000000 nokey-0.0.1/nokey/education/__init__.py
--rw-rw----   0 root         (0) root         (0)     2215 2024-04-10 00:28:20.000000 nokey-0.0.1/nokey/education/university_names_and_domains.py
-drwx------   0 root         (0) root         (0)        0 2024-04-11 00:08:55.859324 nokey-0.0.1/nokey/finance/
--rw-rw----   0 root         (0) root         (0)        0 2024-04-10 00:28:20.000000 nokey-0.0.1/nokey/finance/__init__.py
--rw-rw----   0 root         (0) root         (0)      695 2024-04-10 00:28:20.000000 nokey-0.0.1/nokey/finance/wall_street_bets.py
-drwx------   0 root         (0) root         (0)        0 2024-04-11 00:08:55.867324 nokey-0.0.1/nokey/food/
--rw-rw----   0 root         (0) root         (0)        0 2024-04-10 00:28:20.000000 nokey-0.0.1/nokey/food/__init__.py
--rw-rw----   0 root         (0) root         (0)     3044 2024-04-10 00:28:20.000000 nokey-0.0.1/nokey/food/fruityvice.py
-drwx------   0 root         (0) root         (0)        0 2024-04-11 00:08:55.875324 nokey-0.0.1/nokey/geolocation/
--rw-rw----   0 root         (0) root         (0)        0 2024-04-10 00:28:19.000000 nokey-0.0.1/nokey/geolocation/__init__.py
--rw-rw----   0 root         (0) root         (0)      911 2024-04-10 00:28:19.000000 nokey-0.0.1/nokey/geolocation/ip_api.py
-drwx------   0 root         (0) root         (0)        0 2024-04-11 00:08:55.887324 nokey-0.0.1/nokey/helperFuncs/
--rw-rw----   0 root         (0) root         (0)        0 2024-04-10 00:28:19.000000 nokey-0.0.1/nokey/helperFuncs/__init__.py
--rw-rw----   0 root         (0) root         (0)     1393 2024-04-10 00:28:19.000000 nokey-0.0.1/nokey/helperFuncs/make_request.py
-drwx------   0 root         (0) root         (0)        0 2024-04-11 00:08:55.895324 nokey-0.0.1/nokey/jokes/
--rw-rw----   0 root         (0) root         (0)        0 2024-04-10 00:28:19.000000 nokey-0.0.1/nokey/jokes/__init__.py
--rw-rw----   0 root         (0) root         (0)     2700 2024-04-10 00:28:19.000000 nokey-0.0.1/nokey/jokes/joke_api.py
-drwx------   0 root         (0) root         (0)        0 2024-04-11 00:08:55.903324 nokey-0.0.1/nokey/random/
--rw-rw----   0 root         (0) root         (0)        0 2024-04-10 00:28:19.000000 nokey-0.0.1/nokey/random/__init__.py
--rw-rw----   0 root         (0) root         (0)      932 2024-04-10 00:28:19.000000 nokey-0.0.1/nokey/random/random_user.py
-drwx------   0 root         (0) root         (0)        0 2024-04-11 00:08:55.915324 nokey-0.0.1/nokey/science/
--rw-rw----   0 root         (0) root         (0)        0 2024-04-10 00:28:20.000000 nokey-0.0.1/nokey/science/__init__.py
--rw-rw----   0 root         (0) root         (0)     2802 2024-04-10 00:28:20.000000 nokey-0.0.1/nokey/science/nobel_prize.py
-drwx------   0 root         (0) root         (0)        0 2024-04-11 00:08:55.923324 nokey-0.0.1/nokey/spaceflight/
--rw-rw----   0 root         (0) root         (0)        0 2024-04-10 00:28:19.000000 nokey-0.0.1/nokey/spaceflight/__init__.py
--rw-rw----   0 root         (0) root         (0)     8565 2024-04-10 00:28:19.000000 nokey-0.0.1/nokey/spaceflight/spaceflight_news.py
-drwx------   0 root         (0) root         (0)        0 2024-04-11 00:08:55.931324 nokey-0.0.1/nokey/weather/
--rw-rw----   0 root         (0) root         (0)        0 2024-04-10 00:28:20.000000 nokey-0.0.1/nokey/weather/__init__.py
--rw-rw----   0 root         (0) root         (0)    25903 2024-04-10 00:28:20.000000 nokey-0.0.1/nokey/weather/national_weather_service.py
-drwx------   0 root         (0) root         (0)        0 2024-04-11 00:08:55.939324 nokey-0.0.1/nokey.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2501 2024-04-11 00:08:55.000000 nokey-0.0.1/nokey.egg-info/PKG-INFO
--rw-------   0 root         (0) root         (0)      881 2024-04-11 00:08:55.000000 nokey-0.0.1/nokey.egg-info/SOURCES.txt
--rw-------   0 root         (0) root         (0)        1 2024-04-11 00:08:55.000000 nokey-0.0.1/nokey.egg-info/dependency_links.txt
--rw-------   0 root         (0) root         (0)        6 2024-04-11 00:08:55.000000 nokey-0.0.1/nokey.egg-info/top_level.txt
--rw-rw----   0 root         (0) root         (0)      503 2024-04-11 00:01:03.000000 nokey-0.0.1/pyproject.toml
--rw-------   0 root         (0) root         (0)       38 2024-04-11 00:08:55.947324 nokey-0.0.1/setup.cfg
+drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.425000 nokey-0.1.0/
+-rw-------   0 root         (0) root         (0)     1068 2024-04-10 23:28:41.000000 nokey-0.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2962 2024-04-14 00:33:39.421000 nokey-0.1.0/PKG-INFO
+-rw-------   0 root         (0) root         (0)     2441 2024-04-14 00:25:34.000000 nokey-0.1.0/README.md
+drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.221000 nokey-0.1.0/nokey/
+-rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/__init__.py
+drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.245000 nokey-0.1.0/nokey/animals/
+-rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:34.000000 nokey-0.1.0/nokey/animals/__init__.py
+-rw-------   0 root         (0) root         (0)     2615 2024-04-14 00:27:34.000000 nokey-0.1.0/nokey/animals/dog_api.py
+drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.257000 nokey-0.1.0/nokey/country_info/
+-rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/country_info/__init__.py
+-rw-------   0 root         (0) root         (0)     4631 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/country_info/rest_country.py
+drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.265000 nokey-0.1.0/nokey/developer_tools/
+-rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:34.000000 nokey-0.1.0/nokey/developer_tools/__init__.py
+-rw-------   0 root         (0) root         (0)     1489 2024-04-14 00:27:34.000000 nokey-0.1.0/nokey/developer_tools/url_shortener.py
+drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.273000 nokey-0.1.0/nokey/education/
+-rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/education/__init__.py
+-rw-------   0 root         (0) root         (0)     2215 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/education/university_names_and_domains.py
+drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.285000 nokey-0.1.0/nokey/finance/
+-rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/finance/__init__.py
+-rw-------   0 root         (0) root         (0)      977 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/finance/wall_street_bets.py
+drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.293000 nokey-0.1.0/nokey/food/
+-rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:34.000000 nokey-0.1.0/nokey/food/__init__.py
+-rw-------   0 root         (0) root         (0)     3044 2024-04-14 00:27:34.000000 nokey-0.1.0/nokey/food/fruityvice.py
+drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.305000 nokey-0.1.0/nokey/games/
+-rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:34.000000 nokey-0.1.0/nokey/games/__init__.py
+-rw-------   0 root         (0) root         (0)     6369 2024-04-14 00:27:34.000000 nokey-0.1.0/nokey/games/free_to_game.py
+drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.321000 nokey-0.1.0/nokey/geolocation/
+-rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/geolocation/__init__.py
+-rw-------   0 root         (0) root         (0)      916 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/geolocation/ip_api.py
+-rw-------   0 root         (0) root         (0)     1692 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/geolocation/zippopotamus.py
+drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.341000 nokey-0.1.0/nokey/helperFuncs/
+-rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/helperFuncs/__init__.py
+-rw-------   0 root         (0) root         (0)      822 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/helperFuncs/get_api_list.py
+-rw-------   0 root         (0) root         (0)     1393 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/helperFuncs/make_request.py
+-rw-------   0 root         (0) root         (0)      576 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/helperFuncs/nokey_apis.py
+drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.353000 nokey-0.1.0/nokey/inspiration/
+-rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:34.000000 nokey-0.1.0/nokey/inspiration/__init__.py
+-rw-------   0 root         (0) root         (0)     5764 2024-04-14 00:27:34.000000 nokey-0.1.0/nokey/inspiration/dictum.py
+drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.361000 nokey-0.1.0/nokey/jokes/
+-rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/jokes/__init__.py
+-rw-------   0 root         (0) root         (0)     2700 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/jokes/joke_api.py
+drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.369000 nokey-0.1.0/nokey/language/
+-rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:34.000000 nokey-0.1.0/nokey/language/__init__.py
+-rw-------   0 root         (0) root         (0)     1013 2024-04-14 00:27:34.000000 nokey-0.1.0/nokey/language/free_dictionary.py
+drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.381000 nokey-0.1.0/nokey/random/
+-rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/random/__init__.py
+-rw-------   0 root         (0) root         (0)      932 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/random/random_user.py
+drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.389000 nokey-0.1.0/nokey/science/
+-rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:34.000000 nokey-0.1.0/nokey/science/__init__.py
+-rw-------   0 root         (0) root         (0)     2802 2024-04-14 00:27:34.000000 nokey-0.1.0/nokey/science/nobel_prize.py
+drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.401000 nokey-0.1.0/nokey/spaceflight/
+-rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/spaceflight/__init__.py
+-rw-------   0 root         (0) root         (0)     8565 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/spaceflight/spaceflight_news.py
+drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.409000 nokey-0.1.0/nokey/weather/
+-rw-------   0 root         (0) root         (0)        0 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/weather/__init__.py
+-rw-------   0 root         (0) root         (0)    25903 2024-04-14 00:27:33.000000 nokey-0.1.0/nokey/weather/national_weather_service.py
+drwx------   0 root         (0) root         (0)        0 2024-04-14 00:33:39.417000 nokey-0.1.0/nokey.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2962 2024-04-14 00:33:38.000000 nokey-0.1.0/nokey.egg-info/PKG-INFO
+-rw-------   0 root         (0) root         (0)     1225 2024-04-14 00:33:39.000000 nokey-0.1.0/nokey.egg-info/SOURCES.txt
+-rw-------   0 root         (0) root         (0)        1 2024-04-14 00:33:38.000000 nokey-0.1.0/nokey.egg-info/dependency_links.txt
+-rw-------   0 root         (0) root         (0)        6 2024-04-14 00:33:39.000000 nokey-0.1.0/nokey.egg-info/top_level.txt
+-rw-rw----   0 root         (0) root         (0)      503 2024-04-14 00:28:11.000000 nokey-0.1.0/pyproject.toml
+-rw-------   0 root         (0) root         (0)       38 2024-04-14 00:33:39.425000 nokey-0.1.0/setup.cfg
```

### Comparing `nokey-0.0.1/LICENSE` & `nokey-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nokey-0.0.1/PKG-INFO` & `nokey-0.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,15 @@
-Metadata-Version: 2.1
-Name: nokey
-Version: 0.0.1
-Summary: A python package for accessing APIs that require no key.
-Author-email: Spyder Rex <billyjohnsonauthor@gmail.com>
-Project-URL: Homepage, https://github.com/SpyderRex/nokey
-Project-URL: Issues, https://github.com/Spyder/nokey/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # nokey - Access APIs without a Key
 
 nokey is a Python package designed to provide easy access to various APIs that do not require an API key for authentication. This project aims to simplify the process of interacting with different APIs by offering a unified interface for accessing them, all within a single Python package.
 
 ## Features
 
 - Access a growing collection of keyless APIs conveniently from one place.
-- Organized into submodules based on categories such as country information, finance, geolocation, spaceflight, education, food, random data, jokes, animals, science, and weather.
+- Organized into submodules based on categories such as country information, finance, geolocation, spaceflight, education, food, random data, jokes, animals, science, and weather, developer tools, language, and games.
 - Easily installable via pip, making it accessible to all Python developers.
 
 ## Installation
 
 You can install the module using pip:
 
 ```
@@ -43,24 +29,35 @@
 # Get a random dog image URL
 dog_image_url = dog.get_random_dog_image()
 
 # Print the URL
 print(dog_image_url)
 ```
 
+Also, to print out a list of the APIs supported by nokey, simply run the following script:
+
+```python
+from nokey.helperFuncs import get_api_list
+
+api_list = get_api_list()
+
+prrint(api_list)
+```
+
 ## Contributing
 We welcome contributions to expand the range of APIs available in nokey. Whether you want to add a new submodule or enhance an existing one, your contributions are valuable. To contribute, please fork the repository, make your changes, and submit a pull request.
 
 Supported APIs
 ## Country Info
 RestCountries
 ## Finance
 Wallstreet Bets
 ## Geolocation
 IP API
+Zippopotomus
 ## Spaceflight
 Spaceflight News
 ## Education
 University Names and Domains
 ## Food
 Fruityvice
 ## Random
@@ -69,13 +66,25 @@
 JokeAPI
 ## Animals
 DogAPI
 ## Science
 Nobel Prize API
 ## Weather
 National Weather Service API
+## Inspiration
+Dictum
+## Games
+Free To Game
+## Language
+Free Dictionary
+Developer Tools
+URl Shortener ...
+... and many more on the way.
 
 # Future Roadmap
 As the project grows, we envision expanding the collection of keyless APIs to cover a wide range of categories. Your feedback and contributions will play a crucial role in shaping the future of nokey.
 
 # License
 This project is licensed under the MIT License - see the LICENSE file for details.
+
+# Documentation
+Check out the [docs](https://nokey.readthedocs.io/en/latest/)
```

### Comparing `nokey-0.0.1/nokey/animals/dog_api.py` & `nokey-0.1.0/nokey/animals/dog_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.0.1/nokey/country_info/rest_country.py` & `nokey-0.1.0/nokey/country_info/rest_country.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     
     Attributes:
     - base_url: The base URL of the RestCountries API.
     """
     def __init__(self):
         self.base_url = "https://restcountries.com/v3.1/"
         
-    def get_url(self):
+    def get_docs_url(self):
         """
         Returns url for API docs.
         
         Args:
         - None
         
         Returns:
@@ -53,91 +53,98 @@
         """
         Returns information about countries that use a specific currency.
 
         Args:
         - currency (str): The currency code or name.
 
         Returns:
-        - list: A list of dictionaries containing information about countries using the currency, or an error if no countries found.
+        - list: A list of dictionaries containing information about countries using the currency,
+            or an error if no countries found.
         """
         endpoint = f"currency/{currency}"
         return mr.make_request(self.base_url+endpoint)
 
     def get_country_by_language(self, language):
         """
         Returns information about countries speaking a given language.
 
         Args:
         - language (str): The name of the spoken language of the country.
 
         Returns:
-        - list: A list of dictionaries containing information about countries using the language, or an error if no countries found.
+        - list: A list of dictionaries containing information about countries using the language,
+            or an error if no countries found.
         """
         endpoint = f"lang/{language}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_country_by_capital(self, capital):
         """
         Returns information about a country with the given capital
 
         Args:
         - capital (str): The name of the capital city.
 
         Returns:
-        - list: A list of dictionaries containing information about countries using the capital, or an error if no countries found.
+        - list: A list of dictionaries containing information about countries using the capital,
+            or an error if no countries found.
         """
         endpoint = f"capital/{capital}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_country_by_region(self, region):
         """
         Returns information about countries based on a given region.
 
         Args:
         - region (str): The name of the region.
 
         Returns:
-        - list: A list of dictionaries containing information about countries using the region, or an error if no country is found.
+        - list: A list of dictionaries containing information about countries using the region,
+            or an error if no country is found.
         """
         endpoint = f"region/{region}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_country_by_subregion(self, subregion):
         """
         Returns information about countries based on a given subregion.
 
         Args:
         - subregion (str): The name of the subregion.
 
         Returns:
-        - list: A list of dictionaries containing information about countries using the region, or an error if no country is found.
+        - list: A list of dictionaries containing information about countries using the region,
+            or an error if no country is found.
         """
         endpoint = f"subregion/{subregion}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_country_by_translation(self, translation):
         """
         Returns information about countries based on a translation of the name.
 
         Args:
         - translation (str): The name in a given translation.
 
         Returns:
-        - list: A list of dictionaries containing information about countries using the region, or an error if no country is found.
+        - list: A list of dictionaries containing information about countries using the region,
+            or an error if no country is found.
         """
         endpoint = f"translation/{translation}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_all_countries(self):
         """
         Returns information about all countries listed in the API.
 
         Args:
         - None
 
         Returns:
-        - list: A list of dictionaries containing information about all the countries, or an error if no data is found.
+        - list: A list of dictionaries containing information about all the countries,
+            or an error if no data is found.
         """
         endpoint = "all"
         return mr.make_request(self.base_url+endpoint)
```

### Comparing `nokey-0.0.1/nokey/education/university_names_and_domains.py` & `nokey-0.1.0/nokey/education/university_names_and_domains.py`

 * *Files identical despite different names*

### Comparing `nokey-0.0.1/nokey/finance/wall_street_bets.py` & `nokey-0.1.0/nokey/finance/wall_street_bets.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,18 +2,30 @@
 
 
 class WallstreetBets:
     """
     A class to interact with the Wallstreet Bets API.
     
     Attributes:
-    - base_url: The base URL of the WallStreet Bets API.
+    - base_url: The base URL of the Wallstreet Bets API.
     """
     def __init__(self):
-        self.base_url = "https://tradestie.com/api/v1/apps/reddit"        
+        self.base_url = "https://tradestie.com/api/v1/apps/reddit"
+
+    def get_docs_url(self):
+        """
+        Returns the URL for the Wallstreet Bets API documentation.
+        
+        Args:
+        - None
+        
+        Returns:
+        -string: The URL for the API docs.
+        """
+        return "https://tradestie.com/apps/reddit/api/"       
     
     def get_stock_sentiment_from_reddit(self):
         """
         Returns top 50 stocks discussed on Reddit subeddit - Wallstreetbets.
 
         Args:
         - None
```

### Comparing `nokey-0.0.1/nokey/food/fruityvice.py` & `nokey-0.1.0/nokey/food/fruityvice.py`

 * *Files identical despite different names*

### Comparing `nokey-0.0.1/nokey/geolocation/ip_api.py` & `nokey-0.1.0/nokey/geolocation/ip_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     
     Attributes:
     - base_url: The base URL of IP API.
     """
     def __init__(self):
         self.base_url = "http://ip-api.com/json/" 
         
-    def get_url(self):
+    def get_docs_url(self):
         """
         Returns URL for API docs.
         
         Args:
         - None
         
         Returns:
```

### Comparing `nokey-0.0.1/nokey/helperFuncs/make_request.py` & `nokey-0.1.0/nokey/helperFuncs/make_request.py`

 * *Files identical despite different names*

### Comparing `nokey-0.0.1/nokey/jokes/joke_api.py` & `nokey-0.1.0/nokey/jokes/joke_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.0.1/nokey/random/random_user.py` & `nokey-0.1.0/nokey/random/random_user.py`

 * *Files identical despite different names*

### Comparing `nokey-0.0.1/nokey/science/nobel_prize.py` & `nokey-0.1.0/nokey/science/nobel_prize.py`

 * *Files identical despite different names*

### Comparing `nokey-0.0.1/nokey/spaceflight/spaceflight_news.py` & `nokey-0.1.0/nokey/spaceflight/spaceflight_news.py`

 * *Files identical despite different names*

### Comparing `nokey-0.0.1/nokey/weather/national_weather_service.py` & `nokey-0.1.0/nokey/weather/national_weather_service.py`

 * *Files identical despite different names*

### Comparing `nokey-0.0.1/nokey.egg-info/PKG-INFO` & `nokey-0.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nokey
-Version: 0.0.1
+Version: 0.1.0
 Summary: A python package for accessing APIs that require no key.
 Author-email: Spyder Rex <billyjohnsonauthor@gmail.com>
 Project-URL: Homepage, https://github.com/SpyderRex/nokey
 Project-URL: Issues, https://github.com/Spyder/nokey/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 # nokey - Access APIs without a Key
 
 nokey is a Python package designed to provide easy access to various APIs that do not require an API key for authentication. This project aims to simplify the process of interacting with different APIs by offering a unified interface for accessing them, all within a single Python package.
 
 ## Features
 
 - Access a growing collection of keyless APIs conveniently from one place.
-- Organized into submodules based on categories such as country information, finance, geolocation, spaceflight, education, food, random data, jokes, animals, science, and weather.
+- Organized into submodules based on categories such as country information, finance, geolocation, spaceflight, education, food, random data, jokes, animals, science, and weather, developer tools, language, and games.
 - Easily installable via pip, making it accessible to all Python developers.
 
 ## Installation
 
 You can install the module using pip:
 
 ```
@@ -43,24 +43,35 @@
 # Get a random dog image URL
 dog_image_url = dog.get_random_dog_image()
 
 # Print the URL
 print(dog_image_url)
 ```
 
+Also, to print out a list of the APIs supported by nokey, simply run the following script:
+
+```python
+from nokey.helperFuncs import get_api_list
+
+api_list = get_api_list()
+
+prrint(api_list)
+```
+
 ## Contributing
 We welcome contributions to expand the range of APIs available in nokey. Whether you want to add a new submodule or enhance an existing one, your contributions are valuable. To contribute, please fork the repository, make your changes, and submit a pull request.
 
 Supported APIs
 ## Country Info
 RestCountries
 ## Finance
 Wallstreet Bets
 ## Geolocation
 IP API
+Zippopotomus
 ## Spaceflight
 Spaceflight News
 ## Education
 University Names and Domains
 ## Food
 Fruityvice
 ## Random
@@ -69,13 +80,25 @@
 JokeAPI
 ## Animals
 DogAPI
 ## Science
 Nobel Prize API
 ## Weather
 National Weather Service API
+## Inspiration
+Dictum
+## Games
+Free To Game
+## Language
+Free Dictionary
+Developer Tools
+URl Shortener ...
+... and many more on the way.
 
 # Future Roadmap
 As the project grows, we envision expanding the collection of keyless APIs to cover a wide range of categories. Your feedback and contributions will play a crucial role in shaping the future of nokey.
 
 # License
 This project is licensed under the MIT License - see the LICENSE file for details.
+
+# Documentation
+Check out the [docs](https://nokey.readthedocs.io/en/latest/)
```

### Comparing `nokey-0.0.1/nokey.egg-info/SOURCES.txt` & `nokey-0.1.0/nokey.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -6,26 +6,37 @@
 nokey.egg-info/SOURCES.txt
 nokey.egg-info/dependency_links.txt
 nokey.egg-info/top_level.txt
 nokey/animals/__init__.py
 nokey/animals/dog_api.py
 nokey/country_info/__init__.py
 nokey/country_info/rest_country.py
+nokey/developer_tools/__init__.py
+nokey/developer_tools/url_shortener.py
 nokey/education/__init__.py
 nokey/education/university_names_and_domains.py
 nokey/finance/__init__.py
 nokey/finance/wall_street_bets.py
 nokey/food/__init__.py
 nokey/food/fruityvice.py
+nokey/games/__init__.py
+nokey/games/free_to_game.py
 nokey/geolocation/__init__.py
 nokey/geolocation/ip_api.py
+nokey/geolocation/zippopotamus.py
 nokey/helperFuncs/__init__.py
+nokey/helperFuncs/get_api_list.py
 nokey/helperFuncs/make_request.py
+nokey/helperFuncs/nokey_apis.py
+nokey/inspiration/__init__.py
+nokey/inspiration/dictum.py
 nokey/jokes/__init__.py
 nokey/jokes/joke_api.py
+nokey/language/__init__.py
+nokey/language/free_dictionary.py
 nokey/random/__init__.py
 nokey/random/random_user.py
 nokey/science/__init__.py
 nokey/science/nobel_prize.py
 nokey/spaceflight/__init__.py
 nokey/spaceflight/spaceflight_news.py
 nokey/weather/__init__.py
```

