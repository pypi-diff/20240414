# Comparing `tmp/pkscreener-0.44.20240414.260.tar.gz` & `tmp/pkscreener-0.44.20240414.261.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240414.260.tar", last modified: Sun Apr 14 10:19:34 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240414.261.tar", last modified: Sun Apr 14 11:07:17 2024, max compression
```

## Comparing `pkscreener-0.44.20240414.260.tar` & `pkscreener-0.44.20240414.261.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 10:19:34.058630 pkscreener-0.44.20240414.260/
--rw-rw-rw-   0        0        0     1086 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-14 10:19:34.058630 pkscreener-0.44.20240414.260/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 10:19:34.043005 pkscreener-0.44.20240414.260/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 10:19:34.058630 pkscreener-0.44.20240414.260/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0    17333 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    24554 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9291 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     2995 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    27550 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    20761 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    17381 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8037 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    48885 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   112690 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    45499 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    74365 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-14 10:19:26.000000 pkscreener-0.44.20240414.260/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   113082 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/globals.py
--rw-rw-rw-   0        0        0      565 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    47815 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    18453 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-14 10:19:34.043005 pkscreener-0.44.20240414.260/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-14 10:19:33.000000 pkscreener-0.44.20240414.260/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1250 2024-04-14 10:19:33.000000 pkscreener-0.44.20240414.260/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 10:19:33.000000 pkscreener-0.44.20240414.260/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-04-14 10:19:33.000000 pkscreener-0.44.20240414.260/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-14 10:19:33.000000 pkscreener-0.44.20240414.260/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-14 10:19:33.000000 pkscreener-0.44.20240414.260/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-14 10:19:34.058630 pkscreener-0.44.20240414.260/setup.cfg
--rw-rw-rw-   0        0        0     4715 2024-04-14 10:16:59.000000 pkscreener-0.44.20240414.260/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 11:07:17.174610 pkscreener-0.44.20240414.261/
+-rw-rw-rw-   0        0        0     1086 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-14 11:07:17.174610 pkscreener-0.44.20240414.261/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 11:07:17.158985 pkscreener-0.44.20240414.261/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 11:07:17.174610 pkscreener-0.44.20240414.261/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0    17333 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    24554 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9291 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     2995 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    27580 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    20761 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    17381 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8037 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    48885 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   113669 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    46036 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    74366 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-14 11:07:09.000000 pkscreener-0.44.20240414.261/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   113082 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      565 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    47815 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    18453 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-14 11:07:17.174610 pkscreener-0.44.20240414.261/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-14 11:07:17.000000 pkscreener-0.44.20240414.261/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1250 2024-04-14 11:07:17.000000 pkscreener-0.44.20240414.261/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 11:07:17.000000 pkscreener-0.44.20240414.261/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-04-14 11:07:17.000000 pkscreener-0.44.20240414.261/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-14 11:07:17.000000 pkscreener-0.44.20240414.261/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-14 11:07:17.000000 pkscreener-0.44.20240414.261/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-14 11:07:17.174610 pkscreener-0.44.20240414.261/setup.cfg
+-rw-rw-rw-   0        0        0     4715 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/setup.py
```

### Comparing `pkscreener-0.44.20240414.260/LICENSE` & `pkscreener-0.44.20240414.261/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.260/LICENSE-Others` & `pkscreener-0.44.20240414.261/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.260/PKG-INFO` & `pkscreener-0.44.20240414.261/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240414.260
+Version: 0.44.20240414.261
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240414.260.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240414.261.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.259/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.260/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.259/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.260/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.259/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.260/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240414.260/README.md` & `pkscreener-0.44.20240414.261/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.259/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.260/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.259/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.260/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.259/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.260/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240414.260/pkscreener/__init__.py` & `pkscreener-0.44.20240414.261/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.260/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240414.261/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.260/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240414.261/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.260/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240414.261/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.260/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240414.261/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.260/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240414.261/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.260/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240414.261/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.260/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240414.261/pkscreener/classes/MenuOptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,15 @@
     "3": "Momentum Gainers (Rising Bullish Momentum)",
     "4": "Reversal at Moving Average (Bullish Reversal)",
     "5": "Volume Spread Analysis (Bullish VSA Reversal)",
     "6": "Narrow Range (NRx) Reversal",
     "7": "Lorentzian Classifier (Machine Learning based indicator)",
     "8": "PSAR and RSI reversal",
     "9": "Rising RSI",
