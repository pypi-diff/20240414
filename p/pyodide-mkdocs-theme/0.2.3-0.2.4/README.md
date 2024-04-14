# Comparing `tmp/pyodide_mkdocs_theme-0.2.3.tar.gz` & `tmp/pyodide_mkdocs_theme-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodide_mkdocs_theme-0.2.3.tar", max compression
+gzip compressed data, was "pyodide_mkdocs_theme-0.2.4.tar", max compression
```

## Comparing `pyodide_mkdocs_theme-0.2.3.tar` & `pyodide_mkdocs_theme-0.2.4.tar`

### file list

```diff
@@ -1,75 +1,74 @@
--rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-0.2.3/LICENSE
--rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-0.2.3/README.md
--rw-r--r--   0        0        0     1347 2024-04-12 21:47:48.830344 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/__init__.py
--rw-r--r--   0        0        0     2160 2024-04-12 21:47:09.917172 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/__main__.py
--rw-r--r--   0        0        0       22 2024-04-12 21:47:48.866345 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/__version__.py
--rw-r--r--   0        0        0      807 2024-04-12 21:47:09.925172 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/__init__.py
--rw-r--r--   0        0        0      856 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
--rw-r--r--   0        0        0     1190 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
--rw-r--r--   0        0        0     4974 2024-04-11 09:41:00.019938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
--rw-r--r--   0        0        0     4969 2024-04-09 19:35:36.226493 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py
--rw-r--r--   0        0        0    21303 2024-04-12 21:47:09.925172 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py
--rw-r--r--   0        0        0    14750 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
--rw-r--r--   0        0        0     6073 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
--rw-r--r--   0        0        0     4075 2024-04-12 21:47:09.925172 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
--rw-r--r--   0        0        0    11199 2024-04-11 09:41:00.019938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
--rw-r--r--   0        0        0    12363 2024-04-12 21:47:09.925172 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/messages.py
--rw-r--r--   0        0        0     6945 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
--rw-r--r--   0        0        0     4237 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/parsing.py
--rw-r--r--   0        0        0     4462 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
--rw-r--r--   0        0        0     9077 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
--rw-r--r--   0        0        0    11690 2024-04-12 21:47:09.933172 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
--rw-r--r--   0        0        0    12697 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py
--rw-r--r--   0        0        0     1711 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
--rw-r--r--   0        0        0     3236 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
--rw-r--r--   0        0        0     9993 2024-04-12 21:47:09.941172 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
--rw-r--r--   0        0        0     2658 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
--rw-r--r--   0        0        0     1064 2024-04-12 21:47:48.822343 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
--rw-r--r--   0        0        0     6881 2024-04-12 21:47:09.957173 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
--rw-r--r--   0        0        0      690 2024-04-12 21:47:48.826344 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/scripts/__init__.py
--rw-r--r--   0        0        0     1001 2024-04-12 21:47:09.961173 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/scripts/custom_lang.py
--rw-r--r--   0        0        0     3974 2024-04-12 21:47:48.830344 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/scripts/custom_lang_src.py
--rw-r--r--   0        0        0     5490 2024-04-12 21:47:09.973173 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/__init__.py
--rw-r--r--   0        0        0     4510 2024-04-12 21:47:09.973173 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
--rw-r--r--   0        0        0     7349 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
--rw-r--r--   0        0        0     1675 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
--rw-r--r--   0        0        0     1490 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
--rw-r--r--   0        0        0     4320 2024-04-12 21:47:09.981174 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js
--rw-r--r--   0        0        0     3629 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
--rw-r--r--   0        0        0     1078 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css
--rw-r--r--   0        0        0     6467 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/main.html
--rw-r--r--   0        0        0     1214 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
--rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/partials/copyright.html
--rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/partials/footer.html
--rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/partials/social.html
--rw-r--r--   0        0        0     9780 2024-04-12 21:47:09.981174 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js
--rw-r--r--   0        0        0     5935 2024-04-04 09:56:58.174965 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js
--rw-r--r--   0        0        0     3459 2024-04-12 21:47:09.981174 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css
--rw-r--r--   0        0        0     1645 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png
--rw-r--r--   0        0        0     1328 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png
--rw-r--r--   0        0        0     1761 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png
--rw-r--r--   0        0        0     1283 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png
--rw-r--r--   0        0        0      952 2024-03-05 12:41:09.857670 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png
--rw-r--r--   0        0        0     1296 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png
--rw-r--r--   0        0        0     1702 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js
--rw-r--r--   0        0        0      823 2024-03-04 14:13:04.212401 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md
--rw-r--r--   0        0        0     6600 2024-04-12 21:47:09.985174 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js
--rw-r--r--   0        0        0    16559 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js
--rw-r--r--   0        0        0     9657 2024-04-04 09:56:58.138964 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js
--rw-r--r--   0        0        0      252 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/README.md
--rw-r--r--   0        0        0     1947 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css
--rw-r--r--   0        0        0     9150 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js
--rw-r--r--   0        0        0     3629 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css
--rw-r--r--   0        0        0    31978 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/0_cdn-terminal-replacement-libs.css
--rw-r--r--   0        0        0     1527 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css
--rw-r--r--   0        0        0     5373 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js
--rw-r--r--   0        0        0     4218 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js
--rw-r--r--   0        0        0     1478 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js
--rw-r--r--   0        0        0     2857 2024-03-25 22:17:16.937424 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg
--rw-r--r--   0        0        0     3774 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css
--rw-r--r--   0        0        0    12675 2024-04-12 21:47:09.985174 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js
--rw-r--r--   0        0        0     1775 2024-04-12 21:47:46.082261 pyodide_mkdocs_theme-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2829 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-0.2.4/LICENSE
+-rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-0.2.4/README.md
+-rw-r--r--   0        0        0     1347 2024-04-14 07:05:50.948264 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/__init__.py
+-rw-r--r--   0        0        0     2160 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/__main__.py
+-rw-r--r--   0        0        0       22 2024-04-14 07:05:50.984265 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/__version__.py
+-rw-r--r--   0        0        0      807 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/__init__.py
+-rw-r--r--   0        0        0      856 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
+-rw-r--r--   0        0        0     1190 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
+-rw-r--r--   0        0        0     4974 2024-04-11 09:41:00.019938 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
+-rw-r--r--   0        0        0     4969 2024-04-09 19:35:36.226493 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py
+-rw-r--r--   0        0        0    21303 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py
+-rw-r--r--   0        0        0    14750 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py
+-rw-r--r--   0        0        0      689 2024-04-14 07:02:56.164794 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
+-rw-r--r--   0        0        0     6073 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
+-rw-r--r--   0        0        0     4093 2024-04-14 07:02:56.164794 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
+-rw-r--r--   0        0        0    11511 2024-04-14 07:03:36.550530 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
+-rw-r--r--   0        0        0    12363 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/messages.py
+-rw-r--r--   0        0        0     6945 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
+-rw-r--r--   0        0        0     4237 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/parsing.py
+-rw-r--r--   0        0        0     4462 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
+-rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
+-rw-r--r--   0        0        0     9077 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
+-rw-r--r--   0        0        0    11690 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
+-rw-r--r--   0        0        0    12697 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py
+-rw-r--r--   0        0        0     1711 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
+-rw-r--r--   0        0        0     3236 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
+-rw-r--r--   0        0        0    10035 2024-04-14 07:02:56.164794 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
+-rw-r--r--   0        0        0     2658 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
+-rw-r--r--   0        0        0     1064 2024-04-14 07:05:50.940264 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
+-rw-r--r--   0        0        0     6881 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
+-rw-r--r--   0        0        0      690 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/scripts/__init__.py
+-rw-r--r--   0        0        0     1001 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/scripts/custom_lang.py
+-rw-r--r--   0        0        0     3974 2024-04-14 07:05:50.948264 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/scripts/custom_lang_src.py
+-rw-r--r--   0        0        0     5490 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py
+-rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/__init__.py
+-rw-r--r--   0        0        0     4510 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
+-rw-r--r--   0        0        0     7349 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
+-rw-r--r--   0        0        0     1675 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
+-rw-r--r--   0        0        0     1490 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
+-rw-r--r--   0        0        0     4320 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js
+-rw-r--r--   0        0        0     3629 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
+-rw-r--r--   0        0        0     1078 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css
+-rw-r--r--   0        0        0     6426 2024-04-14 07:03:36.550530 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/main.html
+-rw-r--r--   0        0        0     1924 2024-04-14 07:05:50.944264 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
+-rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/partials/copyright.html
+-rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/partials/footer.html
+-rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/partials/social.html
+-rw-r--r--   0        0        0     9780 2024-04-12 21:48:00.502695 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js
+-rw-r--r--   0        0        0     5935 2024-04-04 09:56:58.174965 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js
+-rw-r--r--   0        0        0     3459 2024-04-12 21:48:00.502695 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css
+-rw-r--r--   0        0        0     1645 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png
+-rw-r--r--   0        0        0     1328 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png
+-rw-r--r--   0        0        0     1761 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png
+-rw-r--r--   0        0        0     1283 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png
+-rw-r--r--   0        0        0      952 2024-03-05 12:41:09.857670 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png
+-rw-r--r--   0        0        0     1296 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png
+-rw-r--r--   0        0        0     1702 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js
+-rw-r--r--   0        0        0      823 2024-03-04 14:13:04.212401 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md
+-rw-r--r--   0        0        0     6600 2024-04-12 21:48:00.502695 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js
+-rw-r--r--   0        0        0    16559 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js
+-rw-r--r--   0        0        0     9657 2024-04-04 09:56:58.138964 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js
+-rw-r--r--   0        0        0      252 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/README.md
+-rw-r--r--   0        0        0     1947 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css
+-rw-r--r--   0        0        0     9150 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js
+-rw-r--r--   0        0        0     3629 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css
+-rw-r--r--   0        0        0     1651 2024-04-14 07:03:36.550530 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css
+-rw-r--r--   0        0        0     5373 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js
+-rw-r--r--   0        0        0     4218 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js
+-rw-r--r--   0        0        0     1478 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js
+-rw-r--r--   0        0        0     2857 2024-03-25 22:17:16.937424 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg
+-rw-r--r--   0        0        0     3774 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css
+-rw-r--r--   0        0        0    12675 2024-04-12 21:48:00.502695 pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js
+-rw-r--r--   0        0        0     1775 2024-04-14 07:05:47.352111 pyodide_mkdocs_theme-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2829 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-0.2.4/PKG-INFO
```

### Comparing `pyodide_mkdocs_theme-0.2.3/LICENSE` & `pyodide_mkdocs_theme-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/README.md` & `pyodide_mkdocs_theme-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/__init__.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/__main__.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/__main__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/__init__.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/exceptions.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,24 +87,24 @@
     """
     @wraps(py)
     def wrapped(nom: str, stop=None, ID:int=None) -> str:
         return script(env, 'py', env.docs_dir_path, nom, stop=stop, ID=ID)
     return wrapped
 
 
-def py_sujet(env:MaestroIDE):
-    """
-    Macro python rapide, pour un sujet sans les tests => code formaté seulement, non modifiable.
-
-    ATTENTION: Ne marche pas sur les exercices avec tous les codes python dans le même fichier.
-    """
-    @wraps(py_sujet)
-    def wrapped(nom: str, stop=None, ID:int=None) -> str:
-        return script(env, 'py_sujet', env.docs_dir_path, nom, stop=stop, ID=ID)
-    return wrapped
+# def py_sujet(env:MaestroIDE):
+#     """
+#     Macro python rapide, pour un sujet sans les tests => code formaté seulement, non modifiable.
+
+#     ATTENTION: Ne marche pas sur les exercices avec tous les codes python dans le même fichier.
+#     """
+#     @wraps(py_sujet)
+#     def wrapped(nom: str, stop=None, ID:int=None) -> str:
+#         return script(env, 'py_sujet', env.docs_dir_path, nom, stop=stop, ID=ID)
+#     return wrapped
 
 
 
 
 
 
 def terminal(env:MaestroIDE):
