# Comparing `tmp/slack-export-viewer-1.4.2.tar.gz` & `tmp/slack_export_viewer-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack-export-viewer-1.4.2.tar", last modified: Thu Mar 28 19:28:53 2024, max compression
+gzip compressed data, was "slack_export_viewer-1.4.3.tar", last modified: Sun Apr 14 00:45:53 2024, max compression
```

## Comparing `slack-export-viewer-1.4.2.tar` & `slack_export_viewer-1.4.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:28:53.514073 slack-export-viewer-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-28 19:28:49.000000 slack-export-viewer-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-28 19:28:49.000000 slack-export-viewer-1.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-28 19:28:53.514073 slack-export-viewer-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-03-28 19:28:49.000000 slack-export-viewer-1.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-28 19:28:49.000000 slack-export-viewer-1.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)   158989 2024-03-28 19:28:49.000000 slack-export-viewer-1.4.2/screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 19:28:53.514073 slack-export-viewer-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-28 19:28:49.000000 slack-export-viewer-1.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:28:53.514073 slack-export-viewer-1.4.2/slack_export_viewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-28 19:28:53.000000 slack-export-viewer-1.4.2/slack_export_viewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-28 19:28:53.000000 slack-export-viewer-1.4.2/slack_export_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 19:28:53.000000 slack-export-viewer-1.4.2/slack_export_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-28 19:28:53.000000 slack-export-viewer-1.4.2/slack_export_viewer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 19:28:53.000000 slack-export-viewer-1.4.2/slack_export_viewer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-28 19:28:53.000000 slack-export-viewer-1.4.2/slack_export_viewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-28 19:28:53.000000 slack-export-viewer-1.4.2/slack_export_viewer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:28:53.514073 slack-export-viewer-1.4.2/slackviewer/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-28 19:28:49.000000 slack-export-viewer-1.4.2/slackviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-03-28 19:28:49.000000 slack-export-viewer-1.4.2/slackviewer/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-03-28 19:28:49.000000 slack-export-viewer-1.4.2/slackviewer/archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-03-28 19:28:49.000000 slack-export-viewer-1.4.2/slackviewer/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-28 19:28:49.000000 slack-export-viewer-1.4.2/slackviewer/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-03-28 19:28:49.000000 slack-export-viewer-1.4.2/slackviewer/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-28 19:28:49.000000 slack-export-viewer-1.4.2/slackviewer/freezer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-03-28 19:28:49.000000 slack-export-viewer-1.4.2/slackviewer/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-03-28 19:28:49.000000 slack-export-viewer-1.4.2/slackviewer/message.py
--rw-r--r--   0 runner    (1001) docker     (127)    10235 2024-03-28 19:28:49.000000 slack-export-viewer-1.4.2/slackviewer/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:28:53.514073 slack-export-viewer-1.4.2/slackviewer/static/
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-03-28 19:28:49.000000 slack-export-viewer-1.4.2/slackviewer/static/viewer.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:28:53.514073 slack-export-viewer-1.4.2/slackviewer/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-03-28 19:28:49.000000 slack-export-viewer-1.4.2/slackviewer/templates/export_single.html
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-03-28 19:28:49.000000 slack-export-viewer-1.4.2/slackviewer/templates/util.html
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-03-28 19:28:49.000000 slack-export-viewer-1.4.2/slackviewer/templates/viewer.html
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-03-28 19:28:49.000000 slack-export-viewer-1.4.2/slackviewer/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:28:53.514073 slack-export-viewer-1.4.2/slackviewer/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 19:28:49.000000 slack-export-viewer-1.4.2/slackviewer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-28 19:28:49.000000 slack-export-viewer-1.4.2/slackviewer/utils/click.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-28 19:28:49.000000 slack-export-viewer-1.4.2/slackviewer/utils/six.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:28:53.514073 slack-export-viewer-1.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-28 19:28:49.000000 slack-export-viewer-1.4.2/tests/test_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:45:53.434623 slack_export_viewer-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-14 00:45:47.000000 slack_export_viewer-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-14 00:45:47.000000 slack_export_viewer-1.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-14 00:45:53.434623 slack_export_viewer-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-04-14 00:45:47.000000 slack_export_viewer-1.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-14 00:45:47.000000 slack_export_viewer-1.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   158989 2024-04-14 00:45:47.000000 slack_export_viewer-1.4.3/screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 00:45:53.434623 slack_export_viewer-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-14 00:45:47.000000 slack_export_viewer-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:45:53.434623 slack_export_viewer-1.4.3/slack_export_viewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-14 00:45:53.000000 slack_export_viewer-1.4.3/slack_export_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-14 00:45:53.000000 slack_export_viewer-1.4.3/slack_export_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 00:45:53.000000 slack_export_viewer-1.4.3/slack_export_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-14 00:45:53.000000 slack_export_viewer-1.4.3/slack_export_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 00:45:53.000000 slack_export_viewer-1.4.3/slack_export_viewer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-14 00:45:53.000000 slack_export_viewer-1.4.3/slack_export_viewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-14 00:45:53.000000 slack_export_viewer-1.4.3/slack_export_viewer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:45:53.434623 slack_export_viewer-1.4.3/slackviewer/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-14 00:45:47.000000 slack_export_viewer-1.4.3/slackviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-14 00:45:47.000000 slack_export_viewer-1.4.3/slackviewer/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-14 00:45:47.000000 slack_export_viewer-1.4.3/slackviewer/archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-14 00:45:47.000000 slack_export_viewer-1.4.3/slackviewer/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-14 00:45:47.000000 slack_export_viewer-1.4.3/slackviewer/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-04-14 00:45:47.000000 slack_export_viewer-1.4.3/slackviewer/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-14 00:45:47.000000 slack_export_viewer-1.4.3/slackviewer/freezer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-14 00:45:47.000000 slack_export_viewer-1.4.3/slackviewer/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-04-14 00:45:47.000000 slack_export_viewer-1.4.3/slackviewer/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10235 2024-04-14 00:45:47.000000 slack_export_viewer-1.4.3/slackviewer/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:45:53.434623 slack_export_viewer-1.4.3/slackviewer/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-14 00:45:47.000000 slack_export_viewer-1.4.3/slackviewer/static/viewer.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:45:53.434623 slack_export_viewer-1.4.3/slackviewer/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-14 00:45:47.000000 slack_export_viewer-1.4.3/slackviewer/templates/export_single.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-04-14 00:45:47.000000 slack_export_viewer-1.4.3/slackviewer/templates/util.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-04-14 00:45:47.000000 slack_export_viewer-1.4.3/slackviewer/templates/viewer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-14 00:45:47.000000 slack_export_viewer-1.4.3/slackviewer/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:45:53.434623 slack_export_viewer-1.4.3/slackviewer/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 00:45:47.000000 slack_export_viewer-1.4.3/slackviewer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-14 00:45:47.000000 slack_export_viewer-1.4.3/slackviewer/utils/click.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-14 00:45:47.000000 slack_export_viewer-1.4.3/slackviewer/utils/six.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:45:53.434623 slack_export_viewer-1.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-14 00:45:47.000000 slack_export_viewer-1.4.3/tests/test_archive.py
```

### Comparing `slack-export-viewer-1.4.2/LICENSE` & `slack_export_viewer-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.4.2/PKG-INFO` & `slack_export_viewer-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-export-viewer
-Version: 1.4.2
+Version: 1.4.3
 Summary: Slack Export Archive Viewer
 Home-page: https://github.com/hfaran/slack-export-viewer
 Author: Hamza Faran
 Author-email: hamzafaran@outlook.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `slack-export-viewer-1.4.2/README.md` & `slack_export_viewer-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.4.2/screenshot.png` & `slack_export_viewer-1.4.3/screenshot.png`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.4.2/setup.py` & `slack_export_viewer-1.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.4.2/slack_export_viewer.egg-info/PKG-INFO` & `slack_export_viewer-1.4.3/slack_export_viewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-export-viewer
