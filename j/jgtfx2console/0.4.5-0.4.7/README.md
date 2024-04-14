# Comparing `tmp/jgtfx2console-0.4.5.tar.gz` & `tmp/jgtfx2console-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jgtfx2console-0.4.5.tar", last modified: Tue Mar 26 23:26:36 2024, max compression
+gzip compressed data, was "jgtfx2console-0.4.7.tar", last modified: Sun Apr 14 12:04:36 2024, max compression
```

## Comparing `jgtfx2console-0.4.5.tar` & `jgtfx2console-0.4.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-03-26 23:26:36.553902 jgtfx2console-0.4.5/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1086 2024-03-16 22:23:35.000000 jgtfx2console-0.4.5/LICENSE
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1395 2024-03-26 23:26:36.553902 jgtfx2console-0.4.5/PKG-INFO
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      696 2024-03-16 22:23:35.000000 jgtfx2console-0.4.5/README.md
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      205 2024-03-16 22:23:35.000000 jgtfx2console-0.4.5/README.rst
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-03-26 23:26:36.549902 jgtfx2console-0.4.5/jgtfx2console/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1610 2024-03-26 23:26:34.000000 jgtfx2console-0.4.5/jgtfx2console/__init__.py
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-03-26 23:26:36.553902 jgtfx2console-0.4.5/jgtfx2console/forexconnect/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1649 2024-01-14 01:04:03.000000 jgtfx2console-0.4.5/jgtfx2console/forexconnect/EachRowListener.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)    25755 2024-01-14 01:04:03.000000 jgtfx2console-0.4.5/jgtfx2console/forexconnect/ForexConnect.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     9925 2024-01-14 01:04:03.000000 jgtfx2console-0.4.5/jgtfx2console/forexconnect/LiveHistory.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     8003 2024-01-14 01:04:03.000000 jgtfx2console-0.4.5/jgtfx2console/forexconnect/ResponseListener.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     4783 2024-01-14 01:04:03.000000 jgtfx2console-0.4.5/jgtfx2console/forexconnect/SessionStatusListener.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     5900 2024-01-14 01:04:03.000000 jgtfx2console-0.4.5/jgtfx2console/forexconnect/TableListener.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     3121 2024-01-14 01:04:03.000000 jgtfx2console-0.4.5/jgtfx2console/forexconnect/TableManagerListener.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     2125 2024-01-14 01:04:03.000000 jgtfx2console-0.4.5/jgtfx2console/forexconnect/__init__.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)    19128 2024-01-14 01:04:03.000000 jgtfx2console-0.4.5/jgtfx2console/forexconnect/common.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      931 2024-01-14 01:04:03.000000 jgtfx2console-0.4.5/jgtfx2console/forexconnect/errors.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      437 2024-01-14 01:04:03.000000 jgtfx2console-0.4.5/jgtfx2console/forexconnect/x-pyd.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     6180 2024-03-16 22:06:11.000000 jgtfx2console-0.4.5/jgtfx2console/fxcli2console.py
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-03-26 23:26:36.549902 jgtfx2console-0.4.5/jgtfx2console.egg-info/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1395 2024-03-26 23:26:36.000000 jgtfx2console-0.4.5/jgtfx2console.egg-info/PKG-INFO
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      817 2024-03-26 23:26:36.000000 jgtfx2console-0.4.5/jgtfx2console.egg-info/SOURCES.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)        1 2024-03-26 23:26:36.000000 jgtfx2console-0.4.5/jgtfx2console.egg-info/dependency_links.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       67 2024-03-26 23:26:36.000000 jgtfx2console-0.4.5/jgtfx2console.egg-info/entry_points.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      328 2024-03-26 23:26:36.000000 jgtfx2console-0.4.5/jgtfx2console.egg-info/requires.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       14 2024-03-26 23:26:36.000000 jgtfx2console-0.4.5/jgtfx2console.egg-info/top_level.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      693 2024-03-26 23:26:34.000000 jgtfx2console-0.4.5/pyproject.toml
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      103 2024-03-26 23:26:36.553902 jgtfx2console-0.4.5/setup.cfg
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1814 2024-03-26 23:26:17.000000 jgtfx2console-0.4.5/setup.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-14 12:04:36.572939 jgtfx2console-0.4.7/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1086 2024-03-16 22:23:35.000000 jgtfx2console-0.4.7/LICENSE
+-rw-r--r--   0 jgi       (1000) jgi       (1000)     2224 2024-04-14 12:04:36.572939 jgtfx2console-0.4.7/PKG-INFO
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      696 2024-03-16 22:23:35.000000 jgtfx2console-0.4.7/README.md
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      205 2024-03-16 22:23:35.000000 jgtfx2console-0.4.7/README.rst
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-14 12:04:36.568940 jgtfx2console-0.4.7/jgtfx2console/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1610 2024-04-14 11:59:58.000000 jgtfx2console-0.4.7/jgtfx2console/__init__.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-14 12:04:36.568940 jgtfx2console-0.4.7/jgtfx2console/forexconnect/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1649 2024-01-14 01:04:03.000000 jgtfx2console-0.4.7/jgtfx2console/forexconnect/EachRowListener.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)    25755 2024-01-14 01:04:03.000000 jgtfx2console-0.4.7/jgtfx2console/forexconnect/ForexConnect.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     9925 2024-01-14 01:04:03.000000 jgtfx2console-0.4.7/jgtfx2console/forexconnect/LiveHistory.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     8003 2024-01-14 01:04:03.000000 jgtfx2console-0.4.7/jgtfx2console/forexconnect/ResponseListener.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     4783 2024-01-14 01:04:03.000000 jgtfx2console-0.4.7/jgtfx2console/forexconnect/SessionStatusListener.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     5900 2024-01-14 01:04:03.000000 jgtfx2console-0.4.7/jgtfx2console/forexconnect/TableListener.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     3121 2024-01-14 01:04:03.000000 jgtfx2console-0.4.7/jgtfx2console/forexconnect/TableManagerListener.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     2125 2024-01-14 01:04:03.000000 jgtfx2console-0.4.7/jgtfx2console/forexconnect/__init__.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)    19128 2024-01-14 01:04:03.000000 jgtfx2console-0.4.7/jgtfx2console/forexconnect/common.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      931 2024-01-14 01:04:03.000000 jgtfx2console-0.4.7/jgtfx2console/forexconnect/errors.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      437 2024-01-14 01:04:03.000000 jgtfx2console-0.4.7/jgtfx2console/forexconnect/x-pyd.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     7504 2024-04-14 11:54:49.000000 jgtfx2console-0.4.7/jgtfx2console/fxcli2console.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-14 12:04:36.568940 jgtfx2console-0.4.7/jgtfx2console.egg-info/
+-rw-r--r--   0 jgi       (1000) jgi       (1000)     2224 2024-04-14 12:04:36.000000 jgtfx2console-0.4.7/jgtfx2console.egg-info/PKG-INFO
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      817 2024-04-14 12:04:36.000000 jgtfx2console-0.4.7/jgtfx2console.egg-info/SOURCES.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)        1 2024-04-14 12:04:36.000000 jgtfx2console-0.4.7/jgtfx2console.egg-info/dependency_links.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       67 2024-04-14 12:04:36.000000 jgtfx2console-0.4.7/jgtfx2console.egg-info/entry_points.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      328 2024-04-14 12:04:36.000000 jgtfx2console-0.4.7/jgtfx2console.egg-info/requires.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       14 2024-04-14 12:04:36.000000 jgtfx2console-0.4.7/jgtfx2console.egg-info/top_level.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      693 2024-04-14 12:03:06.000000 jgtfx2console-0.4.7/pyproject.toml
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      103 2024-04-14 12:04:36.572939 jgtfx2console-0.4.7/setup.cfg
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1814 2024-04-14 11:57:45.000000 jgtfx2console-0.4.7/setup.py
```

### Comparing `jgtfx2console-0.4.5/LICENSE` & `jgtfx2console-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jgtfx2console-0.4.5/README.md` & `jgtfx2console-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `jgtfx2console-0.4.5/jgtfx2console/__init__.py` & `jgtfx2console-0.4.7/jgtfx2console/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 Jean Guillaume Isabelle
+# Copyright 2024 Jean Guillaume Isabelle
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -38,10 +38,10 @@
 import warnings
 
 with warnings.catch_warnings():
     warnings.filterwarnings("ignore", category=RuntimeWarning, module="importlib._bootstrap")
     # your code here
 
 
-__version__ = "0.4.5"
+__version__ = "0.4.7"
```

