# Comparing `tmp/data_downloader-1.0.tar.gz` & `tmp/data_downloader-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_downloader-1.0.tar", last modified: Wed Mar 20 08:03:30 2024, max compression
+gzip compressed data, was "data_downloader-1.1.tar", last modified: Sun Apr 14 16:03:45 2024, max compression
```

## Comparing `data_downloader-1.0.tar` & `data_downloader-1.1.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 08:03:30.675216 data_downloader-1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-20 08:03:24.000000 data_downloader-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-03-20 08:03:30.675216 data_downloader-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-03-20 08:03:24.000000 data_downloader-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 08:03:30.675216 data_downloader-1.0/data_downloader/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-20 08:03:24.000000 data_downloader-1.0/data_downloader/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    38258 2024-03-20 08:03:24.000000 data_downloader-1.0/data_downloader/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 08:03:30.675216 data_downloader-1.0/data_downloader/parse_urls/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-20 08:03:24.000000 data_downloader-1.0/data_downloader/parse_urls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-03-20 08:03:24.000000 data_downloader-1.0/data_downloader/parse_urls/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-03-20 08:03:24.000000 data_downloader-1.0/data_downloader/parse_urls/licsar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-03-20 08:03:24.000000 data_downloader-1.0/data_downloader/parse_urls/sentinel_aux.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 08:03:30.675216 data_downloader-1.0/data_downloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-03-20 08:03:30.000000 data_downloader-1.0/data_downloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-20 08:03:30.000000 data_downloader-1.0/data_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 08:03:30.000000 data_downloader-1.0/data_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-20 08:03:30.000000 data_downloader-1.0/data_downloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-20 08:03:30.000000 data_downloader-1.0/data_downloader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 08:03:30.675216 data_downloader-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-20 08:03:24.000000 data_downloader-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:03:45.127789 data_downloader-1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-14 16:03:38.000000 data_downloader-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-14 16:03:45.127789 data_downloader-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-14 16:03:38.000000 data_downloader-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:03:45.123789 data_downloader-1.1/data_downloader/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-14 16:03:38.000000 data_downloader-1.1/data_downloader/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    38294 2024-04-14 16:03:38.000000 data_downloader-1.1/data_downloader/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-04-14 16:03:38.000000 data_downloader-1.1/data_downloader/parse_urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:03:45.123789 data_downloader-1.1/data_downloader/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-14 16:03:38.000000 data_downloader-1.1/data_downloader/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:03:45.127789 data_downloader-1.1/data_downloader/services/hyp3/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-14 16:03:38.000000 data_downloader-1.1/data_downloader/services/hyp3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-14 16:03:38.000000 data_downloader-1.1/data_downloader/services/hyp3/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28108 2024-04-14 16:03:38.000000 data_downloader-1.1/data_downloader/services/hyp3/hyp3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-04-14 16:03:38.000000 data_downloader-1.1/data_downloader/services/licsar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-14 16:03:38.000000 data_downloader-1.1/data_downloader/services/sentinel_aux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:03:45.127789 data_downloader-1.1/data_downloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-14 16:03:45.000000 data_downloader-1.1/data_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-14 16:03:45.000000 data_downloader-1.1/data_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 16:03:45.000000 data_downloader-1.1/data_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-14 16:03:45.000000 data_downloader-1.1/data_downloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-14 16:03:45.000000 data_downloader-1.1/data_downloader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 16:03:45.127789 data_downloader-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-14 16:03:38.000000 data_downloader-1.1/setup.py
```

### Comparing `data_downloader-1.0/LICENSE` & `data_downloader-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `data_downloader-1.0/PKG-INFO` & `data_downloader-1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,58 @@
 Metadata-Version: 2.1
 Name: data_downloader
-Version: 1.0
+Version: 1.1
 Summary: Make downloading scientific data much easier
 Home-page: https://github.com/Fanchengyan/data_downloader
 Author: fanchegyan
 Author-email: fanchy14@lzu.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx>=0.4.0
 Requires-Dist: requests
 Requires-Dist: tqdm
 Requires-Dist: setuptools
 Requires-Dist: beautifulsoup4
 Requires-Dist: nest_asyncio
 Requires-Dist: python-dateutil
 Requires-Dist: browser-cookie3
+Requires-Dist: hyp3_sdk
+Requires-Dist: pandas
+
+<h1 align="center">
+<img src="https://raw.githubusercontent.com/Fanchengyan/data-downloader/master/docs/source/_static/logo/logo.svg" width="300">
+</h1><br>
 
-# data_downloader
 
 [![Downloads](https://static.pepy.tech/badge/data_downloader)](https://pepy.tech/project/data_downloader) [![PyPI](https://img.shields.io/pypi/v/data_downloader)](https://pypi.org/project/data_downloader/) [![Documentation Status](https://readthedocs.org/projects/data-downloader/badge/?version=latest)](https://data-downloader.readthedocs.io/en/latest/?badge=latest)
 
 Make downloading scientific data much easier
 
 ## Introduction
 
-`data_downloader` is a very convenient and powerful data download package for retrieving files using HTTP/HTTPS. It current includes download model `downloader` and url parsing model `parse_urls`. As `httpx` was used which provided a method to access website with synchronous and asynchronous way, you can download multiple files at the same time.
+DataDownloader is a user-friendly package for downloading files using HTTP/HTTPS. It currently includes a `downloader` module for downloading files, a `parse_urls` module for parsing URLs, and a `services` module for managing well-known online services.
 
 ## Highlight Features
 
-data_downloader has several features to make retrieving files easy, including:
+DataDownloader has several features to make retrieving files easy, including:
 
 * **Resumable**: You can resume aborted downloads automatically when you re-execute the code if website support resuming (status code is 216 or 416 when send a HEAD request to the server supplying a Range header)
 * **Asynchronous**: Can download multiple files at the same time when download a single file very slow. 
 * **Convenient**: Provide a easy way to manage your username and password and parse urls from different sources:
-  * **netrc**: Provide a convenient way to manage your username and password via ``.netrc`` file. You don't need to input your username and password every time when you download files from a website which requires authentication. See sections :ref:`netrc` for more details
+  * **netrc**: Provide a convenient way to manage your username and password via ``.netrc`` file, avoiding providing your login information over and over again.
   * **parse_urls**: Provide various methods to parse urls from different sources. See sections :ref:`parse_urls` for more details
+  * **services**: Provide a convenient way to manage well-known online services, currently support: HyP3, LiCSAR, Sentinel-1 orbit. 
 
 ## Installation
 
-You can install `data_downloader` via pip from [PyPI](https://pypi.org/project/data_downloader/):
+You can install `DataDownloader` via pip from [PyPI](https://pypi.org/project/data_downloader/):
 
 ```bash
 pip install data_downloader
 ```
 
 or you can install the latest version from [GitHub](https://github.com/Fanchengyan/data-downloader):
```

