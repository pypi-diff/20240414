# Comparing `tmp/geoglows-1.1.tar.gz` & `tmp/geoglows-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoglows-1.1.tar", last modified: Fri Apr 12 18:20:01 2024, max compression
+gzip compressed data, was "geoglows-1.2.0.tar", last modified: Sun Apr 14 04:36:00 2024, max compression
```

## Comparing `geoglows-1.1.tar` & `geoglows-1.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:20:01.776823 geoglows-1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-12 18:19:53.000000 geoglows-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-12 18:19:53.000000 geoglows-1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-12 18:20:01.776823 geoglows-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-12 18:19:53.000000 geoglows-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:20:01.772823 geoglows-1.1/geoglows/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:20:01.776823 geoglows-1.1/geoglows/_plots/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/_plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/_plots/format_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/_plots/plotly_bias_corrected.py
--rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/_plots/plotly_forecasts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/_plots/plotly_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/_plots/plotly_retrospective.py
--rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/_plots/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/bias.py
--rw-r--r--   0 runner    (1001) docker     (127)    14367 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    15652 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/streamflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:20:01.776823 geoglows-1.1/geoglows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-12 18:20:01.000000 geoglows-1.1/geoglows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-12 18:20:01.000000 geoglows-1.1/geoglows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:20:01.000000 geoglows-1.1/geoglows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-12 18:20:01.000000 geoglows-1.1/geoglows.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 18:20:01.000000 geoglows-1.1/geoglows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-12 18:19:53.000000 geoglows-1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 18:20:01.776823 geoglows-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-12 18:19:53.000000 geoglows-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:36:00.587682 geoglows-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-14 04:35:54.000000 geoglows-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-14 04:35:54.000000 geoglows-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-14 04:36:00.587682 geoglows-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-14 04:35:54.000000 geoglows-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:36:00.583682 geoglows-1.2.0/geoglows/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:36:00.587682 geoglows-1.2.0/geoglows/_plots/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/_plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/_plots/format_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16447 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/_plots/plotly_bias_corrected.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/_plots/plotly_forecasts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/_plots/plotly_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/_plots/plotly_retrospective.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11701 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/_plots/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15146 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15652 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/streamflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-14 04:35:54.000000 geoglows-1.2.0/geoglows/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:36:00.587682 geoglows-1.2.0/geoglows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-14 04:36:00.000000 geoglows-1.2.0/geoglows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-14 04:36:00.000000 geoglows-1.2.0/geoglows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 04:36:00.000000 geoglows-1.2.0/geoglows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-14 04:36:00.000000 geoglows-1.2.0/geoglows.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 04:36:00.000000 geoglows-1.2.0/geoglows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-14 04:35:54.000000 geoglows-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 04:36:00.587682 geoglows-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-14 04:35:54.000000 geoglows-1.2.0/setup.py
```

### Comparing `geoglows-1.1/LICENSE` & `geoglows-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geoglows-1.1/PKG-INFO` & `geoglows-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.1.0
+Version: 1.2.0
 Summary: Package for accessing data from the GEOGLOWS Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
