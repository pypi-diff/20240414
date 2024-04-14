# Comparing `tmp/tweeterpy-1.0.8.tar.gz` & `tmp/tweeterpy-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweeterpy-1.0.8.tar", last modified: Fri Oct  6 14:43:34 2023, max compression
+gzip compressed data, was "tweeterpy-1.0.9.tar", last modified: Wed Oct 11 13:51:43 2023, max compression
```

## Comparing `tweeterpy-1.0.8.tar` & `tweeterpy-1.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-10-06 14:43:34.182606 tweeterpy-1.0.8/
--rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 tweeterpy-1.0.8/LICENSE
--rw-rw-rw-   0        0        0       22 2023-06-20 15:06:14.000000 tweeterpy-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     3554 2023-10-06 14:43:34.182606 tweeterpy-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2501 2023-09-16 13:05:25.000000 tweeterpy-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-10-06 14:43:34.182606 tweeterpy-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1499 2023-10-06 14:42:56.000000 tweeterpy-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-10-06 14:43:34.151355 tweeterpy-1.0.8/tweeterpy/
--rw-rw-rw-   0        0        0       34 2023-09-16 06:13:29.000000 tweeterpy-1.0.8/tweeterpy/__init__.py
--rw-rw-rw-   0        0        0     6824 2023-09-09 11:53:49.000000 tweeterpy-1.0.8/tweeterpy/api_util.py
--rw-rw-rw-   0        0        0     2413 2023-09-19 17:16:32.000000 tweeterpy-1.0.8/tweeterpy/config.py
--rw-rw-rw-   0        0        0     3770 2023-09-17 11:41:01.000000 tweeterpy-1.0.8/tweeterpy/constants.py
--rw-rw-rw-   0        0        0     2058 2023-09-09 11:19:04.000000 tweeterpy-1.0.8/tweeterpy/logging_util.py
--rw-rw-rw-   0        0        0     9018 2023-10-06 14:34:31.000000 tweeterpy-1.0.8/tweeterpy/login_util.py
--rw-rw-rw-   0        0        0     1984 2023-09-09 10:43:43.000000 tweeterpy-1.0.8/tweeterpy/request_util.py
--rw-rw-rw-   0        0        0     2481 2023-09-07 09:39:56.000000 tweeterpy-1.0.8/tweeterpy/session_util.py
--rw-rw-rw-   0        0        0    26988 2023-10-06 14:34:05.000000 tweeterpy-1.0.8/tweeterpy/tweeterpy.py
--rw-rw-rw-   0        0        0    13542 2023-10-06 14:35:51.000000 tweeterpy-1.0.8/tweeterpy/util.py
-drwxrwxrwx   0        0        0        0 2023-10-06 14:43:34.182606 tweeterpy-1.0.8/tweeterpy.egg-info/
--rw-rw-rw-   0        0        0     3554 2023-10-06 14:43:34.000000 tweeterpy-1.0.8/tweeterpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2023-10-06 14:43:34.000000 tweeterpy-1.0.8/tweeterpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-06 14:43:34.000000 tweeterpy-1.0.8/tweeterpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      192 2023-10-06 14:43:34.000000 tweeterpy-1.0.8/tweeterpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-10-06 14:43:34.000000 tweeterpy-1.0.8/tweeterpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-10-11 13:51:43.393494 tweeterpy-1.0.9/
+-rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 tweeterpy-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0       22 2023-06-20 15:06:14.000000 tweeterpy-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3583 2023-10-11 13:51:43.393494 tweeterpy-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2530 2023-10-11 13:44:39.000000 tweeterpy-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-10-11 13:51:43.393494 tweeterpy-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1499 2023-10-11 13:45:33.000000 tweeterpy-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-10-11 13:51:43.346596 tweeterpy-1.0.9/tweeterpy/
+-rw-rw-rw-   0        0        0       34 2023-09-16 06:13:29.000000 tweeterpy-1.0.9/tweeterpy/__init__.py
+-rw-rw-rw-   0        0        0     6968 2023-10-11 13:29:25.000000 tweeterpy-1.0.9/tweeterpy/api_util.py
+-rw-rw-rw-   0        0        0     2505 2023-10-11 13:49:03.000000 tweeterpy-1.0.9/tweeterpy/config.py
+-rw-rw-rw-   0        0        0     3770 2023-09-17 11:41:01.000000 tweeterpy-1.0.9/tweeterpy/constants.py
+-rw-rw-rw-   0        0        0     2058 2023-09-09 11:19:04.000000 tweeterpy-1.0.9/tweeterpy/logging_util.py
+-rw-rw-rw-   0        0        0     9024 2023-10-10 14:44:59.000000 tweeterpy-1.0.9/tweeterpy/login_util.py
+-rw-rw-rw-   0        0        0     1984 2023-09-09 10:43:43.000000 tweeterpy-1.0.9/tweeterpy/request_util.py
+-rw-rw-rw-   0        0        0     2481 2023-09-07 09:39:56.000000 tweeterpy-1.0.9/tweeterpy/session_util.py
+-rw-rw-rw-   0        0        0    27780 2023-10-11 13:34:59.000000 tweeterpy-1.0.9/tweeterpy/tweeterpy.py
+-rw-rw-rw-   0        0        0    13673 2023-10-07 13:59:32.000000 tweeterpy-1.0.9/tweeterpy/util.py
+drwxrwxrwx   0        0        0        0 2023-10-11 13:51:43.377875 tweeterpy-1.0.9/tweeterpy.egg-info/
+-rw-rw-rw-   0        0        0     3583 2023-10-11 13:51:43.000000 tweeterpy-1.0.9/tweeterpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2023-10-11 13:51:43.000000 tweeterpy-1.0.9/tweeterpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-10-11 13:51:43.000000 tweeterpy-1.0.9/tweeterpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      192 2023-10-11 13:51:43.000000 tweeterpy-1.0.9/tweeterpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-10-11 13:51:43.000000 tweeterpy-1.0.9/tweeterpy.egg-info/top_level.txt
```

### Comparing `tweeterpy-1.0.8/LICENSE` & `tweeterpy-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.0.8/PKG-INFO` & `tweeterpy-1.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweeterpy
-Version: 1.0.8
+Version: 1.0.9
 Summary: TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc.
 Home-page: https://github.com/iSarabjitDhiman/TweeterPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data extraction,twitter api,twitter python,tweet api,tweetpy
 Classifier: Development Status :: 3 - Alpha