+    "10": "RSI MA Reversal",
     "0": "Cancel",
 }
 level3_X_ChartPattern_MenuDict = {
     "1": "Bullish Inside Bar (Flag) Pattern",
     "2": "Bearish Inside Bar (Flag) Pattern(Sell)",
     "3": "The Confluence (50 & 200 MA/EMA)",
     "4": "VCP (Experimental)",
```

### Comparing `pkscreener-0.44.20240414.260/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240414.261/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.260/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240414.261/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.260/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240414.261/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.260/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240414.261/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.260/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240414.261/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.260/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240414.261/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.260/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240414.261/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.260/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240414.261/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.260/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240414.261/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.260/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240414.261/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.260/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240414.261/pkscreener/classes/ScreeningStatistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -691,14 +691,34 @@
                 index -= 1
         else:
             while(diff_df["diff"][index-1] >= 0 and index >=0):
                 index -= 1
         ts = diff_df.tail(len(diff_df)-index +1).head(1).index[-1]
         return ts, df[df.index == ts] #df.head(len(df) -index +1).tail(1)
     
+    # Find stock showing RSI crossing with RSI 9 SMA
+    def findRSICrossingMA(self, df, screenDict, saveDict, maLength=9):
+        if df is None or len(df) == 0:
+            return False
+        data = df.copy()
+        data = data[::-1]
+        maRsi = pktalib.MA(data['RSI'], timeperiod=maLength)
+        data = data[::-1].head(3)
+        maRsi = maRsi[::-1].head(3)
+        saved = self.findCurrentSavedValue(screenDict,saveDict,"Trend")
+        if maRsi.iloc[0] <= data['RSI'].iloc[0] and maRsi.iloc[1] > data['RSI'].iloc[1]:
+            screenDict['MA-Signal'] = saved[0] + colorText.BOLD + colorText.GREEN + f'RSI-MA-Buy' + colorText.END
+            saveDict['MA-Signal'] = saved[1] + f'RSI-MA-Buy'
+            return True
+        elif maRsi.iloc[0] >= data['RSI'].iloc[0] and maRsi.iloc[1] < data['RSI'].iloc[1]:
+            screenDict['MA-Signal'] = saved[0] + colorText.BOLD + colorText.FAIL + f'RSI-MA-Sell' + colorText.END
+            saveDict['MA-Signal'] = saved[1] + f'RSI-MA-Sell'
+            return True
+        return False
+    
     # Find stocks with rising RSI from lower levels
     def findRisingRSI(self, df):
         if df is None or len(df) == 0:
             return False
         data = df.copy()
         data = data[::-1]
         data = data.tail(3)
@@ -903,15 +923,14 @@
         decision = 'T:▲' if isUptrend else ('T:▼' if isDowntrend else '')
         dma50decision = 't:▲' if is50DMAUptrend else ('t:▼' if is50DMADowntrend else '')
         mf_inst_ownershipChange = 0
         change_millions =""
         try:
             mf_inst_ownershipChange = self.getMutualFundStatus(stock,onlyMF=onlyMF,hostData=hostData,force=(hostData is None or hostData.empty or not ("MF" in hostData.columns or "FII" in hostData.columns)),exchangeName=exchangeName)
             if isinstance(mf_inst_ownershipChange, pd.Series):
-                print(f"Unexpected mf_inst_ownershipChange:{mf_inst_ownershipChange}")
                 mf_inst_ownershipChange = 0
             roundOff = 2
             millions = round(mf_inst_ownershipChange/1000000,roundOff)
             while float(millions) == 0 and roundOff <=5:
                 roundOff +=1
                 millions = round(mf_inst_ownershipChange/1000000,roundOff)
             change_millions = f"({millions}M)"
```

### Comparing `pkscreener-0.44.20240414.260/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240414.261/pkscreener/classes/StockScreener.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,15 @@
                 if not screener.validateNewlyListed(fullData, period):
                     raise ScreeningStatistics.NotNewlyListed
 
             if processedData.empty:
                 return returnLegibleData()
             
             with SuppressOutput(suppress_stderr=(logLevel==logging.NOTSET), suppress_stdout=(not (printCounter or testbuild))):
-                self.updateStock(stock, screeningDictionary, saveDictionary, executeOption)
+                self.updateStock(stock, screeningDictionary, saveDictionary, executeOption, exchangeName)
                 
                 self.performBasicLTPChecks(executeOption, screeningDictionary, saveDictionary, fullData, configManager, screener, exchangeName)
                 hasMinVolumeRatio = self.performBasicVolumeChecks(executeOption, volumeRatio, screeningDictionary, saveDictionary, processedData, configManager, screener)
                 
                 isConfluence = False
                 isInsideBar = 0
                 isMaReversal = 0
@@ -152,14 +152,15 @@
                 isMaSupport = False
                 isLorentzian = False
                 isVCP = False
                 isVSA = False
                 isNR = False
                 hasPsarRSIReversal = False
                 hasRisingRSIReversal = False
+                hasRSIMAReversal = False
                 isValidRsi = False
                 isBuyingTrendline = False
                 isMomentum = False
                 mfiStake = 0
                 fairValueDiff = 0
                 consolidationValue = 0
                 isBreaking = False
@@ -215,15 +216,20 @@
                 elif executeOption == 5:
                     isValidRsi = screener.validateRSI(
                         processedData, screeningDictionary, saveDictionary, minRSI, maxRSI
                     )
                     if not isValidRsi:
                         return returnLegibleData()
                 elif executeOption == 6:
-                    if reversalOption == 9:
+                    if reversalOption == 10:
+                        hasRSIMAReversal = screener.findRSICrossingMA(processedData,screeningDictionary,
+                            saveDictionary)
+                        if not hasRSIMAReversal:
+                            return returnLegibleData()
+                    elif reversalOption == 9:
                         hasRisingRSIReversal = screener.findRisingRSI(processedData)
                         if not hasRisingRSIReversal:
                             return returnLegibleData()
                     elif reversalOption == 8:
                         hasPsarRSIReversal = screener.findPSARReversalWithRSI(
                             processedData,
                             screeningDictionary,
@@ -428,14 +434,15 @@
                                                                     and saveDictionary["Pattern"]
                                                                     in CandlePatterns.reversalPatternsBullish
                                                                 ))
                                                                 or (reversalOption == 6 and isNR)
                                                                 or (reversalOption == 7 and isLorentzian)
                                                                 or (reversalOption == 8 and hasPsarRSIReversal)
                                                                 or (reversalOption == 9 and hasRisingRSIReversal)