```

### Comparing `geoglows-1.1/README.md` & `geoglows-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `geoglows-1.1/geoglows/_plots/format_tools.py` & `geoglows-1.2.0/geoglows/_plots/format_tools.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.1/geoglows/_plots/plotly_bias_corrected.py` & `geoglows-1.2.0/geoglows/_plots/plotly_bias_corrected.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,39 +3,38 @@
 import plotly.graph_objects as go
 import scipy.stats
 from plotly.offline import plot as offline_plot
 
 from .format_tools import build_title
 from .plotly_helpers import _rperiod_scatters
 
-
 __all__ = [
-    'corrected_historical',
+    'corrected_retrospective',
     'corrected_scatterplots',
     'corrected_day_average',
     'corrected_month_average',
     'corrected_volume_compare',
 ]
 
 
 # BIAS CORRECTION PLOTS
-def corrected_historical(corrected: pd.DataFrame, simulated: pd.DataFrame, observed: pd.DataFrame,
-                         rperiods: pd.DataFrame = None, plot_titles: list = None,
-                         plot_type: str = 'plotly') -> go.Figure or str:
+def corrected_retrospective(corrected: pd.DataFrame, simulated: pd.DataFrame, observed: pd.DataFrame,
+                            rperiods: pd.DataFrame = None, plot_titles: list = None,
+                            plot_type: str = 'plotly') -> go.Figure or str:
     """
     Creates a plot of corrected discharge, observed discharge, and simulated discharge
 
     Args:
         corrected: the response from the geoglows.bias.correct_historical_simulation function\
         simulated: the csv response from historic_simulation
         observed: the dataframe of observed data. Must have a datetime index and a single column of flow values
         rperiods: the csv response from return_periods
         plot_type: either 'plotly', or 'plotly_html' (default plotly)
         plot_titles: (dict) Extra info to show on the title of the plot. For example:
-            {'Reach ID': 1234567, 'Drainage Area': '1000km^2'}
+            {'River ID': 1234567, 'Drainage Area': '1000km^2'}
 
     Returns:
          plotly.GraphObject: plotly object, especially for use with python notebooks and the .show() method
     """
     startdate = corrected.index[0]
     enddate = corrected.index[-1]
 
@@ -109,15 +108,15 @@
     Args:
         corrected: the response from the geoglows.bias.correct_historical_simulation function
         simulated: the csv response from historic_simulation
         observed: the dataframe of observed data. Must have a datetime index and a single column of flow values
         merged_sim_obs: (optional) if you have already computed it, hydrostats.data.merge_data(simulated, observed)
         merged_cor_obs: (optional) if you have already computed it, hydrostats.data.merge_data(corrected, observed)
         plot_titles: (dict) Extra info to show on the title of the plot. For example:
-            {'Reach ID': 1234567, 'Drainage Area': '1000km^2'}
+            {'River ID': 1234567, 'Drainage Area': '1000km^2'}
 
     Returns:
          plotly.GraphObject: plotly object, especially for use with python notebooks and the .show() method
     """
     if corrected is False and simulated is False and observed is False:
         if merged_sim_obs is not False and merged_cor_obs is not False:
             pass  # if you provided the merged dataframes already, we use those
@@ -197,26 +196,26 @@
     return go.Figure(data=scatter_sets, layout=layout)
 
 
 def corrected_month_average(corrected: pd.DataFrame, simulated: pd.DataFrame, observed: pd.DataFrame,
                             merged_sim_obs: pd.DataFrame = False, merged_cor_obs: pd.DataFrame = False,
                             plot_titles: list = None, ) -> go.Figure or str:
     """
-    Calculates and plots the monthly average streamflow. This function uses
+    Calculates and _plots the monthly average streamflow. This function uses
     hydrostats.data.merge_data on the 3 inputs. If you have already computed these because you are doing a full
     comparison of bias correction, you can provide them to save time
 
     Args:
         corrected: the response from the geoglows.bias.correct_historical_simulation function
         simulated: the csv response from historic_simulation
         observed: the dataframe of observed data. Must have a datetime index and a single column of flow values
         merged_sim_obs: (optional) if you have already computed it, hydrostats.data.merge_data(simulated, observed)
         merged_cor_obs: (optional) if you have already computed it, hydrostats.data.merge_data(corrected, observed)
         plot_titles: (dict) Extra info to show on the title of the plot. For example:
-            {'Reach ID': 1234567, 'Drainage Area': '1000km^2'}
+            {'River ID': 1234567, 'Drainage Area': '1000km^2'}
 
     Returns:
          plotly.GraphObject: plotly object, especially for use with python notebooks and the .show() method
     """
     if corrected is False and simulated is False and observed is False:
         if merged_sim_obs is not False and merged_cor_obs is not False:
             pass  # if you provided the merged dataframes already, we use those
@@ -239,28 +238,28 @@
         showlegend=True)
 
     return go.Figure(data=scatters, layout=layout)
 
 
 def corrected_day_average(corrected: pd.DataFrame, simulated: pd.DataFrame, observed: pd.DataFrame,
                           merged_sim_obs: pd.DataFrame = False, merged_cor_obs: pd.DataFrame = False,
-                          titles: dict = None, ) -> go.Figure or str:
+                          plot_titles: dict = None, ) -> go.Figure or str:
     """
-    Calculates and plots the daily average streamflow. This function uses
+    Calculates and _plots the daily average streamflow. This function uses
     hydrostats.data.merge_data on the 3 inputs. If you have already computed these because you are doing a full
     comparison of bias correction, you can provide them to save time
 
     Args:
         corrected: the response from the geoglows.bias.correct_historical_simulation function
         simulated: the csv response from historic_simulation
         merged_sim_obs: (optional) if you have already computed it, hydrostats.data.merge_data(simulated, observed)
         merged_cor_obs: (optional) if you have already computed it, hydrostats.data.merge_data(corrected, observed)
         observed: the dataframe of observed data. Must have a datetime index and a single column of flow values
-        titles: (dict) Extra info to show on the title of the plot. For example:
-            {'Reach ID': 1234567, 'Drainage Area': '1000km^2'}
+        plot_titles: (dict) Extra info to show on the title of the plot. For example:
+            {'River ID': 1234567, 'Drainage Area': '1000km^2'}
 
     Returns:
          plotly.GraphObject: plotly object, especially for use with python notebooks and the .show() method
     """
     if corrected is False and simulated is False and observed is False:
         if merged_sim_obs is not False and merged_cor_obs is not False:
             pass  # if you provided the merged dataframes already, we use those
@@ -274,37 +273,37 @@
     scatters = [
         go.Scatter(x=daily_avg.index, y=daily_avg.iloc[:, 1].values, name='Observed Data'),
         go.Scatter(x=daily_avg.index, y=daily_avg.iloc[:, 0].values, name='Simulated Data'),
         go.Scatter(x=daily_avg2.index, y=daily_avg2.iloc[:, 0].values, name='Corrected Simulated Data'),
     ]
 
     layout = go.Layout(
-        title=build_title('Daily Average Streamflow Comparison', titles),
+        title=build_title('Daily Average Streamflow Comparison', plot_titles),
         xaxis=dict(title='Days'), yaxis=dict(title='Discharge (m<sup>3</sup>/s)', autorange=True),
         showlegend=True)
 
     return go.Figure(data=scatters, layout=layout)
 
 
 def corrected_volume_compare(corrected: pd.DataFrame, simulated: pd.DataFrame, observed: pd.DataFrame,
                              merged_sim_obs: pd.DataFrame = False, merged_cor_obs: pd.DataFrame = False,
                              plot_titles: dict = None, ) -> go.Figure or str:
     """
-    Calculates and plots the cumulative volume output on each of the 3 datasets provided. This function uses
+    Calculates and _plots the cumulative volume output on each of the 3 datasets provided. This function uses
     hydrostats.data.merge_data on the 3 inputs. If you have already computed these because you are doing a full
     comparison of bias correction, you can provide them to save time
 
     Args:
         corrected: the response from the geoglows.bias.correct_historical_simulation function
         simulated: the csv response from historic_simulation
         observed: the dataframe of observed data. Must have a datetime index and a single column of flow values
         merged_sim_obs: (optional) if you have already computed it, hydrostats.data.merge_data(simulated, observed)
         merged_cor_obs: (optional) if you have already computed it, hydrostats.data.merge_data(corrected, observed)
         plot_titles: (dict) Extra info to show on the title of the plot. For example:
-            {'Reach ID': 1234567, 'Drainage Area': '1000km^2'}
+            {'River ID': 1234567, 'Drainage Area': '1000km^2'}
 
     Returns:
          plotly.GraphObject: plotly object, especially for use with python notebooks and the .show() method
     """
     if corrected is False and simulated is False and observed is False:
         if merged_sim_obs is not False and merged_cor_obs is not False:
             pass  # if you provided the merged dataframes already, we use those
```