-Version: 1.4.2
+Version: 1.4.3
 Summary: Slack Export Archive Viewer
 Home-page: https://github.com/hfaran/slack-export-viewer
 Author: Hamza Faran
 Author-email: hamzafaran@outlook.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `slack-export-viewer-1.4.2/slack_export_viewer.egg-info/SOURCES.txt` & `slack_export_viewer-1.4.3/slack_export_viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.4.2/slackviewer/app.py` & `slack_export_viewer-1.4.3/slackviewer/app.py`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.4.2/slackviewer/archive.py` & `slack_export_viewer-1.4.3/slackviewer/archive.py`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.4.2/slackviewer/cli.py` & `slack_export_viewer-1.4.3/slackviewer/cli.py`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.4.2/slackviewer/formatter.py` & `slack_export_viewer-1.4.3/slackviewer/formatter.py`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.4.2/slackviewer/main.py` & `slack_export_viewer-1.4.3/slackviewer/main.py`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.4.2/slackviewer/message.py` & `slack_export_viewer-1.4.3/slackviewer/message.py`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.4.2/slackviewer/reader.py` & `slack_export_viewer-1.4.3/slackviewer/reader.py`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.4.2/slackviewer/static/viewer.css` & `slack_export_viewer-1.4.3/slackviewer/static/viewer.css`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.4.2/slackviewer/templates/export_single.html` & `slack_export_viewer-1.4.3/slackviewer/templates/export_single.html`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.4.2/slackviewer/templates/util.html` & `slack_export_viewer-1.4.3/slackviewer/templates/util.html`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.4.2/slackviewer/templates/viewer.html` & `slack_export_viewer-1.4.3/slackviewer/templates/viewer.html`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             {% endfor %}
         </ul>
     </div>
     {% endif %}
     <div class="messages">
         {% for message in messages %}
             {% if message.msg or message.files %}
