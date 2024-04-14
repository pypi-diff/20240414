# Comparing `tmp/pkscreener-0.44.20240413.258.tar.gz` & `tmp/pkscreener-0.44.20240413.259.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240413.258.tar", last modified: Sat Apr 13 08:30:04 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240413.259.tar", last modified: Sat Apr 13 22:52:24 2024, max compression
```

## Comparing `pkscreener-0.44.20240413.258.tar` & `pkscreener-0.44.20240413.259.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 08:30:04.852229 pkscreener-0.44.20240413.258/
--rw-rw-rw-   0        0        0     1086 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-13 08:30:04.852229 pkscreener-0.44.20240413.258/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/README.md
-drwxrwxrwx   0        0        0        0 2024-04-13 08:30:04.836631 pkscreener-0.44.20240413.258/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 08:30:04.852229 pkscreener-0.44.20240413.258/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0    17333 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    24554 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9291 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     2995 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    27550 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    20761 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    17381 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8037 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    48885 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   110553 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    44608 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    74274 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-13 08:29:56.000000 pkscreener-0.44.20240413.258/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   112019 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/globals.py
--rw-rw-rw-   0        0        0      565 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    47815 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    18495 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-13 08:30:04.836631 pkscreener-0.44.20240413.258/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-13 08:30:04.000000 pkscreener-0.44.20240413.258/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1250 2024-04-13 08:30:04.000000 pkscreener-0.44.20240413.258/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 08:30:04.000000 pkscreener-0.44.20240413.258/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-04-13 08:30:04.000000 pkscreener-0.44.20240413.258/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-13 08:30:04.000000 pkscreener-0.44.20240413.258/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-13 08:30:04.000000 pkscreener-0.44.20240413.258/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-13 08:30:04.852229 pkscreener-0.44.20240413.258/setup.cfg
--rw-rw-rw-   0        0        0     4715 2024-04-13 08:26:53.000000 pkscreener-0.44.20240413.258/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 22:52:24.736851 pkscreener-0.44.20240413.259/
+-rw-rw-rw-   0        0        0     1086 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-13 22:52:24.736851 pkscreener-0.44.20240413.259/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/README.md
+drwxrwxrwx   0        0        0        0 2024-04-13 22:52:24.721233 pkscreener-0.44.20240413.259/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 22:52:24.736851 pkscreener-0.44.20240413.259/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0    17333 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    24554 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9291 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     2995 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    27550 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    20761 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    17381 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8037 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    48885 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   110608 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    45499 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    74274 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-13 22:52:17.000000 pkscreener-0.44.20240413.259/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   112019 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      565 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    47815 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    18495 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-13 22:52:24.736851 pkscreener-0.44.20240413.259/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-13 22:52:24.000000 pkscreener-0.44.20240413.259/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1250 2024-04-13 22:52:24.000000 pkscreener-0.44.20240413.259/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 22:52:24.000000 pkscreener-0.44.20240413.259/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-04-13 22:52:24.000000 pkscreener-0.44.20240413.259/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-13 22:52:24.000000 pkscreener-0.44.20240413.259/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-13 22:52:24.000000 pkscreener-0.44.20240413.259/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-13 22:52:24.736851 pkscreener-0.44.20240413.259/setup.cfg
+-rw-rw-rw-   0        0        0     4715 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/setup.py
```

### Comparing `pkscreener-0.44.20240413.258/LICENSE` & `pkscreener-0.44.20240413.259/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/LICENSE-Others` & `pkscreener-0.44.20240413.259/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/PKG-INFO` & `pkscreener-0.44.20240413.259/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240413.258
+Version: 0.44.20240413.259
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240413.258.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240413.259.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.257/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.258/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.257/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.258/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.257/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.258/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240413.258/README.md` & `pkscreener-0.44.20240413.259/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.257/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.258/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.257/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.258/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.257/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.258/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240413.258/pkscreener/__init__.py` & `pkscreener-0.44.20240413.259/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240413.259/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240413.259/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240413.259/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240413.259/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240413.259/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240413.259/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240413.259/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240413.259/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240413.259/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240413.259/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240413.259/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240413.259/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240413.259/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240413.259/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240413.259/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240413.259/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240413.259/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240413.259/pkscreener/classes/ScreeningStatistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1289,14 +1289,15 @@
         if result_df is not None:
             result_df.drop_duplicates(keep="last", inplace=True)
             result_df.sort_values(by="Time", inplace=True)
         return result_df[::-1]
 
     # Preprocess the acquired data
     def preprocessData(self, df, daysToLookback=None):
+        assert isinstance(df, pd.DataFrame)
         data = df.copy()
         data = data.replace(np.inf, np.nan).replace(-np.inf, np.nan).dropna(how="all")
         self.default_logger.info(f"Preprocessing data:\n{data.head(1)}\n")
         if daysToLookback is None:
             daysToLookback = self.configManager.daysToLookback
         if self.configManager.useEMA:
             sma = pktalib.EMA(data["Close"], timeperiod=50)