### Comparing `data_downloader-1.0/README.md` & `data_downloader-1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-# data_downloader
+<h1 align="center">
+<img src="https://raw.githubusercontent.com/Fanchengyan/data-downloader/master/docs/source/_static/logo/logo.svg" width="300">
+</h1><br>
+
 
 [![Downloads](https://static.pepy.tech/badge/data_downloader)](https://pepy.tech/project/data_downloader) [![PyPI](https://img.shields.io/pypi/v/data_downloader)](https://pypi.org/project/data_downloader/) [![Documentation Status](https://readthedocs.org/projects/data-downloader/badge/?version=latest)](https://data-downloader.readthedocs.io/en/latest/?badge=latest)
 
 Make downloading scientific data much easier
 
 ## Introduction
 
-`data_downloader` is a very convenient and powerful data download package for retrieving files using HTTP/HTTPS. It current includes download model `downloader` and url parsing model `parse_urls`. As `httpx` was used which provided a method to access website with synchronous and asynchronous way, you can download multiple files at the same time.
+DataDownloader is a user-friendly package for downloading files using HTTP/HTTPS. It currently includes a `downloader` module for downloading files, a `parse_urls` module for parsing URLs, and a `services` module for managing well-known online services.
 
 ## Highlight Features
 
-data_downloader has several features to make retrieving files easy, including:
+DataDownloader has several features to make retrieving files easy, including:
 
 * **Resumable**: You can resume aborted downloads automatically when you re-execute the code if website support resuming (status code is 216 or 416 when send a HEAD request to the server supplying a Range header)
 * **Asynchronous**: Can download multiple files at the same time when download a single file very slow. 
 * **Convenient**: Provide a easy way to manage your username and password and parse urls from different sources:
-  * **netrc**: Provide a convenient way to manage your username and password via ``.netrc`` file. You don't need to input your username and password every time when you download files from a website which requires authentication. See sections :ref:`netrc` for more details
+  * **netrc**: Provide a convenient way to manage your username and password via ``.netrc`` file, avoiding providing your login information over and over again.
   * **parse_urls**: Provide various methods to parse urls from different sources. See sections :ref:`parse_urls` for more details
+  * **services**: Provide a convenient way to manage well-known online services, currently support: HyP3, LiCSAR, Sentinel-1 orbit. 
 
 ## Installation
 
-You can install `data_downloader` via pip from [PyPI](https://pypi.org/project/data_downloader/):
+You can install `DataDownloader` via pip from [PyPI](https://pypi.org/project/data_downloader/):
 
 ```bash
 pip install data_downloader
 ```
 
 or you can install the latest version from [GitHub](https://github.com/Fanchengyan/data-downloader):
```

### Comparing `data_downloader-1.0/data_downloader/downloader.py` & `data_downloader-1.1/data_downloader/downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import asyncio
 import datetime as dt
 import multiprocessing as mp
 import os
 import selectors
 import time
 from netrc import netrc
```

### Comparing `data_downloader-1.0/data_downloader/parse_urls/_core.py` & `data_downloader-1.1/data_downloader/parse_urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from pathlib import Path
 from typing import Optional, Union
 from urllib.parse import urljoin
 from xml.dom.minidom import parse
 
 import requests
 from bs4 import BeautifulSoup
@@ -151,15 +153,15 @@
 
 def from_EarthExplorer_order(
     username: Optional[str] = None,
     passwd: Optional[str] = None,
     email: Optional[str] = None,
     order: Optional[Union[str, dict]] = None,
     url_host: Optional[str] = None,
-)->dict:
+) -> dict:
     """parse urls from orders in earthexplorer.
 
     Reference: [bulk-downloader](https://code.usgs.gov/espa/bulk-downloader)
 
     Parameters:
     -----------
     username, passwd: str, optional
```

### Comparing `data_downloader-1.0/data_downloader/parse_urls/licsar.py` & `data_downloader-1.1/data_downloader/services/licsar.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,49 @@
-import os
 import re
 from datetime import datetime
 from pathlib import Path
 import numpy as np
 import pandas as pd
 
-from data_downloader.parse_urls import _core
+from data_downloader import parse_urls
 
 
-class LiCSAR:
-    """class for LiCSAR.
+class LiCSARService:
+    """a class to retrieve LiCSAR data 
 
     Example:
     --------
     >>> from pathlib import Path
     >>> import pandas as pd
-    >>> from data_downloader import LiCSAR, downloader
+    >>> from data_downloader import downloader, services
     >>> # specify the folder to save data
-    >>> home_dir = Path("/Volumes/Data/GeoData/YNG/Sentinel1/LiCSAR/106D_05248_131313/")
+    >>> home_dir = Path("/Volumes/Data/LiCSAR/106D_05248_131313/")
     >>> pair_dir = home_dir / "GEOC"
 
-    init LiCSAR by frame id and download all metadata files
-    
-    >>> licsar = LiCSAR("106D_05248_131313")
+    init LiCSARService by frame id and download all metadata files
+
+    >>> licsar = services.LiCSARService("106D_05248_131313")
     >>> downloader.download_datas(licsar.meta_urls, folder=home_dir, desc="Metadata")
 
     generate mask data by primary_dates, secondary_dates and day span
-    
+
     >>> mask = (licsar.primary_dates>pd.to_datetime("2019-01-01")) & (licsar.primary_dates<pd.to_datetime("2019-12-31")) & (licsar.days < 12 * 5 + 1)
 
     download interferograms and coherence files filtered by mask
-    
+
     >>> downloader.download_datas(licsar.ifg_urls[mask].values, folder=pair_dir, desc="Interferogram")
     >>> downloader.download_datas(licsar.coh_urls[mask], folder=pair_dir, desc="Coherence")
     """
 
     def __init__(
         self,
         frame_id: str,
         root_url: str = "https://gws-access.jasmin.ac.uk/public/nceo_geohazards/LiCSAR_products",
     ):
-        """init LiCSAR.
+        """init LiCSARService.
 
         Parameters:
         -----------
         frame_id : str
             frame id of LiCSAR.
         root_url : str
             root url of LiCSAR. default is "https://gws-access.jasmin.ac.uk/public/nceo_geohazards/LiCSAR_products".
@@ -68,15 +67,15 @@
         """parse track id from frame id."""
         track_id = str(int(self.frame_id[0:3]))
         return track_id
 
     def _retrieve_pairs_urls(self):
         """retrieve pairs of LiCSAR."""
         url = f"{self.home_url}/interferograms/"
-        page_urls = _core.from_html(url, url_depth=1)
+        page_urls = parse_urls.from_html(url, url_depth=1)
         pairs = []
         ifg_urls = []
         coh_urls = []
         for i in page_urls:
             re_result = re.findall(r"\d{8}_\d{8}", i)
             if re_result:
                 pairs.append(re_result[0])
```

### Comparing `data_downloader-1.0/data_downloader/parse_urls/sentinel_aux.py` & `data_downloader-1.1/data_downloader/services/sentinel_aux.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import datetime as dt
 from pathlib import Path
 
 import pandas as pd
 
-from data_downloader import downloader
-from data_downloader.parse_urls import _core
+from data_downloader import parse_urls
 
 
 class SentinelOrbit:
-    """Sentinel-1 orbit data downloader.
+    """a class to retrieve Sentinel-1 orbit data links.
 
-    Examples:
-    ----------
-    >>> from data_downloader import downloader, SentinelOrbit
+    Examples
+    --------
+    >>> from data_downloader import downloader, services
     >>> from pathlib import Path
 
     >>> folder_cal = Path("/media/data/aux_cal")  # specify the folder to save aux_cal
     >>> folder_preorb = Path("/media/data/poeorb")  # specify the folder to save aux_poeorb
 
     init SentinelOrbit:
 
-    >>> s1_orbit = SentinelOrbit()
+    >>> s1_orbit = services.SentinelOrbit()
 
     Get all aux_cal data links of S1A and S1B and download them:
 
     >>> urls_cal = s1_orbit.cal_urls(platform='all')
     >>> downloader.async_download_datas(urls_cal, folder=folder_cal)
 
     Get all precise orbit data links of S1A during 20210101-20220301 and download them:
@@ -38,33 +37,33 @@
     def __init__(
         self,
         home_aux_cal: str = "https://s1qc.asf.alaska.edu/aux_cal/",
         home_preorb: str = "https://s1qc.asf.alaska.edu/aux_poeorb/",
     ) -> None:
         """init SentinelOrbit.
 
-        Parameters:
-        -----------
+        Parameters
+        ----------
         home_aux_cal : str
             home url of aux_cal, default is "https://s1qc.asf.alaska.edu/aux_cal/".
         home_preorb : str
             home url of aux_poeorb, default is "https://s1qc.asf.alaska.edu/aux_poeorb/".
         """
         self.home_aux_cal = home_aux_cal
         self.home_preorb = home_preorb
 
     def cal_urls(self, platform="all"):
         """filter files from urls of aux_cal by platform.
 
-        Parameters:
-        -----------
+        Parameters
+        ----------
         platform : str, one of ['S1A', 'S1B','all']
             platform of satellite. should be one of ['S1A', 'S1B','all']
         """
-        urls = _core.from_html(self.home_aux_cal)
+        urls = parse_urls.from_html(self.home_aux_cal)
         if platform in ["S1A", "S1B", "all"]:
             if platform == "all":
                 platform = ["S1A", "S1B"]
             else:
                 platform = [platform]
         else:
             raise ValueError("platform must be one of ['S1A', 'S1B','all']")
@@ -78,16 +77,16 @@
         self,
         date_start: str,
         date_end: str,
         platform: str = "all",
     ):
         """filter files from urls of aux_poeorb (precise orbit) by date and platform.
 
-        Parameters:
-        -----------
+        Parameters
+        ----------
         date_start, date_end : str
             start/end date to filter, can be any format that can be converted by
             pd.to_datetime (e.g. '20210101', '2021-01-01', '2021/01/01').
         platform : str, one of ['S1A', 'S1B','all']
             platform of satellite. should be one of ['S1A', 'S1B','all']
         """
         if platform in ["S1A", "S1B", "all"]:
@@ -97,15 +96,15 @@
                 platform = [platform]
         else:
             raise ValueError("platform must be one of ['S1A', 'S1B','all']")
 
         date_start = pd.to_datetime(date_start).date()
         date_end = pd.to_datetime(date_end).date()
 
-        urls = _core.from_html(self.home_preorb)
+        urls = parse_urls.from_html(self.home_preorb)
         _urls = [i for i in urls if Path(i).suffix == ".EOF"]
         urls_filter = []
         for i in _urls:
             name = Path(i).stem
             dt_i = pd.to_datetime(name.split("_")[-1]).date() - dt.timedelta(days=1)
 
             if name[:3] in platform and date_start <= dt_i <= date_end:
```

### Comparing `data_downloader-1.0/data_downloader.egg-info/PKG-INFO` & `data_downloader-1.1/data_downloader.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,58 @@
 Metadata-Version: 2.1
 Name: data_downloader
-Version: 1.0
+Version: 1.1
 Summary: Make downloading scientific data much easier
 Home-page: https://github.com/Fanchengyan/data_downloader
 Author: fanchegyan
 Author-email: fanchy14@lzu.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx>=0.4.0
 Requires-Dist: requests
 Requires-Dist: tqdm
 Requires-Dist: setuptools
 Requires-Dist: beautifulsoup4
 Requires-Dist: nest_asyncio
 Requires-Dist: python-dateutil
 Requires-Dist: browser-cookie3
+Requires-Dist: hyp3_sdk
+Requires-Dist: pandas
+
+<h1 align="center">
+<img src="https://raw.githubusercontent.com/Fanchengyan/data-downloader/master/docs/source/_static/logo/logo.svg" width="300">
+</h1><br>
 
-# data_downloader
 
 [![Downloads](https://static.pepy.tech/badge/data_downloader)](https://pepy.tech/project/data_downloader) [![PyPI](https://img.shields.io/pypi/v/data_downloader)](https://pypi.org/project/data_downloader/) [![Documentation Status](https://readthedocs.org/projects/data-downloader/badge/?version=latest)](https://data-downloader.readthedocs.io/en/latest/?badge=latest)
 
 Make downloading scientific data much easier
 
 ## Introduction
 
-`data_downloader` is a very convenient and powerful data download package for retrieving files using HTTP/HTTPS. It current includes download model `downloader` and url parsing model `parse_urls`. As `httpx` was used which provided a method to access website with synchronous and asynchronous way, you can download multiple files at the same time.
+DataDownloader is a user-friendly package for downloading files using HTTP/HTTPS. It currently includes a `downloader` module for downloading files, a `parse_urls` module for parsing URLs, and a `services` module for managing well-known online services.
 
 ## Highlight Features
 
-data_downloader has several features to make retrieving files easy, including:
+DataDownloader has several features to make retrieving files easy, including:
 
 * **Resumable**: You can resume aborted downloads automatically when you re-execute the code if website support resuming (status code is 216 or 416 when send a HEAD request to the server supplying a Range header)
 * **Asynchronous**: Can download multiple files at the same time when download a single file very slow. 
 * **Convenient**: Provide a easy way to manage your username and password and parse urls from different sources:
-  * **netrc**: Provide a convenient way to manage your username and password via ``.netrc`` file. You don't need to input your username and password every time when you download files from a website which requires authentication. See sections :ref:`netrc` for more details
+  * **netrc**: Provide a convenient way to manage your username and password via ``.netrc`` file, avoiding providing your login information over and over again.
   * **parse_urls**: Provide various methods to parse urls from different sources. See sections :ref:`parse_urls` for more details
+  * **services**: Provide a convenient way to manage well-known online services, currently support: HyP3, LiCSAR, Sentinel-1 orbit. 
 
 ## Installation
 
-You can install `data_downloader` via pip from [PyPI](https://pypi.org/project/data_downloader/):
+You can install `DataDownloader` via pip from [PyPI](https://pypi.org/project/data_downloader/):
 
 ```bash
 pip install data_downloader
 ```
 
 or you can install the latest version from [GitHub](https://github.com/Fanchengyan/data-downloader):
```

### Comparing `data_downloader-1.0/setup.py` & `data_downloader-1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="UTF-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="data_downloader",
-    version="1.0",
+    version="1.1",
     author="fanchegyan",
     author_email="fanchy14@lzu.edu.cn",
     description="Make downloading scientific data much easier",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Fanchengyan/data_downloader",
     packages=setuptools.find_packages(),
@@ -18,15 +18,17 @@
         "requests",
         "tqdm",
         "setuptools",
         "beautifulsoup4",
         "nest_asyncio",
         "python-dateutil",
         "browser-cookie3",
+        "hyp3_sdk",
+        "pandas",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.8",
 )
```