-                {% if "Thread Reply:" in message.msg %}
+                {% if message.msg and "Thread Reply:" in message.msg %}
                     {{render_message(message, None, no_external_references, reply=True)}}
                 {% else %}
                     {{render_message(message, None, no_external_references, reply=False)}}
                 {% endif %}
             {% endif %}
         {% endfor %}
     </div>
```

#### html2text {}

```diff
@@ -19,11 +19,11 @@
 ******** GGrroouupp DDiirreecctt MMeessssaaggeess ********
     * {% for mpim in mpim_users %}
     * __ _{_%_ _f_o_r_ _u_s_e_r_ _i_n_ _m_p_i_m_[_"_u_s_e_r_s_"_]_ _%_}_ _{_{_ _u_s_e_r_._r_e_a_l___n_a_m_e_ _i_f_ _u_s_e_r_._r_e_a_l___n_a_m_e
       _e_l_s_e_ _u_s_e_r_._n_a_m_e_ _}_}_,_ _{_%_ _e_n_d_f_o_r_ _%_}
     * {% endfor %}
 {% endif %}
 {% for message in messages %} {% if message.msg or message.files %} {% if
-"Thread Reply:" in message.msg %} {{render_message(message, None,
-no_external_references, reply=True)}} {% else %} {{render_message(message,
-None, no_external_references, reply=False)}} {% endif %} {% endif %} {% endfor
-%}
+message.msg and "Thread Reply:" in message.msg %} {{render_message(message,
+None, no_external_references, reply=True)}} {% else %} {{render_message
+(message, None, no_external_references, reply=False)}} {% endif %} {% endif %}
+{% endfor %}
```

### Comparing `slack-export-viewer-1.4.2/slackviewer/user.py` & `slack_export_viewer-1.4.3/slackviewer/user.py`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.4.2/slackviewer/utils/six.py` & `slack_export_viewer-1.4.3/slackviewer/utils/six.py`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.4.2/tests/test_archive.py` & `slack_export_viewer-1.4.3/tests/test_archive.py`

 * *Files identical despite different names*