### Comparing `geoglows-1.1/geoglows/_plots/plotly_forecasts.py` & `geoglows-1.2.0/geoglows/_plots/plotly_forecasts.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.1/geoglows/_plots/plotly_helpers.py` & `geoglows-1.2.0/geoglows/_plots/plotly_helpers.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.1/geoglows/_plots/plotly_retrospective.py` & `geoglows-1.2.0/geoglows/_plots/plotly_retrospective.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pandas as pd
 import plotly.graph_objs as go
 import scipy.stats
-from plotly.offline import plot as offline_plot
 
 from .format_tools import build_title
 from .plotly_helpers import _rperiod_scatters
 
 __all__ = [
     'retrospective',
     'daily_averages',
@@ -22,15 +21,15 @@
     Makes the streamflow ensemble data and metadata into a plotly plot
 
     Args:
         retro: the csv response from historic_simulation
         rp_df: the csv response from return_periods
         plot_type: either 'json', 'plotly', or 'html' (default plotly)
         plot_titles: (dict) Extra info to show on the title of the plot. For example:
-            {'Reach ID': 1234567, 'Drainage Area': '1000km^2'}
+            {'River ID': 1234567, 'Drainage Area': '1000km^2'}
 
     Return:
          plotly.GraphObject: plotly object, especially for use with python notebooks and the .show() method
     """
     dates = retro.index.tolist()
     startdate = dates[0]
     enddate = dates[-1]
@@ -69,15 +68,15 @@
 def daily_averages(dayavg: pd.DataFrame, plot_titles: list = None, plot_type: str = 'plotly') -> go.Figure:
     """
     Makes the daily_averages data and metadata into a plotly plot
 
     Args:
         dayavg: the csv response from daily_averages
         plot_titles: (dict) Extra info to show on the title of the plot. For example:
-            {'Reach ID': 1234567, 'Drainage Area': '1000km^2'}
+            {'River ID': 1234567, 'Drainage Area': '1000km^2'}
         plot_type: either 'plotly', or 'html' (default plotly)
 
     Return:
          plotly.GraphObject: plotly object, especially for use with python notebooks and the .show() method
     """
     if plot_type not in ['plotly_scatters', 'plotly', 'html']:
         raise ValueError('invalid plot_type specified. pick plotly, plotly_scatters, or html')
@@ -93,35 +92,25 @@
     if plot_type == 'plotly_scatters':
         return scatter_plots
     layout = go.Layout(
         title=build_title('Daily Average Streamflow (Simulated)', plot_titles),
         yaxis={'title': 'Streamflow (m<sup>3</sup>/s)', 'range': [0, 'auto']},
         xaxis={'title': 'Date (UTC +0:00)', 'hoverformat': '%b %d', 'tickformat': '%b'},
     )
-    figure = go.Figure(scatter_plots, layout=layout)
-    if plot_type == 'plotly':
-        return figure
-    if plot_type == 'html':
-        return offline_plot(
-            figure,
-            config={'autosizable': True, 'responsive': True},
-            output_type='div',
-            include_plotlyjs=False
-        )
-    raise ValueError('Invalid plot_type chosen. Choose plotly, plotly_scatters, or html')
+    return go.Figure(scatter_plots, layout=layout)
 
 
 def monthly_averages(monavg: pd.DataFrame, titles: dict = None, plot_titles: list = None, plot_type: str = 'plotly') -> go.Figure:
     """
     Makes the daily_averages data and metadata into a plotly plot
 
     Args:
         monavg: the csv response from monthly_averages
         titles: (dict) Extra info to show on the title of the plot. For example:
-            {'Reach ID': 1234567, 'Drainage Area': '1000km^2'}
+            {'River ID': 1234567, 'Drainage Area': '1000km^2'}
         plot_type: either 'plotly', or 'html' (default plotly)
 
     Return:
          plotly.GraphObject: plotly object, especially for use with python notebooks and the .show() method
     """
     if plot_type not in ['plotly_scatters', 'plotly', 'html']:
         raise ValueError('invalid plot_type specified. pick plotly, plotly_scatters, or html')
@@ -137,35 +126,25 @@
     if plot_type == 'plotly_scatters':
         return scatter_plots
     layout = go.Layout(
         title=build_title('Monthly Average Streamflow (Simulated)', plot_titles=plot_titles),
         yaxis={'title': 'Streamflow (m<sup>3</sup>/s)'},
         xaxis={'title': 'Month'},
     )
-    figure = go.Figure(scatter_plots, layout=layout)
-    if plot_type == 'plotly':
-        return figure
-    if plot_type == 'html':
-        return offline_plot(
-            figure,
-            config={'autosizable': True, 'responsive': True},
-            output_type='div',
-            include_plotlyjs=False
-        )
-    raise ValueError('Invalid plot_type chosen. Choose plotly, plotly_scatters, or html')
+    return go.Figure(scatter_plots, layout=layout)
 
 
 def annual_averages(df: pd.DataFrame, *, plot_titles: list = None, ) -> go.Figure:
     """
     Makes the annual_averages data and metadata into a plotly plot
 
     Args:
         df: the csv response from annual_averages
         plot_titles: (dict) Extra info to show on the title of the plot. For example:
-            {'Reach ID': 1234567, 'Drainage Area': '1000km^2'}
+            {'River ID': 1234567, 'Drainage Area': '1000km^2'}
 
     Return:
          plotly.GraphObject: plotly object, especially for use with python notebooks and the .show() method
     """
     scatter_plots = [
         go.Scatter(
             name='Average Annual Flow',
@@ -178,22 +157,22 @@
         title=build_title('Annual Average Streamflow (Simulated)', plot_titles),
         yaxis={'title': 'Streamflow (m<sup>3</sup>/s)'},
         xaxis={'title': 'Year'},
     )
     return go.Figure(scatter_plots, layout=layout)
 
 
-def flow_duration_curve(hist: pd.DataFrame, titles: dict = None, plot_type: str = 'plotly') -> go.Figure:
+def flow_duration_curve(hist: pd.DataFrame, plot_titles: dict = None, plot_type: str = 'plotly') -> go.Figure:
     """
     Makes the streamflow ensemble data and metadata into a plotly plot
 
     Args:
         hist: the csv response from historic_simulation
-        titles: (dict) Extra info to show on the title of the plot. For example:
-            {'Reach ID': 1234567, 'Drainage Area': '1000km^2'}
+        plot_titles: (dict) Extra info to show on the title of the plot. For example:
+            {'River ID': 1234567, 'Drainage Area': '1000km^2'}
         plot_type: either 'json', 'plotly', or 'html' (default plotly)
 
     Return:
          plotly.GraphObject: plotly object, especially for use with python notebooks and the .show() method
     """
     if plot_type not in ['json', 'plotly_scatters', 'plotly', 'html']:
         raise ValueError('invalid plot_type specified. pick json, plotly, plotly_scatters, or html')
@@ -222,39 +201,29 @@
             name='Flow Duration Curve',
             x=plot_data['x_probability'],
             y=plot_data['y_flow'])
     ]
     if plot_type == 'plotly_scatters':
         return scatter_plots
     layout = go.Layout(
-        title=build_title('Flow Duration Curve', titles),
+        title=build_title('Flow Duration Curve', plot_titles),
         xaxis={'title': 'Exceedence Probability'},
         yaxis={'title': 'Streamflow (m<sup>3</sup>/s)', 'range': [0, 'auto']},
     )
-    figure = go.Figure(scatter_plots, layout=layout)
-    if plot_type == 'plotly':
-        return figure
-    if plot_type == 'html':
-        return offline_plot(
-            figure,
-            config={'autosizable': True, 'responsive': True},
-            output_type='div',
-            include_plotlyjs=False
-        )
-    raise ValueError('Invalid plot_type chosen. Choose json, plotly, plotly_scatters, or html')
+    return go.Figure(scatter_plots, layout=layout)
 
 
-def daily_stats(hist: pd.DataFrame, titles: dict = None, plot_type: str = 'plotly') -> go.Figure:
+def daily_stats(hist: pd.DataFrame, *, plot_titles: dict = None, plot_type: str = 'plotly') -> go.Figure:
     """
     Plots a graph with statistics for each day of year
 
     Args:
         hist: dataframe of values to plot
-        titles: (dict) Extra info to show on the title of the plot. For example:
-            {'Reach ID': 1234567, 'Drainage Area': '1000km^2'}
+        plot_titles: (dict) Extra info to show on the title of the plot. For example:
+            {'River ID': 1234567, 'Drainage Area': '1000km^2'}
         plot_type: either 'plotly' (python object, default), 'plotly_scatters', or 'html'
 
     returns:
         plot of the graph of the low flows
     """
 
     stats_df = daily_stats(hist)
@@ -266,57 +235,37 @@
             name=column
         ) for column in stats_df.columns
     ]
 
     if plot_type == 'plotly_scatters':
         return data
     layout = go.Layout(
-        title=build_title('Daily Average Streamflow (Simulated)', titles),
+        title=build_title('Daily Average Streamflow (Simulated)', plot_titles),
         yaxis={'title': 'Streamflow (m<sup>3</sup>/s)', 'range': [0, 'auto']},
         xaxis={'title': 'Date (UTC +0:00)', 'hoverformat': '%b %d', 'tickformat': '%b'},
     )
-    figure = go.Figure(data=data, layout=layout)
-    if plot_type == 'plotly':
-        return figure
-    elif plot_type == 'html':
-        return offline_plot(
-            figure,
-            config={'autosizable': True, 'responsive': True},
-            output_type='div',
-            include_plotlyjs=False
-        )
-    raise ValueError('Invalid plot_type chosen. Choose plotly or html')
+    return go.Figure(data=data, layout=layout)
 
 
 def daily_variance(daily_variance: pd.DataFrame, plot_titles: list = None, plot_type: str = 'plotly') -> go.Figure:
     """
     A dataframe of daily variances computed by the geoglows.analysis.compute_daily_variance function
 
     Args:
       daily_variance: dataframe of values to plot coming from geoglows.analysis.compute_daily_variance
       plot_titles: (dict) Extra info to show on the title of the plot. For example:
-        {'Reach ID': 1234567, 'Drainage Area': '1000km^2'}
+        {'River ID': 1234567, 'Drainage Area': '1000km^2'}
       plot_type: either 'plotly' (python object, default), 'plotly_scatters', or 'html'
 
     returns:
       plot of standard deviation and plot of the graph of the low flows
     """
     data = [
         go.Scatter(
             x=daily_variance['date'],
             y=daily_variance['flow_std'],
             name="Daily Standard Deviation"
         ),
     ]
     if plot_type == 'plotly_scatters':
         return data
-    figure = go.Figure(data=data, layout=go.Layout(build_title('Daily Flow Standard Deviation', plot_titles)))
-    if plot_type == 'plotly':
-        return figure
-    elif plot_type == 'html':
-        return offline_plot(
-            figure,
-            config={'autosizable': True, 'responsive': True},
-            output_type='div',
-            include_plotlyjs=False
-        )
-    raise ValueError('Invalid plot_type chosen. Choose plotly or html')
+    return go.Figure(data=data, layout=go.Layout(build_title('Daily Flow Standard Deviation', plot_titles)))
```

### Comparing `geoglows-1.1/geoglows/analyze.py` & `geoglows-1.2.0/geoglows/analyze.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.1/geoglows/bias.py` & `geoglows-1.2.0/geoglows/bias.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.1/geoglows/data.py` & `geoglows-1.2.0/geoglows/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,60 +44,78 @@
     def from_aws(*args, **kwargs):
         product_name = function.__name__.replace("_", "").lower()
         if product_name == 'forecastrecords':
             warnings.warn('forecast_records are not available from the AWS Open Data Program.')
             return from_rest(*args, **kwargs)
 
         river_id = kwargs.get('river_id', '')
-        river_id = args[0] if len(args) > 0 else None
+        river_id = args[0] if len(args) > 0 else river_id
+
+        return_format = kwargs.get('format', 'df')
+        assert return_format in ('df', 'xarray'), f'Unsupported return format requested: {return_format}'
 
         s3 = s3fs.S3FileSystem(anon=True, client_kwargs=dict(region_name=ODP_S3_BUCKET_REGION))
-        if kwargs.get('date', '') and not product_name == 'dates':
-            date = kwargs['date']
-            if len(date) == 8:
-                date = f'{date}00.zarr'
-            elif len(date) == 10:
-                date = f'{date}.zarr'
-            else:
-                raise ValueError('Date must be YYYYMMDD or YYYYMMDDHH format. Use dates() to view available data.')
-        else:
+        date = kwargs.get('date', False)
+        if not date:
             dates = sorted([x.split('/')[-1] for x in s3.ls(ODP_FORECAST_S3_BUCKET_URI)], reverse=True)
             dates = [x.split('.')[0] for x in dates if x.endswith('.zarr')]  # ignore the index.html file
             dates = [x.replace('00.zarr', '') for x in dates]
             if product_name == 'dates':
                 return pd.DataFrame(dict(dates=dates))
-            date = dates[-1]
+            date = dates[0]
+        if len(date) == 8:
+            date = f'{date}00.zarr'
+        elif len(date) == 10:
+            date = f'{date}.zarr'
+        else:
+            raise ValueError('Date must be YYYYMMDD or YYYYMMDDHH format. Use dates() to view available data.')
+
         s3store = s3fs.S3Map(root=f'{ODP_FORECAST_S3_BUCKET_URI}/{date}', s3=s3, check=False)
 
-        df = xr.open_zarr(s3store).sel(rivid=river_id).to_dataframe().round(2).reset_index()
+        attrs = {
+            'source': 'geoglows',
+            'forecast_date': date[:8],
+            'retrieval_date': pd.Timestamp.now().strftime('%Y%m%d'),
+            'units': 'cubic meters per second',
+        }
+        ds = xr.open_zarr(s3store).sel(rivid=river_id)
+        if return_format == 'xarray' and product_name == 'forecastensembles':
+            ds = ds.rename({'time': 'datetime', 'rivid': 'river_id'})
+            ds.attrs = attrs
+            return ds
+        df = ds.to_dataframe().round(2).reset_index()
 
         # rename columns to match the REST API
         if isinstance(river_id, int):
             df = df.pivot(index='time', columns='ensemble', values='Qout')
         else:
             df = df.pivot(index=['time', 'rivid'], columns='ensemble', values='Qout')
             df.index.names = ['time', 'river_id']
         df = df[sorted(df.columns)]
         df.columns = [f'ensemble_{str(x).zfill(2)}' for x in df.columns]
 
-        if product_name == 'forecastensembles':
-            return df
+        if product_name == 'forecast':
+            df = calc_simple_forecast(df)
         elif product_name == 'forecaststats':
-            return calc_forecast_stats(df)
-        elif product_name == 'forecast':
-            return calc_simple_forecast(df)
-        return
+            df = calc_forecast_stats(df)
+
+        if return_format == 'df':
+            return df
+        ds = df.to_xarray()
+        ds.attrs = attrs
+        return ds
 
     def from_rest(*args, **kwargs):
         # update the default values set by the function unless the user has already specified them
         for key, value in function.__kwdefaults__.items() if function.__kwdefaults__ else []:
             if key not in kwargs:
                 kwargs[key] = value
 
-        return_url = kwargs.get('format', 'csv') == 'url'
+        return_format = kwargs.get('format', 'csv')
+        assert return_format in ('csv', 'json', 'url'), f'Unsupported format requested: {return_format}'
 
         # parse out the information necessary to build a request url
         endpoint = kwargs.get('endpoint', DEFAULT_REST_ENDPOINT)
         endpoint = endpoint[:-1] if endpoint[-1] == '/' else endpoint
         endpoint = endpoint + '/api' if not endpoint.endswith('/api') else endpoint
         endpoint = f'https://{endpoint}' if not endpoint.startswith(('https://', 'http://')) else endpoint
 
@@ -111,17 +129,14 @@
         if isinstance(river_id, list):
             raise ValueError('Multiple river_ids are not available via REST API or on v1. '
                              'Use data_source="aws" and version="v2" for multiple river_ids.')
         river_id = int(river_id) if river_id else None
         if river_id and version == 'v2':
             assert river_id < 1_000_000_000 and river_id >= 110_000_000, ValueError('River ID must be a 9 digit integer')
 
-        return_format = kwargs.get('return_format', 'csv')
-        assert return_format in ('csv', 'json', 'url'), f'Unsupported return format requested: {return_format}'
-
         # request parameter validation before submitting
         for key in ('endpoint', 'version', 'river_id'):
             if key in kwargs:
                 del kwargs[key]
         for key, value in kwargs.items():
             if value is None:
                 del kwargs[key]
@@ -135,15 +150,15 @@
         params = '&'.join([f'{key}={value}' for key, value in kwargs.items()])
 
         # piece together the request url
         request_url = f'{endpoint}/{version}/{product_name}'  # build the base url
         request_url = f'{request_url}/{river_id}' if river_id else request_url  # add the river_id if it exists
         request_url = f'{request_url}?{params}'  # add the query parameters
 
-        if return_url:
+        if return_format == 'url':
             return request_url.replace(f'source={kwargs["source"]}', '')
 
         response = requests.get(request_url)
 
         if response.status_code != 200:
             raise RuntimeError('Received an error from the REST API: ' + response.text)
 
@@ -172,125 +187,126 @@
 # Forecast data and derived products
 @_forecast_endpoint_decorator
 def dates(**kwargs) -> dict or str:
     """
     Gets a list of available forecast product dates
 
     Keyword Args:
-        return_format: csv, json, or url, default csv
         data_source: location to query for data, either 'rest' or 'aws'. default is aws.
 
     Returns:
         dict or str
 
         the csv is a single column with a header of 'available_dates' and 1 row per date, sorted oldest to newest
         The dictionary structure is {'available_dates': ['list', 'of', 'dates', 'YYYYMMDD', 'format']}
     """
     pass
 
 
 @_forecast_endpoint_decorator
-def forecast(*, river_id: int, date: str, return_format: str, data_source: str,
+def forecast(*, river_id: int, date: str, format: str, data_source: str,
              **kwargs) -> pd.DataFrame or dict or str:
     """
     Gets the average forecasted flow for a certain river_id on a certain date
 
     Keyword Args:
         river_id (str): the ID of a stream, should be a 9 digit integer
         date (str): a string specifying the date to request in YYYYMMDD format, returns the latest available if not specified
-        return_format (str): csv, json, or url, default csv
+        format (str): csv, json, or url, default csv
         data_source (str): location to query for data, either 'rest' or 'aws'. default is aws.
-        version (str): the version of the API and model data to retrieve. default is 'v2'. should be 'v1' or 'v2'
 
     Returns:
         pd.DataFrame or dict or str
     """
     pass
 
 
 @_forecast_endpoint_decorator
-def forecast_stats(*, river_id: int, date: str, return_format: str, data_source: str,
+def forecast_stats(*, river_id: int, date: str, format: str, data_source: str,
                    **kwargs) -> pd.DataFrame or dict or str:
     """
     Retrieves the min, 25%, mean, median, 75%, and max river discharge of the 51 ensembles members for a river_id
     The 52nd higher resolution member is excluded
 
     Keyword Args:
         river_id: the ID of a stream, should be a 9 digit integer
         date: a string specifying the date to request in YYYYMMDD format, returns the latest available if not specified
-        return_format: csv, json, or url, default csv
+        format: if data_source=="rest": csv, json, or url, default csv. if data_source=="aws": df or xarray
         data_source: location to query for data, either 'rest' or 'aws'. default is aws.
 
     Returns:
         pd.DataFrame or dict or str
     """
     pass
 
 
 @_forecast_endpoint_decorator
-def forecast_ensembles(*, river_id: int, date: str, return_format: str, data_source: str,
+def forecast_ensembles(*, river_id: int, date: str, format: str, data_source: str,
                        **kwargs) -> pd.DataFrame or dict or str:
     """
     Retrieves each of 52 time series of forecasted discharge for a river_id on a certain date
 
     Keyword Args:
         river_id: the ID of a stream, should be a 9 digit integer
         date: a string specifying the date to request in YYYYMMDD format, returns the latest available if not specified
-        return_format: csv, json, or url, default csv
+        format: if data_source=="rest": csv, json, or url, default csv. if data_source=="aws": df or xarray
         data_source: location to query for data, either 'rest' or 'aws'. default is aws.
 
     Returns:
         pd.DataFrame or dict or str
     """
     pass
 
 
 @_forecast_endpoint_decorator
-def forecast_records(*, river_id: int, start_date: str, end_date: str, return_format: str, data_source: str,
+def forecast_records(*, river_id: int, start_date: str, end_date: str, format: str, data_source: str,
                      **kwargs) -> pd.DataFrame or dict or str:
     """
     Retrieves a csv showing the ensemble average forecasted flow for the year from January 1 to the current date
 
     Keyword Args:
         river_id: the ID of a stream, should be a 9 digit integer
         start_date: a YYYYMMDD string giving the earliest date this year to include, defaults to 14 days ago.
         end_date: a YYYYMMDD string giving the latest date this year to include, defaults to latest available
         data_source: location to query for data, either 'rest' or 'aws'. default is aws.
-        return_format: csv, json, or url, default csv
+        format: if data_source=="rest": csv, json, or url, default csv. if data_source=="aws": df or xarray
 
     Returns:
         pd.DataFrame or dict or str
     """
     pass
 
 
 # Retrospective simulation and derived products
-def retrospective(river_id: int or list) -> pd.DataFrame:
+def retrospective(river_id: int or list, format: str = 'df') -> pd.DataFrame or xr.Dataset:
     """
     Retrieves the retrospective simulation of streamflow for a given river_id from the
     AWS Open Data Program GEOGloWS V2 S3 bucket
 
     Args:
         river_id: the ID of a stream, should be a 9 digit integer
+        format: the format to return the data, either 'df' or 'xarray'. default is 'df'
 
     Returns:
         pd.DataFrame
     """
     s3 = s3fs.S3FileSystem(anon=True, client_kwargs=dict(region_name=ODP_S3_BUCKET_REGION))
     s3store = s3fs.S3Map(root=f'{ODP_RETROSPECTIVE_S3_BUCKET_URI}/retrospective.zarr', s3=s3, check=False)
-    return (xr.open_zarr(s3store).sel(rivid=river_id).to_dataframe().reset_index().set_index('time')
-            .pivot(columns='rivid', values='Qout'))
+    ds = xr.open_zarr(s3store).sel(rivid=river_id)
+    if format == 'xarray':
+        return ds
+    return ds.to_dataframe().reset_index().set_index('time').pivot(columns='rivid', values='Qout')
 
 
 def historical(*args, **kwargs):
     """Alias for retrospective"""
     return retrospective(*args, **kwargs)
 
 
-def daily_averages(river_id: int or list) -> pd.DataFrame:
+def daily_averages(river_id: int or list) -> pd.DataFrame or xr.Dataset:
     """
     Retrieves daily average streamflow for a given river_id
 
     Args:
         river_id: the ID of a stream, should be a 9 digit integer
 
     Returns:
@@ -324,34 +340,38 @@
     Returns:
         pd.DataFrame
     """
     df = retrospective(river_id)
     return calc_annual_averages(df)
 
 
-def return_periods(river_id: int or list) -> pd.DataFrame:
+def return_periods(river_id: int or list, format: str = 'df') -> pd.DataFrame:
     """
     Retrieves the return period thresholds based on a specified historic simulation forcing on a certain river_id.
 
     Args:
         river_id: the ID of a stream, should be a 9 digit integer
+        format: the format to return the data, either 'df' or 'xarray'. default is 'df'
 
     Returns:
         pd.DataFrame
     """
     s3 = s3fs.S3FileSystem(anon=True, client_kwargs=dict(region_name=ODP_S3_BUCKET_REGION))
     s3store = s3fs.S3Map(root=f'{ODP_RETROSPECTIVE_S3_BUCKET_URI}/return-periods.zarr', s3=s3, check=False)
-    return (xr.open_zarr(s3store).sel(rivid=river_id)['return_period_flow'].to_dataframe().reset_index()
+    ds = xr.open_zarr(s3store).sel(rivid=river_id)
+    if format == 'xarray':
+        return ds
+    return (ds['return_period_flow'].to_dataframe().reset_index()
             .pivot(index='rivid', columns='return_period', values='return_period_flow'))
 
 
 # model config and supplementary data
 def metadata_tables(columns: list = None) -> pd.DataFrame:
     """
-    Retrieves the master table of stream reaches with all metadata and properties as a pandas DataFrame
+    Retrieves the master table of rivers metadata and properties as a pandas DataFrame
     Args:
         columns: optional subset of columns names to read from the parquet
 
     Returns:
         pd.DataFrame
     """
     if os.path.exists(METADATA_TABLE_PATH):
```

### Comparing `geoglows-1.1/geoglows/streamflow.py` & `geoglows-1.2.0/geoglows/streamflow.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.1/geoglows/streams.py` & `geoglows-1.2.0/geoglows/streams.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import numpy as np
 
 from .data import metadata_tables
 
 __all__ = ['river_to_vpu', 'latlon_to_river', 'river_to_latlon', ]
 
 
-def river_to_vpu(reach_id: int) -> str or int:
+def river_to_vpu(river_id: int) -> str or int:
     return (
         metadata_tables(columns=['LINKNO', 'VPUCode'])
-        .loc[lambda x: x['LINKNO'] == reach_id, 'VPUCode']
+        .loc[lambda x: x['LINKNO'] == river_id, 'VPUCode']
         .values[0]
     )
 
 
 def latlon_to_river(lat: float, lon: float) -> int:
     df = metadata_tables(columns=['LINKNO', 'lat', 'lon'])
     df['dist'] = ((df['lat'] - lat) ** 2 + (df['lon'] - lon) ** 2) ** 0.5
     return df.loc[lambda x: x['dist'] == df['dist'].min(), 'LINKNO'].values[0]
 
 
-def river_to_latlon(reach_id: int) -> np.ndarray:
+def river_to_latlon(river_id: int) -> np.ndarray:
     return (
         metadata_tables(columns=['LINKNO', 'lat', 'lon'])
-        .loc[lambda x: x['LINKNO'] == reach_id, ['lat', 'lon']]
+        .loc[lambda x: x['LINKNO'] == river_id, ['lat', 'lon']]
         .values[0]
     )
```

### Comparing `geoglows-1.1/geoglows/tables.py` & `geoglows-1.2.0/geoglows/tables.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.1/geoglows.egg-info/PKG-INFO` & `geoglows-1.2.0/geoglows.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.1.0
+Version: 1.2.0
 Summary: Package for accessing data from the GEOGLOWS Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
```

### Comparing `geoglows-1.1/geoglows.egg-info/SOURCES.txt` & `geoglows-1.2.0/geoglows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geoglows-1.1/setup.py` & `geoglows-1.2.0/setup.py`

 * *Files identical despite different names*

