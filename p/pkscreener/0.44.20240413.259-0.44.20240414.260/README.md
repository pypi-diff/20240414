# Comparing `tmp/pkscreener-0.44.20240413.259.tar.gz` & `tmp/pkscreener-0.44.20240414.260.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240413.259.tar", last modified: Sat Apr 13 22:52:24 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240414.260.tar", last modified: Sun Apr 14 10:19:34 2024, max compression
```

## Comparing `pkscreener-0.44.20240413.259.tar` & `pkscreener-0.44.20240414.260.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 22:52:24.736851 pkscreener-0.44.20240413.259/
--rw-rw-rw-   0        0        0     1086 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-13 22:52:24.736851 pkscreener-0.44.20240413.259/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/README.md
-drwxrwxrwx   0        0        0        0 2024-04-13 22:52:24.721233 pkscreener-0.44.20240413.259/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 22:52:24.736851 pkscreener-0.44.20240413.259/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0    17333 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    24554 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9291 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     2995 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    27550 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    20761 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    17381 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8037 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    48885 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   110608 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    45499 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    74274 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-13 22:52:17.000000 pkscreener-0.44.20240413.259/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   112019 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/globals.py
--rw-rw-rw-   0        0        0      565 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    47815 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    18495 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-13 22:52:24.736851 pkscreener-0.44.20240413.259/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-13 22:52:24.000000 pkscreener-0.44.20240413.259/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1250 2024-04-13 22:52:24.000000 pkscreener-0.44.20240413.259/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 22:52:24.000000 pkscreener-0.44.20240413.259/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-04-13 22:52:24.000000 pkscreener-0.44.20240413.259/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-13 22:52:24.000000 pkscreener-0.44.20240413.259/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-13 22:52:24.000000 pkscreener-0.44.20240413.259/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-13 22:52:24.736851 pkscreener-0.44.20240413.259/setup.cfg
--rw-rw-rw-   0        0        0     4715 2024-04-13 22:48:36.000000 pkscreener-0.44.20240413.259/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 10:19:34.058630 pkscreener-0.44.20240414.260/
+-rw-rw-rw-   0        0        0     1086 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-14 10:19:34.058630 pkscreener-0.44.20240414.260/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 10:19:34.043005 pkscreener-0.44.20240414.260/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 10:19:34.058630 pkscreener-0.44.20240414.260/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0    17333 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    24554 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9291 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     2995 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    27550 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    20761 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    17381 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8037 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    48885 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   112690 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    45499 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    74365 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-14 10:19:26.000000 pkscreener-0.44.20240414.260/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   113082 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      565 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    47815 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    18453 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-14 10:19:34.043005 pkscreener-0.44.20240414.260/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-14 10:19:33.000000 pkscreener-0.44.20240414.260/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1250 2024-04-14 10:19:33.000000 pkscreener-0.44.20240414.260/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 10:19:33.000000 pkscreener-0.44.20240414.260/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-04-14 10:19:33.000000 pkscreener-0.44.20240414.260/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-14 10:19:33.000000 pkscreener-0.44.20240414.260/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-14 10:19:33.000000 pkscreener-0.44.20240414.260/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-14 10:19:34.058630 pkscreener-0.44.20240414.260/setup.cfg
+-rw-rw-rw-   0        0        0     4715 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/setup.py
```

### Comparing `pkscreener-0.44.20240413.259/LICENSE` & `pkscreener-0.44.20240414.260/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.259/LICENSE-Others` & `pkscreener-0.44.20240414.260/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.259/PKG-INFO` & `pkscreener-0.44.20240414.260/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240413.259
+Version: 0.44.20240414.260
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240413.259.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240414.260.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.258/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.259/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.258/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.259/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.258/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.259/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240413.259/README.md` & `pkscreener-0.44.20240414.260/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.258/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.259/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.258/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.259/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.258/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.259/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240413.259/pkscreener/__init__.py` & `pkscreener-0.44.20240414.260/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.259/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240414.260/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.259/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240414.260/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.259/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240414.260/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.259/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240414.260/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.259/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240414.260/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.259/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240414.260/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.259/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240414.260/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.259/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240414.260/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.259/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240414.260/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.259/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240414.260/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.259/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240414.260/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.259/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240414.260/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.259/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240414.260/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.259/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240414.260/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.259/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240414.260/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.259/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240414.260/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.259/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240414.260/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.259/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240414.260/pkscreener/classes/ScreeningStatistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,16 @@
         ] = f"{highColor}{str('{:.2f}'.format(full52WeekHigh))}{colorText.END}"
         screenDict[
             "52Wk L"
         ] = f"{lowColor}{str('{:.2f}'.format(full52WeekLow))}{colorText.END}"
 
     # Find stocks that have broken through 52 week low.
     def find52WeekLowBreakout(self, df):
