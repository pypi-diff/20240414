# Comparing `tmp/tradingview_indicators-0.3.7.tar.gz` & `tmp/tradingview_indicators-0.3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradingview_indicators-0.3.7.tar", last modified: Mon Nov 13 20:33:13 2023, max compression
+gzip compressed data, was "tradingview_indicators-0.3.7.1.tar", last modified: Tue Nov 14 17:39:29 2023, max compression
```

## Comparing `tradingview_indicators-0.3.7.tar` & `tradingview_indicators-0.3.7.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-11-13 20:33:13.103759 tradingview_indicators-0.3.7/
--rw-rw-rw-   0        0        0     1857 2023-11-13 20:33:13.100454 tradingview_indicators-0.3.7/PKG-INFO
--rw-rw-rw-   0        0        0     1207 2023-11-01 02:44:40.000000 tradingview_indicators-0.3.7/README.md
--rw-rw-rw-   0        0        0       42 2023-11-13 20:33:13.104756 tradingview_indicators-0.3.7/setup.cfg
--rw-rw-rw-   0        0        0      939 2023-11-13 20:32:05.000000 tradingview_indicators-0.3.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-13 20:33:13.085462 tradingview_indicators-0.3.7/tradingview_indicators/
--rw-rw-rw-   0        0        0     4257 2023-09-06 21:48:29.000000 tradingview_indicators-0.3.7/tradingview_indicators/CCI.py
--rw-rw-rw-   0        0        0     6504 2023-11-13 20:31:54.000000 tradingview_indicators-0.3.7/tradingview_indicators/DMI.py
--rw-rw-rw-   0        0        0     3736 2023-09-06 21:24:50.000000 tradingview_indicators-0.3.7/tradingview_indicators/MACD.py
--rw-rw-rw-   0        0        0      974 2023-09-06 21:24:48.000000 tradingview_indicators-0.3.7/tradingview_indicators/RSI.py
--rw-rw-rw-   0        0        0      200 2023-11-01 01:57:44.000000 tradingview_indicators-0.3.7/tradingview_indicators/__init__.py
--rw-rw-rw-   0        0        0     3020 2023-11-01 02:20:21.000000 tradingview_indicators-0.3.7/tradingview_indicators/ichimoku.py
--rw-rw-rw-   0        0        0     6921 2023-08-29 23:51:45.000000 tradingview_indicators-0.3.7/tradingview_indicators/moving_average.py
--rw-rw-rw-   0        0        0     5654 2023-09-06 21:27:36.000000 tradingview_indicators-0.3.7/tradingview_indicators/stoch.py
--rw-rw-rw-   0        0        0     3028 2023-11-13 20:31:54.000000 tradingview_indicators-0.3.7/tradingview_indicators/utils.py
-drwxrwxrwx   0        0        0        0 2023-11-13 20:33:13.098462 tradingview_indicators-0.3.7/tradingview_indicators.egg-info/
--rw-rw-rw-   0        0        0     1857 2023-11-13 20:33:12.000000 tradingview_indicators-0.3.7/tradingview_indicators.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      543 2023-11-13 20:33:13.000000 tradingview_indicators-0.3.7/tradingview_indicators.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-13 20:33:12.000000 tradingview_indicators-0.3.7/tradingview_indicators.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-11-13 20:33:12.000000 tradingview_indicators-0.3.7/tradingview_indicators.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-11-13 20:33:13.000000 tradingview_indicators-0.3.7/tradingview_indicators.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-11-14 17:39:29.158616 tradingview_indicators-0.3.7.1/
+-rw-rw-rw-   0        0        0     1859 2023-11-14 17:39:29.155627 tradingview_indicators-0.3.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1207 2023-11-01 02:44:40.000000 tradingview_indicators-0.3.7.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-11-14 17:39:29.158616 tradingview_indicators-0.3.7.1/setup.cfg
+-rw-rw-rw-   0        0        0      941 2023-11-14 17:37:16.000000 tradingview_indicators-0.3.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-11-14 17:39:29.140677 tradingview_indicators-0.3.7.1/tradingview_indicators/
+-rw-rw-rw-   0        0        0     4257 2023-09-06 21:48:29.000000 tradingview_indicators-0.3.7.1/tradingview_indicators/CCI.py
+-rw-rw-rw-   0        0        0     6491 2023-11-14 17:37:39.000000 tradingview_indicators-0.3.7.1/tradingview_indicators/DMI.py
+-rw-rw-rw-   0        0        0     3736 2023-09-06 21:24:50.000000 tradingview_indicators-0.3.7.1/tradingview_indicators/MACD.py
+-rw-rw-rw-   0        0        0      974 2023-09-06 21:24:48.000000 tradingview_indicators-0.3.7.1/tradingview_indicators/RSI.py
+-rw-rw-rw-   0        0        0      200 2023-11-01 01:57:44.000000 tradingview_indicators-0.3.7.1/tradingview_indicators/__init__.py
+-rw-rw-rw-   0        0        0     3020 2023-11-01 02:20:21.000000 tradingview_indicators-0.3.7.1/tradingview_indicators/ichimoku.py
+-rw-rw-rw-   0        0        0     6921 2023-08-29 23:51:45.000000 tradingview_indicators-0.3.7.1/tradingview_indicators/moving_average.py
+-rw-rw-rw-   0        0        0     5654 2023-09-06 21:27:36.000000 tradingview_indicators-0.3.7.1/tradingview_indicators/stoch.py
+-rw-rw-rw-   0        0        0     3028 2023-11-13 20:31:54.000000 tradingview_indicators-0.3.7.1/tradingview_indicators/utils.py
+drwxrwxrwx   0        0        0        0 2023-11-14 17:39:29.152636 tradingview_indicators-0.3.7.1/tradingview_indicators.egg-info/
+-rw-rw-rw-   0        0        0     1859 2023-11-14 17:39:29.000000 tradingview_indicators-0.3.7.1/tradingview_indicators.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      543 2023-11-14 17:39:29.000000 tradingview_indicators-0.3.7.1/tradingview_indicators.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-11-14 17:39:29.000000 tradingview_indicators-0.3.7.1/tradingview_indicators.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-11-14 17:39:29.000000 tradingview_indicators-0.3.7.1/tradingview_indicators.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-11-14 17:39:29.000000 tradingview_indicators-0.3.7.1/tradingview_indicators.egg-info/top_level.txt
```

### Comparing `tradingview_indicators-0.3.7/PKG-INFO` & `tradingview_indicators-0.3.7.1/tradingview_indicators.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tradingview_indicators
-Version: 0.3.7
+Name: tradingview-indicators
+Version: 0.3.7.1
 Summary: An accurate calculation of technical analysis indicators with values aligning with those in TradingView.
 Author: m-marqx (Mateus Marques)
 Keywords: python,tradingview,technical analysis,indicators
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `tradingview_indicators-0.3.7/README.md` & `tradingview_indicators-0.3.7.1/README.md`

 * *Files identical despite different names*