```

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 
 
 
 
 
 
-
+CORRECT_CLOSE_P = '</p KEEP>'
 
 
 
 def multi_qcm(env:MaestroExtras):
     """
     @inputs:          lists of data for one question, aka:
                         - question title
@@ -113,45 +113,47 @@
 
             title = env.lang.qcm_title.one_or_many( len(questions_data) > 1 )
             admo_title = title if qcm_title is None else qcm_title
             opening = f'{ indent }{ admo_kind } { admo_class } { admo_classes } "{ admo_title }"'
             return [
                 opening,
                 '',         # KEEP!
-                auto_indent('\n</p KEEP><ol>\n'),
+                auto_indent(f'\n{ CORRECT_CLOSE_P }<ol>\n'),
             ]
 
         def qcm_close():
-            admonition_lst.append(auto_indent("</p KEEP></ol>"))
+            admonition_lst.append(auto_indent(f"{ CORRECT_CLOSE_P }</ol>"))
 
 
         def question_open(
             admonition_lst:list, question:str, n:int, lst_answers:List[int], default_multi
         ):
             is_multi = len(lst_answers) > 1
             multi_kls = true_false_none_for(
                 is_multi or default_multi,
                 HtmlClass.qcm_multi,
                 HtmlClass.qcm_single,
             )
             answers = ','.join(map(str,lst_answers))
-            tag_open = f'</p KEEP><li class="{ multi_kls }" correct="{ answers }" markdown>\n{ question }'
+            tag_open = (
+                f'{ CORRECT_CLOSE_P }<li class="{ multi_kls }" correct="{ answers }" markdown>\n{ question }'
+            )
             admonition_lst.append(auto_indent(tag_open))
 
         def question_close():
             admonition_lst.append(auto_indent("</li>\n"))
             # Extra linefeed for presentational purpose only (DEBUG=True): it doesn't have any
             # impact anymore, since everything inside a qcm is inserted through "<tag markdown>".
 
 
         def question_options(admonition_lst:list, items):
             """ Always use "md_in_html" approach, to simplify the construction. It is required
                 anyway when the first item starts with a code block...
             """
-            admonition_lst.append(auto_indent('</p KEEP><ul>'))
+            admonition_lst.append(auto_indent(f'{ CORRECT_CLOSE_P }<ul>'))
             admonition_lst.extend(
                 auto_indent(item, wrap_li=True) for item in items
             )
             admonition_lst.append(auto_indent("</ul>"))
 
 
         def validate_question_config(question, items, lst_correct, multi):
@@ -210,15 +212,16 @@
         qcm_close()
 
 
         output = '\n'.join(admonition_lst)
         output = f'\n\n{ output }\n\n'    # Enforce empty spaces around in the markdown admonition
 
         if DEBUG:
-            print(output)
+            # The user doesn't need to know about the CORRECT_CLOSE_P thing, so remove them first:
+            print(output.replace(CORRECT_CLOSE_P, ''))
         return output
 
     return wrapped
 
 
 
 
@@ -263,14 +266,16 @@
 
 QUOTES = "'‘“\""
 
 
 def extract_csv_file(env:MaestroExtras, input_file, sep=";") -> List[str] :
     """ Extract info from external file, to build a multi qcm """
 
+    env.warn_unmaintained('The macro multi_qcm using the csv data extraction')
+
     def csv_entry_to_qcm_input(entry:dict):
         question = entry["Question"]
         list_answers = [entry[key] for key in entry if "Answer" in key and entry[key] is not None]
         list_correct = list(map(int, entry["Valid"].split(",")))
         dictionnaire_var = to_dict(entry["Variable"]) if entry["Variable"] is not None else None
         return [question, list_answers, list_correct, dictionnaire_var]
```

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/messages.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/messages.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/parsing.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/parsing.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,16 +254,16 @@
         macros = [
             IDEs.IDE,
             IDEs.IDEv,
             IDEs.section,
 
             qcm.multi_qcm,
 
+            # isolated_components.py_sujet,     # just an alias for py, actually...
             isolated_components.py,
-            isolated_components.py_sujet,
             isolated_components.terminal,
         ]
         old_macros = [
             autres.cours,
             autres.exercice,
             autres.ext,
             autres.html_fig,
```

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/scripts/__init__.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/scripts/custom_lang.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/scripts/custom_lang.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/scripts/custom_lang_src.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/scripts/custom_lang_src.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/__init__.py` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,7 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
-
```

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/main.html` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/main.html`

 * *Files 2% similar despite different names*

```diff
@@ -16,32 +16,32 @@
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 -->
 
 {% extends "base.html" %}
 
 <!-- Load CDNs : Pyodide (Python in WASM), Ace (Editor) and JQuery (Terminal) and mathJax, then local scripts. -->
-<!-- WARNING: the mathjax tex-mml-chtml.js cdn must be loaded AFTER the config.js file has been loaded. -->
+<!-- WARNING: the mathjax tex-mml-chtml.js cdn must be loaded AFTER the pmt config-libs.js file has been loaded. -->
 {% block libs %}
 {{ super() }}
 <script src="https://cdn.jsdelivr.net/npm/lodash@4.17.20/lodash.min.js" type="text/javascript"></script>
 <script src="https://cdnjs.cloudflare.com/ajax/libs/ace/1.32.7/ace.min.js" charset="utf-8" type="text/javascript" integrity="sha512-GQpIYSKNIPIC763JKTNALj+t18/nfLdzw5gITgFGa31aK/4NmjyPKsfqrjh7CuzpJaG3nqEleeVcWUhHad9Axg==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
 <script src="https://cdnjs.cloudflare.com/ajax/libs/ace/1.32.7/ext-language_tools.min.js" charset="utf-8" type="text/javascript" integrity="sha512-iK7yTkCkv7MbFwTqRgHTbmIqoiiLq6BsyNjymnFyB5a7pEQwYThj9QIgqBy9+XPPwj7+hAEHyR2npOHL1bz4Qg==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
-<script src="https://cdn.jsdelivr.net/pyodide/v0.25.0/full/pyodide.js"></script>
 <script src="https://cdn.jsdelivr.net/npm/jquery"></script>
-<script src="https://cdn.jsdelivr.net/npm/jquery.terminal@2.34.0/js/jquery.terminal.min.js"></script>
+<script src="https://cdn.jsdelivr.net/npm/jquery.terminal/js/jquery.terminal.min.js"></script>
+<link href="https://cdn.jsdelivr.net/npm/jquery.terminal/css/jquery.terminal.min.css" rel="stylesheet"/>
+<script src="https://cdn.jsdelivr.net/pyodide/v0.25.0/full/pyodide.js"></script>
 <!-- PYODIDE - insertion token -->
 <script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/js-libs/0_config-libs.js"></script>
 {{ config.plugins.pyodide_macros.dump_to_js_config(base_url) }}
 <script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/js-libs/functools-libs.js"></script>
 <script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/js-libs/jsLogger-libs.js"></script>
 <script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/js-libs/mathjax-libs.js"></script>
 <script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/js-libs/securedPagesData-libs.js"></script>
 <script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/js-libs/z_globalGuiButtons-libs.js"></script>
-<link rel="stylesheet" href="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/terminal/css/0_cdn-terminal-replacement-libs.css">
 <link rel="stylesheet" href="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/IDE-and-buttons/ide-libs.css">
 <link rel="stylesheet" href="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/pyoditeur-libs.css">
 <link rel="stylesheet" href="{{ config.plugins.pyodide_macros.rebase(base_url) }}/qcm/qcm-libs.css">
 <link rel="stylesheet" href="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/terminal/css/terminal-libs.css">
 <link rel="stylesheet" href="{{ config.plugins.pyodide_macros.rebase(base_url) }}/js-libs/z_header-btns-libs.css">
 <!-- PYODIDE - insertion token -->
 <script src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js" type="text/javascript" charset="utf-8"></script>
```

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/mkdocs_theme.yml` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/mkdocs_theme.yml`

 * *Files 24% similar despite different names*

```diff
@@ -11,19 +11,36 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 # 
 # You should have received a copy of the GNU General Public License
 # along with this program.
 # If not, see <https://www.gnu.org/licenses/>.
 
+# pyodide-mkdocs-theme
+# Copyleft GNU GPLv3 🄯 2024 Frédéric Zinelli
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+# See the GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.
+# If not, see <https://www.gnu.org/licenses/>.
+
 extends: material
 
 language: fr
 
-font: false     # RGPD ; pas de fonte Google
+font: false     # RGPD ; pas de font Google
 
 palette:        # Palettes de couleurs jour/nuit
   - media: "(prefers-color-scheme: light)"
     scheme: default
     primary: dark blue
     accent: dark blue
     toggle:
```

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/partials/copyright.html` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/partials/copyright.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/partials/footer.html` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/partials/footer.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/partials/social.html` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/partials/social.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 */
 
 
 /* Common to all terminales.
    --n-lines is defined on the parent, through the terminal macro */
 .py_mk_terminal {
   --color: var(--main-theme);
+  --base-color: var(--main-theme);
   --background: var(--gutter-theme);
+  --base-background: var(--md-default-bg-color);    /* FIX wrong colors on selection */
   --size: 1.3;
   width: 100%;
   position: relative;
   overflow: auto;
 }
 
 .term_editor, .py_mk_terminal_solo {
@@ -49,8 +51,8 @@
   width: 24px;
   height: 24px;
   position: absolute;
   right: 7px;
   top: 5px;
   z-index: 101;   /* lol XD */
   font-family: var(--md-text-font-family);    /* for the tooltips */
-}
+}
```

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js` & `pyodide_mkdocs_theme-0.2.4/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.3/pyproject.toml` & `pyodide_mkdocs_theme-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyodide-mkdocs-theme"
-version = "0.2.3"
+version = "0.2.4"
 description = "Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations"
 authors = ["Frédéric Zinelli <frederic.zinelli@gmail.com>"]
 readme = "README.md"
 keywords = [
     "mkdocs", "mkdocs-plugin", "pyodide", "IDE", "terminal"
 ]
 classifiers = [
```

### Comparing `pyodide_mkdocs_theme-0.2.3/PKG-INFO` & `pyodide_mkdocs_theme-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-mkdocs-theme
-Version: 0.2.3
+Version: 0.2.4
 Summary: Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations
 Keywords: mkdocs,mkdocs-plugin,pyodide,IDE,terminal
 Author: Frédéric Zinelli
 Author-email: frederic.zinelli@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