+        if df is None or len(df) == 0:
+            return False
         # https://chartink.com/screener/52-week-low-breakout
         data = df.copy()
         data = data.fillna(0)
         data = data.replace([np.inf, -np.inf], 0)
         one_week = 5
         recent = data.head(1)["Low"].iloc[0]
         # last1Week = data.head(one_week)
@@ -169,14 +171,16 @@
             # or (last1WeekLow <= min(full52WeekLow, last1WeekLow))
             # or (last1WeekLow <= previousWeekLow <= min(full52WeekLow, previousWeekLow))
         )
 
         # Find stocks that have broken through 52 week low.
 
     def find10DaysLowBreakout(self, df):
+        if df is None or len(df) == 0:
+            return False
         data = df.copy()
         data = data.fillna(0)
         data = data.replace([np.inf, -np.inf], 0)
         one_week = 5
         recent = data.head(1)["Low"].iloc[0]
         last1Week = data.head(one_week)
         last2Week = data.head(2 * one_week)
@@ -186,14 +190,16 @@
         return (recent <= min(previousWeekLow, last1WeekLow)) and (
             last1WeekLow <= previousWeekLow
         )
 
         # Find stocks that have broken through 52 week low.
 
     def findAroonBullishCrossover(self, df):
+        if df is None or len(df) == 0:
+            return False
         data = df.copy()
         data = data.fillna(0)
         data = data.replace([np.inf, -np.inf], 0)
         period = 14
         data = data[::-1]  # Reverse the dataframe so that its the oldest date first
         aroondf = pktalib.Aroon(data["High"], data["Low"], period)
         recent = aroondf.tail(1)
@@ -248,14 +254,16 @@
         )
 
     #@measure_time
     # Find accurate breakout value
     def findBreakoutValue(
         self, df, screenDict, saveDict, daysToLookback, alreadyBrokenout=False
     ):
+        if df is None or len(df) == 0:
+            return False
         data = df.copy()
         data = data.fillna(0)
         data = data.replace([np.inf, -np.inf], 0)
         recent = data.head(1)
         data = data[1:]
         maxHigh = round(data.describe()["High"]["max"], 2)
         maxClose = round(data.describe()["Close"]["max"], 2)
@@ -485,14 +493,16 @@
                 colorText.BOLD + colorText.GREEN + " (Potential)" + colorText.END
             )
             return True
         return False
 
     # Find stocks with reversing PSAR and RSI
     def findPSARReversalWithRSI(self, df, screenDict, saveDict,minRSI=50):
+        if df is None or len(df) == 0:
+            return False
         data = df.copy()
         data = data[::-1]
         psar = pktalib.psar(data["High"],data["Low"])
         if len(psar) < 3:
             return False
         psar = psar.tail(3)
         data = data.tail(3)
@@ -526,14 +536,16 @@
                 # (dayMinus2RSI >= minRSI) and \
                 # (dayMinus1RSI >= dayMinus2RSI) and \
                 # (dayRSI >= dayMinus1RSI)) or \
         return hasReversal
 
     # Find stock reversing at given MA
     def findReversalMA(self, df, screenDict, saveDict, maLength, percentage=0.02):
+        if df is None or len(df) == 0:
+            return False
         data = df.copy()
         maRange = [10, 20, 50, 200]
         results = []
         hasReversals = False
         data = data[::-1]
         saved = self.findCurrentSavedValue(screenDict,saveDict, "MA-Signal")
         for maLength in maRange:
@@ -681,14 +693,16 @@
             while(diff_df["diff"][index-1] >= 0 and index >=0):
                 index -= 1
         ts = diff_df.tail(len(diff_df)-index +1).head(1).index[-1]
         return ts, df[df.index == ts] #df.head(len(df) -index +1).tail(1)
     
     # Find stocks with rising RSI from lower levels
     def findRisingRSI(self, df):