### Comparing `tradingview_indicators-0.3.7/setup.py` & `tradingview_indicators-0.3.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.3.7'
+VERSION = '0.3.7.1'
 DESCRIPTION = 'An accurate calculation of technical analysis indicators with values aligning with those in TradingView.'
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name="tradingview_indicators",
```

### Comparing `tradingview_indicators-0.3.7/tradingview_indicators/CCI.py` & `tradingview_indicators-0.3.7.1/tradingview_indicators/CCI.py`

 * *Files identical despite different names*

### Comparing `tradingview_indicators-0.3.7/tradingview_indicators/DMI.py` & `tradingview_indicators-0.3.7.1/tradingview_indicators/DMI.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,41 +5,41 @@
 ma = MovingAverage()
 
 
 class DMI:
     """
     Attributes:
     -----------
-    source : pd.Series
-        The source values from the DataFrame.
+    close : pd.Series
+        The close values from the DataFrame.
     high : pd.Series
         The high prices from the DataFrame.
     low : pd.Series
         The low prices from the DataFrame.
     length : int
         The lookback period for calculating the Stochastic Oscillator.
 
     """
     def __init__(
         self,
         dataframe: pd.DataFrame,
-        source: str = None,
+        close: str = None,
         high: str = None,
         low: str = None,
     ) -> None:
         """
         Initialize the DMI object with the given data and
         parameters.
 
         Parameters:
         -----------
         dataframe : pd.DataFrame
-            The DataFrame containing the source, high, and low data.
-        source : str
-            The column name in the DataFrame representing the source
+            The DataFrame containing the close, high, and low data.
+        close : str
+            The column name in the DataFrame representing the close
             data.
         high : str, optional
             The column name in the DataFrame representing the high
             data. If not provided,
             it will be inferred from common column names.
         low : str, optional
             The column name in the DataFrame representing the low
@@ -47,19 +47,19 @@
             it will be inferred from common column names.
         """
         if not isinstance(dataframe, pd.DataFrame):
             raise ValueError("dataframe param must be a DataFrame")
 
         ohlc_columns_lowercase = ['high', 'low', 'close']
         ohlc_columns_uppercase = ['High', 'Low', 'Close']