@@ -1537,15 +1538,15 @@
     # Validate 'Inside Bar' structure for recent days
     def validateInsideBar(
         self, df, screenDict, saveDict, chartPattern=1, daysToLookback=5
     ):
         data = df.copy()
         orgData = data
         saved = self.findCurrentSavedValue(screenDict, saveDict, "Pattern")
-        for i in range(daysToLookback, round(daysToLookback * 0.5) - 1, -1):
+        for i in range(int(daysToLookback), int(round(daysToLookback * 0.5)) - 1, -1):
             if i == 2:
                 return 0  # Exit if only last 2 candles are left
             if chartPattern == 1:
                 if "Up" in saveDict["Trend"] and (
                     "Bull" in saveDict["MA-Signal"]
                     or "Support" in saveDict["MA-Signal"]
                 ):
```

### Comparing `pkscreener-0.44.20240413.258/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240413.259/pkscreener/classes/StockScreener.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,18 @@
                 hostRef.processingCounter.value += 1
 
             volumeRatio, period = self.determineBasicConfigs(stock, newlyListedOnly, volumeRatio, logLevel, hostRef, configManager, screener, userArgsLog)
             # hostRef.default_logger.info(
             #     f"For stock:{stock}, stock exists in objectDictionary:{hostRef.objectDictionary.get(stock)}, cacheEnabled:{configManager.cacheEnabled}, isTradingTime:{self.isTradingTime}, downloadOnly:{downloadOnly}"
             # )
             data = self.getRelevantDataForStock(totalSymbols, shouldCache, stock, downloadOnly, printCounter, backtestDuration, hostRef, configManager, fetcher, period, testData,exchangeName)
-            if len(data) == 0 or len(data) < backtestDuration:
+            if data is not None:
+                if len(data) == 0 or len(data) < backtestDuration:
+                    return None
+            else:
                 return None
             # hostRef.default_logger.info(f"Will pre-process data:\n{data.tail(10)}")
             fullData, processedData, data = self.getCleanedDataForDuration(backtestDuration, portfolio, screeningDictionary, saveDictionary, configManager, screener, data)
             def returnLegibleData():
                 if backtestDuration == 0 or menuOption not in ["B"]:
                     return None
                 elif (backtestDuration > 0 and backtestDuration <= configManager.maxBacktestWindow):
@@ -723,18 +726,34 @@
                         pass
                     try:
                         data["FairValue"] = hostData["FairValue"]
                     except KeyError:
                         pass
         else:
             self.printProcessingCounter(totalSymbols, stock, printCounter, hostRef)
-            data = hostData
-            data = pd.DataFrame(
-                    data["data"], columns=data["columns"], index=data["index"]
-                )
+            # data = hostData
+            try:
+                columns = hostData["columns"]
+                data = pd.DataFrame(
+                        hostData["data"], columns=columns, index=hostData["index"]
+                    )
+            except (ValueError, AssertionError) as e:
+                # 9 columns passed, passed data had 11 columns
+                # 10 columns passed, passed data had 11 columns
+                hostRef.default_logger.debug(e, exc_info=True)
+                e_diff = str(e).replace(" columns passed, passed data had ",",").replace(" columns","").split(",")
+                num_diff = int(e_diff[1]) - int(e_diff[0])
+                while (num_diff > 0):
+                    columns.append(f"temp{num_diff}")
+                    num_diff -= 1
+                data = pd.DataFrame(
+                        hostData["data"], columns=columns, index=hostData["index"]
+                    )
+                pass
+
         if ((shouldCache and not self.isTradingTime and (hostData is None)) or downloadOnly) \
             or (shouldCache and hostData is None):  # and backtestDuration == 0 # save only if we're NOT backtesting
                 if start is None and data is not None:
                     hostRef.objectDictionary[stock] = data.to_dict("split")
                 if downloadOnly:
                     with hostRef.processingResultsCounter.get_lock():
                         hostRef.processingResultsCounter.value += 1
```

### Comparing `pkscreener-0.44.20240413.258/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240413.259/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240413.259/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240413.259/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/pkscreener/classes/keys.py` & `pkscreener-0.44.20240413.259/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/pkscreener/courbd.ttf` & `pkscreener-0.44.20240413.259/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/pkscreener/globals.py` & `pkscreener-0.44.20240413.259/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240413.259/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240413.259/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240413.259/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240413.259/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240413.258
+Version: 0.44.20240413.259
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240413.258.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240413.259.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.257/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.258/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.257/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.258/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.257/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.258/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240413.258/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240413.259/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.258/setup.py` & `pkscreener-0.44.20240413.259/setup.py`

 * *Files identical despite different names*

