# Comparing `tmp/pytplot-mpl-temp-2.2.8.tar.gz` & `tmp/pytplot-mpl-temp-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytplot-mpl-temp-2.2.8.tar", last modified: Thu Mar 28 00:46:20 2024, max compression
+gzip compressed data, was "pytplot-mpl-temp-2.2.9.tar", last modified: Wed Apr  3 18:32:27 2024, max compression
```

## Comparing `pytplot-mpl-temp-2.2.8.tar` & `pytplot-mpl-temp-2.2.9.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-03-28 00:46:20.388244 pytplot-mpl-temp-2.2.8/
--rw-r--r--   0 jwl        (501) wheel        (0)     1065 2024-03-28 00:45:28.000000 pytplot-mpl-temp-2.2.8/LICENSE
--rw-r--r--   0 jwl        (501) wheel        (0)      363 2024-03-28 00:45:28.000000 pytplot-mpl-temp-2.2.8/MANIFEST.in
--rw-r--r--   0 jwl        (501) wheel        (0)     2791 2024-03-28 00:46:20.388363 pytplot-mpl-temp-2.2.8/PKG-INFO
--rw-r--r--   0 jwl        (501) wheel        (0)     2162 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/README.md
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-03-28 00:46:20.371434 pytplot-mpl-temp-2.2.8/docs/
--rw-r--r--   0 jwl        (501) wheel        (0)     8107 2024-03-28 00:45:28.000000 pytplot-mpl-temp-2.2.8/docs/pytplot_tutorial.html
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-03-28 00:46:20.375189 pytplot-mpl-temp-2.2.8/pytplot/
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-03-28 00:46:20.375630 pytplot-mpl-temp-2.2.8/pytplot/AncillaryPlots/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/AncillaryPlots/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     5398 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/AncillaryPlots/position_mars_2d.py
--rw-r--r--   0 jwl        (501) wheel        (0)     5105 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/AncillaryPlots/position_mars_3d.py
--rw-r--r--   0 jwl        (501) wheel        (0)    11294 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/AncillaryPlots/spec_slicer.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-03-28 00:46:20.376045 pytplot-mpl-temp-2.2.8/pytplot/MPLPlotter/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/MPLPlotter/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)    11841 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/MPLPlotter/lineplot.py
--rw-r--r--   0 jwl        (501) wheel        (0)    17493 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/MPLPlotter/specplot.py
--rw-r--r--   0 jwl        (501) wheel        (0)    29060 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/MPLPlotter/tplot.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-03-28 00:46:20.376999 pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-03-28 00:46:20.377553 pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/CustomAxis/
--rw-r--r--   0 jwl        (501) wheel        (0)    12637 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/CustomAxis/AxisItem.py
--rw-r--r--   0 jwl        (501) wheel        (0)      698 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/CustomAxis/BlankAxis.py
--rw-r--r--   0 jwl        (501) wheel        (0)     6531 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/CustomAxis/DateAxis.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1028 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/CustomAxis/NonLinearAxis.py
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/CustomAxis/__init__.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-03-28 00:46:20.377871 pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/CustomImage/
--rw-r--r--   0 jwl        (501) wheel        (0)     3121 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/CustomImage/ColorbarImage.py
--rw-r--r--   0 jwl        (501) wheel        (0)    11843 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/CustomImage/UpdatingImage.py
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/CustomImage/__init__.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-03-28 00:46:20.378076 pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/CustomLegend/
--rw-r--r--   0 jwl        (501) wheel        (0)     1720 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/CustomLegend/CustomLegend.py
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/CustomLegend/__init__.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-03-28 00:46:20.378169 pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/CustomLinearRegionItem/
--rw-r--r--   0 jwl        (501) wheel        (0)      725 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/CustomLinearRegionItem/CustomLinearRegionItem.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-03-28 00:46:20.378506 pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/CustomViewBox/
--rw-r--r--   0 jwl        (501) wheel        (0)      114 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/CustomViewBox/CustomVB.py
--rw-r--r--   0 jwl        (501) wheel        (0)      262 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/CustomViewBox/NoPaddingPlot.py
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/CustomViewBox/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     5669 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/PyTPlot_Exporter.py
--rw-r--r--   0 jwl        (501) wheel        (0)    22699 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/TVarFigure1D.py
--rw-r--r--   0 jwl        (501) wheel        (0)    15469 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/TVarFigureAlt.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2874 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/TVarFigureAxisOnly.py
--rw-r--r--   0 jwl        (501) wheel        (0)    19328 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/TVarFigureMap.py
--rw-r--r--   0 jwl        (501) wheel        (0)    22827 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/TVarFigureSpec.py
--rw-r--r--   0 jwl        (501) wheel        (0)      619 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     5885 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/generate.py
--rw-r--r--   0 jwl        (501) wheel        (0)     9469 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1720 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/count_traces.py
--rw-r--r--   0 jwl        (501) wheel        (0)     8736 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/data_att_getters_setters.py
--rw-r--r--   0 jwl        (501) wheel        (0)      780 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/data_exists.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2437 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/del_data.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-03-28 00:46:20.378806 pytplot-mpl-temp-2.2.8/pytplot/exporters/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/exporters/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      793 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/exporters/tplot_ascii.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2517 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/exporters/tplot_save.py
--rw-r--r--   0 jwl        (501) wheel        (0)     7237 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/get_data.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1302 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/get_timespan.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1685 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/get_ylimits.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-03-28 00:46:20.379356 pytplot-mpl-temp-2.2.8/pytplot/importers/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/importers/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)    31584 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/importers/cdf_to_tplot.py
--rw-r--r--   0 jwl        (501) wheel        (0)     8574 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/importers/netcdf_to_tplot.py
--rw-r--r--   0 jwl        (501) wheel        (0)     7194 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/importers/sts_to_tplot.py
--rw-r--r--   0 jwl        (501) wheel        (0)    11485 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/importers/tplot_restore.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1225 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/is_pseudovariable.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1471 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/link.py
--rw-r--r--   0 jwl        (501) wheel        (0)    31470 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/options.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1830 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/replace_data.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1664 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/replace_metadata.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-03-28 00:46:20.379469 pytplot-mpl-temp-2.2.8/pytplot/sampledata/
--rw-r--r--   0 jwl        (501) wheel        (0)  6822180 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/sampledata/test_data.tplot
--rw-r--r--   0 jwl        (501) wheel        (0)     4471 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/spedas_colorbar.py
--rw-r--r--   0 jwl        (501) wheel        (0)    17082 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/store_data.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3411 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/time_double.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2509 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/time_string.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4540 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/timebar.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1780 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/timespan.py
--rw-r--r--   0 jwl        (501) wheel        (0)      957 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/timestamp.py
--rw-r--r--   0 jwl        (501) wheel        (0)      794 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tlimit.py
--rw-r--r--   0 jwl        (501) wheel        (0)      876 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tnames.py
--rw-r--r--   0 jwl        (501) wheel        (0)    13550 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2236 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_copy.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-03-28 00:46:20.386340 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/
--rw-r--r--   0 jwl        (501) wheel        (0)     1051 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2292 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/add.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4524 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/add_across.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1881 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/avg_res_data.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3536 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/clean_spikes.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2537 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/clip.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2497 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/crop.py
--rw-r--r--   0 jwl        (501) wheel        (0)     9467 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/deflag.py
--rw-r--r--   0 jwl        (501) wheel        (0)     5766 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/degap.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1853 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/derive.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2320 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/divide.py
--rw-r--r--   0 jwl        (501) wheel        (0)     7158 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/dpwrspc.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2808 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/flatten.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1798 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/interp_nan.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4778 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/join_vec.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3711 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/makegap.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2459 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/multiply.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2619 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/pwr_spec.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3867 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/pwrspc.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2150 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/resample.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2093 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/spec_mult.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3723 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/split_vec.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2321 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/subtract.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2318 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/subtract_average.py
--rw-r--r--   0 jwl        (501) wheel        (0)      784 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/subtract_median.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1550 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/tcrossp.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2657 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/tdeflag.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1420 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/tdotp.py
--rw-r--r--   0 jwl        (501) wheel        (0)     6207 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/tdpwrspc.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-03-28 00:46:20.386522 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     9631 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/tests/tests.py
--rw-r--r--   0 jwl        (501) wheel        (0)     6997 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/time_clip.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1657 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/tinterp.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3021 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/tkm2re.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1837 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/tnormalize.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4665 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/tpwrspc.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3799 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_math/tsmooth.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2072 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_names.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3130 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_options.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1811 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_rename.py
--rw-r--r--   0 jwl        (501) wheel        (0)    30524 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tplot_utilities.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1778 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/tres.py
--rw-r--r--   0 jwl        (501) wheel        (0)     6690 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/pytplot/version.txt
--rw-r--r--   0 jwl        (501) wheel        (0)     1796 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/xlim.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1239 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/ylim.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1410 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/pytplot/zlim.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-03-28 00:46:20.387038 pytplot-mpl-temp-2.2.8/pytplot_mpl_temp.egg-info/
--rw-r--r--   0 jwl        (501) wheel        (0)     2791 2024-03-28 00:46:20.000000 pytplot-mpl-temp-2.2.8/pytplot_mpl_temp.egg-info/PKG-INFO
--rw-r--r--   0 jwl        (501) wheel        (0)     3918 2024-03-28 00:46:20.000000 pytplot-mpl-temp-2.2.8/pytplot_mpl_temp.egg-info/SOURCES.txt
--rw-r--r--   0 jwl        (501) wheel        (0)        1 2024-03-28 00:46:20.000000 pytplot-mpl-temp-2.2.8/pytplot_mpl_temp.egg-info/dependency_links.txt
--rw-r--r--   0 jwl        (501) wheel        (0)      152 2024-03-28 00:46:20.000000 pytplot-mpl-temp-2.2.8/pytplot_mpl_temp.egg-info/requires.txt
--rw-r--r--   0 jwl        (501) wheel        (0)       14 2024-03-28 00:46:20.000000 pytplot-mpl-temp-2.2.8/pytplot_mpl_temp.egg-info/top_level.txt
--rw-r--r--   0 jwl        (501) wheel        (0)     1470 2024-03-28 00:46:20.388745 pytplot-mpl-temp-2.2.8/setup.cfg
--rw-r--r--   0 jwl        (501) wheel        (0)     1311 2024-03-28 00:45:29.000000 pytplot-mpl-temp-2.2.8/setup.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-03-28 00:46:20.388135 pytplot-mpl-temp-2.2.8/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        1 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      852 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/tests/test_alt_plot.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1064 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/tests/test_cdf_to_tplot.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1212 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/tests/test_data_gap.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3774 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/tests/test_docstring_examples.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1105 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/tests/test_maps.py
--rw-r--r--   0 jwl        (501) wheel        (0)    19484 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/tests/test_matplotlib.py
--rw-r--r--   0 jwl        (501) wheel        (0)      640 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/tests/test_netcdf_to_tplot.py
--rw-r--r--   0 jwl        (501) wheel        (0)      140 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/tests/test_qt_import.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2890 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/tests/test_tplot_math.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1276 2024-03-28 00:46:05.000000 pytplot-mpl-temp-2.2.8/tests/test_tplot_restore.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-03 18:32:27.428939 pytplot-mpl-temp-2.2.9/
+-rw-r--r--   0 jwl        (501) wheel        (0)     1065 2024-04-03 18:31:10.000000 pytplot-mpl-temp-2.2.9/LICENSE
+-rw-r--r--   0 jwl        (501) wheel        (0)      363 2024-04-03 18:31:10.000000 pytplot-mpl-temp-2.2.9/MANIFEST.in
+-rw-r--r--   0 jwl        (501) wheel        (0)     2791 2024-04-03 18:32:27.429051 pytplot-mpl-temp-2.2.9/PKG-INFO
+-rw-r--r--   0 jwl        (501) wheel        (0)     2162 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/README.md
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-03 18:32:27.412054 pytplot-mpl-temp-2.2.9/docs/
+-rw-r--r--   0 jwl        (501) wheel        (0)     8107 2024-04-03 18:31:10.000000 pytplot-mpl-temp-2.2.9/docs/pytplot_tutorial.html
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-03 18:32:27.415881 pytplot-mpl-temp-2.2.9/pytplot/
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-03 18:32:27.416315 pytplot-mpl-temp-2.2.9/pytplot/AncillaryPlots/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/AncillaryPlots/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     5398 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/AncillaryPlots/position_mars_2d.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     5105 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/AncillaryPlots/position_mars_3d.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    11294 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/AncillaryPlots/spec_slicer.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-03 18:32:27.416743 pytplot-mpl-temp-2.2.9/pytplot/MPLPlotter/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/MPLPlotter/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    11841 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/MPLPlotter/lineplot.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    17493 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/MPLPlotter/specplot.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    29060 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/MPLPlotter/tplot.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-03 18:32:27.417608 pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-03 18:32:27.418122 pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/CustomAxis/
+-rw-r--r--   0 jwl        (501) wheel        (0)    12637 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/CustomAxis/AxisItem.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      698 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/CustomAxis/BlankAxis.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6531 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/CustomAxis/DateAxis.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1028 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/CustomAxis/NonLinearAxis.py
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/CustomAxis/__init__.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-03 18:32:27.418414 pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/CustomImage/
+-rw-r--r--   0 jwl        (501) wheel        (0)     3121 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/CustomImage/ColorbarImage.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    11843 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/CustomImage/UpdatingImage.py
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/CustomImage/__init__.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-03 18:32:27.418609 pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/CustomLegend/
+-rw-r--r--   0 jwl        (501) wheel        (0)     1720 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/CustomLegend/CustomLegend.py
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/CustomLegend/__init__.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-03 18:32:27.418705 pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/CustomLinearRegionItem/
+-rw-r--r--   0 jwl        (501) wheel        (0)      725 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/CustomLinearRegionItem/CustomLinearRegionItem.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-03 18:32:27.419028 pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/CustomViewBox/
+-rw-r--r--   0 jwl        (501) wheel        (0)      114 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/CustomViewBox/CustomVB.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      262 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/CustomViewBox/NoPaddingPlot.py
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/CustomViewBox/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     5669 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/PyTPlot_Exporter.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    22699 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/TVarFigure1D.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    15469 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/TVarFigureAlt.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2874 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/TVarFigureAxisOnly.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    19328 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/TVarFigureMap.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    22827 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/TVarFigureSpec.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      619 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     5885 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/generate.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     9469 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1720 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/count_traces.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     8736 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/data_att_getters_setters.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      780 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/data_exists.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2437 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/del_data.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-03 18:32:27.419309 pytplot-mpl-temp-2.2.9/pytplot/exporters/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/exporters/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      793 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/exporters/tplot_ascii.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2517 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/exporters/tplot_save.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     7237 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/get_data.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1302 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/get_timespan.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1685 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/get_ylimits.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-03 18:32:27.419822 pytplot-mpl-temp-2.2.9/pytplot/importers/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/importers/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    31584 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/importers/cdf_to_tplot.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     8574 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/importers/netcdf_to_tplot.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     7194 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/importers/sts_to_tplot.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    11485 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/importers/tplot_restore.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1225 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/is_pseudovariable.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1471 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/link.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    31470 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/options.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1830 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/replace_data.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1664 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/replace_metadata.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-03 18:32:27.419936 pytplot-mpl-temp-2.2.9/pytplot/sampledata/
+-rw-r--r--   0 jwl        (501) wheel        (0)  6822180 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/sampledata/test_data.tplot
+-rw-r--r--   0 jwl        (501) wheel        (0)     4471 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/spedas_colorbar.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    17082 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/store_data.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3411 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/time_double.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2509 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/time_string.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4540 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/timebar.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1780 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/timespan.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      957 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/timestamp.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      794 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tlimit.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      876 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tnames.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    13550 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2236 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_copy.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-03 18:32:27.426713 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/
+-rw-r--r--   0 jwl        (501) wheel        (0)     1051 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2292 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/add.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4524 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/add_across.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1881 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/avg_res_data.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3536 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/clean_spikes.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2537 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/clip.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2497 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/crop.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     9467 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/deflag.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     5766 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/degap.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1853 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/derive.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2320 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/divide.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     7158 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/dpwrspc.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2808 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/flatten.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1798 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/interp_nan.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4778 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/join_vec.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3711 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/makegap.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2459 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/multiply.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2619 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/pwr_spec.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3867 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/pwrspc.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2150 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/resample.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2093 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/spec_mult.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3723 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/split_vec.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2321 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/subtract.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2318 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/subtract_average.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      784 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/subtract_median.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1550 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/tcrossp.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2657 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/tdeflag.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1420 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/tdotp.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6207 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/tdpwrspc.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-03 18:32:27.426909 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     9631 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/tests/tests.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6997 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/time_clip.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1657 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/tinterp.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3021 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/tkm2re.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1837 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/tnormalize.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4665 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/tpwrspc.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3799 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_math/tsmooth.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2072 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_names.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3130 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_options.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1811 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_rename.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    30524 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tplot_utilities.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1778 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/tres.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6690 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/pytplot/version.txt
+-rw-r--r--   0 jwl        (501) wheel        (0)     1796 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/xlim.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1239 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/ylim.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1410 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/pytplot/zlim.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-03 18:32:27.427444 pytplot-mpl-temp-2.2.9/pytplot_mpl_temp.egg-info/
+-rw-r--r--   0 jwl        (501) wheel        (0)     2791 2024-04-03 18:32:27.000000 pytplot-mpl-temp-2.2.9/pytplot_mpl_temp.egg-info/PKG-INFO
+-rw-r--r--   0 jwl        (501) wheel        (0)     3918 2024-04-03 18:32:27.000000 pytplot-mpl-temp-2.2.9/pytplot_mpl_temp.egg-info/SOURCES.txt
+-rw-r--r--   0 jwl        (501) wheel        (0)        1 2024-04-03 18:32:27.000000 pytplot-mpl-temp-2.2.9/pytplot_mpl_temp.egg-info/dependency_links.txt
+-rw-r--r--   0 jwl        (501) wheel        (0)      152 2024-04-03 18:32:27.000000 pytplot-mpl-temp-2.2.9/pytplot_mpl_temp.egg-info/requires.txt
+-rw-r--r--   0 jwl        (501) wheel        (0)       14 2024-04-03 18:32:27.000000 pytplot-mpl-temp-2.2.9/pytplot_mpl_temp.egg-info/top_level.txt
+-rw-r--r--   0 jwl        (501) wheel        (0)     1470 2024-04-03 18:32:27.429388 pytplot-mpl-temp-2.2.9/setup.cfg
+-rw-r--r--   0 jwl        (501) wheel        (0)     1311 2024-04-03 18:31:11.000000 pytplot-mpl-temp-2.2.9/setup.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-03 18:32:27.428829 pytplot-mpl-temp-2.2.9/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        1 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      852 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/tests/test_alt_plot.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1064 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/tests/test_cdf_to_tplot.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1212 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/tests/test_data_gap.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3774 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/tests/test_docstring_examples.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1105 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/tests/test_maps.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    19484 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/tests/test_matplotlib.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      640 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/tests/test_netcdf_to_tplot.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      140 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/tests/test_qt_import.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2890 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/tests/test_tplot_math.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1276 2024-04-03 18:32:18.000000 pytplot-mpl-temp-2.2.9/tests/test_tplot_restore.py
```

### Comparing `pytplot-mpl-temp-2.2.8/LICENSE` & `pytplot-mpl-temp-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/PKG-INFO` & `pytplot-mpl-temp-2.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pytplot-mpl-temp
-Version: 2.2.8
+Version: 2.2.9
 Summary: A python version of IDL tplot libraries
 Home-page: https://github.com/MAVENSDC/pytplot
 Author: MAVEN SDC
 Author-email: mavensdc@lasp.colorado.edu
 Keywords: tplot,maven,lasp,IDL,spedas
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 [![build](https://github.com/MAVENSDC/PyTplot/workflows/build/badge.svg)](https://github.com/MAVENSDC/PyTplot/actions)
 [![DOI](https://zenodo.org/badge/68843190.svg)](https://zenodo.org/badge/latestdoi/68843190)
```

### Comparing `pytplot-mpl-temp-2.2.8/README.md` & `pytplot-mpl-temp-2.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/docs/pytplot_tutorial.html` & `pytplot-mpl-temp-2.2.9/docs/pytplot_tutorial.html`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/AncillaryPlots/position_mars_2d.py` & `pytplot-mpl-temp-2.2.9/pytplot/AncillaryPlots/position_mars_2d.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/AncillaryPlots/position_mars_3d.py` & `pytplot-mpl-temp-2.2.9/pytplot/AncillaryPlots/position_mars_3d.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/AncillaryPlots/spec_slicer.py` & `pytplot-mpl-temp-2.2.9/pytplot/AncillaryPlots/spec_slicer.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/MPLPlotter/lineplot.py` & `pytplot-mpl-temp-2.2.9/pytplot/MPLPlotter/lineplot.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/MPLPlotter/specplot.py` & `pytplot-mpl-temp-2.2.9/pytplot/MPLPlotter/specplot.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/MPLPlotter/tplot.py` & `pytplot-mpl-temp-2.2.9/pytplot/MPLPlotter/tplot.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/CustomAxis/AxisItem.py` & `pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/CustomAxis/AxisItem.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/CustomAxis/BlankAxis.py` & `pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/CustomAxis/BlankAxis.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/CustomAxis/DateAxis.py` & `pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/CustomAxis/DateAxis.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/CustomAxis/NonLinearAxis.py` & `pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/CustomAxis/NonLinearAxis.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/CustomImage/ColorbarImage.py` & `pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/CustomImage/ColorbarImage.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/CustomImage/UpdatingImage.py` & `pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/CustomImage/UpdatingImage.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/CustomLegend/CustomLegend.py` & `pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/CustomLegend/CustomLegend.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/CustomLinearRegionItem/CustomLinearRegionItem.py` & `pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/CustomLinearRegionItem/CustomLinearRegionItem.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/PyTPlot_Exporter.py` & `pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/PyTPlot_Exporter.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/TVarFigure1D.py` & `pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/TVarFigure1D.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/TVarFigureAlt.py` & `pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/TVarFigureAlt.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/TVarFigureAxisOnly.py` & `pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/TVarFigureAxisOnly.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/TVarFigureMap.py` & `pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/TVarFigureMap.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/TVarFigureSpec.py` & `pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/TVarFigureSpec.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/__init__.py` & `pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/__init__.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/QtPlotter/generate.py` & `pytplot-mpl-temp-2.2.9/pytplot/QtPlotter/generate.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/__init__.py` & `pytplot-mpl-temp-2.2.9/pytplot/__init__.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/count_traces.py` & `pytplot-mpl-temp-2.2.9/pytplot/count_traces.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/data_att_getters_setters.py` & `pytplot-mpl-temp-2.2.9/pytplot/data_att_getters_setters.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/data_exists.py` & `pytplot-mpl-temp-2.2.9/pytplot/data_exists.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/del_data.py` & `pytplot-mpl-temp-2.2.9/pytplot/del_data.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/exporters/tplot_ascii.py` & `pytplot-mpl-temp-2.2.9/pytplot/exporters/tplot_ascii.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/exporters/tplot_save.py` & `pytplot-mpl-temp-2.2.9/pytplot/exporters/tplot_save.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/get_data.py` & `pytplot-mpl-temp-2.2.9/pytplot/get_data.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/get_timespan.py` & `pytplot-mpl-temp-2.2.9/pytplot/get_timespan.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/get_ylimits.py` & `pytplot-mpl-temp-2.2.9/pytplot/get_ylimits.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/importers/cdf_to_tplot.py` & `pytplot-mpl-temp-2.2.9/pytplot/importers/cdf_to_tplot.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/importers/netcdf_to_tplot.py` & `pytplot-mpl-temp-2.2.9/pytplot/importers/netcdf_to_tplot.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/importers/sts_to_tplot.py` & `pytplot-mpl-temp-2.2.9/pytplot/importers/sts_to_tplot.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/importers/tplot_restore.py` & `pytplot-mpl-temp-2.2.9/pytplot/importers/tplot_restore.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/is_pseudovariable.py` & `pytplot-mpl-temp-2.2.9/pytplot/is_pseudovariable.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/link.py` & `pytplot-mpl-temp-2.2.9/pytplot/link.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/options.py` & `pytplot-mpl-temp-2.2.9/pytplot/options.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/replace_data.py` & `pytplot-mpl-temp-2.2.9/pytplot/replace_data.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/replace_metadata.py` & `pytplot-mpl-temp-2.2.9/pytplot/replace_metadata.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/sampledata/test_data.tplot` & `pytplot-mpl-temp-2.2.9/pytplot/sampledata/test_data.tplot`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/spedas_colorbar.py` & `pytplot-mpl-temp-2.2.9/pytplot/spedas_colorbar.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/store_data.py` & `pytplot-mpl-temp-2.2.9/pytplot/store_data.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/time_double.py` & `pytplot-mpl-temp-2.2.9/pytplot/time_double.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/time_string.py` & `pytplot-mpl-temp-2.2.9/pytplot/time_string.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/timebar.py` & `pytplot-mpl-temp-2.2.9/pytplot/timebar.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/timespan.py` & `pytplot-mpl-temp-2.2.9/pytplot/timespan.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/timestamp.py` & `pytplot-mpl-temp-2.2.9/pytplot/timestamp.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tlimit.py` & `pytplot-mpl-temp-2.2.9/pytplot/tlimit.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tnames.py` & `pytplot-mpl-temp-2.2.9/pytplot/tnames.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_copy.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_copy.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/__init__.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/__init__.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/add.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/add.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/add_across.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/add_across.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/avg_res_data.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/avg_res_data.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/clean_spikes.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/clean_spikes.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/clip.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/clip.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/crop.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/crop.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/deflag.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/deflag.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/degap.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/degap.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/derive.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/derive.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/divide.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/divide.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/dpwrspc.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/dpwrspc.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/flatten.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/flatten.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/interp_nan.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/interp_nan.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/join_vec.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/join_vec.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/makegap.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/makegap.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/multiply.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/multiply.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/pwr_spec.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/pwr_spec.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/pwrspc.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/pwrspc.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/resample.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/resample.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/spec_mult.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/spec_mult.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/split_vec.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/split_vec.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/subtract.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/subtract.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/subtract_average.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/subtract_average.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/subtract_median.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/subtract_median.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/tcrossp.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/tcrossp.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/tdeflag.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/tdeflag.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/tdotp.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/tdotp.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/tdpwrspc.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/tdpwrspc.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/tests/tests.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/time_clip.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/time_clip.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/tinterp.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/tinterp.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/tkm2re.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/tkm2re.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/tnormalize.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/tnormalize.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/tpwrspc.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/tpwrspc.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_math/tsmooth.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_math/tsmooth.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_names.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_names.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_options.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_options.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_rename.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_rename.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tplot_utilities.py` & `pytplot-mpl-temp-2.2.9/pytplot/tplot_utilities.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/tres.py` & `pytplot-mpl-temp-2.2.9/pytplot/tres.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/version.txt` & `pytplot-mpl-temp-2.2.9/pytplot/version.txt`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/xlim.py` & `pytplot-mpl-temp-2.2.9/pytplot/xlim.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/ylim.py` & `pytplot-mpl-temp-2.2.9/pytplot/ylim.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot/zlim.py` & `pytplot-mpl-temp-2.2.9/pytplot/zlim.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/pytplot_mpl_temp.egg-info/PKG-INFO` & `pytplot-mpl-temp-2.2.9/pytplot_mpl_temp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pytplot-mpl-temp
-Version: 2.2.8
+Version: 2.2.9
 Summary: A python version of IDL tplot libraries
 Home-page: https://github.com/MAVENSDC/pytplot
 Author: MAVEN SDC
 Author-email: mavensdc@lasp.colorado.edu
 Keywords: tplot,maven,lasp,IDL,spedas
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 [![build](https://github.com/MAVENSDC/PyTplot/workflows/build/badge.svg)](https://github.com/MAVENSDC/PyTplot/actions)
 [![DOI](https://zenodo.org/badge/68843190.svg)](https://zenodo.org/badge/latestdoi/68843190)
```

### Comparing `pytplot-mpl-temp-2.2.8/pytplot_mpl_temp.egg-info/SOURCES.txt` & `pytplot-mpl-temp-2.2.9/pytplot_mpl_temp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/setup.cfg` & `pytplot-mpl-temp-2.2.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pytplot-mpl-temp
-version = 2.2.8
+version = 2.2.9
 author = MAVEN SDC
 author_email = mavensdc@lasp.colorado.edu
 description = A python version of IDL tplot libraries
 url = https://github.com/MAVENSDC/pytplot
 keywords = 
 	tplot
 	maven
@@ -19,15 +19,15 @@
 	Programming Language :: Python :: 3
 	Topic :: Utilities
 license_file = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
-python_requires = >= 3.8
+python_requires = >= 3.9
 setup_requires = 
 	setuptools >= 38.6
 	pip >= 10
 include_package_data = True
 packages = find:
 install_requires = 
 	numpy >= 1.19.5
```

### Comparing `pytplot-mpl-temp-2.2.8/setup.py` & `pytplot-mpl-temp-2.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/tests/test_alt_plot.py` & `pytplot-mpl-temp-2.2.9/tests/test_alt_plot.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/tests/test_cdf_to_tplot.py` & `pytplot-mpl-temp-2.2.9/tests/test_cdf_to_tplot.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/tests/test_data_gap.py` & `pytplot-mpl-temp-2.2.9/tests/test_data_gap.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/tests/test_docstring_examples.py` & `pytplot-mpl-temp-2.2.9/tests/test_docstring_examples.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/tests/test_maps.py` & `pytplot-mpl-temp-2.2.9/tests/test_maps.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/tests/test_matplotlib.py` & `pytplot-mpl-temp-2.2.9/tests/test_matplotlib.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/tests/test_netcdf_to_tplot.py` & `pytplot-mpl-temp-2.2.9/tests/test_netcdf_to_tplot.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/tests/test_tplot_math.py` & `pytplot-mpl-temp-2.2.9/tests/test_tplot_math.py`

 * *Files identical despite different names*

### Comparing `pytplot-mpl-temp-2.2.8/tests/test_tplot_restore.py` & `pytplot-mpl-temp-2.2.9/tests/test_tplot_restore.py`

 * *Files identical despite different names*