+        if df is None or len(df) == 0:
+            return False
         data = df.copy()
         data = data[::-1]
         data = data.tail(3)
         dayMinus2RSI = data["RSI"].iloc[0]
         dayMinus1RSI = data["RSI"].iloc[1]
         dayRSI = data["RSI"].iloc[2]
         return (dayMinus2RSI <= 35 and dayMinus1RSI > dayMinus2RSI and dayRSI > dayMinus1RSI) or \
@@ -888,14 +902,17 @@
                 pass
         decision = 'T:▲' if isUptrend else ('T:▼' if isDowntrend else '')
         dma50decision = 't:▲' if is50DMAUptrend else ('t:▼' if is50DMADowntrend else '')
         mf_inst_ownershipChange = 0
         change_millions =""
         try:
             mf_inst_ownershipChange = self.getMutualFundStatus(stock,onlyMF=onlyMF,hostData=hostData,force=(hostData is None or hostData.empty or not ("MF" in hostData.columns or "FII" in hostData.columns)),exchangeName=exchangeName)
+            if isinstance(mf_inst_ownershipChange, pd.Series):
+                print(f"Unexpected mf_inst_ownershipChange:{mf_inst_ownershipChange}")
+                mf_inst_ownershipChange = 0
             roundOff = 2
             millions = round(mf_inst_ownershipChange/1000000,roundOff)
             while float(millions) == 0 and roundOff <=5:
                 roundOff +=1
                 millions = round(mf_inst_ownershipChange/1000000,roundOff)
             change_millions = f"({millions}M)"
         except Exception as e:  # pragma: no cover
@@ -1330,14 +1347,16 @@
         # data = data.replace([np.inf, -np.inf], 0)
         fullData = data
         trimmedData = data.head(daysToLookback)
         return (fullData, trimmedData)
 
     # Validate if the stock is bullish in the short term
     def validate15MinutePriceVolumeBreakout(self, df):
+        if df is None or len(df) == 0:
+            return False
         # https://chartink.com/screener/15-min-price-volume-breakout
         data = df.copy()
         data = data.fillna(0)
         data = data.replace([np.inf, -np.inf], 0)
         data = data[::-1]  # Reverse the dataframe so that its the oldest date first
         data["SMA20"] = pktalib.SMA(data["Close"], 20)
         data["SMA20V"] = pktalib.SMA(data["Volume"], 20)
@@ -1384,14 +1403,16 @@
                 < 1
             )
         )
 
     #@measure_time
     # validate if CCI is within given range
     def validateCCI(self, df, screenDict, saveDict, minCCI, maxCCI):
+        if df is None or len(df) == 0:
+            return False
         data = df.copy()
         data = data.fillna(0)
         data = data.replace([np.inf, -np.inf], 0)
         cci = int(data.head(1)["CCI"].iloc[0])
         saveDict["CCI"] = cci
         if (cci >= minCCI and cci <= maxCCI):
             if ("Up" in saveDict["Trend"]):
@@ -1404,14 +1425,16 @@
                 )
             return True
         screenDict["CCI"] = colorText.BOLD + colorText.FAIL + str(cci) + colorText.END
         return False
 
     # Find Conflucence
     def validateConfluence(self, stock, df, screenDict, saveDict, percentage=0.1,confFilter=3):
+        if df is None or len(df) == 0:
+            return False
         data = df.copy()
         recent = data.head(2)
         is50DMAUpTrend = (recent["SMA"].iloc[0] > recent["SMA"].iloc[1])
         is50DMADownTrend = (recent["SMA"].iloc[0] < recent["SMA"].iloc[1])
         isGoldenCrossOver = (recent["SMA"].iloc[0] >= recent["LMA"].iloc[0]) and \
                             (recent["SMA"].iloc[1] <= recent["LMA"].iloc[1])
         isDeadCrossOver = (recent["SMA"].iloc[0] <= recent["LMA"].iloc[0]) and \
@@ -1467,14 +1490,16 @@
                 (confFilter == 1 and isGoldenCrossOver) or \
                 (confFilter == 2 and isDeadCrossOver)
         return False
 
     #@measure_time
     # Validate if share prices are consolidating
     def validateConsolidation(self, df, screenDict, saveDict, percentage=10):