### Comparing `jgtfx2console-0.4.5/jgtfx2console/forexconnect/EachRowListener.py` & `jgtfx2console-0.4.7/jgtfx2console/forexconnect/EachRowListener.py`

 * *Files identical despite different names*

### Comparing `jgtfx2console-0.4.5/jgtfx2console/forexconnect/ForexConnect.py` & `jgtfx2console-0.4.7/jgtfx2console/forexconnect/ForexConnect.py`

 * *Files identical despite different names*

### Comparing `jgtfx2console-0.4.5/jgtfx2console/forexconnect/LiveHistory.py` & `jgtfx2console-0.4.7/jgtfx2console/forexconnect/LiveHistory.py`

 * *Files identical despite different names*

### Comparing `jgtfx2console-0.4.5/jgtfx2console/forexconnect/ResponseListener.py` & `jgtfx2console-0.4.7/jgtfx2console/forexconnect/ResponseListener.py`

 * *Files identical despite different names*

### Comparing `jgtfx2console-0.4.5/jgtfx2console/forexconnect/SessionStatusListener.py` & `jgtfx2console-0.4.7/jgtfx2console/forexconnect/SessionStatusListener.py`

 * *Files identical despite different names*

### Comparing `jgtfx2console-0.4.5/jgtfx2console/forexconnect/TableListener.py` & `jgtfx2console-0.4.7/jgtfx2console/forexconnect/TableListener.py`

 * *Files identical despite different names*