@@ -26,15 +26,14 @@
 <a href="https://choosealicense.com/licenses/mit/"> <img src="https://img.shields.io/badge/License-MIT-green.svg"></a>
 <a href="https://www.python.org/"><img src="https://img.shields.io/pypi/pyversions/tweeterpy"></a>
 <a href="https://pypi.org/project/tweeterpy/"> <img src="https://img.shields.io/pypi/v/tweeterpy"></a>
 <a href="https://github.com/iSarabjitDhiman/TweeterPy/commits"> <img src="https://img.shields.io/github/last-commit/iSarabjitDhiman/TweeterPy"></a>
 <a href="https://discord.gg/pHY6CU5Ke4"> <img alt="Discord" src="https://img.shields.io/discord/1149281691479851018?style=flat&logo=discord&logoColor=white"></a>
 <a href="https://twitter.com/isarabjitdhiman"> <img src="https://img.shields.io/twitter/follow/iSarabjitDhiman?style=social"></a>
 
-
 ## Overview
 
 TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc.
 
 > _Note_ : `Use it on Your Own Risk. Scraping with Residential proxies is advisable while extracting data at scale/in bulk. If possible, use multiple accounts to fetch data from Twitter.` **_DON'T USE YOUR PERSONAL ACCOUNT FOR SCRAPING PURPOSES._**
 
 ## Installation
@@ -81,28 +80,29 @@
 > ### Example - Config Usage
 
 ```python
 from tweeterpy import config
 
 config.PROXY = {"http":"127.0.0.1","https":"127.0.0.1"}
 config.TIMEOUT = 10
+config.UPDATE_API = False
 
 ```
 
 Check out configuration docs for the available settings.
 
 [Configurations](docs/config.md)
 
 ## Features
 
 - Extracts Tweets
 - Extracts User's Followers
 - Extracts User's Followings
 - Extracts User's Profile Details