+        if df is None or len(df) == 0:
+            return False
         data = df.copy()
         data = data.fillna(0)
         data = data.replace([np.inf, -np.inf], 0)
         hc = data.describe()["Close"]["max"]
         lc = data.describe()["Close"]["min"]
         if (hc - lc) <= (hc * percentage / 100) and (hc - lc != 0):
             screenDict["Consol."] = (
@@ -1496,14 +1521,16 @@
             )
         saveDict["Consol."] = f'Range:{str(round((abs((hc-lc)/hc)*100),1))+"%"}'
         return round((abs((hc - lc) / hc) * 100), 1)
 
     # validate if the stock has been having higher highs, higher lows
     # and higher close with latest close > supertrend and 8-EMA.
     def validateHigherHighsHigherLowsHigherClose(self, df):
+        if df is None or len(df) == 0:
+            return False
         data = df.copy()
         day0 = data
         day1 = data[1:]
         day2 = data[2:]
         day3 = data[3:]
         higherHighs = (
             (day0["High"].iloc[0] > day1["High"].iloc[0])
@@ -1535,14 +1562,16 @@
         return higherHighs and higherLows and higherClose
 
     #@measure_time
     # Validate 'Inside Bar' structure for recent days
     def validateInsideBar(
         self, df, screenDict, saveDict, chartPattern=1, daysToLookback=5
     ):
+        if df is None or len(df) == 0:
+            return False
         data = df.copy()
         orgData = data
         saved = self.findCurrentSavedValue(screenDict, saveDict, "Pattern")
         for i in range(int(daysToLookback), int(round(daysToLookback * 0.5)) - 1, -1):
             if i == 2:
                 return 0  # Exit if only last 2 candles are left
             if chartPattern == 1:
@@ -1592,14 +1621,16 @@
                         return i
                 else:
                     return 0
         return 0
 
     # Find IPO base
     def validateIpoBase(self, stock, df, screenDict, saveDict, percentage=0.3):
+        if df is None or len(df) == 0:
+            return False
         data = df.copy()
         listingPrice = data[::-1].head(1)["Open"].iloc[0]
         currentPrice = data.head(1)["Close"].iloc[0]
         ATH = data.describe()["High"]["max"]
         if ATH > (listingPrice + (listingPrice * percentage)):
             return False
         away = round(((currentPrice - listingPrice) / listingPrice) * 100, 1)
@@ -1630,28 +1661,31 @@
             saveDict["Pattern"] = saved[1] + f"IPO Base ({away} %)"
             return True
         return False
 
     #@measure_time
     # Validate Lorentzian Classification signal
     def validateLorentzian(self, df, screenDict, saveDict, lookFor=3):
+        if df is None or len(df) == 0:
+            return False
         data = df.copy()
         # lookFor: 1-Buy, 2-Sell, 3-Any
         data = data[::-1]  # Reverse the dataframe
         data = data.rename(
             columns={
                 "Open": "open",
                 "Close": "close",
                 "High": "high",
                 "Low": "low",
                 "Volume": "volume",
             }
         )
         try:
-            lc = ata.LorentzianClassification(data=data)
+            with SuppressOutput(suppress_stdout=True, suppress_stderr=True):
+                lc = ata.LorentzianClassification(data=data)
             saved = self.findCurrentSavedValue(screenDict, saveDict, "Pattern")
             if lc.df.iloc[-1]["isNewBuySignal"]:
                 screenDict["Pattern"] = (
                     saved[0] + colorText.BOLD + colorText.GREEN + "Lorentzian-Buy" + colorText.END
                 )
                 saveDict["Pattern"] = saved[1] + "Lorentzian-Buy"
                 if lookFor != 2: # Not Sell
@@ -1674,14 +1708,16 @@
             # File "/opt/homebrew/lib/python3.11/site-packages/pandas/core/ops/array_ops.py", line 364, in na_logical_op
             # self.default_logger.debug(e, exc_info=True)
             pass
         return False
 
     # validate if the stock has been having lower lows, lower highs
     def validateLowerHighsLowerLows(self, df):
+        if df is None or len(df) == 0:
+            return False
         data = df.copy()
         day0 = data
         day1 = data[1:]
         day2 = data[2:]
         day3 = data[3:]
         lowerHighs = (
             (day0["High"].iloc[0] < day1["High"].iloc[0])
@@ -1699,14 +1735,16 @@
             and (day2["RSI"].iloc[0] < day3["RSI"].iloc[0])
             and day0["RSI"].iloc[0] >= 50
         )
         return lowerHighs and lowerLows and higherRSI
 
     # Validate if recent volume is lowest of last 'N' Days
     def validateLowestVolume(self, df, daysForLowestVolume):
+        if df is None or len(df) == 0:
+            return False
         data = df.copy()
         data = data.fillna(0)
         data = data.replace([np.inf, -np.inf], 0)
         if daysForLowestVolume is None:
             daysForLowestVolume = 30
         if len(data) < daysForLowestVolume:
             return False
@@ -1796,24 +1834,28 @@
                 saveDict[f"LTP{prd}"] = np.nan
                 saveDict[f"Growth{prd}"] = np.nan
                 screenDict["Date"] = calc_date
                 saveDict["Date"] = calc_date
 
     # Find stocks that are bearish intraday: Macd Histogram negative
     def validateMACDHistogramBelow0(self, df):
+        if df is None or len(df) == 0:
+            return False
         data = df.copy()
         data = data.fillna(0)
         data = data.replace([np.inf, -np.inf], 0)
         data = data[::-1]  # Reverse the dataframe so that its the oldest date first
         macd = pktalib.MACD(data["Close"], 12, 26, 9)[2].tail(1)
         return macd.iloc[:1][0] < 0
 
     #@measure_time
     # Find if stock gaining bullish momentum
     def validateMomentum(self, df, screenDict, saveDict):
+        if df is None or len(df) == 0:
+            return False
         data = df.copy()
         try:
             data = data.head(3)
             if len(data) < 3:
                 return False
             for row in data.iterrows():
                 # All 3 candles should be Green and NOT Circuits
@@ -1969,14 +2011,16 @@
                 )
                 saveDict["MA-Signal"] = saved[1] + "BearCross-200MA"
                 maReversal = -1
         return maReversal
 
     # Find NRx range for Reversal
     def validateNarrowRange(self, df, screenDict, saveDict, nr=4):