### Comparing `jgtfx2console-0.4.5/jgtfx2console/forexconnect/TableManagerListener.py` & `jgtfx2console-0.4.7/jgtfx2console/forexconnect/TableManagerListener.py`

 * *Files identical despite different names*

### Comparing `jgtfx2console-0.4.5/jgtfx2console/forexconnect/__init__.py` & `jgtfx2console-0.4.7/jgtfx2console/forexconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `jgtfx2console-0.4.5/jgtfx2console/forexconnect/common.py` & `jgtfx2console-0.4.7/jgtfx2console/forexconnect/common.py`

 * *Files identical despite different names*

### Comparing `jgtfx2console-0.4.5/jgtfx2console/forexconnect/errors.py` & `jgtfx2console-0.4.7/jgtfx2console/forexconnect/errors.py`

 * *Files identical despite different names*

### Comparing `jgtfx2console-0.4.5/jgtfx2console/fxcli2console.py` & `jgtfx2console-0.4.7/jgtfx2console/fxcli2console.py`

 * *Files 17% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 user_id = os.getenv('user_id')
 password = os.getenv('password')
 url = os.getenv('url')
 connection = os.getenv('connection')
 quotes_count = os.getenv('quotes_count')
 
 #from jgtpy import jgtcommon as jgtcomm,iprops