-- Extracts Twitter Profile Media and so on.
+- Extracts Twitter Profile Media and much more.
 
 ## Authors
 
 - [@iSarabjitDhiman](https://www.github.com/iSarabjitDhiman)
 
 ## Feedback
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tweeterpy Version: 1.0.8 Summary: TweeterPy is a
+Metadata-Version: 2.1 Name: tweeterpy Version: 1.0.9 Summary: TweeterPy is a
 python library to extract data from Twitter. TweeterPy API lets you scrape data
 from a user's profile like username, userid, bio, followers/followings list,
 profile media, tweets, etc. Home-page: https://github.com/iSarabjitDhiman/
 TweeterPy Author: Sarabjit Dhiman Author-email: hello@sarabjitdhiman.com
 License: MIT Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data
 extraction,twitter api,twitter python,tweet api,tweetpy Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: End Users/Desktop
@@ -26,15 +26,15 @@
    Install TweeterPy with pip ```python pip install tweeterpy ``` ## Usage/
  Examples ```python python quickstart.py ``` OR ```python from twitter import
 TweeterPy TweeterPy() ``` > ### Example - Get User ID of a User. ```python from
   tweeterpy import TweeterPy twitter = TweeterPy() print(twitter.get_user_id
        ('elonmusk')) ``` ## Documentation Check out step by step guide.
   [Documentation](docs/docs.md) ## Configuration > ### Example - Config Usage
         ```python from tweeterpy import config config.PROXY = {"http":
-      "127.0.0.1","https":"127.0.0.1"} config.TIMEOUT = 10 ``` Check out
-configuration docs for the available settings. [Configurations](docs/config.md)
-  ## Features - Extracts Tweets - Extracts User's Followers - Extracts User's
- Followings - Extracts User's Profile Details - Extracts Twitter Profile Media
-      and so on. ## Authors - [@iSarabjitDhiman](https://www.github.com/
- iSarabjitDhiman) ## Feedback If you have any feedback, please reach out to us
- at hello@sarabjitdhiman.com or contact me on Social Media @iSarabjitDhiman ##
-              Support For support, email hello@sarabjitdhiman.com
+"127.0.0.1","https":"127.0.0.1"} config.TIMEOUT = 10 config.UPDATE_API = False
+ ``` Check out configuration docs for the available settings. [Configurations]
+ (docs/config.md) ## Features - Extracts Tweets - Extracts User's Followers -
+Extracts User's Followings - Extracts User's Profile Details - Extracts Twitter
+     Profile Media and much more. ## Authors - [@iSarabjitDhiman](https://
+ www.github.com/iSarabjitDhiman) ## Feedback If you have any feedback, please
+   reach out to us at hello@sarabjitdhiman.com or contact me on Social Media
+    @iSarabjitDhiman ## Support For support, email hello@sarabjitdhiman.com
```

### Comparing `tweeterpy-1.0.8/README.md` & `tweeterpy-1.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 <a href="https://choosealicense.com/licenses/mit/"> <img src="https://img.shields.io/badge/License-MIT-green.svg"></a>
 <a href="https://www.python.org/"><img src="https://img.shields.io/pypi/pyversions/tweeterpy"></a>
 <a href="https://pypi.org/project/tweeterpy/"> <img src="https://img.shields.io/pypi/v/tweeterpy"></a>
 <a href="https://github.com/iSarabjitDhiman/TweeterPy/commits"> <img src="https://img.shields.io/github/last-commit/iSarabjitDhiman/TweeterPy"></a>
 <a href="https://discord.gg/pHY6CU5Ke4"> <img alt="Discord" src="https://img.shields.io/discord/1149281691479851018?style=flat&logo=discord&logoColor=white"></a>
 <a href="https://twitter.com/isarabjitdhiman"> <img src="https://img.shields.io/twitter/follow/iSarabjitDhiman?style=social"></a>
 
-
 ## Overview
 
 TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc.
 
 > _Note_ : `Use it on Your Own Risk. Scraping with Residential proxies is advisable while extracting data at scale/in bulk. If possible, use multiple accounts to fetch data from Twitter.` **_DON'T USE YOUR PERSONAL ACCOUNT FOR SCRAPING PURPOSES._**
 
 ## Installation
@@ -59,28 +58,29 @@
 > ### Example - Config Usage
 
 ```python
 from tweeterpy import config
 
 config.PROXY = {"http":"127.0.0.1","https":"127.0.0.1"}
 config.TIMEOUT = 10
+config.UPDATE_API = False
 
 ```
 
 Check out configuration docs for the available settings.
 
 [Configurations](docs/config.md)
 
 ## Features
 
 - Extracts Tweets
 - Extracts User's Followers
 - Extracts User's Followings
 - Extracts User's Profile Details