+                                                                or (reversalOption == 10 and hasRSIMAReversal)
                                                                 ))
                         or ((executeOption == 7) and ((respChartPattern < 3 and isInsideBar > 0) 
                                                                   or (isConfluence)
                                                                   or (isIpoBase and newlyListedOnly and not respChartPattern < 3)
                                                                   or (isVCP)
                                                                   or (isBuyingTrendline))
                                                                   or (respChartPattern == 6 and hasBbandsSqz)
@@ -633,19 +640,19 @@
                     maxLTP=configManager.maxLTP,
                 )
         if not isLtpValid:
             raise ScreeningStatistics.LTPNotInConfiguredRange
         if configManager.stageTwo and not verifyStageTwo and executeOption > 0:
             raise ScreeningStatistics.NotAStageTwoStock
 
-    def updateStock(self, stock, screeningDictionary, saveDictionary, executeOption=0):
+    def updateStock(self, stock, screeningDictionary, saveDictionary, executeOption=0,exchangeName='INDIA'):
         screeningDictionary["Stock"] = (
                     colorText.WHITE
                     + (
-                        f"\x1B]8;;https://in.tradingview.com/chart?symbol=NSE%3A{stock}\x1B\\{stock}\x1B]8;;\x1B\\"
+                        f"\x1B]8;;https://in.tradingview.com/chart?symbol={'NSE' if exchangeName=='INDIA' else 'NASDAQ'}%3A{stock}\x1B\\{stock}\x1B]8;;\x1B\\"
                     )
                     + colorText.END
                 ) if executeOption != 26 else stock
         saveDictionary["Stock"] = stock
 
     def getCleanedDataForDuration(self, backtestDuration, portfolio, screeningDictionary, saveDictionary, configManager, screener, data):
         fullData = None
```

### Comparing `pkscreener-0.44.20240414.260/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240414.261/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.260/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240414.261/pkscreener/classes/Utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -1207,15 +1207,15 @@
                 input(
                     colorText.BOLD
                     + colorText.WARN
                     + """[+] Select Option:"""
                     + colorText.END
                 )
             )
-            if resp >= 0 and resp <= 9:
+            if resp >= 0 and resp <= 10:
                 if resp == 4:
                     try:
                         maLength = int(
                             input(
                                 colorText.BOLD
                                 + colorText.WARN
                                 + "\n[+] Enter MA Length (E.g. 50 or 200): "
```

### Comparing `pkscreener-0.44.20240414.260/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240414.261/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.260/pkscreener/classes/keys.py` & `pkscreener-0.44.20240414.261/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.260/pkscreener/courbd.ttf` & `pkscreener-0.44.20240414.261/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.260/pkscreener/globals.py` & `pkscreener-0.44.20240414.261/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.260/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240414.261/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.260/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240414.261/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.260/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240414.261/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.260/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240414.261/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240414.260
+Version: 0.44.20240414.261
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240414.260.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240414.261.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.259/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.260/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.259/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.260/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240413.259/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.260/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240414.260/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240414.261/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.260/setup.py` & `pkscreener-0.44.20240414.261/setup.py`

 * *Files identical despite different names*