+        if df is None or len(df) == 0:
+            return False
         data = df.copy()
         saved = self.findCurrentSavedValue(screenDict, saveDict, "Pattern")
         if PKDateUtilities.isTradingTime():
             rangeData = data.head(nr + 1)[1:]
             now_candle = data.head(1)
             rangeData["Range"] = abs(rangeData["Close"] - rangeData["Open"])
             recent = rangeData.head(1)
@@ -2001,37 +2045,41 @@
                         saved[0] + colorText.BOLD + colorText.FAIL + f"Sell-NR{nr}" + colorText.END
                     )
                     saveDict["Pattern"] = saved[1] + f"Sell-NR{nr}"
                     return True
             return False
         else:
             rangeData = data.head(nr)
-            rangeData["Range"] = abs(rangeData["Close"] - rangeData["Open"])
+            rangeData.loc[:,'Range'] = abs(rangeData["Close"] - rangeData["Open"])
             recent = rangeData.head(1)
             if recent["Range"].iloc[0] == rangeData.describe()["Range"]["min"]:
                 screenDict["Pattern"] = (
                     saved[0] + colorText.BOLD + colorText.GREEN + f"NR{nr}" + colorText.END
                 )
                 saveDict["Pattern"] = saved[1] + f"NR{nr}"
                 return True
             return False
 
     # Find if stock is newly listed
     def validateNewlyListed(self, df, daysToLookback):
+        if df is None or len(df) == 0:
+            return False
         data = df.copy()
         daysToLookback = int(daysToLookback[:-1])
         recent = data.head(1)
         if len(data) < daysToLookback and (
             recent["Close"].iloc[0] != np.nan and recent["Close"].iloc[0] > 0
         ):
             return True
         return False
 
     # Validate if the stock prices are at least rising by 2% for the last 3 sessions
     def validatePriceRisingByAtLeast2Percent(self, df, screenDict, saveDict):
+        if df is None or len(df) == 0:
+            return False
         data = df.copy()
         data = data.fillna(0)
         data = data.replace([np.inf, -np.inf], 0)
         data = data.head(4)
         if len(data) < 4:
             return False
         day0 = data.iloc[0]["Close"].item()