-- Extracts Twitter Profile Media and so on.
+- Extracts Twitter Profile Media and much more.
 
 ## Authors
 
 - [@iSarabjitDhiman](https://www.github.com/iSarabjitDhiman)
 
 ## Feedback
```

#### html2text {}

```diff
@@ -12,15 +12,15 @@
    Install TweeterPy with pip ```python pip install tweeterpy ``` ## Usage/
  Examples ```python python quickstart.py ``` OR ```python from twitter import
 TweeterPy TweeterPy() ``` > ### Example - Get User ID of a User. ```python from
   tweeterpy import TweeterPy twitter = TweeterPy() print(twitter.get_user_id
        ('elonmusk')) ``` ## Documentation Check out step by step guide.
   [Documentation](docs/docs.md) ## Configuration > ### Example - Config Usage
         ```python from tweeterpy import config config.PROXY = {"http":
-      "127.0.0.1","https":"127.0.0.1"} config.TIMEOUT = 10 ``` Check out
-configuration docs for the available settings. [Configurations](docs/config.md)
-  ## Features - Extracts Tweets - Extracts User's Followers - Extracts User's
- Followings - Extracts User's Profile Details - Extracts Twitter Profile Media
-      and so on. ## Authors - [@iSarabjitDhiman](https://www.github.com/
- iSarabjitDhiman) ## Feedback If you have any feedback, please reach out to us
- at hello@sarabjitdhiman.com or contact me on Social Media @iSarabjitDhiman ##
-              Support For support, email hello@sarabjitdhiman.com
+"127.0.0.1","https":"127.0.0.1"} config.TIMEOUT = 10 config.UPDATE_API = False
+ ``` Check out configuration docs for the available settings. [Configurations]
+ (docs/config.md) ## Features - Extracts Tweets - Extracts User's Followers -
+Extracts User's Followings - Extracts User's Profile Details - Extracts Twitter
+     Profile Media and much more. ## Authors - [@iSarabjitDhiman](https://
+ www.github.com/iSarabjitDhiman) ## Feedback If you have any feedback, please
+   reach out to us at hello@sarabjitdhiman.com or contact me on Social Media
+    @iSarabjitDhiman ## Support For support, email hello@sarabjitdhiman.com
```

### Comparing `tweeterpy-1.0.8/setup.py` & `tweeterpy-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "1.0.8"
+VERSION = "1.0.9"
 SHORT_DESCRIPTION = "TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc."
 
 with open("requirements.txt") as file:
     dependencies = file.read().splitlines()
 with open("README.md", "r") as file:
     DESCRIPTION = file.read()
```

### Comparing `tweeterpy-1.0.8/tweeterpy/api_util.py` & `tweeterpy-1.0.9/tweeterpy/api_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,26 +19,28 @@
 
 
 class ApiUpdater:
     """
         Twitter updates its API quite frequently. Therefore, ApiUpdater checks for the latest updates and modifies the api_endpoints, feature_switches, path etc in constants.py
     """
 
-    def __init__(self):
+    def __init__(self, update_api=True):
         try:
             logger.debug('Updating API...')
             # fmt: off - Turns off formatting for this block of code.
             try:
+                if not update_api:
+                    raise Exception("Skipping API Updates.")
                 page_source = self._get_home_page_source()
                 api_file_url = self._get_api_file_url(page_source)
                 feature_switches = self._get_feature_switches(page_source)
                 api_endpoints_data = self._js_to_py_dict(self._get_api_file_content(api_file_url))
                 self._save_api_data(feature_switches,api_endpoints_data)
-            except:
-                logger.warn("Couldnt get the latest API data.")
+            except Exception as error:
+                logger.warn(f"{error} Couldn't get the latest API data.")
                 logger.debug("Trying to restore API data from the backup file.")
                 feature_switches, api_endpoints_data = self._load_api_data()
             current_api_endpoints = self._get_current_api_endpoints()
             new_api_endpoints = self._map_data(current_api_endpoints, api_endpoints_data)
             self._update_api_endpoints(new_api_endpoints)
             self._update_feature_switches(feature_switches)
             logger.info("API Updated Successfully.")
```

### Comparing `tweeterpy-1.0.8/tweeterpy/config.py` & `tweeterpy-1.0.9/tweeterpy/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,10 +66,12 @@
         '__main__': {  # if __name__ == '__main__'
             'handlers': ['stream', 'file'],
             'level': LOG_LEVEL or 'DEBUG',
         }
     }
 }
 
