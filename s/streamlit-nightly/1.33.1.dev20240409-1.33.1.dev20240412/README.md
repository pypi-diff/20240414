# Comparing `tmp/streamlit-nightly-1.33.1.dev20240409.tar.gz` & `tmp/streamlit-nightly-1.33.1.dev20240412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-nightly-1.33.1.dev20240409.tar", last modified: Wed Apr 10 06:58:02 2024, max compression
+gzip compressed data, was "streamlit-nightly-1.33.1.dev20240412.tar", last modified: Sat Apr 13 17:39:53 2024, max compression
```

## Comparing `streamlit-nightly-1.33.1.dev20240409.tar` & `streamlit-nightly-1.33.1.dev20240412.tar`

### file list

```diff
@@ -1,569 +1,571 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.632056 streamlit-nightly-1.33.1.dev20240409/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-04-10 06:58:02.632056 streamlit-nightly-1.33.1.dev20240409/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.524056 streamlit-nightly-1.33.1.dev20240409/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/bin/streamlit.cmd
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 06:58:02.632056 streamlit-nightly-1.33.1.dev20240409/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.528056 streamlit-nightly-1.33.1.dev20240409/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/case_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/cli_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/code_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/color_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/column_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.532056 streamlit-nightly-1.33.1.dev20240409/streamlit/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/commands/execution_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/commands/experimental_query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    11784 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/commands/page_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.532056 streamlit-nightly-1.33.1.dev20240409/streamlit/components/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.532056 streamlit-nightly-1.33.1.dev20240409/streamlit/components/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/components/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/components/lib/local_component_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.532056 streamlit-nightly-1.33.1.dev20240409/streamlit/components/types/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/components/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/components/types/base_component_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/components/types/base_custom_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.532056 streamlit-nightly-1.33.1.dev20240409/streamlit/components/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/components/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/components/v1/component_arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/components/v1/component_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/components/v1/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/components/v1/custom_component.py
--rw-r--r--   0 runner    (1001) docker     (127)    43895 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/config_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/config_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.532056 streamlit-nightly-1.33.1.dev20240409/streamlit/connections/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/connections/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/connections/snowflake_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/connections/snowpark_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12141 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/connections/sql_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/connections/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    33225 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/delta_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/deprecation_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/development.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/echo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.540056 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/altair_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14636 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)    57049 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/arrow_altair.py
--rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/arrow_vega_lite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/balloons.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/bokeh_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/deck_gl_json_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/doc_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/form.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/graphviz_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    10617 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/heading.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/iframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    20126 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    26685 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/layouts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.540056 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17226 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/lib/column_config_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    51086 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/lib/column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/lib/dicttools.py
--rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/lib/mutable_status_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/lib/pandas_styler_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/lib/streamlit_plotly_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/lib/subtitle_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/map.py
--rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)    26886 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     9897 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/plotly_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/pyplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/snow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/spinner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/toast.py
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.544056 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30875 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     8858 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/camera_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    13325 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)    12074 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/color_picker.py
--rw-r--r--   0 runner    (1001) docker     (127)    35625 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/data_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    17371 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/file_uploader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13288 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/multiselect.py
--rw-r--r--   0 runner    (1001) docker     (127)    17561 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/number_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    12349 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/radio.py
--rw-r--r--   0 runner    (1001) docker     (127)    13158 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/select_slider.py
--rw-r--r--   0 runner    (1001) docker     (127)    11191 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/selectbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    26369 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)    21439 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/text_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    29079 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/time_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    20480 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/elements/write.py
--rw-r--r--   0 runner    (1001) docker     (127)    73749 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/emojis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/env_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/error_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.544056 streamlit-nightly-1.33.1.dev20240409/streamlit/external/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.544056 streamlit-nightly-1.33.1.dev20240409/streamlit/external/langchain/
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/external/langchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/external/langchain/streamlit_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/folder_black_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/git_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.544056 streamlit-nightly-1.33.1.dev20240409/streamlit/hello/
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/hello/Hello.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/hello/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.544056 streamlit-nightly-1.33.1.dev20240409/streamlit/hello/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/hello/pages/0_Animation_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/hello/pages/1_Plotting_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/hello/pages/2_Mapping_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/hello/pages/3_DataFrame_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/hello/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/js_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/net_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.568056 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Alert_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Alert_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/AppPage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/AppPage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/ArrowNamedDataSet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/ArrowNamedDataSet_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/ArrowVegaLiteChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/ArrowVegaLiteChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Arrow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Arrow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Audio_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Audio_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/AutoRerun_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/AutoRerun_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/BackMsg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/BackMsg_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Balloons_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Balloons_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Block_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9942 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Block_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/BokehChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/BokehChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Button_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Button_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/CameraInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/CameraInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/ChatInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/ChatInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Checkbox_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Checkbox_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/ClientState_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/ClientState_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Code_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Code_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/ColorPicker_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/ColorPicker_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Components_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Components_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/DataFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15040 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/DataFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/DateInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/DateInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/DeckGlJsonChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/DeckGlJsonChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Delta_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Delta_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/DocString_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/DocString_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/DownloadButton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/DownloadButton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Element_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16997 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Element_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Empty_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Empty_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Exception_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Exception_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Favicon_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Favicon_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/FileUploader_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/FileUploader_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/ForwardMsg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/ForwardMsg_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/GitInfo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/GitInfo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/GraphVizChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/GraphVizChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Heading_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Heading_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Html_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Html_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/IFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/IFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Image_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Image_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Json_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Json_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/LabelVisibilityMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/LabelVisibilityMessage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/LinkButton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/LinkButton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Markdown_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Markdown_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Metric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Metric_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/MultiSelect_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/MultiSelect_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/NamedDataSet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/NamedDataSet_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/NewSession_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    18437 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/NewSession_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/NumberInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/NumberInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/PageConfig_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/PageConfig_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/PageInfo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/PageInfo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/PageLink_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/PageLink_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/PageNotFound_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/PageNotFound_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/PageProfile_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/PageProfile_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/PagesChanged_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/PagesChanged_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/ParentMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/ParentMessage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/PlotlyChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/PlotlyChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Progress_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Progress_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Radio_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Radio_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/RootContainer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/RootContainer_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Selectbox_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Selectbox_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/SessionEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/SessionEvent_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/SessionStatus_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/SessionStatus_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Skeleton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Skeleton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Slider_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Slider_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Snow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Snow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Spinner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Spinner_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/TextArea_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/TextArea_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/TextInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/TextInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Text_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Text_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/TimeInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/TimeInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Toast_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Toast_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/VegaLiteChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/VegaLiteChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Video_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Video_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/WidgetStates_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/WidgetStates_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/openmetrics_data_model_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-04-10 06:54:14.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/proto/openmetrics_data_model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.572056 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36802 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/app_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.572056 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/caching/
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26158 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/caching/cache_data_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/caching/cache_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    21322 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/caching/cache_resource_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/caching/cache_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    16719 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/caching/cache_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18554 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/caching/cached_message_replay.py
--rw-r--r--   0 runner    (1001) docker     (127)    18986 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/caching/hashing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.572056 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/caching/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/caching/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/caching/storage/cache_storage_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/caching/storage/dummy_cache_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/caching/storage/local_disk_cache_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/connection_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/forward_msg_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/forward_msg_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/fragment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.572056 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/legacy_caching/
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/legacy_caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30549 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/legacy_caching/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/legacy_caching/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/media_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/media_file_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/memory_media_file_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/memory_session_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/memory_uploaded_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/metrics_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    29567 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/runtime_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/script_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.576056 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/scriptrunner/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/scriptrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/scriptrunner/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/scriptrunner/magic_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/scriptrunner/script_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/scriptrunner/script_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/scriptrunner/script_run_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    29149 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/scriptrunner/script_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12302 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/session_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.576056 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/state/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/state/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/state/query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/state/query_params_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/state/safe_session_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    27399 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/state/session_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/state/session_state_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/state/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/uploaded_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/websocket_session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/source_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.576056 streamlit-nightly-1.33.1.dev20240409/streamlit/static/
--rw-r--r--   0 runner    (1001) docker     (127)    14380 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-10 06:54:45.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.520056 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.576056 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/css/2411.8b8f33d6.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/css/3092.95a45cfe.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/css/43.e3b876c5.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)    29048 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/css/main.bf304093.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.608056 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/1074.73973756.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/1168.3029456a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/1307.8ea033f1.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/1451.3b0a3e31.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/1479.6709db03.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/178.b5384fd0.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/1792.b8efa879.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    32468 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/2187.9469f035.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  2090700 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/2411.a8823789.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/2411.a8823789.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/2469.3e9c3ce9.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/2634.1249dc7a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  3636801 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/2736.914069e5.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/2736.914069e5.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/3053.7e70ec3b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    43481 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/3092.ad569cc8.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/3301.1d1b10bb.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/3513.e3e7300a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/3631.be5c35fa.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    13223 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/3998.01237fcf.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/4113.1e7eff4d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/4132.49bf3f2c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/4132.49bf3f2c.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/4177.69f9f18d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     6420 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/4185.78230b2a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   395952 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/4253.749d5244.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/4253.749d5244.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8384 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/43.9ae03282.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/4319.a6745434.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    20661 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/4477.e10e4373.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/4500.b6f348d1.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    14718 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/4666.b694c5a9.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/474.87506447.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/5106.44f0ff51.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    21681 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/5117.04bfe5d3.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/5345.65c91ee7.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/5379.6571574f.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   107585 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/5791.9a42fb4b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    11420 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/6013.8e80e091.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  2249519 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/6150.1294fa0d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/6405.ac5a6f23.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   840843 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/656.ae85f8f1.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/656.ae85f8f1.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    24494 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/6718.802da17e.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/6853.d999ac75.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    88545 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/7142.83028745.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/7175.be4076bc.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    65522 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/7217.d970c074.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  3383788 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/7323.2808d029.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/7323.2808d029.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/7602.6175e969.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/7805.51638fbc.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/8005.43974a35.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/8427.b0ed496b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/8477.e948c092.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    15492 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/8492.f56c9d4c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/8570.6de19120.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/8691.9ccf7f89.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/9330.d29313d4.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/9336.2d95d840.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    20791 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/937.a1248039.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/9656.8c935274.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/9758.6e6d8662.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/9865.fd93213d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  4382108 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/main.37ad7d13.js
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/main.37ad7d13.js.LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.624056 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/
--rw-r--r--   0 runner    (1001) docker     (127)    28076 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    33516 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff
--rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff
--rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff
--rw-r--r--   0 runner    (1001) docker     (127)    53580 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff
--rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    18748 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff
--rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff
--rw-r--r--   0 runner    (1001) docker     (127)    22364 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff
--rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff
--rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    74492 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    63060 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    62096 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74052 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74132 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    62988 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    76860 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44640 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44748 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    77664 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    77452 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    72892 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30756 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    29384 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    68356 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    72668 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30628 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/checkmark.29851c8e9e6ef0c3d6c1e4efe3c1bb9e.svg
--rw-r--r--   0 runner    (1001) docker     (127)   101906 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif
--rw-r--r--   0 runner    (1001) docker     (127)    73528 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png
--rw-r--r--   0 runner    (1001) docker     (127)    86179 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png
--rw-r--r--   0 runner    (1001) docker     (127)    92182 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg
--rw-r--r--   0 runner    (1001) docker     (127)    39315 2024-04-10 06:57:59.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/string_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/temporary_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.624056 streamlit-nightly-1.33.1.dev20240409/streamlit/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.628056 streamlit-nightly-1.33.1.dev20240409/streamlit/testing/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/testing/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36577 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/testing/v1/app_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    59854 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/testing/v1/element_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/testing/v1/local_script_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/testing/v1/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/time_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    44478 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/type_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/url_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/user_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.628056 streamlit-nightly-1.33.1.dev20240409/streamlit/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.628056 streamlit-nightly-1.33.1.dev20240409/streamlit/vendor/ipython/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/vendor/ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/vendor/ipython/modified_sys_path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.628056 streamlit-nightly-1.33.1.dev20240409/streamlit/vendor/pympler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/vendor/pympler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    87925 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/vendor/pympler/asizeof.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.628056 streamlit-nightly-1.33.1.dev20240409/streamlit/watcher/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/watcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/watcher/event_based_path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/watcher/local_sources_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/watcher/path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/watcher/polling_path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/watcher/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.628056 streamlit-nightly-1.33.1.dev20240409/streamlit/web/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/web/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/web/cache_storage_manager_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/web/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.632056 streamlit-nightly-1.33.1.dev20240409/streamlit/web/server/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/web/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/web/server/app_static_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/web/server/browser_websocket_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/web/server/component_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/web/server/media_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/web/server/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14834 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/web/server/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/web/server/server_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/web/server/stats_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/web/server/upload_file_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/streamlit/web/server/websocket_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.632056 streamlit-nightly-1.33.1.dev20240409/streamlit_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-04-10 06:58:01.000000 streamlit-nightly-1.33.1.dev20240409/streamlit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23130 2024-04-10 06:58:01.000000 streamlit-nightly-1.33.1.dev20240409/streamlit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 06:58:01.000000 streamlit-nightly-1.33.1.dev20240409/streamlit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-10 06:58:01.000000 streamlit-nightly-1.33.1.dev20240409/streamlit_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 06:54:08.000000 streamlit-nightly-1.33.1.dev20240409/streamlit_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-10 06:58:01.000000 streamlit-nightly-1.33.1.dev20240409/streamlit_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 06:58:01.000000 streamlit-nightly-1.33.1.dev20240409/streamlit_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:58:02.632056 streamlit-nightly-1.33.1.dev20240409/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-10 06:52:27.000000 streamlit-nightly-1.33.1.dev20240409/tests/testutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.813404 streamlit-nightly-1.33.1.dev20240412/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-04-13 17:39:53.813404 streamlit-nightly-1.33.1.dev20240412/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.681404 streamlit-nightly-1.33.1.dev20240412/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/bin/streamlit.cmd
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 17:39:53.813404 streamlit-nightly-1.33.1.dev20240412/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.689404 streamlit-nightly-1.33.1.dev20240412/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/case_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/cli_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/code_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/color_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/column_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.689404 streamlit-nightly-1.33.1.dev20240412/streamlit/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/commands/execution_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/commands/experimental_query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11784 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/commands/page_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.689404 streamlit-nightly-1.33.1.dev20240412/streamlit/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.689404 streamlit-nightly-1.33.1.dev20240412/streamlit/components/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/components/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/components/lib/local_component_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.689404 streamlit-nightly-1.33.1.dev20240412/streamlit/components/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/components/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/components/types/base_component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/components/types/base_custom_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.689404 streamlit-nightly-1.33.1.dev20240412/streamlit/components/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/components/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/components/v1/component_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/components/v1/component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/components/v1/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/components/v1/custom_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43895 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/config_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/config_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.693404 streamlit-nightly-1.33.1.dev20240412/streamlit/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/connections/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/connections/snowflake_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/connections/snowpark_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12141 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/connections/sql_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/connections/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34224 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/delta_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/deprecation_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/development.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/echo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.697404 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/altair_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14636 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57049 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/arrow_altair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/arrow_vega_lite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/balloons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/bokeh_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/deck_gl_json_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/dialog_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/doc_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/graphviz_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10617 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/heading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/iframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27373 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/layouts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.701404 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17226 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/lib/column_config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51086 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/lib/column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/lib/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/lib/dicttools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/lib/mutable_status_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/lib/pandas_styler_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/lib/streamlit_plotly_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/lib/subtitle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26886 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9897 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/plotly_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/pyplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/snow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/toast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.705404 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30875 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8858 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/camera_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13325 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12074 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35625 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/data_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17371 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/file_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13288 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/multiselect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17561 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/number_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12349 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/radio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13158 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/select_slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11191 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/selectbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26369 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21439 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/text_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29079 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/time_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20480 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/elements/write.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73749 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/env_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/error_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.705404 streamlit-nightly-1.33.1.dev20240412/streamlit/external/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.705404 streamlit-nightly-1.33.1.dev20240412/streamlit/external/langchain/
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/external/langchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/external/langchain/streamlit_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/folder_black_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/git_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.705404 streamlit-nightly-1.33.1.dev20240412/streamlit/hello/
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/hello/Hello.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/hello/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.705404 streamlit-nightly-1.33.1.dev20240412/streamlit/hello/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/hello/pages/0_Animation_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/hello/pages/1_Plotting_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/hello/pages/2_Mapping_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/hello/pages/3_DataFrame_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/hello/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/js_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/net_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.733404 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Alert_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Alert_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/AppPage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/AppPage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/ArrowNamedDataSet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/ArrowNamedDataSet_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/ArrowVegaLiteChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/ArrowVegaLiteChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Arrow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Arrow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Audio_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Audio_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/AutoRerun_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/AutoRerun_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/BackMsg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/BackMsg_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Balloons_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Balloons_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Block_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Block_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/BokehChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/BokehChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Button_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Button_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/CameraInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/CameraInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/ChatInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/ChatInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Checkbox_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Checkbox_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/ClientState_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/ClientState_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Code_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Code_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/ColorPicker_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/ColorPicker_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Components_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Components_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/DataFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15040 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/DataFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/DateInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/DateInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/DeckGlJsonChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/DeckGlJsonChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Delta_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Delta_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/DocString_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/DocString_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/DownloadButton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/DownloadButton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Element_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16997 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Element_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Empty_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Empty_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Exception_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Exception_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Favicon_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Favicon_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/FileUploader_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/FileUploader_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/ForwardMsg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/ForwardMsg_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/GitInfo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/GitInfo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/GraphVizChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/GraphVizChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Heading_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Heading_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Html_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Html_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/IFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/IFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Image_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Image_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Json_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Json_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/LabelVisibilityMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/LabelVisibilityMessage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/LinkButton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/LinkButton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Markdown_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Markdown_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Metric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Metric_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/MultiSelect_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/MultiSelect_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/NamedDataSet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/NamedDataSet_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/NewSession_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18437 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/NewSession_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/NumberInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/NumberInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/PageConfig_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/PageConfig_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/PageInfo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/PageInfo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/PageLink_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/PageLink_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/PageNotFound_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/PageNotFound_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/PageProfile_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/PageProfile_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/PagesChanged_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/PagesChanged_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/ParentMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/ParentMessage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/PlotlyChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/PlotlyChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Progress_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Progress_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Radio_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Radio_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/RootContainer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/RootContainer_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Selectbox_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Selectbox_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/SessionEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/SessionEvent_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/SessionStatus_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/SessionStatus_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Skeleton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Skeleton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Slider_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Slider_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Snow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Snow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Spinner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Spinner_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/TextArea_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/TextArea_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/TextInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/TextInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Text_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Text_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/TimeInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/TimeInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Toast_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Toast_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/VegaLiteChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/VegaLiteChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Video_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Video_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/WidgetStates_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/WidgetStates_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/openmetrics_data_model_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-04-13 17:36:03.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/proto/openmetrics_data_model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.737404 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36802 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/app_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.737404 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/caching/
+-rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26158 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/caching/cache_data_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/caching/cache_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21322 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/caching/cache_resource_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/caching/cache_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16719 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/caching/cache_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18554 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/caching/cached_message_replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18986 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/caching/hashing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.741404 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/caching/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/caching/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/caching/storage/cache_storage_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/caching/storage/dummy_cache_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/caching/storage/local_disk_cache_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/connection_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/forward_msg_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/forward_msg_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/fragment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.741404 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/legacy_caching/
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/legacy_caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30549 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/legacy_caching/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/legacy_caching/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/media_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/media_file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/memory_media_file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/memory_session_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/memory_uploaded_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/metrics_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29567 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/runtime_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/script_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.741404 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/scriptrunner/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/scriptrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/scriptrunner/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/scriptrunner/magic_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/scriptrunner/script_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/scriptrunner/script_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/scriptrunner/script_run_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/scriptrunner/script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12302 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/session_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.741404 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/state/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/state/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/state/query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/state/query_params_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/state/safe_session_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27500 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/state/session_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/state/session_state_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/state/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/uploaded_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/websocket_session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/source_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.745404 streamlit-nightly-1.33.1.dev20240412/streamlit/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    14380 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-13 17:36:34.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.681404 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.745404 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/css/2411.8b8f33d6.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/css/3092.95a45cfe.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/css/43.e3b876c5.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)    29048 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/css/main.bf304093.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.785404 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/1074.73973756.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/1168.1d6408e6.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/1307.8ea033f1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/1451.3b0a3e31.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/1479.6709db03.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/178.b5384fd0.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/1792.b8efa879.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    32468 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/2187.9469f035.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  2090700 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/2411.a8823789.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/2411.a8823789.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/2469.3e9c3ce9.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/2634.1249dc7a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3636801 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/2736.914069e5.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/2736.914069e5.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/3053.7e70ec3b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    43481 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/3092.ad569cc8.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/3301.1d1b10bb.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/3513.e3e7300a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/3631.be5c35fa.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13223 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/3998.01237fcf.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/4113.1e7eff4d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/4132.49bf3f2c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/4132.49bf3f2c.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/4177.69f9f18d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6420 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/4185.78230b2a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   395952 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/4253.749d5244.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/4253.749d5244.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8384 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/43.9ae03282.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/4319.a6745434.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20661 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/4477.e10e4373.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/4500.b6f348d1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14718 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/4666.b694c5a9.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/474.87506447.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/5106.44f0ff51.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21681 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/5117.04bfe5d3.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/5345.65c91ee7.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/5379.6571574f.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   107585 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/5791.9a42fb4b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11420 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/6013.8e80e091.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  2249519 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/6150.1294fa0d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/6405.ac5a6f23.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   840843 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/656.ae85f8f1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/656.ae85f8f1.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    24494 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/6718.802da17e.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/6853.d999ac75.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    88545 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/7142.83028745.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/7175.be4076bc.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    65522 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/7217.d970c074.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3383788 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/7323.2808d029.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/7323.2808d029.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/7602.6175e969.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/7805.51638fbc.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/8005.43974a35.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/8427.d30dffe1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/8477.e948c092.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15492 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/8492.f56c9d4c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/8570.6de19120.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/8691.9ccf7f89.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/9330.d29313d4.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/9336.2d95d840.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20791 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/937.a1248039.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/9656.8c935274.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/9758.6e6d8662.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/9865.fd93213d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  4387465 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/main.46540eaf.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/main.46540eaf.js.LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.805404 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    28076 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    33516 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    53580 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    18748 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    22364 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    74492 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    63060 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    62096 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74052 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74132 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    62988 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    76860 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44640 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44748 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    77664 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    77452 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    72892 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30756 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    29384 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    68356 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    72668 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30628 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/checkmark.29851c8e9e6ef0c3d6c1e4efe3c1bb9e.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   101906 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    73528 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    86179 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92182 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    39315 2024-04-13 17:39:50.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/string_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/temporary_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.805404 streamlit-nightly-1.33.1.dev20240412/streamlit/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.805404 streamlit-nightly-1.33.1.dev20240412/streamlit/testing/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/testing/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36577 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/testing/v1/app_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59854 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/testing/v1/element_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/testing/v1/local_script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/testing/v1/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/time_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44478 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/type_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/url_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/user_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.805404 streamlit-nightly-1.33.1.dev20240412/streamlit/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.805404 streamlit-nightly-1.33.1.dev20240412/streamlit/vendor/ipython/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/vendor/ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/vendor/ipython/modified_sys_path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.805404 streamlit-nightly-1.33.1.dev20240412/streamlit/vendor/pympler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/vendor/pympler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    87925 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/vendor/pympler/asizeof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.805404 streamlit-nightly-1.33.1.dev20240412/streamlit/watcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/watcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/watcher/event_based_path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/watcher/local_sources_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/watcher/path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/watcher/polling_path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/watcher/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.809404 streamlit-nightly-1.33.1.dev20240412/streamlit/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/web/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/web/cache_storage_manager_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/web/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.809404 streamlit-nightly-1.33.1.dev20240412/streamlit/web/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/web/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/web/server/app_static_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/web/server/browser_websocket_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/web/server/component_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/web/server/media_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/web/server/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14834 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/web/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/web/server/server_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/web/server/stats_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/web/server/upload_file_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/streamlit/web/server/websocket_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.813404 streamlit-nightly-1.33.1.dev20240412/streamlit_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-04-13 17:39:52.000000 streamlit-nightly-1.33.1.dev20240412/streamlit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23202 2024-04-13 17:39:52.000000 streamlit-nightly-1.33.1.dev20240412/streamlit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 17:39:52.000000 streamlit-nightly-1.33.1.dev20240412/streamlit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-13 17:39:52.000000 streamlit-nightly-1.33.1.dev20240412/streamlit_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 17:35:57.000000 streamlit-nightly-1.33.1.dev20240412/streamlit_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-13 17:39:52.000000 streamlit-nightly-1.33.1.dev20240412/streamlit_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-13 17:39:52.000000 streamlit-nightly-1.33.1.dev20240412/streamlit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:39:53.809404 streamlit-nightly-1.33.1.dev20240412/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-13 17:34:13.000000 streamlit-nightly-1.33.1.dev20240412/tests/testutil.py
```

### Comparing `streamlit-nightly-1.33.1.dev20240409/PKG-INFO` & `streamlit-nightly-1.33.1.dev20240412/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-nightly
-Version: 1.33.1.dev20240409
+Version: 1.33.1.dev20240412
 Summary: A faster way to build and share data apps
 Home-page: https://streamlit.io
 Author: Snowflake Inc
 Author-email: hello@streamlit.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/streamlit/streamlit
 Project-URL: Bug Tracker, https://github.com/streamlit/streamlit/issues
```

### Comparing `streamlit-nightly-1.33.1.dev20240409/bin/streamlit.cmd` & `streamlit-nightly-1.33.1.dev20240412/bin/streamlit.cmd`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/setup.py` & `streamlit-nightly-1.33.1.dev20240412/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 from setuptools.command.install import install
 
 THIS_DIRECTORY = Path(__file__).parent
 
-VERSION = "1.33.1.dev20240409"  # PEP-440
+VERSION = "1.33.1.dev20240412"  # PEP-440
 
 # IMPORTANT: We should try very hard *not* to add dependencies to Streamlit.
 # And if you do add one, make the required version as general as possible:
 # - Include relevant lower bound for any features we use from our dependencies
 # - Always include the lower bound as >= VERSION, to keep testing min versions easy
 # - And include an upper bound that's < NEXT_MAJOR_VERSION
 INSTALL_REQUIRES = [
```

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/__init__.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,18 @@
 
 from streamlit.delta_generator import (
     main_dg as _main_dg,
     sidebar_dg as _sidebar_dg,
     event_dg as _event_dg,
     bottom_dg as _bottom_dg,
 )
+from streamlit.elements.dialog_decorator import (
+    # rename so that it is available as st.dialog
+    dialog_decorator as experimental_dialog,
+)
 from streamlit.runtime.caching import (
     cache_resource as _cache_resource,
     cache_data as _cache_data,
     experimental_singleton as _experimental_singleton,
     experimental_memo as _experimental_memo,
 )
 from streamlit.runtime.connection_factory import (
@@ -125,15 +129,14 @@
 # in an alternative config.
 _config.on_config_parsed(_update_logger, True)
 
 
 secrets = _secrets_singleton
 
 # DeltaGenerator methods:
-
 _main = _main_dg
 sidebar = _sidebar_dg
 _event = _event_dg
 _bottom = _bottom_dg
 
 altair_chart = _main.altair_chart
 area_chart = _main.area_chart
```

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/__main__.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/__main__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/case_converters.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/case_converters.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/cli_util.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/cli_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/code_util.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/code_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/color_util.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/color_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/column_config.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/column_config.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/commands/__init__.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/commands/execution_control.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/commands/execution_control.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/commands/experimental_query_params.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/commands/experimental_query_params.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/commands/page_config.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/commands/page_config.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/components/__init__.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/components/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/components/lib/__init__.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/components/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/components/lib/local_component_registry.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/components/lib/local_component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/components/types/__init__.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/components/types/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/components/types/base_component_registry.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/components/types/base_component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/components/types/base_custom_component.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/components/types/base_custom_component.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/components/v1/__init__.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/components/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/components/v1/component_arrow.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/components/v1/component_arrow.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/components/v1/component_registry.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/components/v1/component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/components/v1/components.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/components/v1/components.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/components/v1/custom_component.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/components/v1/custom_component.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/config.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/config.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/config_option.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/config_option.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/config_util.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/config_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/connections/__init__.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/connections/base_connection.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/connections/base_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/connections/snowflake_connection.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/connections/snowflake_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/connections/snowpark_connection.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/connections/snowpark_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/connections/sql_connection.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/connections/sql_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/connections/util.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/connections/util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/constants.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/constants.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/cursor.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/cursor.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/delta_generator.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/delta_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Final,
     Hashable,
     Iterable,
+    List,
     Literal,
     NoReturn,
     TypeVar,
     cast,
     overload,
 )
 
@@ -310,17 +311,17 @@
         If we are the main DeltaGenerator, and are inside a `with` block that
         creates a container, our active_dg is that container. Otherwise,
         our active_dg is self.
         """
         if self == self._main_dg:
             # We're being invoked via an `st.foo` pattern - use the current
             # `with` dg (aka the top of the stack).
-            current_stack = dg_stack.get()
-            if len(current_stack) > 1:
-                return current_stack[-1]
+            last_context_stack_dg = get_last_dg_added_to_context_stack()
+            if last_context_stack_dg is not None:
+                return last_context_stack_dg
 
         # We're being invoked via an `st.sidebar.foo` pattern - ignore the
         # current `with` dg.
         return self
 
     @property
     def _main_dg(self) -> DeltaGenerator:
@@ -602,42 +603,15 @@
         # Operate on the active DeltaGenerator, in case we're in a `with` block.
         dg = self._active_dg
 
         # Prevent nested columns & expanders by checking all parents.
         block_type = block_proto.WhichOneof("type")
         # Convert the generator to a list, so we can use it multiple times.
         ancestor_block_types = list(dg._ancestor_block_types)
-
-        if block_type == "column":
-            num_of_parent_columns = self._count_num_of_parent_columns(
-                ancestor_block_types
-            )
-            if (
-                self._root_container == RootContainer.SIDEBAR
-                and num_of_parent_columns > 0
-            ):
-                raise StreamlitAPIException(
-                    "Columns cannot be placed inside other columns in the sidebar. This is only possible in the main area of the app."
-                )
-            if num_of_parent_columns > 1:
-                raise StreamlitAPIException(
-                    "Columns can only be placed inside other columns up to one level of nesting."
-                )
-        if block_type == "chat_message" and block_type in ancestor_block_types:
-            raise StreamlitAPIException(
-                "Chat messages cannot nested inside other chat messages."
-            )
-        if block_type == "expandable" and block_type in ancestor_block_types:
-            raise StreamlitAPIException(
-                "Expanders may not be nested inside other expanders."
-            )
-        if block_type == "popover" and block_type in ancestor_block_types:
-            raise StreamlitAPIException(
-                "Popovers may not be nested inside other popovers."
-            )
+        _check_nested_element_violation(self, block_type, ancestor_block_types)
 
         if dg._root_container is None or dg._cursor is None:
             return dg
 
         msg = ForwardMsg_pb2.ForwardMsg()
         msg.metadata.delta_path[:] = dg._cursor.delta_path
         msg.delta.add_block.CopyFrom(block_proto)
@@ -680,19 +654,17 @@
         )
 
         return block_dg
 
     def _arrow_add_rows(
         self: DG,
         data: Data = None,
-        **kwargs: DataFrame
-        | npt.NDArray[Any]
-        | Iterable[Any]
-        | dict[Hashable, Any]
-        | None,
+        **kwargs: (
+            DataFrame | npt.NDArray[Any] | Iterable[Any] | dict[Hashable, Any] | None
+        ),
     ) -> DG | None:
         """Concatenate a dataframe to the bottom of the current one.
 
         Parameters
         ----------
         data : pandas.DataFrame, pandas.Styler, numpy.ndarray, Iterable, dict, or None
             Table to concat. Optional.
@@ -810,14 +782,28 @@
 # a DeltaGenerator is entered via a `with` block. This is implemented as a ContextVar
 # so that different threads or async tasks can have their own stacks.
 dg_stack: ContextVar[tuple[DeltaGenerator, ...]] = ContextVar(
     "dg_stack", default=(main_dg,)
 )
 
 
+def get_last_dg_added_to_context_stack() -> DeltaGenerator | None:
+    """Get the last added DeltaGenerator of the stack in the current context.
+
+    Returns None if the stack has only one element or is empty for whatever reason.
+    """
+    current_stack = dg_stack.get()
+    # If set to "> 0" and thus return the only delta generator in the stack - which logically makes more sense -, some unit tests
+    # fail. It looks like the reason is that they create their own main delta generator but do not populate the dg_stack correctly. However, to be on the safe-side,
+    # we keep the logic but leave the comment as shared knowledge for whoever will look into this in the future.
+    if len(current_stack) > 1:
+        return current_stack[-1]
+    return None
+
+
 def _prep_data_for_add_rows(
     data: Data,
     delta_type: str,
     add_rows_metadata: AddRowsMetadata,
 ) -> tuple[Data, AddRowsMetadata]:
     out_data: Data
 
@@ -923,7 +909,39 @@
     ctx.enqueue(msg)
 
 
 def _writes_directly_to_sidebar(dg: DG) -> bool:
     in_sidebar = any(a._root_container == RootContainer.SIDEBAR for a in dg._ancestors)
     has_container = bool(len(list(dg._ancestor_block_types)))
     return in_sidebar and not has_container
+
+
+def _check_nested_element_violation(
+    dg: DeltaGenerator, block_type: str | None, ancestor_block_types: List[BlockType]
+) -> None:
+    """Check if elements are nested in a forbidden way.
+
+    Raises
+    ------
+      StreamlitAPIException: throw if an invalid element nesting is detected.
+    """
+
+    if block_type == "column":
+        num_of_parent_columns = dg._count_num_of_parent_columns(ancestor_block_types)
+        if dg._root_container == RootContainer.SIDEBAR and num_of_parent_columns > 0:
+            raise StreamlitAPIException(
+                "Columns cannot be placed inside other columns in the sidebar. This is only possible in the main area of the app."
+            )
+        if num_of_parent_columns > 1:
+            raise StreamlitAPIException(
+                "Columns can only be placed inside other columns up to one level of nesting."
+            )
+    if block_type == "chat_message" and block_type in ancestor_block_types:
+        raise StreamlitAPIException(
+            "Chat messages cannot nested inside other chat messages."
+        )
+    if block_type == "expandable" and block_type in ancestor_block_types:
+        raise StreamlitAPIException(
+            "Expanders may not be nested inside other expanders."
+        )
+    if block_type == "popover" and block_type in ancestor_block_types:
+        raise StreamlitAPIException("Popovers may not be nested inside other popovers.")
```

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/deprecation_util.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/deprecation_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/development.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/development.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/echo.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/echo.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/__init__.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/alert.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/alert.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/altair_utils.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/altair_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/arrow.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/arrow.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/arrow_altair.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/arrow_altair.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/arrow_vega_lite.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/arrow_vega_lite.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/balloons.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/balloons.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/bokeh_chart.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/bokeh_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/code.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/code.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/deck_gl_json_chart.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/deck_gl_json_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/doc_string.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/doc_string.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/empty.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/empty.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/exception.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/exception.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/form.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/form.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/graphviz_chart.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/graphviz_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/heading.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/heading.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/html.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/html.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/iframe.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/iframe.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/image.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/image.py`

 * *Files 5% similar despite different names*

```diff
@@ -292,17 +292,19 @@
 
     if width < 0 and actual_width > MAXIMUM_CONTENT_WIDTH:
         width = MAXIMUM_CONTENT_WIDTH
 
     if width > 0 and actual_width > width:
         # We need to resize the image.
         new_height = int(1.0 * actual_height * width / actual_width)
-        pil_image = pil_image.resize(
-            (width, new_height), resample=Image.Resampling.BILINEAR
-        )
+        # pillow reexports Image.Resampling.BILINEAR as Image.BILINEAR for backwards
+        # compatibility reasons, so we use the reexport to support older pillow
+        # versions. The types don't seem to reflect this, though, hence the type: ignore
+        # below.
+        pil_image = pil_image.resize((width, new_height), resample=Image.BILINEAR)  # type: ignore[attr-defined]
         return _PIL_to_bytes(pil_image, format=image_format, quality=90)
 
     if pil_image.format != image_format:
         # We need to reformat the image.
         return _PIL_to_bytes(pil_image, format=image_format, quality=90)
 
     # No resizing or reformatting necessary - return the original bytes.
```

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/json.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/json.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/layouts.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/layouts.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 from streamlit.errors import StreamlitAPIException
 from streamlit.proto.Block_pb2 import Block as BlockProto
 from streamlit.runtime.metrics_util import gather_metrics
 
 if TYPE_CHECKING:
     from streamlit.delta_generator import DeltaGenerator
+    from streamlit.elements.lib.dialog import Dialog
     from streamlit.elements.lib.mutable_status_container import StatusContainer
 
 SpecType: TypeAlias = Union[int, Sequence[Union[int, float]]]
 
 
 class LayoutsMixin:
     @gather_metrics("container")
@@ -706,11 +707,29 @@
         # We need to import StatusContainer here to avoid a circular import
         from streamlit.elements.lib.mutable_status_container import StatusContainer
 
         return StatusContainer._create(
             self.dg, label=label, expanded=expanded, state=state
         )
 
+    def _dialog(
+        self,
+        title: str,
+        *,
+        dismissible: bool = True,
+        width: Literal["small", "large"] = "small",
+    ) -> "Dialog":
+        """Inserts the dialog container.
+
+        Marked as internal because it is used by the dialog_decorator and is not supposed to be used directly.
+        The dialog_decorator also has a more descriptive docstring since it is user-facing.
+        """
+
+        # We need to import Dialog here to avoid a circular import
+        from streamlit.elements.lib.dialog import Dialog
+
+        return Dialog._create(self.dg, title, dismissible=dismissible, width=width)
+
     @property
     def dg(self) -> DeltaGenerator:
         """Get our DeltaGenerator."""
         return cast("DeltaGenerator", self)
```

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/lib/__init__.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/lib/column_config_utils.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/lib/column_config_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/lib/column_types.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/lib/column_types.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/lib/dicttools.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/lib/dicttools.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/lib/mutable_status_container.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/lib/mutable_status_container.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/lib/pandas_styler_utils.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/lib/pandas_styler_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/lib/streamlit_plotly_theme.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/lib/streamlit_plotly_theme.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/lib/subtitle_utils.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/lib/subtitle_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/map.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/map.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/markdown.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/markdown.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/media.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/media.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/metric.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/metric.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/plotly_chart.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/progress.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/progress.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/pyplot.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/pyplot.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/snow.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/snow.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/spinner.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/spinner.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/text.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/text.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/toast.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/toast.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/utils.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/__init__.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/button.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/button.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/camera_input.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/camera_input.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/chat.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/chat.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/checkbox.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/color_picker.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/color_picker.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/data_editor.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/data_editor.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/file_uploader.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/file_uploader.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/multiselect.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/multiselect.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/number_input.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/number_input.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/radio.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/radio.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/select_slider.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/select_slider.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/selectbox.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/selectbox.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/slider.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/text_widgets.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/text_widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/widgets/time_widgets.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/widgets/time_widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/elements/write.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/elements/write.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/emojis.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/emojis.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/env_util.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/env_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/error_util.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/error_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/errors.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/errors.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/external/__init__.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/external/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/external/langchain/__init__.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/external/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/external/langchain/streamlit_callback_handler.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/external/langchain/streamlit_callback_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/file_util.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/file_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/folder_black_list.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/folder_black_list.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/git_util.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/git_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/hello/Hello.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/hello/Hello.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/hello/__init__.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/hello/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/hello/pages/0_Animation_Demo.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/hello/pages/0_Animation_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/hello/pages/1_Plotting_Demo.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/hello/pages/1_Plotting_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/hello/pages/2_Mapping_Demo.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/hello/pages/2_Mapping_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/hello/pages/3_DataFrame_Demo.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/hello/pages/3_DataFrame_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/hello/utils.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/hello/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/js_number.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/js_number.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/logger.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/logger.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/net_util.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/net_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/platform.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/platform.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Alert_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Alert_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Alert_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/AppPage_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/AppPage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/AppPage_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/AppPage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/ArrowNamedDataSet_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/ArrowNamedDataSet_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/ArrowNamedDataSet_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/ArrowNamedDataSet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/ArrowVegaLiteChart_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/ArrowVegaLiteChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/ArrowVegaLiteChart_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/ArrowVegaLiteChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Arrow_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Arrow_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Arrow_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Arrow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Audio_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Audio_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Audio_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Audio_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/AutoRerun_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/AutoRerun_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/AutoRerun_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/AutoRerun_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/BackMsg_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/BackMsg_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/BackMsg_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/BackMsg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Balloons_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Balloons_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Balloons_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Balloons_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Block_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Block_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,38 +9,42 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bstreamlit/proto/Block.proto\"\xfd\x06\n\x05\x42lock\x12#\n\x08vertical\x18\x01 \x01(\x0b\x32\x0f.Block.VerticalH\x00\x12\'\n\nhorizontal\x18\x02 \x01(\x0b\x32\x11.Block.HorizontalH\x00\x12\x1f\n\x06\x63olumn\x18\x03 \x01(\x0b\x32\r.Block.ColumnH\x00\x12\'\n\nexpandable\x18\x04 \x01(\x0b\x32\x11.Block.ExpandableH\x00\x12\x1b\n\x04\x66orm\x18\x05 \x01(\x0b\x32\x0b.Block.FormH\x00\x12,\n\rtab_container\x18\x06 \x01(\x0b\x32\x13.Block.TabContainerH\x00\x12\x19\n\x03tab\x18\x07 \x01(\x0b\x32\n.Block.TabH\x00\x12*\n\x0c\x63hat_message\x18\t \x01(\x0b\x32\x12.Block.ChatMessageH\x00\x12!\n\x07popover\x18\n \x01(\x0b\x32\x0e.Block.PopoverH\x00\x12\x13\n\x0b\x61llow_empty\x18\x08 \x01(\x08\x1a*\n\x08Vertical\x12\x0e\n\x06\x62order\x18\x01 \x01(\x08\x12\x0e\n\x06height\x18\x02 \x01(\r\x1a\x19\n\nHorizontal\x12\x0b\n\x03gap\x18\x01 \x01(\t\x1a%\n\x06\x43olumn\x12\x0e\n\x06weight\x18\x01 \x01(\x01\x12\x0b\n\x03gap\x18\x02 \x01(\t\x1aM\n\nExpandable\x12\r\n\x05label\x18\x01 \x01(\t\x12\x15\n\x08\x65xpanded\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x0c\n\x04icon\x18\x03 \x01(\tB\x0b\n\t_expanded\x1a@\n\x04\x46orm\x12\x0f\n\x07\x66orm_id\x18\x01 \x01(\t\x12\x17\n\x0f\x63lear_on_submit\x18\x02 \x01(\x08\x12\x0e\n\x06\x62order\x18\x03 \x01(\x08\x1a\x0e\n\x0cTabContainer\x1a\x14\n\x03Tab\x12\r\n\x05label\x18\x01 \x01(\t\x1aU\n\x07Popover\x12\r\n\x05label\x18\x01 \x01(\t\x12\x1b\n\x13use_container_width\x18\x02 \x01(\x08\x12\x0c\n\x04help\x18\x03 \x01(\t\x12\x10\n\x08\x64isabled\x18\x04 \x01(\x08\x1a\x8d\x01\n\x0b\x43hatMessage\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06\x61vatar\x18\x02 \x01(\t\x12\x32\n\x0b\x61vatar_type\x18\x03 \x01(\x0e\x32\x1d.Block.ChatMessage.AvatarType\",\n\nAvatarType\x12\t\n\x05IMAGE\x10\x00\x12\t\n\x05\x45MOJI\x10\x01\x12\x08\n\x04ICON\x10\x02\x42\x06\n\x04typeB*\n\x1c\x63om.snowflake.apps.streamlitB\nBlockProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bstreamlit/proto/Block.proto\"\xbe\x08\n\x05\x42lock\x12#\n\x08vertical\x18\x01 \x01(\x0b\x32\x0f.Block.VerticalH\x00\x12\'\n\nhorizontal\x18\x02 \x01(\x0b\x32\x11.Block.HorizontalH\x00\x12\x1f\n\x06\x63olumn\x18\x03 \x01(\x0b\x32\r.Block.ColumnH\x00\x12\'\n\nexpandable\x18\x04 \x01(\x0b\x32\x11.Block.ExpandableH\x00\x12\x1b\n\x04\x66orm\x18\x05 \x01(\x0b\x32\x0b.Block.FormH\x00\x12,\n\rtab_container\x18\x06 \x01(\x0b\x32\x13.Block.TabContainerH\x00\x12\x19\n\x03tab\x18\x07 \x01(\x0b\x32\n.Block.TabH\x00\x12*\n\x0c\x63hat_message\x18\t \x01(\x0b\x32\x12.Block.ChatMessageH\x00\x12!\n\x07popover\x18\n \x01(\x0b\x32\x0e.Block.PopoverH\x00\x12\x1f\n\x06\x64ialog\x18\x0b \x01(\x0b\x32\r.Block.DialogH\x00\x12\x13\n\x0b\x61llow_empty\x18\x08 \x01(\x08\x1a*\n\x08Vertical\x12\x0e\n\x06\x62order\x18\x01 \x01(\x08\x12\x0e\n\x06height\x18\x02 \x01(\r\x1a\x19\n\nHorizontal\x12\x0b\n\x03gap\x18\x01 \x01(\t\x1a%\n\x06\x43olumn\x12\x0e\n\x06weight\x18\x01 \x01(\x01\x12\x0b\n\x03gap\x18\x02 \x01(\t\x1aM\n\nExpandable\x12\r\n\x05label\x18\x01 \x01(\t\x12\x15\n\x08\x65xpanded\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x0c\n\x04icon\x18\x03 \x01(\tB\x0b\n\t_expanded\x1a\x9d\x01\n\x06\x44ialog\x12\r\n\x05title\x18\x01 \x01(\t\x12\x13\n\x0b\x64ismissible\x18\x02 \x01(\x08\x12(\n\x05width\x18\x03 \x01(\x0e\x32\x19.Block.Dialog.DialogWidth\x12\x14\n\x07is_open\x18\x04 \x01(\x08H\x00\x88\x01\x01\"#\n\x0b\x44ialogWidth\x12\t\n\x05SMALL\x10\x00\x12\t\n\x05LARGE\x10\x01\x42\n\n\x08_is_open\x1a@\n\x04\x46orm\x12\x0f\n\x07\x66orm_id\x18\x01 \x01(\t\x12\x17\n\x0f\x63lear_on_submit\x18\x02 \x01(\x08\x12\x0e\n\x06\x62order\x18\x03 \x01(\x08\x1a\x0e\n\x0cTabContainer\x1a\x14\n\x03Tab\x12\r\n\x05label\x18\x01 \x01(\t\x1aU\n\x07Popover\x12\r\n\x05label\x18\x01 \x01(\t\x12\x1b\n\x13use_container_width\x18\x02 \x01(\x08\x12\x0c\n\x04help\x18\x03 \x01(\t\x12\x10\n\x08\x64isabled\x18\x04 \x01(\x08\x1a\x8d\x01\n\x0b\x43hatMessage\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06\x61vatar\x18\x02 \x01(\t\x12\x32\n\x0b\x61vatar_type\x18\x03 \x01(\x0e\x32\x1d.Block.ChatMessage.AvatarType\",\n\nAvatarType\x12\t\n\x05IMAGE\x10\x00\x12\t\n\x05\x45MOJI\x10\x01\x12\x08\n\x04ICON\x10\x02\x42\x06\n\x04typeB*\n\x1c\x63om.snowflake.apps.streamlitB\nBlockProtob\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'streamlit.proto.Block_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\034com.snowflake.apps.streamlitB\nBlockProto'
   _BLOCK._serialized_start=32
-  _BLOCK._serialized_end=925
-  _BLOCK_VERTICAL._serialized_start=395
-  _BLOCK_VERTICAL._serialized_end=437
-  _BLOCK_HORIZONTAL._serialized_start=439
-  _BLOCK_HORIZONTAL._serialized_end=464
-  _BLOCK_COLUMN._serialized_start=466
-  _BLOCK_COLUMN._serialized_end=503
-  _BLOCK_EXPANDABLE._serialized_start=505
-  _BLOCK_EXPANDABLE._serialized_end=582
-  _BLOCK_FORM._serialized_start=584
-  _BLOCK_FORM._serialized_end=648
-  _BLOCK_TABCONTAINER._serialized_start=650
-  _BLOCK_TABCONTAINER._serialized_end=664
-  _BLOCK_TAB._serialized_start=666
-  _BLOCK_TAB._serialized_end=686
-  _BLOCK_POPOVER._serialized_start=688
-  _BLOCK_POPOVER._serialized_end=773
-  _BLOCK_CHATMESSAGE._serialized_start=776
-  _BLOCK_CHATMESSAGE._serialized_end=917
-  _BLOCK_CHATMESSAGE_AVATARTYPE._serialized_start=873
-  _BLOCK_CHATMESSAGE_AVATARTYPE._serialized_end=917
+  _BLOCK._serialized_end=1118
+  _BLOCK_VERTICAL._serialized_start=428
+  _BLOCK_VERTICAL._serialized_end=470
+  _BLOCK_HORIZONTAL._serialized_start=472
+  _BLOCK_HORIZONTAL._serialized_end=497
+  _BLOCK_COLUMN._serialized_start=499
+  _BLOCK_COLUMN._serialized_end=536
+  _BLOCK_EXPANDABLE._serialized_start=538
+  _BLOCK_EXPANDABLE._serialized_end=615
+  _BLOCK_DIALOG._serialized_start=618
+  _BLOCK_DIALOG._serialized_end=775
+  _BLOCK_DIALOG_DIALOGWIDTH._serialized_start=728
+  _BLOCK_DIALOG_DIALOGWIDTH._serialized_end=763
+  _BLOCK_FORM._serialized_start=777
+  _BLOCK_FORM._serialized_end=841
+  _BLOCK_TABCONTAINER._serialized_start=843
+  _BLOCK_TABCONTAINER._serialized_end=857
+  _BLOCK_TAB._serialized_start=859
+  _BLOCK_TAB._serialized_end=879
+  _BLOCK_POPOVER._serialized_start=881
+  _BLOCK_POPOVER._serialized_end=966
+  _BLOCK_CHATMESSAGE._serialized_start=969
+  _BLOCK_CHATMESSAGE._serialized_end=1110
+  _BLOCK_CHATMESSAGE_AVATARTYPE._serialized_start=1066
+  _BLOCK_CHATMESSAGE_AVATARTYPE._serialized_end=1110
 # @@protoc_insertion_point(module_scope)
```

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Block_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Block_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -92,14 +92,50 @@
             expanded: builtins.bool | None = ...,
             icon: builtins.str = ...,
         ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["_expanded", b"_expanded", "expanded", b"expanded"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["_expanded", b"_expanded", "expanded", b"expanded", "icon", b"icon", "label", b"label"]) -> None: ...
         def WhichOneof(self, oneof_group: typing_extensions.Literal["_expanded", b"_expanded"]) -> typing_extensions.Literal["expanded"] | None: ...
 
+    class Dialog(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        class _DialogWidth:
+            ValueType = typing.NewType("ValueType", builtins.int)
+            V: typing_extensions.TypeAlias = ValueType
+
+        class _DialogWidthEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[Block.Dialog._DialogWidth.ValueType], builtins.type):  # noqa: F821
+            DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+            SMALL: Block.Dialog._DialogWidth.ValueType  # 0
+            LARGE: Block.Dialog._DialogWidth.ValueType  # 1
+
+        class DialogWidth(_DialogWidth, metaclass=_DialogWidthEnumTypeWrapper): ...
+        SMALL: Block.Dialog.DialogWidth.ValueType  # 0
+        LARGE: Block.Dialog.DialogWidth.ValueType  # 1
+
+        TITLE_FIELD_NUMBER: builtins.int
+        DISMISSIBLE_FIELD_NUMBER: builtins.int
+        WIDTH_FIELD_NUMBER: builtins.int
+        IS_OPEN_FIELD_NUMBER: builtins.int
+        title: builtins.str
+        dismissible: builtins.bool
+        width: global___Block.Dialog.DialogWidth.ValueType
+        is_open: builtins.bool
+        def __init__(
+            self,
+            *,
+            title: builtins.str = ...,
+            dismissible: builtins.bool = ...,
+            width: global___Block.Dialog.DialogWidth.ValueType = ...,
+            is_open: builtins.bool | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["_is_open", b"_is_open", "is_open", b"is_open"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["_is_open", b"_is_open", "dismissible", b"dismissible", "is_open", b"is_open", "title", b"title", "width", b"width"]) -> None: ...
+        def WhichOneof(self, oneof_group: typing_extensions.Literal["_is_open", b"_is_open"]) -> typing_extensions.Literal["is_open"] | None: ...
+
     class Form(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         FORM_ID_FIELD_NUMBER: builtins.int
         CLEAR_ON_SUBMIT_FIELD_NUMBER: builtins.int
         BORDER_FIELD_NUMBER: builtins.int
         form_id: builtins.str
@@ -192,14 +228,15 @@
     COLUMN_FIELD_NUMBER: builtins.int
     EXPANDABLE_FIELD_NUMBER: builtins.int
     FORM_FIELD_NUMBER: builtins.int
     TAB_CONTAINER_FIELD_NUMBER: builtins.int
     TAB_FIELD_NUMBER: builtins.int
     CHAT_MESSAGE_FIELD_NUMBER: builtins.int
     POPOVER_FIELD_NUMBER: builtins.int
+    DIALOG_FIELD_NUMBER: builtins.int
     ALLOW_EMPTY_FIELD_NUMBER: builtins.int
     @property
     def vertical(self) -> global___Block.Vertical: ...
     @property
     def horizontal(self) -> global___Block.Horizontal: ...
     @property
     def column(self) -> global___Block.Column: ...
@@ -211,27 +248,30 @@
     def tab_container(self) -> global___Block.TabContainer: ...
     @property
     def tab(self) -> global___Block.Tab: ...
     @property
     def chat_message(self) -> global___Block.ChatMessage: ...
     @property
     def popover(self) -> global___Block.Popover: ...
+    @property
+    def dialog(self) -> global___Block.Dialog: ...
     allow_empty: builtins.bool
     def __init__(
         self,
         *,
         vertical: global___Block.Vertical | None = ...,
         horizontal: global___Block.Horizontal | None = ...,
         column: global___Block.Column | None = ...,
         expandable: global___Block.Expandable | None = ...,
         form: global___Block.Form | None = ...,
         tab_container: global___Block.TabContainer | None = ...,
         tab: global___Block.Tab | None = ...,
         chat_message: global___Block.ChatMessage | None = ...,
         popover: global___Block.Popover | None = ...,
+        dialog: global___Block.Dialog | None = ...,
         allow_empty: builtins.bool = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["chat_message", b"chat_message", "column", b"column", "expandable", b"expandable", "form", b"form", "horizontal", b"horizontal", "popover", b"popover", "tab", b"tab", "tab_container", b"tab_container", "type", b"type", "vertical", b"vertical"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["allow_empty", b"allow_empty", "chat_message", b"chat_message", "column", b"column", "expandable", b"expandable", "form", b"form", "horizontal", b"horizontal", "popover", b"popover", "tab", b"tab", "tab_container", b"tab_container", "type", b"type", "vertical", b"vertical"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["type", b"type"]) -> typing_extensions.Literal["vertical", "horizontal", "column", "expandable", "form", "tab_container", "tab", "chat_message", "popover"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["chat_message", b"chat_message", "column", b"column", "dialog", b"dialog", "expandable", b"expandable", "form", b"form", "horizontal", b"horizontal", "popover", b"popover", "tab", b"tab", "tab_container", b"tab_container", "type", b"type", "vertical", b"vertical"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["allow_empty", b"allow_empty", "chat_message", b"chat_message", "column", b"column", "dialog", b"dialog", "expandable", b"expandable", "form", b"form", "horizontal", b"horizontal", "popover", b"popover", "tab", b"tab", "tab_container", b"tab_container", "type", b"type", "vertical", b"vertical"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["type", b"type"]) -> typing_extensions.Literal["vertical", "horizontal", "column", "expandable", "form", "tab_container", "tab", "chat_message", "popover", "dialog"] | None: ...
 
 global___Block = Block
```

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/BokehChart_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/BokehChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/BokehChart_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/BokehChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Button_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Button_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Button_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Button_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/CameraInput_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/CameraInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/CameraInput_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/CameraInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/ChatInput_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/ChatInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/ChatInput_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/ChatInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Checkbox_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Checkbox_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Checkbox_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Checkbox_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/ClientState_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/ClientState_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/ClientState_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/ClientState_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Code_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Code_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Code_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/ColorPicker_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/ColorPicker_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/ColorPicker_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/ColorPicker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Common_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Common_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cstreamlit/proto/Common.proto\"\x1b\n\x0bStringArray\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\t\"\x1b\n\x0b\x44oubleArray\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x01\"\x1a\n\nInt32Array\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x05\"\x1a\n\nInt64Array\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x03\"\x1b\n\x0bSInt64Array\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x12\"\x1b\n\x0bUInt32Array\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\r\"0\n\x12StringTriggerValue\x12\x11\n\x04\x64\x61ta\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x07\n\x05_data\"M\n\x0f\x46ileURLsRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\t\x12\x12\n\nfile_names\x18\x02 \x03(\t\x12\x12\n\nsession_id\x18\x03 \x01(\t\"C\n\x08\x46ileURLs\x12\x0f\n\x07\x66ile_id\x18\x01 \x01(\t\x12\x12\n\nupload_url\x18\x02 \x01(\t\x12\x12\n\ndelete_url\x18\x03 \x01(\t\"X\n\x10\x46ileURLsResponse\x12\x13\n\x0bresponse_id\x18\x01 \x01(\t\x12\x1c\n\tfile_urls\x18\x02 \x03(\x0b\x32\t.FileURLs\x12\x11\n\terror_msg\x18\x03 \x01(\t\"i\n\x10UploadedFileInfo\x12\n\n\x02id\x18\x01 \x01(\x12\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04size\x18\x03 \x01(\r\x12\x0f\n\x07\x66ile_id\x18\x04 \x01(\t\x12\x1c\n\tfile_urls\x18\x05 \x01(\x0b\x32\t.FileURLs\"W\n\x11\x46ileUploaderState\x12\x13\n\x0bmax_file_id\x18\x01 \x01(\x12\x12-\n\x12uploaded_file_info\x18\x02 \x03(\x0b\x32\x11.UploadedFileInfoB+\n\x1c\x63om.snowflake.apps.streamlitB\x0b\x43ommonProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cstreamlit/proto/Common.proto\"\x1b\n\x0bStringArray\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\t\"\x1b\n\x0b\x44oubleArray\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x01\"\x1a\n\nInt32Array\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x05\"\x1a\n\nInt64Array\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x03\"\x1b\n\x0bSInt64Array\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x12\"\x1b\n\x0bUInt32Array\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\r\"0\n\x12StringTriggerValue\x12\x11\n\x04\x64\x61ta\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x07\n\x05_data\"M\n\x0f\x46ileURLsRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\t\x12\x12\n\nfile_names\x18\x02 \x03(\t\x12\x12\n\nsession_id\x18\x03 \x01(\t\"C\n\x08\x46ileURLs\x12\x0f\n\x07\x66ile_id\x18\x01 \x01(\t\x12\x12\n\nupload_url\x18\x02 \x01(\t\x12\x12\n\ndelete_url\x18\x03 \x01(\t\"X\n\x10\x46ileURLsResponse\x12\x13\n\x0bresponse_id\x18\x01 \x01(\t\x12\x1c\n\tfile_urls\x18\x02 \x03(\x0b\x32\t.FileURLs\x12\x11\n\terror_msg\x18\x03 \x01(\t\"i\n\x10UploadedFileInfo\x12\n\n\x02id\x18\x01 \x01(\x12\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04size\x18\x03 \x01(\x04\x12\x0f\n\x07\x66ile_id\x18\x04 \x01(\t\x12\x1c\n\tfile_urls\x18\x05 \x01(\x0b\x32\t.FileURLs\"W\n\x11\x46ileUploaderState\x12\x13\n\x0bmax_file_id\x18\x01 \x01(\x12\x12-\n\x12uploaded_file_info\x18\x02 \x03(\x0b\x32\x11.UploadedFileInfoB+\n\x1c\x63om.snowflake.apps.streamlitB\x0b\x43ommonProtob\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'streamlit.proto.Common_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\034com.snowflake.apps.streamlitB\013CommonProto'
```

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Common_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Components_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Components_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Components_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Components_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/DataFrame_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/DataFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/DataFrame_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/DataFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/DateInput_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/DateInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/DateInput_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/DateInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/DeckGlJsonChart_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/DeckGlJsonChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/DeckGlJsonChart_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/DeckGlJsonChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Delta_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Delta_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Delta_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Delta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/DocString_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/DocString_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/DocString_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/DocString_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/DownloadButton_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/DownloadButton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/DownloadButton_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/DownloadButton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Element_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Element_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Element_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Element_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Empty_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Empty_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Empty_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Empty_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Exception_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Exception_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Exception_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Exception_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Favicon_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Favicon_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Favicon_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Favicon_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/FileUploader_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/FileUploader_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/FileUploader_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/FileUploader_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/ForwardMsg_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/ForwardMsg_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/ForwardMsg_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/ForwardMsg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/GitInfo_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/GitInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/GitInfo_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/GitInfo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/GraphVizChart_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/GraphVizChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/GraphVizChart_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/GraphVizChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Heading_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Heading_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Heading_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Heading_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Html_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Html_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Html_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Html_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/IFrame_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/IFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/IFrame_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/IFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Image_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Image_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Image_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Image_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Json_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Json_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Json_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Json_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/LabelVisibilityMessage_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/LabelVisibilityMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/LabelVisibilityMessage_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/LabelVisibilityMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/LinkButton_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/LinkButton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/LinkButton_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/LinkButton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Markdown_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Markdown_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Markdown_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Markdown_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Metric_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Metric_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Metric_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Metric_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/MultiSelect_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/MultiSelect_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/MultiSelect_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/MultiSelect_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/NamedDataSet_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/NamedDataSet_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/NamedDataSet_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/NamedDataSet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/NewSession_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/NewSession_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/NewSession_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/NewSession_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/NumberInput_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/NumberInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/NumberInput_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/NumberInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/PageConfig_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/PageConfig_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/PageConfig_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/PageConfig_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/PageInfo_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/PageInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/PageInfo_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/PageInfo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/PageLink_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/PageLink_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/PageLink_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/PageLink_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/PageNotFound_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/PageNotFound_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/PageNotFound_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/PageNotFound_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/PageProfile_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/PageProfile_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/PageProfile_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/PageProfile_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/PagesChanged_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/PagesChanged_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/PagesChanged_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/PagesChanged_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/ParentMessage_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/ParentMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/ParentMessage_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/ParentMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/PlotlyChart_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/PlotlyChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/PlotlyChart_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/PlotlyChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Progress_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Progress_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Progress_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Progress_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Radio_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Radio_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Radio_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Radio_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/RootContainer_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/RootContainer_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/RootContainer_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/RootContainer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Selectbox_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Selectbox_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Selectbox_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Selectbox_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/SessionEvent_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/SessionEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/SessionEvent_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/SessionEvent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/SessionStatus_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/SessionStatus_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/SessionStatus_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/SessionStatus_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Skeleton_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Skeleton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Skeleton_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Skeleton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Slider_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Slider_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Slider_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Slider_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Snow_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Snow_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Snow_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Snow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Spinner_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Spinner_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Spinner_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Spinner_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/TextArea_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/TextArea_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/TextArea_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/TextArea_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/TextInput_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/TextInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/TextInput_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/TextInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Text_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Text_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Text_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Text_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/TimeInput_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/TimeInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/TimeInput_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/TimeInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Toast_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Toast_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Toast_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Toast_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/VegaLiteChart_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/VegaLiteChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/VegaLiteChart_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/VegaLiteChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Video_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Video_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/Video_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/Video_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/WidgetStates_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/WidgetStates_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/WidgetStates_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/WidgetStates_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/__init__.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/openmetrics_data_model_pb2.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/openmetrics_data_model_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/proto/openmetrics_data_model_pb2.pyi` & `streamlit-nightly-1.33.1.dev20240412/streamlit/proto/openmetrics_data_model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/__init__.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/app_session.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/app_session.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/caching/__init__.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/caching/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/caching/cache_data_api.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/caching/cache_data_api.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/caching/cache_errors.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/caching/cache_errors.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/caching/cache_resource_api.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/caching/cache_resource_api.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/caching/cache_type.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/caching/cache_type.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/caching/cache_utils.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/caching/cache_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/caching/cached_message_replay.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/caching/cached_message_replay.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/caching/hashing.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/caching/hashing.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/caching/storage/__init__.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/caching/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/caching/storage/cache_storage_protocol.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/caching/storage/cache_storage_protocol.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/caching/storage/dummy_cache_storage.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/caching/storage/dummy_cache_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/caching/storage/local_disk_cache_storage.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/caching/storage/local_disk_cache_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/connection_factory.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/connection_factory.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/credentials.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/credentials.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/forward_msg_cache.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/forward_msg_cache.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/forward_msg_queue.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/forward_msg_queue.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/fragment.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/fragment.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/legacy_caching/__init__.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/legacy_caching/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/legacy_caching/caching.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/legacy_caching/caching.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/legacy_caching/hashing.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/legacy_caching/hashing.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/media_file_manager.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/media_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/media_file_storage.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/media_file_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/memory_media_file_storage.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/memory_media_file_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/memory_session_storage.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/memory_session_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/memory_uploaded_file_manager.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/memory_uploaded_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/metrics_util.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/metrics_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/runtime.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/runtime_util.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/runtime_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/script_data.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/script_data.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/scriptrunner/__init__.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/scriptrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/scriptrunner/magic.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/scriptrunner/magic.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/scriptrunner/magic_funcs.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/scriptrunner/magic_funcs.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/scriptrunner/script_cache.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/scriptrunner/script_cache.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/scriptrunner/script_requests.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/scriptrunner/script_requests.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/scriptrunner/script_run_context.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/scriptrunner/script_run_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,16 @@
     widget_ids_this_run: set[str] = field(default_factory=set)
     widget_user_keys_this_run: set[str] = field(default_factory=set)
     form_ids_this_run: set[str] = field(default_factory=set)
     cursors: dict[int, "streamlit.cursor.RunningCursor"] = field(default_factory=dict)
     script_requests: ScriptRequests | None = None
     current_fragment_id: str | None = None
     fragment_ids_this_run: set[str] | None = None
+    # we allow only one dialog to be open at the same time
+    has_dialog_opened: bool = False
 
     # TODO(willhuang1997): Remove this variable when experimental query params are removed
     _experimental_query_params_used = False
     _production_query_params_used = False
 
     def reset(
         self,
@@ -98,14 +100,15 @@
         self._set_page_config_allowed = True
         self._has_script_started = False
         self.command_tracking_deactivated: bool = False
         self.tracked_commands = []
         self.tracked_commands_counter = collections.Counter()
         self.current_fragment_id = None
         self.fragment_ids_this_run = fragment_ids_this_run
+        self.has_dialog_opened = False
 
         parsed_query_params = parse.parse_qs(query_string, keep_blank_values=True)
         with self.session_state.query_params() as qp:
             qp.clear_with_no_forward_msg()
             for key, val in parsed_query_params.items():
                 if len(val) == 0:
                     qp.set_with_no_forward_msg(key, val="")
```

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/scriptrunner/script_runner.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/scriptrunner/script_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     get_script_run_ctx,
 )
 from streamlit.runtime.state import (
     SCRIPT_RUN_WITHOUT_ERRORS_KEY,
     SafeSessionState,
     SessionState,
 )
+from streamlit.runtime.state.session_state import SCRIPT_RUN_PAGE_SCRIPT_HASH_KEY
 from streamlit.runtime.uploaded_file_manager import UploadedFileManager
 from streamlit.vendor.ipython.modified_sys_path import modified_sys_path
 
 if TYPE_CHECKING:
     from streamlit.runtime.fragment import FragmentStorage
 
 _LOGGER: Final = get_logger(__name__)
@@ -459,14 +460,26 @@
                 current_page_info["page_script_hash"]
                 if current_page_info is not None
                 else main_page_info["page_script_hash"]
             )
 
             fragment_ids_this_run = set(rerun_data.fragment_id_queue)
 
+            # Clear widget state on page change. This normally happens implicitly
+            # in the script run cleanup steps, but doing it explicitly ensures
+            # it happens even if a script run was interrupted.
+            try:
+                old_hash = self._session_state[SCRIPT_RUN_PAGE_SCRIPT_HASH_KEY]
+            except KeyError:
+                old_hash = None
+
+            if old_hash != page_script_hash:
+                # Page changed, reset widget state
+                self._session_state.on_script_finished(set())
+
             ctx = self._get_script_run_ctx()
             ctx.reset(
                 query_string=rerun_data.query_string,
                 page_script_hash=page_script_hash,
                 fragment_ids_this_run=fragment_ids_this_run,
             )
 
@@ -559,14 +572,17 @@
                 ), self._set_execing_flag():
                     # Run callbacks for widgets whose values have changed.
                     if rerun_data.widget_states is not None:
                         self._session_state.on_script_will_rerun(
                             rerun_data.widget_states
                         )
 
+                    self._session_state[
+                        SCRIPT_RUN_PAGE_SCRIPT_HASH_KEY
+                    ] = page_script_hash
                     ctx.on_script_start()
                     prep_time = timer() - start_time
 
                     if rerun_data.fragment_id_queue:
                         for fragment_id in rerun_data.fragment_id_queue:
                             try:
                                 wrapped_fragment = self._fragment_storage.get(
```

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/secrets.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/secrets.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/session_manager.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/session_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/state/__init__.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/state/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/state/common.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/state/common.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/state/query_params.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/state/query_params.py`

 * *Files 12% similar despite different names*

```diff
@@ -61,14 +61,15 @@
                     # https://www.tornadoweb.org/en/stable/web.html#tornado.web.RequestHandler.get_query_argument
                     return value[-1]
             return value
         except KeyError:
             raise KeyError(missing_key_error_message(key))
 
     def __setitem__(self, key: str, value: str | Iterable[str]) -> None:
+        self._ensure_single_query_api_used()
         self.__set_item_internal(key, value)
         self._send_query_param_msg()
 
     def __set_item_internal(self, key: str, value: str | Iterable[str]) -> None:
         if isinstance(value, dict):
             raise StreamlitAPIException(
                 f"You cannot set a query params key `{key}` to a dictionary."
@@ -82,35 +83,37 @@
         # We will accept any type for the list and serialize to str just in case
         if isinstance(value, Iterable) and not isinstance(value, str):
             self._query_params[key] = [str(item) for item in value]
         else:
             self._query_params[key] = str(value)
 
     def __delitem__(self, key: str) -> None:
+        self._ensure_single_query_api_used()
         try:
             if key in EMBED_QUERY_PARAMS_KEYS:
                 raise KeyError(missing_key_error_message(key))
             del self._query_params[key]
             self._send_query_param_msg()
         except KeyError:
             raise KeyError(missing_key_error_message(key))
 
     def update(
         self,
         other: Iterable[tuple[str, str]] | SupportsKeysAndGetItem[str, str] = (),
         /,
         **kwds: str,
     ):
-        # an update function that only sends one ForwardMsg
-        # once all keys have been updated.
+        # This overrides the `update` provided by MutableMapping
+        # to ensure only one one ForwardMsg is sent.
+        self._ensure_single_query_api_used()
         if hasattr(other, "keys") and hasattr(other, "__getitem__"):
             for key in other.keys():
                 self.__set_item_internal(key, other[key])
         else:
-            for (key, value) in other:
+            for key, value in other:
                 self.__set_item_internal(key, value)
         for key, value in kwds.items():
             self.__set_item_internal(key, value)
         self._send_query_param_msg()
 
     def get_all(self, key: str) -> list[str]:
         self._ensure_single_query_api_used()
@@ -142,36 +145,50 @@
         msg.page_info_changed.query_string = parse.urlencode(
             self._query_params, doseq=True
         )
         ctx.query_string = msg.page_info_changed.query_string
         ctx.enqueue(msg)
 
     def clear(self) -> None:
-        new_query_params = {}
-        for key, value in self._query_params.items():
-            if key in EMBED_QUERY_PARAMS_KEYS:
-                new_query_params[key] = value
-        self._query_params = new_query_params
-
+        self._ensure_single_query_api_used()
+        self.clear_with_no_forward_msg(preserve_embed=True)
         self._send_query_param_msg()
 
     def to_dict(self) -> dict[str, str]:
         self._ensure_single_query_api_used()
         # return the last query param if multiple values are set
         return {
             key: self[key]
             for key in self._query_params
             if key not in EMBED_QUERY_PARAMS_KEYS
         }
 
+    def from_dict(
+        self,
+        _dict: Iterable[tuple[str, str]] | SupportsKeysAndGetItem[str, str],
+    ):
+        self._ensure_single_query_api_used()
+        old_value = self._query_params.copy()
+        self.clear_with_no_forward_msg(preserve_embed=True)
+        try:
+            self.update(_dict)
+        except StreamlitAPIException:
+            # restore the original from before we made any changes.
+            self._query_params = old_value
+            raise
+
     def set_with_no_forward_msg(self, key: str, val: list[str] | str) -> None:
         self._query_params[key] = val
 
-    def clear_with_no_forward_msg(self) -> None:
-        self._query_params.clear()
+    def clear_with_no_forward_msg(self, preserve_embed: bool = False) -> None:
+        self._query_params = {
+            key: value
+            for key, value in self._query_params.items()
+            if key in EMBED_QUERY_PARAMS_KEYS and preserve_embed
+        }
 
     def _ensure_single_query_api_used(self):
         # Avoid circular imports
         from streamlit.runtime.scriptrunner import get_script_run_ctx
 
         ctx = get_script_run_ctx()
         if ctx is None:
```

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/state/query_params_proxy.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/state/query_params_proxy.py`

 * *Files 20% similar despite different names*

```diff
@@ -68,26 +68,41 @@
         with get_session_state().query_params() as qp:
             try:
                 del qp[key]
             except KeyError:
                 raise AttributeError(missing_key_error_message(key))
 
     @overload
-    def update(self, mapping: SupportsKeysAndGetItem[str, str], /, **kwds: str):
+    def update(self, mapping: SupportsKeysAndGetItem[str, str], /, **kwds: str) -> None:
         ...
 
     @overload
-    def update(self, keys_and_values: Iterable[tuple[str, str]], /, **kwds: str):
+    def update(
+        self, keys_and_values: Iterable[tuple[str, str]], /, **kwds: str
+    ) -> None:
         ...
 
     @overload
-    def update(self, **kwds: str):
+    def update(self, **kwds: str) -> None:
         ...
 
     def update(self, other=(), /, **kwds):
+        """
+        Update one or more values in query_params at once from a dictionary or
+        dictionary-like object.
+
+        See `Mapping.update()` from Python's `collections` library.
+
+        Parameters
+        ----------
+        other: SupportsKeysAndGetItem[str, str] | Iterable[tuple[str, str]]
+            A dictionary or mapping of strings to strings.
+        **kwds: str
+            Additional key/value pairs to update passed as keyword arguments.
+        """
         with get_session_state().query_params() as qp:
             qp.update(other, **kwds)
 
     @gather_metrics("query_params.set_attr")
     def __setattr__(self, key: str, value: str | Iterable[str]) -> None:
         with get_session_state().query_params() as qp:
             qp[key] = value
@@ -142,7 +157,40 @@
         Returns
         -------
         Dict[str,str]
             A dictionary of the current query paramters in the app's URL.
         """
         with get_session_state().query_params() as qp:
             return qp.to_dict()
+
+    @overload
+    def from_dict(self, keys_and_values: Iterable[tuple[str, str]]) -> None:
+        ...
+
+    @overload
+    def from_dict(self, mapping: SupportsKeysAndGetItem[str, str]) -> None:
+        ...
+
+    @gather_metrics("query_params.from_dict")
+    def from_dict(self, other):
+        """
+        Set all of the query parameters from a dictionary or dictionary-like object.
+
+        This method primarily exists for advanced users who want to be able to control
+        multiple query string parameters in a single update. To set individual
+        query string parameters you should still use `st.query_params["parameter"] = "value"`
+        or `st.query_params.parameter = "value"`.
+
+        `embed` and `embed_options` may not be set via this method and may not be keys in the
+        `other` dictionary.
+
+        Note that this method is NOT a direct inverse of `st.query_params.to_dict()` when
+        the URL query string contains multiple values for a single key. A true inverse
+        operation for from_dict is `{key: st.query_params.get_all(key) for key st.query_params}`.
+
+        Parameters
+        -------
+        other: SupportsKeysAndGetItem[str, str] | Iterable[tuple[str, str]]
+            A dictionary used to replace the current query_params.
+        """
+        with get_session_state().query_params() as qp:
+            return qp.from_dict(other)
```

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/state/safe_session_state.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/state/safe_session_state.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/state/session_state.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/state/session_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,17 @@
     from streamlit.runtime.session_manager import SessionManager
 
 
 STREAMLIT_INTERNAL_KEY_PREFIX: Final = "$$STREAMLIT_INTERNAL_KEY"
 SCRIPT_RUN_WITHOUT_ERRORS_KEY: Final = (
     f"{STREAMLIT_INTERNAL_KEY_PREFIX}_SCRIPT_RUN_WITHOUT_ERRORS"
 )
+SCRIPT_RUN_PAGE_SCRIPT_HASH_KEY: Final = (
+    f"{STREAMLIT_INTERNAL_KEY_PREFIX}_PAGE_SCRIPT_HASH"
+)
 
 
 @dataclass(frozen=True)
 class Serialized:
     """A widget value that's serialized to a protobuf. Immutable."""
 
     value: WidgetStateProto
```

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/state/session_state_proxy.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/state/session_state_proxy.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/state/widgets.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/state/widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/stats.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/stats.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/uploaded_file_manager.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/uploaded_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/runtime/websocket_session_manager.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/runtime/websocket_session_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/source_util.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/source_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/asset-manifest.json` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/asset-manifest.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8258830022075054%*

 * *Differences: {"'entrypoints'": "{insert: [(1, 'static/js/main.46540eaf.js')], delete: [1]}",*

 * * "'files'": "{'main.js': './static/js/main.46540eaf.js', 'static/js/8427.d30dffe1.chunk.js': "*

 * *            "'./static/js/8427.d30dffe1.chunk.js', 'static/js/1168.1d6408e6.chunk.js': "*

 * *            "'./static/js/1168.1d6408e6.chunk.js', delete: ['static/js/8427.b0ed496b.chunk.js', "*

 * *            "'static/js/1168.3029456a.chunk.js']}"}*

```diff
@@ -1,21 +1,21 @@
 {
     "entrypoints": [
         "static/css/main.bf304093.css",
-        "static/js/main.37ad7d13.js"
+        "static/js/main.46540eaf.js"
     ],
     "files": {
         "index.html": "./index.html",
         "main.css": "./static/css/main.bf304093.css",
-        "main.js": "./static/js/main.37ad7d13.js",
+        "main.js": "./static/js/main.46540eaf.js",
         "static/css/2411.8b8f33d6.chunk.css": "./static/css/2411.8b8f33d6.chunk.css",
         "static/css/3092.95a45cfe.chunk.css": "./static/css/3092.95a45cfe.chunk.css",
         "static/css/43.e3b876c5.chunk.css": "./static/css/43.e3b876c5.chunk.css",
         "static/js/1074.73973756.chunk.js": "./static/js/1074.73973756.chunk.js",
-        "static/js/1168.3029456a.chunk.js": "./static/js/1168.3029456a.chunk.js",
+        "static/js/1168.1d6408e6.chunk.js": "./static/js/1168.1d6408e6.chunk.js",
         "static/js/1307.8ea033f1.chunk.js": "./static/js/1307.8ea033f1.chunk.js",
         "static/js/1451.3b0a3e31.chunk.js": "./static/js/1451.3b0a3e31.chunk.js",
         "static/js/1479.6709db03.chunk.js": "./static/js/1479.6709db03.chunk.js",
         "static/js/178.b5384fd0.chunk.js": "./static/js/178.b5384fd0.chunk.js",
         "static/js/1792.b8efa879.chunk.js": "./static/js/1792.b8efa879.chunk.js",
         "static/js/2187.9469f035.chunk.js": "./static/js/2187.9469f035.chunk.js",
         "static/js/2411.a8823789.chunk.js": "./static/js/2411.a8823789.chunk.js",
@@ -53,15 +53,15 @@
         "static/js/7142.83028745.chunk.js": "./static/js/7142.83028745.chunk.js",
         "static/js/7175.be4076bc.chunk.js": "./static/js/7175.be4076bc.chunk.js",
         "static/js/7217.d970c074.chunk.js": "./static/js/7217.d970c074.chunk.js",
         "static/js/7323.2808d029.chunk.js": "./static/js/7323.2808d029.chunk.js",
         "static/js/7602.6175e969.chunk.js": "./static/js/7602.6175e969.chunk.js",
         "static/js/7805.51638fbc.chunk.js": "./static/js/7805.51638fbc.chunk.js",
         "static/js/8005.43974a35.chunk.js": "./static/js/8005.43974a35.chunk.js",
-        "static/js/8427.b0ed496b.chunk.js": "./static/js/8427.b0ed496b.chunk.js",
+        "static/js/8427.d30dffe1.chunk.js": "./static/js/8427.d30dffe1.chunk.js",
         "static/js/8477.e948c092.chunk.js": "./static/js/8477.e948c092.chunk.js",
         "static/js/8492.f56c9d4c.chunk.js": "./static/js/8492.f56c9d4c.chunk.js",
         "static/js/8570.6de19120.chunk.js": "./static/js/8570.6de19120.chunk.js",
         "static/js/8691.9ccf7f89.chunk.js": "./static/js/8691.9ccf7f89.chunk.js",
         "static/js/9330.d29313d4.chunk.js": "./static/js/9330.d29313d4.chunk.js",
         "static/js/9336.2d95d840.chunk.js": "./static/js/9336.2d95d840.chunk.js",
         "static/js/937.a1248039.chunk.js": "./static/js/937.a1248039.chunk.js",
```

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/favicon.png` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/favicon.png`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/index.html` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/index.html`

 * *Files 12% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1,shrink-to-fit=no"/><link rel="shortcut icon" href="./favicon.png"/><link rel="preload" href="./static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2" as="font" type="font/woff2" crossorigin><title>Streamlit</title><script>window.prerenderReady=!1</script><script defer="defer" src="./static/js/main.37ad7d13.js"></script><link href="./static/css/main.bf304093.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
+<!doctype html><html lang="en"><head><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1,shrink-to-fit=no"/><link rel="shortcut icon" href="./favicon.png"/><link rel="preload" href="./static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2" as="font" type="font/woff2" crossorigin><title>Streamlit</title><script>window.prerenderReady=!1</script><script defer="defer" src="./static/js/main.46540eaf.js"></script><link href="./static/css/main.bf304093.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
```

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/css/2411.8b8f33d6.chunk.css` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/css/2411.8b8f33d6.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/css/3092.95a45cfe.chunk.css` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/css/3092.95a45cfe.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/css/43.e3b876c5.chunk.css` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/css/43.e3b876c5.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/css/main.bf304093.css` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/css/main.bf304093.css`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/1074.73973756.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/1074.73973756.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/1168.3029456a.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/1168.1d6408e6.chunk.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 "use strict";
 (self.webpackChunk_streamlit_app = self.webpackChunk_streamlit_app || []).push([
     [1168], {
         71168: (l, e, o) => {
             o.r(e), o.d(e, {
-                default: () => h
+                default: () => b
             });
             var r = o(66845),
                 t = o(25621),
                 c = o(62622),
                 a = o(42736),
                 n = o(96825),
                 i = o.n(n),
@@ -57,19 +57,19 @@
                         a = "#000024",
                         n = "#000025",
                         i = "#000026",
                         s = "#000027",
                         f = "#000028",
                         y = "#000029",
                         d = "#000030",
-                        A = "#000031";
+                        u = "#000031";
                     if ("streamlit" === o) {
                         const o = (0, p.ru)(e);
-                        l = (l = (l = (l = (l = (l = (l = (l = (l = (l = (l = l.replaceAll(r, o[0])).replaceAll(t, o[1])).replaceAll(c, o[2])).replaceAll(a, o[3])).replaceAll(n, o[4])).replaceAll(i, o[5])).replaceAll(s, o[6])).replaceAll(f, o[7])).replaceAll(y, o[8])).replaceAll(d, o[9])).replaceAll(A, o[10])
-                    } else l = (l = (l = (l = (l = (l = (l = (l = (l = (l = (l = l.replaceAll(r, "#8e0152")).replaceAll(t, "#c51b7d")).replaceAll(c, "#de77ae")).replaceAll(a, "#f1b6da")).replaceAll(n, "#fde0ef")).replaceAll(i, "#f7f7f7")).replaceAll(s, "#e6f5d0")).replaceAll(f, "#b8e186")).replaceAll(y, "#7fbc41")).replaceAll(d, "#4d9221")).replaceAll(A, "#276419");
+                        l = (l = (l = (l = (l = (l = (l = (l = (l = (l = (l = l.replaceAll(r, o[0])).replaceAll(t, o[1])).replaceAll(c, o[2])).replaceAll(a, o[3])).replaceAll(n, o[4])).replaceAll(i, o[5])).replaceAll(s, o[6])).replaceAll(f, o[7])).replaceAll(y, o[8])).replaceAll(d, o[9])).replaceAll(u, o[10])
+                    } else l = (l = (l = (l = (l = (l = (l = (l = (l = (l = (l = l.replaceAll(r, "#8e0152")).replaceAll(t, "#c51b7d")).replaceAll(c, "#de77ae")).replaceAll(a, "#f1b6da")).replaceAll(n, "#fde0ef")).replaceAll(i, "#f7f7f7")).replaceAll(s, "#e6f5d0")).replaceAll(f, "#b8e186")).replaceAll(y, "#7fbc41")).replaceAll(d, "#4d9221")).replaceAll(u, "#276419");
                     return l
                 }(l, e, o), l
             }
 
             function d(l, e) {
                 try {
                     ! function(l, e) {
@@ -241,34 +241,31 @@
                     const l = (0, s.b)(o);
                     (0, f.H)(l)
                 }
                 "title" in l.layout && (l.layout.title = i()(l.layout.title, {
                     text: "<b>".concat(l.layout.title.text, "</b>")
                 }))
             }
-            var A = o(40864);
-            const u = 450;
+            var u = o(40864);
+            const A = 450;
 
             function g(l) {
-                return !!l
-            }
-
-            function b(l) {
                 let {
                     element: e,
                     width: o,
-                    height: c
+                    height: c,
+                    isFullScreen: n
                 } = l;
-                const n = e.figure,
-                    i = (0, t.u)(),
-                    p = (0, r.useCallback)((() => {
-                        const l = JSON.parse(y(n.spec, i, e.theme)),
+                const i = e.figure,
+                    p = (0, t.u)(),
+                    s = (0, r.useCallback)((() => {
+                        const l = JSON.parse(y(i.spec, p, e.theme)),
                             r = l.layout.height,
                             t = l.layout.width;
-                        return g(c) ? (l.layout.width = o, l.layout.height = c) : e.useContainerWidth ? l.layout.width = o : (l.layout.width = t, l.layout.height = r), "streamlit" === e.theme ? d(l, i) : l.layout = function(l, e) {
+                        return n ? (l.layout.width = o, l.layout.height = c) : e.useContainerWidth ? l.layout.width = o : (l.layout.width = t, l.layout.height = r), "streamlit" === e.theme ? d(l, p) : l.layout = function(l, e) {
                             const {
                                 colors: o,
                                 genericFonts: r
                             } = e, t = {
                                 font: {
                                     color: o.bodyText,
                                     family: r.bodyFont
@@ -281,68 +278,70 @@
                                 font: {
                                     ...t.font,
                                     ...l.font
                                 },
                                 paper_bgcolor: l.paper_bgcolor || t.paper_bgcolor,
                                 plot_bgcolor: l.plot_bgcolor || t.plot_bgcolor
                             }
-                        }(l.layout, i), l
-                    }), [e.theme, e.useContainerWidth, n.spec, c, i, o]),
-                    [s, f] = (0, r.useState)(JSON.parse(n.config)),
-                    [u, b] = (0, r.useState)(p());
+                        }(l.layout, p), l
+                    }), [e.theme, e.useContainerWidth, i.spec, c, p, o, n]),
+                    [f, A] = (0, r.useState)(JSON.parse(i.config)),
+                    [g, b] = (0, r.useState)(s());
                 (0, r.useLayoutEffect)((() => {
-                    f(JSON.parse(n.config)), b(p())
-                }), [e, i, c, o, n.config, p]);
+                    A(JSON.parse(i.config)), b(s())
+                }), [e, p, c, o, i.config, s]);
                 const {
                     data: h,
                     layout: m,
                     frames: x
-                } = u;
-                return (0, A.jsx)(a.Z, {
+                } = g;
+                return (0, u.jsx)(a.Z, {
                     className: "stPlotlyChart",
                     data: h,
                     layout: m,
-                    config: s,
+                    config: f,
                     frames: x
-                }, g(c) ? "fullscreen" : "original")
+                }, n ? "fullscreen" : "original")
             }
-            const h = (0, c.Z)((function(l) {
+            const b = (0, c.Z)((function(l) {
                 let {
                     width: e,
                     element: o,
-                    height: r
+                    height: r,
+                    isFullScreen: t
                 } = l;
                 switch (o.chart) {
                     case "url":
                         return function(l) {
                             let {
                                 url: e,
                                 width: o,
                                 height: r
                             } = l;
-                            const t = r || u;
-                            return (0, A.jsx)("iframe", {
+                            const t = r || A;
+                            return (0, u.jsx)("iframe", {
                                 title: "Plotly",
                                 src: e,
                                 style: {
                                     width: o,
                                     height: t,
                                     colorScheme: "normal"
                                 }
                             })
                         }({
                             url: o.url,
                             height: r,
                             width: e
                         });
                     case "figure":
-                        return (0, A.jsx)(b, {
+                        return (0, u.jsx)(g, {
                             width: e,
                             element: o,
-                            height: r
+                            height: r,
+                            isFullScreen: t
                         });
                     default:
                         throw new Error("Unrecognized PlotlyChart type: ".concat(o.chart))
                 }
             }))
         }
     }
```

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/1307.8ea033f1.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/1307.8ea033f1.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/1451.3b0a3e31.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/1451.3b0a3e31.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/1479.6709db03.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/1479.6709db03.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/178.b5384fd0.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/178.b5384fd0.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/1792.b8efa879.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/1792.b8efa879.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/2187.9469f035.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/2187.9469f035.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/2411.a8823789.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/2411.a8823789.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/2469.3e9c3ce9.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/2469.3e9c3ce9.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/2634.1249dc7a.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/2634.1249dc7a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/2736.914069e5.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/2736.914069e5.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/2736.914069e5.chunk.js.LICENSE.txt` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/2736.914069e5.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/3053.7e70ec3b.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/3053.7e70ec3b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/3092.ad569cc8.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/3092.ad569cc8.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/3301.1d1b10bb.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/3301.1d1b10bb.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/3513.e3e7300a.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/3513.e3e7300a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/3631.be5c35fa.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/3631.be5c35fa.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/3998.01237fcf.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/3998.01237fcf.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/4113.1e7eff4d.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/4113.1e7eff4d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/4132.49bf3f2c.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/4132.49bf3f2c.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/4177.69f9f18d.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/4177.69f9f18d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/4185.78230b2a.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/4185.78230b2a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/4253.749d5244.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/4253.749d5244.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/43.9ae03282.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/43.9ae03282.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/4319.a6745434.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/4319.a6745434.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/4477.e10e4373.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/4477.e10e4373.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/4500.b6f348d1.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/4500.b6f348d1.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/4666.b694c5a9.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/4666.b694c5a9.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/474.87506447.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/474.87506447.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/5106.44f0ff51.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/5106.44f0ff51.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/5117.04bfe5d3.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/5117.04bfe5d3.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/5345.65c91ee7.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/5345.65c91ee7.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/5379.6571574f.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/5379.6571574f.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/5791.9a42fb4b.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/5791.9a42fb4b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/6013.8e80e091.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/6013.8e80e091.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/6150.1294fa0d.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/6150.1294fa0d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/6405.ac5a6f23.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/6405.ac5a6f23.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/656.ae85f8f1.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/656.ae85f8f1.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/6718.802da17e.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/6718.802da17e.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/6853.d999ac75.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/6853.d999ac75.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/7142.83028745.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/7142.83028745.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/7175.be4076bc.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/7175.be4076bc.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/7217.d970c074.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/7217.d970c074.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/7323.2808d029.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/7323.2808d029.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/7323.2808d029.chunk.js.LICENSE.txt` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/7323.2808d029.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/7602.6175e969.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/7602.6175e969.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/7805.51638fbc.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/7805.51638fbc.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/8005.43974a35.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/8005.43974a35.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/8427.b0ed496b.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/8427.d30dffe1.chunk.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -82,65 +82,65 @@
                 let {
                     theme: t,
                     body: o,
                     icon: r,
                     width: c
                 } = e;
                 const b = function(e) {
-                        if (e.length > 114) {
-                            let t = e.replace(/^(.{114}[^\s]*).*/, "$1");
-                            return t.length > 114 && (t = t.substring(0, 114).split(" ").slice(0, -1).join(" ")), t.trim()
+                        if (e.length > 109) {
+                            let t = e.replace(/^(.{109}[^\s]*).*/, "$1");
+                            return t.length > 109 && (t = t.substring(0, 109).split(" ").slice(0, -1).join(" ")), t.trim()
                         }
                         return e
                     }(o),
                     m = o !== b,
                     [x, w] = (0, i.useState)(!m),
                     [y, S] = (0, i.useState)(0),
                     v = (0, i.useCallback)((() => {
                         w(!x)
                     }), [x]),
-                    z = (0, i.useMemo)((() => function(e, t) {
-                        const o = (0, n.Iy)(t);
+                    z = (0, i.useMemo)((() => function(e) {
+                        const t = (0, n.Iy)(e);
                         return {
                             Body: {
                                 props: {
                                     "data-testid": "stToast"
                                 },
                                 style: {
                                     display: "flex",
                                     flexDirection: "row",
-                                    gap: t.spacing.md,
-                                    width: t.sizes.sidebar,
+                                    gap: e.spacing.md,
+                                    width: e.sizes.sidebar,
                                     marginTop: "8px",
-                                    borderTopLeftRadius: t.radii.lg,
-                                    borderTopRightRadius: t.radii.lg,
-                                    borderBottomLeftRadius: t.radii.lg,
-                                    borderBottomRightRadius: t.radii.lg,
-                                    paddingTop: t.spacing.lg,
-                                    paddingBottom: t.spacing.lg,
-                                    paddingLeft: t.spacing.twoXL,
-                                    paddingRight: t.spacing.twoXL,
-                                    backgroundColor: o ? t.colors.gray10 : t.colors.gray90,
-                                    color: t.colors.bodyText,
-                                    boxShadow: o ? "0px 4px 16px rgba(0, 0, 0, 0.16)" : "0px 4px 16px rgba(0, 0, 0, 0.7)"
+                                    borderTopLeftRadius: e.radii.lg,
+                                    borderTopRightRadius: e.radii.lg,
+                                    borderBottomLeftRadius: e.radii.lg,
+                                    borderBottomRightRadius: e.radii.lg,
+                                    paddingTop: e.spacing.lg,
+                                    paddingBottom: e.spacing.lg,
+                                    paddingLeft: e.spacing.twoXL,
+                                    paddingRight: e.spacing.twoXL,
+                                    backgroundColor: t ? e.colors.gray10 : e.colors.gray90,
+                                    color: e.colors.bodyText,
+                                    boxShadow: t ? "0px 4px 16px rgba(0, 0, 0, 0.16)" : "0px 4px 16px rgba(0, 0, 0, 0.7)"
                                 }
                             },
                             CloseIcon: {
                                 style: {
-                                    color: t.colors.fadedText40,
-                                    width: t.fontSizes.lg,
-                                    height: t.fontSizes.lg,
-                                    marginRight: "calc(-1 * ".concat(t.spacing.lg, " / 2)"),
+                                    color: e.colors.fadedText40,
+                                    width: e.fontSizes.lg,
+                                    height: e.fontSizes.lg,
+                                    marginRight: "calc(-1 * ".concat(e.spacing.lg, " / 2)"),
                                     ":hover": {
-                                        color: t.colors.bodyText
+                                        color: e.colors.bodyText
                                     }
                                 }
                             }
                         }
-                    }(0, t)), [x, t]),
+                    }(t)), [t]),
                     R = (0, i.useMemo)((() => (0, f.jsx)(f.Fragment, {
                         children: (0, f.jsxs)(p, {
                             expanded: x,
                             children: [(0, f.jsx)(u, {
                                 children: r
                             }), (0, f.jsxs)(h, {
                                 children: [(0, f.jsx)(a.ZP, {
```

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/8477.e948c092.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/8477.e948c092.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/8492.f56c9d4c.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/8492.f56c9d4c.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/8570.6de19120.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/8570.6de19120.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/8691.9ccf7f89.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/8691.9ccf7f89.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/9330.d29313d4.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/9330.d29313d4.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/9336.2d95d840.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/9336.2d95d840.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/937.a1248039.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/937.a1248039.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/9656.8c935274.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/9656.8c935274.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/9758.6e6d8662.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/9758.6e6d8662.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/9865.fd93213d.chunk.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/9865.fd93213d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/main.37ad7d13.js` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/main.46540eaf.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,21 +1,28 @@
-/*! For license information please see main.37ad7d13.js.LICENSE.txt */
+/*! For license information please see main.46540eaf.js.LICENSE.txt */
 (() => {
     var __webpack_modules__ = {
             68785: (e, t, n) => {
                 "use strict";
                 n.d(t, {
                     B: () => i,
                     Id: () => r,
                     td: () => o
                 });
                 const r = 8501,
                     o = 3e3 === +window.location.port,
                     i = !1
             },
+            78693: (e, t, n) => {
+                "use strict";
+                n.d(t, {
+                    Z: () => r
+                });
+                const r = n(66845).createContext(!1)
+            },
             84457: (e, t, n) => {
                 "use strict";
                 n.d(t, {
                     Z: () => r
                 });
                 const r = n(66845).createContext(!1)
             },
@@ -8598,18 +8605,18 @@
                             padding: (0, a.ZB)(r, o)
                         }
                     }), "")
             },
             21e3: (e, t, n) => {
                 "use strict";
                 n.d(t, {
-                    U6: () => td,
-                    cw: () => od,
-                    $G: () => Jp,
-                    ZP: () => sd
+                    U6: () => nd,
+                    cw: () => id,
+                    $G: () => Qp,
+                    ZP: () => ld
                 });
                 var r = {};
                 n.r(r), n.d(r, {
                     attentionMarkers: () => zt,
                     contentInitial: () => ft,
                     disable: () => yt,
                     document: () => bt,
@@ -26847,147 +26854,149 @@
                     return (0, Fp.jsx)(jp.l1, {
                         className: "stCodeBlock",
                         "data-testid": "stCodeBlock",
                         isMarkdown: !0,
                         children: t
                     })
                 }
-                var Vp = n(84457),
-                    Hp = n(95899),
-                    Xp = n(92627),
-                    Gp = n(66694),
-                    $p = n(40108),
-                    Kp = (n(32170), n(94735)),
-                    Yp = n.n(Kp),
-                    Zp = n(88112);
-                let Jp;
+                var Vp = n(78693),
+                    Hp = n(84457),
+                    Xp = n(95899),
+                    Gp = n(92627),
+                    $p = n(66694),
+                    Kp = n(40108),
+                    Yp = (n(32170), n(94735)),
+                    Zp = n.n(Yp),
+                    Jp = n(88112);
+                let Qp;
 
-                function Qp(e) {
+                function ed(e) {
                     return e
                 }! function(e) {
                     e.H1 = "h1", e.H2 = "h2", e.H3 = "h3"
-                }(Jp || (Jp = {}));
-                const ed = pr()((e => {
+                }(Qp || (Qp = {}));
+                const td = pr()((e => {
                         e.scrollIntoView(!0)
                     })),
-                    td = e => {
+                    nd = e => {
                         let {
                             tag: t,
                             anchor: n,
                             hideAnchor: r,
                             children: o,
                             tagProps: a
                         } = e;
-                        const s = i.useContext(Vp.Z),
-                            [l, c] = i.useState(n),
-                            [u, p] = i.useState(null),
+                        const s = i.useContext(Hp.Z),
+                            l = i.useContext(Vp.Z),
+                            [c, u] = i.useState(n),
+                            [p, d] = i.useState(null),
                             {
-                                addScriptFinishedHandler: d,
-                                removeScriptFinishedHandler: b
-                            } = i.useContext(Gp.E),
-                            f = i.useCallback((() => {
-                                null !== u && window.setTimeout((() => {
-                                    ed(u)
+                                addScriptFinishedHandler: b,
+                                removeScriptFinishedHandler: f
+                            } = i.useContext($p.E),
+                            h = i.useCallback((() => {
+                                null !== p && window.setTimeout((() => {
+                                    td(p)
                                 }), 300)
-                            }), [u]);
-                        i.useEffect((() => (d(f), () => {
-                            b(f)
-                        })), [d, b, f]);
-                        const h = i.useCallback((e => {
+                            }), [p]);
+                        i.useEffect((() => (b(h), () => {
+                            f(h)
+                        })), [b, f, h]);
+                        const m = i.useCallback((e => {
                             if (null === e) return;
                             const t = n || function(e) {
                                 let t = "";
-                                return e && /^[\x00-\x7F]*$/.test(e) ? t = null === e || void 0 === e ? void 0 : e.toLowerCase().split(/[^\p{L}\p{N}]+/gu).filter(Boolean).join("-") : e && (t = Yp().h32(e, 43981).toString(16)), t
+                                return e && /^[\x00-\x7F]*$/.test(e) ? t = null === e || void 0 === e ? void 0 : e.toLowerCase().split(/[^\p{L}\p{N}]+/gu).filter(Boolean).join("-") : e && (t = Zp().h32(e, 43981).toString(16)), t
                             }(e.textContent);
-                            c(t), window.location.hash.slice(1) === t && p(e)
+                            u(t), window.location.hash.slice(1) === t && d(e)
                         }), [n]);
-                        return s ? i.createElement(t, a, o) : i.createElement(t, {
+                        return s || l ? i.createElement(t, a, o) : i.createElement(t, {
                             ...a,
-                            ref: h,
-                            id: l
-                        }, (0, Fp.jsxs)($p.P7, {
+                            ref: m,
+                            id: c
+                        }, (0, Fp.jsxs)(Kp.P7, {
                             "data-testid": "StyledLinkIconContainer",
-                            children: [l && !r && (0, Fp.jsx)($p.Cv, {
-                                href: "#".concat(l),
+                            children: [c && !r && (0, Fp.jsx)(Kp.Cv, {
+                                href: "#".concat(c),
                                 children: (0, Fp.jsx)(Au, {
                                     size: "18"
                                 })
-                            }), (0, Fp.jsx)($p.h$, {
+                            }), (0, Fp.jsx)(Kp.h$, {
                                 children: o
                             })]
                         }))
                     },
-                    nd = e => {
+                    rd = e => {
                         let {
                             node: t,
                             children: n,
                             ...r
                         } = e;
                         const o = r["data-anchor"];
-                        return (0, Fp.jsx)($p.jO, {
-                            children: (0, Fp.jsx)(td, {
+                        return (0, Fp.jsx)(Kp.jO, {
+                            children: (0, Fp.jsx)(nd, {
                                 tag: t.tagName,
                                 anchor: o,
                                 tagProps: r,
                                 children: n
                             })
                         })
                     },
-                    rd = e => {
+                    od = e => {
                         let {
                             inline: t,
                             className: n,
                             children: r,
                             ...o
                         } = e;
                         const i = /language-(\w+)/.exec(n || ""),
                             a = String(r).trim().replace(/\n$/, ""),
                             s = i && i[1] || "";
                         return t ? (0, Fp.jsx)("code", {
                             className: n,
                             ...br()(o, "node"),
                             children: r
-                        }) : (0, Fp.jsx)(Zp.default, {
+                        }) : (0, Fp.jsx)(Jp.default, {
                             language: s,
                             showLineNumbers: !1,
                             children: a
                         })
                     };
 
-                function od(e) {
+                function id(e) {
                     let {
                         allowHTML: t,
                         source: n,
                         overrideComponents: r,
                         isLabel: o,
                         disableLinks: i
                     } = e;
                     const a = {
                             pre: Up,
-                            code: rd,
-                            a: ad,
-                            h1: nd,
-                            h2: nd,
-                            h3: nd,
-                            h4: nd,
-                            h5: nd,
-                            h6: nd,
+                            code: od,
+                            a: sd,
+                            h1: rd,
+                            h2: rd,
+                            h3: rd,
+                            h4: rd,
+                            h5: rd,
+                            h6: rd,
                             ...r || {}
                         },
                         s = (0, b.u)(),
                         {
                             red: l,
                             orange: c,
                             yellow: u,
                             green: p,
                             blue: f,
                             violet: h,
                             purple: m,
                             gray: M
-                        } = (0, Xp.KQ)(s),
+                        } = (0, Gp.KQ)(s),
                         O = new Map(Object.entries({
                             red: "color: ".concat(l),
                             blue: "color: ".concat(f),
                             green: "color: ".concat(p),
                             violet: "color: ".concat(h),
                             orange: "color: ".concat(c),
                             gray: "color: ".concat(M),
@@ -27007,27 +27016,27 @@
                                         }
                                     }
                                 }))
                             }
                         }],
                         z = [Ou, ...t ? [Jo] : []],
                         y = ["img", "table", "thead", "tbody", "tr", "th", "td", "h1", "h2", "h3", "ul", "ol", "li", "input", "hr", "blockquote", ...i ? ["a"] : []];
-                    return (0, Fp.jsx)(Hp.Z, {
+                    return (0, Fp.jsx)(Xp.Z, {
                         children: (0, Fp.jsx)(cr, {
                             remarkPlugins: g,
                             rehypePlugins: z,
                             components: a,
-                            transformLinkUri: Qp,
+                            transformLinkUri: ed,
                             disallowedElements: o ? y : [],
                             unwrapDisallowed: !0,
                             children: n
                         })
                     })
                 }
-                class id extends i.PureComponent {
+                class ad extends i.PureComponent {
                     constructor() {
                         super(...arguments), this.context = void 0, this.componentDidCatch = () => {
                             const {
                                 source: e
                             } = this.props;
                             throw Object.assign(new Error, {
                                 name: "Error parsing Markdown or HTML in this string",
@@ -27046,34 +27055,34 @@
                             isCaption: r,
                             isLabel: o,
                             boldLabel: i,
                             largerLabel: a,
                             disableLinks: s,
                             isToast: l
                         } = this.props, c = this.context;
-                        return (0, Fp.jsx)($p.r$, {
+                        return (0, Fp.jsx)(Kp.r$, {
                             isCaption: Boolean(r),
                             isInSidebar: c,
                             isLabel: o,
                             boldLabel: i,
                             largerLabel: a,
                             isToast: l,
                             style: n,
                             "data-testid": r ? "stCaptionContainer" : "stMarkdownContainer",
-                            children: (0, Fp.jsx)(od, {
+                            children: (0, Fp.jsx)(id, {
                                 source: e,
                                 allowHTML: t,
                                 isLabel: o,
                                 disableLinks: s
                             })
                         })
                     }
                 }
 
-                function ad(e) {
+                function sd(e) {
                     const {
                         href: t
                     } = e;
                     if (t && t.startsWith("#")) {
                         const {
                             children: t,
                             ...n
@@ -27095,16 +27104,16 @@
                         title: n,
                         target: o || "_blank",
                         rel: i || "noopener noreferrer",
                         ...br()(a, "node"),
                         children: r
                     })
                 }
-                id.contextType = Vp.Z;
-                const sd = id
+                ad.contextType = Hp.Z;
+                const ld = ad
             },
             40108: (e, t, n) => {
                 "use strict";
                 n.d(t, {
                     Cv: () => l,
                     IW: () => p,
                     P7: () => s,
@@ -36896,21 +36905,21 @@
                         }, e
                     })(), s.Block = (() => {
                         function e(e) {
                             if (e)
                                 for (let t = Object.keys(e), n = 0; n < t.length; ++n) null != e[t[n]] && (this[t[n]] = e[t[n]])
                         }
                         let t;
-                        return e.prototype.vertical = null, e.prototype.horizontal = null, e.prototype.column = null, e.prototype.expandable = null, e.prototype.form = null, e.prototype.tabContainer = null, e.prototype.tab = null, e.prototype.chatMessage = null, e.prototype.popover = null, e.prototype.allowEmpty = !1, Object.defineProperty(e.prototype, "type", {
-                            get: a.oneOfGetter(t = ["vertical", "horizontal", "column", "expandable", "form", "tabContainer", "tab", "chatMessage", "popover"]),
+                        return e.prototype.vertical = null, e.prototype.horizontal = null, e.prototype.column = null, e.prototype.expandable = null, e.prototype.form = null, e.prototype.tabContainer = null, e.prototype.tab = null, e.prototype.chatMessage = null, e.prototype.popover = null, e.prototype.dialog = null, e.prototype.allowEmpty = !1, Object.defineProperty(e.prototype, "type", {
+                            get: a.oneOfGetter(t = ["vertical", "horizontal", "column", "expandable", "form", "tabContainer", "tab", "chatMessage", "popover", "dialog"]),
                             set: a.oneOfSetter(t)
                         }), e.create = function(t) {
                             return new e(t)
                         }, e.encode = function(e, t) {
-                            return t || (t = i.create()), null != e.vertical && Object.hasOwnProperty.call(e, "vertical") && s.Block.Vertical.encode(e.vertical, t.uint32(10).fork()).ldelim(), null != e.horizontal && Object.hasOwnProperty.call(e, "horizontal") && s.Block.Horizontal.encode(e.horizontal, t.uint32(18).fork()).ldelim(), null != e.column && Object.hasOwnProperty.call(e, "column") && s.Block.Column.encode(e.column, t.uint32(26).fork()).ldelim(), null != e.expandable && Object.hasOwnProperty.call(e, "expandable") && s.Block.Expandable.encode(e.expandable, t.uint32(34).fork()).ldelim(), null != e.form && Object.hasOwnProperty.call(e, "form") && s.Block.Form.encode(e.form, t.uint32(42).fork()).ldelim(), null != e.tabContainer && Object.hasOwnProperty.call(e, "tabContainer") && s.Block.TabContainer.encode(e.tabContainer, t.uint32(50).fork()).ldelim(), null != e.tab && Object.hasOwnProperty.call(e, "tab") && s.Block.Tab.encode(e.tab, t.uint32(58).fork()).ldelim(), null != e.allowEmpty && Object.hasOwnProperty.call(e, "allowEmpty") && t.uint32(64).bool(e.allowEmpty), null != e.chatMessage && Object.hasOwnProperty.call(e, "chatMessage") && s.Block.ChatMessage.encode(e.chatMessage, t.uint32(74).fork()).ldelim(), null != e.popover && Object.hasOwnProperty.call(e, "popover") && s.Block.Popover.encode(e.popover, t.uint32(82).fork()).ldelim(), t
+                            return t || (t = i.create()), null != e.vertical && Object.hasOwnProperty.call(e, "vertical") && s.Block.Vertical.encode(e.vertical, t.uint32(10).fork()).ldelim(), null != e.horizontal && Object.hasOwnProperty.call(e, "horizontal") && s.Block.Horizontal.encode(e.horizontal, t.uint32(18).fork()).ldelim(), null != e.column && Object.hasOwnProperty.call(e, "column") && s.Block.Column.encode(e.column, t.uint32(26).fork()).ldelim(), null != e.expandable && Object.hasOwnProperty.call(e, "expandable") && s.Block.Expandable.encode(e.expandable, t.uint32(34).fork()).ldelim(), null != e.form && Object.hasOwnProperty.call(e, "form") && s.Block.Form.encode(e.form, t.uint32(42).fork()).ldelim(), null != e.tabContainer && Object.hasOwnProperty.call(e, "tabContainer") && s.Block.TabContainer.encode(e.tabContainer, t.uint32(50).fork()).ldelim(), null != e.tab && Object.hasOwnProperty.call(e, "tab") && s.Block.Tab.encode(e.tab, t.uint32(58).fork()).ldelim(), null != e.allowEmpty && Object.hasOwnProperty.call(e, "allowEmpty") && t.uint32(64).bool(e.allowEmpty), null != e.chatMessage && Object.hasOwnProperty.call(e, "chatMessage") && s.Block.ChatMessage.encode(e.chatMessage, t.uint32(74).fork()).ldelim(), null != e.popover && Object.hasOwnProperty.call(e, "popover") && s.Block.Popover.encode(e.popover, t.uint32(82).fork()).ldelim(), null != e.dialog && Object.hasOwnProperty.call(e, "dialog") && s.Block.Dialog.encode(e.dialog, t.uint32(90).fork()).ldelim(), t
                         }, e.encodeDelimited = function(e, t) {
                             return this.encode(e, t).ldelim()
                         }, e.decode = function(e, t) {
                             e instanceof o || (e = o.create(e));
                             let n = void 0 === t ? e.len : e.pos + t,
                                 r = new s.Block;
                             for (; e.pos < n;) {
@@ -36939,14 +36948,17 @@
                                         break;
                                     case 9:
                                         r.chatMessage = s.Block.ChatMessage.decode(e, e.uint32());
                                         break;
                                     case 10:
                                         r.popover = s.Block.Popover.decode(e, e.uint32());
                                         break;
+                                    case 11:
+                                        r.dialog = s.Block.Dialog.decode(e, e.uint32());
+                                        break;
                                     case 8:
                                         r.allowEmpty = e.bool();
                                         break;
                                     default:
                                         e.skipType(7 & t)
                                 }
                             }
@@ -37023,14 +37035,22 @@
                                 if (1 === t.type) return "type: multiple values";
                                 t.type = 1;
                                 {
                                     let t = s.Block.Popover.verify(e.popover);
                                     if (t) return "popover." + t
                                 }
                             }
+                            if (null != e.dialog && e.hasOwnProperty("dialog")) {
+                                if (1 === t.type) return "type: multiple values";
+                                t.type = 1;
+                                {
+                                    let t = s.Block.Dialog.verify(e.dialog);
+                                    if (t) return "dialog." + t
+                                }
+                            }
                             return null != e.allowEmpty && e.hasOwnProperty("allowEmpty") && "boolean" !== typeof e.allowEmpty ? "allowEmpty: boolean expected" : null
                         }, e.fromObject = function(e) {
                             if (e instanceof s.Block) return e;
                             let t = new s.Block;
                             if (null != e.vertical) {
                                 if ("object" !== typeof e.vertical) throw TypeError(".Block.vertical: object expected");
                                 t.vertical = s.Block.Vertical.fromObject(e.vertical)
@@ -37063,19 +37083,23 @@
                                 if ("object" !== typeof e.chatMessage) throw TypeError(".Block.chatMessage: object expected");
                                 t.chatMessage = s.Block.ChatMessage.fromObject(e.chatMessage)
                             }
                             if (null != e.popover) {
                                 if ("object" !== typeof e.popover) throw TypeError(".Block.popover: object expected");
                                 t.popover = s.Block.Popover.fromObject(e.popover)
                             }
+                            if (null != e.dialog) {
+                                if ("object" !== typeof e.dialog) throw TypeError(".Block.dialog: object expected");
+                                t.dialog = s.Block.Dialog.fromObject(e.dialog)
+                            }
                             return null != e.allowEmpty && (t.allowEmpty = Boolean(e.allowEmpty)), t
                         }, e.toObject = function(e, t) {
                             t || (t = {});
                             let n = {};
-                            return t.defaults && (n.allowEmpty = !1), null != e.vertical && e.hasOwnProperty("vertical") && (n.vertical = s.Block.Vertical.toObject(e.vertical, t), t.oneofs && (n.type = "vertical")), null != e.horizontal && e.hasOwnProperty("horizontal") && (n.horizontal = s.Block.Horizontal.toObject(e.horizontal, t), t.oneofs && (n.type = "horizontal")), null != e.column && e.hasOwnProperty("column") && (n.column = s.Block.Column.toObject(e.column, t), t.oneofs && (n.type = "column")), null != e.expandable && e.hasOwnProperty("expandable") && (n.expandable = s.Block.Expandable.toObject(e.expandable, t), t.oneofs && (n.type = "expandable")), null != e.form && e.hasOwnProperty("form") && (n.form = s.Block.Form.toObject(e.form, t), t.oneofs && (n.type = "form")), null != e.tabContainer && e.hasOwnProperty("tabContainer") && (n.tabContainer = s.Block.TabContainer.toObject(e.tabContainer, t), t.oneofs && (n.type = "tabContainer")), null != e.tab && e.hasOwnProperty("tab") && (n.tab = s.Block.Tab.toObject(e.tab, t), t.oneofs && (n.type = "tab")), null != e.allowEmpty && e.hasOwnProperty("allowEmpty") && (n.allowEmpty = e.allowEmpty), null != e.chatMessage && e.hasOwnProperty("chatMessage") && (n.chatMessage = s.Block.ChatMessage.toObject(e.chatMessage, t), t.oneofs && (n.type = "chatMessage")), null != e.popover && e.hasOwnProperty("popover") && (n.popover = s.Block.Popover.toObject(e.popover, t), t.oneofs && (n.type = "popover")), n
+                            return t.defaults && (n.allowEmpty = !1), null != e.vertical && e.hasOwnProperty("vertical") && (n.vertical = s.Block.Vertical.toObject(e.vertical, t), t.oneofs && (n.type = "vertical")), null != e.horizontal && e.hasOwnProperty("horizontal") && (n.horizontal = s.Block.Horizontal.toObject(e.horizontal, t), t.oneofs && (n.type = "horizontal")), null != e.column && e.hasOwnProperty("column") && (n.column = s.Block.Column.toObject(e.column, t), t.oneofs && (n.type = "column")), null != e.expandable && e.hasOwnProperty("expandable") && (n.expandable = s.Block.Expandable.toObject(e.expandable, t), t.oneofs && (n.type = "expandable")), null != e.form && e.hasOwnProperty("form") && (n.form = s.Block.Form.toObject(e.form, t), t.oneofs && (n.type = "form")), null != e.tabContainer && e.hasOwnProperty("tabContainer") && (n.tabContainer = s.Block.TabContainer.toObject(e.tabContainer, t), t.oneofs && (n.type = "tabContainer")), null != e.tab && e.hasOwnProperty("tab") && (n.tab = s.Block.Tab.toObject(e.tab, t), t.oneofs && (n.type = "tab")), null != e.allowEmpty && e.hasOwnProperty("allowEmpty") && (n.allowEmpty = e.allowEmpty), null != e.chatMessage && e.hasOwnProperty("chatMessage") && (n.chatMessage = s.Block.ChatMessage.toObject(e.chatMessage, t), t.oneofs && (n.type = "chatMessage")), null != e.popover && e.hasOwnProperty("popover") && (n.popover = s.Block.Popover.toObject(e.popover, t), t.oneofs && (n.type = "popover")), null != e.dialog && e.hasOwnProperty("dialog") && (n.dialog = s.Block.Dialog.toObject(e.dialog, t), t.oneofs && (n.type = "dialog")), n
                         }, e.prototype.toJSON = function() {
                             return this.constructor.toObject(this, r.util.toJSONOptions)
                         }, e.getTypeUrl = function(e) {
                             return void 0 === e && (e = "type.googleapis.com"), e + "/Block"
                         }, e.Vertical = function() {
                             function e(e) {
                                 if (e)
@@ -37257,14 +37281,99 @@
                                 let n = {};
                                 return t.defaults && (n.label = "", n.icon = ""), null != e.label && e.hasOwnProperty("label") && (n.label = e.label), null != e.expanded && e.hasOwnProperty("expanded") && (n.expanded = e.expanded, t.oneofs && (n._expanded = "expanded")), null != e.icon && e.hasOwnProperty("icon") && (n.icon = e.icon), n
                             }, e.prototype.toJSON = function() {
                                 return this.constructor.toObject(this, r.util.toJSONOptions)
                             }, e.getTypeUrl = function(e) {
                                 return void 0 === e && (e = "type.googleapis.com"), e + "/Block.Expandable"
                             }, e
+                        }(), e.Dialog = function() {
+                            function e(e) {
+                                if (e)
+                                    for (let t = Object.keys(e), n = 0; n < t.length; ++n) null != e[t[n]] && (this[t[n]] = e[t[n]])
+                            }
+                            let t;
+                            return e.prototype.title = "", e.prototype.dismissible = !1, e.prototype.width = 0, e.prototype.isOpen = null, Object.defineProperty(e.prototype, "_isOpen", {
+                                get: a.oneOfGetter(t = ["isOpen"]),
+                                set: a.oneOfSetter(t)
+                            }), e.create = function(t) {
+                                return new e(t)
+                            }, e.encode = function(e, t) {
+                                return t || (t = i.create()), null != e.title && Object.hasOwnProperty.call(e, "title") && t.uint32(10).string(e.title), null != e.dismissible && Object.hasOwnProperty.call(e, "dismissible") && t.uint32(16).bool(e.dismissible), null != e.width && Object.hasOwnProperty.call(e, "width") && t.uint32(24).int32(e.width), null != e.isOpen && Object.hasOwnProperty.call(e, "isOpen") && t.uint32(32).bool(e.isOpen), t
+                            }, e.encodeDelimited = function(e, t) {
+                                return this.encode(e, t).ldelim()
+                            }, e.decode = function(e, t) {
+                                e instanceof o || (e = o.create(e));
+                                let n = void 0 === t ? e.len : e.pos + t,
+                                    r = new s.Block.Dialog;
+                                for (; e.pos < n;) {
+                                    let t = e.uint32();
+                                    switch (t >>> 3) {
+                                        case 1:
+                                            r.title = e.string();
+                                            break;
+                                        case 2:
+                                            r.dismissible = e.bool();
+                                            break;
+                                        case 3:
+                                            r.width = e.int32();
+                                            break;
+                                        case 4:
+                                            r.isOpen = e.bool();
+                                            break;
+                                        default:
+                                            e.skipType(7 & t)
+                                    }
+                                }
+                                return r
+                            }, e.decodeDelimited = function(e) {
+                                return e instanceof o || (e = new o(e)), this.decode(e, e.uint32())
+                            }, e.verify = function(e) {
+                                if ("object" !== typeof e || null === e) return "object expected";
+                                let t = {};
+                                if (null != e.title && e.hasOwnProperty("title") && !a.isString(e.title)) return "title: string expected";
+                                if (null != e.dismissible && e.hasOwnProperty("dismissible") && "boolean" !== typeof e.dismissible) return "dismissible: boolean expected";
+                                if (null != e.width && e.hasOwnProperty("width")) switch (e.width) {
+                                    default:
+                                        return "width: enum value expected";
+                                    case 0:
+                                    case 1:
+                                }
+                                return null != e.isOpen && e.hasOwnProperty("isOpen") && (t._isOpen = 1, "boolean" !== typeof e.isOpen) ? "isOpen: boolean expected" : null
+                            }, e.fromObject = function(e) {
+                                if (e instanceof s.Block.Dialog) return e;
+                                let t = new s.Block.Dialog;
+                                switch (null != e.title && (t.title = String(e.title)), null != e.dismissible && (t.dismissible = Boolean(e.dismissible)), e.width) {
+                                    default:
+                                        if ("number" === typeof e.width) {
+                                            t.width = e.width;
+                                            break
+                                        }
+                                        break;
+                                    case "SMALL":
+                                    case 0:
+                                        t.width = 0;
+                                        break;
+                                    case "LARGE":
+                                    case 1:
+                                        t.width = 1
+                                }
+                                return null != e.isOpen && (t.isOpen = Boolean(e.isOpen)), t
+                            }, e.toObject = function(e, t) {
+                                t || (t = {});
+                                let n = {};
+                                return t.defaults && (n.title = "", n.dismissible = !1, n.width = t.enums === String ? "SMALL" : 0), null != e.title && e.hasOwnProperty("title") && (n.title = e.title), null != e.dismissible && e.hasOwnProperty("dismissible") && (n.dismissible = e.dismissible), null != e.width && e.hasOwnProperty("width") && (n.width = t.enums === String ? void 0 === s.Block.Dialog.DialogWidth[e.width] ? e.width : s.Block.Dialog.DialogWidth[e.width] : e.width), null != e.isOpen && e.hasOwnProperty("isOpen") && (n.isOpen = e.isOpen, t.oneofs && (n._isOpen = "isOpen")), n
+                            }, e.prototype.toJSON = function() {
+                                return this.constructor.toObject(this, r.util.toJSONOptions)
+                            }, e.getTypeUrl = function(e) {
+                                return void 0 === e && (e = "type.googleapis.com"), e + "/Block.Dialog"
+                            }, e.DialogWidth = function() {
+                                const e = {},
+                                    t = Object.create(e);
+                                return t[e[0] = "SMALL"] = 0, t[e[1] = "LARGE"] = 1, t
+                            }(), e
                         }(), e.Form = function() {
                             function e(e) {
                                 if (e)
                                     for (let t = Object.keys(e), n = 0; n < t.length; ++n) null != e[t[n]] && (this[t[n]] = e[t[n]])
                             }
                             return e.prototype.formId = "", e.prototype.clearOnSubmit = !1, e.prototype.border = !1, e.create = function(t) {
                                 return new e(t)
@@ -38697,18 +38806,18 @@
                             return void 0 === e && (e = "type.googleapis.com"), e + "/FileURLsResponse"
                         }, e
                     })(), s.UploadedFileInfo = (() => {
                         function e(e) {
                             if (e)
                                 for (let t = Object.keys(e), n = 0; n < t.length; ++n) null != e[t[n]] && (this[t[n]] = e[t[n]])
                         }
-                        return e.prototype.id = a.Long ? a.Long.fromBits(0, 0, !1) : 0, e.prototype.name = "", e.prototype.size = 0, e.prototype.fileId = "", e.prototype.fileUrls = null, e.create = function(t) {
+                        return e.prototype.id = a.Long ? a.Long.fromBits(0, 0, !1) : 0, e.prototype.name = "", e.prototype.size = a.Long ? a.Long.fromBits(0, 0, !0) : 0, e.prototype.fileId = "", e.prototype.fileUrls = null, e.create = function(t) {
                             return new e(t)
                         }, e.encode = function(e, t) {
-                            return t || (t = i.create()), null != e.id && Object.hasOwnProperty.call(e, "id") && t.uint32(8).sint64(e.id), null != e.name && Object.hasOwnProperty.call(e, "name") && t.uint32(18).string(e.name), null != e.size && Object.hasOwnProperty.call(e, "size") && t.uint32(24).uint32(e.size), null != e.fileId && Object.hasOwnProperty.call(e, "fileId") && t.uint32(34).string(e.fileId), null != e.fileUrls && Object.hasOwnProperty.call(e, "fileUrls") && s.FileURLs.encode(e.fileUrls, t.uint32(42).fork()).ldelim(), t
+                            return t || (t = i.create()), null != e.id && Object.hasOwnProperty.call(e, "id") && t.uint32(8).sint64(e.id), null != e.name && Object.hasOwnProperty.call(e, "name") && t.uint32(18).string(e.name), null != e.size && Object.hasOwnProperty.call(e, "size") && t.uint32(24).uint64(e.size), null != e.fileId && Object.hasOwnProperty.call(e, "fileId") && t.uint32(34).string(e.fileId), null != e.fileUrls && Object.hasOwnProperty.call(e, "fileUrls") && s.FileURLs.encode(e.fileUrls, t.uint32(42).fork()).ldelim(), t
                         }, e.encodeDelimited = function(e, t) {
                             return this.encode(e, t).ldelim()
                         }, e.decode = function(e, t) {
                             e instanceof o || (e = o.create(e));
                             let n = void 0 === t ? e.len : e.pos + t,
                                 r = new s.UploadedFileInfo;
                             for (; e.pos < n;) {
@@ -38717,15 +38826,15 @@
                                     case 1:
                                         r.id = e.sint64();
                                         break;
                                     case 2:
                                         r.name = e.string();
                                         break;
                                     case 3:
-                                        r.size = e.uint32();
+                                        r.size = e.uint64();
                                         break;
                                     case 4:
                                         r.fileId = e.string();
                                         break;
                                     case 5:
                                         r.fileUrls = s.FileURLs.decode(e, e.uint32());
                                         break;
@@ -38736,40 +38845,44 @@
                             return r
                         }, e.decodeDelimited = function(e) {
                             return e instanceof o || (e = new o(e)), this.decode(e, e.uint32())
                         }, e.verify = function(e) {
                             if ("object" !== typeof e || null === e) return "object expected";
                             if (null != e.id && e.hasOwnProperty("id") && !a.isInteger(e.id) && !(e.id && a.isInteger(e.id.low) && a.isInteger(e.id.high))) return "id: integer|Long expected";
                             if (null != e.name && e.hasOwnProperty("name") && !a.isString(e.name)) return "name: string expected";
-                            if (null != e.size && e.hasOwnProperty("size") && !a.isInteger(e.size)) return "size: integer expected";
+                            if (null != e.size && e.hasOwnProperty("size") && !a.isInteger(e.size) && !(e.size && a.isInteger(e.size.low) && a.isInteger(e.size.high))) return "size: integer|Long expected";
                             if (null != e.fileId && e.hasOwnProperty("fileId") && !a.isString(e.fileId)) return "fileId: string expected";
                             if (null != e.fileUrls && e.hasOwnProperty("fileUrls")) {
                                 let t = s.FileURLs.verify(e.fileUrls);
                                 if (t) return "fileUrls." + t
                             }
                             return null
                         }, e.fromObject = function(e) {
                             if (e instanceof s.UploadedFileInfo) return e;
                             let t = new s.UploadedFileInfo;
-                            if (null != e.id && (a.Long ? (t.id = a.Long.fromValue(e.id)).unsigned = !1 : "string" === typeof e.id ? t.id = parseInt(e.id, 10) : "number" === typeof e.id ? t.id = e.id : "object" === typeof e.id && (t.id = new a.LongBits(e.id.low >>> 0, e.id.high >>> 0).toNumber())), null != e.name && (t.name = String(e.name)), null != e.size && (t.size = e.size >>> 0), null != e.fileId && (t.fileId = String(e.fileId)), null != e.fileUrls) {
+                            if (null != e.id && (a.Long ? (t.id = a.Long.fromValue(e.id)).unsigned = !1 : "string" === typeof e.id ? t.id = parseInt(e.id, 10) : "number" === typeof e.id ? t.id = e.id : "object" === typeof e.id && (t.id = new a.LongBits(e.id.low >>> 0, e.id.high >>> 0).toNumber())), null != e.name && (t.name = String(e.name)), null != e.size && (a.Long ? (t.size = a.Long.fromValue(e.size)).unsigned = !0 : "string" === typeof e.size ? t.size = parseInt(e.size, 10) : "number" === typeof e.size ? t.size = e.size : "object" === typeof e.size && (t.size = new a.LongBits(e.size.low >>> 0, e.size.high >>> 0).toNumber(!0))), null != e.fileId && (t.fileId = String(e.fileId)), null != e.fileUrls) {
                                 if ("object" !== typeof e.fileUrls) throw TypeError(".UploadedFileInfo.fileUrls: object expected");
                                 t.fileUrls = s.FileURLs.fromObject(e.fileUrls)
                             }
                             return t
                         }, e.toObject = function(e, t) {
                             t || (t = {});
                             let n = {};
                             if (t.defaults) {
                                 if (a.Long) {
                                     let e = new a.Long(0, 0, !1);
                                     n.id = t.longs === String ? e.toString() : t.longs === Number ? e.toNumber() : e
                                 } else n.id = t.longs === String ? "0" : 0;
-                                n.name = "", n.size = 0, n.fileId = "", n.fileUrls = null
+                                if (n.name = "", a.Long) {
+                                    let e = new a.Long(0, 0, !0);
+                                    n.size = t.longs === String ? e.toString() : t.longs === Number ? e.toNumber() : e
+                                } else n.size = t.longs === String ? "0" : 0;
+                                n.fileId = "", n.fileUrls = null
                             }
-                            return null != e.id && e.hasOwnProperty("id") && ("number" === typeof e.id ? n.id = t.longs === String ? String(e.id) : e.id : n.id = t.longs === String ? a.Long.prototype.toString.call(e.id) : t.longs === Number ? new a.LongBits(e.id.low >>> 0, e.id.high >>> 0).toNumber() : e.id), null != e.name && e.hasOwnProperty("name") && (n.name = e.name), null != e.size && e.hasOwnProperty("size") && (n.size = e.size), null != e.fileId && e.hasOwnProperty("fileId") && (n.fileId = e.fileId), null != e.fileUrls && e.hasOwnProperty("fileUrls") && (n.fileUrls = s.FileURLs.toObject(e.fileUrls, t)), n
+                            return null != e.id && e.hasOwnProperty("id") && ("number" === typeof e.id ? n.id = t.longs === String ? String(e.id) : e.id : n.id = t.longs === String ? a.Long.prototype.toString.call(e.id) : t.longs === Number ? new a.LongBits(e.id.low >>> 0, e.id.high >>> 0).toNumber() : e.id), null != e.name && e.hasOwnProperty("name") && (n.name = e.name), null != e.size && e.hasOwnProperty("size") && ("number" === typeof e.size ? n.size = t.longs === String ? String(e.size) : e.size : n.size = t.longs === String ? a.Long.prototype.toString.call(e.size) : t.longs === Number ? new a.LongBits(e.size.low >>> 0, e.size.high >>> 0).toNumber(!0) : e.size), null != e.fileId && e.hasOwnProperty("fileId") && (n.fileId = e.fileId), null != e.fileUrls && e.hasOwnProperty("fileUrls") && (n.fileUrls = s.FileURLs.toObject(e.fileUrls, t)), n
                         }, e.prototype.toJSON = function() {
                             return this.constructor.toObject(this, r.util.toJSONOptions)
                         }, e.getTypeUrl = function(e) {
                             return void 0 === e && (e = "type.googleapis.com"), e + "/UploadedFileInfo"
                         }, e
                     })()),
                     O = s.FileUploaderState = (() => {
@@ -48523,15 +48636,14 @@
             },
             48266: (e, t, n) => {
                 "use strict";
                 n.d(t, {
                     A: () => r
                 });
                 const r = {
-                    toast: "68px",
                     hideWidgetDetails: 180,
                     hideNumberInputControls: 120,
                     sm: "576px",
                     columns: "640px",
                     md: "768px",
                     lg: "992px",
                     xl: "1200px"
@@ -77049,14 +77161,15 @@
                             }(e, i, te(e, o), r)
                     }
 
                     function te(e, t) {
                         if (N("{", !0)) {
                             for (var n = {}; !N("}", !0);) {
                                 if (!y.test(x = k())) throw j(x, "name");
+                                if (null === x) throw j(x, "end of input");
                                 var r, o = x;
                                 if (N(":", !0), "{" === W()) r = te(e, t + "." + x);
                                 else if ("[" === W()) {
                                     var i;
                                     if (r = [], N("[", !0)) {
                                         do {
                                             i = U(!0), r.push(i)
@@ -77212,15 +77325,20 @@
                     var e = o.float.readDoubleLE(this.buf, this.pos);
                     return this.pos += 8, e
                 }, l.prototype.bytes = function() {
                     var e = this.uint32(),
                         t = this.pos,
                         n = this.pos + e;
                     if (n > this.len) throw s(this, e);
-                    return this.pos += e, Array.isArray(this.buf) ? this.buf.slice(t, n) : t === n ? new this.buf.constructor(0) : this._slice.call(this.buf, t, n)
+                    if (this.pos += e, Array.isArray(this.buf)) return this.buf.slice(t, n);
+                    if (t === n) {
+                        var r = o.Buffer;
+                        return r ? r.alloc(0) : new this.buf.constructor(0)
+                    }
+                    return this._slice.call(this.buf, t, n)
                 }, l.prototype.string = function() {
                     var e = this.bytes();
                     return a.read(e, 0, e.length)
                 }, l.prototype.skip = function(e) {
                     if ("number" === typeof e) {
                         if (this.pos + e > this.len) throw s(this, e);
                         this.pos += e
@@ -77576,15 +77694,15 @@
                         for (var p = e.substring(t, n).split(a), h = 0; h < p.length; ++h) p[h] = p[h].replace(l ? i : o, "").trim();
                         c.text = p.join("\n").trim(), f[d] = c, b = d
                     }
 
                     function z(t) {
                         var n = y(t),
                             r = e.substring(t, n);
-                        return /^\s*\/{1,2}/.test(r)
+                        return /^\s*\/\//.test(r)
                     }
 
                     function y(e) {
                         for (var t = e; t < p && "\n" !== O(t);) t++;
                         return t
                     }
 
@@ -77602,15 +77720,15 @@
                             if (c === p) return null;
                             for (o = !1; s.test(a = O(c));)
                                 if ("\n" === a && (A = !0, ++d), ++c === p) return null;
                             if ("/" === O(c)) {
                                 if (++c === p) throw M("comment");
                                 if ("/" === O(c))
                                     if (l) {
-                                        if (b = c, f = !1, z(c)) {
+                                        if (b = c, f = !1, z(c - 1)) {
                                             f = !0;
                                             do {
                                                 if ((c = y(c)) === p) break;
                                                 if (c++, !A) break
                                             } while (z(c))
                                         } else c = Math.min(p, y(c) + 1);
                                         f && (g(b, c, A), A = !0), d++, o = !0
@@ -115374,15 +115492,15 @@
     }, __webpack_require__.f = {}, __webpack_require__.e = e => Promise.all(Object.keys(__webpack_require__.f).reduce(((t, n) => (__webpack_require__.f[n](e, t), t)), [])), __webpack_require__.u = e => "static/js/" + e + "." + {
         43: "9ae03282",
         178: "b5384fd0",
         474: "87506447",
         656: "ae85f8f1",
         937: "a1248039",
         1074: "73973756",
-        1168: "3029456a",
+        1168: "1d6408e6",
         1307: "8ea033f1",
         1451: "3b0a3e31",
         1479: "6709db03",
         1792: "b8efa879",
         2187: "9469f035",
         2411: "a8823789",
         2469: "3e9c3ce9",
@@ -115416,15 +115534,15 @@
         7142: "83028745",
         7175: "be4076bc",
         7217: "d970c074",
         7323: "2808d029",
         7602: "6175e969",
         7805: "51638fbc",
         8005: "43974a35",
-        8427: "b0ed496b",
+        8427: "d30dffe1",
         8477: "e948c092",
         8492: "f56c9d4c",
         8570: "6de19120",
         8691: "9ccf7f89",
         9330: "d29313d4",
         9336: "2d95d840",
         9656: "8c935274",
@@ -115556,21 +115674,21 @@
         n.forEach(t.bind(null, 0)), n.push = t.bind(null, n.push.bind(n))
     })();
     var __webpack_exports__ = {};
     (() => {
         "use strict";
         var e = {};
         __webpack_require__.r(e), __webpack_require__.d(e, {
-            exclude: () => zo,
-            extract: () => fo,
-            parse: () => ho,
-            parseUrl: () => Mo,
-            pick: () => go,
-            stringify: () => mo,
-            stringifyUrl: () => Oo
+            exclude: () => ci,
+            extract: () => ri,
+            parse: () => oi,
+            parseUrl: () => ai,
+            pick: () => li,
+            stringify: () => ii,
+            stringifyUrl: () => si
         });
         var t = __webpack_require__(66845),
             n = __webpack_require__(17664);
         class r {
             constructor() {
                 let e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "";
                 this.prefix = e, this.count = 0, this.offset = 374, this.msb = 1295, this.power = 2
@@ -116322,15 +116440,14 @@
             embedded: !1,
             showPadding: !1,
             disableScrolling: !1,
             showToolbar: !1,
             showColoredLine: !1,
             pageLinkBaseUrl: "",
             sidebarChevronDownshift: 0,
-            toastAdjustment: !1,
             gitInfo: null,
             appConfig: {}
         });
         var Fe = __webpack_require__(66694),
             Ue = __webpack_require__(28391),
             Ve = __webpack_require__(63765),
             He = __webpack_require__(50641);
@@ -117504,15 +117621,15 @@
                                     "data-testid": "stPopoverBody"
                                 },
                                 style: () => ({
                                     marginRight: c.spacing.lg,
                                     marginBottom: c.spacing.lg,
                                     maxHeight: "70vh",
                                     overflow: "auto",
-                                    maxWidth: "calc(".concat(c.sizes.contentMaxWidth, " - 2rem)"),
+                                    maxWidth: "calc(".concat(c.sizes.contentMaxWidth, " - 2*").concat(c.spacing.lg, ")"),
                                     minWidth: n.useContainerWidth ? "".concat(Math.max(o, 160), "px") : "20rem",
                                     ["@media (max-width: ".concat(c.breakpoints.sm, ")")]: {
                                         maxWidth: "calc(100% - 2rem)"
                                     },
                                     borderTopLeftRadius: c.radii.xl,
                                     borderTopRightRadius: c.radii.xl,
                                     borderBottomRightRadius: c.radii.xl,
@@ -117760,15 +117877,755 @@
                 }), (0, ge.jsx)(Mn, {
                     "data-testid": "stChatMessageContent",
                     "aria-label": "Chat message from ".concat(a),
                     children: r
                 })]
             })
         };
-        var vn = t.forwardRef((function(e, n) {
+        var vn = {
+                default: "default",
+                full: "full",
+                auto: "auto"
+            },
+            wn = {
+                default: "500px",
+                full: "100%",
+                auto: "auto"
+            },
+            Sn = "closeButton",
+            qn = "backdrop",
+            En = "escape";
+
+        function _n(e, t) {
+            var n = Object.keys(e);
+            if (Object.getOwnPropertySymbols) {
+                var r = Object.getOwnPropertySymbols(e);
+                t && (r = r.filter((function(t) {
+                    return Object.getOwnPropertyDescriptor(e, t).enumerable
+                }))), n.push.apply(n, r)
+            }
+            return n
+        }
+
+        function xn(e) {
+            for (var t = 1; t < arguments.length; t++) {
+                var n = null != arguments[t] ? arguments[t] : {};
+                t % 2 ? _n(Object(n), !0).forEach((function(t) {
+                    Rn(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : _n(Object(n)).forEach((function(t) {
+                    Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
+                }))
+            }
+            return e
+        }
+
+        function Rn(e, t, n) {
+            return t in e ? Object.defineProperty(e, t, {
+                value: n,
+                enumerable: !0,
+                configurable: !0,
+                writable: !0
+            }) : e[t] = n, e
+        }
+        var Tn = (0, at.zo)("div", (function(e) {
+            return {
+                position: "fixed",
+                overflow: "auto",
+                right: 0,
+                bottom: 0,
+                top: 0,
+                left: 0,
+                pointerEvents: e.$isOpen ? "auto" : "none"
+            }
+        }));
+        Tn.displayName = "Root", Tn.displayName = "Root";
+        var kn = (0, at.zo)("div", (function(e) {
+            var t = e.$animate,
+                n = e.$isOpen,
+                r = e.$isVisible,
+                o = e.$theme,
+                i = {
+                    transitionProperty: "opacity",
+                    transitionDuration: o.animation.timing400,
+                    transitionTimingFunction: o.animation.easeOutCurve
+                };
+            return xn({
+                display: "flex",
+                alignItems: "center",
+                justifyContent: "center",
+                width: "100%",
+                minHeight: "100%",
+                userSelect: "none",
+                pointerEvents: "auto",
+                backgroundColor: "rgba(0, 0, 0, 0.5)",
+                WebkitTapHighlightColor: "transparent",
+                opacity: r && n ? 1 : 0
+            }, t ? i : null)
+        }));
+        kn.displayName = "DialogContainer", kn.displayName = "DialogContainer";
+        var Cn = (0, at.zo)("div", (function(e) {
+            var t = e.$animate,
+                n = e.$isOpen,
+                r = e.$isVisible,
+                o = e.$size,
+                i = e.$theme;
+            return xn(xn(xn({
+                position: "relative",
+                backgroundColor: i.colors.backgroundPrimary,
+                borderTopLeftRadius: i.borders.radius500,
+                borderTopRightRadius: i.borders.radius500,
+                borderBottomRightRadius: i.borders.radius500,
+                borderBottomLeftRadius: i.borders.radius500,
+                marginLeft: i.sizing.scale600,
+                marginTop: i.sizing.scale600,
+                marginRight: i.sizing.scale600,
+                marginBottom: i.sizing.scale600
+            }, function(e) {
+                var t = {
+                    maxWidth: "100%",
+                    width: null
+                };
+                return "number" === typeof e ? t.width = "".concat(e, "px") : vn[e] ? t.width = wn[e] : "string" === typeof e && (t.width = e), e === vn.full && (t.alignSelf = "stretch"), t
+            }(o)), {}, {
+                opacity: r && n ? 1 : 0,
+                transform: r ? "translateY(0)" : "translateY(20px)"
+            }, t ? {
+                transitionProperty: "opacity, transform",
+                transitionDuration: i.animation.timing400,
+                transitionTimingFunction: i.animation.easeOutCurve
+            } : null), {}, {
+                userSelect: "text",
+                pointerEvents: n ? "all" : "none",
+                ":focus": {
+                    outline: "none"
+                }
+            })
+        }));
+        Cn.displayName = "Dialog", Cn.displayName = "Dialog";
+        var Wn = (0, at.zo)("button", (function(e) {
+            var t, n = e.$theme,
+                r = e.$isFocusVisible,
+                o = "rtl" === n.direction ? "left" : "right";
+            return Rn(t = {
+                background: "transparent",
+                outline: 0,
+                paddingLeft: 0,
+                paddingTop: 0,
+                paddingRight: 0,
+                paddingBottom: 0,
+                color: n.colors.modalCloseColor,
+                transitionProperty: "color, border-color",
+                transitionDuration: n.animation.timing200,
+                borderLeftWidth: "1px",
+                borderRightWidth: "1px",
+                borderTopWidth: "1px",
+                borderBottomWidth: "1px",
+                borderLeftStyle: "solid",
+                borderRightStyle: "solid",
+                borderTopStyle: "solid",
+                borderBottomStyle: "solid",
+                borderLeftColor: "transparent",
+                borderRightColor: "transparent",
+                borderTopColor: "transparent",
+                borderBottomColor: "transparent",
+                ":hover": {
+                    color: n.colors.modalCloseColorHover
+                },
+                ":focus": {
+                    outline: r ? "3px solid ".concat(n.colors.accent) : "none"
+                },
+                position: "absolute",
+                top: n.sizing.scale500
+            }, o, n.sizing.scale500), Rn(t, "width", n.sizing.scale800), Rn(t, "height", n.sizing.scale800), Rn(t, "display", "flex"), Rn(t, "justifyContent", "center"), Rn(t, "alignItems", "center"), Rn(t, "cursor", "pointer"), t
+        }));
+        Wn.displayName = "Close", Wn.displayName = "Close";
+        var Nn = (0, at.zo)("div", (function(e) {
+            var t, n = e.$theme,
+                r = "rtl" === n.direction ? "marginRight" : "marginLeft",
+                o = "rtl" === n.direction ? "marginLeft" : "marginRight";
+            return xn(xn({}, n.typography.font550), {}, (Rn(t = {
+                color: n.colors.contentPrimary,
+                marginTop: n.sizing.scale900,
+                marginBottom: n.sizing.scale600
+            }, r, n.sizing.scale800), Rn(t, o, n.sizing.scale900), t))
+        }));
+        Nn.displayName = "ModalHeader", Nn.displayName = "ModalHeader";
+        var Ln = (0, at.zo)("div", (function(e) {
+            var t = e.$theme;
+            return xn(xn({}, t.typography.font200), {}, {
+                color: t.colors.contentSecondary,
+                marginTop: t.sizing.scale600,
+                marginLeft: t.sizing.scale800,
+                marginRight: t.sizing.scale800,
+                marginBottom: t.sizing.scale700
+            })
+        }));
+        Ln.displayName = "ModalBody", Ln.displayName = "ModalBody";
+        var In = (0, at.zo)("div", (function(e) {
+            var t = e.$theme;
+            return xn(xn({}, t.typography.font200), {}, {
+                marginTop: t.sizing.scale700,
+                marginLeft: t.sizing.scale800,
+                marginRight: t.sizing.scale800,
+                paddingTop: t.sizing.scale500,
+                paddingBottom: t.sizing.scale500,
+                textAlign: "rtl" === t.direction ? "left" : "right"
+            })
+        }));
+        In.displayName = "ModalFooter", In.displayName = "ModalFooter";
+        var Pn = __webpack_require__(2989),
+            Dn = __webpack_require__(99282),
+            Bn = __webpack_require__(42450);
+
+        function jn() {
+            return t.createElement("svg", {
+                width: "10",
+                height: "10",
+                viewBox: "0 0 10 10",
+                style: {
+                    stroke: "currentColor"
+                },
+                xmlns: "http://www.w3.org/2000/svg"
+            }, t.createElement("path", {
+                d: "M9 1L5 5M1 9L5 5M5 5L1 1M5 5L9 9",
+                strokeWidth: "2",
+                strokeLinecap: "round"
+            }))
+        }
+
+        function Fn(e) {
+            return Fn = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+                return typeof e
+            } : function(e) {
+                return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
+            }, Fn(e)
+        }
+
+        function Un() {
+            return Un = Object.assign ? Object.assign.bind() : function(e) {
+                for (var t = 1; t < arguments.length; t++) {
+                    var n = arguments[t];
+                    for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
+                }
+                return e
+            }, Un.apply(this, arguments)
+        }
+
+        function Vn(e, t) {
+            return function(e) {
+                if (Array.isArray(e)) return e
+            }(e) || function(e, t) {
+                var n = null == e ? null : "undefined" !== typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
+                if (null == n) return;
+                var r, o, i = [],
+                    a = !0,
+                    s = !1;
+                try {
+                    for (n = n.call(e); !(a = (r = n.next()).done) && (i.push(r.value), !t || i.length !== t); a = !0);
+                } catch (l) {
+                    s = !0, o = l
+                } finally {
+                    try {
+                        a || null == n.return || n.return()
+                    } finally {
+                        if (s) throw o
+                    }
+                }
+                return i
+            }(e, t) || function(e, t) {
+                if (!e) return;
+                if ("string" === typeof e) return Hn(e, t);
+                var n = Object.prototype.toString.call(e).slice(8, -1);
+                "Object" === n && e.constructor && (n = e.constructor.name);
+                if ("Map" === n || "Set" === n) return Array.from(e);
+                if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return Hn(e, t)
+            }(e, t) || function() {
+                throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
+            }()
+        }
+
+        function Hn(e, t) {
+            (null == t || t > e.length) && (t = e.length);
+            for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
+            return r
+        }
+
+        function Xn(e, t) {
+            for (var n = 0; n < t.length; n++) {
+                var r = t[n];
+                r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, r.key, r)
+            }
+        }
+
+        function Gn(e, t) {
+            return Gn = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
+                return e.__proto__ = t, e
+            }, Gn(e, t)
+        }
+
+        function $n(e) {
+            var t = function() {
+                if ("undefined" === typeof Reflect || !Reflect.construct) return !1;
+                if (Reflect.construct.sham) return !1;
+                if ("function" === typeof Proxy) return !0;
+                try {
+                    return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
+                } catch (e) {
+                    return !1
+                }
+            }();
+            return function() {
+                var n, r = Yn(e);
+                if (t) {
+                    var o = Yn(this).constructor;
+                    n = Reflect.construct(r, arguments, o)
+                } else n = r.apply(this, arguments);
+                return function(e, t) {
+                    if (t && ("object" === Fn(t) || "function" === typeof t)) return t;
+                    if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
+                    return Kn(e)
+                }(this, n)
+            }
+        }
+
+        function Kn(e) {
+            if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
+            return e
+        }
+
+        function Yn(e) {
+            return Yn = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
+                return e.__proto__ || Object.getPrototypeOf(e)
+            }, Yn(e)
+        }
+
+        function Zn(e, t, n) {
+            return t in e ? Object.defineProperty(e, t, {
+                value: n,
+                enumerable: !0,
+                configurable: !0,
+                writable: !0
+            }) : e[t] = n, e
+        }
+        var Jn = function(e) {
+            ! function(e, t) {
+                if ("function" !== typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
+                e.prototype = Object.create(t && t.prototype, {
+                    constructor: {
+                        value: e,
+                        writable: !0,
+                        configurable: !0
+                    }
+                }), Object.defineProperty(e, "prototype", {
+                    writable: !1
+                }), t && Gn(e, t)
+            }(a, e);
+            var n, r, o, i = $n(a);
+
+            function a() {
+                var e;
+                ! function(e, t) {
+                    if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
+                }(this, a);
+                for (var n = arguments.length, r = new Array(n), o = 0; o < n; o++) r[o] = arguments[o];
+                return Zn(Kn(e = i.call.apply(i, [this].concat(r))), "animateOutTimer", void 0), Zn(Kn(e), "animateStartTimer", void 0), Zn(Kn(e), "dialogContainerRef", t.createRef()), Zn(Kn(e), "lastFocus", null), Zn(Kn(e), "lastMountNodeOverflowStyle", null), Zn(Kn(e), "rootRef", t.createRef()), Zn(Kn(e), "state", {
+                    isVisible: !1,
+                    mounted: !1,
+                    isFocusVisible: !1
+                }), Zn(Kn(e), "handleFocus", (function(t) {
+                    (0, lt.E)(t) && e.setState({
+                        isFocusVisible: !0
+                    })
+                })), Zn(Kn(e), "handleBlur", (function(t) {
+                    !1 !== e.state.isFocusVisible && e.setState({
+                        isFocusVisible: !1
+                    })
+                })), Zn(Kn(e), "onEscape", (function() {
+                    e.props.closeable && e.triggerClose(En)
+                })), Zn(Kn(e), "onDocumentClick", (function(t) {
+                    t.target && t.target instanceof HTMLElement && t.target.contains(e.dialogContainerRef.current) && e.onBackdropClick()
+                })), Zn(Kn(e), "onBackdropClick", (function() {
+                    e.props.closeable && e.triggerClose(qn)
+                })), Zn(Kn(e), "onCloseClick", (function() {
+                    e.triggerClose(Sn)
+                })), Zn(Kn(e), "animateOutComplete", (function() {
+                    e.setState({
+                        isVisible: !1
+                    })
+                })), e
+            }
+            return n = a, r = [{
+                key: "componentDidMount",
+                value: function() {
+                    this.setState({
+                        mounted: !0
+                    })
+                }
+            }, {
+                key: "componentWillUnmount",
+                value: function() {
+                    this.resetMountNodeScroll(), this.clearTimers()
+                }
+            }, {
+                key: "componentDidUpdate",
+                value: function(e, t) {
+                    var n = this.props.isOpen;
+                    (n !== e.isOpen || n && this.state.mounted && !t.mounted) && (n ? this.didOpen() : this.didClose())
+                }
+            }, {
+                key: "disableMountNodeScroll",
+                value: function() {
+                    var e = this.getMountNode();
+                    this.lastMountNodeOverflowStyle = e.style.overflow || "", e.style.overflow = "hidden"
+                }
+            }, {
+                key: "resetMountNodeScroll",
+                value: function() {
+                    var e = this.getMountNode(),
+                        t = this.lastMountNodeOverflowStyle;
+                    e && null !== t && ("hidden" === e.style.overflow && (e.style.overflow = t || ""), this.lastMountNodeOverflowStyle = null)
+                }
+            }, {
+                key: "clearTimers",
+                value: function() {
+                    this.animateOutTimer && clearTimeout(this.animateOutTimer), this.animateStartTimer && cancelAnimationFrame(this.animateStartTimer)
+                }
+            }, {
+                key: "didOpen",
+                value: function() {
+                    var e = this,
+                        t = this.rootRef.current;
+                    t && (t.scrollTop = 0), this.clearTimers(), this.disableMountNodeScroll(), this.animateStartTimer = requestAnimationFrame((function() {
+                        e.setState({
+                            isVisible: !0
+                        })
+                    }))
+                }
+            }, {
+                key: "didClose",
+                value: function() {
+                    this.resetMountNodeScroll(), this.animateOutTimer = setTimeout(this.animateOutComplete, 500)
+                }
+            }, {
+                key: "triggerClose",
+                value: function(e) {
+                    this.props.onClose && e && this.props.onClose({
+                        closeSource: e
+                    })
+                }
+            }, {
+                key: "getSharedProps",
+                value: function() {
+                    var e = this.props,
+                        t = e.animate,
+                        n = e.isOpen,
+                        r = e.size,
+                        o = e.role,
+                        i = e.closeable;
+                    return {
+                        $animate: t,
+                        $isVisible: this.state.isVisible,
+                        $isOpen: !!n,
+                        $size: r,
+                        $role: o,
+                        $closeable: !!i,
+                        $isFocusVisible: this.state.isFocusVisible
+                    }
+                }
+            }, {
+                key: "getMountNode",
+                value: function() {
+                    var e = this.props.mountNode;
+                    return e || document.body
+                }
+            }, {
+                key: "getChildren",
+                value: function() {
+                    var e = this.props.children;
+                    return "function" === typeof e ? e() : e
+                }
+            }, {
+                key: "renderModal",
+                value: function() {
+                    var e = this,
+                        n = this.props,
+                        r = n.overrides,
+                        o = void 0 === r ? {} : r,
+                        i = n.closeable,
+                        a = n.role,
+                        s = n.autoFocus,
+                        l = n.focusLock,
+                        c = n.returnFocus,
+                        u = o.Root,
+                        p = o.Dialog,
+                        d = o.DialogContainer,
+                        b = o.Close,
+                        f = Vn((0, st.jb)(u, Tn), 2),
+                        h = f[0],
+                        m = f[1],
+                        M = Vn((0, st.jb)(d, kn), 2),
+                        O = M[0],
+                        g = M[1],
+                        z = Vn((0, st.jb)(p, Cn), 2),
+                        y = z[0],
+                        A = z[1],
+                        v = Vn((0, st.jb)(b, Wn), 2),
+                        w = v[0],
+                        S = v[1],
+                        q = this.getSharedProps(),
+                        E = this.getChildren();
+                    return t.createElement(Dn.R.Consumer, null, (function(n) {
+                        return t.createElement(Pn.ZP, {
+                            disabled: !l,
+                            crossFrame: !1,
+                            returnFocus: c,
+                            autoFocus: s
+                        }, t.createElement(h, Un({
+                            "data-baseweb": "modal",
+                            ref: e.rootRef
+                        }, q, m), t.createElement(O, Un({
+                            ref: e.dialogContainerRef
+                        }, q, g), t.createElement(y, Un({
+                            tabIndex: -1,
+                            "aria-modal": !0,
+                            "aria-label": "dialog",
+                            role: a
+                        }, q, A), E, i ? t.createElement(w, Un({
+                            "aria-label": n.modal.close,
+                            onClick: e.onCloseClick
+                        }, q, S, {
+                            onFocus: (0, lt.Ah)(S, e.handleFocus),
+                            onBlur: (0, lt.Z5)(S, e.handleBlur)
+                        }), t.createElement(jn, null)) : null))))
+                    }))
+                }
+            }, {
+                key: "render",
+                value: function() {
+                    return this.state.mounted && (this.props.isOpen || this.state.isVisible) ? t.createElement(Bn.Z, {
+                        onEscape: this.onEscape,
+                        onDocumentClick: this.onDocumentClick,
+                        mountNode: this.props.mountNode
+                    }, this.renderModal()) : null
+                }
+            }], r && Xn(n.prototype, r), o && Xn(n, o), Object.defineProperty(n, "prototype", {
+                writable: !1
+            }), a
+        }(t.Component);
+        Zn(Jn, "defaultProps", {
+            animate: !0,
+            autoFocus: !0,
+            focusLock: !0,
+            returnFocus: !0,
+            closeable: !0,
+            name: "dialog",
+            isOpen: !1,
+            overrides: {},
+            role: "dialog",
+            size: vn.default
+        });
+        const Qn = Jn;
+        var er = __webpack_require__(96825),
+            tr = __webpack_require__.n(er);
+        const nr = (0, Qe.Z)("span", {
+            target: "e18cebhv0"
+        })((e => {
+            let {
+                theme: t
+            } = e;
+            return {
+                marginRight: t.spacing.twoXS
+            }
+        }), "");
+
+        function rr(e) {
+            let {
+                children: t
+            } = e;
+            const {
+                genericFonts: n,
+                fontSizes: r,
+                spacing: o
+            } = (0, Ee.u)();
+            return (0, ge.jsx)(Nn, {
+                style: {
+                    marginTop: o.none,
+                    marginLeft: o.none,
+                    marginRight: o.none,
+                    marginBottom: o.none,
+                    paddingTop: o.twoXL,
+                    paddingRight: o.twoXL,
+                    paddingBottom: o.md,
+                    paddingLeft: o.twoXL,
+                    fontFamily: n.bodyFont,
+                    fontSize: r.xl,
+                    fontWeight: 600,
+                    margin: o.none,
+                    lineHeight: 1.5,
+                    textTransform: "none",
+                    display: "flex",
+                    alignItems: "center",
+                    maxHeight: "80vh",
+                    flexDirection: "row"
+                },
+                children: t
+            })
+        }
+
+        function or(e) {
+            let {
+                children: t
+            } = e;
+            const {
+                colors: n,
+                fontSizes: r,
+                spacing: o
+            } = (0, Ee.u)();
+            return (0, ge.jsx)(Ln, {
+                style: {
+                    marginTop: o.none,
+                    marginLeft: o.none,
+                    marginRight: o.none,
+                    marginBottom: o.none,
+                    paddingTop: o.md,
+                    paddingRight: o.twoXL,
+                    paddingBottom: o.twoXL,
+                    paddingLeft: o.twoXL,
+                    color: n.bodyText,
+                    fontSize: r.md,
+                    overflowY: "auto"
+                },
+                children: t
+            })
+        }
+
+        function ir(e) {
+            let {
+                children: t
+            } = e;
+            const {
+                spacing: n
+            } = (0, Ee.u)();
+            return (0, ge.jsx)(In, {
+                style: {
+                    marginTop: n.none,
+                    marginLeft: n.none,
+                    marginRight: n.none,
+                    marginBottom: n.none,
+                    paddingTop: n.md,
+                    paddingRight: n.md,
+                    paddingBottom: n.md,
+                    paddingLeft: n.md
+                },
+                children: (0, ge.jsx)("div", {
+                    className: "ModalBody",
+                    children: t
+                })
+            })
+        }
+        const ar = e => (0, ge.jsx)(nr, {
+            children: (0, ge.jsx)(an.ZP, {
+                ...e
+            })
+        });
+        const sr = function(e) {
+            const {
+                spacing: t,
+                radii: n,
+                colors: r
+            } = (0, Ee.u)(), o = {
+                Root: {
+                    style: {
+                        background: r.darkenedBgMix25
+                    },
+                    props: {
+                        "data-testid": "stModal"
+                    }
+                },
+                DialogContainer: {
+                    style: {
+                        alignItems: "start",
+                        paddingTop: "3rem"
+                    }
+                },
+                Dialog: {
+                    style: {
+                        borderBottomRadius: n.xl,
+                        borderTopRadius: n.xl,
+                        borderLeftRadius: n.xl,
+                        borderRightRadius: n.xl,
+                        minWidth: "20rem"
+                    }
+                },
+                Close: {
+                    style: {
+                        top: "calc(".concat(t.twoXL, " + .375rem)"),
+                        right: t.twoXL
+                    }
+                }
+            }, i = tr()(o, e.overrides);
+            return (0, ge.jsx)(Qn, {
+                ...e,
+                overrides: i
+            })
+        };
+        var lr = __webpack_require__(78693);
+        const cr = (0, Qe.Z)("div", {
+            target: "eh5ke330"
+        })((e => {
+            let {
+                theme: t
+            } = e;
+            return (0, ye.XE)(t)
+        }), "");
+        const ur = e => {
+            let {
+                element: n,
+                children: r
+            } = e;
+            const {
+                title: o,
+                dismissible: i,
+                width: a,
+                isOpen: s
+            } = n, [l, c] = (0, t.useState)(!1);
+            (0, t.useEffect)((() => {
+                (0, He.bb)(s) && c(s)
+            }), [s]);
+            const u = (0, Ee.u)(),
+                p = (0, t.useMemo)((() => function(e, t) {
+                    if (e === Be.gO.Dialog.DialogWidth.LARGE) {
+                        const e = t.spacing.lg;
+                        return "calc(".concat(t.sizes.contentMaxWidth, " + ").concat(e, ")")
+                    }
+                    return vn.default
+                }(null !== a && void 0 !== a ? a : Be.gO.Dialog.DialogWidth.SMALL, u)), [a, u]);
+            return (0, ge.jsxs)(sr, {
+                isOpen: l,
+                closeable: i,
+                onClose: () => c(!1),
+                size: p,
+                children: [(0, ge.jsx)(rr, {
+                    children: o
+                }), (0, ge.jsx)(or, {
+                    children: (0, ge.jsx)(cr, {
+                        children: r
+                    })
+                })]
+            })
+        };
+        const pr = function(e) {
+            return (0, ge.jsx)(lr.Z.Provider, {
+                value: !0,
+                children: (0, ge.jsx)(ur, {
+                    ...e
+                })
+            })
+        };
+        var dr = t.forwardRef((function(e, n) {
             return t.createElement(en.D, (0, Qt.Z)({
                 iconAttrs: {
                     fill: "currentColor",
                     xmlns: "http://www.w3.org/2000/svg"
                 },
                 iconVerticalAlign: "middle",
                 iconViewBox: "0 0 24 24"
@@ -117777,37 +118634,37 @@
             }), t.createElement("path", {
                 fill: "none",
                 d: "M0 0h24v24H0V0z"
             }), t.createElement("path", {
                 d: "M9 16.17L4.83 12l-1.42 1.41L9 19 21 7l-1.41-1.41L9 16.17z"
             }))
         }));
-        vn.displayName = "Check";
-        var wn = t.forwardRef((function(e, n) {
+        dr.displayName = "Check";
+        var br = t.forwardRef((function(e, n) {
             return t.createElement(en.D, (0, Qt.Z)({
                 iconAttrs: {
                     fill: "currentColor",
                     xmlns: "http://www.w3.org/2000/svg"
                 },
                 iconVerticalAlign: "middle",
                 iconViewBox: "0 0 24 24"
             }, e, {
                 ref: n
             }), t.createElement("path", {
                 d: "M11 15h2v2h-2v-2zm0-8h2v6h-2V7zm.99-5C6.47 2 2 6.48 2 12s4.47 10 9.99 10C17.52 22 22 17.52 22 12S17.52 2 11.99 2zM12 20c-4.42 0-8-3.58-8-8s3.58-8 8-8 8 3.58 8 8-3.58 8-8 8z"
             }))
         }));
-        wn.displayName = "ErrorOutline";
-        const Sn = (0, Qe.Z)("div", {
+        br.displayName = "ErrorOutline";
+        const fr = (0, Qe.Z)("div", {
                 target: "eqpbllx5"
             })({
                 name: "0",
                 styles: ""
             }),
-            qn = (0, Qe.Z)("details", {
+            hr = (0, Qe.Z)("details", {
                 target: "eqpbllx4"
             })((e => {
                 let {
                     isStale: t,
                     theme: n
                 } = e;
                 return {
@@ -117820,28 +118677,28 @@
                     borderRadius: n.radii.lg,
                     ...t ? {
                         borderColor: n.colors.fadedText05,
                         transition: "border 1s ease-in 0.5s"
                     } : {}
                 }
             }), ""),
-            En = (0, Qe.Z)("span", {
+            mr = (0, Qe.Z)("span", {
                 target: "eqpbllx3"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     display: "flex",
                     gap: t.spacing.sm,
                     alignItems: "center",
                     flexGrow: 1
                 }
             }), ""),
-            _n = (0, Qe.Z)("summary", {
+            Mr = (0, Qe.Z)("summary", {
                 target: "eqpbllx2"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     position: "relative",
@@ -117865,27 +118722,27 @@
                         color: t.colors.primary
                     },
                     "&:hover svg": {
                         fill: t.colors.primary
                     }
                 }
             }), ""),
-            xn = (0, Qe.Z)("div", {
+            Or = (0, Qe.Z)("div", {
                 target: "eqpbllx1"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     paddingBottom: t.spacing.lg,
                     paddingLeft: t.spacing.lg,
                     paddingRight: t.spacing.lg
                 }
             }), ""),
-            Rn = (0, Qe.Z)("div", {
+            gr = (0, Qe.Z)("div", {
                 target: "eqpbllx0"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     color: t.colors.darkGray,
@@ -117893,15 +118750,15 @@
                     fontSize: t.fontSizes.sm,
                     textAlign: "center",
                     paddingBottom: t.spacing.lg,
                     paddingLeft: t.spacing.lg,
                     paddingRight: t.spacing.lg
                 }
             }), ""),
-            Tn = e => {
+            zr = e => {
                 const {
                     icon: n
                 } = e, {
                     activeTheme: r
                 } = t.useContext(Fe.E), o = {
                     size: "lg",
                     margin: "",
@@ -117912,28 +118769,28 @@
                     return (0, ge.jsx)(rn.qu, {
                         usingCustomTheme: e,
                         "data-testid": "stExpanderIconSpinner",
                         ...o
                     })
                 }
                 return "check" === n ? (0, ge.jsx)(rn.xL, {
-                    as: vn,
+                    as: dr,
                     color: "inherit",
                     "aria-hidden": "true",
                     "data-testid": "stExpanderIconCheck",
                     ...o
                 }) : "error" === n ? (0, ge.jsx)(rn.xL, {
-                    as: wn,
+                    as: br,
                     color: "inherit",
                     "aria-hidden": "true",
                     "data-testid": "stExpanderIconError",
                     ...o
                 }) : (0, ge.jsx)(ge.Fragment, {})
             },
-            kn = e => {
+            yr = e => {
                 let {
                     element: n,
                     isStale: r,
                     empty: o,
                     children: i
                 } = e;
                 const {
@@ -117953,20 +118810,20 @@
                         easing: "cubic-bezier(0.23, 1, 0.32, 1)"
                     });
                     o.onfinish = () => {
                         return e = r, void(u.current && (u.current.open = e, d.current = null, u.current.style.height = "", u.current.style.overflow = ""));
                         var e
                     }, d.current = o
                 };
-                return (0, ge.jsx)(Sn, {
+                return (0, ge.jsx)(fr, {
                     "data-testid": "stExpander",
-                    children: (0, ge.jsxs)(qn, {
+                    children: (0, ge.jsxs)(hr, {
                         isStale: r,
                         ref: u,
-                        children: [(0, ge.jsxs)(_n, {
+                        children: [(0, ge.jsxs)(Mr, {
                             onClick: e => {
                                 e.preventDefault(), c(!l);
                                 const t = u.current;
                                 if (!t || !p.current) return;
                                 t.style.overflow = "hidden";
                                 const n = t.getBoundingClientRect().height,
                                     r = p.current.getBoundingClientRect().height;
@@ -117975,16 +118832,16 @@
                                         if (!f.current) return;
                                         const e = f.current.getBoundingClientRect().height;
                                         h(t, n, r + e + 2)
                                     }), 100)
                                 })))
                             },
                             ref: p,
-                            children: [(0, ge.jsxs)(En, {
-                                children: [n.icon && (0, ge.jsx)(Tn, {
+                            children: [(0, ge.jsxs)(mr, {
+                                children: [n.icon && (0, ge.jsx)(zr, {
                                     icon: n.icon
                                 }), (0, ge.jsx)(Yt.ZP, {
                                     source: a,
                                     allowHTML: !1,
                                     isLabel: !0
                                 })]
                             }), (0, ge.jsx)(rn.xL, {
@@ -117992,96 +118849,96 @@
                                 color: "inherit",
                                 "aria-hidden": "true",
                                 "data-testid": "stExpanderToggleIcon",
                                 size: "lg",
                                 margin: "",
                                 padding: ""
                             })]
-                        }), o ? (0, ge.jsx)(Rn, {
+                        }), o ? (0, ge.jsx)(gr, {
                             "data-testid": "stExpanderDetails",
                             ref: f,
                             children: "empty"
-                        }) : (0, ge.jsx)(xn, {
+                        }) : (0, ge.jsx)(Or, {
                             "data-testid": "stExpanderDetails",
                             ref: f,
                             children: i
                         })]
                     })
                 })
             };
-        const Cn = 100;
+        const Ar = 100;
 
-        function Wn(e, n) {
+        function vr(e, n) {
             const r = (0, t.useRef)(n),
                 o = (0, t.useMemo)((() => function(e, t) {
                     if (!t) return e;
                     let n = 0,
                         r = null;
                     return function() {
                         for (var o = arguments.length, i = new Array(o), a = 0; a < o; a++) i[a] = arguments[a];
                         const s = Date.now();
                         s - n > t ? (e(...i), n = s) : (r && clearTimeout(r), r = setTimeout((() => {
                             e(...i), n = Date.now()
                         }), Math.max(0, t - s + n)))
                     }
                 }((e => {
                     r.current(e)
-                }), Cn)), [r]),
+                }), Ar)), [r]),
                 i = (0, t.useCallback)((e => {
                     e.timeStampLow = Date.now(), o(e)
                 }), [o]);
             (0, t.useLayoutEffect)((() => e ? (e.addEventListener("scroll", i, {
                 passive: !0
             }), i({
                 target: e
             }), () => e.removeEventListener("scroll", i)) : () => {}), [i, e])
         }
 
-        function Nn(e, t) {
+        function wr(e, t) {
             const n = Math.sign(t - e),
                 r = e + Math.sqrt(Math.abs(t - e)) * n;
             return n > 0 ? Math.min(t, r) : Math.max(t, r)
         }
 
-        function Ln(e) {
+        function Sr(e) {
             const [n, r] = (0, t.useState)(e), o = (0, t.useRef)(e);
             return o.current = n, [n, r, o]
         }
-        const In = 1,
-            Pn = 34,
-            Dn = 17;
+        const qr = 1,
+            Er = 34,
+            _r = 17;
 
-        function Bn(e) {
+        function xr(e) {
             let {
                 scrollHeight: t,
                 offsetHeight: n,
                 scrollTop: r
             } = e;
-            return t - r - n < In
+            return t - r - n < qr
         }
 
-        function jn() {
+        function Rr() {
             const e = (0, t.useRef)(null),
-                [n, r, o] = Ln(!1),
-                [i, a, s] = Ln(!0),
+                [n, r, o] = Sr(!1),
+                [i, a, s] = Sr(!0),
                 l = (0, t.useRef)(0),
                 c = (0, t.useRef)(0),
                 u = (0, t.useRef)(0),
                 p = (0, t.useCallback)((() => {
                     l.current = Date.now(), s.current || r(!1), a(!1)
                 }), [l, s, a, r]),
                 d = (0, t.useCallback)((t => {
                     let {
                         timeStampLow: n
                     } = t;
                     const {
                         current: i
                     } = e, p = s.current;
                     if (n <= l.current || !i) return;
-                    const d = Bn(i),
+                    const d = xr(i),
                         {
                             offsetHeight: b,
                             scrollHeight: f
                         } = i,
                         {
                             current: h
                         } = c,
@@ -118101,42 +118958,42 @@
                         let t = 0;
                         const n = function(e, t) {
                             return e(), setInterval(e, t)
                         }((() => {
                             const {
                                 current: n
                             } = e, i = s.current;
-                            o.current && n ? Bn(n) ? t = 0 : t ? Date.now() - t > Pn && (i || (a(!0), r(!0)), t = 0) : t = Date.now() : n && n.scrollHeight <= n.offsetHeight && !o.current && r(!0)
-                        }), Dn);
+                            o.current && n ? xr(n) ? t = 0 : t ? Date.now() - t > Er && (i || (a(!0), r(!0)), t = 0) : t = Date.now() : n && n.scrollHeight <= n.offsetHeight && !o.current && r(!0)
+                        }), _r);
                         return () => clearInterval(n)
                     }
                 }), [e, n, i, s, o, r, a]), (0, t.useEffect)((() => {
                     const t = e.current;
                     if (t) {
                         const e = () => {
                             u.current = t.scrollHeight
                         };
                         return t.addEventListener("focus", e, {
                             capture: !0,
                             passive: !0
                         }), () => t.removeEventListener("focus", e)
                     }
-                }), [e]), Wn(e.current, d),
+                }), [e]), vr(e.current, d),
                 function(e, n, r) {
                     const o = (0, t.useRef)(0),
                         i = (0, t.useCallback)((function(t, r) {
                             let a = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : Date.now();
                             cancelAnimationFrame(o.current), o.current = requestAnimationFrame((() => {
                                 if (e) {
                                     const o = e.scrollHeight - e.offsetHeight;
                                     let s = function(e, t, n, r) {
                                         let o = e;
                                         for (let i = 0; i < r; i++) o = n(o, t);
                                         return o
-                                    }(t, o, Nn, (Date.now() - a) / 5);
+                                    }(t, o, wr, (Date.now() - a) / 5);
                                     Math.abs(o - s) < 1.5 && (s = o), e.scrollTop = s, o === s ? n() : i(t, r + 1, a)
                                 }
                             }))
                         }), [o, n, e]),
                         a = (0, t.useCallback)((() => {
                             cancelAnimationFrame(o.current), n()
                         }), [n]);
@@ -118147,117 +119004,117 @@
                             passive: !0
                         }), () => {
                             e.removeEventListener("pointerdown", a), e.removeEventListener("wheel", a), cancelAnimationFrame(o.current)
                         }) : () => cancelAnimationFrame(o.current)
                     }), [i, o, a, e, r])
                 }(e.current, p, i), e
         }
-        const Fn = jn;
-        var Un = __webpack_require__(19336),
-            Vn = __webpack_require__.n(Un),
-            Hn = __webpack_require__(13005),
-            Xn = __webpack_require__.n(Hn);
+        const Tr = Rr;
+        var kr = __webpack_require__(19336),
+            Cr = __webpack_require__.n(kr),
+            Wr = __webpack_require__(13005),
+            Nr = __webpack_require__.n(Wr);
 
-        function Gn(e, n, r) {
+        function Lr(e, n, r) {
             class o extends t.Component {
                 constructor() {
-                    super(...arguments), this.updateDebounced = Vn()(this.forceUpdate, n, r)
+                    super(...arguments), this.updateDebounced = Cr()(this.forceUpdate, n, r)
                 }
                 shouldComponentUpdate() {
                     return this.updateDebounced(), !1
                 }
                 componentWillUnmount() {
                     this.updateDebounced.cancel()
                 }
                 render() {
                     return t.createElement(e, Object.assign({}, this.props))
                 }
             }
-            return o.displayName = "debounceRender(".concat(e.displayName || e.name || "Component", ")"), Xn()(o, e)
+            return o.displayName = "debounceRender(".concat(e.displayName || e.name || "Component", ")"), Nr()(o, e)
         }
-        const $n = Gn;
-        var Kn = __webpack_require__(7974),
-            Yn = __webpack_require__.n(Kn),
-            Zn = __webpack_require__(62622);
-        const Jn = (0, Qe.Z)("div", {
+        const Ir = Lr;
+        var Pr = __webpack_require__(7974),
+            Dr = __webpack_require__.n(Pr),
+            Br = __webpack_require__(62622);
+        const jr = (0, Qe.Z)("div", {
                 target: "e1q9reml4"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     fontSize: t.fontSizes.md,
                     fontFamily: t.genericFonts.bodyFont,
                     padding: "".concat(t.spacing.twoXS, " ").concat(t.spacing.xs),
                     lineHeight: t.lineHeights.table,
                     overflow: ["auto", "overlay"]
                 }
             }), ""),
-            Qn = (0, Qe.Z)("table", {
+            Fr = (0, Qe.Z)("table", {
                 target: "e1q9reml3"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     width: t.sizes.full,
                     marginBottom: t.spacing.lg,
                     color: t.colors.bodyText,
                     borderCollapse: "collapse",
                     border: "1px solid ".concat(t.colors.fadedText05)
                 }
             }), ""),
-            er = e => ({
+            Ur = e => ({
                 borderBottom: "1px solid ".concat(e.colors.fadedText05),
                 borderRight: "1px solid ".concat(e.colors.fadedText05),
                 verticalAlign: "middle",
                 padding: "".concat(e.spacing.twoXS, " ").concat(e.spacing.xs),
                 fontWeight: e.fontWeights.normal
             }),
-            tr = (0, Qe.Z)("td", {
+            Vr = (0, Qe.Z)("td", {
                 target: "e1q9reml2"
             })((e => {
                 let {
                     theme: t
                 } = e;
-                return er(t)
+                return Ur(t)
             }), ""),
-            nr = (0, Qe.Z)("th", {
+            Hr = (0, Qe.Z)("th", {
                 target: "e1q9reml1"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
-                    ...er(t),
+                    ...Ur(t),
                     color: t.colors.fadedText60,
                     "@media print": {
                         "@-moz-document url-prefix()": {
                             fontWeight: "normal"
                         }
                     }
                 }
             }), ""),
-            rr = (0, Qe.Z)(tr, {
+            Xr = (0, Qe.Z)(Vr, {
                 target: "e1q9reml0"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     color: t.colors.darkGray,
                     fontStyle: "italic",
                     fontSize: t.fontSizes.md,
                     textAlign: "center"
                 }
             }), "");
 
-        function or(e, t, n) {
+        function Gr(e, t, n) {
             return (0, ge.jsx)("tr", {
-                children: Yn()(n).map((n => function(e, t, n) {
+                children: Dr()(n).map((n => function(e, t, n) {
                     var r;
                     const {
                         type: o,
                         cssId: i,
                         cssClass: a,
                         content: s,
                         contentType: l,
@@ -118266,149 +119123,149 @@
                     } = e.getCell(t, n), p = c || Ue.fu.format(s, l, u), {
                         headerColumns: d
                     } = e.dimensions, b = null === (r = e.types.data[n - d]) || void 0 === r ? void 0 : r.pandas_type, f = {
                         textAlign: "int64" === b || "float64" === b ? "right" : "left"
                     };
                     switch (o) {
                         case "blank":
-                            return (0, ge.jsx)(nr, {
+                            return (0, ge.jsx)(Hr, {
                                 className: a,
                                 children: "\xa0"
                             }, n);
                         case "index":
-                            return (0, ge.jsx)(nr, {
+                            return (0, ge.jsx)(Hr, {
                                 scope: "row",
                                 id: i,
                                 className: a,
                                 children: p
                             }, n);
                         case "columns":
-                            return (0, ge.jsx)(nr, {
+                            return (0, ge.jsx)(Hr, {
                                 scope: "col",
                                 className: a,
                                 style: f,
                                 children: p
                             }, n);
                         case "data":
-                            return (0, ge.jsx)(tr, {
+                            return (0, ge.jsx)(Vr, {
                                 id: i,
                                 style: f,
                                 children: p
                             }, n);
                         default:
                             throw new Error('Cannot parse type "'.concat(o, '".'))
                     }
                 }(e, t, n)))
             }, t)
         }
-        const ir = (0, Zn.Z)((function(e) {
+        const $r = (0, Br.Z)((function(e) {
                 const t = e.element,
                     {
                         cssId: n,
                         cssStyles: r,
                         caption: o
                     } = t,
                     {
                         headerRows: i,
                         rows: a,
                         columns: s
                     } = t.dimensions,
-                    l = Yn()(a),
+                    l = Dr()(a),
                     c = l.slice(0, i),
                     u = l.slice(i);
-                return (0, ge.jsxs)(Jn, {
+                return (0, ge.jsxs)(jr, {
                     "data-testid": "stTable",
                     children: [r && (0, ge.jsx)("style", {
                         children: r
-                    }), (0, ge.jsxs)(Qn, {
+                    }), (0, ge.jsxs)(Fr, {
                         id: n,
                         "data-testid": "stTableStyledTable",
                         children: [o && (0, ge.jsx)("caption", {
                             children: (0, ge.jsx)("small", {
                                 children: o
                             })
                         }), c.length > 0 && (0, ge.jsx)("thead", {
-                            children: c.map((e => or(t, e, s)))
+                            children: c.map((e => Gr(t, e, s)))
                         }), (0, ge.jsx)("tbody", {
                             children: 0 === u.length ? (0, ge.jsx)("tr", {
-                                children: (0, ge.jsx)(rr, {
+                                children: (0, ge.jsx)(Xr, {
                                     "data-testid": "stTableStyledEmptyTableCell",
                                     colSpan: s || 1,
                                     children: "empty"
                                 })
-                            }) : u.map((e => or(t, e, s)))
+                            }) : u.map((e => Gr(t, e, s)))
                         })]
                     })]
                 })
             })),
-            ar = (0, Qe.Z)("span", {
+            Kr = (0, Qe.Z)("span", {
                 target: "ejycmjn10"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     "& > *": {
                         marginRight: t.spacing.sm
                     }
                 }
             }), ""),
-            sr = (0, Qe.Z)("span", {
+            Yr = (0, Qe.Z)("span", {
                 target: "ejycmjn9"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     fontWeight: t.fontWeights.bold
                 }
             }), ""),
-            lr = (0, Qe.Z)("span", {
+            Zr = (0, Qe.Z)("span", {
                 target: "ejycmjn8"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     color: t.colors.green70
                 }
             }), ""),
-            cr = (0, Qe.Z)("span", {
+            Jr = (0, Qe.Z)("span", {
                 target: "ejycmjn7"
             })(""),
-            ur = (0, Qe.Z)("span", {
+            Qr = (0, Qe.Z)("span", {
                 target: "ejycmjn6"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     display: "flex",
                     flexDirection: "column",
                     borderRadius: t.radii.lg,
                     border: "1px solid ".concat(t.colors.fadedText05),
                     fontFamily: t.genericFonts.codeFont,
                     fontSize: t.fontSizes.sm
                 }
             }), ""),
-            pr = (0, Qe.Z)("div", {
+            eo = (0, Qe.Z)("div", {
                 target: "ejycmjn5"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     padding: "".concat(t.spacing.sm, " ").concat(t.spacing.lg),
                     backgroundColor: t.colors.docStringContainerBackground,
                     borderBottom: "1px solid ".concat(t.colors.fadedText05),
                     fontSize: t.fontSizes.sm,
                     overflow: ["auto", "overlay"]
                 }
             }), ""),
-            dr = (0, Qe.Z)("div", {
+            to = (0, Qe.Z)("div", {
                 target: "ejycmjn4"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     whiteSpace: "pre",
@@ -118417,175 +119274,175 @@
                     padding: "".concat(t.spacing.sm, " ").concat(t.spacing.lg),
                     fontSize: t.fontSizes.sm,
                     "&:not(:last-child)": {
                         borderBottom: "1px solid ".concat(t.colors.fadedText05)
                     }
                 }
             }), ""),
-            br = (0, Qe.Z)("table", {
+            no = (0, Qe.Z)("table", {
                 target: "ejycmjn3"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     width: "100%",
                     fontSize: t.fontSizes.twoSm,
                     backgroundColor: t.colors.docStringContainerBackground,
                     tableLayout: "fixed",
                     borderCollapse: "collapse"
                 }
             }), ""),
-            fr = (0, Qe.Z)("tr", {
+            ro = (0, Qe.Z)("tr", {
                 target: "ejycmjn2"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     "&:not(:last-child)": {
                         borderBottom: "1px dotted ".concat(t.colors.fadedText05)
                     }
                 }
             }), ""),
-            hr = (0, Qe.Z)("td", {
+            oo = (0, Qe.Z)("td", {
                 target: "ejycmjn1"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     width: "30%",
                     overflow: ["auto", "overlay"],
                     padding: "".concat(t.spacing.sm, " ").concat(t.spacing.lg),
                     "& > *": {
                         marginRight: t.spacing.sm
                     }
                 }
             }), ""),
-            mr = (0, Qe.Z)("td", {
+            io = (0, Qe.Z)("td", {
                 target: "ejycmjn0"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     width: "70%",
                     overflow: ["auto", "overlay"],
                     padding: "".concat(t.spacing.sm, " ").concat(t.spacing.lg)
                 }
             }), "");
 
-        function Mr(e) {
+        function ao(e) {
             let {
                 width: t,
                 element: n
             } = e;
             const {
                 name: r,
                 type: o,
                 value: i,
                 docString: a,
                 members: s
             } = n;
-            return (0, ge.jsxs)(ur, {
+            return (0, ge.jsxs)(Qr, {
                 width: t,
                 "data-testid": "stDocstring",
-                children: [(0, ge.jsx)(pr, {
-                    children: (0, ge.jsxs)(ar, {
-                        children: [r ? (0, ge.jsx)(sr, {
+                children: [(0, ge.jsx)(eo, {
+                    children: (0, ge.jsxs)(Kr, {
+                        children: [r ? (0, ge.jsx)(Yr, {
                             "data-testid": "stDocstringName",
                             children: r
-                        }) : null, o ? (0, ge.jsx)(lr, {
+                        }) : null, o ? (0, ge.jsx)(Zr, {
                             "data-testid": "stDocstringType",
                             children: o
-                        }) : null, i ? (0, ge.jsx)(cr, {
+                        }) : null, i ? (0, ge.jsx)(Jr, {
                             "data-testid": "stDocstringValue",
                             children: i
                         }) : null]
                     })
-                }), (0, ge.jsx)(dr, {
+                }), (0, ge.jsx)(to, {
                     "data-testid": "stDocstring-Doc",
                     children: a || "No docs available"
-                }), s.length > 0 ? (0, ge.jsx)(br, {
+                }), s.length > 0 ? (0, ge.jsx)(no, {
                     "data-testid": "stDocstringMembersTable",
-                    children: s.map((e => (0, ge.jsx)(Or, {
+                    children: s.map((e => (0, ge.jsx)(so, {
                         member: e
                     }, e.name)))
                 }) : null]
             })
         }
 
-        function Or(e) {
+        function so(e) {
             let {
                 member: t
             } = e;
             const {
                 name: n,
                 type: r,
                 value: o,
                 docString: i
             } = t;
-            return (0, ge.jsxs)(fr, {
+            return (0, ge.jsxs)(ro, {
                 "data-testid": "stMember",
-                children: [(0, ge.jsxs)(hr, {
-                    children: [n ? (0, ge.jsx)(sr, {
+                children: [(0, ge.jsxs)(oo, {
+                    children: [n ? (0, ge.jsx)(Yr, {
                         "data-testid": "stMemberDocName",
                         children: n
-                    }) : null, r ? (0, ge.jsx)(lr, {
+                    }) : null, r ? (0, ge.jsx)(Zr, {
                         "data-testid": "stMemberDocType",
                         children: r
                     }) : null]
-                }), (0, ge.jsx)(mr, {
-                    children: o ? (0, ge.jsx)(cr, {
+                }), (0, ge.jsx)(io, {
+                    children: o ? (0, ge.jsx)(Jr, {
                         "data-testid": "stMemberDocValue",
                         children: o
-                    }) : (0, ge.jsx)(cr, {
+                    }) : (0, ge.jsx)(Jr, {
                         "data-testid": "stMemberDocString",
                         children: i || "No docs available"
                     })
                 })]
             })
         }
-        var gr = __webpack_require__(95899);
-        const zr = (0, Qe.Z)("div", {
+        var lo = __webpack_require__(95899);
+        const co = (0, Qe.Z)("div", {
                 target: "e1dl0tyv3"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     marginTop: t.spacing.sm,
                     "&:first-of-type": {
                         marginTop: 0
                     }
                 }
             }), ""),
-            yr = (0, Qe.Z)("span", {
+            uo = (0, Qe.Z)("span", {
                 target: "e1dl0tyv2"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     fontWeight: t.fontWeights.bold
                 }
             }), ""),
-            Ar = (0, Qe.Z)("div", {
+            po = (0, Qe.Z)("div", {
                 target: "e1dl0tyv1"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     marginTop: "calc(".concat(t.spacing.sm, " + ").concat(t.spacing.xl, ")"),
                     marginBottom: t.spacing.sm
                 }
             }), ""),
-            vr = (0, Qe.Z)("pre", {
+            bo = (0, Qe.Z)("pre", {
                 target: "e1dl0tyv0"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     whiteSpace: "pre-wrap",
@@ -118595,111 +119452,111 @@
                     backgroundColor: t.colors.transparent,
                     code: {
                         color: "inherit"
                     }
                 }
             }), "");
 
-        function wr(e) {
+        function fo(e) {
             let {
                 type: t,
                 message: n,
                 messageIsMarkdown: r
             } = e;
             if (r) {
                 let e = "**".concat(t, "**");
                 return n && (e += ": ".concat(n)), (0, ge.jsx)(Yt.ZP, {
                     source: e,
                     allowHTML: !1
                 })
             }
             return (0, ge.jsxs)(ge.Fragment, {
-                children: [(0, ge.jsx)(yr, {
+                children: [(0, ge.jsx)(uo, {
                     children: t
                 }), (o = n, null != o && "" !== o ? ": ".concat(n) : null)]
             });
             var o
         }
 
-        function Sr(e) {
+        function ho(e) {
             let {
                 stackTrace: t
             } = e;
             return (0, ge.jsxs)(ge.Fragment, {
-                children: [(0, ge.jsx)(Ar, {
+                children: [(0, ge.jsx)(po, {
                     children: "Traceback:"
-                }), (0, ge.jsx)(vr, {
+                }), (0, ge.jsx)(bo, {
                     children: (0, ge.jsx)("code", {
-                        children: t.map(((e, t) => (0, ge.jsx)(zr, {
+                        children: t.map(((e, t) => (0, ge.jsx)(co, {
                             "data-testid": "stExceptionTraceRow",
                             children: e
                         }, t)))
                     })
                 })]
             })
         }
 
-        function qr(e) {
+        function mo(e) {
             let {
                 element: t,
                 width: n
             } = e;
             return (0, ge.jsx)("div", {
                 className: "stException",
                 "data-testid": "stException",
                 children: (0, ge.jsxs)(Ze.Z, {
                     kind: t.isWarning ? Ze.h.WARNING : Ze.h.ERROR,
                     width: n,
                     children: [(0, ge.jsx)("div", {
                         className: "message",
-                        children: (0, ge.jsx)(wr, {
+                        children: (0, ge.jsx)(fo, {
                             type: t.type,
                             message: t.message,
                             messageIsMarkdown: t.messageIsMarkdown
                         })
-                    }), t.stackTrace && t.stackTrace.length > 0 ? (0, ge.jsx)(Sr, {
+                    }), t.stackTrace && t.stackTrace.length > 0 ? (0, ge.jsx)(ho, {
                         stackTrace: t.stackTrace
                     }) : null]
                 })
             })
         }
-        var Er = __webpack_require__(97365),
-            _r = __webpack_require__(34838),
-            xr = __webpack_require__.n(_r),
-            Rr = __webpack_require__(82309);
+        var Mo = __webpack_require__(97365),
+            Oo = __webpack_require__(34838),
+            go = __webpack_require__.n(Oo),
+            zo = __webpack_require__(82309);
 
-        function Tr(e) {
+        function yo(e) {
             let {
                 width: t,
                 element: n
             } = e;
             const r = {
                     width: t
                 },
                 o = (0, Ee.u)();
             let i;
             try {
                 i = JSON.parse(n.body)
             } catch (s) {
                 const e = (0, Ve.b)(s);
                 try {
-                    i = Er.Z.parse(n.body)
+                    i = Mo.Z.parse(n.body)
                 } catch (l) {
                     const t = parseInt(e.message.replace(/[^0-9]/g, ""), 10);
-                    return e.message += "\n".concat(n.body.substr(0, t + 1), " \u2190 here"), (0, ge.jsx)(Rr.Z, {
+                    return e.message += "\n".concat(n.body.substr(0, t + 1), " \u2190 here"), (0, ge.jsx)(zo.Z, {
                         name: "Json Parse Error",
                         message: e.message
                     })
                 }
             }
             const a = (0, ye.Iy)(o) ? "rjv-default" : "monokai";
             return (0, ge.jsx)("div", {
                 "data-testid": "stJson",
                 style: r,
-                children: (0, ge.jsx)(xr(), {
+                children: (0, ge.jsx)(go(), {
                     src: i,
                     collapsed: !n.expanded,
                     displayDataTypes: !1,
                     displayObjectSize: !1,
                     name: !1,
                     theme: a,
                     style: {
@@ -118707,46 +119564,46 @@
                         fontSize: o.fontSizes.sm,
                         backgroundColor: o.colors.bgColor,
                         whiteSpace: "pre-wrap"
                     }
                 })
             })
         }
-        var kr = __webpack_require__(19660),
-            Cr = __webpack_require__(8879);
+        var Ao = __webpack_require__(19660),
+            vo = __webpack_require__(8879);
 
-        function Wr(e) {
+        function wo(e) {
             let {
                 width: t,
                 element: n
             } = e;
             const r = {
                 width: t
             };
             return (0, ge.jsx)("div", {
                 className: "stMarkdown",
                 style: r,
                 "data-testid": "stMarkdown",
-                children: n.help ? (0, ge.jsxs)(kr.KH, {
+                children: n.help ? (0, ge.jsxs)(Ao.KH, {
                     children: [(0, ge.jsx)(Yt.ZP, {
                         isCaption: n.isCaption,
                         source: n.body,
                         allowHTML: n.allowHtml
-                    }), (0, ge.jsx)(Cr.w, {
+                    }), (0, ge.jsx)(vo.w, {
                         content: n.help,
                         isLatex: n.elementType === Be.UG.Type.LATEX
                     })]
                 }) : (0, ge.jsx)(Yt.ZP, {
                     isCaption: n.isCaption,
                     source: n.body,
                     allowHTML: n.allowHtml
                 })
             })
         }
-        var Nr = t.forwardRef((function(e, n) {
+        var So = t.forwardRef((function(e, n) {
             return t.createElement(en.D, (0, Qt.Z)({
                 iconAttrs: {
                     fill: "currentColor",
                     xmlns: "http://www.w3.org/2000/svg"
                 },
                 iconVerticalAlign: "middle",
                 iconViewBox: "0 0 24 24"
@@ -118755,16 +119612,16 @@
             }), t.createElement("path", {
                 fill: "none",
                 d: "M0 0h24v24H0V0z"
             }), t.createElement("path", {
                 d: "M20 12l-1.41-1.41L13 16.17V4h-2v12.17l-5.58-5.59L4 12l8 8 8-8z"
             }))
         }));
-        Nr.displayName = "ArrowDownward";
-        var Lr = t.forwardRef((function(e, n) {
+        So.displayName = "ArrowDownward";
+        var qo = t.forwardRef((function(e, n) {
             return t.createElement(en.D, (0, Qt.Z)({
                 iconAttrs: {
                     fill: "currentColor",
                     xmlns: "http://www.w3.org/2000/svg"
                 },
                 iconVerticalAlign: "middle",
                 iconViewBox: "0 0 24 24"
@@ -118773,18 +119630,18 @@
             }), t.createElement("path", {
                 fill: "none",
                 d: "M0 0h24v24H0V0z"
             }), t.createElement("path", {
                 d: "M4 12l1.41 1.41L11 7.83V20h2V7.83l5.58 5.59L20 12l-8-8-8 8z"
             }))
         }));
-        Lr.displayName = "ArrowUpward";
-        var Ir = __webpack_require__(86659),
-            Pr = __webpack_require__(68411);
-        const Dr = (0, Qe.Z)("div", {
+        qo.displayName = "ArrowUpward";
+        var Eo = __webpack_require__(86659),
+            _o = __webpack_require__(68411);
+        const xo = (0, Qe.Z)("div", {
                 target: "e1i5pmia3"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     overflowWrap: "normal",
@@ -118800,55 +119657,55 @@
                         "& > p": {
                             textOverflow: "ellipsis",
                             overflow: "hidden"
                         }
                     }
                 }
             }), ""),
-            Br = (0, Qe.Z)(Ir.y8, {
+            Ro = (0, Qe.Z)(Eo.y8, {
                 target: "e1i5pmia2"
             })((e => {
                 let {
                     visibility: t
                 } = e;
                 return {
                     marginBottom: 0,
                     display: t === He.Ws.Collapsed ? "none" : "grid",
                     gridTemplateColumns: t === He.Ws.Collapsed ? "initial" : "auto 1fr",
                     visibility: t === He.Ws.Hidden ? "hidden" : "visible"
                 }
             }), ""),
-            jr = (0, Qe.Z)("div", {
+            To = (0, Qe.Z)("div", {
                 target: "e1i5pmia1"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     fontSize: t.fontSizes.threeXL,
                     color: t.colors.textColor,
                     paddingBottom: t.spacing.twoXS
                 }
             }), ""),
-            Fr = (0, Qe.Z)("div", {
+            ko = (0, Qe.Z)("div", {
                 target: "e1i5pmia0"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     fontSize: t.fontSizes.md,
                     display: "flex",
                     flexDirection: "row",
                     alignItems: "center",
                     fontWeight: t.fontWeights.normal
                 }
             }), "");
 
-        function Ur(e) {
+        function Co(e) {
             var t;
             let {
                 element: n
             } = e;
             const {
                 colors: r
             } = (0, Ee.u)(), {
@@ -118865,236 +119722,236 @@
                     s = r.green;
                     break;
                 default:
                     s = r.fadedText60
             }
             switch (n.direction) {
                 case i.DOWN:
-                    a = Nr;
+                    a = So;
                     break;
                 case i.UP:
-                    a = Lr;
+                    a = qo;
                     break;
                 default:
                     a = null
             }
             const l = {
                     color: s
                 },
                 c = "" !== n.delta;
             return (0, ge.jsxs)("div", {
                 "data-testid": "stMetric",
-                children: [(0, ge.jsxs)(Br, {
+                children: [(0, ge.jsxs)(Ro, {
                     "data-testid": "stMetricLabel",
                     visibility: (0, He.iF)(null === (t = n.labelVisibility) || void 0 === t ? void 0 : t.value),
-                    children: [(0, ge.jsx)(Dr, {
+                    children: [(0, ge.jsx)(xo, {
                         children: (0, ge.jsx)(Yt.ZP, {
                             source: n.label,
                             allowHTML: !1,
                             isLabel: !0
                         })
-                    }), n.help && (0, ge.jsx)(Ir.Hp, {
-                        children: (0, ge.jsx)(Cr.Z, {
+                    }), n.help && (0, ge.jsx)(Eo.Hp, {
+                        children: (0, ge.jsx)(vo.Z, {
                             content: n.help,
-                            placement: Pr.u.TOP_RIGHT
+                            placement: _o.u.TOP_RIGHT
                         })
                     })]
-                }), (0, ge.jsx)(jr, {
+                }), (0, ge.jsx)(To, {
                     "data-testid": "stMetricValue",
-                    children: (0, ge.jsxs)(Dr, {
+                    children: (0, ge.jsxs)(xo, {
                         children: [" ", n.body, " "]
                     })
-                }), c && (0, ge.jsxs)(Fr, {
+                }), c && (0, ge.jsxs)(ko, {
                     "data-testid": "stMetricDelta",
                     style: l,
                     children: [(0, ge.jsx)(hn.Z, {
-                        testid: a === Lr ? "stMetricDeltaIcon-Up" : "stMetricDeltaIcon-Down",
+                        testid: a === qo ? "stMetricDeltaIcon-Up" : "stMetricDeltaIcon-Down",
                         content: a,
                         size: "lg",
                         margin: "0 threeXS 0 0"
-                    }), (0, ge.jsxs)(Dr, {
+                    }), (0, ge.jsxs)(xo, {
                         children: [" ", n.delta, " "]
                     })]
                 })]
             })
         }
-        var Vr = __webpack_require__(87786);
-        const Hr = () => {
+        var Wo = __webpack_require__(87786);
+        const No = () => {
                 const [e, n] = (0, t.useState)(!1);
                 return (0, t.useEffect)((() => {
                     const e = setTimeout((() => {
                         n(!0)
                     }), 500);
                     return () => {
                         clearTimeout(e)
                     }
-                }), []), e ? (0, ge.jsxs)(Vr.ps, {
+                }), []), e ? (0, ge.jsxs)(Wo.ps, {
                     "data-testid": "stAppSkeleton",
-                    children: [(0, ge.jsx)(Vr.Li, {}), (0, ge.jsxs)(Vr.AU, {
-                        children: [(0, ge.jsx)(Vr.HH, {
+                    children: [(0, ge.jsx)(Wo.Li, {}), (0, ge.jsxs)(Wo.AU, {
+                        children: [(0, ge.jsx)(Wo.HH, {
                             width: "98%"
-                        }), (0, ge.jsx)(Vr.HH, {
+                        }), (0, ge.jsx)(Wo.HH, {
                             width: "100%"
-                        }), (0, ge.jsx)(Vr.HH, {
+                        }), (0, ge.jsx)(Wo.HH, {
                             width: "96%"
-                        }), (0, ge.jsx)(Vr.HH, {
+                        }), (0, ge.jsx)(Wo.HH, {
                             width: "65%"
                         })]
-                    }), (0, ge.jsx)(Vr.a3, {
+                    }), (0, ge.jsx)(Wo.a3, {
                         width: "75%",
                         height: "9rem"
                     })]
                 }) : (0, ge.jsx)(ge.Fragment, {})
             },
-            Xr = (0, t.memo)(Hr);
-        var Gr = __webpack_require__(55140);
-        const $r = (0, Qe.Z)("div", {
+            Lo = (0, t.memo)(No);
+        var Io = __webpack_require__(55140);
+        const Po = (0, Qe.Z)("div", {
             target: "exotz4b0"
         })((e => {
             let {
                 theme: t
             } = e;
             return {
                 fontFamily: t.genericFonts.codeFont,
                 whiteSpace: "pre",
                 fontSize: t.fontSizes.sm,
                 overflowX: "auto"
             }
         }), "");
 
-        function Kr(e) {
+        function Do(e) {
             let {
                 width: t,
                 element: n
             } = e;
             const r = {
                 width: t
             };
-            return (0, ge.jsxs)(kr.KH, {
+            return (0, ge.jsxs)(Ao.KH, {
                 style: r,
                 className: "stTextLabelWrapper",
-                children: [(0, ge.jsx)($r, {
+                children: [(0, ge.jsx)(Po, {
                     "data-testid": "stText",
                     children: n.body
-                }), n.help && (0, ge.jsx)(Cr.w, {
+                }), n.help && (0, ge.jsx)(vo.w, {
                     content: n.help
                 })]
             })
         }
-        const Yr = "%[a-f0-9]{2}",
-            Zr = new RegExp("(" + Yr + ")|([^%]+?)", "gi"),
-            Jr = new RegExp("(" + Yr + ")+", "gi");
+        const Bo = "%[a-f0-9]{2}",
+            jo = new RegExp("(" + Bo + ")|([^%]+?)", "gi"),
+            Fo = new RegExp("(" + Bo + ")+", "gi");
 
-        function Qr(e, t) {
+        function Uo(e, t) {
             try {
                 return [decodeURIComponent(e.join(""))]
             } catch {}
             if (1 === e.length) return e;
             t = t || 1;
             const n = e.slice(0, t),
                 r = e.slice(t);
-            return Array.prototype.concat.call([], Qr(n), Qr(r))
+            return Array.prototype.concat.call([], Uo(n), Uo(r))
         }
 
-        function eo(e) {
+        function Vo(e) {
             try {
                 return decodeURIComponent(e)
             } catch {
-                let t = e.match(Zr) || [];
-                for (let n = 1; n < t.length; n++) t = (e = Qr(t, n).join("")).match(Zr) || [];
+                let t = e.match(jo) || [];
+                for (let n = 1; n < t.length; n++) t = (e = Uo(t, n).join("")).match(jo) || [];
                 return e
             }
         }
 
-        function to(e) {
+        function Ho(e) {
             if ("string" !== typeof e) throw new TypeError("Expected `encodedURI` to be of type `string`, got `" + typeof e + "`");
             try {
                 return decodeURIComponent(e)
             } catch {
                 return function(e) {
                     const t = {
                         "%FE%FF": "\ufffd\ufffd",
                         "%FF%FE": "\ufffd\ufffd"
                     };
-                    let n = Jr.exec(e);
+                    let n = Fo.exec(e);
                     for (; n;) {
                         try {
                             t[n[0]] = decodeURIComponent(n[0])
                         } catch {
-                            const e = eo(n[0]);
+                            const e = Vo(n[0]);
                             e !== n[0] && (t[n[0]] = e)
                         }
-                        n = Jr.exec(e)
+                        n = Fo.exec(e)
                     }
                     t["%C2"] = "\ufffd";
                     const r = Object.keys(t);
                     for (const o of r) e = e.replace(new RegExp(o, "g"), t[o]);
                     return e
                 }(e)
             }
         }
 
-        function no(e, t) {
+        function Xo(e, t) {
             if ("string" !== typeof e || "string" !== typeof t) throw new TypeError("Expected the arguments to be of type `string`");
             if ("" === e || "" === t) return [];
             const n = e.indexOf(t);
             return -1 === n ? [] : [e.slice(0, n), e.slice(n + t.length)]
         }
 
-        function ro(e, t) {
+        function Go(e, t) {
             const n = {};
             if (Array.isArray(t))
                 for (const r of t) {
                     const t = Object.getOwnPropertyDescriptor(e, r);
                     null !== t && void 0 !== t && t.enumerable && Object.defineProperty(n, r, t)
                 } else
                     for (const r of Reflect.ownKeys(e)) {
                         const o = Object.getOwnPropertyDescriptor(e, r);
                         if (o.enumerable) {
                             t(r, e[r], e) && Object.defineProperty(n, r, o)
                         }
                     }
             return n
         }
-        const oo = e => null === e || void 0 === e,
-            io = e => encodeURIComponent(e).replace(/[!'()*]/g, (e => "%".concat(e.charCodeAt(0).toString(16).toUpperCase()))),
-            ao = Symbol("encodeFragmentIdentifier");
+        const $o = e => null === e || void 0 === e,
+            Ko = e => encodeURIComponent(e).replace(/[!'()*]/g, (e => "%".concat(e.charCodeAt(0).toString(16).toUpperCase()))),
+            Yo = Symbol("encodeFragmentIdentifier");
 
-        function so(e) {
+        function Zo(e) {
             if ("string" !== typeof e || 1 !== e.length) throw new TypeError("arrayFormatSeparator must be single character string")
         }
 
-        function lo(e, t) {
-            return t.encode ? t.strict ? io(e) : encodeURIComponent(e) : e
+        function Jo(e, t) {
+            return t.encode ? t.strict ? Ko(e) : encodeURIComponent(e) : e
         }
 
-        function co(e, t) {
-            return t.decode ? to(e) : e
+        function Qo(e, t) {
+            return t.decode ? Ho(e) : e
         }
 
-        function uo(e) {
-            return Array.isArray(e) ? e.sort() : "object" === typeof e ? uo(Object.keys(e)).sort(((e, t) => Number(e) - Number(t))).map((t => e[t])) : e
+        function ei(e) {
+            return Array.isArray(e) ? e.sort() : "object" === typeof e ? ei(Object.keys(e)).sort(((e, t) => Number(e) - Number(t))).map((t => e[t])) : e
         }
 
-        function po(e) {
+        function ti(e) {
             const t = e.indexOf("#");
             return -1 !== t && (e = e.slice(0, t)), e
         }
 
-        function bo(e, t) {
+        function ni(e, t) {
             return t.parseNumbers && !Number.isNaN(Number(e)) && "string" === typeof e && "" !== e.trim() ? e = Number(e) : !t.parseBooleans || null === e || "true" !== e.toLowerCase() && "false" !== e.toLowerCase() || (e = "true" === e.toLowerCase()), e
         }
 
-        function fo(e) {
-            const t = (e = po(e)).indexOf("?");
+        function ri(e) {
+            const t = (e = ti(e)).indexOf("?");
             return -1 === t ? "" : e.slice(t + 1)
         }
 
-        function ho(e, t) {
-            so((t = {
+        function oi(e, t) {
+            Zo((t = {
                 decode: !0,
                 sort: !0,
                 arrayFormat: "none",
                 arrayFormatSeparator: ",",
                 parseNumbers: !1,
                 parseBooleans: !1,
                 ...t
@@ -119114,262 +119971,262 @@
                             return (e, n, r) => {
                                 t = /(:list)$/.exec(e), e = e.replace(/:list$/, ""), t ? void 0 !== r[e] ? r[e] = [...r[e], n] : r[e] = [n] : r[e] = n
                             };
                         case "comma":
                         case "separator":
                             return (t, n, r) => {
                                 const o = "string" === typeof n && n.includes(e.arrayFormatSeparator),
-                                    i = "string" === typeof n && !o && co(n, e).includes(e.arrayFormatSeparator);
-                                n = i ? co(n, e) : n;
-                                const a = o || i ? n.split(e.arrayFormatSeparator).map((t => co(t, e))) : null === n ? n : co(n, e);
+                                    i = "string" === typeof n && !o && Qo(n, e).includes(e.arrayFormatSeparator);
+                                n = i ? Qo(n, e) : n;
+                                const a = o || i ? n.split(e.arrayFormatSeparator).map((t => Qo(t, e))) : null === n ? n : Qo(n, e);
                                 r[t] = a
                             };
                         case "bracket-separator":
                             return (t, n, r) => {
                                 const o = /(\[])$/.test(t);
-                                if (t = t.replace(/\[]$/, ""), !o) return void(r[t] = n ? co(n, e) : n);
-                                const i = null === n ? [] : n.split(e.arrayFormatSeparator).map((t => co(t, e)));
+                                if (t = t.replace(/\[]$/, ""), !o) return void(r[t] = n ? Qo(n, e) : n);
+                                const i = null === n ? [] : n.split(e.arrayFormatSeparator).map((t => Qo(t, e)));
                                 void 0 !== r[t] ? r[t] = [...r[t], ...i] : r[t] = i
                             };
                         default:
                             return (e, t, n) => {
                                 void 0 !== n[e] ? n[e] = [...[n[e]].flat(), t] : n[e] = t
                             }
                     }
                 }(t),
                 r = Object.create(null);
             if ("string" !== typeof e) return r;
             if (!(e = e.trim().replace(/^[?#&]/, ""))) return r;
             for (const o of e.split("&")) {
                 if ("" === o) continue;
                 const e = t.decode ? o.replace(/\+/g, " ") : o;
-                let [i, a] = no(e, "=");
-                void 0 === i && (i = e), a = void 0 === a ? null : ["comma", "separator", "bracket-separator"].includes(t.arrayFormat) ? a : co(a, t), n(co(i, t), a, r)
+                let [i, a] = Xo(e, "=");
+                void 0 === i && (i = e), a = void 0 === a ? null : ["comma", "separator", "bracket-separator"].includes(t.arrayFormat) ? a : Qo(a, t), n(Qo(i, t), a, r)
             }
             for (const [o, i] of Object.entries(r))
                 if ("object" === typeof i && null !== i)
-                    for (const [e, n] of Object.entries(i)) i[e] = bo(n, t);
-                else r[o] = bo(i, t);
+                    for (const [e, n] of Object.entries(i)) i[e] = ni(n, t);
+                else r[o] = ni(i, t);
             return !1 === t.sort ? r : (!0 === t.sort ? Object.keys(r).sort() : Object.keys(r).sort(t.sort)).reduce(((e, t) => {
                 const n = r[t];
-                return Boolean(n) && "object" === typeof n && !Array.isArray(n) ? e[t] = uo(n) : e[t] = n, e
+                return Boolean(n) && "object" === typeof n && !Array.isArray(n) ? e[t] = ei(n) : e[t] = n, e
             }), Object.create(null))
         }
 
-        function mo(e, t) {
+        function ii(e, t) {
             if (!e) return "";
-            so((t = {
+            Zo((t = {
                 encode: !0,
                 strict: !0,
                 arrayFormat: "none",
                 arrayFormatSeparator: ",",
                 ...t
             }).arrayFormatSeparator);
-            const n = n => t.skipNull && oo(e[n]) || t.skipEmptyString && "" === e[n],
+            const n = n => t.skipNull && $o(e[n]) || t.skipEmptyString && "" === e[n],
                 r = function(e) {
                     switch (e.arrayFormat) {
                         case "index":
                             return t => (n, r) => {
                                 const o = n.length;
-                                return void 0 === r || e.skipNull && null === r || e.skipEmptyString && "" === r ? n : null === r ? [...n, [lo(t, e), "[", o, "]"].join("")] : [...n, [lo(t, e), "[", lo(o, e), "]=", lo(r, e)].join("")]
+                                return void 0 === r || e.skipNull && null === r || e.skipEmptyString && "" === r ? n : null === r ? [...n, [Jo(t, e), "[", o, "]"].join("")] : [...n, [Jo(t, e), "[", Jo(o, e), "]=", Jo(r, e)].join("")]
                             };
                         case "bracket":
-                            return t => (n, r) => void 0 === r || e.skipNull && null === r || e.skipEmptyString && "" === r ? n : null === r ? [...n, [lo(t, e), "[]"].join("")] : [...n, [lo(t, e), "[]=", lo(r, e)].join("")];
+                            return t => (n, r) => void 0 === r || e.skipNull && null === r || e.skipEmptyString && "" === r ? n : null === r ? [...n, [Jo(t, e), "[]"].join("")] : [...n, [Jo(t, e), "[]=", Jo(r, e)].join("")];
                         case "colon-list-separator":
-                            return t => (n, r) => void 0 === r || e.skipNull && null === r || e.skipEmptyString && "" === r ? n : null === r ? [...n, [lo(t, e), ":list="].join("")] : [...n, [lo(t, e), ":list=", lo(r, e)].join("")];
+                            return t => (n, r) => void 0 === r || e.skipNull && null === r || e.skipEmptyString && "" === r ? n : null === r ? [...n, [Jo(t, e), ":list="].join("")] : [...n, [Jo(t, e), ":list=", Jo(r, e)].join("")];
                         case "comma":
                         case "separator":
                         case "bracket-separator": {
                             const t = "bracket-separator" === e.arrayFormat ? "[]=" : "=";
                             return n => (r, o) => void 0 === o || e.skipNull && null === o || e.skipEmptyString && "" === o ? r : (o = null === o ? "" : o, 0 === r.length ? [
-                                [lo(n, e), t, lo(o, e)].join("")
+                                [Jo(n, e), t, Jo(o, e)].join("")
                             ] : [
-                                [r, lo(o, e)].join(e.arrayFormatSeparator)
+                                [r, Jo(o, e)].join(e.arrayFormatSeparator)
                             ])
                         }
                         default:
-                            return t => (n, r) => void 0 === r || e.skipNull && null === r || e.skipEmptyString && "" === r ? n : null === r ? [...n, lo(t, e)] : [...n, [lo(t, e), "=", lo(r, e)].join("")]
+                            return t => (n, r) => void 0 === r || e.skipNull && null === r || e.skipEmptyString && "" === r ? n : null === r ? [...n, Jo(t, e)] : [...n, [Jo(t, e), "=", Jo(r, e)].join("")]
                     }
                 }(t),
                 o = {};
             for (const [a, s] of Object.entries(e)) n(a) || (o[a] = s);
             const i = Object.keys(o);
             return !1 !== t.sort && i.sort(t.sort), i.map((n => {
                 const o = e[n];
-                return void 0 === o ? "" : null === o ? lo(n, t) : Array.isArray(o) ? 0 === o.length && "bracket-separator" === t.arrayFormat ? lo(n, t) + "[]" : o.reduce(r(n), []).join("&") : lo(n, t) + "=" + lo(o, t)
+                return void 0 === o ? "" : null === o ? Jo(n, t) : Array.isArray(o) ? 0 === o.length && "bracket-separator" === t.arrayFormat ? Jo(n, t) + "[]" : o.reduce(r(n), []).join("&") : Jo(n, t) + "=" + Jo(o, t)
             })).filter((e => e.length > 0)).join("&")
         }
 
-        function Mo(e, t) {
+        function ai(e, t) {
             var n, r, o;
             t = {
                 decode: !0,
                 ...t
             };
-            let [i, a] = no(e, "#");
+            let [i, a] = Xo(e, "#");
             return void 0 === i && (i = e), {
                 url: null !== (n = null === (r = i) || void 0 === r || null === (o = r.split("?")) || void 0 === o ? void 0 : o[0]) && void 0 !== n ? n : "",
-                query: ho(fo(e), t),
+                query: oi(ri(e), t),
                 ...t && t.parseFragmentIdentifier && a ? {
-                    fragmentIdentifier: co(a, t)
+                    fragmentIdentifier: Qo(a, t)
                 } : {}
             }
         }
 
-        function Oo(e, t) {
+        function si(e, t) {
             t = {
                 encode: !0,
                 strict: !0,
-                [ao]: !0,
+                [Yo]: !0,
                 ...t
             };
-            const n = po(e.url).split("?")[0] || "";
-            let r = mo({
-                ...ho(fo(e.url), {
+            const n = ti(e.url).split("?")[0] || "";
+            let r = ii({
+                ...oi(ri(e.url), {
                     sort: !1
                 }),
                 ...e.query
             }, t);
             r && (r = "?".concat(r));
             let o = function(e) {
                 let t = "";
                 const n = e.indexOf("#");
                 return -1 !== n && (t = e.slice(n)), t
             }(e.url);
             if (e.fragmentIdentifier) {
                 const r = new URL(n);
-                r.hash = e.fragmentIdentifier, o = t[ao] ? r.hash : "#".concat(e.fragmentIdentifier)
+                r.hash = e.fragmentIdentifier, o = t[Yo] ? r.hash : "#".concat(e.fragmentIdentifier)
             }
             return "".concat(n).concat(r).concat(o)
         }
 
-        function go(e, t, n) {
+        function li(e, t, n) {
             n = {
                 parseFragmentIdentifier: !0,
-                [ao]: !1,
+                [Yo]: !1,
                 ...n
             };
             const {
                 url: r,
                 query: o,
                 fragmentIdentifier: i
-            } = Mo(e, n);
-            return Oo({
+            } = ai(e, n);
+            return si({
                 url: r,
-                query: ro(o, t),
+                query: Go(o, t),
                 fragmentIdentifier: i
             }, n)
         }
 
-        function zo(e, t, n) {
-            return go(e, Array.isArray(t) ? e => !t.includes(e) : (e, n) => !t(e, n), n)
+        function ci(e, t, n) {
+            return li(e, Array.isArray(t) ? e => !t.includes(e) : (e, n) => !t(e, n), n)
         }
-        const yo = e;
-        const Ao = function(e, n) {
+        const ui = e;
+        const pi = function(e, n) {
             const r = (0, t.useRef)(null),
                 o = (0, t.useRef)(e);
             return (0, t.useEffect)((() => {
                 o.current = e
             }), [e]), (0, t.useEffect)((() => (r.current = setTimeout(o.current, n), () => {
                 r.current && (clearTimeout(r.current), r.current = null)
             })), [n]), (0, t.useCallback)((() => {
                 r.current && clearTimeout(r.current)
             }), [])
         };
-        var vo = __webpack_require__(90994),
-            wo = __webpack_require__(23849),
-            So = __webpack_require__(84192);
-        let qo, Eo;
+        var di = __webpack_require__(90994),
+            bi = __webpack_require__(23849),
+            fi = __webpack_require__(84192);
+        let hi, mi;
         ! function(e) {
             e.COMPONENT_READY = "streamlit:componentReady", e.SET_COMPONENT_VALUE = "streamlit:setComponentValue", e.SET_FRAME_HEIGHT = "streamlit:setFrameHeight"
-        }(qo || (qo = {})),
+        }(hi || (hi = {})),
         function(e) {
             e.RENDER = "streamlit:render"
-        }(Eo || (Eo = {}));
-        const _o = 1;
+        }(mi || (mi = {}));
+        const Mi = 1;
 
-        function xo(e) {
+        function Oi(e) {
             return (t, n) => {
                 if (!e.current) return;
                 const {
                     isReady: r,
                     element: o,
                     widgetMgr: i,
                     setComponentError: a,
                     componentReadyCallback: s,
                     frameHeightCallback: l,
                     fragmentId: c
                 } = e.current, u = r();
                 switch (t) {
-                    case qo.COMPONENT_READY: {
+                    case hi.COMPONENT_READY: {
                         const {
                             apiVersion: e
                         } = n;
-                        e !== _o ? a(new Error("Unrecognized component API version: '".concat(e, "'"))) : s();
+                        e !== Mi ? a(new Error("Unrecognized component API version: '".concat(e, "'"))) : s();
                         break
                     }
-                    case qo.SET_COMPONENT_VALUE:
+                    case hi.SET_COMPONENT_VALUE:
                         u ? function(e, t, n, r, o, i) {
-                            if (void 0 === e) return void(0, wo.KE)("handleSetComponentValue: missing 'value' prop");
+                            if (void 0 === e) return void(0, bi.KE)("handleSetComponentValue: missing 'value' prop");
                             switch (t) {
                                 case "dataframe":
                                     o.setArrowValue(r, e, n, i);
                                     break;
                                 case "bytes":
                                     o.setBytesValue(r, e, n, i);
                                     break;
                                 default:
                                     o.setJsonValue(r, e, n, i)
                             }
-                        }(To(n, "value"), n.dataType, {
+                        }(zi(n, "value"), n.dataType, {
                             fromUi: !0
-                        }, o, i, c) : (0, wo.KE)("Got ".concat(t, " before ").concat(qo.COMPONENT_READY, "!"));
+                        }, o, i, c) : (0, bi.KE)("Got ".concat(t, " before ").concat(hi.COMPONENT_READY, "!"));
                         break;
-                    case qo.SET_FRAME_HEIGHT:
-                        u ? l(To(n, "height")) : (0, wo.KE)("Got ".concat(t, " before ").concat(qo.COMPONENT_READY, "!"));
+                    case hi.SET_FRAME_HEIGHT:
+                        u ? l(zi(n, "height")) : (0, bi.KE)("Got ".concat(t, " before ").concat(hi.COMPONENT_READY, "!"));
                         break;
                     default:
-                        (0, wo.KE)("Unrecognized ComponentBackMsgType: ".concat(t))
+                        (0, bi.KE)("Unrecognized ComponentBackMsgType: ".concat(t))
                 }
             }
         }
 
-        function Ro(e, t, n, r, o) {
+        function gi(e, t, n, r, o) {
             o ? null != o.contentWindow ? o.contentWindow.postMessage({
-                type: Eo.RENDER,
+                type: mi.RENDER,
                 args: e,
                 dfs: t,
                 disabled: n,
                 theme: (0, ye.ol)(r)
-            }, "*") : (0, wo.KE)("Can't send ForwardMsg; iframe has no contentWindow!") : (0, wo.KE)("Can't send ForwardMsg; missing our iframe!")
+            }, "*") : (0, bi.KE)("Can't send ForwardMsg; iframe has no contentWindow!") : (0, bi.KE)("Can't send ForwardMsg; missing our iframe!")
         }
 
-        function To(e, t) {
+        function zi(e, t) {
             let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : void 0;
             return e.hasOwnProperty(t) ? e[t] : n
         }
 
-        function ko(e, t, n) {
+        function yi(e, t, n) {
             let r;
             r = null != n && "" !== n ? n : t.getComponentURL(e, "index.html");
             const o = new URL(window.location.href);
-            return r = yo.stringifyUrl({
+            return r = ui.stringifyUrl({
                 url: r,
                 query: {
                     streamlitUrl: o.origin + o.pathname
                 }
             }), r
         }
 
-        function Co(e, t) {
+        function Ai(e, t) {
             let n;
-            return n = t && "" !== t ? "Your app is having trouble loading the **".concat(e, "** component.") + "\nThe app is attempting to load the component from **".concat(t, "**,") + "\nand hasn't received its `Streamlit.setComponentReady()` message.\n\nIf this is a development build, have you started the dev server?" + "\n\nFor more troubleshooting help, please see the [Streamlit Component docs](".concat(So.Mu, ") or visit our [forums](").concat(So.xz, ").") : "Your app is having trouble loading the **".concat(e, "** component.") + "\n\nIf this is an installed component that works locally, the app may be having trouble accessing the component frontend assets due to network latency or proxy settings in your app deployment." + "\n\nFor more troubleshooting help, please see the [Streamlit Component docs](".concat(So.Mu, ") or visit our [forums](").concat(So.xz, ")."), n
+            return n = t && "" !== t ? "Your app is having trouble loading the **".concat(e, "** component.") + "\nThe app is attempting to load the component from **".concat(t, "**,") + "\nand hasn't received its `Streamlit.setComponentReady()` message.\n\nIf this is a development build, have you started the dev server?" + "\n\nFor more troubleshooting help, please see the [Streamlit Component docs](".concat(fi.Mu, ") or visit our [forums](").concat(fi.xz, ").") : "Your app is having trouble loading the **".concat(e, "** component.") + "\n\nIf this is an installed component that works locally, the app may be having trouble accessing the component frontend assets due to network latency or proxy settings in your app deployment." + "\n\nFor more troubleshooting help, please see the [Streamlit Component docs](".concat(fi.Mu, ") or visit our [forums](").concat(fi.xz, ")."), n
         }
 
-        function Wo(e, t, n, r) {
+        function vi(e, t, n, r) {
             if (!r) try {
                 return function(e, t) {
                     const n = JSON.parse(e),
                         r = [];
                     for (const i of t) {
                         var o;
                         const {
@@ -119394,102 +120251,102 @@
             } catch (o) {
                 n((0, Ve.b)(o))
             }
             return [{},
                 []
             ]
         }
-        const No = (0, Ee.b)((function(e) {
+        const wi = (0, Ee.b)((function(e) {
             const [n, r] = (0, t.useState)(), {
                 disabled: o,
                 element: i,
                 registry: a,
                 theme: s,
                 widgetMgr: l,
                 width: c,
                 fragmentId: u
             } = e, {
                 componentName: p,
                 jsonArgs: d,
                 specialArgs: b,
                 url: f
-            } = i, [h, m] = Wo(d, b, r, n), M = (0, t.useRef)({
+            } = i, [h, m] = vi(d, b, r, n), M = (0, t.useRef)({
                 args: {},
                 dataframeArgs: []
             }), O = (g = M.current.dataframeArgs) === (z = m) || g.length === z.length && g.every(((e, t) => {
                 const n = z[t];
                 return e.key === n.key && e.value === n.value
             }));
             var g, z;
             M.current.args = h, M.current.dataframeArgs = m;
-            const [y, A] = (0, t.useState)(), [v, w] = (0, t.useState)(isNaN(h.height) ? void 0 : h.height), S = (0, t.useRef)(!1), q = (0, t.useRef)(null), E = (0, t.useRef)(), _ = Ao((() => (0, wo.KE)(Co(p, f))), 15e3), x = Ao((() => A(!0)), 6e4);
+            const [y, A] = (0, t.useState)(), [v, w] = (0, t.useState)(isNaN(h.height) ? void 0 : h.height), S = (0, t.useRef)(!1), q = (0, t.useRef)(null), E = (0, t.useRef)(), _ = pi((() => (0, bi.KE)(Ai(p, f))), 15e3), x = pi((() => A(!0)), 6e4);
             if ((0, t.useEffect)((() => {
                     var e;
-                    S.current && Ro(M.current.args, M.current.dataframeArgs, o, s, null !== (e = q.current) && void 0 !== e ? e : void 0)
+                    S.current && gi(M.current.args, M.current.dataframeArgs, o, s, null !== (e = q.current) && void 0 !== e ? e : void 0)
                 }), [o, v, O, d, s, c]), (0, t.useEffect)((() => {
                     E.current = {
                         isReady: () => S.current,
                         element: i,
                         widgetMgr: l,
                         setComponentError: r,
                         componentReadyCallback: () => {
                             var e;
-                            Ro(M.current.args, M.current.dataframeArgs, o, s, null !== (e = q.current) && void 0 !== e ? e : void 0), _(), x(), S.current = !0, A(!1)
+                            gi(M.current.args, M.current.dataframeArgs, o, s, null !== (e = q.current) && void 0 !== e ? e : void 0), _(), x(), S.current = !0, A(!1)
                         },
                         frameHeightCallback: e => {
-                            void 0 !== e ? e !== v && (null != q.current ? (q.current.height = e.toString(), w(e)) : (0, wo.KE)("handleSetFrameHeight: missing our iframeRef!")) : (0, wo.KE)("handleSetFrameHeight: missing 'height' prop")
+                            void 0 !== e ? e !== v && (null != q.current ? (q.current.height = e.toString(), w(e)) : (0, bi.KE)("handleSetFrameHeight: missing our iframeRef!")) : (0, bi.KE)("handleSetFrameHeight: missing 'height' prop")
                         },
                         fragmentId: u
                     }
                 }), [p, o, i, v, O, y, d, s, l, x, _, u]), (0, t.useEffect)((() => {
                     var e, t;
                     const n = null !== (e = null === (t = q.current) || void 0 === t ? void 0 : t.contentWindow) && void 0 !== e ? e : void 0;
-                    if (n) return a.registerListener(n, xo(E)), () => {
+                    if (n) return a.registerListener(n, Oi(E)), () => {
                         n && a.deregisterListener(n)
                     }
-                }), [a, p]), n) return (0, ge.jsx)(Rr.Z, {
+                }), [a, p]), n) return (0, ge.jsx)(zo.Z, {
                 name: n.name,
                 message: n.message
             });
-            const R = !S.current && !y && 0 !== v && (0, ge.jsx)(Gr.O, {
+            const R = !S.current && !y && 0 !== v && (0, ge.jsx)(Io.O, {
                     height: void 0 === v ? void 0 : "".concat(v, "px")
                 }),
                 T = !S.current && y ? (0, ge.jsx)(Ye.Z, {
                     width: c,
-                    body: Co(p, f),
+                    body: Ai(p, f),
                     kind: Ze.h.WARNING
                 }) : null;
             return (0, ge.jsxs)(ge.Fragment, {
                 children: [R, T, (0, ge.jsx)("iframe", {
-                    allow: vo.p,
+                    allow: di.p,
                     ref: q,
-                    src: ko(p, a, f),
+                    src: yi(p, a, f),
                     width: c,
                     height: null !== v && void 0 !== v ? v : 0,
                     style: {
                         colorScheme: "normal",
                         display: S.current ? "initial" : "none"
                     },
                     scrolling: "no",
-                    sandbox: vo.T,
+                    sandbox: di.T,
                     title: p
                 })]
             })
         }));
-        class Lo extends t.Component {
+        class Si extends t.Component {
             shouldComponentUpdate(e) {
                 return this.props.enable || e.enable
             }
             render() {
                 return this.props.children
             }
         }
-        const Io = Lo;
+        const qi = Si;
 
-        function Po(e) {
+        function Ei(e) {
             const {
                 disabled: n,
                 element: r,
                 widgetMgr: o,
                 hasInProgressUpload: i,
                 width: a,
                 fragmentId: s
@@ -119522,44 +120379,44 @@
                             disableLinks: !0
                         })
                     })
                 })
             })
         }
 
-        function Do(e) {
+        function _i(e) {
             const {
                 width: t
             } = e, n = {
                 width: t
             };
             return (0, ge.jsx)(et, {
                 className: "row-widget",
                 style: n,
-                children: (0, ge.jsx)(Po, {
+                children: (0, ge.jsx)(Ei, {
                     ...e
                 })
             })
         }
-        var Bo = __webpack_require__(40108);
+        var xi = __webpack_require__(40108);
         __webpack_require__(32170);
 
-        function jo(e, t) {
+        function Ri(e, t) {
             switch (e.toLowerCase()) {
                 case Yt.$G.H1:
                     return "# ".concat(t);
                 case Yt.$G.H2:
                     return "## ".concat(t);
                 case Yt.$G.H3:
                     return "### ".concat(t);
                 default:
                     throw new Error("Unrecognized tag for header: ".concat(e))
             }
         }
-        const Fo = function(e) {
+        const Ti = function(e) {
             const {
                 width: n,
                 element: r
             } = e, {
                 tag: o,
                 anchor: i,
                 body: a,
@@ -119571,45 +120428,45 @@
                 className: "stHeadingContainer",
                 "data-testid": "stHeading",
                 children: [(0, ge.jsx)("div", {
                     className: "stMarkdown",
                     style: {
                         width: n
                     },
-                    children: (0, ge.jsxs)(Bo.r$, {
+                    children: (0, ge.jsxs)(xi.r$, {
                         isCaption: Boolean(!1),
                         isInSidebar: u,
                         style: {
                             width: n
                         },
                         "data-testid": "stMarkdownContainer",
-                        children: [(0, ge.jsx)(Bo.jO, {
+                        children: [(0, ge.jsx)(xi.jO, {
                             children: (0, ge.jsx)(Yt.U6, {
                                 tag: o,
                                 anchor: i,
                                 hideAnchor: l,
-                                children: s ? (0, ge.jsxs)(kr.KH, {
+                                children: s ? (0, ge.jsxs)(Ao.KH, {
                                     children: [(0, ge.jsx)(Yt.cw, {
-                                        source: jo(o, p),
+                                        source: Ri(o, p),
                                         allowHTML: !1,
                                         overrideComponents: {
                                             p: t.Fragment,
                                             h1: t.Fragment,
                                             h2: t.Fragment,
                                             h3: t.Fragment,
                                             h4: t.Fragment,
                                             h5: t.Fragment,
                                             h6: t.Fragment
                                         }
-                                    }), (0, ge.jsx)(Cr.w, {
+                                    }), (0, ge.jsx)(vo.w, {
                                         content: s
                                     })]
                                 }) : (0, ge.jsx)(ge.Fragment, {
                                     children: (0, ge.jsx)(Yt.cw, {
-                                        source: jo(o, p),
+                                        source: Ri(o, p),
                                         allowHTML: !1,
                                         overrideComponents: {
                                             p: t.Fragment,
                                             h1: t.Fragment,
                                             h2: t.Fragment,
                                             h3: t.Fragment,
                                             h4: t.Fragment,
@@ -119620,43 +120477,43 @@
                                 })
                             })
                         }), d.length > 0 && (0, ge.jsx)(Yt.cw, {
                             source: d.join("\n"),
                             allowHTML: !1
                         })]
                     })
-                }), c && (0, ge.jsx)(Bo.IW, {
+                }), c && (0, ge.jsx)(xi.IW, {
                     "data-testid": "stHeadingDivider",
                     rainbow: c.includes("linear"),
                     color: c
                 })]
             })
         };
 
-        function Uo(e, t) {
+        function ki(e, t) {
             let n = t.spacing.lg;
             return "medium" === e ? n = t.spacing.threeXL : "large" === e && (n = t.spacing.fourXL), n
         }
-        const Vo = (0, Qe.Z)("div", {
+        const Ci = (0, Qe.Z)("div", {
                 target: "e1f1d6gn5"
             })((e => {
                 let {
                     theme: t,
                     gap: n
                 } = e;
                 return {
                     display: "flex",
                     flexWrap: "wrap",
                     flexGrow: 1,
                     alignItems: "stretch",
-                    gap: Uo(n, t)
+                    gap: ki(n, t)
                 }
             }), ""),
-            Ho = ["balloons", "snow"],
-            Xo = (0, Qe.Z)("div", {
+            Wi = ["balloons", "snow"],
+            Ni = (0, Qe.Z)("div", {
                 target: "e1f1d6gn4"
             })((e => {
                 let {
                     theme: t,
                     isStale: n,
                     width: r,
                     elementType: o
@@ -119687,39 +120544,39 @@
                     ...n && "skeleton" !== o ? {
                         opacity: .33,
                         transition: "opacity 1s ease-in 0.5s"
                     } : {},
                     ..."empty" === o ? {
                         display: "none"
                     } : {},
-                    ...Ho.includes(o) ? {
+                    ...Wi.includes(o) ? {
                         marginBottom: "-".concat(t.spacing.lg)
                     } : {}
                 }
             }), ""),
-            Go = (0, Qe.Z)("div", {
+            Li = (0, Qe.Z)("div", {
                 target: "e1f1d6gn3"
             })((e => {
                 let {
                     weight: t,
                     gap: n,
                     theme: r
                 } = e;
                 const o = 100 * t,
-                    i = Uo(n, r),
+                    i = ki(n, r),
                     a = "calc(".concat(o, "% - ").concat(i, ")");
                 return {
                     width: a,
                     flex: "1 1 ".concat(a),
                     ["@media (max-width: ".concat(r.breakpoints.columns, ")")]: {
                         minWidth: "calc(100% - ".concat(r.spacing.twoXL, ")")
                     }
                 }
             }), ""),
-            $o = (0, Qe.Z)("div", {
+            Ii = (0, Qe.Z)("div", {
                 target: "e1f1d6gn2"
             })((e => {
                 let {
                     width: t,
                     theme: n
                 } = e;
                 return {
@@ -119727,21 +120584,21 @@
                     position: "relative",
                     display: "flex",
                     flex: 1,
                     flexDirection: "column",
                     gap: n.spacing.lg
                 }
             }), ""),
-            Ko = (0, Qe.Z)("div", {
+            Pi = (0, Qe.Z)("div", {
                 target: "e1f1d6gn1"
             })({
                 name: "1wmy9hl",
                 styles: "display:flex;flex-direction:column;flex:1"
             }),
-            Yo = (0, Qe.Z)("div", {
+            Di = (0, Qe.Z)("div", {
                 target: "e1f1d6gn0"
             })((e => {
                 let {
                     theme: t,
                     border: n,
                     height: r
                 } = e;
@@ -119753,54 +120610,54 @@
                     },
                     ...r && {
                         height: "".concat(r, "px"),
                         overflow: "auto"
                     }
                 }
             }), ""),
-            Zo = t.lazy((() => __webpack_require__.e(9330).then(__webpack_require__.bind(__webpack_require__, 69330)))),
-            Jo = t.lazy((() => __webpack_require__.e(7217).then(__webpack_require__.bind(__webpack_require__, 62736)))),
-            Qo = t.lazy((() => __webpack_require__.e(3301).then(__webpack_require__.bind(__webpack_require__, 69436)))),
-            ei = t.lazy((() => Promise.all([__webpack_require__.e(4253), __webpack_require__.e(3092)]).then(__webpack_require__.bind(__webpack_require__, 49839)))),
-            ti = t.lazy((() => Promise.all([__webpack_require__.e(3998), __webpack_require__.e(656), __webpack_require__.e(43)]).then(__webpack_require__.bind(__webpack_require__, 10043)))),
-            ni = t.lazy((() => __webpack_require__.e(8427).then(__webpack_require__.bind(__webpack_require__, 18427)))),
-            ri = $n(t.lazy((() => __webpack_require__.e(7323).then(__webpack_require__.bind(__webpack_require__, 47323)))), 100),
-            oi = t.lazy((() => Promise.all([__webpack_require__.e(2411), __webpack_require__.e(4185)]).then(__webpack_require__.bind(__webpack_require__, 72394)))),
-            ii = t.lazy((() => Promise.all([__webpack_require__.e(3998), __webpack_require__.e(6150), __webpack_require__.e(7805)]).then(__webpack_require__.bind(__webpack_require__, 32508)))),
-            ai = t.lazy((() => __webpack_require__.e(4500).then(__webpack_require__.bind(__webpack_require__, 54500)))),
-            si = t.lazy((() => __webpack_require__.e(1307).then(__webpack_require__.bind(__webpack_require__, 51307)))),
-            li = t.lazy((() => __webpack_require__.e(2469).then(__webpack_require__.bind(__webpack_require__, 62469)))),
-            ci = t.lazy((() => __webpack_require__.e(4113).then(__webpack_require__.bind(__webpack_require__, 34113)))),
-            ui = t.lazy((() => Promise.all([__webpack_require__.e(2736), __webpack_require__.e(1168)]).then(__webpack_require__.bind(__webpack_require__, 71168)))),
-            pi = t.lazy((() => __webpack_require__.e(178).then(__webpack_require__.bind(__webpack_require__, 178)))),
-            di = t.lazy((() => __webpack_require__.e(1792).then(__webpack_require__.bind(__webpack_require__, 61792)))),
-            bi = t.lazy((() => __webpack_require__.e(3513).then(__webpack_require__.bind(__webpack_require__, 33513)))),
-            fi = t.lazy((() => Promise.all([__webpack_require__.e(8570), __webpack_require__.e(4132), __webpack_require__.e(7602)]).then(__webpack_require__.bind(__webpack_require__, 47602)))),
-            hi = t.lazy((() => Promise.all([__webpack_require__.e(9656), __webpack_require__.e(6013)]).then(__webpack_require__.bind(__webpack_require__, 46013)))),
-            mi = t.lazy((() => __webpack_require__.e(8492).then(__webpack_require__.bind(__webpack_require__, 28492)))),
-            Mi = t.lazy((() => __webpack_require__.e(4177).then(__webpack_require__.bind(__webpack_require__, 94177)))),
-            Oi = t.lazy((() => Promise.all([__webpack_require__.e(9656), __webpack_require__.e(7142), __webpack_require__.e(5791), __webpack_require__.e(1451)]).then(__webpack_require__.bind(__webpack_require__, 61451)))),
-            gi = t.lazy((() => Promise.all([__webpack_require__.e(937), __webpack_require__.e(2634)]).then(__webpack_require__.bind(__webpack_require__, 72634)))),
-            zi = t.lazy((() => __webpack_require__.e(1074).then(__webpack_require__.bind(__webpack_require__, 91074)))),
-            yi = t.lazy((() => Promise.all([__webpack_require__.e(8570), __webpack_require__.e(8477)]).then(__webpack_require__.bind(__webpack_require__, 58477)))),
-            Ai = t.lazy((() => __webpack_require__.e(6853).then(__webpack_require__.bind(__webpack_require__, 76853)))),
-            vi = t.lazy((() => __webpack_require__.e(4477).then(__webpack_require__.bind(__webpack_require__, 74477)))),
-            wi = t.lazy((() => __webpack_require__.e(4319).then(__webpack_require__.bind(__webpack_require__, 94319)))),
-            Si = t.lazy((() => Promise.all([__webpack_require__.e(2187), __webpack_require__.e(5106)]).then(__webpack_require__.bind(__webpack_require__, 5106)))),
-            qi = t.lazy((() => Promise.all([__webpack_require__.e(8570), __webpack_require__.e(5117), __webpack_require__.e(4666)]).then(__webpack_require__.bind(__webpack_require__, 14666)))),
-            Ei = t.lazy((() => Promise.all([__webpack_require__.e(9656), __webpack_require__.e(5379)]).then(__webpack_require__.bind(__webpack_require__, 35379)))),
-            _i = t.lazy((() => Promise.all([__webpack_require__.e(9656), __webpack_require__.e(8691)]).then(__webpack_require__.bind(__webpack_require__, 58691)))),
-            xi = t.lazy((() => Promise.all([__webpack_require__.e(7142), __webpack_require__.e(6718)]).then(__webpack_require__.bind(__webpack_require__, 36718)))),
-            Ri = t.lazy((() => Promise.all([__webpack_require__.e(9656), __webpack_require__.e(1479), __webpack_require__.e(7175)]).then(__webpack_require__.bind(__webpack_require__, 67175)))),
-            Ti = t.lazy((() => Promise.resolve().then(__webpack_require__.bind(__webpack_require__, 88112))));
+            Bi = t.lazy((() => __webpack_require__.e(9330).then(__webpack_require__.bind(__webpack_require__, 69330)))),
+            ji = t.lazy((() => __webpack_require__.e(7217).then(__webpack_require__.bind(__webpack_require__, 62736)))),
+            Fi = t.lazy((() => __webpack_require__.e(3301).then(__webpack_require__.bind(__webpack_require__, 69436)))),
+            Ui = t.lazy((() => Promise.all([__webpack_require__.e(4253), __webpack_require__.e(3092)]).then(__webpack_require__.bind(__webpack_require__, 49839)))),
+            Vi = t.lazy((() => Promise.all([__webpack_require__.e(3998), __webpack_require__.e(656), __webpack_require__.e(43)]).then(__webpack_require__.bind(__webpack_require__, 10043)))),
+            Hi = t.lazy((() => __webpack_require__.e(8427).then(__webpack_require__.bind(__webpack_require__, 18427)))),
+            Xi = Ir(t.lazy((() => __webpack_require__.e(7323).then(__webpack_require__.bind(__webpack_require__, 47323)))), 100),
+            Gi = t.lazy((() => Promise.all([__webpack_require__.e(2411), __webpack_require__.e(4185)]).then(__webpack_require__.bind(__webpack_require__, 72394)))),
+            $i = t.lazy((() => Promise.all([__webpack_require__.e(3998), __webpack_require__.e(6150), __webpack_require__.e(7805)]).then(__webpack_require__.bind(__webpack_require__, 32508)))),
+            Ki = t.lazy((() => __webpack_require__.e(4500).then(__webpack_require__.bind(__webpack_require__, 54500)))),
+            Yi = t.lazy((() => __webpack_require__.e(1307).then(__webpack_require__.bind(__webpack_require__, 51307)))),
+            Zi = t.lazy((() => __webpack_require__.e(2469).then(__webpack_require__.bind(__webpack_require__, 62469)))),
+            Ji = t.lazy((() => __webpack_require__.e(4113).then(__webpack_require__.bind(__webpack_require__, 34113)))),
+            Qi = t.lazy((() => Promise.all([__webpack_require__.e(2736), __webpack_require__.e(1168)]).then(__webpack_require__.bind(__webpack_require__, 71168)))),
+            ea = t.lazy((() => __webpack_require__.e(178).then(__webpack_require__.bind(__webpack_require__, 178)))),
+            ta = t.lazy((() => __webpack_require__.e(1792).then(__webpack_require__.bind(__webpack_require__, 61792)))),
+            na = t.lazy((() => __webpack_require__.e(3513).then(__webpack_require__.bind(__webpack_require__, 33513)))),
+            ra = t.lazy((() => Promise.all([__webpack_require__.e(8570), __webpack_require__.e(4132), __webpack_require__.e(7602)]).then(__webpack_require__.bind(__webpack_require__, 47602)))),
+            oa = t.lazy((() => Promise.all([__webpack_require__.e(9656), __webpack_require__.e(6013)]).then(__webpack_require__.bind(__webpack_require__, 46013)))),
+            ia = t.lazy((() => __webpack_require__.e(8492).then(__webpack_require__.bind(__webpack_require__, 28492)))),
+            aa = t.lazy((() => __webpack_require__.e(4177).then(__webpack_require__.bind(__webpack_require__, 94177)))),
+            sa = t.lazy((() => Promise.all([__webpack_require__.e(9656), __webpack_require__.e(7142), __webpack_require__.e(5791), __webpack_require__.e(1451)]).then(__webpack_require__.bind(__webpack_require__, 61451)))),
+            la = t.lazy((() => Promise.all([__webpack_require__.e(937), __webpack_require__.e(2634)]).then(__webpack_require__.bind(__webpack_require__, 72634)))),
+            ca = t.lazy((() => __webpack_require__.e(1074).then(__webpack_require__.bind(__webpack_require__, 91074)))),
+            ua = t.lazy((() => Promise.all([__webpack_require__.e(8570), __webpack_require__.e(8477)]).then(__webpack_require__.bind(__webpack_require__, 58477)))),
+            pa = t.lazy((() => __webpack_require__.e(6853).then(__webpack_require__.bind(__webpack_require__, 76853)))),
+            da = t.lazy((() => __webpack_require__.e(4477).then(__webpack_require__.bind(__webpack_require__, 74477)))),
+            ba = t.lazy((() => __webpack_require__.e(4319).then(__webpack_require__.bind(__webpack_require__, 94319)))),
+            fa = t.lazy((() => Promise.all([__webpack_require__.e(2187), __webpack_require__.e(5106)]).then(__webpack_require__.bind(__webpack_require__, 5106)))),
+            ha = t.lazy((() => Promise.all([__webpack_require__.e(8570), __webpack_require__.e(5117), __webpack_require__.e(4666)]).then(__webpack_require__.bind(__webpack_require__, 14666)))),
+            ma = t.lazy((() => Promise.all([__webpack_require__.e(9656), __webpack_require__.e(5379)]).then(__webpack_require__.bind(__webpack_require__, 35379)))),
+            Ma = t.lazy((() => Promise.all([__webpack_require__.e(9656), __webpack_require__.e(8691)]).then(__webpack_require__.bind(__webpack_require__, 58691)))),
+            Oa = t.lazy((() => Promise.all([__webpack_require__.e(7142), __webpack_require__.e(6718)]).then(__webpack_require__.bind(__webpack_require__, 36718)))),
+            ga = t.lazy((() => Promise.all([__webpack_require__.e(9656), __webpack_require__.e(1479), __webpack_require__.e(7175)]).then(__webpack_require__.bind(__webpack_require__, 67175)))),
+            za = t.lazy((() => Promise.resolve().then(__webpack_require__.bind(__webpack_require__, 88112))));
 
-        function ki(e, t) {
+        function ya(e, t) {
             return e ? (0, ge.jsx)(ge.Fragment, {}) : t
         }
-        const Ci = e => {
+        const Aa = e => {
                 const {
                     node: t
                 } = e;
                 if (!t) throw new Error("ElementNode not found.");
                 const n = {
                         width: e.width,
                         disableFullscreenMode: e.disableFullscreenMode
@@ -119818,356 +120675,360 @@
                             icon: e.icon,
                             body: e.body,
                             kind: (0, Ye.O)(e.format),
                             ...n
                         })
                     }
                     case "arrowTable":
-                        return (0, ge.jsx)(ir, {
+                        return (0, ge.jsx)($r, {
                             element: t.quiverElement,
                             ...n
                         });
                     case "arrowVegaLiteChart":
-                        return (0, ge.jsx)(ti, {
+                        return (0, ge.jsx)(Vi, {
                             element: t.vegaLiteChartElement,
                             ...n
                         });
                     case "audio":
-                        return (0, ge.jsx)(Zo, {
+                        return (0, ge.jsx)(Bi, {
                             element: t.element.audio,
                             endpoints: e.endpoints,
                             ...n
                         });
                     case "balloons":
-                        return ki(e.isStale, (0, ge.jsx)(Jo, {
+                        return ya(e.isStale, (0, ge.jsx)(ji, {
                             scriptRunId: e.scriptRunId
                         }));
                     case "bokehChart":
-                        return (0, ge.jsx)(ri, {
+                        return (0, ge.jsx)(Xi, {
                             element: t.element.bokehChart,
                             ...n
                         });
                     case "code": {
                         const e = t.element.code;
-                        return (0, ge.jsx)(Ti, {
+                        return (0, ge.jsx)(za, {
                             language: e.language,
                             showLineNumbers: e.showLineNumbers,
                             children: e.codeText
                         })
                     }
                     case "deckGlJsonChart":
-                        return (0, ge.jsx)(oi, {
+                        return (0, ge.jsx)(Gi, {
                             element: t.element.deckGlJsonChart,
                             ...n
                         });
                     case "docString":
-                        return (0, ge.jsx)(Mr, {
+                        return (0, ge.jsx)(ao, {
                             element: t.element.docString,
                             ...n
                         });
                     case "empty":
                         return (0, ge.jsx)("div", {
                             className: "stHidden"
                         });
                     case "exception":
-                        return (0, ge.jsx)(qr, {
+                        return (0, ge.jsx)(mo, {
                             element: t.element.exception,
                             ...n
                         });
                     case "graphvizChart":
-                        return (0, ge.jsx)(ii, {
+                        return (0, ge.jsx)($i, {
                             element: t.element.graphvizChart,
                             ...n
                         });
                     case "heading":
-                        return (0, ge.jsx)(Fo, {
+                        return (0, ge.jsx)(Ti, {
                             element: t.element.heading,
                             ...n
                         });
                     case "iframe":
-                        return (0, ge.jsx)(ai, {
+                        return (0, ge.jsx)(Ki, {
                             element: t.element.iframe,
                             ...n
                         });
                     case "imgs":
-                        return (0, ge.jsx)(si, {
+                        return (0, ge.jsx)(Yi, {
                             element: t.element.imgs,
                             endpoints: e.endpoints,
                             ...n
                         });
                     case "json":
-                        return (0, ge.jsx)(Tr, {
+                        return (0, ge.jsx)(yo, {
                             element: t.element.json,
                             ...n
                         });
                     case "markdown":
-                        return (0, ge.jsx)(Wr, {
+                        return (0, ge.jsx)(wo, {
                             element: t.element.markdown,
                             ...n
                         });
                     case "metric":
-                        return (0, ge.jsx)(Ur, {
+                        return (0, ge.jsx)(Co, {
                             element: t.element.metric
                         });
                     case "html":
-                        return (0, ge.jsx)(gi, {
+                        return (0, ge.jsx)(la, {
                             element: t.element.html,
                             ...n
                         });
                     case "pageLink": {
                         const e = t.element.pageLink,
                             o = r.disabled || e.disabled;
-                        return (0, ge.jsx)(ci, {
+                        return (0, ge.jsx)(Ji, {
                             element: e,
                             disabled: o,
                             ...n
                         })
                     }
                     case "plotlyChart":
-                        return (0, ge.jsx)(ui, {
+                        return (0, ge.jsx)(Qi, {
                             element: t.element.plotlyChart,
                             height: void 0,
                             ...n
                         });
                     case "progress":
-                        return (0, ge.jsx)(yi, {
+                        return (0, ge.jsx)(ua, {
                             element: t.element.progress,
                             ...n
                         });
                     case "skeleton":
-                        return (0, ge.jsx)(Xr, {});
+                        return (0, ge.jsx)(Lo, {});
                     case "snow":
-                        return ki(e.isStale, (0, ge.jsx)(Qo, {
+                        return ya(e.isStale, (0, ge.jsx)(Fi, {
                             scriptRunId: e.scriptRunId
                         }));
                     case "spinner":
-                        return (0, ge.jsx)(Ai, {
+                        return (0, ge.jsx)(pa, {
                             element: t.element.spinner,
                             ...n
                         });
                     case "text":
-                        return (0, ge.jsx)(Kr, {
+                        return (0, ge.jsx)(Do, {
                             element: t.element.text,
                             ...n
                         });
                     case "video":
-                        return (0, ge.jsx)(pi, {
+                        return (0, ge.jsx)(ea, {
                             element: t.element.video,
                             endpoints: e.endpoints,
                             ...n
                         });
                     case "toast": {
                         const e = t.element.toast;
-                        return (0, ge.jsx)(ni, {
+                        return (0, ge.jsx)(Hi, {
                             body: e.body,
                             icon: e.icon,
                             ...n
                         }, t.scriptRunId)
                     }
                     case "arrowDataFrame": {
                         const e = t.element.arrowDataFrame;
-                        return r.disabled = r.disabled || e.disabled, (0, ge.jsx)(ei, {
+                        return r.disabled = r.disabled || e.disabled, (0, ge.jsx)(Ui, {
                             element: e,
                             data: t.quiverElement,
                             ...e.id && {
                                 key: e.id
                             },
                             ...r
                         })
                     }
                     case "button": {
                         const n = t.element.button;
                         if (r.disabled = r.disabled || n.disabled, n.isFormSubmitter) {
                             const {
                                 formId: t
                             } = n, o = e.formsData.formsWithUploads.has(t);
-                            return (0, ge.jsx)(Do, {
+                            return (0, ge.jsx)(_i, {
                                 element: n,
                                 hasInProgressUpload: o,
                                 ...r
                             })
                         }
-                        return (0, ge.jsx)(di, {
+                        return (0, ge.jsx)(ta, {
                             element: n,
                             ...r
                         })
                     }
                     case "downloadButton": {
                         const n = t.element.downloadButton;
-                        return r.disabled = r.disabled || n.disabled, (0, ge.jsx)(bi, {
+                        return r.disabled = r.disabled || n.disabled, (0, ge.jsx)(na, {
                             endpoints: e.endpoints,
                             element: n,
                             ...r
                         }, n.id)
                     }
                     case "cameraInput": {
                         const n = t.element.cameraInput;
-                        return r.disabled = r.disabled || n.disabled, (0, ge.jsx)(fi, {
+                        return r.disabled = r.disabled || n.disabled, (0, ge.jsx)(ra, {
                             element: n,
                             uploadClient: e.uploadClient,
                             ...r
                         }, n.id)
                     }
                     case "chatInput": {
                         const e = t.element.chatInput;
-                        return r.disabled = r.disabled || e.disabled, (0, ge.jsx)(hi, {
+                        return r.disabled = r.disabled || e.disabled, (0, ge.jsx)(oa, {
                             element: e,
                             ...r
                         }, e.id)
                     }
                     case "checkbox": {
                         const e = t.element.checkbox;
-                        return r.disabled = r.disabled || e.disabled, (0, ge.jsx)(mi, {
+                        return r.disabled = r.disabled || e.disabled, (0, ge.jsx)(ia, {
                             element: e,
                             ...r
                         }, e.id)
                     }
                     case "colorPicker": {
                         const e = t.element.colorPicker;
-                        return r.disabled = r.disabled || e.disabled, (0, ge.jsx)(Mi, {
+                        return r.disabled = r.disabled || e.disabled, (0, ge.jsx)(aa, {
                             element: e,
                             ...r
                         }, e.id)
                     }
                     case "componentInstance":
-                        return (0, ge.jsx)(No, {
+                        return (0, ge.jsx)(wi, {
                             registry: e.componentRegistry,
                             element: t.element.componentInstance,
                             ...r
                         });
                     case "dateInput": {
                         const e = t.element.dateInput;
-                        return r.disabled = r.disabled || e.disabled, (0, ge.jsx)(Oi, {
+                        return r.disabled = r.disabled || e.disabled, (0, ge.jsx)(sa, {
                             element: e,
                             ...r
                         }, e.id)
                     }
                     case "fileUploader": {
                         const n = t.element.fileUploader;
-                        return r.disabled = r.disabled || n.disabled, (0, ge.jsx)(qi, {
+                        return r.disabled = r.disabled || n.disabled, (0, ge.jsx)(ha, {
                             element: n,
                             uploadClient: e.uploadClient,
                             ...r
                         }, n.id)
                     }
                     case "linkButton": {
                         const e = t.element.linkButton;
-                        return r.disabled = r.disabled || e.disabled, (0, ge.jsx)(li, {
+                        return r.disabled = r.disabled || e.disabled, (0, ge.jsx)(Zi, {
                             element: e,
                             ...r
                         })
                     }
                     case "multiselect": {
                         const e = t.element.multiselect;
-                        return r.disabled = r.disabled || e.disabled, (0, ge.jsx)(zi, {
+                        return r.disabled = r.disabled || e.disabled, (0, ge.jsx)(ca, {
                             element: e,
                             ...r
                         }, e.id)
                     }
                     case "numberInput": {
                         const e = t.element.numberInput;
-                        return r.disabled = r.disabled || e.disabled, (0, ge.jsx)(Ri, {
+                        return r.disabled = r.disabled || e.disabled, (0, ge.jsx)(ga, {
                             element: e,
                             ...r
                         }, e.id)
                     }
                     case "radio": {
                         const e = t.element.radio;
-                        return r.disabled = r.disabled || e.disabled, (0, ge.jsx)(vi, {
+                        return r.disabled = r.disabled || e.disabled, (0, ge.jsx)(da, {
                             element: e,
                             ...r
                         }, e.id)
                     }
                     case "selectbox": {
                         const e = t.element.selectbox;
-                        return r.disabled = r.disabled || e.disabled, (0, ge.jsx)(wi, {
+                        return r.disabled = r.disabled || e.disabled, (0, ge.jsx)(ba, {
                             element: e,
                             ...r
                         }, e.id)
                     }
                     case "slider": {
                         const e = t.element.slider;
-                        return r.disabled = r.disabled || e.disabled, (0, ge.jsx)(Si, {
+                        return r.disabled = r.disabled || e.disabled, (0, ge.jsx)(fa, {
                             element: e,
                             ...r
                         }, e.id)
                     }
                     case "textArea": {
                         const e = t.element.textArea;
-                        return r.disabled = r.disabled || e.disabled, (0, ge.jsx)(Ei, {
+                        return r.disabled = r.disabled || e.disabled, (0, ge.jsx)(ma, {
                             element: e,
                             ...r
                         }, e.id)
                     }
                     case "textInput": {
                         const e = t.element.textInput;
-                        return r.disabled = r.disabled || e.disabled, (0, ge.jsx)(_i, {
+                        return r.disabled = r.disabled || e.disabled, (0, ge.jsx)(Ma, {
                             element: e,
                             ...r
                         }, e.id)
                     }
                     case "timeInput": {
                         const e = t.element.timeInput;
-                        return r.disabled = r.disabled || e.disabled, (0, ge.jsx)(xi, {
+                        return r.disabled = r.disabled || e.disabled, (0, ge.jsx)(Oa, {
                             element: e,
                             ...r
                         }, e.id)
                     }
                     default:
                         throw new Error("Unrecognized Element type ".concat(t.element.type))
                 }
             },
-            Wi = e => {
+            va = e => {
                 const {
                     isFullScreen: n,
                     fragmentIdsThisRun: r
                 } = t.useContext(Fe.E), {
                     node: o,
                     width: i
                 } = e, a = o.element.type || "", s = Gt(a, e.scriptRunState), l = Kt(s, o, e.scriptRunState, e.scriptRunId, r);
-                return (0, ge.jsx)(Io, {
+                return (0, ge.jsx)(qi, {
                     enable: s,
-                    children: (0, ge.jsx)(Xo, {
+                    children: (0, ge.jsx)(Ni, {
                         "data-stale": l,
                         isStale: l && !n,
                         width: i,
                         className: "element-container",
                         "data-testid": "element-container",
                         elementType: a,
-                        children: (0, ge.jsx)(gr.Z, {
+                        children: (0, ge.jsx)(lo.Z, {
                             width: i,
                             children: (0, ge.jsx)(t.Suspense, {
-                                fallback: (0, ge.jsx)(Gr.O, {}),
-                                children: (0, ge.jsx)(Ci, {
+                                fallback: (0, ge.jsx)(Io.O, {}),
+                                children: (0, ge.jsx)(Aa, {
                                     ...e,
                                     isStale: l
                                 })
                             })
                         })
                     })
                 })
             },
-            Ni = e => {
+            wa = e => {
                 const {
                     node: n
                 } = e, {
                     fragmentIdsThisRun: r
                 } = (0, t.useContext)(Fe.E);
                 if (n.isEmpty && !n.deltaBlock.allowEmpty) return (0, ge.jsx)(ge.Fragment, {});
                 const o = Kt(Gt("", e.scriptRunState), n, e.scriptRunState, e.scriptRunId, r),
                     i = {
                         ...e,
                         node: n
                     },
-                    a = e.disableFullscreenMode || (0, He.bb)(n.deltaBlock.popover),
-                    s = (0, ge.jsx)(Bi, {
+                    a = e.disableFullscreenMode || (0, He.bb)(n.deltaBlock.dialog) || (0, He.bb)(n.deltaBlock.popover),
+                    s = (0, ge.jsx)(xa, {
                         ...i,
                         disableFullscreenMode: a
                     });
-                if (n.deltaBlock.expandable) return (0, ge.jsx)(kn, {
+                if (n.deltaBlock.dialog) return (0, ge.jsx)(pr, {
+                    element: n.deltaBlock.dialog,
+                    children: s
+                });
+                if (n.deltaBlock.expandable) return (0, ge.jsx)(yr, {
                     empty: n.isEmpty,
                     isStale: o,
                     element: n.deltaBlock.expandable,
                     children: s
                 });
                 if (n.deltaBlock.popover) return (0, ge.jsx)(dn, {
                     empty: n.isEmpty,
@@ -120194,36 +121055,36 @@
                 }
                 if (n.deltaBlock.chatMessage) return (0, ge.jsx)(An, {
                     element: n.deltaBlock.chatMessage,
                     endpoints: e.endpoints,
                     children: s
                 });
                 var l, c;
-                if (n.deltaBlock.column) return (0, ge.jsx)(Go, {
+                if (n.deltaBlock.column) return (0, ge.jsx)(Li, {
                     weight: null !== (l = n.deltaBlock.column.weight) && void 0 !== l ? l : 0,
                     gap: null !== (c = n.deltaBlock.column.gap) && void 0 !== c ? c : "",
                     "data-testid": "column",
                     children: s
                 });
                 if (n.deltaBlock.tabContainer) {
-                    const e = e => (0, ge.jsx)(Pi, {
+                    const e = e => (0, ge.jsx)(Ea, {
                             ...e
                         }),
                         t = {
                             ...i,
                             isStale: o,
                             renderTabContent: e
                         };
                     return (0, ge.jsx)(Jt, {
                         ...t
                     })
                 }
                 return s
             },
-            Li = e => {
+            Sa = e => {
                 const {
                     libConfig: n
                 } = (0, t.useContext)(Fe.E);
                 return function(e, t) {
                     const n = (0, ye.GJ)(t),
                         r = Object.keys(n),
                         {
@@ -120257,49 +121118,49 @@
                         if (t instanceof Ge) {
                             const n = {
                                     ...e,
                                     disableFullscreenMode: o,
                                     node: t
                                 },
                                 i = (0, He.po)(t.element) || r;
-                            return (0, ge.jsx)(Wi, {
+                            return (0, ge.jsx)(va, {
                                 ...n
                             }, i)
                         }
                         if (t instanceof $e) {
                             const n = {
                                 ...e,
                                 disableFullscreenMode: o,
                                 node: t
                             };
-                            return (0, ge.jsx)(Ni, {
+                            return (0, ge.jsx)(wa, {
                                 ...n
                             }, r)
                         }
                         throw new Error("Unrecognized AppNode: ".concat(t))
                     }))
                 })
             };
 
-        function Ii(e) {
+        function qa(e) {
             const {
                 border: t,
                 height: n,
                 children: r
-            } = e, o = jn();
-            return (0, ge.jsx)(Yo, {
+            } = e, o = Rr();
+            return (0, ge.jsx)(Di, {
                 border: t,
                 height: n,
                 "data-testid": "stVerticalBlockBorderWrapper",
                 "data-test-scroll-behavior": "scroll-to-bottom",
                 ref: o,
                 children: r
             })
         }
-        const Pi = e => {
+        const Ea = e => {
                 var n, r, o;
                 const i = (0, t.useRef)(null),
                     [a, s] = t.useState(-1),
                     l = (0, t.useMemo)((() => new ResizeObserver((e => {
                         let [t] = e;
                         window.requestAnimationFrame((() => {
                             s(t.target.getBoundingClientRect().width || -1)
@@ -120307,73 +121168,73 @@
                     }))), [s]),
                     c = null !== (n = null === (r = e.node.deltaBlock.vertical) || void 0 === r ? void 0 : r.border) && void 0 !== n && n,
                     u = (null === (o = e.node.deltaBlock.vertical) || void 0 === o ? void 0 : o.height) || void 0,
                     p = u && void 0 !== e.node.children.find((e => e instanceof $e && "chatMessage" === e.deltaBlock.type));
                 (0, t.useEffect)((() => (i.current && l.observe(i.current), () => {
                     l.disconnect()
                 })), [l, p]);
-                const d = p ? Ii : Yo,
+                const d = p ? qa : Di,
                     b = {
                         ...e,
                         width: a
                     };
                 return (0, ge.jsx)(d, {
                     border: c,
                     height: u,
                     "data-testid": "stVerticalBlockBorderWrapper",
                     "data-test-scroll-behavior": "normal",
-                    children: (0, ge.jsx)(Ko, {
+                    children: (0, ge.jsx)(Pi, {
                         ref: i,
-                        children: (0, ge.jsx)($o, {
+                        children: (0, ge.jsx)(Ii, {
                             width: a,
                             "data-testid": "stVerticalBlock",
-                            children: (0, ge.jsx)(Li, {
+                            children: (0, ge.jsx)(Sa, {
                                 ...b
                             })
                         })
                     })
                 })
             },
-            Di = e => {
+            _a = e => {
                 var t, n;
                 const r = null !== (t = null === (n = e.node.deltaBlock.horizontal) || void 0 === n ? void 0 : n.gap) && void 0 !== t ? t : "";
-                return (0, ge.jsx)(Vo, {
+                return (0, ge.jsx)(Ci, {
                     gap: r,
                     "data-testid": "stHorizontalBlock",
-                    children: (0, ge.jsx)(Li, {
+                    children: (0, ge.jsx)(Sa, {
                         ...e
                     })
                 })
             };
 
-        function Bi(e) {
-            return e.node.deltaBlock.horizontal ? (0, ge.jsx)(Di, {
+        function xa(e) {
+            return e.node.deltaBlock.horizontal ? (0, ge.jsx)(_a, {
                 ...e
-            }) : (0, ge.jsx)(Pi, {
+            }) : (0, ge.jsx)(Ea, {
                 ...e
             })
         }
-        const ji = Pi;
-        var Fi = __webpack_require__(97652);
-        const Ui = function(e) {
+        const Ra = Ea;
+        var Ta = __webpack_require__(97652);
+        const ka = function(e) {
             let {
                 theme: t,
                 baseuiTheme: n,
                 children: r
             } = e;
             return (0, ge.jsx)(we.Z, {
-                theme: n || Fi.t,
+                theme: n || Ta.t,
                 children: (0, ge.jsx)(Ee.a, {
                     theme: t,
                     children: r
                 })
             })
         };
-        var Vi = __webpack_require__(14609),
-            Hi = t.forwardRef((function(e, n) {
+        var Ca = __webpack_require__(14609),
+            Wa = t.forwardRef((function(e, n) {
                 return t.createElement(en.D, (0, Qt.Z)({
                     iconAttrs: {
                         fill: "currentColor",
                         xmlns: "http://www.w3.org/2000/svg"
                     },
                     iconVerticalAlign: "middle",
                     iconViewBox: "0 0 24 24"
@@ -120382,19 +121243,19 @@
                 }), t.createElement("path", {
                     fill: "none",
                     d: "M0 0h24v24H0V0z"
                 }), t.createElement("path", {
                     d: "M19 6.41L17.59 5 12 10.59 6.41 5 5 6.41 10.59 12 5 17.59 6.41 19 12 13.41 17.59 19 19 17.59 13.41 12 19 6.41z"
                 }))
             }));
-        Hi.displayName = "Close";
-        var Xi, Gi = __webpack_require__(17330),
-            $i = __webpack_require__(35365),
-            Ki = __webpack_require__(50669);
-        const Yi = (0, Qe.Z)("section", {
+        Wa.displayName = "Close";
+        var Na, La = __webpack_require__(17330),
+            Ia = __webpack_require__(35365),
+            Pa = __webpack_require__(50669);
+        const Da = (0, Qe.Z)("section", {
                 target: "eczjsme11"
             })((e => {
                 let {
                     theme: t,
                     isCollapsed: n,
                     adjustTop: r,
                     sidebarWidth: o
@@ -120423,20 +121284,20 @@
                         maxWidth: "none",
                         minWidth: "100%",
                         width: "100% !important",
                         paddingTop: "1rem"
                     }
                 }
             }), ""),
-            Zi = (0, Qe.Z)("div", {
+            Ba = (0, Qe.Z)("div", {
                 target: "eczjsme10"
             })((() => ({
                 position: "relative"
             })), ""),
-            Ji = (0, Qe.Z)("ul", {
+            ja = (0, Qe.Z)("ul", {
                 target: "eczjsme9"
             })((e => {
                 let {
                     isExpanded: t,
                     isOverflowing: n,
                     hasSidebarElements: r,
                     theme: o
@@ -120470,16 +121331,16 @@
                         bottom: 0,
                         left: 0,
                         right: 0,
                         pointerEvents: "none"
                     } : null
                 }
             }), ""),
-            Qi = (0, Oe.F4)(Xi || (Xi = (0, Ki.Z)(["\n  from, to {\n    transform: translateY(0);\n  }\n\n  50% {\n    transform: translateY(-0.25rem);\n  }\n"]))),
-            ea = (0, Qe.Z)("div", {
+            Fa = (0, Oe.F4)(Na || (Na = (0, Pa.Z)(["\n  from, to {\n    transform: translateY(0);\n  }\n\n  50% {\n    transform: translateY(-0.25rem);\n  }\n"]))),
+            Ua = (0, Qe.Z)("div", {
                 target: "eczjsme8"
             })((e => {
                 let {
                     isExpanded: t,
                     isOverflowing: n,
                     theme: r
                 } = e;
@@ -120497,27 +121358,27 @@
                     borderBottom: "1px solid ".concat(r.colors.fadedText10),
                     transition: "color 500ms",
                     ...(t || n) && {
                         "&:hover": {
                             color: r.colors.bodyText,
                             background: "linear-gradient(0deg, ".concat(r.colors.darkenedBgMix15, ", transparent)"),
                             "& > *": {
-                                animation: "".concat(Qi, " 0.5s ease infinite")
+                                animation: "".concat(Fa, " 0.5s ease infinite")
                             }
                         }
                     }
                 }
             }), ""),
-            ta = (0, Qe.Z)("div", {
+            Va = (0, Qe.Z)("div", {
                 target: "eczjsme7"
             })((() => ({
                 display: "flex",
                 flexDirection: "column"
             })), ""),
-            na = (0, Qe.Z)("a", {
+            Ha = (0, Qe.Z)("a", {
                 target: "eczjsme6"
             })((e => {
                 let {
                     isActive: t,
                     theme: n
                 } = e;
                 const r = {
@@ -120552,30 +121413,30 @@
                         backgroundColor: n.colors.darkenedBgMix15
                     },
                     "@media print": {
                         paddingLeft: n.spacing.none
                     }
                 }
             }), ""),
-            ra = (0, Qe.Z)("span", {
+            Xa = (0, Qe.Z)("span", {
                 target: "eczjsme5"
             })((e => {
                 let {
                     isActive: t,
                     theme: n
                 } = e;
                 return {
                     color: t ? n.colors.bodyText : n.colors.fadedText60,
                     overflow: "hidden",
                     whiteSpace: "nowrap",
                     textOverflow: "ellipsis",
                     display: "table-cell"
                 }
             }), ""),
-            oa = (0, Qe.Z)("div", {
+            Ga = (0, Qe.Z)("div", {
                 target: "eczjsme4"
             })((e => {
                 let {
                     hasPageNavAbove: t,
                     theme: n
                 } = e;
                 return {
@@ -120585,28 +121446,28 @@
                     paddingRight: n.spacing.twoXL,
                     "@media print": {
                         paddingTop: "1rem"
                     },
                     ...(0, ye.XE)(n)
                 }
             }), ""),
-            ia = (0, Qe.Z)("div", {
+            $a = (0, Qe.Z)("div", {
                 target: "eczjsme3"
             })((e => {
                 let {
                     hideScrollbar: t
                 } = e;
                 return {
                     position: "relative",
                     height: "100%",
                     width: "100%",
                     overflow: t ? "hidden" : ["auto", "overlay"]
                 }
             }), ""),
-            aa = (0, Qe.Z)("div", {
+            Ka = (0, Qe.Z)("div", {
                 target: "eczjsme2"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     position: "absolute",
@@ -120617,15 +121478,15 @@
                         backgroundColor: (0, _e.DZ)(t.colors.fadedText60, .5)
                     },
                     "@media print": {
                         display: "none"
                     }
                 }
             }), ""),
-            sa = (0, Qe.Z)("div", {
+            Ya = (0, Qe.Z)("div", {
                 target: "eczjsme1"
             })((e => {
                 let {
                     chevronDownshift: t,
                     isCollapsed: n,
                     theme: r
                 } = e;
@@ -120641,15 +121502,15 @@
                         color: r.colors.bodyText
                     },
                     "@media print": {
                         display: "none"
                     }
                 }
             }), ""),
-            la = (0, Qe.Z)("div", {
+            Za = (0, Qe.Z)("div", {
                 target: "eczjsme0"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     position: "absolute",
@@ -120658,69 +121519,69 @@
                     cursor: "col-resize",
                     zIndex: t.zIndices.sidebarMobile,
                     "&:hover": {
                         backgroundImage: "linear-gradient(to right, transparent 20%, ".concat(t.colors.fadedText20, " 28%, transparent 36%)")
                     }
                 }
             }), "");
-        var ca = __webpack_require__(91706),
-            ua = __webpack_require__(88235);
-        const pa = e => {
+        var Ja = __webpack_require__(91706),
+            Qa = __webpack_require__(88235);
+        const es = e => {
             let {
                 endpoints: n,
                 appPages: r,
                 collapseSidebar: o,
                 currentPageScriptHash: i,
                 hasSidebarElements: a,
                 hideParentScrollbar: s,
                 onPageChange: l
             } = e;
             const {
                 pageLinkBaseUrl: c
-            } = t.useContext(je), [u, p] = (0, t.useState)(!1), d = (0, t.useRef)(null), b = (0, ua.d)(d, u), f = (0, t.useCallback)((() => {
+            } = t.useContext(je), [u, p] = (0, t.useState)(!1), d = (0, t.useRef)(null), b = (0, Qa.d)(d, u), f = (0, t.useCallback)((() => {
                 b && s(!0)
             }), [b, s]), h = (0, t.useCallback)((() => s(!1)), [s]), m = (0, t.useCallback)((() => {
                 !u && b ? p(!0) : u && p(!1)
             }), [u, b]);
-            return r.length < 2 ? null : (0, ge.jsxs)(Zi, {
+            return r.length < 2 ? null : (0, ge.jsxs)(Ba, {
                 "data-testid": "stSidebarNav",
-                children: [(0, ge.jsx)(Ji, {
+                children: [(0, ge.jsx)(ja, {
                     ref: d,
                     isExpanded: u,
                     isOverflowing: b,
                     hasSidebarElements: a,
                     onMouseOver: f,
                     onMouseOut: h,
                     "data-testid": "stSidebarNavItems",
                     children: r.map(((e, t) => {
                         const r = n.buildAppPageURL(c, e, t),
                             a = e.pageName,
                             s = a.replace(/_/g, " "),
                             u = e.pageScriptHash === i;
                         return (0, ge.jsx)("li", {
-                            children: (0, ge.jsx)(ta, {
-                                children: (0, ge.jsxs)(na, {
+                            children: (0, ge.jsx)(Va, {
+                                children: (0, ge.jsxs)(Ha, {
                                     "data-testid": "stSidebarNavLink",
                                     isActive: u,
                                     href: r,
                                     onClick: t => {
-                                        t.preventDefault(), l(e.pageScriptHash), ca.tq && o()
+                                        t.preventDefault(), l(e.pageScriptHash), Ja.tq && o()
                                     },
                                     children: [e.icon && e.icon.length && (0, ge.jsx)(hn.S, {
                                         size: "lg",
                                         children: e.icon
-                                    }), (0, ge.jsx)(ra, {
+                                    }), (0, ge.jsx)(Xa, {
                                         isActive: u,
                                         children: s
                                     })]
                                 })
                             })
                         }, a)
                     }))
-                }), a && (0, ge.jsxs)(ea, {
+                }), a && (0, ge.jsxs)(Ua, {
                     "data-testid": "stSidebarNavSeparator",
                     isExpanded: u,
                     isOverflowing: b,
                     onClick: m,
                     children: [b && !u && (0, ge.jsx)(hn.Z, {
                         content: nn,
                         size: "md",
@@ -120729,15 +121590,15 @@
                         content: tn,
                         size: "md",
                         testid: "stSidebarNavCollapseIcon"
                     })]
                 })]
             })
         };
-        class da extends t.PureComponent {
+        class ts extends t.PureComponent {
             static calculateMaxBreakpoint(e) {
                 return parseInt(e, 10) - .02
             }
             constructor(e) {
                 super(e), this.mediumBreakpointPx = void 0, this.sidebarRef = t.createRef(), this.handleClickOutside = e => {
                     if (this.sidebarRef && window) {
                         const {
@@ -120749,19 +121610,19 @@
                             collapsedSidebar: !0
                         })
                     }
                 }, this.setSidebarWidth = e => {
                     const t = e.toString();
                     this.setState({
                         sidebarWidth: t
-                    }), (0, $i.V)() && window.localStorage.setItem("sidebarWidth", t)
+                    }), (0, Ia.V)() && window.localStorage.setItem("sidebarWidth", t)
                 }, this.resetSidebarWidth = e => {
                     2 === e.detail && (this.setState({
-                        sidebarWidth: da.minWidth
-                    }), (0, $i.V)() && window.localStorage.setItem("sidebarWidth", da.minWidth))
+                        sidebarWidth: ts.minWidth
+                    }), (0, Ia.V)() && window.localStorage.setItem("sidebarWidth", ts.minWidth))
                 }, this.checkMobileOnResize = () => {
                     if (!window) return !1;
                     const {
                         innerWidth: e
                     } = window;
                     return e < this.state.lastInnerWidth && e <= this.mediumBreakpointPx && this.setState({
                         collapsedSidebar: !0
@@ -120775,26 +121636,26 @@
                     this.setState({
                         collapsedSidebar: !e
                     })
                 }, this.hideScrollbar = e => {
                     this.setState({
                         hideScrollbar: e
                     })
-                }, this.mediumBreakpointPx = da.calculateMaxBreakpoint(e.theme.breakpoints.md);
-                const n = (0, $i.V)() ? localStorage.getItem("sidebarWidth") : void 0;
+                }, this.mediumBreakpointPx = ts.calculateMaxBreakpoint(e.theme.breakpoints.md);
+                const n = (0, Ia.V)() ? localStorage.getItem("sidebarWidth") : void 0;
                 this.state = {
-                    collapsedSidebar: da.shouldCollapse(e, this.mediumBreakpointPx),
-                    sidebarWidth: n || da.minWidth,
+                    collapsedSidebar: ts.shouldCollapse(e, this.mediumBreakpointPx),
+                    sidebarWidth: n || ts.minWidth,
                     lastInnerWidth: window ? window.innerWidth : 1 / 0,
                     hideScrollbar: !1
                 }
             }
             componentDidUpdate(e) {
-                this.mediumBreakpointPx = da.calculateMaxBreakpoint(this.props.theme.breakpoints.md), this.props.initialSidebarState === e.initialSidebarState && this.props.hasElements === e.hasElements || this.setState({
-                    collapsedSidebar: da.shouldCollapse(this.props, this.mediumBreakpointPx)
+                this.mediumBreakpointPx = ts.calculateMaxBreakpoint(this.props.theme.breakpoints.md), this.props.initialSidebarState === e.initialSidebarState && this.props.hasElements === e.hasElements || this.setState({
+                    collapsedSidebar: ts.shouldCollapse(this.props, this.mediumBreakpointPx)
                 })
             }
             static shouldCollapse(e, t) {
                 switch (e.initialSidebarState) {
                     case Be.Pz.SidebarState.EXPANDED:
                         return !1;
                     case Be.Pz.SidebarState.COLLAPSED:
@@ -120834,27 +121695,27 @@
                     children: i,
                     hasElements: a,
                     onPageChange: s,
                     currentPageScriptHash: l,
                     hideSidebarNav: c
                 } = this.props, u = r.length > 1 && !c, p = !((0, He.P2)() && !(0, He.av)()) && this.headerDecorationVisible();
                 return (0, ge.jsxs)(ge.Fragment, {
-                    children: [e && (0, ge.jsx)(sa, {
+                    children: [e && (0, ge.jsx)(Ya, {
                         chevronDownshift: o,
                         isCollapsed: e,
                         "data-testid": "collapsedControl",
                         children: (0, ge.jsx)(an.ZP, {
                             kind: sn.nW.HEADER_NO_PADDING,
                             onClick: this.toggleCollapse,
                             children: (0, ge.jsx)(hn.Z, {
-                                content: Vi._,
+                                content: Ca._,
                                 size: "lg"
                             })
                         })
-                    }), (0, ge.jsx)(Gi.e, {
+                    }), (0, ge.jsx)(La.e, {
                         "data-testid": "stSidebar",
                         "aria-expanded": !e,
                         enable: {
                             top: !1,
                             right: !0,
                             bottom: !1,
                             left: !1
@@ -120862,111 +121723,111 @@
                         handleStyles: {
                             right: {
                                 width: "8px",
                                 right: "-6px"
                             }
                         },
                         handleComponent: {
-                            right: (0, ge.jsx)(la, {
+                            right: (0, ge.jsx)(Za, {
                                 onClick: this.resetSidebarWidth
                             })
                         },
                         size: {
                             width: t,
                             height: p ? window.innerHeight - 2 : "100%"
                         },
-                        as: Yi,
+                        as: Da,
                         onResizeStop: (e, n, r, o) => {
                             const i = parseInt(t, 10) + o.width;
                             this.setSidebarWidth(i)
                         },
                         isCollapsed: e,
                         adjustTop: p,
                         sidebarWidth: t,
-                        children: (0, ge.jsxs)(ia, {
+                        children: (0, ge.jsxs)($a, {
                             "data-testid": "stSidebarContent",
                             hideScrollbar: n,
                             ref: this.sidebarRef,
-                            children: [(0, ge.jsx)(aa, {
+                            children: [(0, ge.jsx)(Ka, {
                                 children: (0, ge.jsx)(an.ZP, {
                                     kind: sn.nW.HEADER_BUTTON,
                                     onClick: this.toggleCollapse,
                                     children: (0, ge.jsx)(hn.Z, {
-                                        content: Hi,
+                                        content: Wa,
                                         size: "lg"
                                     })
                                 })
-                            }), !c && (0, ge.jsx)(pa, {
+                            }), !c && (0, ge.jsx)(es, {
                                 endpoints: this.props.endpoints,
                                 appPages: r,
                                 collapseSidebar: this.toggleCollapse,
                                 currentPageScriptHash: l,
                                 hasSidebarElements: a,
                                 hideParentScrollbar: this.hideScrollbar,
                                 onPageChange: s
-                            }), (0, ge.jsx)(oa, {
+                            }), (0, ge.jsx)(Ga, {
                                 "data-testid": "stSidebarUserContent",
                                 hasPageNavAbove: u,
                                 children: i
                             })]
                         })
                     })]
                 })
             }
         }
-        da.minWidth = "336";
-        const ba = (0, Ee.b)((function(e) {
+        ts.minWidth = "336";
+        const ns = (0, Ee.b)((function(e) {
                 return (0, ge.jsx)(ln.Z.Provider, {
                     value: !0,
-                    children: (0, ge.jsx)(da, {
+                    children: (0, ge.jsx)(ts, {
                         ...e
                     })
                 })
             })),
-            fa = e => {
+            rs = e => {
                 let {
                     children: n,
                     ...r
                 } = e;
                 const {
                     sidebarChevronDownshift: o
                 } = t.useContext(je), {
                     activeTheme: i
                 } = t.useContext(Fe.E), a = (e => (0, ye.jG)("Sidebar", {
                     secondaryBackgroundColor: e.emotion.colors.bgColor,
                     backgroundColor: e.emotion.colors.secondaryBg,
                     bodyFont: e.emotion.genericFonts.bodyFont,
                     codeFont: e.emotion.genericFonts.codeFont
                 }, e, !0))(i);
-                return (0, ge.jsx)(Ui, {
+                return (0, ge.jsx)(ka, {
                     theme: a.emotion,
                     baseuiTheme: a.basewebTheme,
-                    children: (0, ge.jsx)(ba, {
+                    children: (0, ge.jsx)(ns, {
                         ...r,
                         chevronDownshift: o,
                         children: n
                     })
                 })
             };
-        var ha = __webpack_require__(69021),
-            ma = __webpack_require__(92775);
-        const Ma = function(e) {
+        var os = __webpack_require__(69021),
+            is = __webpack_require__(92775);
+        const as = function(e) {
                 let {
                     scriptRunId: n,
                     children: r
                 } = e;
                 const {
                     sizes: o
                 } = (0, Ee.u)();
                 return (0, t.useEffect)((() => {
                     var e;
-                    null === (e = ha.Z.getRef()) || void 0 === e || e.clearAll()
+                    null === (e = os.Z.getRef()) || void 0 === e || e.clearAll()
                 }), [n]), (0, ge.jsxs)(ge.Fragment, {
-                    children: [(0, ge.jsx)(ha.w, {
-                        placement: ma.r4.topRight,
+                    children: [(0, ge.jsx)(os.w, {
+                        placement: is.r4.topRight,
                         autoHideDuration: 4e3,
                         overrides: {
                             Root: {
                                 style: {
                                     top: o.headerHeight,
                                     zIndex: 100
                                 },
@@ -120974,15 +121835,15 @@
                                     "data-testid": "toastContainer"
                                 }
                             }
                         }
                     }), r]
                 })
             },
-            Oa = (0, Qe.Z)("div", {
+            ss = (0, Qe.Z)("div", {
                 target: "ea3mdgi9"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     display: "flex",
@@ -121001,15 +121862,15 @@
                         float: "none",
                         height: t.sizes.full,
                         position: "static",
                         overflow: "visible"
                     }
                 }
             }), ""),
-            ga = (0, Qe.Z)("section", {
+            ls = (0, Qe.Z)("section", {
                 target: "ea3mdgi8"
             })((e => {
                 let {
                     disableScrolling: t,
                     theme: n
                 } = e;
                 return {
@@ -121030,23 +121891,23 @@
                     },
                     "@media print": {
                         position: "relative",
                         display: "block"
                     }
                 }
             }), ""),
-            za = (0, Qe.Z)("div", {
+            cs = (0, Qe.Z)("div", {
                 target: "ea3mdgi7"
             })((() => ({
                 position: "sticky",
                 left: 0,
                 bottom: 0,
                 width: "100%"
             })), ""),
-            ya = (0, Qe.Z)("div", {
+            us = (0, Qe.Z)("div", {
                 target: "ea3mdgi6"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     position: "relative",
@@ -121056,15 +121917,15 @@
                     backgroundColor: t.colors.bgColor,
                     display: "flex",
                     flexDirection: "column",
                     alignItems: "center",
                     zIndex: t.zIndices.bottom
                 }
             }), ""),
-            Aa = (0, Qe.Z)("div", {
+            ps = (0, Qe.Z)("div", {
                 target: "ea3mdgi5"
             })((e => {
                 let {
                     hasSidebar: t,
                     hasBottom: n,
                     isEmbedded: r,
                     isWideMode: o,
@@ -121096,30 +121957,30 @@
                     ...d,
                     "@media print": {
                         minWidth: "100%",
                         paddingTop: 0
                     }
                 }
             }), ""),
-            va = (0, Qe.Z)("div", {
+            ds = (0, Qe.Z)("div", {
                 target: "ea3mdgi4"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     width: t.sizes.full
                 }
             }), ""),
-            wa = (0, Qe.Z)("div", {
+            bs = (0, Qe.Z)("div", {
                 target: "ea3mdgi3"
             })((() => ({
                 display: "none"
             })), ""),
-            Sa = (0, Qe.Z)("div", {
+            fs = (0, Qe.Z)("div", {
                 target: "ea3mdgi2"
             })((e => {
                 let {
                     isWideMode: t,
                     showPadding: n,
                     theme: r
                 } = e;
@@ -121138,51 +121999,51 @@
                     maxWidth: t ? "initial" : r.sizes.contentMaxWidth,
                     "@media print": {
                         minWidth: "100%",
                         paddingTop: 0
                     }
                 }
             }), ""),
-            qa = (0, Qe.Z)("div", {
+            hs = (0, Qe.Z)("div", {
                 target: "ea3mdgi1"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     width: t.sizes.full,
                     flexGrow: 1
                 }
             }), ""),
-            Ea = (0, Qe.Z)("div", {
+            ms = (0, Qe.Z)("div", {
                 target: "ea3mdgi0"
             })((() => ({
                 position: "relative",
                 bottom: "0"
             })), "");
 
-        function _a(e) {
+        function Ms(e) {
             const {
                 className: t,
                 tabIndex: n,
                 children: r,
                 isEmbedded: o,
                 disableScrolling: i
-            } = e, a = Fn();
-            return (0, ge.jsx)(ga, {
+            } = e, a = Tr();
+            return (0, ge.jsx)(ls, {
                 tabIndex: n,
                 className: t,
                 isEmbedded: o,
                 disableScrolling: i,
                 ref: a,
                 "data-testid": "ScrollToBottomContainer",
                 children: r
             })
         }
-        const xa = function(e) {
+        const Os = function(e) {
             const {
                 elements: n,
                 sessionInfo: r,
                 scriptRunId: o,
                 scriptRunState: i,
                 widgetMgr: a,
                 widgetsDisabled: s,
@@ -121208,145 +122069,143 @@
             const {
                 wideMode: M,
                 initialSidebarState: O,
                 embedded: g,
                 showPadding: z,
                 disableScrolling: y,
                 showToolbar: A,
-                showColoredLine: v,
-                toastAdjustment: w
+                showColoredLine: v
             } = t.useContext(je), {
-                addScriptFinishedHandler: S,
-                removeScriptFinishedHandler: q,
-                libConfig: E
-            } = t.useContext(Fe.E), _ = M ? "wide" : "narrow", x = !n.sidebar.isEmpty, R = !n.event.isEmpty, T = !n.bottom.isEmpty, [k, C] = t.useState(!1), W = x || !f && p.length > 1 || k;
+                addScriptFinishedHandler: w,
+                removeScriptFinishedHandler: S,
+                libConfig: q
+            } = t.useContext(Fe.E), E = M ? "wide" : "narrow", _ = !n.sidebar.isEmpty, x = !n.event.isEmpty, R = !n.bottom.isEmpty, [T, k] = t.useState(!1), C = _ || !f && p.length > 1 || T;
             t.useEffect((() => {
-                W && f && !k && C(!0)
-            }), [W, f, k]);
-            const N = t.useCallback((() => {
-                !x && k && C(!1)
-            }), [x, k]);
-            t.useEffect((() => (S(N), () => {
-                q(N)
-            })), [N, S, q]);
-            const L = T ? _a : ga,
-                I = e => (0, ge.jsx)(ji, {
+                C && f && !T && k(!0)
+            }), [C, f, T]);
+            const W = t.useCallback((() => {
+                !_ && T && k(!1)
+            }), [_, T]);
+            t.useEffect((() => (w(W), () => {
+                S(W)
+            })), [W, w, S]);
+            const N = R ? Ms : ls,
+                L = e => (0, ge.jsx)(Ra, {
                     node: e,
                     endpoints: m,
                     sessionInfo: r,
                     scriptRunId: o,
                     scriptRunState: i,
                     widgetMgr: a,
                     widgetsDisabled: s,
                     uploadClient: l,
                     componentRegistry: c,
                     formsData: u
                 });
-            return (0, ge.jsxs)(Oa, {
+            return (0, ge.jsxs)(ss, {
                 className: "appview-container",
                 "data-testid": "stAppViewContainer",
-                "data-layout": _,
-                children: [W && (0, ge.jsx)(fa, {
+                "data-layout": E,
+                children: [C && (0, ge.jsx)(rs, {
                     endpoints: m,
                     initialSidebarState: O,
                     appPages: p,
-                    hasElements: x,
+                    hasElements: _,
                     onPageChange: d,
                     currentPageScriptHash: b,
                     hideSidebarNav: f,
-                    children: (0, ge.jsx)(va, {
-                        children: I(n.sidebar)
+                    children: (0, ge.jsx)(ds, {
+                        children: L(n.sidebar)
                     })
-                }), (0, ge.jsxs)(L, {
+                }), (0, ge.jsxs)(N, {
                     tabIndex: 0,
                     isEmbedded: g,
                     disableScrolling: y,
                     className: "main",
-                    children: [(0, ge.jsx)(Aa, {
+                    children: [(0, ge.jsx)(ps, {
                         className: "block-container",
                         "data-testid": "stAppViewBlockContainer",
                         isWideMode: M,
                         showPadding: z,
                         addPaddingForHeader: A || v,
-                        hasBottom: T,
+                        hasBottom: R,
                         isEmbedded: g,
-                        hasSidebar: W,
-                        disableFullscreenMode: Boolean(E.disableFullscreenMode),
-                        children: I(n.main)
-                    }), !T && (0, ge.jsx)(Ea, {
+                        hasSidebar: C,
+                        disableFullscreenMode: Boolean(q.disableFullscreenMode),
+                        children: L(n.main)
+                    }), !R && (0, ge.jsx)(ms, {
                         "data-testid": "IframeResizerAnchor",
                         "data-iframe-height": !0
-                    }), T && (0, ge.jsxs)(ge.Fragment, {
-                        children: [(0, ge.jsx)(qa, {}), (0, ge.jsx)(za, {
+                    }), R && (0, ge.jsxs)(ge.Fragment, {
+                        children: [(0, ge.jsx)(hs, {}), (0, ge.jsx)(cs, {
                             "data-testid": "stBottom",
-                            children: (0, ge.jsx)(ya, {
-                                children: (0, ge.jsx)(Sa, {
+                            children: (0, ge.jsx)(us, {
+                                children: (0, ge.jsx)(fs, {
                                     "data-testid": "stBottomBlockContainer",
                                     isWideMode: M,
                                     showPadding: z,
-                                    children: I(n.bottom)
+                                    children: L(n.bottom)
                                 })
                             })
                         })]
                     })]
-                }), R && (0, ge.jsx)(Ma, {
-                    toastAdjustment: w,
+                }), x && (0, ge.jsx)(as, {
                     scriptRunId: n.event.scriptRunId,
-                    children: (0, ge.jsx)(wa, {
-                        children: I(n.event)
+                    children: (0, ge.jsx)(bs, {
+                        children: L(n.event)
                     })
                 })]
             })
         };
-        var Ra = t.forwardRef((function(e, n) {
+        var gs = t.forwardRef((function(e, n) {
             return t.createElement(en.D, (0, Qt.Z)({
                 iconAttrs: {
                     fill: "currentColor",
                     xmlns: "http://www.w3.org/2000/svg"
                 },
                 iconVerticalAlign: "middle",
                 iconViewBox: "0 0 8 8"
             }, e, {
                 ref: n
             }), t.createElement("path", {
                 d: "M5 0c-.55 0-1 .45-1 1s.45 1 1 1 1-.45 1-1-.45-1-1-1zM3.5 2.5C2.67 2.5 2 3.17 2 4h1c0-.28.22-.5.5-.5s.5.22.5.5-1 1.64-1 2.5C3 7.36 3.67 8 4.5 8S6 7.33 6 6.5H5c0 .28-.22.5-.5.5S4 6.78 4 6.5C4 6.14 5 4.66 5 4c0-.81-.67-1.5-1.5-1.5z"
             }))
         }));
-        Ra.displayName = "Info";
-        var Ta = t.forwardRef((function(e, n) {
+        gs.displayName = "Info";
+        var zs = t.forwardRef((function(e, n) {
             return t.createElement(en.D, (0, Qt.Z)({
                 iconAttrs: {
                     fill: "currentColor",
                     xmlns: "http://www.w3.org/2000/svg"
                 },
                 iconVerticalAlign: "middle",
                 iconViewBox: "0 0 8 8"
             }, e, {
                 ref: n
             }), t.createElement("path", {
                 d: "M0 3v2h2V3H0zm3 0v2h2V3H3zm3 0v2h2V3H6z"
             }))
         }));
-        Ta.displayName = "Ellipses";
-        var ka = t.forwardRef((function(e, n) {
+        zs.displayName = "Ellipses";
+        var ys = t.forwardRef((function(e, n) {
             return t.createElement(en.D, (0, Qt.Z)({
                 iconAttrs: {
                     fill: "currentColor",
                     xmlns: "http://www.w3.org/2000/svg"
                 },
                 iconVerticalAlign: "middle",
                 iconViewBox: "0 0 8 8"
             }, e, {
                 ref: n
             }), t.createElement("path", {
                 d: "M3.09 0c-.06 0-.1.04-.13.09L.02 6.9c-.02.05-.03.13-.03.19v.81c0 .05.04.09.09.09h6.81c.05 0 .09-.04.09-.09v-.81c0-.05-.01-.14-.03-.19L4.01.09A.142.142 0 003.88 0h-.81zM3 3h1v2H3V3zm0 3h1v1H3V6z"
             }))
         }));
-        ka.displayName = "Warning";
-        class Ca {
+        ys.displayName = "Warning";
+        class As {
             constructor() {
                 this.timerHandle = void 0, this.duration = 0, this.startTime = 0, this.running = !1
             }
             get isRunning() {
                 return this.running
             }
             get remainingTime() {
@@ -121359,116 +122218,116 @@
                     this.running = !1, e()
                 }), t)
             }
             cancel() {
                 void 0 !== this.timerHandle && (window.clearTimeout(this.timerHandle), this.timerHandle = void 0, this.running = !1)
             }
         }
-        var Wa = __webpack_require__(68785),
-            Na = __webpack_require__(30808),
-            La = __webpack_require__(93219);
+        var vs = __webpack_require__(68785),
+            ws = __webpack_require__(30808),
+            Ss = __webpack_require__(93219);
 
-        function Ia(e, t) {
+        function qs(e, t) {
             return e.replace(new RegExp("(^|\\s)" + t + "(?:\\s|$)", "g"), "$1").replace(/\s+/g, " ").replace(/^\s*|\s*$/g, "")
         }
-        const Pa = !1,
-            Da = t.createContext(null);
-        var Ba = function(e) {
+        const Es = !1,
+            _s = t.createContext(null);
+        var xs = function(e) {
                 return e.scrollTop
             },
-            ja = "unmounted",
-            Fa = "exited",
-            Ua = "entering",
-            Va = "entered",
-            Ha = "exiting",
-            Xa = function(e) {
+            Rs = "unmounted",
+            Ts = "exited",
+            ks = "entering",
+            Cs = "entered",
+            Ws = "exiting",
+            Ns = function(e) {
                 function r(t, n) {
                     var r;
                     r = e.call(this, t, n) || this;
                     var o, i = n && !n.isMounting ? t.enter : t.appear;
-                    return r.appearStatus = null, t.in ? i ? (o = Fa, r.appearStatus = Ua) : o = Va : o = t.unmountOnExit || t.mountOnEnter ? ja : Fa, r.state = {
+                    return r.appearStatus = null, t.in ? i ? (o = Ts, r.appearStatus = ks) : o = Cs : o = t.unmountOnExit || t.mountOnEnter ? Rs : Ts, r.state = {
                         status: o
                     }, r.nextCallback = null, r
-                }(0, La.Z)(r, e), r.getDerivedStateFromProps = function(e, t) {
-                    return e.in && t.status === ja ? {
-                        status: Fa
+                }(0, Ss.Z)(r, e), r.getDerivedStateFromProps = function(e, t) {
+                    return e.in && t.status === Rs ? {
+                        status: Ts
                     } : null
                 };
                 var o = r.prototype;
                 return o.componentDidMount = function() {
                     this.updateStatus(!0, this.appearStatus)
                 }, o.componentDidUpdate = function(e) {
                     var t = null;
                     if (e !== this.props) {
                         var n = this.state.status;
-                        this.props.in ? n !== Ua && n !== Va && (t = Ua) : n !== Ua && n !== Va || (t = Ha)
+                        this.props.in ? n !== ks && n !== Cs && (t = ks) : n !== ks && n !== Cs || (t = Ws)
                     }
                     this.updateStatus(!1, t)
                 }, o.componentWillUnmount = function() {
                     this.cancelNextCallback()
                 }, o.getTimeouts = function() {
                     var e, t, n, r = this.props.timeout;
                     return e = t = n = r, null != r && "number" !== typeof r && (e = r.exit, t = r.enter, n = void 0 !== r.appear ? r.appear : t), {
                         exit: e,
                         enter: t,
                         appear: n
                     }
                 }, o.updateStatus = function(e, t) {
                     if (void 0 === e && (e = !1), null !== t)
-                        if (this.cancelNextCallback(), t === Ua) {
+                        if (this.cancelNextCallback(), t === ks) {
                             if (this.props.unmountOnExit || this.props.mountOnEnter) {
                                 var r = this.props.nodeRef ? this.props.nodeRef.current : n.findDOMNode(this);
-                                r && Ba(r)
+                                r && xs(r)
                             }
                             this.performEnter(e)
                         } else this.performExit();
-                    else this.props.unmountOnExit && this.state.status === Fa && this.setState({
-                        status: ja
+                    else this.props.unmountOnExit && this.state.status === Ts && this.setState({
+                        status: Rs
                     })
                 }, o.performEnter = function(e) {
                     var t = this,
                         r = this.props.enter,
                         o = this.context ? this.context.isMounting : e,
                         i = this.props.nodeRef ? [o] : [n.findDOMNode(this), o],
                         a = i[0],
                         s = i[1],
                         l = this.getTimeouts(),
                         c = o ? l.appear : l.enter;
-                    !e && !r || Pa ? this.safeSetState({
-                        status: Va
+                    !e && !r || Es ? this.safeSetState({
+                        status: Cs
                     }, (function() {
                         t.props.onEntered(a)
                     })) : (this.props.onEnter(a, s), this.safeSetState({
-                        status: Ua
+                        status: ks
                     }, (function() {
                         t.props.onEntering(a, s), t.onTransitionEnd(c, (function() {
                             t.safeSetState({
-                                status: Va
+                                status: Cs
                             }, (function() {
                                 t.props.onEntered(a, s)
                             }))
                         }))
                     })))
                 }, o.performExit = function() {
                     var e = this,
                         t = this.props.exit,
                         r = this.getTimeouts(),
                         o = this.props.nodeRef ? void 0 : n.findDOMNode(this);
-                    t && !Pa ? (this.props.onExit(o), this.safeSetState({
-                        status: Ha
+                    t && !Es ? (this.props.onExit(o), this.safeSetState({
+                        status: Ws
                     }, (function() {
                         e.props.onExiting(o), e.onTransitionEnd(r.exit, (function() {
                             e.safeSetState({
-                                status: Fa
+                                status: Ts
                             }, (function() {
                                 e.props.onExited(o)
                             }))
                         }))
                     }))) : this.safeSetState({
-                        status: Fa
+                        status: Ts
                     }, (function() {
                         e.props.onExited(o)
                     }))
                 }, o.cancelNextCallback = function() {
                     null !== this.nextCallback && (this.nextCallback.cancel(), this.nextCallback = null)
                 }, o.safeSetState = function(e, t) {
                     t = this.setNextCallback(t), this.setState(e, t)
@@ -121491,47 +122350,47 @@
                                 s = i[1];
                             this.props.addEndListener(a, s)
                         }
                         null != e && setTimeout(this.nextCallback, e)
                     } else setTimeout(this.nextCallback, 0)
                 }, o.render = function() {
                     var e = this.state.status;
-                    if (e === ja) return null;
+                    if (e === Rs) return null;
                     var n = this.props,
                         r = n.children,
-                        o = (n.in, n.mountOnEnter, n.unmountOnExit, n.appear, n.enter, n.exit, n.timeout, n.addEndListener, n.onEnter, n.onEntering, n.onEntered, n.onExit, n.onExiting, n.onExited, n.nodeRef, (0, Na.Z)(n, ["children", "in", "mountOnEnter", "unmountOnExit", "appear", "enter", "exit", "timeout", "addEndListener", "onEnter", "onEntering", "onEntered", "onExit", "onExiting", "onExited", "nodeRef"]));
-                    return t.createElement(Da.Provider, {
+                        o = (n.in, n.mountOnEnter, n.unmountOnExit, n.appear, n.enter, n.exit, n.timeout, n.addEndListener, n.onEnter, n.onEntering, n.onEntered, n.onExit, n.onExiting, n.onExited, n.nodeRef, (0, ws.Z)(n, ["children", "in", "mountOnEnter", "unmountOnExit", "appear", "enter", "exit", "timeout", "addEndListener", "onEnter", "onEntering", "onEntered", "onExit", "onExiting", "onExited", "nodeRef"]));
+                    return t.createElement(_s.Provider, {
                         value: null
                     }, "function" === typeof r ? r(e, o) : t.cloneElement(t.Children.only(r), o))
                 }, r
             }(t.Component);
 
-        function Ga() {}
-        Xa.contextType = Da, Xa.propTypes = {}, Xa.defaultProps = {
+        function Ls() {}
+        Ns.contextType = _s, Ns.propTypes = {}, Ns.defaultProps = {
             in: !1,
             mountOnEnter: !1,
             unmountOnExit: !1,
             appear: !1,
             enter: !0,
             exit: !0,
-            onEnter: Ga,
-            onEntering: Ga,
-            onEntered: Ga,
-            onExit: Ga,
-            onExiting: Ga,
-            onExited: Ga
-        }, Xa.UNMOUNTED = ja, Xa.EXITED = Fa, Xa.ENTERING = Ua, Xa.ENTERED = Va, Xa.EXITING = Ha;
-        const $a = Xa;
-        var Ka = function(e, t) {
+            onEnter: Ls,
+            onEntering: Ls,
+            onEntered: Ls,
+            onExit: Ls,
+            onExiting: Ls,
+            onExited: Ls
+        }, Ns.UNMOUNTED = Rs, Ns.EXITED = Ts, Ns.ENTERING = ks, Ns.ENTERED = Cs, Ns.EXITING = Ws;
+        const Is = Ns;
+        var Ps = function(e, t) {
                 return e && t && t.split(" ").forEach((function(t) {
-                    return r = t, void((n = e).classList ? n.classList.remove(r) : "string" === typeof n.className ? n.className = Ia(n.className, r) : n.setAttribute("class", Ia(n.className && n.className.baseVal || "", r)));
+                    return r = t, void((n = e).classList ? n.classList.remove(r) : "string" === typeof n.className ? n.className = qs(n.className, r) : n.setAttribute("class", qs(n.className && n.className.baseVal || "", r)));
                     var n, r
                 }))
             },
-            Ya = function(e) {
+            Ds = function(e) {
                 function n() {
                     for (var t, n = arguments.length, r = new Array(n), o = 0; o < n; o++) r[o] = arguments[o];
                     return (t = e.call.apply(e, [this].concat(r)) || this).appliedClasses = {
                         appear: {},
                         enter: {},
                         exit: {}
                     }, t.onEnter = function(e, n) {
@@ -121566,69 +122425,69 @@
                             o = r ? "" + (r && n ? n + "-" : "") + e : n[e];
                         return {
                             baseClassName: o,
                             activeClassName: r ? o + "-active" : n[e + "Active"],
                             doneClassName: r ? o + "-done" : n[e + "Done"]
                         }
                     }, t
-                }(0, La.Z)(n, e);
+                }(0, Ss.Z)(n, e);
                 var r = n.prototype;
                 return r.addClass = function(e, t, n) {
                     var r = this.getClassNames(t)[n + "ClassName"],
                         o = this.getClassNames("enter").doneClassName;
-                    "appear" === t && "done" === n && o && (r += " " + o), "active" === n && e && Ba(e), r && (this.appliedClasses[t][n] = r, function(e, t) {
+                    "appear" === t && "done" === n && o && (r += " " + o), "active" === n && e && xs(e), r && (this.appliedClasses[t][n] = r, function(e, t) {
                         e && t && t.split(" ").forEach((function(t) {
                             return r = t, void((n = e).classList ? n.classList.add(r) : function(e, t) {
                                 return e.classList ? !!t && e.classList.contains(t) : -1 !== (" " + (e.className.baseVal || e.className) + " ").indexOf(" " + t + " ")
                             }(n, r) || ("string" === typeof n.className ? n.className = n.className + " " + r : n.setAttribute("class", (n.className && n.className.baseVal || "") + " " + r)));
                             var n, r
                         }))
                     }(e, r))
                 }, r.removeClasses = function(e, t) {
                     var n = this.appliedClasses[t],
                         r = n.base,
                         o = n.active,
                         i = n.done;
-                    this.appliedClasses[t] = {}, r && Ka(e, r), o && Ka(e, o), i && Ka(e, i)
+                    this.appliedClasses[t] = {}, r && Ps(e, r), o && Ps(e, o), i && Ps(e, i)
                 }, r.render = function() {
                     var e = this.props,
-                        n = (e.classNames, (0, Na.Z)(e, ["classNames"]));
-                    return t.createElement($a, (0, Qt.Z)({}, n, {
+                        n = (e.classNames, (0, ws.Z)(e, ["classNames"]));
+                    return t.createElement(Is, (0, Qt.Z)({}, n, {
                         onEnter: this.onEnter,
                         onEntered: this.onEntered,
                         onEntering: this.onEntering,
                         onExit: this.onExit,
                         onExiting: this.onExiting,
                         onExited: this.onExited
                     }))
                 }, n
             }(t.Component);
-        Ya.defaultProps = {
+        Ds.defaultProps = {
             classNames: ""
-        }, Ya.propTypes = {};
-        const Za = Ya;
-        let Ja;
+        }, Ds.propTypes = {};
+        const Bs = Ds;
+        let js;
         ! function(e) {
             e.CONNECTED = "CONNECTED", e.DISCONNECTED_FOREVER = "DISCONNECTED_FOREVER", e.INITIAL = "INITIAL", e.PINGING_SERVER = "PINGING_SERVER", e.CONNECTING = "CONNECTING"
-        }(Ja || (Ja = {}));
-        const Qa = __webpack_require__.p + "static/media/fireworks.0906f02ea43f1018a6d2.gif",
-            es = (0, Qe.Z)("div", {
+        }(js || (js = {}));
+        const Fs = __webpack_require__.p + "static/media/fireworks.0906f02ea43f1018a6d2.gif",
+            Us = (0, Qe.Z)("div", {
                 target: "en6cib67"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     display: "flex",
                     alignItems: "center",
                     justifyContent: "center",
                     color: t.colors.gray
                 }
             }), ""),
-            ts = (0, Qe.Z)("label", {
+            Vs = (0, Qe.Z)("label", {
                 target: "en6cib66"
             })((e => {
                 let {
                     isMinimized: t,
                     theme: n
                 } = e;
                 return {
@@ -121643,15 +122502,15 @@
                     maxWidth: t ? "0" : "20rem",
                     transition: "opacity 500ms 0ms, clip 500ms 0ms, max-width 500ms 0ms, margin 500ms 0ms, visibility 0ms 500ms",
                     opacity: t ? 0 : 1,
                     visibility: t ? "hidden" : "visible",
                     lineHeight: 1
                 }
             }), ""),
-            ns = (0, Qe.Z)("div", {
+            Hs = (0, Qe.Z)("div", {
                 target: "en6cib65"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     display: "flex",
@@ -121659,23 +122518,23 @@
                     justifyContent: "center",
                     borderRadius: t.radii.md,
                     margin: "0 ".concat(t.spacing.sm, " 0 0"),
                     paddingLeft: t.spacing.sm,
                     height: "1.6rem"
                 }
             }), ""),
-            rs = e => ({
+            Xs = e => ({
                 opacity: 0,
                 padding: e.spacing.none,
                 margin: e.spacing.none,
                 maxWidth: 0,
                 minWidth: 0,
                 border: 0
             }),
-            os = (0, Qe.Z)("label", {
+            Gs = (0, Qe.Z)("label", {
                 target: "en6cib64"
             })((e => {
                 let {
                     isPrompt: t,
                     isMinimized: n,
                     theme: r
                 } = e;
@@ -121684,32 +122543,32 @@
                     color: t ? r.colors.bodyText : r.colors.gray,
                     textTransform: t ? "none" : "uppercase",
                     margin: "0 0 0 ".concat(r.spacing.lg),
                     whiteSpace: "nowrap",
                     maxWidth: "20rem",
                     borderRadius: t ? r.radii.md : void 0,
                     transition: "opacity 200ms ease-out 0s,\n  clip 200ms ease-out 0s, min-width 200ms ease-out 0s,\n  max-width 200ms ease-out 0s, padding 200ms ease-out 0s",
-                    ...n ? rs(r) : {}
+                    ...n ? Xs(r) : {}
                 }
             }), ""),
-            is = (0, Qe.Z)("span", {
+            $s = (0, Qe.Z)("span", {
                 target: "en6cib63"
             })((e => {
                 let {
                     isMinimized: t,
                     theme: n
                 } = e;
                 return {
                     marginLeft: n.spacing.sm,
                     whiteSpace: "nowrap",
                     transition: "opacity 200ms ease-out 0s,\n  clip 200ms ease-out 0s, min-width 200ms ease-out 0s,\n  max-width 200ms ease-out 0s, padding 200ms ease-out 0s",
-                    ...t ? rs(n) : {}
+                    ...t ? Xs(n) : {}
                 }
             }), ""),
-            as = (0, Qe.Z)("img", {
+            Ks = (0, Qe.Z)("img", {
                 target: "en6cib62"
             })((e => {
                 let {
                     isNewYears: t,
                     theme: n
                 } = e;
                 const r = (0, ye.Iy)(n) ? "" : "invert(1)";
@@ -121717,15 +122576,15 @@
                     opacity: t ? 1 : .4,
                     width: t ? "2.2rem" : "1.6rem",
                     height: t ? "2.2rem" : "1.6rem",
                     marginRight: "-".concat(n.spacing.sm),
                     filter: t ? "" : r
                 }
             }), ""),
-            ss = (0, Qe.Z)("div", {
+            Ys = (0, Qe.Z)("div", {
                 target: "en6cib61"
             })((() => ({
                 "&.StatusWidget-appear": {
                     opacity: 0
                 },
                 "&.StatusWidget-appear-active": {
                     opacity: 1,
@@ -121742,26 +122601,26 @@
                     opacity: 1
                 },
                 "&.StatusWidget-exit-active": {
                     opacity: 0,
                     transition: "opacity 200ms ease-out"
                 }
             })), ""),
-            ls = (0, Qe.Z)("div", {
+            Zs = (0, Qe.Z)("div", {
                 target: "en6cib60"
             })((() => ({
                 "&::first-letter": {
                     textDecoration: "underline"
                 }
             })), "");
-        class cs extends t.PureComponent {
+        class Js extends t.PureComponent {
             constructor(e) {
-                super(e), this.sessionEventConn = void 0, this.curView = void 0, this.minimizePromptTimer = new Ca, this.keyHandlers = void 0, this.handleScroll = () => {
+                super(e), this.sessionEventConn = void 0, this.curView = void 0, this.minimizePromptTimer = new As, this.keyHandlers = void 0, this.handleScroll = () => {
                     this.setState({
-                        statusMinimized: cs.shouldMinimize()
+                        statusMinimized: Js.shouldMinimize()
                     })
                 }, this.onAppPromptHover = () => {
                     this.setState({
                         promptHovered: !0
                     })
                 }, this.onAppPromptUnhover = () => {
                     this.setState({
@@ -121771,15 +122630,15 @@
                 }, this.handleStopScriptClick = () => {
                     this.props.stopScript()
                 }, this.handleRerunClick = () => {
                     this.props.rerunScript(!1)
                 }, this.handleAlwaysRerunClick = () => {
                     this.props.allowRunOnSave && this.props.rerunScript(!0)
                 }, this.state = {
-                    statusMinimized: cs.shouldMinimize(),
+                    statusMinimized: Js.shouldMinimize(),
                     promptMinimized: !1,
                     scriptChangedOnDisk: !1,
                     promptHovered: !1
                 }, this.keyHandlers = {
                     a: this.handleAlwaysRerunClick
                 }
             }
@@ -121792,15 +122651,15 @@
             componentDidMount() {
                 this.sessionEventConn = this.props.sessionEventDispatcher.onSessionEvent.connect((e => this.handleSessionEvent(e))), window.addEventListener("scroll", this.handleScroll)
             }
             componentWillUnmount() {
                 void 0 !== this.sessionEventConn && (this.sessionEventConn.disconnect(), this.sessionEventConn = void 0), this.minimizePromptTimer.cancel(), window.removeEventListener("scroll", this.handleScroll)
             }
             isConnected() {
-                return this.props.connectionState === Ja.CONNECTED
+                return this.props.connectionState === js.CONNECTED
             }
             handleSessionEvent(e) {
                 "scriptChangedOnDisk" === e.type && (this.setState({
                     scriptChangedOnDisk: !0,
                     promptMinimized: !1
                 }), this.minimizePromptAfterTimeout(15e3))
             }
@@ -121814,44 +122673,44 @@
             static shouldMinimize() {
                 return window.scrollY > 32
             }
             render() {
                 const e = this.curView;
                 if (this.curView = this.renderWidget(), null == e && null == this.curView) return null;
                 let t, n;
-                return null != this.curView ? (t = !0, n = this.curView) : (t = !1, n = e), (0, ge.jsx)(Za, {
+                return null != this.curView ? (t = !0, n = this.curView) : (t = !1, n = e), (0, ge.jsx)(Bs, {
                     appear: !0,
                     in: t,
                     timeout: 200,
                     unmountOnExit: !0,
                     classNames: "StatusWidget",
-                    children: (0, ge.jsx)(ss, {
+                    children: (0, ge.jsx)(Ys, {
                         "data-testid": "stStatusWidget",
                         children: n
                     }, "StatusWidget")
                 })
             }
             renderWidget() {
                 if (this.isConnected()) {
                     if (this.props.scriptRunState === Je.RUNNING || this.props.scriptRunState === Je.RERUN_REQUESTED) return this.renderScriptIsRunning();
-                    if (!Wa.B && this.state.scriptChangedOnDisk) return this.renderRerunScriptPrompt()
+                    if (!vs.B && this.state.scriptChangedOnDisk) return this.renderRerunScriptPrompt()
                 }
                 return this.renderConnectionStatus()
             }
             renderConnectionStatus() {
-                const e = cs.getConnectionStateUI(this.props.connectionState);
-                return void 0 === e ? null : (0, ge.jsx)(Pr.Z, {
+                const e = Js.getConnectionStateUI(this.props.connectionState);
+                return void 0 === e ? null : (0, ge.jsx)(_o.Z, {
                     content: e.tooltip,
-                    placement: Pr.u.BOTTOM,
-                    children: (0, ge.jsxs)(es, {
+                    placement: _o.u.BOTTOM,
+                    children: (0, ge.jsxs)(Us, {
                         "data-testid": "stConnectionStatus",
                         children: [(0, ge.jsx)(hn.Z, {
                             size: "sm",
                             content: e.icon
-                        }), (0, ge.jsx)(ts, {
+                        }), (0, ge.jsx)(Vs, {
                             isMinimized: this.state.statusMinimized,
                             children: e.label
                         })]
                     })
                 })
             }
             static isNewYears() {
@@ -121859,28 +122718,28 @@
                     t = e.getMonth(),
                     n = e.getDate();
                 return 11 === t && 31 === n || 0 === t && n <= 6
             }
             renderScriptIsRunning() {
                 const e = this.state.statusMinimized,
                     t = this.props.scriptRunState === Je.STOP_REQUESTED,
-                    n = cs.promptButton(t ? "Stopping..." : "Stop", t, this.handleStopScriptClick, e),
-                    r = cs.isNewYears(),
-                    o = r ? Qa : "data:image/gif;base64,R0lGODlhgACAAPAAAAAAAAAAACH5BAkUAAEAIf8LTkVUU0NBUEUyLjADAQAAACwAAAAAgACAAAAC/oyPqcvtD6OctNqLs968+w+G4kiW5omm6sq27gvH8kzX9o3nKcD3vA5s+Ia9oNFATAKOQKWSiXM6oTbpkzqzTrEx7ZX78ibBYfGYzDKf0So1kZ12/+Ar+Zy+s+Pr7j1f7ffnFRinRegiddg1pNho5OMIKbhGZpXXl6N3YrdlwvlF8ik6SioZWoqaauap2ur6xvoqm4oya1t6easL2Lbra1j2+5sp3ApWjKmI7Bghy1zh/DwRLd38Wi1Bje2gvc3Q7a0AHo4wTo50fb5gfs5O7h4O7y2/TY9tX40vrf/Mz+wfKZ26BAAbFVQmcOCBg4cYEnIYCKIfiXso4rFIByMcnY1sOKLxWCmhwgCWhCQaufDkN5UoS67s1JKlOJkKXa6jOdDmTJgjdRLEqc5nOaDtiJI0Gs+o0KBKkc5ryrMmVFA9p1KqGnVoVqZb0XV9ZxUWyqNflxYt67ReWEZjyVL9+TUp2rhP577NudZUTLtXpfIVu/duSrpq/7Id6zRtYcAvGQfWy60vYsgPDre9jDmz5s2cO3v+DDq06NEnCgAAIfkECRQAAQAsAAAAAIAAgAAAAv6Mj6nL7Q+jnLTai7PevPsPhuJIluaJpurKtu4Lx/JM1/aN5/rO9/4P1AGGxGGwV0wSjzmlE8C0PZ/R2XRahV2vWdcW22V9qeHV2FlWnclp0xrddr+T8dN8WZff8/o5v3/2BzgmOMhVaAiHaAe2qEbnGCk56XBHSLlgaYl5oOmJ6Rk6GUoaSVrqeIpaqLoq2OqaBxtbNyv6eljZyprbAMvL5vuLG8wwTKxofIxcBLGM2Oz8zKm8S/0wfZ0wq62r2i1sDa6QPc49Ti6O3lkObFR9Opq8rc6sBB/v3kj/rb/PXi/Om0wB2/jh10/WQQTtumxCaGsekocMI2758QmixfZiNxbi28ixxpoIIC91NCmtZC+RXyiobCkFpsuX/2TIrEAz5IubOHNK3Hkxg897NIJuGIrHptGjSIuubPLUS9STNaVWpapTzFWsP1tM5UpUadaYW82U1bA05dhHa4V+JXg2RVoPc721RVGXQ96PkMTetbAX7t9EST8EFtzV69sLh9PFlbu4Z2SNff0OVps43GXChd1OphzNaWNsPEl+xotS8umKj9mOdvwadGcrqUnXlhAbciDbt3Gv1j0QoEfVmbUMRfvbtUqmm82+7NDaOEjDYSdaDBEayPV1wmlxz8dd88jwvnOTP48+vfr17Nu7fw8/vnz4BQAAIfkECRQAAQAsAAAAAIAAgAAAAv6Mj6nL7Q+jnLTai7PevPsPhuJIluaJpurKtu4Lx/IG1PaMc/a+537FC9Z+xIfwWEwmjkylkgl1FqFN6Y9atc6wWW2Mi/TKwELxmMwzf9E99YvddrvgQ/kcbofh828yf431FxK2ECjowcVAeKgDxsjC9phCJ2lCV1c5eImZ2bEZ16nxmRaaMRpUenFaljqxutja8NoVqzAbVWt7i5trsJuYOxuAVivsS1xqfBDZqYxAKfkquyko7TDKtxpxasctge3m7foZTq56KUdtCq2G3ojcvofomC4PQpVtr0ma594ryu4fBn8CB+orCOQgwnHMYuH7ppAGLxQRn1WkcFGiuv5p8Axu9GRNUcOE2t450+UH4y6AvwBcSwmx5bmWnFAa2kazJoScoGxOfMnTZUxgPn8uuQkUqUV6RpQmpXXUaFFWOB9yhFoV6zKpS7U+hRUVLEOvw8g6HUt1as+ZadXq7IpKo1ircuMW8srVAt1jYte1hcvP7T1aeT3+5Xu4bGKWacn6tRsWMuAbIrr0BXlYquPH/DZzXqs482WTpEZjDrx17uJ5cU2TXmvUM+MesmdTnnw7NeoRGU/Dhur69V4SYGOv/tCxRHHgx1kTtfTXuGTiMKFPl76bd3Xl0ZlP187U+m7soCtvp37de3bz4bmnX/6dfXvw49WXH1wmuO3ciK/fx0fOin6fvaVZc3VRVhtboBX4n29tJEhSfH1BqBJVFGa1Xn9CiWSgXosUZliGEYoYImoXfnXfiCR62J2AO53IYYcYZgfiUDLOuCKO/OnmoltvHZjjVZed9WKNJTYo5HHPFQmjjin6uONdRPJo5ICmzZckTRQF9WOWK00SlIK33CHTkeK0UOZ+H5FZknMEnWGOfOf5EJB7VeKw5EJ67slnn37+CWiggg5KaKGGMlIAACH5BAkUAAEALAAAAACAAIAAAAL+jI+py+0Po5y02ouz3rz7D4biSJbmiabqyrbuC8cyBNT2jHP2vud+xQvefsSG8AgoKhFI5HLZPD6LUefUV5Vec1nhFtfVfmFh75hc5p3R6do61na/X/HknJ6+s8P6fbUPlwUo8zc4I2aYqLjI2Ehk5rhSGGlSRilSd+lRJ6eZwdnjCQQaJCpBimi6gNqkqsAq6GoAG6tKy2d6aymqi6vZu3sJ7BuZN0sr3JWgSzm5zOwYxTAc3bpKzSh9ja2o/To8ZOj9DB7eN34AGtAGiH6cyXnnvp75Hj82f5+u/pVfz8TviruAAPU9GWiwYJwtCBc6+HfQmkJjD9gJtELOYoTpYFMw7oO40VlHSBMpjiLZL9Q3hxtUZgMpa0LCmCFh0qw48+ZDgjp3kuqJExXQaciGZmRltKTQpPSgGf3DsmcsjVLHUb0p0iTWhsqqSlTq8Y1LCrWOfj0zj+hZs6lSElsZFm5chjBFbpt7sZw5I2vz6rVDo+/Iv4CDtqX795TgwXoV4/XLLfBjyL1kLkbrtObhdj/JXhanVTPKX5/5TvZUGENappI3szY8+nXr2LJ9uq59lzbu3KV2i+7tGzbw4KZvE29qnPjq48h1M19+HLry0sGlV6d+3Tnz5mO3y+3kvWL48eTLmz8PoQAAIfkECRQAAQAsAAAAAIAAgAAAAv6Mj6nL7Q+jnLTai7PevPsPhuJIluaJpurKtu4Lx/JM1/aN5/rO9/4PDAqHQ4DRWDseiQalc8l6PoXSKgBllQKz1RJX2/taRWLwrjz2oM25dbfjdvLibAxdrrvXK3pou49nAeiHM6h0YXiVl4jEZxjG6Dj4EzmRSARo+cgUoCdxydlEFwEa2jn6UGp66gYxuYqA2vAKeyDL0FercLtwp9sb5+D7uxs820oMjHz8lSxs/PzmHL32STjNDI0Nl7vNseltpxquWUluzdh4npp+uJ7drv4eGz81b1u/R56fts6f5e8fwHACm20rKAYbwjLOulFD03BZOYYRDYqzOI3Lt/aB++x98HgvpMiRJEuaPIkypcqKIDVw3NDPBUREMwVRTDEMnUR22khk4ukJKK+P4/AVFQWO28KlP2EyferwItSpPSVRvXqTJtatGjNw/RrTZldltBKYKzZWa1iyQ9EGfdhSbFx4NUm1xSXNZSAK1dRinCjvxlqpc1caPow4seLFjBs7hqTP7169kXFm5VsXc0IVb13dxVs1RFO6oc1GBXGW3lFWZTeCBav0NWzKsl/Trv31Nu6tundf7V2Y9WjVrYkPBhzcaGfQy9kmt1vZbV+d0z1HB0w4rebNVgPbOC73+ePx5MubP48+vfr17Nu7fw8/vvzGBQAAIfkECRQAAQAsAAAAAIAAgAAAAv6Mj6nL7Q+jnLTai7PevPsPhuJIluaJphPAAuoLI+3cxrZJ5+7Ne/q/6wkvQN3wSCn+kEyHEtiMJp5LqZVqtEaxVS2Sm/UewTnxlzwzn9HqNbk9RgfhPTY9jr27n3omv99UBKiVNmh4iJiouMjY6FhX9hijJJnCVVnyhhkit/khx+LJARoqmkFaY0qEOqcqwVrq+gobK+tEW2u7gJuqu8ub62sA3Cs8TBxsi1wovMys7PysGh05TV29eQ1Vqf2H2N35jXyMKg4sw3o4jl5ueK4Aq07bEO+efts+eI9PKp/PUM/eP3j7BPYDWFDcAU0EBzZiyO4gNzC/JE681DBcNvCKGSFi8kgO5MU8HUmaEmnHGsYpHF2hXOmyZURKul7S/JjM5raRrUJSqdjlUZiZ3ohKY7TTqKCSyRTdVJp0ITakRaXCtNrUXFWsWwMUo3qV69OFkjSyNLnRLNShZR36HPsw4NmfQuchROs07Aq9+vjuxdsX8CrBd2RuMFzYLwbEbRiPcutH8WHIQxx/ogyJ7omEeOBmwmxDswrOmaOOBv3C82mLQkzDkNt6amjYpXvOpm1srcjcXnnxZopa1rrfvd8RL47ruNjg0HATd36ceW5Qyh+krE5PMva3Qbfz6+79O43wSdiShyD7PPqv6tsbKgAAOw==",
-                    i = (0, ge.jsx)(as, {
+                    n = Js.promptButton(t ? "Stopping..." : "Stop", t, this.handleStopScriptClick, e),
+                    r = Js.isNewYears(),
+                    o = r ? Fs : "data:image/gif;base64,R0lGODlhgACAAPAAAAAAAAAAACH5BAkUAAEAIf8LTkVUU0NBUEUyLjADAQAAACwAAAAAgACAAAAC/oyPqcvtD6OctNqLs968+w+G4kiW5omm6sq27gvH8kzX9o3nKcD3vA5s+Ia9oNFATAKOQKWSiXM6oTbpkzqzTrEx7ZX78ibBYfGYzDKf0So1kZ12/+Ar+Zy+s+Pr7j1f7ffnFRinRegiddg1pNho5OMIKbhGZpXXl6N3YrdlwvlF8ik6SioZWoqaauap2ur6xvoqm4oya1t6easL2Lbra1j2+5sp3ApWjKmI7Bghy1zh/DwRLd38Wi1Bje2gvc3Q7a0AHo4wTo50fb5gfs5O7h4O7y2/TY9tX40vrf/Mz+wfKZ26BAAbFVQmcOCBg4cYEnIYCKIfiXso4rFIByMcnY1sOKLxWCmhwgCWhCQaufDkN5UoS67s1JKlOJkKXa6jOdDmTJgjdRLEqc5nOaDtiJI0Gs+o0KBKkc5ryrMmVFA9p1KqGnVoVqZb0XV9ZxUWyqNflxYt67ReWEZjyVL9+TUp2rhP577NudZUTLtXpfIVu/duSrpq/7Id6zRtYcAvGQfWy60vYsgPDre9jDmz5s2cO3v+DDq06NEnCgAAIfkECRQAAQAsAAAAAIAAgAAAAv6Mj6nL7Q+jnLTai7PevPsPhuJIluaJpurKtu4Lx/JM1/aN5/rO9/4P1AGGxGGwV0wSjzmlE8C0PZ/R2XRahV2vWdcW22V9qeHV2FlWnclp0xrddr+T8dN8WZff8/o5v3/2BzgmOMhVaAiHaAe2qEbnGCk56XBHSLlgaYl5oOmJ6Rk6GUoaSVrqeIpaqLoq2OqaBxtbNyv6eljZyprbAMvL5vuLG8wwTKxofIxcBLGM2Oz8zKm8S/0wfZ0wq62r2i1sDa6QPc49Ti6O3lkObFR9Opq8rc6sBB/v3kj/rb/PXi/Om0wB2/jh10/WQQTtumxCaGsekocMI2758QmixfZiNxbi28ixxpoIIC91NCmtZC+RXyiobCkFpsuX/2TIrEAz5IubOHNK3Hkxg897NIJuGIrHptGjSIuubPLUS9STNaVWpapTzFWsP1tM5UpUadaYW82U1bA05dhHa4V+JXg2RVoPc721RVGXQ96PkMTetbAX7t9EST8EFtzV69sLh9PFlbu4Z2SNff0OVps43GXChd1OphzNaWNsPEl+xotS8umKj9mOdvwadGcrqUnXlhAbciDbt3Gv1j0QoEfVmbUMRfvbtUqmm82+7NDaOEjDYSdaDBEayPV1wmlxz8dd88jwvnOTP48+vfr17Nu7fw8/vnz4BQAAIfkECRQAAQAsAAAAAIAAgAAAAv6Mj6nL7Q+jnLTai7PevPsPhuJIluaJpurKtu4Lx/IG1PaMc/a+537FC9Z+xIfwWEwmjkylkgl1FqFN6Y9atc6wWW2Mi/TKwELxmMwzf9E99YvddrvgQ/kcbofh828yf431FxK2ECjowcVAeKgDxsjC9phCJ2lCV1c5eImZ2bEZ16nxmRaaMRpUenFaljqxutja8NoVqzAbVWt7i5trsJuYOxuAVivsS1xqfBDZqYxAKfkquyko7TDKtxpxasctge3m7foZTq56KUdtCq2G3ojcvofomC4PQpVtr0ma594ryu4fBn8CB+orCOQgwnHMYuH7ppAGLxQRn1WkcFGiuv5p8Axu9GRNUcOE2t450+UH4y6AvwBcSwmx5bmWnFAa2kazJoScoGxOfMnTZUxgPn8uuQkUqUV6RpQmpXXUaFFWOB9yhFoV6zKpS7U+hRUVLEOvw8g6HUt1as+ZadXq7IpKo1ircuMW8srVAt1jYte1hcvP7T1aeT3+5Xu4bGKWacn6tRsWMuAbIrr0BXlYquPH/DZzXqs482WTpEZjDrx17uJ5cU2TXmvUM+MesmdTnnw7NeoRGU/Dhur69V4SYGOv/tCxRHHgx1kTtfTXuGTiMKFPl76bd3Xl0ZlP187U+m7soCtvp37de3bz4bmnX/6dfXvw49WXH1wmuO3ciK/fx0fOin6fvaVZc3VRVhtboBX4n29tJEhSfH1BqBJVFGa1Xn9CiWSgXosUZliGEYoYImoXfnXfiCR62J2AO53IYYcYZgfiUDLOuCKO/OnmoltvHZjjVZed9WKNJTYo5HHPFQmjjin6uONdRPJo5ICmzZckTRQF9WOWK00SlIK33CHTkeK0UOZ+H5FZknMEnWGOfOf5EJB7VeKw5EJ67slnn37+CWiggg5KaKGGMlIAACH5BAkUAAEALAAAAACAAIAAAAL+jI+py+0Po5y02ouz3rz7D4biSJbmiabqyrbuC8cyBNT2jHP2vud+xQvefsSG8AgoKhFI5HLZPD6LUefUV5Vec1nhFtfVfmFh75hc5p3R6do61na/X/HknJ6+s8P6fbUPlwUo8zc4I2aYqLjI2Ehk5rhSGGlSRilSd+lRJ6eZwdnjCQQaJCpBimi6gNqkqsAq6GoAG6tKy2d6aymqi6vZu3sJ7BuZN0sr3JWgSzm5zOwYxTAc3bpKzSh9ja2o/To8ZOj9DB7eN34AGtAGiH6cyXnnvp75Hj82f5+u/pVfz8TviruAAPU9GWiwYJwtCBc6+HfQmkJjD9gJtELOYoTpYFMw7oO40VlHSBMpjiLZL9Q3hxtUZgMpa0LCmCFh0qw48+ZDgjp3kuqJExXQaciGZmRltKTQpPSgGf3DsmcsjVLHUb0p0iTWhsqqSlTq8Y1LCrWOfj0zj+hZs6lSElsZFm5chjBFbpt7sZw5I2vz6rVDo+/Iv4CDtqX795TgwXoV4/XLLfBjyL1kLkbrtObhdj/JXhanVTPKX5/5TvZUGENappI3szY8+nXr2LJ9uq59lzbu3KV2i+7tGzbw4KZvE29qnPjq48h1M19+HLry0sGlV6d+3Tnz5mO3y+3kvWL48eTLmz8PoQAAIfkECRQAAQAsAAAAAIAAgAAAAv6Mj6nL7Q+jnLTai7PevPsPhuJIluaJpurKtu4Lx/JM1/aN5/rO9/4PDAqHQ4DRWDseiQalc8l6PoXSKgBllQKz1RJX2/taRWLwrjz2oM25dbfjdvLibAxdrrvXK3pou49nAeiHM6h0YXiVl4jEZxjG6Dj4EzmRSARo+cgUoCdxydlEFwEa2jn6UGp66gYxuYqA2vAKeyDL0FercLtwp9sb5+D7uxs820oMjHz8lSxs/PzmHL32STjNDI0Nl7vNseltpxquWUluzdh4npp+uJ7drv4eGz81b1u/R56fts6f5e8fwHACm20rKAYbwjLOulFD03BZOYYRDYqzOI3Lt/aB++x98HgvpMiRJEuaPIkypcqKIDVw3NDPBUREMwVRTDEMnUR22khk4ukJKK+P4/AVFQWO28KlP2EyferwItSpPSVRvXqTJtatGjNw/RrTZldltBKYKzZWa1iyQ9EGfdhSbFx4NUm1xSXNZSAK1dRinCjvxlqpc1caPow4seLFjBs7hqTP7169kXFm5VsXc0IVb13dxVs1RFO6oc1GBXGW3lFWZTeCBav0NWzKsl/Trv31Nu6tundf7V2Y9WjVrYkPBhzcaGfQy9kmt1vZbV+d0z1HB0w4rebNVgPbOC73+ePx5MubP48+vfr17Nu7fw8/vvzGBQAAIfkECRQAAQAsAAAAAIAAgAAAAv6Mj6nL7Q+jnLTai7PevPsPhuJIluaJphPAAuoLI+3cxrZJ5+7Ne/q/6wkvQN3wSCn+kEyHEtiMJp5LqZVqtEaxVS2Sm/UewTnxlzwzn9HqNbk9RgfhPTY9jr27n3omv99UBKiVNmh4iJiouMjY6FhX9hijJJnCVVnyhhkit/khx+LJARoqmkFaY0qEOqcqwVrq+gobK+tEW2u7gJuqu8ub62sA3Cs8TBxsi1wovMys7PysGh05TV29eQ1Vqf2H2N35jXyMKg4sw3o4jl5ueK4Aq07bEO+efts+eI9PKp/PUM/eP3j7BPYDWFDcAU0EBzZiyO4gNzC/JE681DBcNvCKGSFi8kgO5MU8HUmaEmnHGsYpHF2hXOmyZURKul7S/JjM5raRrUJSqdjlUZiZ3ohKY7TTqKCSyRTdVJp0ITakRaXCtNrUXFWsWwMUo3qV69OFkjSyNLnRLNShZR36HPsw4NmfQuchROs07Aq9+vjuxdsX8CrBd2RuMFzYLwbEbRiPcutH8WHIQxx/ogyJ7omEeOBmwmxDswrOmaOOBv3C82mLQkzDkNt6amjYpXvOpm1srcjcXnnxZopa1rrfvd8RL47ruNjg0HATd36ceW5Qyh+krE5PMva3Qbfz6+79O43wSdiShyD7PPqv6tsbKgAAOw==",
+                    i = (0, ge.jsx)(Ks, {
                         isNewYears: r,
                         src: o,
                         alt: "Running..."
                     });
-                return (0, ge.jsxs)(ns, {
-                    children: [e ? (0, ge.jsx)(Pr.Z, {
-                        placement: Pr.u.BOTTOM,
+                return (0, ge.jsxs)(Hs, {
+                    children: [e ? (0, ge.jsx)(_o.Z, {
+                        placement: _o.u.BOTTOM,
                         content: "This script is currently running",
                         children: i
-                    }) : i, (0, ge.jsx)(os, {
+                    }) : i, (0, ge.jsx)(Gs, {
                         isMinimized: this.state.statusMinimized,
                         isPrompt: !1,
                         children: "Running..."
                     }), n]
                 })
             }
             renderRerunScriptPrompt() {
@@ -121892,66 +122751,66 @@
                 return (0, ge.jsx)(Le.HotKeys, {
                     handlers: this.keyHandlers,
                     attach: window,
                     focused: !0,
                     children: (0, ge.jsx)("div", {
                         onMouseEnter: this.onAppPromptHover,
                         onMouseLeave: this.onAppPromptUnhover,
-                        children: (0, ge.jsxs)(ns, {
+                        children: (0, ge.jsxs)(Hs, {
                             children: [(0, ge.jsx)(hn.Z, {
-                                content: Ra,
+                                content: gs,
                                 margin: "0 sm 0 0",
                                 color: n.bodyText
-                            }), (0, ge.jsx)(os, {
+                            }), (0, ge.jsx)(Gs, {
                                 isMinimized: t,
                                 isPrompt: !0,
                                 children: "Source file changed."
-                            }), cs.promptButton((0, ge.jsx)(ls, {
+                            }), Js.promptButton((0, ge.jsx)(Zs, {
                                 children: "Rerun"
-                            }), e, this.handleRerunClick, t), this.props.allowRunOnSave && cs.promptButton((0, ge.jsx)(ls, {
+                            }), e, this.handleRerunClick, t), this.props.allowRunOnSave && Js.promptButton((0, ge.jsx)(Zs, {
                                 children: "Always rerun"
                             }), e, this.handleAlwaysRerunClick, t)]
                         })
                     })
                 })
             }
             static promptButton(e, t, n, r) {
-                return (0, ge.jsx)(is, {
+                return (0, ge.jsx)($s, {
                     isMinimized: r,
                     children: (0, ge.jsx)(an.ZP, {
                         kind: sn.nW.HEADER_BUTTON,
                         disabled: t,
                         fluidWidth: !0,
                         onClick: n,
                         children: e
                     })
                 })
             }
             static getConnectionStateUI(e) {
                 switch (e) {
-                    case Ja.INITIAL:
-                    case Ja.PINGING_SERVER:
-                    case Ja.CONNECTING:
+                    case js.INITIAL:
+                    case js.PINGING_SERVER:
+                    case js.CONNECTING:
                         return {
-                            icon: Ta, label: "Connecting", tooltip: "Connecting to Streamlit server"
+                            icon: zs, label: "Connecting", tooltip: "Connecting to Streamlit server"
                         };
-                    case Ja.CONNECTED:
+                    case js.CONNECTED:
                         return;
-                    case Ja.DISCONNECTED_FOREVER:
+                    case js.DISCONNECTED_FOREVER:
                     default:
                         return {
-                            icon: ka, label: "Error", tooltip: "Unable to connect to Streamlit server"
+                            icon: ys, label: "Error", tooltip: "Unable to connect to Streamlit server"
                         }
                 }
             }
         }
-        const us = (0, Ee.b)(cs);
-        var ps = __webpack_require__(37701),
-            ds = __webpack_require__(96386),
-            bs = t.forwardRef((function(e, n) {
+        const Qs = (0, Ee.b)(Js);
+        var el = __webpack_require__(37701),
+            tl = __webpack_require__(96386),
+            nl = t.forwardRef((function(e, n) {
                 return t.createElement(en.D, (0, Qt.Z)({
                     iconAttrs: {
                         fill: "currentColor",
                         xmlns: "http://www.w3.org/2000/svg"
                     },
                     iconVerticalAlign: "middle",
                     iconViewBox: "0 0 24 24"
@@ -121960,20 +122819,20 @@
                 }), t.createElement("path", {
                     fill: "none",
                     d: "M0 0h24v24H0V0z"
                 }), t.createElement("path", {
                     d: "M12 8c1.1 0 2-.9 2-2s-.9-2-2-2-2 .9-2 2 .9 2 2 2zm0 2c-1.1 0-2 .9-2 2s.9 2 2 2 2-.9 2-2-.9-2-2-2zm0 6c-1.1 0-2 .9-2 2s.9 2 2 2 2-.9 2-2-.9-2-2-2z"
                 }))
             }));
-        bs.displayName = "MoreVert";
-        const fs = "video/webm";
-        const hs = class {
+        nl.displayName = "MoreVert";
+        const rl = "video/webm";
+        const ol = class {
             static isSupportedBrowser() {
                 try {
-                    return null != navigator.mediaDevices && null != navigator.mediaDevices.getUserMedia && null != navigator.mediaDevices.getDisplayMedia && MediaRecorder.isTypeSupported(fs)
+                    return null != navigator.mediaDevices && null != navigator.mediaDevices.getUserMedia && null != navigator.mediaDevices.getDisplayMedia && MediaRecorder.isTypeSupported(rl)
                 } catch (e) {
                     return !1
                 }
             }
             constructor(e) {
                 let {
                     recordAudio: t,
@@ -121989,24 +122848,24 @@
                     const t = await navigator.mediaDevices.getUserMedia({
                         video: !1,
                         audio: !0
                     });
                     e = e.concat(t.getAudioTracks())
                 }
                 this.recordedChunks = [], this.inputStream = new MediaStream(e), this.mediaRecorder = new MediaRecorder(this.inputStream, {
-                    mimeType: fs
+                    mimeType: rl
                 }), this.mediaRecorder.ondataavailable = e => this.recordedChunks.push(e.data)
             }
             getState() {
                 return this.mediaRecorder ? this.mediaRecorder.state : "inactive"
             }
             start() {
-                if (!this.mediaRecorder) return (0, wo.KE)("ScreenCastRecorder.start: mediaRecorder is null"), !1;
+                if (!this.mediaRecorder) return (0, bi.KE)("ScreenCastRecorder.start: mediaRecorder is null"), !1;
                 const e = e => {
-                    (0, wo.KE)("mediaRecorder.start threw an error: ".concat(e))
+                    (0, bi.KE)("mediaRecorder.start threw an error: ".concat(e))
                 };
                 this.mediaRecorder.onerror = t => {
                     e(t), this.onErrorOrStopCallback()
                 }, this.mediaRecorder.onstop = () => this.onErrorOrStopCallback();
                 try {
                     this.mediaRecorder.start()
                 } catch (t) {
@@ -122020,65 +122879,65 @@
                 const t = new Promise((t => {
                     e = t
                 }));
                 return this.mediaRecorder.onstop = () => e(), this.mediaRecorder.stop(), this.inputStream && (this.inputStream.getTracks().forEach((e => e.stop())), this.inputStream = null), t.then((() => this.buildOutputBlob()))
             }
             buildOutputBlob() {
                 return new Blob(this.recordedChunks, {
-                    type: fs
+                    type: rl
                 })
             }
         };
-        var ms;
-        const Ms = e => (0, Oe.F4)(ms || (ms = (0, Ki.Z)(["\n0% {\n  box-shadow: 0 0 ", " ", ";\n}\n50% {\n  box-shadow: 0 0 ", " ", " ", ";\n}\n100% {\n  box-shadow: 0 0 ", " ", ";\n}"])), e.spacing.twoXS, e.colors.red, e.spacing.sm, e.spacing.twoXS, e.colors.red, e.spacing.twoXS, e.colors.red),
-            Os = (0, Qe.Z)("div", {
+        var il;
+        const al = e => (0, Oe.F4)(il || (il = (0, Pa.Z)(["\n0% {\n  box-shadow: 0 0 ", " ", ";\n}\n50% {\n  box-shadow: 0 0 ", " ", " ", ";\n}\n100% {\n  box-shadow: 0 0 ", " ", ";\n}"])), e.spacing.twoXS, e.colors.red, e.spacing.sm, e.spacing.twoXS, e.colors.red, e.spacing.twoXS, e.colors.red),
+            sl = (0, Qe.Z)("div", {
                 target: "e16jpq808"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     position: "absolute",
                     bottom: t.spacing.lg,
                     right: t.spacing.sm,
                     width: t.spacing.sm,
                     height: t.spacing.sm,
                     backgroundColor: "red",
                     borderRadius: t.radii.full,
                     boxShadow: "0 0 ".concat(t.spacing.twoXS, " ").concat(t.colors.red),
-                    animation: "".concat(Ms(t), " 2s linear infinite")
+                    animation: "".concat(al(t), " 2s linear infinite")
                 }
             }), ""),
-            gs = (0, Qe.Z)("div", {
+            ll = (0, Qe.Z)("div", {
                 target: "e16jpq807"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     borderTop: "1px solid ".concat(t.colors.fadedText10),
                     margin: "".concat(t.spacing.sm, " ").concat(t.spacing.none)
                 }
             }), ""),
-            zs = (0, Qe.Z)("span", {
+            cl = (0, Qe.Z)("span", {
                 target: "e16jpq806"
             })((e => {
                 let {
                     isRecording: t,
                     theme: n
                 } = e;
                 return {
                     color: t ? n.colors.red : n.colors.fadedText60,
                     fontSize: n.fontSizes.sm,
                     marginTop: n.spacing.twoXS,
                     fontVariant: "small-caps",
                     textTransform: "uppercase"
                 }
             }), ""),
-            ys = (0, Qe.Z)("ul", {
+            ul = (0, Qe.Z)("ul", {
                 target: "e16jpq805"
             })((e => {
                 let {
                     isDisabled: t,
                     isRecording: n,
                     theme: r
                 } = e;
@@ -122087,15 +122946,15 @@
                     color: r.colors.fadedText60,
                     cursor: "not-allowed"
                 } : {
                     "&:active": {
                         backgroundColor: r.colors.primary,
                         color: r.colors.white,
                         outline: "none",
-                        [zs]: {
+                        [cl]: {
                             color: r.colors.white
                         }
                     },
                     "&:focus": {
                         backgroundColor: r.colors.primary,
                         color: r.colors.white
                     }
@@ -122111,15 +122970,15 @@
                     } || {},
                     ...o,
                     "@media print": {
                         display: "none !important"
                     }
                 }
             }), ""),
-            As = (0, Qe.Z)("li", {
+            pl = (0, Qe.Z)("li", {
                 target: "e16jpq804"
             })((e => {
                 let {
                     isHighlighted: t,
                     styleProps: n,
                     theme: r
                 } = e;
@@ -122133,15 +122992,15 @@
                     padding: (null === n || void 0 === n ? void 0 : n.padding) || "".concat(r.spacing.twoXS, " ").concat(r.spacing.twoXL),
                     backgroundColor: (null === n || void 0 === n ? void 0 : n.backgroundColor) || r.colors.primaryBg,
                     fontSize: (null === n || void 0 === n ? void 0 : n.fontSize) || r.fontSizes.md,
                     ...o || {},
                     display: "block"
                 }
             }), ""),
-            vs = (0, Qe.Z)("li", {
+            dl = (0, Qe.Z)("li", {
                 target: "e16jpq803"
             })((e => {
                 let {
                     isHighlighted: t,
                     styleProps: n,
                     theme: r
                 } = e;
@@ -122155,27 +123014,27 @@
                     padding: (null === n || void 0 === n ? void 0 : n.padding) || "".concat(r.spacing.twoXS, " ").concat(r.spacing.twoXL),
                     backgroundColor: (null === n || void 0 === n ? void 0 : n.backgroundColor) || r.colors.secondaryBg,
                     fontSize: (null === n || void 0 === n ? void 0 : n.fontSize) || r.fontSizes.md,
                     ...o || {},
                     display: "block"
                 }
             }), ""),
-            ws = (0, Qe.Z)("span", {
+            bl = (0, Qe.Z)("span", {
                 target: "e16jpq802"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     marginRight: t.spacing.md,
                     flexGrow: 1,
                     fontFamily: t.fonts.sansSerif
                 }
             }), ""),
-            Ss = (0, Qe.Z)("div", {
+            fl = (0, Qe.Z)("div", {
                 target: "e16jpq801"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     ul: {
@@ -122189,29 +123048,29 @@
                         borderTopLeftRadius: 0,
                         borderTopRightRadius: 0,
                         boxShadow: "none",
                         borderTop: "none"
                     }
                 }
             }), ""),
-            qs = (0, Qe.Z)("span", {
+            hl = (0, Qe.Z)("span", {
                 target: "e16jpq800"
             })((() => ({
                 lineHeight: "initial"
             })), ""),
-            Es = {
+            ml = {
                 COUNTDOWN: "Cancel screencast",
                 RECORDING: "Stop recording"
             },
-            _s = e => () => {
+            Ml = e => () => {
                 window.open(e, "_blank")
             },
-            xs = () => "localhost" === window.location.hostname || "127.0.0.1" === window.location.hostname;
+            Ol = () => "localhost" === window.location.hostname || "127.0.0.1" === window.location.hostname;
 
-        function Rs(e, n) {
+        function gl(e, n) {
             const r = (0, t.forwardRef)(((t, r) => {
                 let {
                     item: o,
                     "aria-selected": i,
                     onClick: a,
                     onMouseEnter: s,
                     $disabled: l,
@@ -122235,52 +123094,52 @@
                         n.enqueue("menuClick", {
                             label: u
                         }), a(e)
                     },
                     onMouseEnter: s
                 });
                 return (0, ge.jsxs)(ge.Fragment, {
-                    children: [d && (0, ge.jsx)(gs, {
+                    children: [d && (0, ge.jsx)(ll, {
                         "data-testid": "main-menu-divider"
-                    }), (0, ge.jsx)(ys, {
+                    }), (0, ge.jsx)(ul, {
                         ref: r,
                         role: "option",
                         "aria-selected": i,
                         "aria-disabled": l,
                         ...m,
                         ...O,
                         children: (0, ge.jsxs)(e, {
                             ...M,
-                            children: [(0, ge.jsx)(ws, {
+                            children: [(0, ge.jsx)(bl, {
                                 ...m,
                                 children: u
-                            }), p && (0, ge.jsx)(zs, {
+                            }), p && (0, ge.jsx)(cl, {
                                 ...m,
                                 children: p
                             })]
                         })
                     })]
                 })
             }));
             return r.displayName = "MenuItem", r
         }
-        const Ts = e => {
+        const zl = e => {
             const {
                 colors: t
-            } = (0, Ee.u)(), n = e.isDevMenu ? vs : As;
-            return (0, ge.jsx)(ps.Z, {
+            } = (0, Ee.u)(), n = e.isDevMenu ? dl : pl;
+            return (0, ge.jsx)(el.Z, {
                 items: e.menuItems,
                 onItemSelect: t => {
                     let {
                         item: n
                     } = t;
                     n.onClick(), e.closeMenu()
                 },
                 overrides: {
-                    Option: Rs(n, e.metricsMgr),
+                    Option: gl(n, e.metricsMgr),
                     List: {
                         props: {
                             "data-testid": "main-menu-list"
                         },
                         style: {
                             backgroundColor: "inherit",
                             borderBottomRadius: 0,
@@ -122293,15 +123152,15 @@
                             border: "1px solid ".concat(t.fadedText10)
                         }
                     }
                 }
             })
         };
 
-        function ks(e) {
+        function yl(e) {
             var t, n, r, o, i, a, s;
             const l = !e.isServerConnected,
                 c = e.toolbarMode != Be.De.ToolbarMode.MINIMAL || e.toolbarMode == Be.De.ToolbarMode.MINIMAL && (null === (t = e.menuItems) || void 0 === t ? void 0 : t.aboutSectionMd),
                 u = {
                     DIVIDER: {
                         isDivider: !0
                     },
@@ -122313,31 +123172,31 @@
                     },
                     print: {
                         onClick: e.printCallback,
                         label: "Print"
                     },
                     recordScreencast: {
                         onClick: e.screencastCallback,
-                        label: Es[e.screenCastState] || "Record a screencast",
-                        shortcut: Es[e.screenCastState] ? "esc" : "",
-                        stopRecordingIndicator: Boolean(Es[e.screenCastState])
+                        label: ml[e.screenCastState] || "Record a screencast",
+                        shortcut: ml[e.screenCastState] ? "esc" : "",
+                        stopRecordingIndicator: Boolean(ml[e.screenCastState])
                     },
                     saveSnapshot: {
                         disabled: l,
                         label: "Save a snapshot"
                     },
                     ...!(null !== (n = e.menuItems) && void 0 !== n && n.hideGetHelp) && (null === (r = e.menuItems) || void 0 === r ? void 0 : r.getHelpUrl) && {
                         community: {
-                            onClick: _s(null === (o = e.menuItems) || void 0 === o ? void 0 : o.getHelpUrl),
+                            onClick: Ml(null === (o = e.menuItems) || void 0 === o ? void 0 : o.getHelpUrl),
                             label: "Get help"
                         }
                     },
                     ...!(null !== (i = e.menuItems) && void 0 !== i && i.hideReportABug) && (null === (a = e.menuItems) || void 0 === a ? void 0 : a.reportABugUrl) && {
                         report: {
-                            onClick: _s(null === (s = e.menuItems) || void 0 === s ? void 0 : s.reportABugUrl),
+                            onClick: Ml(null === (s = e.menuItems) || void 0 === s ? void 0 : s.reportABugUrl),
                             label: "Report a bug"
                         }
                     },
                     settings: {
                         onClick: e.settingsCallback,
                         label: "Settings"
                     },
@@ -122386,15 +123245,15 @@
                 b = function(e, t, n) {
                     let r;
                     if (e.toolbarMode == Be.De.ToolbarMode.MINIMAL) {
                         for (r = [n.report, n.community, n.DIVIDER, ...t.length > 0 ? t : [n.DIVIDER], n.about], r = r.filter((e => e)); r.length > 0 && r[0] == n.DIVIDER;) r.shift();
                         for (; r.length > 0 && r.at(r.length - 1) == n.DIVIDER;) r.pop();
                         return r
                     }
-                    return [n.rerun, n.settings, n.DIVIDER, n.print, ...hs.isSupportedBrowser() ? [n.recordScreencast] : [], n.DIVIDER, n.report, n.community, ...t.length > 0 ? t : [n.DIVIDER], n.about]
+                    return [n.rerun, n.settings, n.DIVIDER, n.print, ...ol.isSupportedBrowser() ? [n.recordScreencast] : [], n.DIVIDER, n.report, n.community, ...t.length > 0 ? t : [n.DIVIDER], n.about]
                 }(e, d, u),
                 f = [];
             let h = null;
             for (const M of b) M && (M !== u.DIVIDER && (h === u.DIVIDER ? f.push({
                 ...M,
                 hasDividerAbove: !0
             }) : f.push(M)), h = M);
@@ -122407,180 +123266,180 @@
                     hasDividerAbove: !0
                 }) : t.push(o)), r = o);
                 return null != r && (r.styleProps = {
                     margin: "0 0 -.5rem 0",
                     padding: ".25rem 0 .25rem 1.5rem"
                 }), t
             }(p) : [];
-            return 0 == f.length && 0 == m.length ? (0, ge.jsx)(ge.Fragment, {}) : (0, ge.jsx)(ds.Z, {
+            return 0 == f.length && 0 == m.length ? (0, ge.jsx)(ge.Fragment, {}) : (0, ge.jsx)(tl.Z, {
                 focusLock: !0,
                 placement: un.r4.bottomRight,
                 content: t => {
                     let {
                         close: n
                     } = t;
-                    return (0, ge.jsxs)(Ss, {
-                        children: [0 != f.length && (0, ge.jsx)(Ts, {
+                    return (0, ge.jsxs)(fl, {
+                        children: [0 != f.length && (0, ge.jsx)(zl, {
                             menuItems: f,
                             closeMenu: n,
                             isDevMenu: !1,
                             metricsMgr: e.metricsMgr
-                        }), 0 != m.length && (0, ge.jsx)(Ts, {
+                        }), 0 != m.length && (0, ge.jsx)(zl, {
                             menuItems: m,
                             closeMenu: n,
                             isDevMenu: !0,
                             metricsMgr: e.metricsMgr
                         })]
                     })
                 },
                 overrides: {
                     Body: {
                         props: {
                             "data-testid": "stMainMenuPopover"
                         }
                     }
                 },
-                children: (0, ge.jsxs)(qs, {
+                children: (0, ge.jsxs)(hl, {
                     id: "MainMenu",
                     "data-testid": "stMainMenu",
                     children: [(0, ge.jsx)(an.ZP, {
                         kind: sn.nW.HEADER_NO_PADDING,
                         children: (0, ge.jsx)(hn.Z, {
-                            content: bs,
+                            content: nl,
                             size: "lg"
                         })
-                    }), "RECORDING" === e.screenCastState && (0, ge.jsx)(Os, {})]
+                    }), "RECORDING" === e.screenCastState && (0, ge.jsx)(sl, {})]
                 })
             })
         }
-        const Cs = (0, t.memo)(ks),
-            Ws = (0, Qe.Z)("div", {
+        const Al = (0, t.memo)(yl),
+            vl = (0, Qe.Z)("div", {
                 target: "e3g6aar2"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     display: "flex",
                     gap: t.spacing.sm,
                     alignItems: "center",
                     lineHeight: t.iconSizes.md
                 }
             }), ""),
-            Ns = (0, Qe.Z)("div", {
+            wl = (0, Qe.Z)("div", {
                 target: "e3g6aar1"
             })((e => {
                 let {
                     icon: t
                 } = e;
                 return {
                     background: 'url("'.concat(t, '") no-repeat center / contain'),
                     width: "1rem",
                     height: "1rem"
                 }
             }), ""),
-            Ls = (0, Qe.Z)("div", {
+            Sl = (0, Qe.Z)("div", {
                 target: "e3g6aar0"
             })((e => {
                 let {} = e;
                 return {
                     display: "flex",
                     alignItems: "center",
                     flexDirection: "row"
                 }
             }), "");
 
-        function Is(e) {
+        function ql(e) {
             let {
                 label: t,
                 icon: n,
                 onClick: r
             } = e;
             return (0, ge.jsx)("div", {
                 className: "stActionButton",
                 "data-testid": "stActionButton",
                 children: (0, ge.jsx)(an.ZP, {
                     onClick: r,
                     kind: sn.nW.HEADER_BUTTON,
-                    children: (0, ge.jsxs)(Ws, {
-                        children: [n && (0, ge.jsx)(Ns, {
+                    children: (0, ge.jsxs)(vl, {
+                        children: [n && (0, ge.jsx)(wl, {
                             "data-testid": "stActionButtonIcon",
                             icon: n
                         }), t && (0, ge.jsx)("span", {
                             "data-testid": "stActionButtonLabel",
                             children: t
                         })]
                     })
                 })
             })
         }
-        const Ps = function(e) {
+        const El = function(e) {
                 let {
                     sendMessageToHost: t,
                     hostToolbarItems: n,
                     metricsMgr: r
                 } = e;
-                return (0, ge.jsx)(Ls, {
+                return (0, ge.jsx)(Sl, {
                     "data-testid": "stToolbarActions",
                     children: n.map((e => {
                         let {
                             key: n,
                             label: o,
                             icon: i
                         } = e;
-                        return (0, ge.jsx)(Is, {
+                        return (0, ge.jsx)(ql, {
                             label: o,
                             icon: i,
                             onClick: () => {
                                 r.enqueue("menuClick", {
                                     key: n
                                 }), t({
                                     type: "TOOLBAR_ITEM_CALLBACK",
                                     key: n
                                 })
                             }
                         }, n)
                     }))
                 })
             },
-            Ds = (0, Qe.Z)("div", {
+            _l = (0, Qe.Z)("div", {
                 target: "e17vllj40"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     display: "flex",
                     gap: t.spacing.sm,
                     alignItems: "center",
                     lineHeight: t.iconSizes.md
                 }
             }), "");
-        class Bs extends t.Component {
+        class xl extends t.Component {
             render() {
                 const {
                     onClick: e
                 } = this.props;
                 return (0, ge.jsx)("div", {
                     className: "stDeployButton",
                     "data-testid": "stDeployButton",
                     children: (0, ge.jsx)(an.ZP, {
                         kind: sn.nW.HEADER_BUTTON,
                         onClick: e,
-                        children: (0, ge.jsx)(Ds, {
+                        children: (0, ge.jsx)(_l, {
                             children: (0, ge.jsx)("span", {
                                 children: "Deploy"
                             })
                         })
                     })
                 })
             }
         }
-        const js = Bs,
-            Fs = (0, Qe.Z)("header", {
+        const Rl = xl,
+            Tl = (0, Qe.Z)("header", {
                 target: "ezrtsby2"
             })((e => {
                 let {
                     showHeader: t,
                     theme: n
                 } = e;
                 return {
@@ -122594,15 +123453,15 @@
                     zIndex: n.zIndices.header,
                     display: t ? "block" : "none",
                     "@media print": {
                         display: "none"
                     }
                 }
             }), ""),
-            Us = (0, Qe.Z)("div", {
+            kl = (0, Qe.Z)("div", {
                 target: "ezrtsby1"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     position: "absolute",
@@ -122610,867 +123469,180 @@
                     right: t.spacing.none,
                     left: t.spacing.none,
                     height: "0.125rem",
                     backgroundImage: "linear-gradient(90deg, ".concat(t.colors.red70, ", #fffd80)"),
                     zIndex: t.zIndices.header
                 }
             }), ""),
-            Vs = (0, Qe.Z)("div", {
+            Cl = (0, Qe.Z)("div", {
                 target: "ezrtsby0"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     position: "absolute",
                     top: t.spacing.sm,
                     right: t.spacing.twoXS,
                     display: "flex",
                     flexDirection: "row",
                     alignItems: "center"
                 }
             }), "");
-        const Hs = function(e) {
+        const Wl = function(e) {
             let {
                 isStale: n,
                 children: r
             } = e;
             const {
                 wideMode: o,
                 embedded: i,
                 showToolbar: a,
                 showColoredLine: s
             } = t.useContext(je);
             let l = !0;
-            return i && (l = a || s), (0, ge.jsxs)(Fs, {
+            return i && (l = a || s), (0, ge.jsxs)(Tl, {
                 showHeader: l,
                 isWideMode: o,
                 tabIndex: -1,
                 isStale: n,
                 "data-testid": "stHeader",
-                children: [s && (0, ge.jsx)(Us, {
+                children: [s && (0, ge.jsx)(kl, {
                     "data-testid": "stDecoration",
                     id: "stDecoration"
-                }), a && (0, ge.jsx)(Vs, {
+                }), a && (0, ge.jsx)(Cl, {
                     "data-testid": "stToolbar",
                     children: r
                 })]
             })
         };
-        var Xs = {
-                default: "default",
-                full: "full",
-                auto: "auto"
-            },
-            Gs = {
-                default: "500px",
-                full: "100%",
-                auto: "auto"
-            },
-            $s = "closeButton",
-            Ks = "backdrop",
-            Ys = "escape";
-
-        function Zs(e, t) {
-            var n = Object.keys(e);
-            if (Object.getOwnPropertySymbols) {
-                var r = Object.getOwnPropertySymbols(e);
-                t && (r = r.filter((function(t) {
-                    return Object.getOwnPropertyDescriptor(e, t).enumerable
-                }))), n.push.apply(n, r)
-            }
-            return n
-        }
-
-        function Js(e) {
-            for (var t = 1; t < arguments.length; t++) {
-                var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? Zs(Object(n), !0).forEach((function(t) {
-                    Qs(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Zs(Object(n)).forEach((function(t) {
-                    Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
-                }))
-            }
-            return e
-        }
-
-        function Qs(e, t, n) {
-            return t in e ? Object.defineProperty(e, t, {
-                value: n,
-                enumerable: !0,
-                configurable: !0,
-                writable: !0
-            }) : e[t] = n, e
-        }
-        var el = (0, at.zo)("div", (function(e) {
-            return {
-                position: "fixed",
-                overflow: "auto",
-                right: 0,
-                bottom: 0,
-                top: 0,
-                left: 0,
-                pointerEvents: e.$isOpen ? "auto" : "none"
-            }
-        }));
-        el.displayName = "Root", el.displayName = "Root";
-        var tl = (0, at.zo)("div", (function(e) {
-            var t = e.$animate,
-                n = e.$isOpen,
-                r = e.$isVisible,
-                o = e.$theme,
-                i = {
-                    transitionProperty: "opacity",
-                    transitionDuration: o.animation.timing400,
-                    transitionTimingFunction: o.animation.easeOutCurve
-                };
-            return Js({
-                display: "flex",
-                alignItems: "center",
-                justifyContent: "center",
-                width: "100%",
-                minHeight: "100%",
-                userSelect: "none",
-                pointerEvents: "auto",
-                backgroundColor: "rgba(0, 0, 0, 0.5)",
-                WebkitTapHighlightColor: "transparent",
-                opacity: r && n ? 1 : 0
-            }, t ? i : null)
-        }));
-        tl.displayName = "DialogContainer", tl.displayName = "DialogContainer";
-        var nl = (0, at.zo)("div", (function(e) {
-            var t = e.$animate,
-                n = e.$isOpen,
-                r = e.$isVisible,
-                o = e.$size,
-                i = e.$theme;
-            return Js(Js(Js({
-                position: "relative",
-                backgroundColor: i.colors.backgroundPrimary,
-                borderTopLeftRadius: i.borders.radius500,
-                borderTopRightRadius: i.borders.radius500,
-                borderBottomRightRadius: i.borders.radius500,
-                borderBottomLeftRadius: i.borders.radius500,
-                marginLeft: i.sizing.scale600,
-                marginTop: i.sizing.scale600,
-                marginRight: i.sizing.scale600,
-                marginBottom: i.sizing.scale600
-            }, function(e) {
-                var t = {
-                    maxWidth: "100%",
-                    width: null
-                };
-                return "number" === typeof e ? t.width = "".concat(e, "px") : Xs[e] ? t.width = Gs[e] : "string" === typeof e && (t.width = e), e === Xs.full && (t.alignSelf = "stretch"), t
-            }(o)), {}, {
-                opacity: r && n ? 1 : 0,
-                transform: r ? "translateY(0)" : "translateY(20px)"
-            }, t ? {
-                transitionProperty: "opacity, transform",
-                transitionDuration: i.animation.timing400,
-                transitionTimingFunction: i.animation.easeOutCurve
-            } : null), {}, {
-                userSelect: "text",
-                pointerEvents: n ? "all" : "none",
-                ":focus": {
-                    outline: "none"
-                }
-            })
-        }));
-        nl.displayName = "Dialog", nl.displayName = "Dialog";
-        var rl = (0, at.zo)("button", (function(e) {
-            var t, n = e.$theme,
-                r = e.$isFocusVisible,
-                o = "rtl" === n.direction ? "left" : "right";
-            return Qs(t = {
-                background: "transparent",
-                outline: 0,
-                paddingLeft: 0,
-                paddingTop: 0,
-                paddingRight: 0,
-                paddingBottom: 0,
-                color: n.colors.modalCloseColor,
-                transitionProperty: "color, border-color",
-                transitionDuration: n.animation.timing200,
-                borderLeftWidth: "1px",
-                borderRightWidth: "1px",
-                borderTopWidth: "1px",
-                borderBottomWidth: "1px",
-                borderLeftStyle: "solid",
-                borderRightStyle: "solid",
-                borderTopStyle: "solid",
-                borderBottomStyle: "solid",
-                borderLeftColor: "transparent",
-                borderRightColor: "transparent",
-                borderTopColor: "transparent",
-                borderBottomColor: "transparent",
-                ":hover": {
-                    color: n.colors.modalCloseColorHover
-                },
-                ":focus": {
-                    outline: r ? "3px solid ".concat(n.colors.accent) : "none"
-                },
-                position: "absolute",
-                top: n.sizing.scale500
-            }, o, n.sizing.scale500), Qs(t, "width", n.sizing.scale800), Qs(t, "height", n.sizing.scale800), Qs(t, "display", "flex"), Qs(t, "justifyContent", "center"), Qs(t, "alignItems", "center"), Qs(t, "cursor", "pointer"), t
-        }));
-        rl.displayName = "Close", rl.displayName = "Close";
-        var ol = (0, at.zo)("div", (function(e) {
-            var t, n = e.$theme,
-                r = "rtl" === n.direction ? "marginRight" : "marginLeft",
-                o = "rtl" === n.direction ? "marginLeft" : "marginRight";
-            return Js(Js({}, n.typography.font550), {}, (Qs(t = {
-                color: n.colors.contentPrimary,
-                marginTop: n.sizing.scale900,
-                marginBottom: n.sizing.scale600
-            }, r, n.sizing.scale800), Qs(t, o, n.sizing.scale900), t))
-        }));
-        ol.displayName = "ModalHeader", ol.displayName = "ModalHeader";
-        var il = (0, at.zo)("div", (function(e) {
-            var t = e.$theme;
-            return Js(Js({}, t.typography.font200), {}, {
-                color: t.colors.contentSecondary,
-                marginTop: t.sizing.scale600,
-                marginLeft: t.sizing.scale800,
-                marginRight: t.sizing.scale800,
-                marginBottom: t.sizing.scale700
-            })
-        }));
-        il.displayName = "ModalBody", il.displayName = "ModalBody";
-        var al = (0, at.zo)("div", (function(e) {
-            var t = e.$theme;
-            return Js(Js({}, t.typography.font200), {}, {
-                marginTop: t.sizing.scale700,
-                marginLeft: t.sizing.scale800,
-                marginRight: t.sizing.scale800,
-                paddingTop: t.sizing.scale500,
-                paddingBottom: t.sizing.scale500,
-                textAlign: "rtl" === t.direction ? "left" : "right"
-            })
-        }));
-        al.displayName = "ModalFooter", al.displayName = "ModalFooter";
-        var sl = __webpack_require__(2989),
-            ll = __webpack_require__(99282),
-            cl = __webpack_require__(42450);
+        var Nl = __webpack_require__(8984),
+            Ll = __webpack_require__.n(Nl);
 
-        function ul() {
-            return t.createElement("svg", {
-                width: "10",
-                height: "10",
-                viewBox: "0 0 10 10",
-                style: {
-                    stroke: "currentColor"
-                },
-                xmlns: "http://www.w3.org/2000/svg"
-            }, t.createElement("path", {
-                d: "M9 1L5 5M1 9L5 5M5 5L1 1M5 5L9 9",
-                strokeWidth: "2",
-                strokeLinecap: "round"
-            }))
-        }
-
-        function pl(e) {
-            return pl = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
-                return typeof e
-            } : function(e) {
-                return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-            }, pl(e)
-        }
-
-        function dl() {
-            return dl = Object.assign ? Object.assign.bind() : function(e) {
+        function Il() {
+            return Il = Object.assign || function(e) {
                 for (var t = 1; t < arguments.length; t++) {
                     var n = arguments[t];
                     for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
                 }
                 return e
-            }, dl.apply(this, arguments)
+            }, Il.apply(this, arguments)
         }
 
-        function bl(e, t) {
-            return function(e) {
-                if (Array.isArray(e)) return e
-            }(e) || function(e, t) {
-                var n = null == e ? null : "undefined" !== typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
-                if (null == n) return;
-                var r, o, i = [],
-                    a = !0,
-                    s = !1;
-                try {
-                    for (n = n.call(e); !(a = (r = n.next()).done) && (i.push(r.value), !t || i.length !== t); a = !0);
-                } catch (l) {
-                    s = !0, o = l
-                } finally {
-                    try {
-                        a || null == n.return || n.return()
-                    } finally {
-                        if (s) throw o
-                    }
-                }
-                return i
-            }(e, t) || function(e, t) {
-                if (!e) return;
-                if ("string" === typeof e) return fl(e, t);
-                var n = Object.prototype.toString.call(e).slice(8, -1);
-                "Object" === n && e.constructor && (n = e.constructor.name);
-                if ("Map" === n || "Set" === n) return Array.from(e);
-                if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return fl(e, t)
-            }(e, t) || function() {
-                throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
-            }()
-        }
-
-        function fl(e, t) {
-            (null == t || t > e.length) && (t = e.length);
-            for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
-            return r
-        }
-
-        function hl(e, t) {
-            for (var n = 0; n < t.length; n++) {
-                var r = t[n];
-                r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, r.key, r)
-            }
-        }
-
-        function ml(e, t) {
-            return ml = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
-                return e.__proto__ = t, e
-            }, ml(e, t)
-        }
-
-        function Ml(e) {
-            var t = function() {
-                if ("undefined" === typeof Reflect || !Reflect.construct) return !1;
-                if (Reflect.construct.sham) return !1;
-                if ("function" === typeof Proxy) return !0;
-                try {
-                    return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
-                } catch (e) {
-                    return !1
-                }
-            }();
-            return function() {
-                var n, r = gl(e);
-                if (t) {
-                    var o = gl(this).constructor;
-                    n = Reflect.construct(r, arguments, o)
-                } else n = r.apply(this, arguments);
-                return function(e, t) {
-                    if (t && ("object" === pl(t) || "function" === typeof t)) return t;
-                    if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
-                    return Ol(e)
-                }(this, n)
-            }
-        }
-
-        function Ol(e) {
-            if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
-            return e
-        }
-
-        function gl(e) {
-            return gl = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
-                return e.__proto__ || Object.getPrototypeOf(e)
-            }, gl(e)
-        }
-
-        function zl(e, t, n) {
-            return t in e ? Object.defineProperty(e, t, {
-                value: n,
-                enumerable: !0,
-                configurable: !0,
-                writable: !0
-            }) : e[t] = n, e
-        }
-        var yl = function(e) {
-            ! function(e, t) {
-                if ("function" !== typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
-                e.prototype = Object.create(t && t.prototype, {
-                    constructor: {
-                        value: e,
-                        writable: !0,
-                        configurable: !0
-                    }
-                }), Object.defineProperty(e, "prototype", {
-                    writable: !1
-                }), t && ml(e, t)
-            }(a, e);
-            var n, r, o, i = Ml(a);
-
-            function a() {
-                var e;
-                ! function(e, t) {
-                    if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
-                }(this, a);
-                for (var n = arguments.length, r = new Array(n), o = 0; o < n; o++) r[o] = arguments[o];
-                return zl(Ol(e = i.call.apply(i, [this].concat(r))), "animateOutTimer", void 0), zl(Ol(e), "animateStartTimer", void 0), zl(Ol(e), "dialogContainerRef", t.createRef()), zl(Ol(e), "lastFocus", null), zl(Ol(e), "lastMountNodeOverflowStyle", null), zl(Ol(e), "rootRef", t.createRef()), zl(Ol(e), "state", {
-                    isVisible: !1,
-                    mounted: !1,
-                    isFocusVisible: !1
-                }), zl(Ol(e), "handleFocus", (function(t) {
-                    (0, lt.E)(t) && e.setState({
-                        isFocusVisible: !0
-                    })
-                })), zl(Ol(e), "handleBlur", (function(t) {
-                    !1 !== e.state.isFocusVisible && e.setState({
-                        isFocusVisible: !1
-                    })
-                })), zl(Ol(e), "onEscape", (function() {
-                    e.props.closeable && e.triggerClose(Ys)
-                })), zl(Ol(e), "onDocumentClick", (function(t) {
-                    t.target && t.target instanceof HTMLElement && t.target.contains(e.dialogContainerRef.current) && e.onBackdropClick()
-                })), zl(Ol(e), "onBackdropClick", (function() {
-                    e.props.closeable && e.triggerClose(Ks)
-                })), zl(Ol(e), "onCloseClick", (function() {
-                    e.triggerClose($s)
-                })), zl(Ol(e), "animateOutComplete", (function() {
-                    e.setState({
-                        isVisible: !1
-                    })
-                })), e
-            }
-            return n = a, r = [{
-                key: "componentDidMount",
-                value: function() {
-                    this.setState({
-                        mounted: !0
-                    })
-                }
-            }, {
-                key: "componentWillUnmount",
-                value: function() {
-                    this.resetMountNodeScroll(), this.clearTimers()
-                }
-            }, {
-                key: "componentDidUpdate",
-                value: function(e, t) {
-                    var n = this.props.isOpen;
-                    (n !== e.isOpen || n && this.state.mounted && !t.mounted) && (n ? this.didOpen() : this.didClose())
-                }
-            }, {
-                key: "disableMountNodeScroll",
-                value: function() {
-                    var e = this.getMountNode();
-                    this.lastMountNodeOverflowStyle = e.style.overflow || "", e.style.overflow = "hidden"
-                }
-            }, {
-                key: "resetMountNodeScroll",
-                value: function() {
-                    var e = this.getMountNode(),
-                        t = this.lastMountNodeOverflowStyle;
-                    e && null !== t && ("hidden" === e.style.overflow && (e.style.overflow = t || ""), this.lastMountNodeOverflowStyle = null)
-                }
-            }, {
-                key: "clearTimers",
-                value: function() {
-                    this.animateOutTimer && clearTimeout(this.animateOutTimer), this.animateStartTimer && cancelAnimationFrame(this.animateStartTimer)
-                }
-            }, {
-                key: "didOpen",
-                value: function() {
-                    var e = this,
-                        t = this.rootRef.current;
-                    t && (t.scrollTop = 0), this.clearTimers(), this.disableMountNodeScroll(), this.animateStartTimer = requestAnimationFrame((function() {
-                        e.setState({
-                            isVisible: !0
-                        })
-                    }))
-                }
-            }, {
-                key: "didClose",
-                value: function() {
-                    this.resetMountNodeScroll(), this.animateOutTimer = setTimeout(this.animateOutComplete, 500)
-                }
-            }, {
-                key: "triggerClose",
-                value: function(e) {
-                    this.props.onClose && e && this.props.onClose({
-                        closeSource: e
-                    })
-                }
-            }, {
-                key: "getSharedProps",
-                value: function() {
-                    var e = this.props,
-                        t = e.animate,
-                        n = e.isOpen,
-                        r = e.size,
-                        o = e.role,
-                        i = e.closeable;
-                    return {
-                        $animate: t,
-                        $isVisible: this.state.isVisible,
-                        $isOpen: !!n,
-                        $size: r,
-                        $role: o,
-                        $closeable: !!i,
-                        $isFocusVisible: this.state.isFocusVisible
-                    }
-                }
-            }, {
-                key: "getMountNode",
-                value: function() {
-                    var e = this.props.mountNode;
-                    return e || document.body
-                }
-            }, {
-                key: "getChildren",
-                value: function() {
-                    var e = this.props.children;
-                    return "function" === typeof e ? e() : e
-                }
-            }, {
-                key: "renderModal",
-                value: function() {
-                    var e = this,
-                        n = this.props,
-                        r = n.overrides,
-                        o = void 0 === r ? {} : r,
-                        i = n.closeable,
-                        a = n.role,
-                        s = n.autoFocus,
-                        l = n.focusLock,
-                        c = n.returnFocus,
-                        u = o.Root,
-                        p = o.Dialog,
-                        d = o.DialogContainer,
-                        b = o.Close,
-                        f = bl((0, st.jb)(u, el), 2),
-                        h = f[0],
-                        m = f[1],
-                        M = bl((0, st.jb)(d, tl), 2),
-                        O = M[0],
-                        g = M[1],
-                        z = bl((0, st.jb)(p, nl), 2),
-                        y = z[0],
-                        A = z[1],
-                        v = bl((0, st.jb)(b, rl), 2),
-                        w = v[0],
-                        S = v[1],
-                        q = this.getSharedProps(),
-                        E = this.getChildren();
-                    return t.createElement(ll.R.Consumer, null, (function(n) {
-                        return t.createElement(sl.ZP, {
-                            disabled: !l,
-                            crossFrame: !1,
-                            returnFocus: c,
-                            autoFocus: s
-                        }, t.createElement(h, dl({
-                            "data-baseweb": "modal",
-                            ref: e.rootRef
-                        }, q, m), t.createElement(O, dl({
-                            ref: e.dialogContainerRef
-                        }, q, g), t.createElement(y, dl({
-                            tabIndex: -1,
-                            "aria-modal": !0,
-                            "aria-label": "dialog",
-                            role: a
-                        }, q, A), E, i ? t.createElement(w, dl({
-                            "aria-label": n.modal.close,
-                            onClick: e.onCloseClick
-                        }, q, S, {
-                            onFocus: (0, lt.Ah)(S, e.handleFocus),
-                            onBlur: (0, lt.Z5)(S, e.handleBlur)
-                        }), t.createElement(ul, null)) : null))))
-                    }))
-                }
-            }, {
-                key: "render",
-                value: function() {
-                    return this.state.mounted && (this.props.isOpen || this.state.isVisible) ? t.createElement(cl.Z, {
-                        onEscape: this.onEscape,
-                        onDocumentClick: this.onDocumentClick,
-                        mountNode: this.props.mountNode
-                    }, this.renderModal()) : null
-                }
-            }], r && hl(n.prototype, r), o && hl(n, o), Object.defineProperty(n, "prototype", {
-                writable: !1
-            }), a
-        }(t.Component);
-        zl(yl, "defaultProps", {
-            animate: !0,
-            autoFocus: !0,
-            focusLock: !0,
-            returnFocus: !0,
-            closeable: !0,
-            name: "dialog",
-            isOpen: !1,
-            overrides: {},
-            role: "dialog",
-            size: Xs.default
-        });
-        const Al = yl;
-        var vl = __webpack_require__(96825),
-            wl = __webpack_require__.n(vl);
-        const Sl = (0, Qe.Z)("span", {
-            target: "e18cebhv0"
-        })((e => {
-            let {
-                theme: t
-            } = e;
-            return {
-                marginRight: t.spacing.twoXS
-            }
-        }), "");
-
-        function ql(e) {
-            let {
-                children: t
-            } = e;
-            const {
-                genericFonts: n,
-                fontSizes: r,
-                spacing: o
-            } = (0, Ee.u)();
-            return (0, ge.jsx)(ol, {
-                style: {
-                    marginTop: o.none,
-                    marginLeft: o.none,
-                    marginRight: o.none,
-                    marginBottom: o.none,
-                    paddingTop: o.twoXL,
-                    paddingRight: o.twoXL,
-                    paddingBottom: o.md,
-                    paddingLeft: o.twoXL,
-                    fontFamily: n.bodyFont,
-                    fontSize: r.xl,
-                    fontWeight: 600,
-                    margin: o.none,
-                    lineHeight: 1.5,
-                    textTransform: "none",
-                    display: "flex",
-                    alignItems: "center",
-                    maxHeight: "80vh",
-                    flexDirection: "row"
-                },
-                children: t
-            })
-        }
-
-        function El(e) {
-            let {
-                children: t
-            } = e;
-            const {
-                colors: n,
-                fontSizes: r,
-                spacing: o
-            } = (0, Ee.u)();
-            return (0, ge.jsx)(il, {
-                style: {
-                    marginTop: o.none,
-                    marginLeft: o.none,
-                    marginRight: o.none,
-                    marginBottom: o.none,
-                    paddingTop: o.md,
-                    paddingRight: o.twoXL,
-                    paddingBottom: o.twoXL,
-                    paddingLeft: o.twoXL,
-                    color: n.bodyText,
-                    fontSize: r.md,
-                    overflowY: "auto"
-                },
-                children: t
-            })
-        }
-
-        function _l(e) {
-            let {
-                children: t
-            } = e;
-            const {
-                spacing: n
-            } = (0, Ee.u)();
-            return (0, ge.jsx)(al, {
-                style: {
-                    marginTop: n.none,
-                    marginLeft: n.none,
-                    marginRight: n.none,
-                    marginBottom: n.none,
-                    paddingTop: n.md,
-                    paddingRight: n.md,
-                    paddingBottom: n.md,
-                    paddingLeft: n.md
-                },
-                children: (0, ge.jsx)("div", {
-                    className: "ModalBody",
-                    children: t
-                })
-            })
-        }
-        const xl = e => (0, ge.jsx)(Sl, {
-            children: (0, ge.jsx)(an.ZP, {
-                ...e
-            })
-        });
-        const Rl = function(e) {
-            const {
-                spacing: t,
-                radii: n,
-                colors: r
-            } = (0, Ee.u)(), o = {
-                Root: {
-                    style: {
-                        background: r.darkenedBgMix25
-                    },
-                    props: {
-                        "data-testid": "stModal"
-                    }
-                },
-                DialogContainer: {
-                    style: {
-                        alignItems: "start",
-                        paddingTop: "3rem"
-                    }
-                },
-                Dialog: {
-                    style: {
-                        borderBottomRadius: n.xl,
-                        borderTopRadius: n.xl,
-                        borderLeftRadius: n.xl,
-                        borderRightRadius: n.xl,
-                        minWidth: "20rem"
-                    }
-                },
-                Close: {
-                    style: {
-                        top: "calc(".concat(t.twoXL, " + .375rem)"),
-                        right: t.twoXL
-                    }
-                }
-            }, i = wl()(o, e.overrides);
-            return (0, ge.jsx)(Al, {
-                ...e,
-                overrides: i
-            })
-        };
-        var Tl = __webpack_require__(8984),
-            kl = __webpack_require__.n(Tl);
-
-        function Cl() {
-            return Cl = Object.assign || function(e) {
-                for (var t = 1; t < arguments.length; t++) {
-                    var n = arguments[t];
-                    for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
-                }
-                return e
-            }, Cl.apply(this, arguments)
-        }
-
-        function Wl(e, t) {
+        function Pl(e, t) {
             if (null == e) return {};
             var n, r, o = function(e, t) {
                 if (null == e) return {};
                 var n, r, o = {},
                     i = Object.keys(e);
                 for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || (o[n] = e[n]);
                 return o
             }(e, t);
             if (Object.getOwnPropertySymbols) {
                 var i = Object.getOwnPropertySymbols(e);
                 for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
             }
             return o
         }
-        var Nl = (0, t.forwardRef)((function(e, n) {
+        var Dl = (0, t.forwardRef)((function(e, n) {
             var r = e.color,
                 o = void 0 === r ? "currentColor" : r,
                 i = e.size,
                 a = void 0 === i ? 24 : i,
-                s = Wl(e, ["color", "size"]);
-            return t.createElement("svg", Cl({
+                s = Pl(e, ["color", "size"]);
+            return t.createElement("svg", Il({
                 ref: n,
                 xmlns: "http://www.w3.org/2000/svg",
                 width: a,
                 height: a,
                 viewBox: "0 0 24 24",
                 fill: "none",
                 stroke: o,
                 strokeWidth: "2",
                 strokeLinecap: "round",
                 strokeLinejoin: "round"
             }, s), t.createElement("polyline", {
                 points: "15 18 9 12 15 6"
             }))
         }));
-        Nl.propTypes = {
-            color: kl().string,
-            size: kl().oneOfType([kl().string, kl().number])
-        }, Nl.displayName = "ChevronLeft";
-        const Ll = Nl;
-        var Il = __webpack_require__(33746);
-        const Pl = (0, Qe.Z)("div", {
+        Dl.propTypes = {
+            color: Ll().string,
+            size: Ll().oneOfType([Ll().string, Ll().number])
+        }, Dl.displayName = "ChevronLeft";
+        const Bl = Dl;
+        var jl = __webpack_require__(33746);
+        const Fl = (0, Qe.Z)("div", {
                 target: "e1x90zqc14"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     marginBottom: t.spacing.sm
                 }
             }), ""),
-            Dl = (0, Qe.Z)("textarea", {
+            Ul = (0, Qe.Z)("textarea", {
                 target: "e1x90zqc13"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     width: t.sizes.full,
                     fontFamily: t.genericFonts.codeFont,
                     fontSize: t.fontSizes.sm,
                     height: "6rem"
                 }
             }), ""),
-            Bl = (0, Qe.Z)("span", {
+            Vl = (0, Qe.Z)("span", {
                 target: "e1x90zqc12"
             })((() => ({
                 "&::first-letter": {
                     textDecoration: "underline"
                 }
             })), ""),
-            jl = (0, Qe.Z)(Ll, {
+            Hl = (0, Qe.Z)(Bl, {
                 target: "e1x90zqc11"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     cursor: "pointer",
                     marginRight: t.spacing.lg
                 }
             }), ""),
-            Fl = (0, Qe.Z)("div", {
+            Xl = (0, Qe.Z)("div", {
                 target: "e1x90zqc10"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     display: "grid",
                     gap: t.spacing.twoXL,
                     gridTemplateColumns: "1fr 1fr",
                     margin: 0,
                     padding: 0
                 }
             }), ""),
-            Ul = (0, Qe.Z)("div", {
+            Gl = (0, Qe.Z)("div", {
                 target: "e1x90zqc9"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     gridColumnStart: 1,
                     gridColumnEnd: -1,
                     display: "grid",
                     gap: t.spacing.xs
                 }
             }), ""),
-            Vl = (0, Qe.Z)("h2", {
+            $l = (0, Qe.Z)("h2", {
                 target: "e1x90zqc8"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     paddingBottom: 0,
@@ -123485,50 +123657,50 @@
                     gridAutoFlow: "row",
                     gap: t.spacing.xs,
                     "&:first-of-type": {
                         marginTop: 0
                     }
                 }
             }), ""),
-            Hl = (0, Qe.Z)("label", {
+            Kl = (0, Qe.Z)("label", {
                 target: "e1x90zqc7"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     paddingBottom: 0,
                     paddingTop: 0,
                     marginBottom: 0,
                     marginTop: 0,
                     lineHeight: 1.25,
                     fontSize: t.fontSizes.sm
                 }
             }), ""),
-            Xl = (0, Qe.Z)(Il.x, {
+            Yl = (0, Qe.Z)(jl.x, {
                 target: "e1x90zqc6"
             })((() => ({
                 display: "block",
                 paddingBottom: 0,
                 paddingTop: 0,
                 marginBottom: 0,
                 marginTop: 0,
                 lineHeight: 1.5
             })), ""),
-            Gl = (0, Qe.Z)("div", {
+            Zl = (0, Qe.Z)("div", {
                 target: "e1x90zqc4"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     marginTop: t.spacing.md
                 }
             }), ""),
-            $l = (0, Qe.Z)("input", {
+            Jl = (0, Qe.Z)("input", {
                 target: "e1x90zqc3"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     marginRight: t.spacing.xs,
@@ -123557,90 +123729,90 @@
                         }
                     },
                     "&:disabled": {
                         backgroundColor: t.colors.secondaryBg
                     }
                 }
             }), ""),
-            Kl = (0, Qe.Z)("div", {
+            Ql = (0, Qe.Z)("div", {
                 target: "e1x90zqc2"
             })((() => ({
                 "& > ul": {
                     paddingLeft: "1.4rem"
                 }
             })), ""),
-            Yl = (0, Qe.Z)("div", {
+            ec = (0, Qe.Z)("div", {
                 target: "e1x90zqc1"
             })((() => ({
                 padding: "0 0 1rem 0",
                 overflowY: "scroll"
             })), ""),
-            Zl = (0, Qe.Z)("a", {
+            tc = (0, Qe.Z)("a", {
                 target: "e1x90zqc0"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     color: "".concat(t.colors.linkText, " !important"),
                     "&:hover": {
                         color: "".concat((0, _e._j)(t.colors.linkText, .15), " !important")
                     }
                 }
             }), "");
-        class Jl extends t.PureComponent {
+        class nc extends t.PureComponent {
             constructor(e) {
                 super(e), this.keyHandlers = void 0, this.rerun = () => {
                     this.props.onRerun(!1)
                 }, this.alwaysRerun = () => {
                     this.props.onRerun(!0)
                 }, this.keyHandlers = {
                     a: this.alwaysRerun
                 }
             }
             render() {
                 return (0, ge.jsx)(Le.HotKeys, {
                     handlers: this.keyHandlers,
                     attach: window,
                     focused: !0,
-                    children: (0, ge.jsxs)(Rl, {
+                    children: (0, ge.jsxs)(sr, {
                         isOpen: !0,
                         onClose: this.props.onClose,
-                        children: [(0, ge.jsx)(ql, {
+                        children: [(0, ge.jsx)(rr, {
                             children: "App changed"
-                        }), (0, ge.jsx)(El, {
+                        }), (0, ge.jsx)(or, {
                             children: (0, ge.jsx)("div", {
                                 children: "The source files for this app have changed on disk."
                             })
-                        }), (0, ge.jsxs)(_l, {
-                            children: [this.props.allowRunOnSave ? (0, ge.jsx)(xl, {
+                        }), (0, ge.jsxs)(ir, {
+                            children: [this.props.allowRunOnSave ? (0, ge.jsx)(ar, {
                                 kind: sn.nW.TERTIARY,
                                 onClick: this.alwaysRerun,
-                                children: (0, ge.jsx)(Bl, {
+                                children: (0, ge.jsx)(Vl, {
                                     children: "Always rerun"
                                 })
-                            }) : null, (0, ge.jsx)(xl, {
+                            }) : null, (0, ge.jsx)(ar, {
                                 kind: sn.nW.SECONDARY,
                                 onClick: this.rerun,
-                                children: (0, ge.jsx)(Bl, {
+                                children: (0, ge.jsx)(Vl, {
                                     children: "Rerun"
                                 })
                             })]
                         })]
                     })
                 })
             }
         }
-        const Ql = "https://streamlit.io",
-            ec = "https://docs.streamlit.io/streamlit-community-cloud/get-started",
-            tc = "https://docs.streamlit.io/knowledge-base/tutorials/deploy";
-        var nc = __webpack_require__(97965);
-        class rc extends t.PureComponent {
+        const rc = "https://streamlit.io",
+            oc = "https://docs.streamlit.io/streamlit-community-cloud/get-started",
+            ic = "https://docs.streamlit.io/knowledge-base/tutorials/deploy";
+        var ac = __webpack_require__(97965);
+        class sc extends t.PureComponent {
             constructor(e) {
-                super(e), this.activeSettings = void 0, this.context = void 0, this.renderThemeCreatorButton = () => this.props.developerMode && (0, ge.jsx)(Gl, {
+                super(e), this.activeSettings = void 0, this.context = void 0, this.renderThemeCreatorButton = () => this.props.developerMode && (0, ge.jsx)(Zl, {
                     "data-testid": "edit-theme",
                     children: (0, ge.jsx)(an.ZP, {
                         onClick: this.props.openThemeCreator,
                         kind: sn.nW.SECONDARY,
                         children: "Edit active theme"
                     })
                 }), this.changeSingleSetting = (e, t) => {
@@ -123669,55 +123841,55 @@
                     ...this.props.settings
                 }, this.activeSettings = {
                     ...this.props.settings
                 }
             }
             render() {
                 const e = this.context.availableThemes.findIndex((e => e.name === this.context.activeTheme.name));
-                return (0, ge.jsxs)(Rl, {
+                return (0, ge.jsxs)(sr, {
                     animate: this.props.animateModal,
                     isOpen: !0,
                     onClose: this.handleCancelButtonClick,
-                    children: [(0, ge.jsx)(ql, {
+                    children: [(0, ge.jsx)(rr, {
                         children: "Settings"
-                    }), (0, ge.jsx)(El, {
-                        children: (0, ge.jsxs)(Fl, {
+                    }), (0, ge.jsx)(or, {
+                        children: (0, ge.jsxs)(Xl, {
                             children: [this.props.allowRunOnSave && (0, ge.jsx)(t.Fragment, {
-                                children: (0, ge.jsxs)(Ul, {
-                                    children: [(0, ge.jsx)(Vl, {
+                                children: (0, ge.jsxs)(Gl, {
+                                    children: [(0, ge.jsx)($l, {
                                         children: "Development"
                                     }), (0, ge.jsxs)("label", {
-                                        children: [(0, ge.jsx)($l, {
+                                        children: [(0, ge.jsx)(Jl, {
                                             disabled: !this.props.isServerConnected,
                                             type: "checkbox",
                                             name: "runOnSave",
                                             checked: this.state.runOnSave && this.props.isServerConnected,
                                             onChange: this.handleCheckboxChange
                                         }), " ", "Run on save"]
-                                    }), (0, ge.jsx)(Xl, {
+                                    }), (0, ge.jsx)(Yl, {
                                         children: "Automatically updates the app when the underlying code is updated."
                                     })]
                                 })
-                            }), (0, ge.jsxs)(Ul, {
-                                children: [(0, ge.jsx)(Vl, {
+                            }), (0, ge.jsxs)(Gl, {
+                                children: [(0, ge.jsx)($l, {
                                     children: "Appearance"
                                 }), (0, ge.jsxs)("label", {
-                                    children: [(0, ge.jsx)($l, {
+                                    children: [(0, ge.jsx)(Jl, {
                                         type: "checkbox",
                                         name: "wideMode",
                                         checked: this.state.wideMode,
                                         onChange: this.handleCheckboxChange
                                     }), " ", "Wide mode"]
-                                }), (0, ge.jsx)(Xl, {
+                                }), (0, ge.jsx)(Yl, {
                                     children: "Turn on to make this app occupy the entire width of the screen"
                                 })]
-                            }), this.context.availableThemes.length && (0, ge.jsxs)(Ul, {
-                                children: [(0, ge.jsx)(Hl, {
+                            }), this.context.availableThemes.length && (0, ge.jsxs)(Gl, {
+                                children: [(0, ge.jsx)(Kl, {
                                     children: "Choose app theme, colors and fonts"
-                                }), (0, ge.jsx)(nc.ZP, {
+                                }), (0, ge.jsx)(ac.ZP, {
                                     options: this.context.availableThemes.map((e => e.name)),
                                     disabled: !1,
                                     onChange: this.handleThemeChange,
                                     value: e
                                 }), this.renderThemeCreatorButton()]
                             })]
                         })
@@ -123726,92 +123898,92 @@
             }
             componentDidMount() {
                 this.setState({
                     ...this.activeSettings
                 })
             }
         }
-        rc.contextType = Fe.E;
-        var oc = __webpack_require__(26218),
-            ic = __webpack_require__.n(oc),
-            ac = __webpack_require__(97910),
-            sc = __webpack_require__.n(ac),
-            lc = __webpack_require__(74516),
-            cc = __webpack_require__(44722);
-        const uc = (e, t) => (0, _e.NC)(e).toUpperCase(),
-            pc = e => ic()(Be.MA.FontFamily[e]),
-            dc = {
+        sc.contextType = Fe.E;
+        var lc = __webpack_require__(26218),
+            cc = __webpack_require__.n(lc),
+            uc = __webpack_require__(97910),
+            pc = __webpack_require__.n(uc),
+            dc = __webpack_require__(74516),
+            bc = __webpack_require__(44722);
+        const fc = (e, t) => (0, _e.NC)(e).toUpperCase(),
+            hc = e => cc()(Be.MA.FontFamily[e]),
+            mc = {
                 primaryColor: {
                     help: "Primary accent color for interactive elements.",
                     title: "Primary color",
-                    component: lc.Z,
-                    getValue: uc
+                    component: dc.Z,
+                    getValue: fc
                 },
                 backgroundColor: {
                     help: "Background color for the main content area.",
                     title: "Background color",
-                    component: lc.Z,
-                    getValue: uc
+                    component: dc.Z,
+                    getValue: fc
                 },
                 secondaryBackgroundColor: {
                     help: "Background color used for the sidebar and most interactive widgets.",
                     title: "Secondary background color",
-                    component: lc.Z,
-                    getValue: uc
+                    component: dc.Z,
+                    getValue: fc
                 },
                 textColor: {
                     help: "Color used for almost all text.",
                     title: "Text color",
-                    component: lc.Z,
-                    getValue: uc
+                    component: dc.Z,
+                    getValue: fc
                 },
                 font: {
                     help: "Font family for all text in the app, except code blocks.",
                     title: "Font family",
-                    options: Object.keys(Be.MA.FontFamily).map((e => ic()(e))),
-                    getValue: (e, t) => t.options && t.options.findIndex((t => t === pc(e))) || 0,
-                    component: nc.ZP
+                    options: Object.keys(Be.MA.FontFamily).map((e => cc()(e))),
+                    getValue: (e, t) => t.options && t.options.findIndex((t => t === hc(e))) || 0,
+                    component: ac.ZP
                 }
             },
-            bc = (e, t) => {
+            Mc = (e, t) => {
                 const n = e => "string" === typeof e ? e.toLowerCase() : e,
-                    r = sc()((0, ye.Zf)(t), n),
+                    r = pc()((0, ye.Zf)(t), n),
                     o = [];
-                return (e = sc()(e, n)).primaryColor !== r.primaryColor && o.push('primaryColor="'.concat(e.primaryColor, '"')), e.backgroundColor !== r.backgroundColor && o.push('backgroundColor="'.concat(e.backgroundColor, '"')), e.secondaryBackgroundColor !== r.secondaryBackgroundColor && o.push('secondaryBackgroundColor="'.concat(e.secondaryBackgroundColor, '"')), e.textColor !== r.textColor && o.push('textColor="'.concat(e.textColor, '"')), o
+                return (e = pc()(e, n)).primaryColor !== r.primaryColor && o.push('primaryColor="'.concat(e.primaryColor, '"')), e.backgroundColor !== r.backgroundColor && o.push('backgroundColor="'.concat(e.backgroundColor, '"')), e.secondaryBackgroundColor !== r.secondaryBackgroundColor && o.push('secondaryBackgroundColor="'.concat(e.secondaryBackgroundColor, '"')), e.textColor !== r.textColor && o.push('textColor="'.concat(e.textColor, '"')), o
             },
-            fc = e => {
+            Oc = e => {
                 const [n, r] = t.useState(!1), {
                     activeTheme: o,
                     addThemes: i,
                     setTheme: a
                 } = t.useContext(Fe.E), s = (0, ye.Zf)(o.emotion), l = (e, t) => {
                     (e => {
                         i([e]), a(e)
                     })((0, ye.jG)(ye.UO, {
                         ...s,
                         [e]: t
                     })), r(!1)
                 }, c = (e => {
                     const t = ["[theme]"],
-                        n = bc(e, cc.Wb.emotion),
-                        r = bc(e, cc.$_.emotion),
+                        n = Mc(e, bc.Wb.emotion),
+                        r = Mc(e, bc.$_.emotion),
                         o = n.length,
                         i = r.length;
                     if (o === i ? t.push(...n) : o < i ? t.push('base="light"', ...n) : t.push('base="dark"', ...r), e.font) {
-                        const n = pc(e.font).toLowerCase();
+                        const n = hc(e.font).toLowerCase();
                         t.push('font="'.concat(n, '"'))
                     }
                     return [...t, ""].join("\n")
                 })(s), u = e => {
                     let {
                         name: n,
                         value: r
                     } = e;
-                    const o = dc[n],
-                        i = o.component === lc.Z,
+                    const o = mc[n],
+                        i = o.component === dc.Z,
                         a = {
                             options: o.options || void 0,
                             showValue: i,
                             value: o.getValue(r, o)
                         };
                     return (0, ge.jsx)(t.Fragment, {
                         children: (0, ge.jsx)(o.component, {
@@ -123826,144 +123998,144 @@
                     }, n)
                 }, {
                     primaryColor: p,
                     textColor: d,
                     backgroundColor: b,
                     secondaryBackgroundColor: f
                 } = s;
-                return (0, ge.jsxs)(Rl, {
+                return (0, ge.jsxs)(sr, {
                     animate: !1,
                     isOpen: !0,
                     onClose: e.onClose,
-                    children: [(0, ge.jsxs)(ql, {
-                        children: [(0, ge.jsx)(jl, {
+                    children: [(0, ge.jsxs)(rr, {
+                        children: [(0, ge.jsx)(Hl, {
                             onClick: () => {
                                 e.backToSettings(!1)
                             },
                             "data-testid": "stThemeCreatorBack"
                         }), "Edit active theme"]
-                    }), (0, ge.jsx)(El, {
-                        children: (0, ge.jsxs)(Fl, {
+                    }), (0, ge.jsx)(or, {
+                        children: (0, ge.jsxs)(Xl, {
                             "data-testid": "stThemeCreatorDialog",
-                            children: [(0, ge.jsx)(Ul, {
-                                children: (0, ge.jsx)(Xl, {
+                            children: [(0, ge.jsx)(Gl, {
+                                children: (0, ge.jsx)(Yl, {
                                     children: "Changes made to the active theme will exist for the duration of a session. To discard changes and recover the original theme, refresh the page."
                                 })
                             }), (0, ge.jsx)(u, {
                                 name: "primaryColor",
                                 value: p
                             }), (0, ge.jsx)(u, {
                                 name: "backgroundColor",
                                 value: b
                             }), (0, ge.jsx)(u, {
                                 name: "textColor",
                                 value: d
                             }), (0, ge.jsx)(u, {
                                 name: "secondaryBackgroundColor",
                                 value: f
-                            }), (0, ge.jsx)(Ul, {
+                            }), (0, ge.jsx)(Gl, {
                                 children: (0, ge.jsx)(u, {
                                     name: "font",
                                     value: String(s.font)
                                 })
-                            }), (0, ge.jsx)(Ul, {
-                                children: (0, ge.jsxs)(Xl, {
+                            }), (0, ge.jsx)(Gl, {
+                                children: (0, ge.jsxs)(Yl, {
                                     children: ["To save your changes, copy your custom theme into the clipboard and paste it into the", (0, ge.jsx)("code", {
                                         children: "[theme]"
                                     }), " section of your", " ", (0, ge.jsx)("code", {
                                         children: ".streamlit/config.toml"
                                     }), " file."]
                                 })
-                            }), (0, ge.jsx)(Ul, {
+                            }), (0, ge.jsx)(Gl, {
                                 children: (0, ge.jsx)("div", {
                                     children: (0, ge.jsx)(an.ZP, {
                                         onClick: () => {
                                             navigator.clipboard.writeText(c), r(!0)
                                         },
                                         kind: sn.nW.SECONDARY,
                                         children: n ? (0, ge.jsxs)(t.Fragment, {
                                             children: ["Copied to clipboard ", (0, ge.jsx)(hn.Z, {
-                                                content: vn,
+                                                content: dr,
                                                 size: "lg",
                                                 color: o.emotion.colors.success
                                             })]
                                         }) : "Copy theme to clipboard"
                                     })
                                 })
                             })]
                         })
                     })]
                 })
             };
-        var hc = __webpack_require__(30067);
+        var gc = __webpack_require__(30067);
 
-        function mc(e, t) {
+        function zc(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function Mc(e) {
+        function yc(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? mc(Object(n), !0).forEach((function(t) {
-                    Oc(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : mc(Object(n)).forEach((function(t) {
+                t % 2 ? zc(Object(n), !0).forEach((function(t) {
+                    Ac(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : zc(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
 
-        function Oc(e, t, n) {
+        function Ac(e, t, n) {
             return t in e ? Object.defineProperty(e, t, {
                 value: n,
                 enumerable: !0,
                 configurable: !0,
                 writable: !0
             }) : e[t] = n, e
         }
-        var gc = (0, at.zo)("div", (function(e) {
-            return Mc({}, e.$theme.typography.LabelMedium)
+        var vc = (0, at.zo)("div", (function(e) {
+            return yc({}, e.$theme.typography.LabelMedium)
         }));
-        gc.displayName = "Action", gc.displayName = "Action";
-        var zc = (0, at.zo)("div", (function(e) {
+        vc.displayName = "Action", vc.displayName = "Action";
+        var wc = (0, at.zo)("div", (function(e) {
             var t = e.$theme;
-            return Mc({
+            return yc({
                 marginBottom: t.sizing.scale600,
                 color: t.colors.contentPrimary
             }, t.typography.ParagraphMedium)
         }));
-        zc.displayName = "Body", zc.displayName = "Body";
-        var yc = (0, at.zo)("div", (function(e) {
+        wc.displayName = "Body", wc.displayName = "Body";
+        var Sc = (0, at.zo)("div", (function(e) {
             var t = e.$theme;
             return {
                 marginLeft: t.sizing.scale600,
                 marginTop: t.sizing.scale600,
                 marginRight: t.sizing.scale600,
                 marginBottom: t.sizing.scale600
             }
         }));
-        yc.displayName = "Contents", yc.displayName = "Contents";
-        var Ac = (0, at.zo)("img", (function(e) {
+        Sc.displayName = "Contents", Sc.displayName = "Contents";
+        var qc = (0, at.zo)("img", (function(e) {
             var t = e.$theme;
             return {
                 borderTopLeftRadius: t.borders.surfaceBorderRadius,
                 borderTopRightRadius: t.borders.surfaceBorderRadius,
                 objectFit: "contain",
                 maxWidth: "100%"
             }
         }));
-        Ac.displayName = "HeaderImage", Ac.displayName = "HeaderImage";
-        var vc = (0, at.zo)("section", (function(e) {
+        qc.displayName = "HeaderImage", qc.displayName = "HeaderImage";
+        var Ec = (0, at.zo)("section", (function(e) {
             var t = e.$theme;
             return {
                 borderLeftWidth: "2px",
                 borderTopWidth: "2px",
                 borderRightWidth: "2px",
                 borderBottomWidth: "2px",
                 borderLeftStyle: "solid",
@@ -123978,205 +124150,205 @@
                 borderTopRightRadius: t.borders.radius400,
                 borderBottomLeftRadius: t.borders.radius400,
                 borderBottomRightRadius: t.borders.radius400,
                 backgroundColor: t.colors.backgroundPrimary,
                 overflow: "hidden"
             }
         }));
-        vc.displayName = "Root", vc.displayName = "Root";
-        var wc = (0, at.zo)("img", (function(e) {
+        Ec.displayName = "Root", Ec.displayName = "Root";
+        var _c = (0, at.zo)("img", (function(e) {
             var t = e.$theme;
-            return Mc(Mc({
+            return yc(yc({
                 float: "right",
                 height: t.sizing.scale2400,
                 width: t.sizing.scale2400,
                 objectFit: "cover",
                 borderTopLeftRadius: t.borders.surfaceBorderRadius,
                 borderTopRightRadius: t.borders.surfaceBorderRadius,
                 borderBottomLeftRadius: t.borders.surfaceBorderRadius,
                 borderBottomRightRadius: t.borders.surfaceBorderRadius
-            }, (0, hc.Qj)(t.borders.border200)), {}, {
+            }, (0, gc.Qj)(t.borders.border200)), {}, {
                 margin: "0 0 ".concat(t.sizing.scale500, " ").concat(t.sizing.scale500)
             })
         }));
-        wc.displayName = "Thumbnail", wc.displayName = "Thumbnail";
-        var Sc = (0, at.zo)("h1", (function(e) {
+        _c.displayName = "Thumbnail", _c.displayName = "Thumbnail";
+        var xc = (0, at.zo)("h1", (function(e) {
             var t = e.$theme;
-            return Mc(Mc({}, t.typography.HeadingSmall), {}, {
+            return yc(yc({}, t.typography.HeadingSmall), {}, {
                 color: t.colors.contentPrimary,
                 marginLeft: 0,
                 marginTop: 0,
                 marginRight: 0,
                 marginBottom: t.sizing.scale500,
                 paddingLeft: 0,
                 paddingTop: 0,
                 paddingRight: 0,
                 paddingBottom: 0
             })
         }));
-        Sc.displayName = "Title", Sc.displayName = "Title";
-        const qc = __webpack_require__.p + "static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg";
-        const Ec = __webpack_require__.p + "static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg";
-        const _c = function() {
+        xc.displayName = "Title", xc.displayName = "Title";
+        const Rc = __webpack_require__.p + "static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg";
+        const Tc = __webpack_require__.p + "static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg";
+        const kc = function() {
                 return {
                     title: "Unable to deploy",
                     body: (0, ge.jsxs)(ge.Fragment, {
                         children: [(0, ge.jsx)("p", {
                             children: "This Git tree is in a detached HEAD state."
                         }), (0, ge.jsx)("p", {
                             children: "Please commit the latest changes and push to GitHub to continue."
                         })]
                     })
                 }
             },
-            xc = (0, Qe.Z)("p", {
+            Cc = (0, Qe.Z)("p", {
                 target: "epbg7au0"
             })((() => ({
                 textAlign: "justify"
             })), "");
-        const Rc = function(e) {
+        const Wc = function(e) {
             return {
                 title: "Unable to deploy",
-                body: (0, ge.jsxs)(xc, {
+                body: (0, ge.jsxs)(Cc, {
                     children: ["The app\u2019s main file ", (0, ge.jsx)("code", {
                         children: e
                     }), " has not been pushed to GitHub. Please add it to continue."]
                 })
             }
         };
-        const Tc = function() {
+        const Nc = function() {
             return {
                 title: "Unable to deploy",
-                body: (0, ge.jsxs)(xc, {
+                body: (0, ge.jsxs)(Cc, {
                     children: ["The app\u2019s code is not connected to a remote GitHub repository. To deploy on Streamlit Community Cloud, please put your code in a GitHub repository and publish the current branch. Read more in", " ", (0, ge.jsx)("a", {
-                        href: ec,
+                        href: oc,
                         rel: "noopener noreferrer",
                         target: "_blank",
                         children: "our documentation"
                     }), "."]
                 })
             }
         };
-        const kc = function(e) {
+        const Lc = function(e) {
             const {
                 children: t,
                 onClose: n
             } = e;
-            return (0, ge.jsxs)(Rl, {
+            return (0, ge.jsxs)(sr, {
                 isOpen: !0,
                 closeable: !0,
                 onClose: n,
                 overrides: {
                     Dialog: {
                         style: {
                             width: "860px"
                         }
                     }
                 },
-                children: [(0, ge.jsx)(ql, {
+                children: [(0, ge.jsx)(rr, {
                     children: "Deploy this app"
-                }), (0, ge.jsx)(El, {
+                }), (0, ge.jsx)(or, {
                     children: t
                 })]
             })
         };
-        var Cc = t.createContext(0);
-        var Wc = ["children"],
-            Nc = ["action", "children", "hasThumbnail", "headerImage", "thumbnail", "title", "overrides"];
+        var Ic = t.createContext(0);
+        var Pc = ["children"],
+            Dc = ["action", "children", "hasThumbnail", "headerImage", "thumbnail", "title", "overrides"];
 
-        function Lc() {
-            return Lc = Object.assign ? Object.assign.bind() : function(e) {
+        function Bc() {
+            return Bc = Object.assign ? Object.assign.bind() : function(e) {
                 for (var t = 1; t < arguments.length; t++) {
                     var n = arguments[t];
                     for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
                 }
                 return e
-            }, Lc.apply(this, arguments)
+            }, Bc.apply(this, arguments)
         }
 
-        function Ic(e, t) {
+        function jc(e, t) {
             if (null == e) return {};
             var n, r, o = function(e, t) {
                 if (null == e) return {};
                 var n, r, o = {},
                     i = Object.keys(e);
                 for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || (o[n] = e[n]);
                 return o
             }(e, t);
             if (Object.getOwnPropertySymbols) {
                 var i = Object.getOwnPropertySymbols(e);
                 for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
             }
             return o
         }
-        var Pc = function(e) {
+        var Fc = function(e) {
             var n = e.children,
-                r = Ic(e, Wc),
+                r = jc(e, Pc),
                 o = ["", "h1", "h2", "h3", "h4", "h5", "h6"];
-            return t.createElement(Cc.Consumer, null, (function(e) {
-                return t.createElement(Sc, Lc({
+            return t.createElement(Ic.Consumer, null, (function(e) {
+                return t.createElement(xc, Bc({
                     $as: o[e]
                 }, r), n)
             }))
         };
 
-        function Dc(e) {
+        function Uc(e) {
             var n = e.action,
                 r = e.children,
                 o = e.hasThumbnail,
                 i = e.headerImage,
                 a = e.thumbnail,
                 s = e.title,
                 l = e.overrides,
-                c = Ic(e, Nc),
+                c = jc(e, Dc),
                 u = l.Action,
                 p = l.Body,
                 d = l.Contents,
                 b = l.HeaderImage,
                 f = l.Root,
                 h = l.Thumbnail,
                 m = l.Title,
-                M = (0, st.XG)(u) || gc,
-                O = (0, st.XG)(p) || zc,
-                g = (0, st.XG)(d) || yc,
-                z = (0, st.XG)(b) || Ac,
-                y = (0, st.XG)(f) || vc,
-                A = (0, st.XG)(h) || wc,
-                v = (0, st.XG)(m) || Pc,
+                M = (0, st.XG)(u) || vc,
+                O = (0, st.XG)(p) || wc,
+                g = (0, st.XG)(d) || Sc,
+                z = (0, st.XG)(b) || qc,
+                y = (0, st.XG)(f) || Ec,
+                A = (0, st.XG)(h) || _c,
+                v = (0, st.XG)(m) || Fc,
                 w = "string" === typeof i ? {
                     src: i
                 } : i,
                 S = o(e);
-            return t.createElement(y, Lc({
+            return t.createElement(y, Bc({
                 "data-baseweb": "card"
-            }, c, (0, st.ch)(f)), i && t.createElement(z, Lc({}, w, (0, st.ch)(b))), t.createElement(g, (0, st.ch)(d), a && t.createElement(A, Lc({
+            }, c, (0, st.ch)(f)), i && t.createElement(z, Bc({}, w, (0, st.ch)(b))), t.createElement(g, (0, st.ch)(d), a && t.createElement(A, Bc({
                 src: a
-            }, (0, st.ch)(h))), s && t.createElement(v, Lc({
+            }, (0, st.ch)(h))), s && t.createElement(v, Bc({
                 $hasThumbnail: S
             }, (0, st.ch)(m)), s), t.createElement(O, (0, st.ch)(p), r), n && t.createElement(M, (0, st.ch)(u), n)))
         }
-        Dc.defaultProps = {
+        Uc.defaultProps = {
             action: null,
             children: null,
             hasThumbnail: function(e) {
                 return !!e.thumbnail
             },
             overrides: {}
         };
-        const Bc = Dc;
-        const jc = function(e) {
+        const Vc = Uc;
+        const Hc = function(e) {
                 const {
                     colors: t,
                     spacing: n,
                     radii: r,
                     breakpoints: o
                 } = (0, Ee.u)(), {
                     children: i
                 } = e;
-                return (0, ge.jsx)(Bc, {
+                return (0, ge.jsx)(Vc, {
                     overrides: {
                         Root: {
                             style: {
                                 borderTopWidth: "1px",
                                 borderBottomWidth: "1px",
                                 borderLeftWidth: "1px",
                                 borderRightWidth: "1px",
@@ -124214,15 +124386,15 @@
                                 }
                             }
                         }
                     },
                     children: i
                 })
             },
-            Fc = (0, Qe.Z)("div", {
+            Xc = (0, Qe.Z)("div", {
                 target: "e97l2ve3"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     fontFamily: t.fonts.sansSerif,
@@ -124232,30 +124404,30 @@
                     marginTop: t.spacing.twoXL,
                     marginBottom: t.spacing.md,
                     ["@media (max-width: ".concat(t.breakpoints.md, ")")]: {
                         marginTop: t.spacing.md
                     }
                 }
             }), ""),
-            Uc = (0, Qe.Z)("div", {
+            Gc = (0, Qe.Z)("div", {
                 target: "e97l2ve2"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     display: "grid",
                     gridTemplateColumns: "1fr 1fr",
                     gridGap: t.spacing.twoXL,
                     ["@media (max-width: ".concat(t.breakpoints.md, ")")]: {
                         gridTemplateColumns: "1fr"
                     }
                 }
             }), ""),
-            Vc = (0, Qe.Z)("div", {
+            $c = (0, Qe.Z)("div", {
                 target: "e97l2ve1"
             })((e => {
                 let {
                     theme: t,
                     extraSpacing: n
                 } = e;
                 return {
@@ -124270,15 +124442,15 @@
                     },
                     "& > img": {
                         position: "absolute",
                         marginTop: t.spacing.sm
                     }
                 }
             }), ""),
-            Hc = (0, Qe.Z)("div", {
+            Kc = (0, Qe.Z)("div", {
                 target: "e97l2ve0"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     display: "flex",
@@ -124287,407 +124459,407 @@
                         marginRight: t.spacing.twoXL
                     },
                     ["@media (max-width: ".concat(t.breakpoints.md, ")")]: {
                         marginTop: t.spacing.xl
                     }
                 }
             }), "");
-        const Xc = __webpack_require__.p + "static/media/checkmark.29851c8e9e6ef0c3d6c1e4efe3c1bb9e.svg";
-        const Gc = function(e) {
+        const Yc = __webpack_require__.p + "static/media/checkmark.29851c8e9e6ef0c3d6c1e4efe3c1bb9e.svg";
+        const Zc = function(e) {
                 const {
                     children: t,
                     extraSpacing: n
                 } = e;
-                return (0, ge.jsxs)(Vc, {
+                return (0, ge.jsxs)($c, {
                     extraSpacing: n,
                     children: [(0, ge.jsx)("img", {
-                        src: Xc,
+                        src: Yc,
                         alt: "Checkmark"
                     }), (0, ge.jsx)("span", {
                         children: t
                     })]
                 })
             },
             {
-                GitStates: $c
+                GitStates: Jc
             } = Be.ef,
-            Kc = e => {
+            Qc = e => {
                 window.open(e, "_blank")
             },
-            Yc = e => {
+            eu = e => {
                 if (e) {
                     const t = new URL("https://share.streamlit.io/deploy");
                     return t.searchParams.set("repository", e.repository || ""), t.searchParams.set("branch", e.branch || ""), t.searchParams.set("mainModule", e.module || ""), t.toString()
                 }
                 return "https://streamlit.io/cloud"
             };
 
-        function Zc(e) {
+        function tu(e) {
             const {
                 gitInfo: n
             } = (0, t.useContext)(je), {
                 onClose: r,
                 metricsMgr: o
             } = e, i = (0, t.useCallback)((() => {
                 const {
                     showDeployError: t,
                     isDeployErrorModalOpen: o,
                     metricsMgr: i
                 } = e;
                 if (i.enqueue("menuClick", {
                         label: "deployButtonInDialog"
                     }), !n) {
-                    const e = Tc();
+                    const e = Nc();
                     return void t(e.title, e.body)
                 }
                 const {
                     repository: a,
                     branch: s,
                     module: l,
                     untrackedFiles: c,
                     state: u
                 } = n;
-                if ((!a || !s || !l) && u === $c.DEFAULT) {
-                    const e = Tc();
+                if ((!a || !s || !l) && u === Jc.DEFAULT) {
+                    const e = Nc();
                     t(e.title, e.body)
-                } else if (u !== $c.HEAD_DETACHED)
+                } else if (u !== Jc.HEAD_DETACHED)
                     if (l && null !== c && void 0 !== c && c.includes(l)) {
-                        const e = Rc(l);
+                        const e = Wc(l);
                         t(e.title, e.body)
-                    } else o && r(), Kc(Yc(n));
+                    } else o && r(), Qc(eu(n));
                 else {
-                    const e = _c();
+                    const e = kc();
                     t(e.title, e.body)
                 }
             }), [e, r, n]);
-            return (0, ge.jsx)(kc, {
+            return (0, ge.jsx)(Lc, {
                 onClose: r,
-                children: (0, ge.jsxs)(Uc, {
-                    children: [(0, ge.jsxs)(jc, {
-                        children: [(0, ge.jsxs)(zc, {
+                children: (0, ge.jsxs)(Gc, {
+                    children: [(0, ge.jsxs)(Hc, {
+                        children: [(0, ge.jsxs)(wc, {
                             children: [(0, ge.jsx)("img", {
-                                src: qc,
+                                src: Rc,
                                 alt: "Streamlit Logo",
                                 "data-testid": "stDeployDialogCommunityCloudIcon"
-                            }), (0, ge.jsx)(Fc, {
+                            }), (0, ge.jsx)(Xc, {
                                 children: "Streamlit Community Cloud"
-                            }), (0, ge.jsx)(Gc, {
+                            }), (0, ge.jsx)(Zc, {
                                 extraSpacing: !0,
                                 children: "For the community"
-                            }), (0, ge.jsx)(Gc, {
+                            }), (0, ge.jsx)(Zc, {
                                 extraSpacing: !0,
                                 children: "Deploy unlimited public apps for free"
-                            }), (0, ge.jsx)(Gc, {
+                            }), (0, ge.jsx)(Zc, {
                                 extraSpacing: !0,
                                 children: "Apps are discoverable through the Streamlit gallery and search engines"
                             })]
-                        }), (0, ge.jsx)(gc, {
-                            children: (0, ge.jsxs)(Hc, {
+                        }), (0, ge.jsx)(vc, {
+                            children: (0, ge.jsxs)(Kc, {
                                 children: [(0, ge.jsx)(an.ZP, {
                                     kind: sn.nW.SECONDARY,
                                     onClick: i,
                                     children: "Deploy now"
                                 }), (0, ge.jsx)(an.ZP, {
                                     onClick: () => {
                                         o.enqueue("menuClick", {
                                             label: "readMoreCommunityCloudInDeployDialog"
-                                        }), Kc(ec)
+                                        }), Qc(oc)
                                     },
                                     kind: sn.nW.MINIMAL,
                                     children: "Read more"
                                 })]
                             })
                         })]
-                    }), (0, ge.jsxs)(jc, {
-                        children: [(0, ge.jsxs)(zc, {
+                    }), (0, ge.jsxs)(Hc, {
+                        children: [(0, ge.jsxs)(wc, {
                             children: [(0, ge.jsx)("img", {
-                                src: Ec,
+                                src: Tc,
                                 alt: "Rocket",
                                 "data-testid": "stDeployDialogCustomDeploymentIcon"
-                            }), (0, ge.jsx)(Fc, {
+                            }), (0, ge.jsx)(Xc, {
                                 children: "Custom deployment"
-                            }), (0, ge.jsx)(Gc, {
+                            }), (0, ge.jsx)(Zc, {
                                 children: "For companies"
-                            }), (0, ge.jsx)(Gc, {
+                            }), (0, ge.jsx)(Zc, {
                                 children: "Deploy on your own hardware or in the cloud, with Docker, Kubernetes, etc"
-                            }), (0, ge.jsx)(Gc, {
+                            }), (0, ge.jsx)(Zc, {
                                 children: "Set up your own authentication"
                             })]
-                        }), (0, ge.jsx)(gc, {
-                            children: (0, ge.jsx)(Hc, {
+                        }), (0, ge.jsx)(vc, {
+                            children: (0, ge.jsx)(Kc, {
                                 children: (0, ge.jsx)(an.ZP, {
                                     onClick: () => {
                                         o.enqueue("menuClick", {
                                             label: "readMoreDeployTutorialInDeployDialog"
-                                        }), Kc(tc)
+                                        }), Qc(ic)
                                     },
                                     kind: sn.nW.MINIMAL,
                                     children: "Read more"
                                 })
                             })
                         })]
                     })]
                 })
             })
         }
-        let Jc;
+        let nu;
 
-        function Qc(e) {
+        function ru(e) {
             switch (e.type) {
-                case Jc.ABOUT:
+                case nu.ABOUT:
                     return function(e) {
                         if (e.aboutSectionMd) {
                             const t = {
                                     overflowY: "auto",
                                     overflowX: "hidden",
                                     maxHeight: "35vh"
                                 },
                                 n = "  \n",
-                                r = ["Made with Streamlit v".concat(e.sessionInfo.current.streamlitVersion), Ql, "Copyright ".concat((new Date).getFullYear(), " Snowflake Inc. All rights reserved.")].join(n),
+                                r = ["Made with Streamlit v".concat(e.sessionInfo.current.streamlitVersion), rc, "Copyright ".concat((new Date).getFullYear(), " Snowflake Inc. All rights reserved.")].join(n),
                                 o = "".concat(e.aboutSectionMd, " ").concat(n, " ").concat(n, " ").concat(r);
-                            return (0, ge.jsxs)(Rl, {
+                            return (0, ge.jsxs)(sr, {
                                 isOpen: !0,
                                 onClose: e.onClose,
-                                children: [(0, ge.jsx)(ql, {
+                                children: [(0, ge.jsx)(rr, {
                                     children: "About"
-                                }), (0, ge.jsx)(El, {
-                                    children: (0, ge.jsx)(Yl, {
+                                }), (0, ge.jsx)(or, {
+                                    children: (0, ge.jsx)(ec, {
                                         children: (0, ge.jsx)(Yt.ZP, {
                                             source: o,
                                             allowHTML: !1,
                                             style: t
                                         })
                                     })
                                 })]
                             })
                         }
-                        return (0, ge.jsxs)(Rl, {
+                        return (0, ge.jsxs)(sr, {
                             isOpen: !0,
                             onClose: e.onClose,
-                            children: [(0, ge.jsx)(ql, {
+                            children: [(0, ge.jsx)(rr, {
                                 children: "Made with"
-                            }), (0, ge.jsx)(El, {
+                            }), (0, ge.jsx)(or, {
                                 children: (0, ge.jsxs)("div", {
                                     children: [e.sessionInfo.isSet && (0, ge.jsxs)(ge.Fragment, {
                                         children: ["Streamlit v", e.sessionInfo.current.streamlitVersion, (0, ge.jsx)("br", {})]
-                                    }), (0, ge.jsx)(Zl, {
-                                        href: Ql,
-                                        children: Ql
+                                    }), (0, ge.jsx)(tc, {
+                                        href: rc,
+                                        children: rc
                                     }), (0, ge.jsx)("br", {}), "Copyright ", (new Date).getFullYear(), " Snowflake Inc. All rights reserved."]
                                 })
                             })]
                         })
                     }(e);
-                case Jc.CLEAR_CACHE:
+                case nu.CLEAR_CACHE:
                     return function(e) {
                         const t = {
                             enter: () => e.defaultAction()
                         };
                         return (0, ge.jsx)(Le.HotKeys, {
                             handlers: t,
                             attach: window,
                             children: (0, ge.jsx)("div", {
                                 "data-testid": "stClearCacheDialog",
-                                children: (0, ge.jsxs)(Rl, {
+                                children: (0, ge.jsxs)(sr, {
                                     isOpen: !0,
                                     onClose: e.onClose,
-                                    children: [(0, ge.jsx)(ql, {
+                                    children: [(0, ge.jsx)(rr, {
                                         children: "Clear caches"
-                                    }), (0, ge.jsxs)(El, {
+                                    }), (0, ge.jsxs)(or, {
                                         children: [(0, ge.jsx)("div", {
                                             children: (0, ge.jsx)("b", {
                                                 children: "Are you sure you want to clear the app's function caches?"
                                             })
                                         }), (0, ge.jsxs)("div", {
                                             children: ["This will remove all cached entries from functions using", " ", (0, ge.jsx)("code", {
                                                 children: "@st.cache"
                                             }), ", ", (0, ge.jsx)("code", {
                                                 children: "@st.cache_data"
                                             }), ", and", " ", (0, ge.jsx)("code", {
                                                 children: "@st.cache_resource"
                                             }), "."]
                                         })]
-                                    }), (0, ge.jsxs)(_l, {
-                                        children: [(0, ge.jsx)(xl, {
+                                    }), (0, ge.jsxs)(ir, {
+                                        children: [(0, ge.jsx)(ar, {
                                             kind: sn.nW.TERTIARY,
                                             onClick: e.onClose,
                                             children: "Cancel"
-                                        }), (0, ge.jsx)(xl, {
+                                        }), (0, ge.jsx)(ar, {
                                             autoFocus: !0,
                                             kind: sn.nW.SECONDARY,
                                             onClick: e.confirmCallback,
                                             children: "Clear caches"
                                         })]
                                     })]
                                 })
                             })
                         })
                     }(e);
-                case Jc.RERUN_SCRIPT:
+                case nu.RERUN_SCRIPT:
                     return function(e) {
                         const t = {
                             enter: () => e.defaultAction()
                         };
                         return (0, ge.jsx)(Le.HotKeys, {
                             handlers: t,
                             attach: window,
-                            children: (0, ge.jsxs)(Rl, {
+                            children: (0, ge.jsxs)(sr, {
                                 isOpen: !0,
                                 onClose: e.onClose,
-                                children: [(0, ge.jsxs)(El, {
-                                    children: [(0, ge.jsx)(Pl, {
+                                children: [(0, ge.jsxs)(or, {
+                                    children: [(0, ge.jsx)(Fl, {
                                         children: "Command line:"
                                     }), (0, ge.jsx)("div", {
-                                        children: (0, ge.jsx)(Dl, {
+                                        children: (0, ge.jsx)(Ul, {
                                             autoFocus: !0,
                                             className: "command-line",
                                             value: e.getCommandLine(),
                                             onChange: t => e.setCommandLine(t.target.value)
                                         })
                                     })]
-                                }), (0, ge.jsxs)(_l, {
-                                    children: [(0, ge.jsx)(xl, {
+                                }), (0, ge.jsxs)(ir, {
+                                    children: [(0, ge.jsx)(ar, {
                                         kind: sn.nW.TERTIARY,
                                         onClick: e.onClose,
                                         children: "Cancel"
-                                    }), (0, ge.jsx)(xl, {
+                                    }), (0, ge.jsx)(ar, {
                                         kind: sn.nW.SECONDARY,
                                         onClick: () => e.rerunCallback(),
                                         children: "Rerun"
                                     })]
                                 })]
                             })
                         })
                     }(e);
-                case Jc.SETTINGS:
-                    return t = e, (0, ge.jsx)(rc, {
+                case nu.SETTINGS:
+                    return t = e, (0, ge.jsx)(sc, {
                         ...t
                     });
-                case Jc.SCRIPT_CHANGED:
-                    return (0, ge.jsx)(Jl, {
+                case nu.SCRIPT_CHANGED:
+                    return (0, ge.jsx)(nc, {
                         ...e
                     });
-                case Jc.SCRIPT_COMPILE_ERROR:
+                case nu.SCRIPT_COMPILE_ERROR:
                     return function(e) {
-                        return (0, ge.jsxs)(Rl, {
+                        return (0, ge.jsxs)(sr, {
                             isOpen: !0,
                             onClose: e.onClose,
                             size: "auto",
                             autoFocus: !1,
-                            children: [(0, ge.jsx)(ql, {
+                            children: [(0, ge.jsx)(rr, {
                                 children: "Script execution error"
-                            }), (0, ge.jsx)(El, {
+                            }), (0, ge.jsx)(or, {
                                 children: (0, ge.jsx)("div", {
                                     children: (0, ge.jsx)("pre", {
                                         children: (0, ge.jsx)("code", {
                                             children: e.exception ? e.exception.message : "No message"
                                         })
                                     })
                                 })
-                            }), (0, ge.jsx)(_l, {
-                                children: (0, ge.jsx)(xl, {
+                            }), (0, ge.jsx)(ir, {
+                                children: (0, ge.jsx)(ar, {
                                     kind: sn.nW.SECONDARY,
                                     onClick: e.onClose,
                                     children: "Close"
                                 })
                             })]
                         })
                     }(e);
-                case Jc.THEME_CREATOR:
-                    return (0, ge.jsx)(fc, {
+                case nu.THEME_CREATOR:
+                    return (0, ge.jsx)(Oc, {
                         ...e
                     });
-                case Jc.WARNING:
+                case nu.WARNING:
                     return function(e) {
-                        return (0, ge.jsxs)(Rl, {
+                        return (0, ge.jsxs)(sr, {
                             isOpen: !0,
                             onClose: e.onClose,
-                            children: [(0, ge.jsx)(ql, {
+                            children: [(0, ge.jsx)(rr, {
                                 children: e.title
-                            }), (0, ge.jsx)(El, {
+                            }), (0, ge.jsx)(or, {
                                 children: e.msg
                             })]
                         })
                     }(e);
-                case Jc.DEPLOY_DIALOG:
-                    return (0, ge.jsx)(Zc, {
+                case nu.DEPLOY_DIALOG:
+                    return (0, ge.jsx)(tu, {
                         ...e
                     });
-                case Jc.DEPLOY_ERROR:
+                case nu.DEPLOY_ERROR:
                     return function(e) {
                         let {
                             title: t,
                             msg: n,
                             onClose: r,
                             onContinue: o,
                             onTryAgain: i
                         } = e;
                         const a = () => {
                             r(), o && o()
                         };
-                        return (0, ge.jsxs)(Rl, {
+                        return (0, ge.jsxs)(sr, {
                             isOpen: !0,
                             onClose: r,
-                            children: [(0, ge.jsx)(ql, {
+                            children: [(0, ge.jsx)(rr, {
                                 children: t
-                            }), (0, ge.jsx)(El, {
-                                children: (0, ge.jsx)(Kl, {
+                            }), (0, ge.jsx)(or, {
+                                children: (0, ge.jsx)(Ql, {
                                     children: n
                                 })
-                            }), (0, ge.jsxs)(_l, {
-                                children: [(0, ge.jsx)(xl, {
+                            }), (0, ge.jsxs)(ir, {
+                                children: [(0, ge.jsx)(ar, {
                                     kind: sn.nW.TERTIARY,
                                     onClick: i,
                                     children: "Try again"
-                                }), (0, ge.jsx)(xl, {
+                                }), (0, ge.jsx)(ar, {
                                     kind: sn.nW.SECONDARY,
                                     onClick: a,
                                     children: o ? "Continue anyway" : "Close"
                                 })]
                             })]
                         })
                     }(e);
                 case void 0:
                     return function(e) {
                         let {
                             onClose: t
                         } = e;
-                        return (0, ge.jsx)(Rl, {
+                        return (0, ge.jsx)(sr, {
                             isOpen: !1,
                             onClose: t
                         })
                     }(e);
                 default:
                     return function(e) {
-                        return (0, ge.jsx)(Rl, {
+                        return (0, ge.jsx)(sr, {
                             isOpen: !0,
                             onClose: e.onClose,
-                            children: (0, ge.jsx)(El, {
+                            children: (0, ge.jsx)(or, {
                                 children: 'Dialog type "'.concat(e.type, '" not recognized.')
                             })
                         })
                     }(e)
             }
             var t
         }! function(e) {
             e.ABOUT = "about", e.CLEAR_CACHE = "clearCache", e.RERUN_SCRIPT = "rerunScript", e.SETTINGS = "settings", e.SCRIPT_CHANGED = "scriptChanged", e.SCRIPT_COMPILE_ERROR = "scriptCompileError", e.THEME_CREATOR = "themeCreator", e.WARNING = "warning", e.DEPLOY_ERROR = "deployError", e.DEPLOY_DIALOG = "deployDialog"
-        }(Jc || (Jc = {}));
-        var eu = __webpack_require__(16840),
-            tu = __webpack_require__.n(eu);
-        const nu = /\/+$/,
-            ru = /^\/+/;
+        }(nu || (nu = {}));
+        var ou = __webpack_require__(16840),
+            iu = __webpack_require__.n(ou);
+        const au = /\/+$/,
+            su = /^\/+/;
 
-        function ou() {
+        function lu() {
             const e = function() {
                     const e = window.location.hostname;
                     let t;
-                    return t = Wa.td ? Wa.Id : window.location.port ? Number(window.location.port) : su() ? 443 : 80, {
+                    return t = vs.td ? vs.Id : window.location.port ? Number(window.location.port) : pu() ? 443 : 80, {
                         host: e,
                         port: t,
-                        basePath: window.location.pathname.replace(nu, "").replace(ru, "")
+                        basePath: window.location.pathname.replace(au, "").replace(su, "")
                     }
                 }(),
                 {
                     basePath: t
                 } = e;
             if (!t) return [e];
             const n = t.split("/"),
@@ -124695,269 +124867,269 @@
             for (; n.length > 0;) r.push({
                 ...e,
                 basePath: n.join("/")
             }), n.pop();
             return r.push({
                 ...e,
                 basePath: ""
-            }), tu()(r, 2)
+            }), iu()(r, 2)
         }
 
-        function iu(e, t) {
+        function cu(e, t) {
             let {
                 host: n,
                 port: r,
                 basePath: o
             } = e;
-            const i = su() ? "https" : "http",
-                a = au(o, t);
+            const i = pu() ? "https" : "http",
+                a = uu(o, t);
             return "".concat(i, "://").concat(n, ":").concat(r, "/").concat(a)
         }
 
-        function au(e, t) {
-            return e = e.replace(nu, "").replace(ru, ""), t = t.replace(nu, "").replace(ru, ""), 0 === e.length ? t : "".concat(e, "/").concat(t)
+        function uu(e, t) {
+            return e = e.replace(au, "").replace(su, ""), t = t.replace(au, "").replace(su, ""), 0 === e.length ? t : "".concat(e, "/").concat(t)
         }
 
-        function su() {
+        function pu() {
             return window.location.href.startsWith("https://")
         }
-        var lu = __webpack_require__(18080);
-        class cu {
+        var du = __webpack_require__(18080);
+        class bu {
             getAge(e) {
                 return e - this.scriptRunCount
             }
             constructor(e, t) {
                 this.encodedMsg = void 0, this.scriptRunCount = 0, this.encodedMsg = e, this.scriptRunCount = t
             }
         }
-        class uu {
+        class fu {
             constructor(e) {
                 this.messages = new Map, this.endpoints = void 0, this.scriptRunCount = 0, this.endpoints = e
             }
             incrementRunCount(e) {
                 this.scriptRunCount += 1, this.messages.forEach(((t, n) => {
-                    t.getAge(this.scriptRunCount) > e && ((0, wo.ji)("Removing expired ForwardMsg [hash=".concat(n, "]")), this.messages.delete(n))
+                    t.getAge(this.scriptRunCount) > e && ((0, bi.ji)("Removing expired ForwardMsg [hash=".concat(n, "]")), this.messages.delete(n))
                 }))
             }
             async processMessagePayload(e, t) {
                 if (this.maybeCacheMessage(e, t), "refHash" !== e.type) return e;
                 let n = this.getCachedMessage(e.refHash, !0);
-                if (null != n)(0, wo.ji)("Cached ForwardMsg HIT [hash=".concat(e.refHash, "]"));
+                if (null != n)(0, bi.ji)("Cached ForwardMsg HIT [hash=".concat(e.refHash, "]"));
                 else {
-                    (0, wo.ji)("Cached ForwardMsg MISS [hash=".concat(e.refHash, "]"));
+                    (0, bi.ji)("Cached ForwardMsg MISS [hash=".concat(e.refHash, "]"));
                     const t = await this.endpoints.fetchCachedForwardMsg(e.refHash);
                     try {
                         n = Be.eI.decode(t)
                     } catch (r) {
                         throw new Error("Failed to decode ForwardMsg (hash=".concat(e.refHash, "): ").concat((0, Ve.b)(r).message))
                     }
                     this.maybeCacheMessage(n, t)
                 }
                 if (!e.metadata) throw new Error("ForwardMsg has no metadata");
                 return n.metadata = Be.eI.decode(t).metadata, n
             }
             maybeCacheMessage(e, t) {
-                "refHash" !== e.type && e.metadata && e.metadata.cacheable && void 0 === this.getCachedMessage(e.hash, !0) && ((0, wo.ji)("Caching ForwardMsg [hash=".concat(e.hash, "]")), this.messages.set(e.hash, new cu(t, this.scriptRunCount)))
+                "refHash" !== e.type && e.metadata && e.metadata.cacheable && void 0 === this.getCachedMessage(e.hash, !0) && ((0, bi.ji)("Caching ForwardMsg [hash=".concat(e.hash, "]")), this.messages.set(e.hash, new bu(t, this.scriptRunCount)))
             }
             getCachedMessage(e, t) {
                 const n = this.messages.get(e);
                 if (null != n) return t && (n.scriptRunCount = this.scriptRunCount), Be.eI.decode(n.encodedMsg)
             }
         }
 
-        function pu(e, t, n) {
+        function hu(e, t, n) {
             for (let r = "number" === typeof t ? t : e.indexOf(t); r < e.length; ++r)
                 if (n(e[r])) return r
         }
 
-        function du(e, t, n) {
+        function mu(e, t, n) {
             for (let r = "number" === typeof t ? t : e.indexOf(t); r >= 0; --r) {
                 if (n(e[r])) return r
             }
         }
 
-        function bu(e) {
+        function Mu(e) {
             return void 0 !== e.messageIndex
         }
 
-        function fu(e, t) {
+        function Ou(e, t) {
             return Math.abs(t.timestamp - e.timestamp)
         }
-        class hu {
+        class gu {
             constructor(e, t) {
                 this.rerunEvents = void 0, this.requestedRerun = void 0, this.getResults = () => {
                     const e = new Set;
                     if (this.rerunEvents.forEach((t => {
-                            bu(t) && e.add(t.messageIndex)
+                            Mu(t) && e.add(t.messageIndex)
                         })), 0 === e.size) return "No rerun messages found!";
-                    const t = Array.from(e).sort(mu),
+                    const t = Array.from(e).sort(zu),
                         n = this.rerunEvents[this.rerunEvents.length - 1],
                         r = this.rerunEvents[0],
                         o = {
                             messages: t.map(this.getMessageAnalysis),
-                            rerunDuration: fu(r, n)
+                            rerunDuration: Ou(r, n)
                         };
-                    return void 0 !== this.requestedRerun && (o.requestedRerun = !0, o.scriptRunStateAtStart = this.requestedRerun.scriptRunState, o.requestToRerunStart = fu(this.requestedRerun, r)), o
+                    return void 0 !== this.requestedRerun && (o.requestedRerun = !0, o.scriptRunStateAtStart = this.requestedRerun.scriptRunState, o.requestToRerunStart = Ou(this.requestedRerun, r)), o
                 }, this.getMessageAnalysis = e => {
                     const t = [];
                     let n = 0;
                     for (; n < this.rerunEvents.length;) {
-                        const r = Mu(this.rerunEvents, n, e);
+                        const r = yu(this.rerunEvents, n, e);
                         if (void 0 === r) break;
                         t.push(this.rerunEvents[r]), n = r + 1
                     }
                     if (0 === t.length) throw new Error("No messages for the given index: ".concat(e));
                     const r = {
                         messageIndex: e,
-                        duration: fu(t[0], t[t.length - 1]),
+                        duration: Ou(t[0], t[t.length - 1]),
                         steps: []
                     };
                     for (let o = 1; o < t.length; ++o) {
                         const e = t[o - 1],
                             n = t[o];
                         "DecodedMessage" === n.name && (r.messageType = n.messageType, r.len = n.len), r.steps.push({
                             name: n.name,
-                            duration: fu(e, n)
+                            duration: Ou(e, n)
                         })
                     }
                     return r
                 };
                 const n = function(e, t) {
-                    const n = du(e, t - 1, (e => "DecodedMessage" === e.name && "newSession" === e.messageType));
+                    const n = mu(e, t - 1, (e => "DecodedMessage" === e.name && "newSession" === e.messageType));
                     if (void 0 === n) return;
                     const {
                         messageIndex: r
                     } = e[n];
-                    return du(e, n, (e => "BeginHandleMessage" === e.name && e.messageIndex === r))
+                    return mu(e, n, (e => "BeginHandleMessage" === e.name && e.messageIndex === r))
                 }(e, t);
                 if (void 0 === n) throw new Error("Unable to find run start!");
                 this.rerunEvents = e.slice(n, t + 1), this.requestedRerun = function(e, t, n) {
-                    const r = du(e, t, n);
+                    const r = mu(e, t, n);
                     return void 0 !== r ? e[r] : void 0
                 }(e, n - 1, (e => "RequestedRerun" === e.name))
             }
         }
 
-        function mu(e, t) {
+        function zu(e, t) {
             return e < t ? -1 : e > t ? 1 : 0
         }
 
-        function Mu(e, t, n) {
-            return pu(e, t, (e => bu(e) && e.messageIndex === n))
+        function yu(e, t, n) {
+            return hu(e, t, (e => Mu(e) && e.messageIndex === n))
         }
-        class Ou {
+        class Au {
             static record(e) {
                 var t, n;
-                this.enabled && (e.timestamp = performance.now(), this.events.push(e), "DispatchedMessage" === e.name && "scriptFinished" === e.messageType && ((0, wo.ji)("Rerun results", (t = this.events, new hu(t, null !== n && void 0 !== n ? n : t.length - 1).getResults())), this.events = []))
+                this.enabled && (e.timestamp = performance.now(), this.events.push(e), "DispatchedMessage" === e.name && "scriptFinished" === e.messageType && ((0, bi.ji)("Rerun results", (t = this.events, new gu(t, null !== n && void 0 !== n ? n : t.length - 1).getResults())), this.events = []))
             }
         }
-        Ou.enabled = !1, Ou.events = [];
-        class gu {
+        Au.enabled = !1, Au.events = [];
+        class vu {
             constructor() {
                 this.resolve = void 0, this.reject = void 0, this.promise = void 0, this.resolve = () => {}, this.reject = () => {}, this.promise = new Promise(((e, t) => {
                     this.resolve = e, this.reject = t
                 }))
             }
         }
-        const zu = "WebsocketConnection",
-            yu = "_stcore/health",
-            Au = "_stcore/host-config",
-            vu = 15e3,
-            wu = "https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS";
-        class Su {
+        const wu = "WebsocketConnection",
+            Su = "_stcore/health",
+            qu = "_stcore/host-config",
+            Eu = 15e3,
+            _u = "https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS";
+        class xu {
             constructor(e) {
-                this.args = void 0, this.cache = void 0, this.uriIndex = 0, this.lastDispatchedMessageIndex = -1, this.nextMessageIndex = 0, this.messageQueue = {}, this.state = Ja.INITIAL, this.websocket = void 0, this.wsConnectionTimeoutId = void 0, this.args = e, this.cache = new uu(e.endpoints), this.stepFsm("INITIALIZED")
+                this.args = void 0, this.cache = void 0, this.uriIndex = 0, this.lastDispatchedMessageIndex = -1, this.nextMessageIndex = 0, this.messageQueue = {}, this.state = js.INITIAL, this.websocket = void 0, this.wsConnectionTimeoutId = void 0, this.args = e, this.cache = new fu(e.endpoints), this.stepFsm("INITIALIZED")
             }
             getBaseUriParts() {
-                if (this.state === Ja.CONNECTED) return this.args.baseUriPartsList[this.uriIndex]
+                if (this.state === js.CONNECTED) return this.args.baseUriPartsList[this.uriIndex]
             }
             disconnect() {
-                this.setFsmState(Ja.DISCONNECTED_FOREVER)
+                this.setFsmState(js.DISCONNECTED_FOREVER)
             }
             setFsmState(e, t) {
-                if ((0, wo.ji)(zu, "New state: ".concat(e)), this.state = e, this.state === Ja.PINGING_SERVER) this.pingServer();
+                if ((0, bi.ji)(wu, "New state: ".concat(e)), this.state = e, this.state === js.PINGING_SERVER) this.pingServer();
                 switch (this.args.onConnectionStateChange(e, t), this.state) {
-                    case Ja.CONNECTING:
+                    case js.CONNECTING:
                         this.connectToWebSocket();
                         break;
-                    case Ja.DISCONNECTED_FOREVER:
+                    case js.DISCONNECTED_FOREVER:
                         this.closeConnection()
                 }
             }
             stepFsm(e, t) {
-                if ((0, wo.ji)(zu, "State: ".concat(this.state, "; Event: ").concat(e)), "FATAL_ERROR" !== e || this.state === Ja.DISCONNECTED_FOREVER) {
+                if ((0, bi.ji)(wu, "State: ".concat(this.state, "; Event: ").concat(e)), "FATAL_ERROR" !== e || this.state === js.DISCONNECTED_FOREVER) {
                     switch (this.state) {
-                        case Ja.INITIAL:
-                            if ("INITIALIZED" === e) return void this.setFsmState(Ja.PINGING_SERVER);
+                        case js.INITIAL:
+                            if ("INITIALIZED" === e) return void this.setFsmState(js.PINGING_SERVER);
                             break;
-                        case Ja.CONNECTING:
-                            if ("CONNECTION_SUCCEEDED" === e) return void this.setFsmState(Ja.CONNECTED);
-                            if ("CONNECTION_TIMED_OUT" === e || "CONNECTION_ERROR" === e || "CONNECTION_CLOSED" === e) return void this.setFsmState(Ja.PINGING_SERVER);
+                        case js.CONNECTING:
+                            if ("CONNECTION_SUCCEEDED" === e) return void this.setFsmState(js.CONNECTED);
+                            if ("CONNECTION_TIMED_OUT" === e || "CONNECTION_ERROR" === e || "CONNECTION_CLOSED" === e) return void this.setFsmState(js.PINGING_SERVER);
                             break;
-                        case Ja.CONNECTED:
-                            if ("CONNECTION_CLOSED" === e || "CONNECTION_ERROR" === e) return void this.setFsmState(Ja.PINGING_SERVER);
+                        case js.CONNECTED:
+                            if ("CONNECTION_CLOSED" === e || "CONNECTION_ERROR" === e) return void this.setFsmState(js.PINGING_SERVER);
                             break;
-                        case Ja.PINGING_SERVER:
-                            if ("SERVER_PING_SUCCEEDED" === e) return void this.setFsmState(Ja.CONNECTING);
+                        case js.PINGING_SERVER:
+                            if ("SERVER_PING_SUCCEEDED" === e) return void this.setFsmState(js.CONNECTING);
                             break;
-                        case Ja.DISCONNECTED_FOREVER:
-                            return void(0, wo.KE)(zu, "Discarding ".concat(e, " while in ").concat(Ja.DISCONNECTED_FOREVER))
+                        case js.DISCONNECTED_FOREVER:
+                            return void(0, bi.KE)(wu, "Discarding ".concat(e, " while in ").concat(js.DISCONNECTED_FOREVER))
                     }
                     throw new Error("Unsupported state transition.\n" + "State: ".concat(this.state, "\n") + "Event: ".concat(e))
                 }
-                this.setFsmState(Ja.DISCONNECTED_FOREVER, t)
+                this.setFsmState(js.DISCONNECTED_FOREVER, t)
             }
             async pingServer() {
                 this.uriIndex = await
                 function(e, n, r, o, i) {
-                    const a = new gu;
+                    const a = new vu;
                     let s = 0,
                         l = 0,
                         c = () => {};
                     const u = () => {
                             l++, l >= e.length && (l = 0), c()
                         },
                         p = e => {
                             const t = .4 * Math.random() - .2,
                                 i = 1 === s ? n : n * 2 ** (s - 1) * (1 + t),
                                 a = Math.min(r, i);
                             o(s, e, a), window.setTimeout(u, a)
                         },
                         d = () => {
                             const n = e[l];
-                            "localhost" === new URL(iu(n, "")).hostname ? p((0, ge.jsxs)(t.Fragment, {
+                            "localhost" === new URL(cu(n, "")).hostname ? p((0, ge.jsxs)(t.Fragment, {
                                 children: [(0, ge.jsx)("p", {
                                     children: "Is Streamlit still running? If you accidentally stopped Streamlit, just restart it in your terminal:"
                                 }), (0, ge.jsx)("pre", {
-                                    children: (0, ge.jsx)(qu, {
+                                    children: (0, ge.jsx)(Ru, {
                                         children: "streamlit run yourscript.py"
                                     })
                                 })]
                             })) : p("Connection failed with status 0.")
                         },
                         b = () => {
                             p((0, ge.jsxs)(t.Fragment, {
                                 children: [(0, ge.jsx)("p", {
                                     children: "Cannot connect to Streamlit (HTTP status: 403)."
                                 }), (0, ge.jsxs)("p", {
                                     children: ["If you are trying to access a Streamlit app running on another server, this could be due to the app's", " ", (0, ge.jsx)("a", {
-                                        href: wu,
+                                        href: _u,
                                         children: "CORS"
                                     }), " settings."]
                                 })]
                             }))
                         };
                     return c = () => {
                         const t = e[l],
-                            n = iu(t, yu),
-                            r = iu(t, Au);
-                        (0, wo.ji)(zu, "Attempting to connect to ".concat(n, ".")), 0 === l && s++, Promise.all([lu.Z.get(n, {
-                            timeout: vu
-                        }), lu.Z.get(r, {
-                            timeout: vu
+                            n = cu(t, Su),
+                            r = cu(t, qu);
+                        (0, bi.ji)(wu, "Attempting to connect to ".concat(n, ".")), 0 === l && s++, Promise.all([du.Z.get(n, {
+                            timeout: Eu
+                        }), du.Z.get(r, {
+                            timeout: Eu
                         })]).then((e => {
                             let [t, n] = e;
                             i(n.data), a.resolve(l)
                         })).catch((e => {
                             if ("ECONNABORTED" === e.code) return p("Connection timed out.");
                             if (e.response) {
                                 const {
@@ -124979,148 +125151,148 @@
             async connectToWebSocket() {
                 const e = function(e, t) {
                     let {
                         host: n,
                         port: r,
                         basePath: o
                     } = e;
-                    const i = su() ? "wss" : "ws",
-                        a = au(o, t);
+                    const i = pu() ? "wss" : "ws",
+                        a = uu(o, t);
                     return "".concat(i, "://").concat(n, ":").concat(r, "/").concat(a)
                 }(this.args.baseUriPartsList[this.uriIndex], "_stcore/stream");
                 if (null != this.websocket) throw new Error("Websocket already exists");
-                (0, wo.ji)(zu, "creating WebSocket");
+                (0, bi.ji)(wu, "creating WebSocket");
                 const t = await this.getSessionTokens();
                 this.websocket = new WebSocket(e, ["streamlit", ...t]), this.websocket.binaryType = "arraybuffer", this.setConnectionTimeout(e);
                 const n = this.websocket,
                     r = () => n === this.websocket;
                 this.websocket.onmessage = e => {
                     r() && this.handleMessage(e.data).catch((e => {
                         const t = "Failed to process a Websocket message (".concat(e, ")");
-                        (0, wo.H)(zu, t), this.stepFsm("FATAL_ERROR", t)
+                        (0, bi.H)(wu, t), this.stepFsm("FATAL_ERROR", t)
                     }))
                 }, this.websocket.onopen = () => {
-                    r() && ((0, wo.ji)(zu, "WebSocket onopen"), this.stepFsm("CONNECTION_SUCCEEDED"))
+                    r() && ((0, bi.ji)(wu, "WebSocket onopen"), this.stepFsm("CONNECTION_SUCCEEDED"))
                 }, this.websocket.onclose = () => {
-                    r() && ((0, wo.KE)(zu, "WebSocket onclose"), this.closeConnection(), this.stepFsm("CONNECTION_CLOSED"))
+                    r() && ((0, bi.KE)(wu, "WebSocket onclose"), this.closeConnection(), this.stepFsm("CONNECTION_CLOSED"))
                 }, this.websocket.onerror = () => {
-                    r() && ((0, wo.H)(zu, "WebSocket onerror"), this.closeConnection(), this.stepFsm("CONNECTION_ERROR"))
+                    r() && ((0, bi.H)(wu, "WebSocket onerror"), this.closeConnection(), this.stepFsm("CONNECTION_ERROR"))
                 }
             }
             setConnectionTimeout(e) {
                 if (null != this.wsConnectionTimeoutId) throw new Error("WS timeout is already set");
                 const t = this.websocket;
                 this.wsConnectionTimeoutId = window.setTimeout((() => {
                     if (t === this.websocket) {
-                        if (null != this.wsConnectionTimeoutId) return null == this.websocket ? (this.closeConnection(), void this.stepFsm("FATAL_ERROR", "Null Websocket in setConnectionTimeout")) : void(0 === this.websocket.readyState && ((0, wo.ji)(zu, "".concat(e, " timed out")), this.closeConnection(), this.stepFsm("CONNECTION_TIMED_OUT")));
-                        (0, wo.KE)(zu, "Timeout fired after cancellation")
+                        if (null != this.wsConnectionTimeoutId) return null == this.websocket ? (this.closeConnection(), void this.stepFsm("FATAL_ERROR", "Null Websocket in setConnectionTimeout")) : void(0 === this.websocket.readyState && ((0, bi.ji)(wu, "".concat(e, " timed out")), this.closeConnection(), this.stepFsm("CONNECTION_TIMED_OUT")));
+                        (0, bi.KE)(wu, "Timeout fired after cancellation")
                     }
-                }), 15e3), (0, wo.ji)(zu, "Set WS timeout ".concat(this.wsConnectionTimeoutId))
+                }), 15e3), (0, bi.ji)(wu, "Set WS timeout ".concat(this.wsConnectionTimeoutId))
             }
             closeConnection() {
-                this.websocket && (this.websocket.close(), this.websocket = void 0), null != this.wsConnectionTimeoutId && ((0, wo.ji)(zu, "Clearing WS timeout ".concat(this.wsConnectionTimeoutId)), window.clearTimeout(this.wsConnectionTimeoutId), this.wsConnectionTimeoutId = void 0)
+                this.websocket && (this.websocket.close(), this.websocket = void 0), null != this.wsConnectionTimeoutId && ((0, bi.ji)(wu, "Clearing WS timeout ".concat(this.wsConnectionTimeoutId)), window.clearTimeout(this.wsConnectionTimeoutId), this.wsConnectionTimeoutId = void 0)
             }
             sendMessage(e) {
                 if (!this.websocket) return;
                 const t = Be._b.create(e),
                     n = Be._b.encode(t).finish();
                 this.websocket.send(n)
             }
             incrementMessageCacheRunCount(e) {
                 this.cache.incrementRunCount(e)
             }
             async handleMessage(e) {
                 const t = this.nextMessageIndex;
-                this.nextMessageIndex += 1, Ou.record({
+                this.nextMessageIndex += 1, Au.record({
                     name: "BeginHandleMessage",
                     messageIndex: t
                 });
                 const n = new Uint8Array(e),
                     r = Be.eI.decode(n);
-                for (Ou.record({
+                for (Au.record({
                         name: "DecodedMessage",
                         messageIndex: t,
                         messageType: r.type,
                         len: e.byteLength
-                    }), this.messageQueue[t] = await this.cache.processMessagePayload(r, n), Ou.record({
+                    }), this.messageQueue[t] = await this.cache.processMessagePayload(r, n), Au.record({
                         name: "GotCachedPayload",
                         messageIndex: t
                     }); this.lastDispatchedMessageIndex + 1 in this.messageQueue;) {
                     const e = this.lastDispatchedMessageIndex + 1;
-                    this.args.onMessage(this.messageQueue[e]), Ou.record({
+                    this.args.onMessage(this.messageQueue[e]), Au.record({
                         name: "DispatchedMessage",
                         messageIndex: e,
                         messageType: this.messageQueue[e].type
                     }), delete this.messageQueue[e], this.lastDispatchedMessageIndex = e
                 }
             }
         }
-        const qu = (0, Qe.Z)("code", {
+        const Ru = (0, Qe.Z)("code", {
             target: "e1xobb530"
         })({
             name: "28m1rt",
             styles: '&::before{content:"$";margin-right:1ex;}'
         });
-        class Eu {
+        class Tu {
             constructor(e) {
-                this.props = void 0, this.connection = void 0, this.connectionState = Ja.INITIAL, this.setConnectionState = (e, t) => {
+                this.props = void 0, this.connection = void 0, this.connectionState = js.INITIAL, this.setConnectionState = (e, t) => {
                     this.connectionState !== e && (this.connectionState = e, this.props.connectionStateChanged(e)), t && this.props.onConnectionError(t)
                 }, this.showRetryError = (e, t, n) => {
                     6 === e && this.props.onConnectionError(t)
                 }, this.props = e, this.connect()
             }
             isConnected() {
-                return this.connectionState === Ja.CONNECTED
+                return this.connectionState === js.CONNECTED
             }
             getBaseUriParts() {
-                if (this.connection instanceof Su) return this.connection.getBaseUriParts()
+                if (this.connection instanceof xu) return this.connection.getBaseUriParts()
             }
             sendMessage(e) {
-                this.connection instanceof Su && this.isConnected() ? this.connection.sendMessage(e) : (0, wo.H)("Cannot send message when server is disconnected: ".concat(e))
+                this.connection instanceof xu && this.isConnected() ? this.connection.sendMessage(e) : (0, bi.H)("Cannot send message when server is disconnected: ".concat(e))
             }
             incrementMessageCacheRunCount(e) {
-                this.connection instanceof Su && this.connection.incrementMessageCacheRunCount(e)
+                this.connection instanceof xu && this.connection.incrementMessageCacheRunCount(e)
             }
             async connect() {
                 try {
                     this.connection = await this.connectToRunningServer()
                 } catch (e) {
                     const t = (0, Ve.b)(e);
-                    (0, wo.H)(t.message), this.setConnectionState(Ja.DISCONNECTED_FOREVER, t.message)
+                    (0, bi.H)(t.message), this.setConnectionState(js.DISCONNECTED_FOREVER, t.message)
                 }
             }
             disconnect() {
                 var e;
                 null === (e = this.connection) || void 0 === e || e.disconnect()
             }
             connectToRunningServer() {
-                const e = ou();
-                return new Su({
+                const e = lu();
+                return new xu({
                     sessionInfo: this.props.sessionInfo,
                     endpoints: this.props.endpoints,
                     baseUriPartsList: e,
                     onMessage: this.props.onMessage,
                     onConnectionStateChange: this.setConnectionState,
                     onRetry: this.showRetryError,
                     claimHostAuthToken: this.props.claimHostAuthToken,
                     resetHostAuthToken: this.props.resetHostAuthToken,
                     onHostConfigResp: this.props.onHostConfigResp
                 })
             }
         }
-        var _u = __webpack_require__(54735);
-        class xu {
+        var ku = __webpack_require__(54735);
+        class Cu {
             constructor() {
-                this.onSessionEvent = new _u.MZ
+                this.onSessionEvent = new ku.MZ
             }
             handleSessionEventMsg(e) {
                 this.onSessionEvent.emit(e)
             }
         }
-        class Ru {
+        class Wu {
             constructor() {
                 this._current = void 0, this._last = void 0
             }
             get current() {
                 if (!this._current) throw new Error("Tried to use SessionInfo before it was initialized");
                 return this._current
             }
@@ -125156,57 +125328,57 @@
                     installationId: r.installationId,
                     installationIdV3: r.installationIdV3,
                     maxCachedMessageAge: n.maxCachedMessageAge,
                     isHello: t.isHello
                 }
             }
         }
-        var Tu = __webpack_require__(76005),
-            ku = __webpack_require__.n(Tu);
-        const Cu = /\uFE0F/g,
-            Wu = String.fromCharCode(8205);
+        var Nu = __webpack_require__(76005),
+            Lu = __webpack_require__.n(Nu);
+        const Iu = /\uFE0F/g,
+            Pu = String.fromCharCode(8205);
 
-        function Nu(e, t, n) {
+        function Du(e, t, n) {
             const r = function(e) {
                 const t = e.replace("-", "_");
-                if (ku().hasEmoji(ku().get(t))) return ku().get(t);
-                if (ku().hasEmoji(e)) return e;
+                if (Lu().hasEmoji(Lu().get(t))) return Lu().get(t);
+                if (Lu().hasEmoji(e)) return e;
                 return ""
             }(e);
             let o;
             if (r) {
                 const e = function(e, t) {
                     const n = [];
                     let r = 0,
                         o = 0,
                         i = 0;
                     for (; i < e.length;) r = e.charCodeAt(i++), o ? (n.push((65536 + (o - 55296 << 10) + (r - 56320)).toString(16)), o = 0) : 55296 <= r && r <= 56319 ? o = r : n.push(r.toString(16));
                     return n.join(t || "-")
-                }((i = r).indexOf(Wu) < 0 ? i.replace(Cu, "") : i);
+                }((i = r).indexOf(Pu) < 0 ? i.replace(Iu, "") : i);
                 o = "https://cdn.jsdelivr.net/gh/twitter/twemoji@14.0.2/assets/72x72/".concat(e, ".png")
             } else o = n.buildMediaURL(e);
             var i;
             ! function(e) {
                 const t = document.querySelector("link[rel='shortcut icon']");
                 t && (t.href = e)
             }(o), t({
                 type: "SET_PAGE_FAVICON",
                 favicon: o
             })
         }
-        var Lu = __webpack_require__(43396);
+        var Bu = __webpack_require__(43396);
 
-        function Iu() {
+        function ju() {
             return {
                 formsWithPendingChanges: new Set,
                 formsWithUploads: new Set,
                 submitButtons: new Map
             }
         }
-        class Pu {
+        class Fu {
             constructor() {
                 this.widgetStates = new Map
             }
             createState(e) {
                 const t = new Be.KR({
                     id: e
                 });
@@ -125238,25 +125410,25 @@
                     this.widgetStates.set(t, e)
                 }))
             }
             forEach(e) {
                 this.widgetStates.forEach(e)
             }
         }
-        class Du {
+        class Uu {
             constructor() {
-                this.widgetStates = new Pu, this.clearOnSubmit = !1, this.formCleared = new _u.MZ
+                this.widgetStates = new Fu, this.clearOnSubmit = !1, this.formCleared = new ku.MZ
             }
             get hasPendingChanges() {
                 return !this.widgetStates.isEmpty
             }
         }
-        class Bu {
+        class Vu {
             constructor(e) {
-                this.props = void 0, this.widgetStates = new Pu, this.forms = new Map, this.formsData = void 0, this.props = e, this.formsData = Iu()
+                this.props = void 0, this.widgetStates = new Fu, this.forms = new Map, this.formsData = void 0, this.props = e, this.formsData = ju()
             }
             addFormClearedListener(e, t) {
                 return this.getOrCreateFormState(e).formCleared.connect(t)
             }
             setFormClearOnSubmit(e, t) {
                 this.getOrCreateFormState(e).clearOnSubmit = t
             }
@@ -125283,15 +125455,15 @@
                 if (null != t && "boolValue" === t.value) return t.boolValue
             }
             setBoolValue(e, t, n, r) {
                 this.createWidgetState(e, n).boolValue = t, this.onWidgetValueChanged(e.formId, n, r)
             }
             getIntValue(e) {
                 const t = this.getWidgetState(e);
-                if (null != t && "intValue" === t.value) return ju(t.intValue)
+                if (null != t && "intValue" === t.value) return Hu(t.intValue)
             }
             setIntValue(e, t, n, r) {
                 this.createWidgetState(e, n).intValue = t, this.onWidgetValueChanged(e.formId, n, r)
             }
             getDoubleValue(e) {
                 const t = this.getWidgetState(e);
                 if (null != t && "doubleValue" === t.value) return t.doubleValue
@@ -125322,15 +125494,15 @@
             setDoubleArrayValue(e, t, n, r) {
                 this.createWidgetState(e, n).doubleArrayValue = new Be.qj({
                     data: t
                 }), this.onWidgetValueChanged(e.formId, n, r)
             }
             getIntArrayValue(e) {
                 const t = this.getWidgetState(e);
-                if (null != t && "intArrayValue" === t.value && null != t.intArrayValue && null != t.intArrayValue.data) return t.intArrayValue.data.map(ju)
+                if (null != t && "intArrayValue" === t.value && null != t.intArrayValue && null != t.intArrayValue.data) return t.intArrayValue.data.map(Hu)
             }
             setIntArrayValue(e, t, n, r) {
                 this.createWidgetState(e, n).intArrayValue = new Be.Zh({
                     data: t
                 }), this.onWidgetValueChanged(e.formId, n, r)
             }
             getJsonValue(e) {
@@ -125390,15 +125562,15 @@
                 return this.widgetStates.getState(e.id)
             }
             deleteWidgetState(e) {
                 this.widgetStates.deleteState(e)
             }
             getOrCreateFormState(e) {
                 let t = this.forms.get(e);
-                return null != t || (t = new Du, this.forms.set(e, t)), t
+                return null != t || (t = new Uu, this.forms.set(e, t)), t
             }
             setFormsWithUploads(e) {
                 this.updateFormsData((t => {
                     t.formsWithUploads = e
                 }))
             }
             addSubmitButton(e, t) {
@@ -125425,30 +125597,30 @@
             }
             updateFormsData(e) {
                 const t = (0, Ie.ZP)(this.formsData, e);
                 this.formsData !== t && (this.formsData = t, this.props.formsDataChanged(this.formsData))
             }
         }
 
-        function ju(e) {
+        function Hu(e) {
             if ("number" === typeof e) return e;
-            const t = Lu.util.LongBits.from(e).toNumber();
+            const t = Bu.util.LongBits.from(e).toNumber();
             if (Number.isSafeInteger(t)) return t;
             throw new Error("value ".concat(e, " cannot be converted to number without a loss of precision!"))
         }
-        class Fu {
+        class Xu {
             constructor(e) {
                 this.props = void 0, this.allowedOrigins = void 0, this.deferredAuthToken = void 0, this.openHostCommunication = () => {
                     window.addEventListener("message", this.receiveHostMessage), this.sendMessageToHost({
                         type: "GUEST_READY"
                     })
                 }, this.closeHostCommunication = () => {
                     window.removeEventListener("message", this.receiveHostMessage)
                 }, this.resetAuthToken = () => {
-                    this.deferredAuthToken = new gu
+                    this.deferredAuthToken = new vu
                 }, this.claimAuthToken = () => this.deferredAuthToken.promise, this.setAllowedOrigins = e => {
                     let {
                         allowedOrigins: t,
                         useExternalAuthToken: n
                     } = e;
                     n || this.deferredAuthToken.resolve(void 0), null !== t && void 0 !== t && t.length && (this.allowedOrigins = t, this.openHostCommunication())
                 }, this.sendMessageToHost = e => {
@@ -125472,118 +125644,118 @@
                             hostname: i
                         } = r;
                         if (o === i) return !0;
                         const a = o.replace(/%2A/g, "*").split("."),
                             s = i.split(".");
                         return a.length === s.length && a.every(((e, t) => "*" === e || e === s[t]))
                     }(t, e.origin))) && ("CLOSE_MODAL" === t.type && this.props.closeModal(), "STOP_SCRIPT" === t.type && this.props.stopScript(), "RERUN_SCRIPT" === t.type && this.props.rerunScript(), "CLEAR_CACHE" === t.type && this.props.clearCache(), "REQUEST_PAGE_CHANGE" === t.type && this.props.pageChanged(t.pageScriptHash), "SEND_APP_HEARTBEAT" === t.type && this.props.sendAppHeartbeat(), "SET_INPUTS_DISABLED" === t.type && this.props.setInputsDisabled(t.disabled), "SET_AUTH_TOKEN" === t.type && (this.deferredAuthToken.resolve(t.authToken), void 0 !== t.jwtHeaderName && this.props.jwtHeaderChanged(t)), "SET_IS_OWNER" === t.type && this.props.isOwnerChanged(t.isOwner), "SET_MENU_ITEMS" === t.type && this.props.hostMenuItemsChanged(t.items), "SET_METADATA" === t.type && this.props.deployedAppMetadataChanged(t.metadata), "SET_PAGE_LINK_BASE_URL" === t.type && this.props.pageLinkBaseUrlChanged(t.pageLinkBaseUrl), "SET_SIDEBAR_CHEVRON_DOWNSHIFT" === t.type && this.props.sidebarChevronDownshiftChanged(t.sidebarChevronDownshift), "SET_SIDEBAR_NAV_VISIBILITY" === t.type && this.props.hostHideSidebarNavChanged(t.hidden), "SET_TOOLBAR_ITEMS" === t.type && this.props.hostToolbarItemsChanged(t.items), "UPDATE_FROM_QUERY_PARAMS" === t.type && (this.props.queryParamsChanged(t.queryParams), this.props.sendRerunBackMsg()), "UPDATE_HASH" === t.type && (window.location.hash = t.hash), "SET_CUSTOM_THEME_CONFIG" === t.type && this.props.themeChanged(t.themeInfo))
-                }, this.props = e, this.allowedOrigins = [], this.deferredAuthToken = new gu
+                }, this.props = e, this.allowedOrigins = [], this.deferredAuthToken = new vu
             }
         }
-        var Uu = __webpack_require__(62813),
-            Vu = __webpack_require__.n(Uu);
-        const Hu = {
+        var Gu = __webpack_require__(62813),
+            $u = __webpack_require__.n(Gu);
+        const Ku = {
             randomUUID: "undefined" !== typeof crypto && crypto.randomUUID && crypto.randomUUID.bind(crypto)
         };
-        let Xu;
-        const Gu = new Uint8Array(16);
+        let Yu;
+        const Zu = new Uint8Array(16);
 
-        function $u() {
-            if (!Xu && (Xu = "undefined" !== typeof crypto && crypto.getRandomValues && crypto.getRandomValues.bind(crypto), !Xu)) throw new Error("crypto.getRandomValues() not supported. See https://github.com/uuidjs/uuid#getrandomvalues-not-supported");
-            return Xu(Gu)
+        function Ju() {
+            if (!Yu && (Yu = "undefined" !== typeof crypto && crypto.getRandomValues && crypto.getRandomValues.bind(crypto), !Yu)) throw new Error("crypto.getRandomValues() not supported. See https://github.com/uuidjs/uuid#getrandomvalues-not-supported");
+            return Yu(Zu)
         }
-        const Ku = [];
-        for (let Ip = 0; Ip < 256; ++Ip) Ku.push((Ip + 256).toString(16).slice(1));
+        const Qu = [];
+        for (let jp = 0; jp < 256; ++jp) Qu.push((jp + 256).toString(16).slice(1));
 
-        function Yu(e) {
+        function ep(e) {
             let t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 0;
-            return (Ku[e[t + 0]] + Ku[e[t + 1]] + Ku[e[t + 2]] + Ku[e[t + 3]] + "-" + Ku[e[t + 4]] + Ku[e[t + 5]] + "-" + Ku[e[t + 6]] + Ku[e[t + 7]] + "-" + Ku[e[t + 8]] + Ku[e[t + 9]] + "-" + Ku[e[t + 10]] + Ku[e[t + 11]] + Ku[e[t + 12]] + Ku[e[t + 13]] + Ku[e[t + 14]] + Ku[e[t + 15]]).toLowerCase()
+            return (Qu[e[t + 0]] + Qu[e[t + 1]] + Qu[e[t + 2]] + Qu[e[t + 3]] + "-" + Qu[e[t + 4]] + Qu[e[t + 5]] + "-" + Qu[e[t + 6]] + Qu[e[t + 7]] + "-" + Qu[e[t + 8]] + Qu[e[t + 9]] + "-" + Qu[e[t + 10]] + Qu[e[t + 11]] + Qu[e[t + 12]] + Qu[e[t + 13]] + Qu[e[t + 14]] + Qu[e[t + 15]]).toLowerCase()
         }
-        const Zu = function(e, t, n) {
-            if (Hu.randomUUID && !t && !e) return Hu.randomUUID();
-            const r = (e = e || {}).random || (e.rng || $u)();
+        const tp = function(e, t, n) {
+            if (Ku.randomUUID && !t && !e) return Ku.randomUUID();
+            const r = (e = e || {}).random || (e.rng || Ju)();
             if (r[6] = 15 & r[6] | 64, r[8] = 63 & r[8] | 128, t) {
                 n = n || 0;
                 for (let e = 0; e < 16; ++e) t[n + e] = r[e];
                 return t
             }
-            return Yu(r)
+            return ep(r)
         };
-        class Ju {
+        class np {
             constructor(e) {
                 this.sessionInfo = void 0, this.endpoints = void 0, this.formsWithPendingRequests = new Map, this.pendingFormUploadsChanged = void 0, this.requestFileURLs = void 0, this.pendingFileURLsRequests = new Map, this.sessionInfo = e.sessionInfo, this.endpoints = e.endpoints, this.pendingFormUploadsChanged = e.formsWithPendingRequestsChanged, this.requestFileURLs = e.requestFileURLs
             }
             async uploadFile(e, t, n, r, o) {
                 return this.offsetPendingRequestCount(e.formId, 1), this.endpoints.uploadFileUploaderFile(t, n, this.sessionInfo.current.sessionId, r, o).finally((() => this.offsetPendingRequestCount(e.formId, -1)))
             }
             deleteFile(e) {
                 return this.endpoints.deleteFileAtURL ? this.endpoints.deleteFileAtURL(e, this.sessionInfo.current.sessionId) : Promise.resolve()
             }
             fetchFileURLs(e) {
                 if (!this.requestFileURLs) return Promise.resolve([]);
-                const t = new gu,
-                    n = Zu();
+                const t = new vu,
+                    n = tp();
                 return this.pendingFileURLsRequests.set(n, t), this.requestFileURLs(n, e), t.promise
             }
             onFileURLsResponse(e) {
                 const t = e.responseId,
                     n = this.pendingFileURLsRequests.get(t);
-                n ? (e.errorMsg ? n.reject(e.errorMsg) : n.resolve(e.fileUrls || []), this.pendingFileURLsRequests.delete(t)) : (0, wo.KE)("fileURLsResponse received for nonexistent request, ignoring.")
+                n ? (e.errorMsg ? n.reject(e.errorMsg) : n.resolve(e.fileUrls || []), this.pendingFileURLsRequests.delete(t)) : (0, bi.KE)("fileURLsResponse received for nonexistent request, ignoring.")
             }
             getFormIdSet() {
                 return new Set(this.formsWithPendingRequests.keys())
             }
             offsetPendingRequestCount(e, t) {
                 var n;
                 if (0 === t) return;
                 if (!(0, He.bM)(e)) return;
                 const r = null !== (n = this.formsWithPendingRequests.get(e)) && void 0 !== n ? n : 0,
                     o = r + t;
                 if (o < 0) throw new Error("Can't offset pendingRequestCount below 0 (formId=".concat(e, ", curCount=").concat(r, ", offset=").concat(t, ")"));
                 const i = this.getFormIdSet();
                 0 === o ? this.formsWithPendingRequests.delete(e) : this.formsWithPendingRequests.set(e, o);
                 const a = this.getFormIdSet();
-                Vu()(a, i) || this.pendingFormUploadsChanged(a)
+                $u()(a, i) || this.pendingFormUploadsChanged(a)
             }
         }
-        class Qu {
+        class rp {
             constructor(e) {
                 this.endpoints = void 0, this.msgListeners = new Map, this.registerListener = (e, t) => {
-                    this.msgListeners.has(e) && (0, wo.KE)("MessageEventSource registered multiple times!", e), this.msgListeners.set(e, t)
+                    this.msgListeners.has(e) && (0, bi.KE)("MessageEventSource registered multiple times!", e), this.msgListeners.set(e, t)
                 }, this.deregisterListener = e => {
-                    this.msgListeners.delete(e) || (0, wo.KE)("Could not deregister unregistered MessageEventSource!")
+                    this.msgListeners.delete(e) || (0, bi.KE)("Could not deregister unregistered MessageEventSource!")
                 }, this.getComponentURL = (e, t) => this.endpoints.buildComponentURL(e, t), this.onMessageEvent = e => {
                     if (null == e.data || !e.data.hasOwnProperty("isStreamlitMessage")) return;
-                    if (null == e.source) return void(0, wo.KE)("Received component message with no eventSource!", e.data);
+                    if (null == e.source) return void(0, bi.KE)("Received component message with no eventSource!", e.data);
                     const t = this.msgListeners.get(e.source);
-                    if (null == t || "function" !== typeof t) return void(0, wo.KE)("Received component message for unregistered ComponentInstance!", e.data);
+                    if (null == t || "function" !== typeof t) return void(0, bi.KE)("Received component message for unregistered ComponentInstance!", e.data);
                     const {
                         type: n
                     } = e.data;
-                    null != n ? t(n, e.data) : (0, wo.KE)("Received Streamlit message with no type!", e.data)
+                    null != n ? t(n, e.data) : (0, bi.KE)("Received Streamlit message with no type!", e.data)
                 }, this.endpoints = e, window.addEventListener("message", this.onMessageEvent)
             }
         }
-        var ep = __webpack_require__(81810),
-            tp = __webpack_require__.n(ep);
-        class np {
+        var op = __webpack_require__(81810),
+            ip = __webpack_require__.n(op);
+        class ap {
             constructor(e) {
                 this.getServerUri = void 0, this.csrfEnabled = void 0, this.cachedServerUri = void 0, this.jwtHeader = void 0, this.getServerUri = e.getServerUri, this.csrfEnabled = e.csrfEnabled
             }
             buildComponentURL(e, t) {
-                return iu(this.requireServerUri(), "".concat("/component", "/").concat(e, "/").concat(t))
+                return cu(this.requireServerUri(), "".concat("/component", "/").concat(e, "/").concat(t))
             }
             setJWTHeader(e) {
                 this.jwtHeader = e
             }
             buildMediaURL(e) {
-                return e.startsWith("/media") ? iu(this.requireServerUri(), e) : e
+                return e.startsWith("/media") ? cu(this.requireServerUri(), e) : e
             }
             buildFileUploadURL(e) {
-                return e.startsWith("/_stcore/upload_file") ? iu(this.requireServerUri(), e) : e
+                return e.startsWith("/_stcore/upload_file") ? cu(this.requireServerUri(), e) : e
             }
             buildAppPageURL(e, t, n) {
                 const r = t.pageName,
                     o = 0 === n ? "" : r;
                 if (null != e && e.length > 0) return "".concat(e, "/").concat(o);
                 const {
                     port: i,
@@ -125613,16 +125785,16 @@
                     data: {
                         sessionId: t
                     }
                 }).then((() => {}))
             }
             async fetchCachedForwardMsg(e) {
                 const t = this.requireServerUri(),
-                    n = await lu.Z.request({
-                        url: iu(t, "".concat("/_stcore/message", "?hash=").concat(e)),
+                    n = await du.Z.request({
+                        url: cu(t, "".concat("/_stcore/message", "?hash=").concat(e)),
                         method: "GET",
                         responseType: "arraybuffer"
                     });
                 return new Uint8Array(n.data)
             }
             requireServerUri() {
                 const e = this.getServerUri();
@@ -125634,20 +125806,20 @@
                 if (t.url = e, this.csrfEnabled) {
                     const e = (0, He.ej)("_streamlit_xsrf");
                     null != e && (t.headers = {
                         "X-Xsrftoken": e,
                         ...t.headers || {}
                     }, t.withCredentials = !0)
                 }
-                return lu.Z.request(t)
+                return du.Z.request(t)
             }
         }
-        var rp = __webpack_require__(1866),
-            op = __webpack_require__.n(rp);
-        class ip {
+        var sp = __webpack_require__(1866),
+            lp = __webpack_require__.n(sp);
+        class cp {
             constructor(e) {
                 this.sessionInfo = void 0, this.initialized = !1, this.actuallySendMetrics = !1, this.pendingEvents = [], this.pendingCustomComponentCounter = {}, this.appHash = "Not initialized", this.metadata = {}, this.setAppHash = e => {
                     this.appHash = e
                 }, this.sessionInfo = e
             }
             initialize(e) {
                 let {
@@ -125672,15 +125844,15 @@
                             e.load = function(t, n) {
                                 const r = document.createElement("script");
                                 r.type = "text/javascript", r.async = !0, r.src = "https://cdn.segment.com/analytics.js/v1/" + t + "/analytics.min.js";
                                 const o = document.getElementsByTagName("script")[0];
                                 o && o.parentNode && o.parentNode.insertBefore(r, o), e._loadOptions = n
                             }, e.SNIPPET_VERSION = "4.1.0", e.load("iCkMy7ymtJ9qYzQRXkQpnAJEq7D4NyMU")
                         }
-                })(), this.sendPendingEvents()), (0, wo.up)("Gather usage stats: ", this.actuallySendMetrics)
+                })(), this.sendPendingEvents()), (0, bi.up)("Gather usage stats: ", this.actuallySendMetrics)
             }
             enqueue(e) {
                 let t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                 this.initialized && this.sessionInfo.isSet ? this.actuallySendMetrics && (this.pendingEvents.length && this.sendPendingEvents(), this.send(e, t)) : this.pendingEvents.push([e, t])
             }
             handleDeltaMessage(e) {
                 if ("newElement" === e.type) {
@@ -125704,20 +125876,20 @@
             }
             send(e) {
                 const t = {
                     ...arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {},
                     ...this.getHostTrackingData(),
                     ...this.getInstallationData(),
                     reportHash: this.appHash,
-                    dev: Wa.td,
+                    dev: vs.td,
                     source: "browser",
                     streamlitVersion: this.sessionInfo.current.streamlitVersion,
                     isHello: this.sessionInfo.isHello
                 };
-                Wa.td ? (0, wo.up)("[Dev mode] Not tracking stat datapoint: ", e, t) : this.track(e, t, {
+                vs.td ? (0, bi.up)("[Dev mode] Not tracking stat datapoint: ", e, t) : this.track(e, t, {
                     context: {
                         ip: "0.0.0.0"
                     }
                 })
             }
             sendPendingEvents() {
                 this.pendingEvents.forEach((e => {
@@ -125733,18 +125905,18 @@
                     machineIdV3: this.sessionInfo.current.installationIdV3
                 }
             }
             setMetadata(e) {
                 this.metadata = e
             }
             getHostTrackingData() {
-                return this.metadata ? op()(this.metadata, ["hostedAt", "owner", "repo", "branch", "mainModule", "creatorId"]) : {}
+                return this.metadata ? lp()(this.metadata, ["hostedAt", "owner", "repo", "branch", "mainModule", "creatorId"]) : {}
             }
         }
-        const ap = (0, Qe.Z)("div", {
+        const up = (0, Qe.Z)("div", {
                 target: "erw9t6i1"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 const n = (0, ye.Iy)(t);
                 return {
@@ -125761,41 +125933,41 @@
                         float: "none",
                         height: t.sizes.full,
                         position: "static",
                         overflow: "visible"
                     }
                 }
             }), ""),
-            sp = (0, Qe.Z)("div", {
+            pp = (0, Qe.Z)("div", {
                 target: "erw9t6i0"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     position: "fixed",
                     top: 0,
                     left: 0,
                     zIndex: t.zIndices.tablePortal,
                     lineHeight: "100%"
                 }
             }), "");
-        const lp = (0, Qe.Z)("label", {
+        const dp = (0, Qe.Z)("label", {
                 target: "emfz9mr1"
             })({
                 name: "ti75j2",
                 styles: "margin:0"
             }),
-            cp = (0, Qe.Z)("p", {
+            bp = (0, Qe.Z)("p", {
                 target: "emfz9mr0"
             })({
                 name: "ti75j2",
                 styles: "margin:0"
             });
-        class up extends t.PureComponent {
+        class fp extends t.PureComponent {
             constructor() {
                 super(...arguments), this.state = {
                     recordAudio: this.props.recordAudio
                 }, this.handleRecordAudioCheckbox = e => {
                     const {
                         checked: t
                     } = e.target, {
@@ -125816,260 +125988,260 @@
             }
             render() {
                 const {
                     recordAudio: e
                 } = this.state, {
                     onClose: t
                 } = this.props;
-                return (0, ge.jsxs)(Rl, {
+                return (0, ge.jsxs)(sr, {
                     isOpen: !0,
                     onClose: t,
-                    children: [(0, ge.jsx)(ql, {
+                    children: [(0, ge.jsx)(rr, {
                         children: "Record a screencast"
-                    }), (0, ge.jsxs)(El, {
+                    }), (0, ge.jsxs)(or, {
                         children: [(0, ge.jsx)("p", {
                             children: "This will record a video with the contents of your screen, so you can easily share what you're seeing with others."
                         }), (0, ge.jsx)("p", {
-                            children: (0, ge.jsxs)(lp, {
+                            children: (0, ge.jsxs)(dp, {
                                 "data-testid": "stScreencastAudioCheckbox",
                                 children: [(0, ge.jsx)("input", {
                                     type: "checkbox",
                                     name: "recordAudio",
                                     checked: e,
                                     onChange: this.handleRecordAudioCheckbox
                                 }), " ", "Also record audio"]
                             })
-                        }), (0, ge.jsxs)(cp, {
+                        }), (0, ge.jsxs)(bp, {
                             "data-testid": "stScreencastInstruction",
                             children: ["Press ", (0, ge.jsx)("kbd", {
                                 children: "Esc"
                             }), " any time to stop recording."]
                         })]
-                    }), (0, ge.jsx)(_l, {
-                        children: (0, ge.jsx)(xl, {
+                    }), (0, ge.jsx)(ir, {
+                        children: (0, ge.jsx)(ar, {
                             kind: sn.nW.SECONDARY,
                             onClick: this.handleStartButton,
                             children: "Start recording!"
                         })
                     })]
                 })
             }
         }
-        const pp = up,
-            dp = (0, Qe.Z)("video", {
+        const hp = fp,
+            mp = (0, Qe.Z)("video", {
                 target: "ecutw1r6"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     width: t.sizes.full,
                     borderRadius: t.radii.md
                 }
             }), ""),
-            bp = (0, Qe.Z)("div", {
+            Mp = (0, Qe.Z)("div", {
                 target: "ecutw1r5"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     display: "flex",
                     flexDirection: "column",
                     width: t.sizes.full
                 }
             }), ""),
-            fp = (0, Qe.Z)("div", {
+            Op = (0, Qe.Z)("div", {
                 target: "ecutw1r4"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     display: "flex",
                     flexDirection: "row",
                     paddingTop: t.spacing.md,
                     paddingBottom: t.spacing.md
                 }
             }), ""),
-            hp = (0, Qe.Z)("div", {
+            gp = (0, Qe.Z)("div", {
                 target: "ecutw1r3"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     paddingRight: t.spacing.lg,
                     textAlign: "right",
                     color: t.colors.gray,
                     fontWeight: t.fontWeights.bold,
                     width: "6em"
                 }
             }), ""),
-            mp = (0, Qe.Z)("div", {
+            zp = (0, Qe.Z)("div", {
                 target: "ecutw1r2"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     flex: 1,
                     paddingRight: t.spacing.lg,
                     marginRight: "6em",
                     ["@media (max-width: ".concat(t.breakpoints.sm, ")")]: {
                         marginRight: t.spacing.none
                     }
                 }
             }), ""),
-            Mp = (0, Qe.Z)("p", {
+            yp = (0, Qe.Z)("p", {
                 target: "ecutw1r1"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     marginTop: t.spacing.sm,
                     marginBottom: t.spacing.none,
                     fontSize: t.fontSizes.sm
                 }
             }), ""),
-            Op = (0, Qe.Z)("div", {
+            Ap = (0, Qe.Z)("div", {
                 target: "ecutw1r0"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     marginTop: t.spacing.twoXS
                 }
             }), ""),
-            gp = e => {
+            vp = e => {
                 let {
                     onClose: t,
                     videoBlob: n,
                     fileName: r
                 } = e;
                 const o = URL.createObjectURL(n);
-                return (0, ge.jsxs)(Rl, {
+                return (0, ge.jsxs)(sr, {
                     isOpen: !0,
                     onClose: t,
                     overrides: {
                         Dialog: {
                             style: {
                                 width: "80vw"
                             }
                         }
                     },
-                    children: [(0, ge.jsx)(ql, {
+                    children: [(0, ge.jsx)(rr, {
                         children: "Next steps"
-                    }), (0, ge.jsx)(El, {
-                        children: (0, ge.jsxs)(bp, {
+                    }), (0, ge.jsx)(or, {
+                        children: (0, ge.jsxs)(Mp, {
                             "data-testid": "stVideoRecordedDialog",
-                            children: [(0, ge.jsxs)(fp, {
-                                children: [(0, ge.jsx)(hp, {
+                            children: [(0, ge.jsxs)(Op, {
+                                children: [(0, ge.jsx)(gp, {
                                     children: "Step 1"
-                                }), (0, ge.jsxs)(mp, {
+                                }), (0, ge.jsxs)(zp, {
                                     children: [(0, ge.jsx)("p", {
                                         children: "Preview your video below:"
-                                    }), (0, ge.jsx)(dp, {
+                                    }), (0, ge.jsx)(mp, {
                                         src: o,
                                         controls: !0
                                     })]
                                 })]
-                            }), (0, ge.jsxs)(fp, {
-                                children: [(0, ge.jsx)(hp, {
+                            }), (0, ge.jsxs)(Op, {
+                                children: [(0, ge.jsx)(gp, {
                                     children: "Step 2"
-                                }), (0, ge.jsxs)(mp, {
-                                    children: [(0, ge.jsx)(Op, {
+                                }), (0, ge.jsxs)(zp, {
+                                    children: [(0, ge.jsx)(Ap, {
                                         children: (0, ge.jsx)(an.ZP, {
                                             kind: sn.nW.SECONDARY,
                                             onClick: () => {
                                                 const e = document.createElement("a");
                                                 e.setAttribute("href", o), e.setAttribute("download", "".concat(r, ".webm")), e.click(), t()
                                             },
                                             children: "Save video to disk"
                                         })
-                                    }), (0, ge.jsxs)(Mp, {
+                                    }), (0, ge.jsxs)(yp, {
                                         children: ["This video is encoded in the", " ", (0, ge.jsx)("a", {
                                             href: "https://www.webmproject.org/",
                                             children: "WebM format"
                                         }), ", which is only supported by newer video players. You can also play it by dragging the file directly into your browser."]
                                     })]
                                 })]
-                            }), (0, ge.jsxs)(fp, {
-                                children: [(0, ge.jsx)(hp, {
+                            }), (0, ge.jsxs)(Op, {
+                                children: [(0, ge.jsx)(gp, {
                                     children: "Step 3"
-                                }), (0, ge.jsxs)(mp, {
+                                }), (0, ge.jsxs)(zp, {
                                     children: ["Share your video with the world on Twitter, LinkedIn, YouTube, or just plain email!", " ", (0, ge.jsx)("span", {
                                         role: "img",
                                         "aria-label": "Happy",
                                         children: "\ud83d\ude00"
                                     })]
                                 })]
                             })]
                         })
                     })]
                 })
             },
-            zp = (0, Qe.Z)("div", {
+            wp = (0, Qe.Z)("div", {
                 target: "e16i1uly2"
             })((() => ({
                 display: "flex"
             })), ""),
-            yp = (0, Qe.Z)("div", {
+            Sp = (0, Qe.Z)("div", {
                 target: "e16i1uly1"
             })((() => ({
                 display: "flex",
                 alignItems: "center",
                 justifyItems: "center",
                 marginRight: "26px",
                 marginLeft: "10px",
                 fontSize: "50px"
             })), ""),
-            Ap = (0, Qe.Z)("p", {
+            qp = (0, Qe.Z)("p", {
                 target: "e16i1uly0"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     margin: t.spacing.none
                 }
             }), "");
-        class vp extends t.PureComponent {
+        class Ep extends t.PureComponent {
             render() {
                 const {
                     onClose: e
                 } = this.props;
-                return (0, ge.jsxs)(Rl, {
+                return (0, ge.jsxs)(sr, {
                     isOpen: !0,
                     onClose: e,
-                    children: [(0, ge.jsx)(ql, {
+                    children: [(0, ge.jsx)(rr, {
                         children: "Record a screencast"
-                    }), (0, ge.jsx)(El, {
-                        children: (0, ge.jsxs)(zp, {
+                    }), (0, ge.jsx)(or, {
+                        children: (0, ge.jsxs)(wp, {
                             "data-testid": "stUnsupportedBrowserDialog",
-                            children: [(0, ge.jsx)(yp, {
+                            children: [(0, ge.jsx)(Sp, {
                                 children: (0, ge.jsx)("span", {
                                     role: "img",
                                     "aria-label": "Alien Monster",
                                     children: "\ud83d\udc7e"
                                 })
-                            }), (0, ge.jsx)(Ap, {
+                            }), (0, ge.jsx)(qp, {
                                 children: "Due to limitations with some browsers, this feature is only supported on recent desktop versions of Chrome, Firefox, and Edge."
                             })]
                         })
                     })]
                 })
             }
         }
-        const wp = vp;
-        var Sp;
-        const qp = (0, Oe.F4)(Sp || (Sp = (0, Ki.Z)(["\n0% {\n  opacity: 0;\n}\n25% {\n  opacity: 1;\n}\n100% {\n  opacity: 0;\n}"]))),
-            Ep = (0, Qe.Z)("div", {
+        const _p = Ep;
+        var xp;
+        const Rp = (0, Oe.F4)(xp || (xp = (0, Pa.Z)(["\n0% {\n  opacity: 0;\n}\n25% {\n  opacity: 1;\n}\n100% {\n  opacity: 0;\n}"]))),
+            Tp = (0, Qe.Z)("div", {
                 target: "e7qru6u0"
             })((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     position: "fixed",
@@ -126083,18 +126255,18 @@
                     fontSize: "40vh",
                     color: t.colors.red,
                     fontWeight: t.fontWeights.bold,
                     opacity: "0.8",
                     textShadow: "1px 1px 10px ".concat(t.colors.darkGray),
                     transition: "opacity 0.3s ease-in-out",
                     fontFamily: 'Helvetica, Calibri, Roboto, "Open Sans", Arial, sans-serif',
-                    animation: "".concat(qp, " 1s")
+                    animation: "".concat(Rp, " 1s")
                 }
             }), "");
-        class _p extends t.PureComponent {
+        class kp extends t.PureComponent {
             constructor() {
                 super(...arguments), this.state = {
                     countdown: this.props.countdown
                 }, this.onAnimationEnd = async () => {
                     const {
                         countdown: e
                     } = this.state, {
@@ -126105,28 +126277,28 @@
                     }), 0 === n && t()
                 }
             }
             render() {
                 const {
                     countdown: e
                 } = this.state;
-                return (0, ge.jsx)(Ep, {
+                return (0, ge.jsx)(Tp, {
                     "data-testid": "stCountdown",
                     onAnimationEnd: this.onAnimationEnd,
                     children: (0, ge.jsx)("span", {
                         children: e
                     })
                 }, "frame".concat(e))
             }
         }
-        _p.defaultProps = {
+        kp.defaultProps = {
             endCallback: () => {}
         };
-        const xp = _p;
-        const Rp = function(e) {
+        const Cp = kp;
+        const Wp = function(e) {
                 class n extends t.PureComponent {
                     constructor() {
                         super(...arguments), this.recorder = void 0, this.state = {
                             fileName: "streamlit-screencast",
                             recordAudio: !1,
                             currentState: this.props.testOverride || "OFF"
                         }, this.toggleRecordAudio = () => {
@@ -126136,32 +126308,32 @@
                             this.setState({
                                 recordAudio: !e
                             })
                         }, this.showDialog = e => {
                             const {
                                 currentState: t
                             } = this.state;
-                            hs.isSupportedBrowser() ? "OFF" === t ? this.setState({
+                            ol.isSupportedBrowser() ? "OFF" === t ? this.setState({
                                 fileName: e,
                                 currentState: "SETUP"
-                            }) : this.stopRecording().catch((e => (0, wo.KE)("withScreencast.stopRecording threw an error: ".concat(e)))) : this.setState({
+                            }) : this.stopRecording().catch((e => (0, bi.KE)("withScreencast.stopRecording threw an error: ".concat(e)))) : this.setState({
                                 currentState: "UNSUPPORTED"
                             })
                         }, this.startRecording = async () => {
                             const {
                                 recordAudio: e
                             } = this.state;
-                            this.recorder = new hs({
+                            this.recorder = new ol({
                                 recordAudio: e,
                                 onErrorOrStop: () => this.stopRecording()
                             });
                             try {
                                 await this.recorder.initialize()
                             } catch (t) {
-                                return (0, wo.KE)("ScreenCastRecorder.initialize error: ".concat(t)), void this.setState({
+                                return (0, bi.KE)("ScreenCastRecorder.initialize error: ".concat(t)), void this.setState({
                                     currentState: "UNSUPPORTED"
                                 })
                             }
                             this.setState({
                                 currentState: "COUNTDOWN"
                             })
                         }, this.stopRecording = async () => {
@@ -126177,15 +126349,15 @@
                                 outputBlob: e,
                                 currentState: "PREVIEW_FILE"
                             }))))
                         }, this.onCountdownEnd = async () => {
                             if (null == this.recorder) throw new Error("Countdown finished but recorder is null");
                             this.recorder.start() ? this.setState({
                                 currentState: "RECORDING"
-                            }) : this.stopRecording().catch((e => (0, wo.KE)("withScreencast.stopRecording threw an error: ".concat(e))))
+                            }) : this.stopRecording().catch((e => (0, bi.KE)("withScreencast.stopRecording threw an error: ".concat(e))))
                         }, this.getScreenCastProps = () => ({
                             currentState: this.state.currentState,
                             toggleRecordAudio: this.toggleRecordAudio,
                             startRecording: this.showDialog,
                             stopRecording: this.stopRecording
                         }), this.closeDialog = () => {
                             this.setState({
@@ -126200,79 +126372,79 @@
                             } = this.state;
                             return (0, ge.jsxs)("div", {
                                 className: "withScreencast",
                                 "data-testid": "stScreencast",
                                 children: [(0, ge.jsx)(e, {
                                     ...this.props,
                                     screenCast: this.getScreenCastProps()
-                                }), "UNSUPPORTED" === o && (0, ge.jsx)(wp, {
+                                }), "UNSUPPORTED" === o && (0, ge.jsx)(_p, {
                                     onClose: this.closeDialog
-                                }), "SETUP" === o && (0, ge.jsx)(pp, {
+                                }), "SETUP" === o && (0, ge.jsx)(hp, {
                                     recordAudio: r,
                                     onClose: this.closeDialog,
                                     startRecording: this.startRecording,
                                     toggleRecordAudio: this.toggleRecordAudio
-                                }), "COUNTDOWN" === o && (0, ge.jsx)(xp, {
+                                }), "COUNTDOWN" === o && (0, ge.jsx)(Cp, {
                                     countdown: 3,
                                     endCallback: this.onCountdownEnd
-                                }), "PREVIEW_FILE" === o && t && (0, ge.jsx)(gp, {
+                                }), "PREVIEW_FILE" === o && t && (0, ge.jsx)(vp, {
                                     onClose: this.closeDialog,
                                     videoBlob: t,
                                     fileName: n
                                 })]
                             })
                         }
                     }
                 }
-                return n.displayName = "withScreencast(".concat(e.displayName || e.name, ")"), Xn()(n, e)
+                return n.displayName = "withScreencast(".concat(e.displayName || e.name, ")"), Nr()(n, e)
             },
-            Tp = "<null>",
-            kp = (e, t) => t == Be.De.ToolbarMode.DEVELOPER || Be.De.ToolbarMode.VIEWER != t && Be.De.ToolbarMode.MINIMAL != t && (e || xs());
-        class Cp extends t.PureComponent {
+            Np = "<null>",
+            Lp = (e, t) => t == Be.De.ToolbarMode.DEVELOPER || Be.De.ToolbarMode.VIEWER != t && Be.De.ToolbarMode.MINIMAL != t && (e || Ol());
+        class Ip extends t.PureComponent {
             constructor(e) {
                 var t;
-                super(e), t = this, this.endpoints = void 0, this.sessionInfo = new Ru, this.metricsMgr = new ip(this.sessionInfo), this.sessionEventDispatcher = new xu, this.connectionManager = void 0, this.widgetMgr = void 0, this.hostCommunicationMgr = void 0, this.uploadClient = void 0, this.pendingElementsBuffer = void 0, this.pendingElementsTimerRunning = void 0, this.componentRegistry = void 0, this.embeddingId = (0, He.D)(), this.keyMap = {
+                super(e), t = this, this.endpoints = void 0, this.sessionInfo = new Wu, this.metricsMgr = new cp(this.sessionInfo), this.sessionEventDispatcher = new Cu, this.connectionManager = void 0, this.widgetMgr = void 0, this.hostCommunicationMgr = void 0, this.uploadClient = void 0, this.pendingElementsBuffer = void 0, this.pendingElementsTimerRunning = void 0, this.componentRegistry = void 0, this.embeddingId = (0, He.D)(), this.keyMap = {
                     RERUN: "r",
                     CLEAR_CACHE: "c",
                     STOP_RECORDING: {
                         sequence: "esc",
                         action: "keyup"
                     }
                 }, this.keyHandlers = {
                     RERUN: () => {
                         this.rerunScript()
                     },
                     CLEAR_CACHE: () => {
-                        kp(this.state.isOwner, this.state.toolbarMode) && this.openClearCacheDialog()
+                        Lp(this.state.isOwner, this.state.toolbarMode) && this.openClearCacheDialog()
                     },
                     STOP_RECORDING: this.props.screenCast.stopRecording
                 }, this.showDeployError = (e, t, n) => {
                     this.openDialog({
-                        type: Jc.DEPLOY_ERROR,
+                        type: nu.DEPLOY_ERROR,
                         title: e,
                         msg: t,
                         onContinue: n,
                         onClose: () => {},
                         onTryAgain: this.sendLoadGitInfoBackMsg
                     })
                 }, this.handleConnectionStateChanged = e => {
-                    (0, wo.ji)("Connection state changed from ".concat(this.state.connectionState, " to ").concat(e)), this.setState({
+                    (0, bi.ji)("Connection state changed from ".concat(this.state.connectionState, " to ").concat(e)), this.setState({
                         connectionState: e
-                    }), e === Ja.CONNECTED ? ((0, wo.ji)("Reconnected to server; requesting a script run"), this.widgetMgr.sendUpdateWidgetsMessage(), this.setState({
+                    }), e === js.CONNECTED ? ((0, bi.ji)("Reconnected to server; requesting a script run"), this.widgetMgr.sendUpdateWidgetsMessage(), this.setState({
                         dialog: null
                     })) : ((0, He.d8)("_streamlit_xsrf", ""), this.sessionInfo.isSet && this.sessionInfo.clearCurrent())
                 }, this.handleGitInfoChanged = e => {
                     this.setState({
                         gitInfo: e
                     })
                 }, this.handleCustomParentMessage = e => {
                     this.state.appConfig.enableCustomParentMessages ? this.hostCommunicationMgr.sendMessageToHost({
                         type: "CUSTOM_PARENT_MESSAGE",
                         message: e.message
-                    }) : (0, wo.H)("Sending messages to the host is disabled in line with the platform policy.")
+                    }) : (0, bi.H)("Sending messages to the host is disabled in line with the platform policy.")
                 }, this.handleMessage = e => {
                     try {
                         ((e, t, n) => {
                             const r = e[t];
                             if (r in n) return n[r](e[r]);
                             throw new Error("Cannot handle ".concat(t, ' "').concat(r, '".'))
                         })(e, "type", {
@@ -126289,28 +126461,28 @@
                             pageProfile: e => this.handlePageProfileMsg(e),
                             autoRerun: e => this.handleAutoRerun(e),
                             fileUrlsResponse: e => this.uploadClient.onFileURLsResponse(e),
                             parentMessage: e => this.handleCustomParentMessage(e)
                         })
                     } catch (t) {
                         const e = (0, Ve.b)(t);
-                        (0, wo.H)(e), this.showError("Bad message format", e.message)
+                        (0, bi.H)(e), this.showError("Bad message format", e.message)
                     }
                 }, this.handlePageConfigChanged = e => {
                     const {
                         title: t,
                         favicon: n,
                         layout: r,
                         initialSidebarState: o,
                         menuItems: i
                     } = e;
                     t && (this.hostCommunicationMgr.sendMessageToHost({
                         type: "SET_PAGE_TITLE",
                         title: t
-                    }), document.title = t), n && Nu(n, this.hostCommunicationMgr.sendMessageToHost, this.endpoints), r !== this.state.layout && this.setState((e => ({
+                    }), document.title = t), n && Du(n, this.hostCommunicationMgr.sendMessageToHost, this.endpoints), r !== this.state.layout && this.setState((e => ({
                         layout: r,
                         userSettings: {
                             ...e.userSettings,
                             wideMode: r === Be.Pz.Layout.WIDE
                         }
                     }))), o !== this.state.initialSidebarState && this.setState((() => ({
                         initialSidebarState: o
@@ -126375,15 +126547,15 @@
                 }, this.handleSessionStatusChanged = e => {
                     this.setState((t => {
                         let {
                             scriptRunState: n
                         } = t, {
                             dialog: r
                         } = t;
-                        if (e.scriptIsRunning && t.scriptRunState !== Je.STOP_REQUESTED) n = Je.RUNNING, null != r && r.type === Jc.SCRIPT_COMPILE_ERROR && (r = void 0);
+                        if (e.scriptIsRunning && t.scriptRunState !== Je.STOP_REQUESTED) n = Je.RUNNING, null != r && r.type === nu.SCRIPT_COMPILE_ERROR && (r = void 0);
                         else if (!e.scriptIsRunning && t.scriptRunState !== Je.RERUN_REQUESTED && t.scriptRunState !== Je.COMPILATION_ERROR) {
                             n = Je.NOT_RUNNING;
                             const e = this.metricsMgr.getAndResetCustomComponentCounter();
                             Object.entries(e).forEach((e => {
                                 let [t, n] = e;
                                 this.metricsMgr.enqueue("customComponentStats", {
                                     name: t,
@@ -126402,22 +126574,22 @@
                     }))
                 }, this.handleSessionEvent = e => {
                     if (this.sessionEventDispatcher.handleSessionEventMsg(e), "scriptCompilationException" === e.type) {
                         this.setState({
                             scriptRunState: Je.COMPILATION_ERROR
                         });
                         const t = {
-                            type: Jc.SCRIPT_COMPILE_ERROR,
+                            type: nu.SCRIPT_COMPILE_ERROR,
                             exception: e.scriptCompilationException,
                             onClose: () => {}
                         };
                         this.openDialog(t)
-                    } else if (Wa.B && "scriptChangedOnDisk" === e.type) {
+                    } else if (vs.B && "scriptChangedOnDisk" === e.type) {
                         const e = {
-                            type: Jc.SCRIPT_CHANGED,
+                            type: nu.SCRIPT_CHANGED,
                             onRerun: this.rerunScript,
                             onClose: () => {},
                             allowRunOnSave: this.state.allowRunOnSave
                         };
                         this.openDialog(e)
                     }
                 }, this.handleNewSession = e => {
@@ -126475,27 +126647,27 @@
                                 type: "SET_APP_PAGES",
                                 appPages: e.appPages
                             }), this.hostCommunicationMgr.sendMessageToHost({
                                 type: "SET_CURRENT_PAGE_NAME",
                                 currentPageName: d ? "" : p,
                                 currentPageScriptHash: c
                             })
-                        })), document.title = "".concat(p, " \xb7 Streamlit"), Nu("".concat(".", "/favicon.png"), this.hostCommunicationMgr.sendMessageToHost, this.endpoints)
+                        })), document.title = "".concat(p, " \xb7 Streamlit"), Du("".concat(".", "/favicon.png"), this.hostCommunicationMgr.sendMessageToHost, this.endpoints)
                     }
                     const b = (0, He.Wu)(this.sessionInfo.current.installationId + s);
                     this.metricsMgr.setMetadata(this.state.deployedAppMetadata), this.metricsMgr.setAppHash(b), this.metricsMgr.enqueue("updateReport", {
                         numPages: e.appPages.length,
                         isMainPage: d
                     }), r === b && o === c ? this.setState({
                         scriptRunId: i
                     }) : this.clearAppState(b, i, a)
                 }, this.handleOneTimeInitialization = e => {
                     const t = e.initialize,
                         n = e.config;
-                    this.sessionInfo.setCurrent(Ru.propsFromNewSessionMessage(e)), this.metricsMgr.initialize({
+                    this.sessionInfo.setCurrent(Wu.propsFromNewSessionMessage(e)), this.metricsMgr.initialize({
                         gatherUsageStats: n.gatherUsageStats
                     }), this.handleSessionStatusChanged(t.sessionStatus)
                 }, this.onHistoryChange = () => {
                     var e;
                     const t = null !== (e = this.state.appPages.find((e => document.location.pathname.endsWith("/" + e.pageName)))) && void 0 !== e ? e : this.state.appPages[0],
                         n = document.location.toString().includes("#"),
                         r = (null === t || void 0 === t ? void 0 : t.pageScriptHash) === this.state.currentPageScriptHash;
@@ -126549,32 +126721,32 @@
                         const e = new Be._b({
                             debugDisconnectWebsocket: !0
                         });
                         e.type = "debugDisconnectWebsocket", this.sendBackMsg(e)
                     }
                 }, this.debugClearForwardMsgCache = () => {
                     var e, t;
-                    xs() && (null === (e = this.connectionManager) || void 0 === e || null === (t = e.connection) || void 0 === t || t.cache.messages.clear())
+                    Ol() && (null === (e = this.connectionManager) || void 0 === e || null === (t = e.connection) || void 0 === t || t.cache.messages.clear())
                 }, this.rerunScript = function() {
                     let e = arguments.length > 0 && void 0 !== arguments[0] && arguments[0];
                     t.closeDialog(), t.isServerConnected() ? t.state.scriptRunState !== Je.RUNNING && t.state.scriptRunState !== Je.RERUN_REQUESTED && (t.metricsMgr.enqueue("rerunScript"), t.setState({
                         scriptRunState: Je.RERUN_REQUESTED
                     }), !0 === e && t.saveSettings({
                         ...t.state.userSettings,
                         runOnSave: !0
-                    }), t.widgetMgr.sendUpdateWidgetsMessage()) : (0, wo.H)("Cannot rerun script when disconnected from server.")
+                    }), t.widgetMgr.sendUpdateWidgetsMessage()) : (0, bi.H)("Cannot rerun script when disconnected from server.")
                 }, this.sendLoadGitInfoBackMsg = () => {
                     this.isServerConnected() ? this.sendBackMsg(new Be._b({
                         loadGitInfo: !0
-                    })) : (0, wo.H)("Cannot load git information when disconnected from server.")
+                    })) : (0, bi.H)("Cannot load git information when disconnected from server.")
                 }, this.onPageChange = e => {
                     this.sendRerunBackMsg(void 0, void 0, e)
-                }, this.isAppInReadyState = e => this.state.connectionState === Ja.CONNECTED && this.state.scriptRunState === Je.NOT_RUNNING && e.scriptRunState === Je.RUNNING && e.connectionState === Ja.CONNECTED, this.sendRerunBackMsg = (e, t, n) => {
+                }, this.isAppInReadyState = e => this.state.connectionState === js.CONNECTED && this.state.scriptRunState === Je.NOT_RUNNING && e.scriptRunState === Je.RUNNING && e.connectionState === js.CONNECTED, this.sendRerunBackMsg = (e, t, n) => {
                     const r = this.getBaseUriParts();
-                    if (!r) return void(0, wo.H)("Cannot send rerun backMessage when disconnected from server.");
+                    if (!r) return void(0, bi.H)("Cannot send rerun backMessage when disconnected from server.");
                     const {
                         currentPageScriptHash: o
                     } = this.state, {
                         basePath: i
                     } = r;
                     let a = this.getQueryString(),
                         s = "";
@@ -126585,93 +126757,93 @@
                         rerunScript: {
                             queryString: a,
                             widgetStates: e,
                             pageScriptHash: n,
                             pageName: s,
                             fragmentId: t
                         }
-                    })), Ou.record({
+                    })), Au.record({
                         name: "RequestedRerun",
                         scriptRunState: this.state.scriptRunState
                     })
                 }, this.stopScript = () => {
-                    if (!this.isServerConnected()) return void(0, wo.H)("Cannot stop app when disconnected from server.");
+                    if (!this.isServerConnected()) return void(0, bi.H)("Cannot stop app when disconnected from server.");
                     if (this.state.scriptRunState === Je.NOT_RUNNING || this.state.scriptRunState === Je.STOP_REQUESTED) return;
                     const e = new Be._b({
                         stopScript: !0
                     });
                     e.type = "stopScript", this.sendBackMsg(e), this.setState({
                         scriptRunState: Je.STOP_REQUESTED
                     })
                 }, this.openClearCacheDialog = () => {
                     if (this.isServerConnected()) {
                         const e = {
-                            type: Jc.CLEAR_CACHE,
+                            type: nu.CLEAR_CACHE,
                             confirmCallback: this.clearCache,
                             defaultAction: this.clearCache,
                             onClose: () => {}
                         };
                         this.openDialog(e)
-                    } else(0, wo.H)("Cannot clear cache: disconnected from server")
+                    } else(0, bi.H)("Cannot clear cache: disconnected from server")
                 }, this.openDeployDialog = () => {
                     var e;
                     const t = {
-                        type: Jc.DEPLOY_DIALOG,
+                        type: nu.DEPLOY_DIALOG,
                         onClose: this.closeDialog,
                         showDeployError: this.showDeployError,
-                        isDeployErrorModalOpen: (null === (e = this.state.dialog) || void 0 === e ? void 0 : e.type) === Jc.DEPLOY_ERROR,
+                        isDeployErrorModalOpen: (null === (e = this.state.dialog) || void 0 === e ? void 0 : e.type) === nu.DEPLOY_ERROR,
                         metricsMgr: this.metricsMgr
                     };
                     this.openDialog(t)
                 }, this.openThemeCreatorDialog = () => {
                     const e = {
-                        type: Jc.THEME_CREATOR,
+                        type: nu.THEME_CREATOR,
                         backToSettings: this.settingsCallback,
                         onClose: this.closeDialog
                     };
                     this.openDialog(e)
                 }, this.clearCache = () => {
                     if (this.closeDialog(), this.isServerConnected()) {
                         this.metricsMgr.enqueue("clearCache");
                         const e = new Be._b({
                             clearCache: !0
                         });
                         e.type = "clearCache", this.sendBackMsg(e)
-                    } else(0, wo.H)("Cannot clear cache: disconnected from server")
+                    } else(0, bi.H)("Cannot clear cache: disconnected from server")
                 }, this.sendAppHeartbeat = () => {
                     if (this.isServerConnected()) {
                         const e = new Be._b({
                             appHeartbeat: !0
                         });
                         e.type = "appHeartbeat", this.sendBackMsg(e)
-                    } else(0, wo.H)("Cannot send app heartbeat: disconnected from server")
+                    } else(0, bi.H)("Cannot send app heartbeat: disconnected from server")
                 }, this.sendBackMsg = e => {
-                    this.connectionManager ? ((0, wo.ji)(e), this.connectionManager.sendMessage(e)) : (0, wo.H)("Not connected. Cannot send back message: ".concat(e))
+                    this.connectionManager ? ((0, bi.ji)(e), this.connectionManager.sendMessage(e)) : (0, bi.H)("Not connected. Cannot send back message: ".concat(e))
                 }, this.handleConnectionError = e => {
                     this.showError("Connection error", e)
                 }, this.isServerConnected = () => !!this.connectionManager && this.connectionManager.isConnected(), this.settingsCallback = function() {
                     let e = !(arguments.length > 0 && void 0 !== arguments[0]) || arguments[0];
                     const n = {
-                        type: Jc.SETTINGS,
+                        type: nu.SETTINGS,
                         isServerConnected: t.isServerConnected(),
                         settings: t.state.userSettings,
                         allowRunOnSave: t.state.allowRunOnSave,
                         onSave: t.saveSettings,
                         onClose: () => {},
-                        developerMode: kp(t.state.isOwner, t.state.toolbarMode),
+                        developerMode: Lp(t.state.isOwner, t.state.toolbarMode),
                         openThemeCreator: t.openThemeCreatorDialog,
                         animateModal: e,
                         metricsMgr: t.metricsMgr
                     };
                     t.openDialog(n)
                 }, this.aboutCallback = () => {
                     const {
                         menuItems: e
                     } = this.state, t = {
-                        type: Jc.ABOUT,
+                        type: nu.ABOUT,
                         sessionInfo: this.sessionInfo,
                         onClose: this.closeDialog,
                         aboutSectionMd: null === e || void 0 === e ? void 0 : e.aboutSectionMd
                     };
                     this.openDialog(t)
                 }, this.printCallback = () => {
                     const {
@@ -126708,27 +126880,27 @@
                     })
                 }, this.addScriptFinishedHandler = e => {
                     this.setState(((t, n) => ({
                         scriptFinishedHandlers: t.scriptFinishedHandlers.concat(e)
                     })))
                 }, this.removeScriptFinishedHandler = e => {
                     this.setState(((t, n) => ({
-                        scriptFinishedHandlers: tp()(t.scriptFinishedHandlers, e)
+                        scriptFinishedHandlers: ip()(t.scriptFinishedHandlers, e)
                     })))
                 }, this.getBaseUriParts = () => this.connectionManager ? this.connectionManager.getBaseUriParts() : void 0, this.getQueryString = () => {
                     const {
                         queryParams: e
                     } = this.state, t = e && e.length > 0 ? e : document.location.search;
                     return t.startsWith("?") ? t.substring(1) : t
                 }, this.isInCloudEnvironment = () => {
                     const {
                         hostMenuItems: e
                     } = this.state;
                     return e && (null === e || void 0 === e ? void 0 : e.length) > 0
-                }, this.showDeployButton = () => kp(this.state.isOwner, this.state.toolbarMode) && !this.isInCloudEnvironment() && this.sessionInfo.isSet && !this.sessionInfo.isHello, this.deployButtonClicked = () => {
+                }, this.showDeployButton = () => Lp(this.state.isOwner, this.state.toolbarMode) && !this.isInCloudEnvironment() && this.sessionInfo.isSet && !this.sessionInfo.isHello, this.deployButtonClicked = () => {
                     this.metricsMgr.enqueue("menuClick", {
                         label: "deployButtonInApp"
                     }), this.sendLoadGitInfoBackMsg(), this.openDeployDialog()
                 }, this.requestFileURLs = (e, t) => {
                     if (this.isServerConnected()) {
                         const n = new Be._b({
                             fileUrlsRequest: {
@@ -126736,33 +126908,33 @@
                                 fileNames: t.map((e => e.name)),
                                 sessionId: this.sessionInfo.current.sessionId
                             }
                         });
                         n.type = "fileUrlsRequest", this.sendBackMsg(n)
                     }
                 }, (0, Ie.GP)(), this.state = {
-                    connectionState: Ja.INITIAL,
+                    connectionState: js.INITIAL,
                     elements: Ke.empty(!0),
                     isFullScreen: !1,
                     scriptName: "",
-                    scriptRunId: Tp,
+                    scriptRunId: Np,
                     appHash: null,
                     scriptRunState: Je.NOT_RUNNING,
                     userSettings: {
                         wideMode: !1,
                         runOnSave: !1
                     },
                     layout: Be.Pz.Layout.CENTERED,
                     initialSidebarState: Be.Pz.SidebarState.AUTO,
                     menuItems: void 0,
                     allowRunOnSave: !0,
                     scriptFinishedHandlers: [],
                     themeHash: this.createThemeHash(),
                     gitInfo: null,
-                    formsData: Iu(),
+                    formsData: ju(),
                     appPages: [],
                     currentPageScriptHash: "",
                     hideTopBar: !0,
                     hideSidebarNav: !0,
                     toolbarMode: Be.De.ToolbarMode.MINIMAL,
                     latestRunTime: performance.now(),
                     fragmentIdsThisRun: [],
@@ -126774,20 +126946,20 @@
                     pageLinkBaseUrl: "",
                     queryParams: "",
                     deployedAppMetadata: {},
                     libConfig: {},
                     appConfig: {},
                     autoReruns: [],
                     inputsDisabled: !1
-                }, this.connectionManager = null, this.widgetMgr = new Bu({
+                }, this.connectionManager = null, this.widgetMgr = new Vu({
                     sendRerunBackMsg: this.sendRerunBackMsg,
                     formsDataChanged: e => this.setState({
                         formsData: e
                     })
-                }), this.hostCommunicationMgr = new Fu({
+                }), this.hostCommunicationMgr = new Xu({
                     sendRerunBackMsg: this.sendRerunBackMsg,
                     closeModal: this.closeDialog,
                     stopScript: this.stopScript,
                     rerunScript: this.rerunScript,
                     clearCache: this.clearCache,
                     sendAppHeartbeat: this.sendAppHeartbeat,
                     setInputsDisabled: e => {
@@ -126841,30 +127013,30 @@
                         })
                     },
                     deployedAppMetadataChanged: e => {
                         this.setState({
                             deployedAppMetadata: e
                         })
                     }
-                }), this.endpoints = new np({
+                }), this.endpoints = new ap({
                     getServerUri: this.getBaseUriParts,
                     csrfEnabled: !0
-                }), this.uploadClient = new Ju({
+                }), this.uploadClient = new np({
                     sessionInfo: this.sessionInfo,
                     endpoints: this.endpoints,
                     formsWithPendingRequestsChanged: e => this.widgetMgr.setFormsWithUploads(e),
                     requestFileURLs: this.requestFileURLs
-                }), this.componentRegistry = new Qu(this.endpoints), this.pendingElementsTimerRunning = !1, this.pendingElementsBuffer = this.state.elements, window.streamlitDebug = {
+                }), this.componentRegistry = new rp(this.endpoints), this.pendingElementsTimerRunning = !1, this.pendingElementsBuffer = this.state.elements, window.streamlitDebug = {
                     clearForwardMsgCache: this.debugClearForwardMsgCache,
                     disconnectWebsocket: this.debugDisconnectWebsocket,
                     shutdownRuntime: this.debugShutdownRuntime
                 }
             }
             componentDidMount() {
-                this.connectionManager = new Eu({
+                this.connectionManager = new Tu({
                     sessionInfo: this.sessionInfo,
                     endpoints: this.endpoints,
                     onMessage: this.handleMessage,
                     onConnectionError: this.handleConnectionError,
                     connectionStateChanged: this.handleConnectionStateChanged,
                     claimHostAuthToken: this.hostCommunicationMgr.claimAuthToken,
                     resetHostAuthToken: this.hostCommunicationMgr.resetAuthToken,
@@ -126906,17 +127078,17 @@
                 })
             }
             componentWillUnmount() {
                 var e;
                 null === (e = this.connectionManager) || void 0 === e || e.disconnect(), this.hostCommunicationMgr.closeHostCommunication(), window.removeEventListener("popstate", this.onHistoryChange, !1)
             }
             showError(e, t) {
-                (0, wo.H)(t);
+                (0, bi.H)(t);
                 const n = {
-                    type: Jc.WARNING,
+                    type: nu.WARNING,
                     title: e,
                     msg: t,
                     onClose: () => {}
                 };
                 this.openDialog(n)
             }
             hasStreamlitVersionChanged(e) {
@@ -127003,33 +127175,32 @@
                     pageLinkBaseUrl: f,
                     sidebarChevronDownshift: h,
                     hostMenuItems: m,
                     hostToolbarItems: M,
                     libConfig: O,
                     appConfig: g,
                     inputsDisabled: z
-                } = this.state, y = kp(this.state.isOwner, this.state.toolbarMode), A = De()("stApp", (0, He.l7)(this.embeddingId), {
+                } = this.state, y = Lp(this.state.isOwner, this.state.toolbarMode), A = De()("stApp", (0, He.l7)(this.embeddingId), {
                     "streamlit-embedded": (0, He.P2)(),
                     "streamlit-wide": c.wideMode
-                }), v = n ? Qc({
+                }), v = n ? ru({
                     ...n,
                     onClose: this.closeDialog
-                }) : null, w = z || t !== Ja.CONNECTED;
+                }) : null, w = z || t !== js.CONNECTED;
                 return (0, ge.jsx)(je.Provider, {
                     value: {
                         initialSidebarState: o,
                         wideMode: c.wideMode,
                         embedded: (0, He.P2)(),
                         showPadding: !(0, He.P2)() || (0, He._A)(),
                         disableScrolling: (0, He.G$)(),
                         showToolbar: !(0, He.P2)() || (0, He.GP)(),
                         showColoredLine: !(0, He.P2)() || (0, He.av)(),
                         pageLinkBaseUrl: f,
                         sidebarChevronDownshift: h,
-                        toastAdjustment: M.length > 0,
                         gitInfo: this.state.gitInfo,
                         appConfig: g
                     },
                     children: (0, ge.jsx)(Fe.E.Provider, {
                         value: {
                             isFullScreen: a,
                             setFullScreen: this.handleFullScreen,
@@ -127045,35 +127216,35 @@
                             fragmentIdsThisRun: this.state.fragmentIdsThisRun
                         },
                         children: (0, ge.jsx)(Le.HotKeys, {
                             keyMap: this.keyMap,
                             handlers: this.keyHandlers,
                             attach: window,
                             focused: !0,
-                            children: (0, ge.jsxs)(ap, {
+                            children: (0, ge.jsxs)(up, {
                                 className: A,
                                 "data-testid": "stApp",
-                                "data-teststate": s == Tp ? "initial" : l,
-                                children: [(0, ge.jsxs)(Hs, {
+                                "data-teststate": s == Np ? "initial" : l,
+                                children: [(0, ge.jsxs)(Wl, {
                                     children: [!u && (0, ge.jsxs)(ge.Fragment, {
-                                        children: [(0, ge.jsx)(us, {
+                                        children: [(0, ge.jsx)(Qs, {
                                             connectionState: t,
                                             sessionEventDispatcher: this.sessionEventDispatcher,
                                             scriptRunState: l,
                                             rerunScript: this.rerunScript,
                                             stopScript: this.stopScript,
                                             allowRunOnSave: e
-                                        }), (0, ge.jsx)(Ps, {
+                                        }), (0, ge.jsx)(El, {
                                             hostToolbarItems: M,
                                             sendMessageToHost: this.hostCommunicationMgr.sendMessageToHost,
                                             metricsMgr: this.metricsMgr
                                         })]
-                                    }), this.showDeployButton() && (0, ge.jsx)(js, {
+                                    }), this.showDeployButton() && (0, ge.jsx)(Rl, {
                                         onClick: this.deployButtonClicked.bind(this)
-                                    }), (0, ge.jsx)(Cs, {
+                                    }), (0, ge.jsx)(Al, {
                                         isServerConnected: this.isServerConnected(),
                                         quickRerunCallback: this.rerunScript,
                                         clearCacheCallback: this.openClearCacheDialog,
                                         settingsCallback: this.settingsCallback,
                                         aboutCallback: this.aboutCallback,
                                         printCallback: this.printCallback,
                                         screencastCallback: this.screencastCallback,
@@ -127081,15 +127252,15 @@
                                         hostMenuItems: m,
                                         developmentMode: y,
                                         sendMessageToHost: this.hostCommunicationMgr.sendMessageToHost,
                                         menuItems: i,
                                         metricsMgr: this.metricsMgr,
                                         toolbarMode: this.state.toolbarMode
                                     })]
-                                }), (0, ge.jsx)(xa, {
+                                }), (0, ge.jsx)(Os, {
                                     endpoints: this.endpoints,
                                     sessionInfo: this.sessionInfo,
                                     sendMessageToHost: this.hostCommunicationMgr.sendMessageToHost,
                                     elements: r,
                                     scriptRunId: s,
                                     scriptRunState: l,
                                     widgetMgr: this.widgetMgr,
@@ -127104,16 +127275,16 @@
                                 }), v]
                             })
                         })
                     })
                 })
             }
         }
-        const Wp = Rp(Cp);
-        const Np = () => {
+        const Pp = Wp(Ip);
+        const Dp = () => {
                 const [e, n] = function() {
                     const e = (0, ye.Vx)(),
                         [n, r] = (0, t.useState)(e),
                         [o, i] = (0, t.useState)([]),
                         [a, s] = (0, t.useState)([...(0, ye.Uy)(), ...(0, ye.MJ)(e) ? [] : [e]]),
                         l = (0, t.useCallback)((e => {
                             e !== n && (r(e), e.name === ye.oo ? (0, ye.rk)() : (0, ye.b3)(e))
@@ -127128,15 +127299,15 @@
                             const t = new Be.MA(e),
                                 n = (0, ye.jG)(ye.UO, t);
                             l(n)
                         }), [i, l]);
                     return (0, t.useEffect)((() => {
                         const e = window.matchMedia("(prefers-color-scheme: dark)");
                         return e.addEventListener("change", c), window.addEventListener("afterprint", c), () => {
-                            e.removeEventListener("change", c), window.removeEventListener("afterprint", c)
+                            window.removeEventListener("afterprint", c), e.removeEventListener("change", c)
                         }
                     }), [n, a, c]), [{
                         setTheme: l,
                         activeTheme: n,
                         addThemes: e => {
                             s([...(0, ye.Uy)(), ...e])
                         },
@@ -127146,24 +127317,24 @@
                 }(), {
                     activeTheme: r
                 } = e, o = r.name === ye.UO && n.length > 0;
                 return (0, ge.jsxs)(Ce, {
                     theme: r,
                     children: [o && (0, ge.jsx)(ze, {
                         fontFaces: n
-                    }), (0, ge.jsx)(Wp, {
+                    }), (0, ge.jsx)(Pp, {
                         theme: e
-                    }), (0, ge.jsx)(sp, {
+                    }), (0, ge.jsx)(pp, {
                         id: "portal",
                         "data-testid": "portal"
                     })]
                 })
             },
-            Lp = new me({
+            Bp = new me({
                 prefix: "st-"
             });
         n.render((0, ge.jsx)(Me.zt, {
-            value: Lp,
-            children: (0, ge.jsx)(Np, {})
+            value: Bp,
+            children: (0, ge.jsx)(Dp, {})
         }), document.getElementById("root"))
     })()
 })();
```

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/js/main.37ad7d13.js.LICENSE.txt` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/js/main.46540eaf.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg` & `streamlit-nightly-1.33.1.dev20240412/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/string_util.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/string_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/temporary_directory.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/temporary_directory.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/testing/__init__.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/testing/v1/__init__.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/testing/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/testing/v1/app_test.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/testing/v1/app_test.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/testing/v1/element_tree.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/testing/v1/element_tree.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/testing/v1/local_script_runner.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/testing/v1/local_script_runner.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/testing/v1/util.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/testing/v1/util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/time_util.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/time_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/type_util.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/type_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/url_util.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/url_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/user_info.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/user_info.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/util.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/vendor/ipython/modified_sys_path.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/vendor/ipython/modified_sys_path.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/vendor/pympler/asizeof.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/vendor/pympler/asizeof.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/version.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/version.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/watcher/__init__.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/watcher/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/watcher/event_based_path_watcher.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/watcher/event_based_path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/watcher/local_sources_watcher.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/watcher/local_sources_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/watcher/path_watcher.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/watcher/path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/watcher/polling_path_watcher.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/watcher/polling_path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/watcher/util.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/watcher/util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/web/__init__.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/web/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/web/bootstrap.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/web/bootstrap.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/web/cache_storage_manager_config.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/web/cache_storage_manager_config.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/web/cli.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/web/cli.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/web/server/__init__.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/web/server/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/web/server/app_static_file_handler.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/web/server/app_static_file_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/web/server/browser_websocket_handler.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/web/server/browser_websocket_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/web/server/component_request_handler.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/web/server/component_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/web/server/media_file_handler.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/web/server/media_file_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/web/server/routes.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/web/server/routes.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/web/server/server.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/web/server/server.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/web/server/server_util.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/web/server/server_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/web/server/stats_request_handler.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/web/server/stats_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/web/server/upload_file_request_handler.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/web/server/upload_file_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit/web/server/websocket_headers.py` & `streamlit-nightly-1.33.1.dev20240412/streamlit/web/server/websocket_headers.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit_nightly.egg-info/PKG-INFO` & `streamlit-nightly-1.33.1.dev20240412/streamlit_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-nightly
-Version: 1.33.1.dev20240409
+Version: 1.33.1.dev20240412
 Summary: A faster way to build and share data apps
 Home-page: https://streamlit.io
 Author: Snowflake Inc
 Author-email: hello@streamlit.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/streamlit/streamlit
 Project-URL: Bug Tracker, https://github.com/streamlit/streamlit/issues
```

### Comparing `streamlit-nightly-1.33.1.dev20240409/streamlit_nightly.egg-info/SOURCES.txt` & `streamlit-nightly-1.33.1.dev20240412/streamlit_nightly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 streamlit/elements/arrow.py
 streamlit/elements/arrow_altair.py
 streamlit/elements/arrow_vega_lite.py
 streamlit/elements/balloons.py
 streamlit/elements/bokeh_chart.py
 streamlit/elements/code.py
 streamlit/elements/deck_gl_json_chart.py
+streamlit/elements/dialog_decorator.py
 streamlit/elements/doc_string.py
 streamlit/elements/empty.py
 streamlit/elements/exception.py
 streamlit/elements/form.py
 streamlit/elements/graphviz_chart.py
 streamlit/elements/heading.py
 streamlit/elements/html.py
@@ -92,14 +93,15 @@
 streamlit/elements/text.py
 streamlit/elements/toast.py
 streamlit/elements/utils.py
 streamlit/elements/write.py
 streamlit/elements/lib/__init__.py
 streamlit/elements/lib/column_config_utils.py
 streamlit/elements/lib/column_types.py
+streamlit/elements/lib/dialog.py
 streamlit/elements/lib/dicttools.py
 streamlit/elements/lib/mutable_status_container.py
 streamlit/elements/lib/pandas_styler_utils.py
 streamlit/elements/lib/streamlit_plotly_theme.py
 streamlit/elements/lib/subtitle_utils.py
 streamlit/elements/widgets/__init__.py
 streamlit/elements/widgets/button.py
@@ -332,15 +334,15 @@
 streamlit/static/favicon.png
 streamlit/static/index.html
 streamlit/static/static/css/2411.8b8f33d6.chunk.css
 streamlit/static/static/css/3092.95a45cfe.chunk.css
 streamlit/static/static/css/43.e3b876c5.chunk.css
 streamlit/static/static/css/main.bf304093.css
 streamlit/static/static/js/1074.73973756.chunk.js
-streamlit/static/static/js/1168.3029456a.chunk.js
+streamlit/static/static/js/1168.1d6408e6.chunk.js
 streamlit/static/static/js/1307.8ea033f1.chunk.js
 streamlit/static/static/js/1451.3b0a3e31.chunk.js
 streamlit/static/static/js/1479.6709db03.chunk.js
 streamlit/static/static/js/178.b5384fd0.chunk.js
 streamlit/static/static/js/1792.b8efa879.chunk.js
 streamlit/static/static/js/2187.9469f035.chunk.js
 streamlit/static/static/js/2411.a8823789.chunk.js
@@ -384,28 +386,28 @@
 streamlit/static/static/js/7175.be4076bc.chunk.js
 streamlit/static/static/js/7217.d970c074.chunk.js
 streamlit/static/static/js/7323.2808d029.chunk.js
 streamlit/static/static/js/7323.2808d029.chunk.js.LICENSE.txt
 streamlit/static/static/js/7602.6175e969.chunk.js
 streamlit/static/static/js/7805.51638fbc.chunk.js
 streamlit/static/static/js/8005.43974a35.chunk.js
-streamlit/static/static/js/8427.b0ed496b.chunk.js
+streamlit/static/static/js/8427.d30dffe1.chunk.js
 streamlit/static/static/js/8477.e948c092.chunk.js
 streamlit/static/static/js/8492.f56c9d4c.chunk.js
 streamlit/static/static/js/8570.6de19120.chunk.js
 streamlit/static/static/js/8691.9ccf7f89.chunk.js
 streamlit/static/static/js/9330.d29313d4.chunk.js
 streamlit/static/static/js/9336.2d95d840.chunk.js
 streamlit/static/static/js/937.a1248039.chunk.js
 streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
 streamlit/static/static/js/9656.8c935274.chunk.js
 streamlit/static/static/js/9758.6e6d8662.chunk.js
 streamlit/static/static/js/9865.fd93213d.chunk.js
-streamlit/static/static/js/main.37ad7d13.js
-streamlit/static/static/js/main.37ad7d13.js.LICENSE.txt
+streamlit/static/static/js/main.46540eaf.js
+streamlit/static/static/js/main.46540eaf.js.LICENSE.txt
 streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
 streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
 streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
 streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
```

### Comparing `streamlit-nightly-1.33.1.dev20240409/tests/testutil.py` & `streamlit-nightly-1.33.1.dev20240412/tests/testutil.py`

 * *Files identical despite different names*

