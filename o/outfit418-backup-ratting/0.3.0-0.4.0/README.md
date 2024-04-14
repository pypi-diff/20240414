# Comparing `tmp/outfit418_backup_ratting-0.3.0.tar.gz` & `tmp/outfit418_backup_ratting-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outfit418_backup_ratting-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "outfit418_backup_ratting-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `outfit418_backup_ratting-0.3.0.tar` & `outfit418_backup_ratting-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     1539 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/LICENSE
--rwxr-xr-x   0        0        0      536 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/README.md
--rwxr-xr-x   0        0        0      143 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/__init__.py
--rwxr-xr-x   0        0        0      178 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/apps.py
--rwxr-xr-x   0        0        0     1206 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/auth_hooks.py
--rwxr-xr-x   0        0        0      108 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/forms.py
--rwxr-xr-x   0        0        0     1409 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/migrations/0001_initial.py
--rw-r--r--   0        0        0      660 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/migrations/0002_general.py
--rwxr-xr-x   0        0        0        0 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/migrations/__init__.py
--rwxr-xr-x   0        0        0      782 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/models.py
--rwxr-xr-x   0        0        0     3877 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/tasks.py
--rw-r--r--   0        0        0     1434 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/templates/outfit418_backup_ratting/audit.html
--rwxr-xr-x   0        0        0      486 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/templates/outfit418_backup_ratting/index.html
--rw-r--r--   0        0        0        0 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/templatetags/__init__.py
--rw-r--r--   0        0        0      269 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/templatetags/outfit_tags.py
--rwxr-xr-x   0        0        0      247 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/urls.py
--rwxr-xr-x   0        0        0      851 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/utils.py
--rwxr-xr-x   0        0        0     2363 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/views.py
--rwxr-xr-x   0        0        0      868 2024-04-08 14:03:34.489759 outfit418_backup_ratting-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 outfit418_backup_ratting-0.3.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1539 2024-04-14 15:37:02.715637 outfit418_backup_ratting-0.4.0/LICENSE
+-rwxr-xr-x   0        0        0      536 2024-04-14 15:37:02.715637 outfit418_backup_ratting-0.4.0/README.md
+-rwxr-xr-x   0        0        0      143 2024-04-14 15:37:02.715637 outfit418_backup_ratting-0.4.0/outfit418_backup_ratting/__init__.py
+-rwxr-xr-x   0        0        0      178 2024-04-14 15:37:02.715637 outfit418_backup_ratting-0.4.0/outfit418_backup_ratting/apps.py
+-rwxr-xr-x   0        0        0     1206 2024-04-14 15:37:02.715637 outfit418_backup_ratting-0.4.0/outfit418_backup_ratting/auth_hooks.py
+-rwxr-xr-x   0        0        0      108 2024-04-14 15:37:02.715637 outfit418_backup_ratting-0.4.0/outfit418_backup_ratting/forms.py
+-rwxr-xr-x   0        0        0     1409 2024-04-14 15:37:02.715637 outfit418_backup_ratting-0.4.0/outfit418_backup_ratting/migrations/0001_initial.py
+-rw-r--r--   0        0        0      660 2024-04-14 15:37:02.715637 outfit418_backup_ratting-0.4.0/outfit418_backup_ratting/migrations/0002_general.py
+-rwxr-xr-x   0        0        0        0 2024-04-14 15:37:02.715637 outfit418_backup_ratting-0.4.0/outfit418_backup_ratting/migrations/__init__.py
+-rwxr-xr-x   0        0        0      782 2024-04-14 15:37:02.715637 outfit418_backup_ratting-0.4.0/outfit418_backup_ratting/models.py
+-rwxr-xr-x   0        0        0     3877 2024-04-14 15:37:02.715637 outfit418_backup_ratting-0.4.0/outfit418_backup_ratting/tasks.py
+-rw-r--r--   0        0        0     1854 2024-04-14 15:37:02.715637 outfit418_backup_ratting-0.4.0/outfit418_backup_ratting/templates/outfit418_backup_ratting/audit.html
+-rwxr-xr-x   0        0        0      486 2024-04-14 15:37:02.719637 outfit418_backup_ratting-0.4.0/outfit418_backup_ratting/templates/outfit418_backup_ratting/index.html
+-rw-r--r--   0        0        0        0 2024-04-14 15:37:02.719637 outfit418_backup_ratting-0.4.0/outfit418_backup_ratting/templatetags/__init__.py
+-rw-r--r--   0        0        0      269 2024-04-14 15:37:02.719637 outfit418_backup_ratting-0.4.0/outfit418_backup_ratting/templatetags/outfit_tags.py
+-rwxr-xr-x   0        0        0      247 2024-04-14 15:37:02.719637 outfit418_backup_ratting-0.4.0/outfit418_backup_ratting/urls.py
+-rwxr-xr-x   0        0        0      851 2024-04-14 15:37:02.719637 outfit418_backup_ratting-0.4.0/outfit418_backup_ratting/utils.py
+-rwxr-xr-x   0        0        0     2363 2024-04-14 15:37:02.719637 outfit418_backup_ratting-0.4.0/outfit418_backup_ratting/views.py
+-rwxr-xr-x   0        0        0      868 2024-04-14 15:37:02.719637 outfit418_backup_ratting-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 outfit418_backup_ratting-0.4.0/PKG-INFO
```

### Comparing `outfit418_backup_ratting-0.3.0/LICENSE` & `outfit418_backup_ratting-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.3.0/README.md` & `outfit418_backup_ratting-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/auth_hooks.py` & `outfit418_backup_ratting-0.4.0/outfit418_backup_ratting/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/migrations/0001_initial.py` & `outfit418_backup_ratting-0.4.0/outfit418_backup_ratting/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/migrations/0002_general.py` & `outfit418_backup_ratting-0.4.0/outfit418_backup_ratting/migrations/0002_general.py`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/models.py` & `outfit418_backup_ratting-0.4.0/outfit418_backup_ratting/models.py`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/tasks.py` & `outfit418_backup_ratting-0.4.0/outfit418_backup_ratting/tasks.py`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/templates/outfit418_backup_ratting/audit.html` & `outfit418_backup_ratting-0.4.0/outfit418_backup_ratting/templates/outfit418_backup_ratting/audit.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 {% extends 'allianceauth/base-bs5.html' %}
 {% load outfit_tags %}
+{% load static %}
 
 {% block page_title %}418 Audit{% endblock page_title %}
 
 {% block extra_css %}
     {% include "bundles/datatables-css-bs5.html" %}
+    <link rel="stylesheet" type="text/css" href="{% static 'allianceauth_pve/css/spop.css' %}">
+    <link rel="stylesheet" type="text/css" href="{% allianceauth_pve_static 'allianceauth_pve/css/copy_text.css' %}">
 {% endblock %}
 
 {% block content %}
     <div class="col-lg-12" style="padding: 10px 10px 10px 10px">
         <table class="table table-aa">
             <thead>
                 <tr>
                     <th>Main</th>
                     <th>Characters</th>
                 </tr>
             </thead>
             <tbody>
                 {% for main in mains %}
                     <tr>
-                        <td>{{ main.character.character_name }}</td>
+                        <td><span class="copy-text">{{ main.character.character_name }}</span></td>
                         <td>
                             {% for char in main.character.character_ownership.user.chars %}
-                                <span class="badge {% if char.character|ct_is_active %}text-bg-primary{% else %}text-bg-danger{% endif %}">{{ char.character.character_name }}</span>
+                                <span class="badge {% if char.character|ct_is_active %}text-bg-primary{% else %}text-bg-danger{% endif %} copy-text">{{ char.character.character_name }}</span>
                             {% endfor %}
                         </td>
                     </tr>
                 {% endfor %}
             </tbody>
         </table>
     </div>
 {% endblock content %}
 
 {% block extra_javascript %}
     {% include "bundles/datatables-js-bs5.html" %}
+    <script src="{% static 'allianceauth_pve/js/spop.js' %}"></script>
+    <script src="{% static 'allianceauth_pve/js/copy_text.js' %}"></script>
 {% endblock extra_javascript %}
 
 {% block extra_script %}
     $(document).ready(function() {
         $('.table').DataTable({
             "pageLength": 50
         });
```

### Comparing `outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/utils.py` & `outfit418_backup_ratting-0.4.0/outfit418_backup_ratting/utils.py`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.3.0/outfit418_backup_ratting/views.py` & `outfit418_backup_ratting-0.4.0/outfit418_backup_ratting/views.py`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.3.0/pyproject.toml` & `outfit418_backup_ratting-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `outfit418_backup_ratting-0.3.0/PKG-INFO` & `outfit418_backup_ratting-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outfit418_backup_ratting
-Version: 0.3.0
+Version: 0.4.0
 Summary: Backup for Outfit418 data
 Keywords: allianceauth,allianceauth_pve,outfit418,eveonline
 Author-email: Matteo Ghia <matteo.ghia@yahoo.it>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: allianceauth~=4.0
 Requires-Dist: allianceauth_pve~=1.10
```