-from jgtutils import jgtcommon as jgtcomm,iprops
+from jgtutils import jgtcommon as jgtcomm,iprops,jgtconstants as c
 
 ##import jgtcommon as jgtcomm,iprops
 
 import common_samples
 """
 
 url='https://www.fxcorporate.com/Hosts.jsp'
@@ -59,23 +59,31 @@
     parser = argparse.ArgumentParser(description='Process command parameters.')
     #jgtcomm.add_main_arguments(parser)
     jgtcomm.add_instrument_timeframe_arguments(parser)
     #common_samples.add_date_arguments(parser)
     jgtcomm.add_tlid_range_argument(parser)
     #jgtcomm.add_date_arguments(parser)
     jgtcomm.add_max_bars_arguments(parser)
+    jgtcomm.add_keepbidask_argument(parser)
     args = parser.parse_args()
     return args
 
 
 def main():
     args = parse_args()
     str_user_id = user_id#args.l
     str_password = password#args.p
     str_url = url#args.u
+    
+    keep_bid_ask = args.keepbidask
+    #env variable bypass if env exist JGT_KEEP_BID_ASK=1, keep_bid_ask = True
+    if os.getenv("JGT_KEEP_BID_ASK","0") == "1":
+        print("KEEP BID ASK ENV VAR ON (bypassing the --keepbidask argument)")
+        keep_bid_ask = True
+        
     using_tlid = False
     if args.tlidrange is not None:
       using_tlid= True
       tlid_range = args.tlidrange
       #print(tlid_range)
       dtf,dtt = jgtcomm.tlid_range_to_start_end_datetime(tlid_range)
       #print(str(dtf) + " " + str(dtt))
@@ -116,38 +124,48 @@
             if current_unit == fxcorepy.O2GTimeFrameUnit.TICK:
                 print("Date, Bid, Ask")
                 #print(history.dtype.names)
                 for row in history:
                     print("{0:s}, {1:,.5f}, {2:,.5f}".format(
                         pd.to_datetime(str(row['Date'])).strftime(date_format), row['Bid'], row['Ask']))
             else:
-                print("Date, Open, High, Low, Close, Median, Volume")
+                csv_header_OHLC = "Date,Open,High,Low,Close,Median,Volume"
+                csv_header_OHLCBIDASK="Date,BidOpen,BidHigh,BidLow,BidClose,AskOpen,AskHigh,AskLow,AskClose,Volume,Open,High,Low,Close,Median"
+                csv_header=csv_header_OHLC
+                if keep_bid_ask:
+                    csv_header=csv_header_OHLCBIDASK
+                print(csv_header)
                 rounder = lpip+1
                 for row in history:
-                    print(format_output(rounder,row,rounder,date_format))
+                    print(format_output(rounder,row,rounder,date_format,keep_bid_ask=keep_bid_ask))
                     
                     # print("{0:s},{1:.5f},{2:.5f},{3:.5f},{4:.5f},{5:.5f},{6:d}".format(                    
                     #     pd.to_datetime(str(row['Date'])).strftime(date_format), open_price, high_price,
                     #     low_price, close_price, median, row['Volume']))
         except Exception as e:
             jgtcomm.print_exception(e)
         try:
             fx.logout()
         except Exception as e:
             jgtcomm.print_exception(e)
 
-def format_output(nb_decimal, row, rounder, date_format = '%Y-%m-%d %H:%M:%S'):
-    open_price = round(((row['BidOpen'] + row['AskOpen']) / 2), rounder)
-    high_price = round(((row['BidHigh'] + row['AskHigh']) / 2), rounder)
-    low_price = round(((row['BidLow'] + row['AskLow']) / 2), rounder)
-    close_price = round(((row['BidClose'] + row['AskClose']) / 2), rounder)
+def format_output(nb_decimal, row, rounder, date_format = '%Y-%m-%d %H:%M:%S',keep_bid_ask=False):
+    open_price = round(((row[c.BIDOPEN] + row[c.ASKOPEN]) / 2), rounder)
+    high_price = round(((row[c.BIDHIGH] + row[c.ASKHIGH]) / 2), rounder)
+    low_price = round(((row[c.BIDLOW] + row[c.ASKLOW]) / 2), rounder)
+    close_price = round(((row[c.BIDCLOSE] + row[c.ASKCLOSE]) / 2), rounder)
     median = round(((high_price + low_price) / 2), rounder)
-    dt_formatted=pd.to_datetime(str(row['Date'])).strftime(date_format)
+    dt_formatted=pd.to_datetime(str(row[c.DATE])).strftime(date_format)
     #print("dt formatted: " + dt_formatted)
-    formatted_string = f"{dt_formatted},{open_price:.{nb_decimal}f},{high_price:.{nb_decimal}f},{low_price:.{nb_decimal}f},{close_price:.{nb_decimal}f},{median:.{nb_decimal}f},{row['Volume']:d}"
+    #if keep_bid_ask:Date,BidOpen,BidHigh,BidLow,BidClose,AskOpen,AskHigh,AskLow,AskClose,Volume,Open,High,Low,Close,Median
+    if keep_bid_ask:
+        formatted_string = f"{dt_formatted},{row[c.BIDOPEN]:.{nb_decimal}f},{row[c.BIDHIGH]:.{nb_decimal}f},{row[c.BIDLOW]:.{nb_decimal}f},{row[c.BIDCLOSE]:.{nb_decimal}f},{row[c.ASKOPEN]:.{nb_decimal}f},{row[c.ASKHIGH]:.{nb_decimal}f},{row[c.ASKLOW]:.{nb_decimal}f},{row[c.ASKCLOSE]:.{nb_decimal}f},{row[c.VOLUME]:d},{open_price:.{nb_decimal}f},{high_price:.{nb_decimal}f},{low_price:.{nb_decimal}f},{close_price:.{nb_decimal}f},{median:.{nb_decimal}f}"
+    else:
+        formatted_string = f"{dt_formatted},{open_price:.{nb_decimal}f},{high_price:.{nb_decimal}f},{low_price:.{nb_decimal}f},{close_price:.{nb_decimal}f},{median:.{nb_decimal}f},{row['Volume']:d}"
+        
     return formatted_string
   
 def format_output1(nb_decimal, row, rounder,date_format = '%Y-%m-%d %H:%M:%S'):
     open_price = round(((row['BidOpen'] + row['AskOpen']) / 2),rounder)
     high_price = round(((row['BidHigh'] + row['AskHigh']) / 2),rounder)
     low_price = round(((row['BidLow'] + row['AskLow']) / 2),rounder)
     close_price = round(((row['BidClose'] + row['AskClose']) / 2),rounder)
```

### Comparing `jgtfx2console-0.4.5/jgtfx2console.egg-info/SOURCES.txt` & `jgtfx2console-0.4.7/jgtfx2console.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jgtfx2console-0.4.5/pyproject.toml` & `jgtfx2console-0.4.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["setuptools>=40.8.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jgtfx2console"
-version = "0.4.5"
+version = "0.4.7"
 authors = [
   { name="Guillaume Isabelle", email="jgi@jgwill.com" },
 ]
 
 description = "PDS Services"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
   'pandas>=0.25.1',
   'python-dotenv>=0.19.2',
-  'jgtutils>=0.1.47',
+  'jgtutils>=0.1.57',
   'tlid',
   'flask'
 ]	
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `jgtfx2console-0.4.5/setup.py` & `jgtfx2console-0.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 
 
 INSTALL_REQUIRES = [
     'pandas>=0.25.1',
     'python-dotenv>=0.19.2',
-    'jgtutils>=0.1.47',
+    'jgtutils>=0.1.57',
     'tlid',
     'flask'
 ]
 
 EXTRAS_DEV_LINT = [
     "flake8>=3.6.0,<3.7.0",
     "isort>=4.3.4,<4.4.0",
```