@@ -2052,14 +2100,16 @@
             screenDict["%Chng"] = colorText.GREEN + pct_change_text + colorText.END
             return True and self.getCandleType(data.head(1))
         return False
 
     #@measure_time
     # validate if RSI is within given range
     def validateRSI(self, df, screenDict, saveDict, minRSI, maxRSI):
+        if df is None or len(df) == 0:
+            return False
         data = df.copy()
         data = data.fillna(0)
         data = data.replace([np.inf, -np.inf], 0)
         rsi = int(data.head(1)["RSI"].iloc[0])
         saveDict["RSI"] = rsi
         # https://chartink.com/screener/rsi-screening
         if rsi >= minRSI and rsi <= maxRSI:  # or (rsi <= 71 and rsi >= 67):
@@ -2068,14 +2118,16 @@
             )
             return True
         screenDict["RSI"] = colorText.BOLD + colorText.FAIL + str(rsi) + colorText.END
         return False
 
     # Validate if the stock is bullish in the short term
     def validateShortTermBullish(self, df, screenDict, saveDict):
+        if df is None or len(df) == 0:
+            return False
         data = df.copy()
         # https://chartink.com/screener/short-term-bullish
         data = data.fillna(0)
         data = data.replace([np.inf, -np.inf], 0)
         recent = data.head(1)
         fk = 0 if len(data) < 3 else np.round(data["FASTK"].iloc[2], 5)
         # Reverse the dataframe for ichimoku calculations with date in ascending order
@@ -2138,14 +2190,16 @@
                         return True
         return False
 
     # Validate VPC
     def validateVCP(
         self, df, screenDict, saveDict, stockName=None, window=3, percentageFromTop=3
     ):