-        source_columns = [source, high, low]
+        source_columns = [close, high, low]
 
         is_na_source = all(
-            source is None
-            for source in source_columns
+            close is None
+            for close in source_columns
         )
 
         is_hlc_columns_lowercase = all(
             column in dataframe.columns
             for column in ohlc_columns_lowercase
         )
 
@@ -72,23 +72,23 @@
             not is_hlc_columns_lowercase
             and not is_ohlc_columns_uppercase
         )
 
         if is_na_source and columns_not_found:
             raise ValueError("OHLC columns not found in dataframe")
 
-        if source is None:
+        if close is None:
             if "Close" in dataframe.columns:
                 self.close = dataframe["Close"]
             elif "close" in dataframe.columns:
                 self.close = dataframe["close"]
             else:
                 self.close = None
         else:
-            self.close = dataframe[source]
+            self.close = dataframe[close]
 
         if high is None:
             if "High" in dataframe.columns:
                 self.high = dataframe["High"]
             elif "high" in dataframe.columns:
                 self.high = dataframe["high"]
             else:
@@ -119,16 +119,16 @@
         Returns:
         --------
         pd.Series
             The True Range (TR) values.
         """
         true_range = np.maximum(
             self.high - self.low,
-            abs(self.high - self.source.shift()),
-            abs(self.low - self.source.shift())
+            abs(self.high - self.close.shift()),
+            abs(self.low - self.close.shift())
         )
         return true_range
 
     def adx(
         self,
         adx_smoothing: int = 14,
         di_length: int = 14
```

### Comparing `tradingview_indicators-0.3.7/tradingview_indicators/MACD.py` & `tradingview_indicators-0.3.7.1/tradingview_indicators/MACD.py`

 * *Files identical despite different names*

### Comparing `tradingview_indicators-0.3.7/tradingview_indicators/RSI.py` & `tradingview_indicators-0.3.7.1/tradingview_indicators/RSI.py`

 * *Files identical despite different names*

### Comparing `tradingview_indicators-0.3.7/tradingview_indicators/ichimoku.py` & `tradingview_indicators-0.3.7.1/tradingview_indicators/ichimoku.py`

 * *Files identical despite different names*

### Comparing `tradingview_indicators-0.3.7/tradingview_indicators/moving_average.py` & `tradingview_indicators-0.3.7.1/tradingview_indicators/moving_average.py`

 * *Files identical despite different names*

### Comparing `tradingview_indicators-0.3.7/tradingview_indicators/stoch.py` & `tradingview_indicators-0.3.7.1/tradingview_indicators/stoch.py`

 * *Files identical despite different names*

### Comparing `tradingview_indicators-0.3.7/tradingview_indicators/utils.py` & `tradingview_indicators-0.3.7.1/tradingview_indicators/utils.py`

 * *Files identical despite different names*

### Comparing `tradingview_indicators-0.3.7/tradingview_indicators.egg-info/PKG-INFO` & `tradingview_indicators-0.3.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tradingview-indicators
-Version: 0.3.7
+Name: tradingview_indicators
+Version: 0.3.7.1
 Summary: An accurate calculation of technical analysis indicators with values aligning with those in TradingView.
 Author: m-marqx (Mateus Marques)
 Keywords: python,tradingview,technical analysis,indicators
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `tradingview_indicators-0.3.7/tradingview_indicators.egg-info/SOURCES.txt` & `tradingview_indicators-0.3.7.1/tradingview_indicators.egg-info/SOURCES.txt`

 * *Files identical despite different names*