+# Disable/Enable Api Update which occurs at the startup Initialization.
+UPDATE_API = True
 
 if __name__ == "__main__":
     pass
```

### Comparing `tweeterpy-1.0.8/tweeterpy/constants.py` & `tweeterpy-1.0.9/tweeterpy/constants.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.0.8/tweeterpy/logging_util.py` & `tweeterpy-1.0.9/tweeterpy/logging_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.0.8/tweeterpy/login_util.py` & `tweeterpy-1.0.9/tweeterpy/login_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         task_flow_mapper = {"LoginJsInstrumentationSubtask":{"task_executor": self._get_user_flow_token,"task_parameter":None},
                             "LoginEnterUserIdentifierSSO":{"task_executor": self._get_password_flow_token,"task_parameter":username},
                             "LoginEnterAlternateIdentifierSubtask":{"task_executor": self._handle_suspicious_login,"task_parameter":verification_input_data},
                             "LoginEnterPassword":{"task_executor": self._get_account_duplication_flow_token,"task_parameter":password},
                             "DenyLoginSubtask":{"task_executor": self._check_suspicious_login,"task_parameter":None},
                             "AccountDuplicationCheck":{"task_executor": self._check_account_duplication,"task_parameter":None},
                             "LoginAcid":{"task_executor":self._handle_suspicious_login,"task_parameter":verification_input_data},
-                            "LoginSuccessSubtask":{"task_output": "\nSuccessfully Logged In.."}}
+                            "LoginSuccessSubtask":{"task_output": "\nPlease Wait... Logging In...\n"}}
         return task_flow_mapper
 
     def _get_flow_token(self):
         params = {'flow_name': 'login'}
         payload = {'input_flow_data': {
             'flow_context': {'debug_overrides': {}, 'start_location': {'location': 'manual_link'}, }, },
             'subtask_versions': {'action_list': 2, 'alert_dialog': 1, 'app_download_cta': 1, 'check_logged_in_account': 1,
```

### Comparing `tweeterpy-1.0.8/tweeterpy/request_util.py` & `tweeterpy-1.0.9/tweeterpy/request_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.0.8/tweeterpy/session_util.py` & `tweeterpy-1.0.9/tweeterpy/session_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.0.8/tweeterpy/tweeterpy.py` & `tweeterpy-1.0.9/tweeterpy/tweeterpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,20 +24,22 @@
         if config.DISABLE_LOGS or config.DISABLE_EXTERNAL_LOGS:
             logger.debug("Disabling logs...")
             config.LOG_LEVEL = "ERROR" if config.DISABLE_LOGS else config.LOG_LEVEL
             disable_external_only = config.DISABLE_EXTERNAL_LOGS if not config.DISABLE_LOGS else False
             set_log_level(logging.ERROR, external_only=disable_external_only)
         self.generate_session()
         # update api endpoints
-        ApiUpdater()
+        ApiUpdater(update_api=config.UPDATE_API)
 
     def _generate_request_data(self, endpoint, variables=None, **kwargs):
         # fmt: off - Turns off formatting for this block of code. Just for the readability purpose.
         url = util.generate_url(domain=Path.API_URL, url_path=endpoint)
-        query_params = {"variables": json.dumps({**variables})}
+        query_params = {}
+        if variables:
+            query_params["variables"] = json.dumps(variables)
         if kwargs:
             features = FeatureSwitch().get_query_features(endpoint) or util.generate_features(**kwargs)
             query_params["features"] = json.dumps(features)
         # fmt: on   
         request_payload = {"url": url, "params": query_params}
         logger.debug(f"Request Payload => {request_payload}")
         return request_payload
@@ -107,19 +109,19 @@
     @property
     def me(self):
         """Returns logged in user information.
 
         Returns:
             dict: Currently logged in user's data.
         """
-        url = util.generate_url(url_path=Path.VIEWER_ENDPOINT)
-        query = {"variables": json.dumps({"withCommunitiesMemberships": True,
-                                          "withSubscribedTab": True, "withCommunitiesCreation": True}),
-                 "features": json.dumps(util.generate_features(user_data_features=True))}
-        response = self.session.get(url, params=query)
+        variables = {"withCommunitiesMemberships": True,
+                     "withSubscribedTab": True, "withCommunitiesCreation": True}
+        request_payload = self._generate_request_data(
+            Path.VIEWER_ENDPOINT, variables, user_data_features=True)
+        response = self.session.get(**request_payload)
         try:
             return response.json()
         except:
             logger.info("Guest Session")
             return
 
     def login_decorator(original_function):
@@ -136,14 +138,15 @@
         Args:
             auth_token (str, optional): Generate session with an auth-token. If auth_token is None (Default Behaviour), generates a guest session without login. Defaults to None.
 
         Returns:
             requests.Session: requests.Session Object.
         """
         try:
+            logger.debug("Trying to generate a new session.")
             self.session = requests.Session()
             if config.PROXY is not None:
                 self.session.proxies = config.PROXY
                 self.session.verify = False
             self.session.headers.update(util.generate_headers())
             make_request(Path.BASE_URL, session=self.session)
             guest_token = make_request(
@@ -152,14 +155,15 @@
             self.session.cookies.update({'gt': guest_token})
             if auth_token:
                 self.session.cookies.update({'auth_token': auth_token})
                 util.generate_headers(self.session)
         except Exception as error:
             logger.exception(f"Couldn't generate a new session.\n{error}\n")
             raise
+        logger.debug("Session has been generated.")
         return self.session
 
     def save_session(self, session=None, session_name=None):
         """Save a logged in session to avoid frequent logins in future.
 
         Args:
             session (requests.Session, optional): requests.Session object you want to save. If None, saves current session by default. Defaults to None. 
@@ -202,20 +206,33 @@
     def login(self, username=None, password=None):
         """Log into an account.
 
         Args:
             username (str, optional): Twitter username or email. Defaults to None.
             password (str, optional): Password. Defaults to None.
         """
+        if "auth_token" in self.session.cookies.keys():
+            self.generate_session()
         if username is None:
             username = str(input("Enter Your Username or Email : ")).strip()
         if password is None:
             password = getpass.getpass()
         TaskHandler().login(username, password)
         util.generate_headers(session=self.session)
+        try:
+            user = self.me
+            username = util.find_nested_key(user, 'screen_name')
+            account_locked = util.find_nested_key(user, 'bounce_location')
+            if account_locked and not username:
+                raise Exception(
+                    "Account logged in but couldn't get the user's details ! Make sure, the given account is working. (Ignore if its working)")
+            if username:
+                print(f"Welcome {username} : Successfully Logged In.")
+        except Exception as error:
+            logger.warn(error)
 
     def get_user_id(self, username):
         """Get user ID of a twitter user.
 
         Args:
             username (str): Twitter username.
```

### Comparing `tweeterpy-1.0.8/tweeterpy/util.py` & `tweeterpy-1.0.9/tweeterpy/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,19 @@
                "User-Agent": config._USER_AGENT,
                "X-Twitter-Active-User": "yes",
                "X-Twitter-Client-Language": "en"
                }
     if session:
         if "auth_token" in session.cookies.keys():
             session.get(Path.BASE_URL)
-            session.headers.update(
-                {"X-Csrf-Token": session.cookies.get("ct0", None), "X-Twitter-Auth-Type": "OAuth2Session"})
+            csrf_token = session.cookies.get("ct0", None)
+            auth_headers = {"X-Csrf-Token": csrf_token,
+                            "X-Twitter-Auth-Type": "OAuth2Session"}
+            session.headers.update(auth_headers)
+            headers.update(auth_headers)
     return headers
 
 
 def generate_features(default_features=True, user_data_features=False, user_info_feautres=False, additional_features=False):
     features = {}
     if default_features:
         default_features = {"responsive_web_graphql_exclude_directive_enabled": True, "verified_phone_label_enabled": True,
```

### Comparing `tweeterpy-1.0.8/tweeterpy.egg-info/PKG-INFO` & `tweeterpy-1.0.9/tweeterpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweeterpy
-Version: 1.0.8
+Version: 1.0.9
 Summary: TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc.
 Home-page: https://github.com/iSarabjitDhiman/TweeterPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data extraction,twitter api,twitter python,tweet api,tweetpy
 Classifier: Development Status :: 3 - Alpha
@@ -26,15 +26,14 @@
 <a href="https://choosealicense.com/licenses/mit/"> <img src="https://img.shields.io/badge/License-MIT-green.svg"></a>
 <a href="https://www.python.org/"><img src="https://img.shields.io/pypi/pyversions/tweeterpy"></a>
 <a href="https://pypi.org/project/tweeterpy/"> <img src="https://img.shields.io/pypi/v/tweeterpy"></a>
 <a href="https://github.com/iSarabjitDhiman/TweeterPy/commits"> <img src="https://img.shields.io/github/last-commit/iSarabjitDhiman/TweeterPy"></a>
 <a href="https://discord.gg/pHY6CU5Ke4"> <img alt="Discord" src="https://img.shields.io/discord/1149281691479851018?style=flat&logo=discord&logoColor=white"></a>
 <a href="https://twitter.com/isarabjitdhiman"> <img src="https://img.shields.io/twitter/follow/iSarabjitDhiman?style=social"></a>
 
-
 ## Overview
 
 TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc.
 
 > _Note_ : `Use it on Your Own Risk. Scraping with Residential proxies is advisable while extracting data at scale/in bulk. If possible, use multiple accounts to fetch data from Twitter.` **_DON'T USE YOUR PERSONAL ACCOUNT FOR SCRAPING PURPOSES._**
 
 ## Installation
@@ -81,28 +80,29 @@
 > ### Example - Config Usage
 
 ```python
 from tweeterpy import config
 
 config.PROXY = {"http":"127.0.0.1","https":"127.0.0.1"}
 config.TIMEOUT = 10
+config.UPDATE_API = False
 
 ```
 
 Check out configuration docs for the available settings.
 
 [Configurations](docs/config.md)
 
 ## Features
 
 - Extracts Tweets
 - Extracts User's Followers
 - Extracts User's Followings
 - Extracts User's Profile Details
-- Extracts Twitter Profile Media and so on.
+- Extracts Twitter Profile Media and much more.
 
 ## Authors
 
 - [@iSarabjitDhiman](https://www.github.com/iSarabjitDhiman)
 
 ## Feedback
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tweeterpy Version: 1.0.8 Summary: TweeterPy is a
+Metadata-Version: 2.1 Name: tweeterpy Version: 1.0.9 Summary: TweeterPy is a
 python library to extract data from Twitter. TweeterPy API lets you scrape data
 from a user's profile like username, userid, bio, followers/followings list,
 profile media, tweets, etc. Home-page: https://github.com/iSarabjitDhiman/
 TweeterPy Author: Sarabjit Dhiman Author-email: hello@sarabjitdhiman.com
 License: MIT Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data
 extraction,twitter api,twitter python,tweet api,tweetpy Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: End Users/Desktop
@@ -26,15 +26,15 @@
    Install TweeterPy with pip ```python pip install tweeterpy ``` ## Usage/
  Examples ```python python quickstart.py ``` OR ```python from twitter import
 TweeterPy TweeterPy() ``` > ### Example - Get User ID of a User. ```python from
   tweeterpy import TweeterPy twitter = TweeterPy() print(twitter.get_user_id
        ('elonmusk')) ``` ## Documentation Check out step by step guide.
   [Documentation](docs/docs.md) ## Configuration > ### Example - Config Usage
         ```python from tweeterpy import config config.PROXY = {"http":
-      "127.0.0.1","https":"127.0.0.1"} config.TIMEOUT = 10 ``` Check out
-configuration docs for the available settings. [Configurations](docs/config.md)
-  ## Features - Extracts Tweets - Extracts User's Followers - Extracts User's
- Followings - Extracts User's Profile Details - Extracts Twitter Profile Media
-      and so on. ## Authors - [@iSarabjitDhiman](https://www.github.com/
- iSarabjitDhiman) ## Feedback If you have any feedback, please reach out to us
- at hello@sarabjitdhiman.com or contact me on Social Media @iSarabjitDhiman ##
-              Support For support, email hello@sarabjitdhiman.com
+"127.0.0.1","https":"127.0.0.1"} config.TIMEOUT = 10 config.UPDATE_API = False
+ ``` Check out configuration docs for the available settings. [Configurations]
+ (docs/config.md) ## Features - Extracts Tweets - Extracts User's Followers -
+Extracts User's Followings - Extracts User's Profile Details - Extracts Twitter
+     Profile Media and much more. ## Authors - [@iSarabjitDhiman](https://
+ www.github.com/iSarabjitDhiman) ## Feedback If you have any feedback, please
+   reach out to us at hello@sarabjitdhiman.com or contact me on Social Media
+    @iSarabjitDhiman ## Support For support, email hello@sarabjitdhiman.com
```