+        if df is None or len(df) == 0:
+            return False
         data = df.copy()
         try:
             percentageFromTop /= 100
             data.reset_index(inplace=True)
             data.rename(columns={"index": "Date"}, inplace=True)
             data["tops"] = (
                 data["High"]
@@ -2215,14 +2269,16 @@
             self.default_logger.debug(e, exc_info=True)
         return False
 
     # Validate if volume of last day is higher than avg
     def validateVolume(
         self, df, screenDict, saveDict, volumeRatio=2.5, minVolume=100
     ):
+        if df is None or len(df) == 0:
+            return False, False
         data = df.copy()
         data = data.fillna(0)
         data = data.replace([np.inf, -np.inf], 0)
         recent = data.head(1)
         # Either the rolling volume of past 20 sessions or today's volume should be > min volume
         hasMinimumVolume = (
             recent["VolMA"].iloc[0] >= minVolume
@@ -2239,14 +2295,16 @@
             return True, hasMinimumVolume
         screenDict["Volume"] = ratio
         return False, hasMinimumVolume
 
     # Find if stock is validating volume spread analysis
     def validateVolumeSpreadAnalysis(self, df, screenDict, saveDict):
         try:
+            if df is None or len(df) == 0:
+                return False
             data = df.copy()
             data = data.head(2)
             if len(data) < 2:
                 return False
             try:
                 # Check for previous RED candles
                 # Current candle = 0th, Previous Candle = 1st for following logic
```

### Comparing `pkscreener-0.44.20240413.259/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240414.260/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.259/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240414.260/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.259/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240414.260/pkscreener/classes/Utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,16 @@
 
 class tools:
     def clearScreen(userArgs=None):
         if "RUNNER" in os.environ.keys() or (userArgs is not None and userArgs.prodbuild):
             if userArgs is not None and userArgs.v:
                 os.environ["RUNNER"]="LOCAL_RUN_SCANNER"
             return
+        elif (userArgs is not None and userArgs.runintradayanalysis):
+            return
         if platform.system() == "Windows":
             os.system("cls")
         else:
             os.system("clear")
         try:
             art = colorText.GREEN + artText + colorText.END + f" | {marketStatus()}"
             print(art.encode('utf-8').decode(STD_ENCODING))
```

### Comparing `pkscreener-0.44.20240413.259/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240414.260/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.259/pkscreener/classes/keys.py` & `pkscreener-0.44.20240414.260/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.259/pkscreener/courbd.ttf` & `pkscreener-0.44.20240414.260/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.259/pkscreener/globals.py` & `pkscreener-0.44.20240414.260/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -552,16 +552,22 @@
             if reversalOption in [3]:
                 sortKey = ["Volume","MA-Signal"]
                 ascending = [False, False]
         elif executeOption == 23:
             sortKey = ["bbands_ulr_ratio_max5"]
             ascending = [False]
         try:
-            screenResults[sortKey] = screenResults[sortKey].replace("", np.nan).replace(np.inf, np.nan).replace(-np.inf, np.nan).astype(float)
-            saveResults[sortKey] = saveResults[sortKey].replace("", np.nan).replace(np.inf, np.nan).replace(-np.inf, np.nan).astype(float)
+            try:
+                screenResults[sortKey] = screenResults[sortKey].replace("", np.nan).replace(np.inf, np.nan).replace(-np.inf, np.nan).astype(float)
+            except:
+                pass
+            try:
+                saveResults[sortKey] = saveResults[sortKey].replace("", np.nan).replace(np.inf, np.nan).replace(-np.inf, np.nan).astype(float)
+            except:
+                pass
             screenResults.sort_values(by=sortKey, ascending=ascending, inplace=True)
             saveResults.sort_values(by=sortKey, ascending=ascending, inplace=True)
         except Exception as e:
             default_logger().debug(e, exc_info=True)
             pass
         columnsToBeDeleted = ["MFI","FVDiff","ConfDMADifference","bbands_ulr_ratio_max5"]
         for column in columnsToBeDeleted:
@@ -1667,32 +1673,32 @@
             maxcolwidths=Utility.tools.getMaxColumnWidths(strategy_df)
         ).encode("utf-8").decode(STD_ENCODING)
         print(addendumLabel)
         print(tabulated_strategy)
     if screenResults is not None and len(screenResults) >= 1:
         choiceSegments = menuChoiceHierarchy.split(">")
         choiceSegments = f"{choiceSegments[-2]} > {choiceSegments[-1]}" if len(choiceSegments)>=4 else f"{choiceSegments[-1]}"
-        title = f'<b>{choiceSegments}</b> {"" if selectedChoice["0"] != "G" else "for Date:"+ targetDateG10k}'
+        title = f'<b>{choiceSegments}</b>{"" if selectedChoice["0"] != "G" else " for Date:"+ targetDateG10k}'
         if (
             ("RUNNER" in os.environ.keys() and os.environ["RUNNER"] != "LOCAL_RUN_SCANNER")
             or "PKDevTools_Default_Log_Level" in os.environ.keys()
         ):
             if eligible:
                 # There's no need to save data locally.
                 # This scan must have been triggered by github workflow by a user or scheduled job
                 # Let's just send the image result to telegram
                 screenResultsTrimmed = screenResults.copy()
                 saveResultsTrimmed = saveResults.copy()
                 # No point sending a photo with more than MAX_ALLOWED stocks.
                 warn_text = (
-                    f" but only including top {MAX_ALLOWED} results here. "
+                    f" but showing only {MAX_ALLOWED}. "
                     if (len(saveResults) > MAX_ALLOWED)
                     else ""
                 )
-                caption = f"<b>({len(saveResults)}{'+' if (len(saveResults) > MAX_ALLOWED) else ''}</b> stocks found in {str('{:.2f}'.format(elapsed_time))} sec){warn_text}. {title}"
+                caption = f"({len(saveResults)}{'+' if (len(saveResults) > MAX_ALLOWED) else ''} stocks found in {str(int(elapsed_time))} sec){warn_text}.{title}"
                 backtestExtension = "_backtest.png"
                 if len(screenResultsTrimmed) > MAX_ALLOWED:
                     screenResultsTrimmed = screenResultsTrimmed.head(MAX_ALLOWED)
                     saveResultsTrimmed = saveResultsTrimmed.head(MAX_ALLOWED)
                     if saveResultsTrimmed is not None and len(saveResultsTrimmed) > 0:
                         tabulated_results = colorText.miniTabulator().tabulate(
                             screenResultsTrimmed,
@@ -1704,20 +1710,34 @@
                 if saveResultsTrimmed is not None and len(saveResultsTrimmed) > 0:
                     markdown_results = colorText.miniTabulator().tabulate(
                         saveResultsTrimmed,
                         headers="keys",
                         tablefmt=colorText.No_Pad_GridFormat,
                         maxcolwidths=Utility.tools.getMaxColumnWidths(saveResultsTrimmed)
                     ).encode("utf-8").decode(STD_ENCODING)
+                    caption_df = saveResultsTrimmed[['LTP','%Chng','Volume']].head(5)
+                    caption_df.loc[:, "LTP"] = caption_df.loc[:, "LTP"].apply(
+                        lambda x: str(int(round(x,0)))
+                    )
+                    caption_df.loc[:, "%Chng"] = caption_df.loc[:, "%Chng"].apply(
+                        lambda x: f'{int(round(float(x.replace("%","")),0))}%'
+                    )
+                    caption_df.loc[:, "Volume"] = caption_df.loc[:, "Volume"].apply(
+                        lambda x: f'{int(round(float(x.replace("x","")),0))}x'
+                    )
+                    caption_df.rename(columns={"%Chng": "Ch%","Volume":"Vol"}, inplace=True)
+                    for col in caption_df.columns:
+                        caption_df[col] = caption_df[col].astype(str)
                     caption_results = colorText.miniTabulator().tabulate(
-                        saveResultsTrimmed[['LTP','%Chng','Volume']].head(5),
+                        caption_df,
                         headers="keys",
-                        tablefmt=colorText.No_Pad_GridFormat
-                    ).encode("utf-8").decode(STD_ENCODING)
-                    caption = f"{caption}.First few samples are below. Open the attached image for more details.\n<pre>{caption_results}</pre>\n...\n<i>The author is <u><b>NOT</b> a SEBI registered financial advisor</u> and MUST NEVER be deemed as one.</i>"
+                        tablefmt=colorText.No_Pad_GridFormat,
+                        maxcolwidths=[None,None,3,3]
+                    ).encode("utf-8").decode(STD_ENCODING).replace("-+-----+-----+-----+","-+-----+---+---+").replace("%  ","%").replace("=+=====+=====+=====+","=+=====+===+===+").replace("Vol  |","Vol|").replace("x  ","x")
+                    caption = f"{caption}.Open attached image for more. 5 samples:<pre>{caption_results}</pre><i>Author is <u><b>NOT</b> a SEBI registered financial advisor</u> and MUST NOT be deemed as one.</i>"
                 if not testing and not userPassedArgs.runintradayanalysis:
                     sendQuickScanResult(
                         menuChoiceHierarchy,
                         user,
                         tabulated_results,
                         markdown_results,
                         caption,
```

### Comparing `pkscreener-0.44.20240413.259/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240414.260/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.259/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240414.260/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.259/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240414.260/pkscreener/pkscreenercli.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,17 +299,17 @@
                     traceback.print_exc()
         if optionalFinalOutcome_df is not None:
             final_df = None
             df_grouped = optionalFinalOutcome_df.groupby("Stock")
             for stock, df_group in df_grouped:
                 if stock == "PORTFOLIO":
                     if final_df is None:
-                        final_df = df_group[["Pattern","LTP","AlertTime","SqrOffLTP","SqrOff","SqrOffDiff","EoDLTP","EoDDiff","%Chng"]]
+                        final_df = df_group[["Pattern","LTP","SqrOffLTP","SqrOffDiff","EoDLTP","EoDDiff","%Chng"]]
                     else:
-                        final_df = pd.concat([final_df, df_group[["Pattern","LTP","AlertTime","SqrOffLTP","SqrOff","SqrOffDiff","EoDLTP","EoDDiff","%Chng"]]], axis=0)
+                        final_df = pd.concat([final_df, df_group[["Pattern","LTP","SqrOffLTP","SqrOffDiff","EoDLTP","EoDDiff","%Chng"]]], axis=0)
             mark_down = colorText.miniTabulator().tabulate(
                                 final_df,
                                 headers="keys",
                                 tablefmt=colorText.No_Pad_GridFormat,
                                 showindex = False
                             ).encode("utf-8").decode(Utility.STD_ENCODING)
             print(mark_down)
```

### Comparing `pkscreener-0.44.20240413.259/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240414.260/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240413.259
+Version: 0.44.20240414.260
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240413.259.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240414.260.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.258/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.259/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.258/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.259/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.258/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.259/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240413.259/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240414.260/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240413.259/setup.py` & `pkscreener-0.44.20240414.260/setup.py`

 * *Files identical despite different names*

