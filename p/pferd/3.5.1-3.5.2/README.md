# Comparing `tmp/pferd-3.5.1.tar.gz` & `tmp/pferd-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pferd-3.5.1.tar", last modified: Tue Apr  9 12:36:09 2024, max compression
+gzip compressed data, was "pferd-3.5.2.tar", last modified: Sun Apr 14 10:22:27 2024, max compression
```

## Comparing `pferd-3.5.1.tar` & `pferd-3.5.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 pavel      (501) staff       (20)        0 2024-04-09 12:36:09.063778 pferd-3.5.1/
--rw-r--r--   0 pavel      (501) staff       (20)     1193 2024-04-09 12:36:05.000000 pferd-3.5.1/LICENSE
-drwxr-xr-x   0 pavel      (501) staff       (20)        0 2024-04-09 12:36:09.058623 pferd-3.5.1/PFERD/
--rw-r--r--   0 pavel      (501) staff       (20)        0 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/__init__.py
--rw-r--r--   0 pavel      (501) staff       (20)     5556 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/__main__.py
-drwxr-xr-x   0 pavel      (501) staff       (20)        0 2024-04-09 12:36:09.059517 pferd-3.5.1/PFERD/auth/
--rw-r--r--   0 pavel      (501) staff       (20)     1170 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/auth/__init__.py
--rw-r--r--   0 pavel      (501) staff       (20)     2194 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/auth/authenticator.py
--rw-r--r--   0 pavel      (501) staff       (20)     1649 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/auth/credential_file.py
--rw-r--r--   0 pavel      (501) staff       (20)     2234 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/auth/keyring.py
--rw-r--r--   0 pavel      (501) staff       (20)     3914 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/auth/pass_.py
--rw-r--r--   0 pavel      (501) staff       (20)     2052 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/auth/simple.py
--rw-r--r--   0 pavel      (501) staff       (20)      865 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/auth/tfa.py
-drwxr-xr-x   0 pavel      (501) staff       (20)        0 2024-04-09 12:36:09.060130 pferd-3.5.1/PFERD/cli/
--rw-r--r--   0 pavel      (501) staff       (20)      700 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/cli/__init__.py
--rw-r--r--   0 pavel      (501) staff       (20)     3415 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/cli/command_kit_ilias_web.py
--rw-r--r--   0 pavel      (501) staff       (20)     1199 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/cli/command_kit_ipd.py
--rw-r--r--   0 pavel      (501) staff       (20)     1688 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/cli/command_local.py
--rw-r--r--   0 pavel      (501) staff       (20)     7363 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/cli/parser.py
--rw-r--r--   0 pavel      (501) staff       (20)     6270 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/config.py
-drwxr-xr-x   0 pavel      (501) staff       (20)        0 2024-04-09 12:36:09.061401 pferd-3.5.1/PFERD/crawl/
--rw-r--r--   0 pavel      (501) staff       (20)     1013 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/crawl/__init__.py
--rw-r--r--   0 pavel      (501) staff       (20)    12151 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/crawl/crawler.py
--rw-r--r--   0 pavel      (501) staff       (20)     8191 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/crawl/http_crawler.py
-drwxr-xr-x   0 pavel      (501) staff       (20)        0 2024-04-09 12:36:09.062246 pferd-3.5.1/PFERD/crawl/ilias/
--rw-r--r--   0 pavel      (501) staff       (20)      144 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/crawl/ilias/__init__.py
--rw-r--r--   0 pavel      (501) staff       (20)     9052 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/crawl/ilias/file_templates.py
--rw-r--r--   0 pavel      (501) staff       (20)     2209 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/crawl/ilias/ilias_html_cleaner.py
--rw-r--r--   0 pavel      (501) staff       (20)    48636 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/crawl/ilias/kit_ilias_html.py
--rw-r--r--   0 pavel      (501) staff       (20)    47253 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/crawl/ilias/kit_ilias_web_crawler.py
--rw-r--r--   0 pavel      (501) staff       (20)     5832 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/crawl/kit_ipd_crawler.py
--rw-r--r--   0 pavel      (501) staff       (20)     3676 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/crawl/local_crawler.py
--rw-r--r--   0 pavel      (501) staff       (20)     2816 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/deduplicator.py
--rw-r--r--   0 pavel      (501) staff       (20)     2808 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/limiter.py
--rw-r--r--   0 pavel      (501) staff       (20)     9320 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/logging.py
--rw-r--r--   0 pavel      (501) staff       (20)    18050 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/output_dir.py
--rw-r--r--   0 pavel      (501) staff       (20)     7442 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/pferd.py
--rw-r--r--   0 pavel      (501) staff       (20)     7944 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/report.py
--rw-r--r--   0 pavel      (501) staff       (20)    11927 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/transformer.py
--rw-r--r--   0 pavel      (501) staff       (20)     3858 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/utils.py
--rw-r--r--   0 pavel      (501) staff       (20)       33 2024-04-09 12:36:05.000000 pferd-3.5.1/PFERD/version.py
--rw-r--r--   0 pavel      (501) staff       (20)     6597 2024-04-09 12:36:09.063710 pferd-3.5.1/PKG-INFO
--rw-r--r--   0 pavel      (501) staff       (20)     4654 2024-04-09 12:36:05.000000 pferd-3.5.1/README.md
-drwxr-xr-x   0 pavel      (501) staff       (20)        0 2024-04-09 12:36:09.063309 pferd-3.5.1/pferd.egg-info/
--rw-r--r--   0 pavel      (501) staff       (20)     6597 2024-04-09 12:36:09.000000 pferd-3.5.1/pferd.egg-info/PKG-INFO
--rw-r--r--   0 pavel      (501) staff       (20)     1045 2024-04-09 12:36:09.000000 pferd-3.5.1/pferd.egg-info/SOURCES.txt
--rw-r--r--   0 pavel      (501) staff       (20)        1 2024-04-09 12:36:09.000000 pferd-3.5.1/pferd.egg-info/dependency_links.txt
--rw-r--r--   0 pavel      (501) staff       (20)       46 2024-04-09 12:36:09.000000 pferd-3.5.1/pferd.egg-info/entry_points.txt
--rw-r--r--   0 pavel      (501) staff       (20)       86 2024-04-09 12:36:09.000000 pferd-3.5.1/pferd.egg-info/requires.txt
--rw-r--r--   0 pavel      (501) staff       (20)        6 2024-04-09 12:36:09.000000 pferd-3.5.1/pferd.egg-info/top_level.txt
--rw-r--r--   0 pavel      (501) staff       (20)      781 2024-04-09 12:36:05.000000 pferd-3.5.1/pyproject.toml
--rw-r--r--   0 pavel      (501) staff       (20)      395 2024-04-09 12:36:09.064047 pferd-3.5.1/setup.cfg
+drwxr-xr-x   0 pavel      (501) staff       (20)        0 2024-04-14 10:22:27.680773 pferd-3.5.2/
+-rw-r--r--   0 pavel      (501) staff       (20)     1193 2024-04-14 10:22:21.000000 pferd-3.5.2/LICENSE
+drwxr-xr-x   0 pavel      (501) staff       (20)        0 2024-04-14 10:22:27.676076 pferd-3.5.2/PFERD/
+-rw-r--r--   0 pavel      (501) staff       (20)        0 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/__init__.py
+-rw-r--r--   0 pavel      (501) staff       (20)     5556 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/__main__.py
+drwxr-xr-x   0 pavel      (501) staff       (20)        0 2024-04-14 10:22:27.676989 pferd-3.5.2/PFERD/auth/
+-rw-r--r--   0 pavel      (501) staff       (20)     1170 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/auth/__init__.py
+-rw-r--r--   0 pavel      (501) staff       (20)     2194 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/auth/authenticator.py
+-rw-r--r--   0 pavel      (501) staff       (20)     1649 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/auth/credential_file.py
+-rw-r--r--   0 pavel      (501) staff       (20)     2234 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/auth/keyring.py
+-rw-r--r--   0 pavel      (501) staff       (20)     3914 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/auth/pass_.py
+-rw-r--r--   0 pavel      (501) staff       (20)     2052 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/auth/simple.py
+-rw-r--r--   0 pavel      (501) staff       (20)      865 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/auth/tfa.py
+drwxr-xr-x   0 pavel      (501) staff       (20)        0 2024-04-14 10:22:27.677574 pferd-3.5.2/PFERD/cli/
+-rw-r--r--   0 pavel      (501) staff       (20)      700 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/cli/__init__.py
+-rw-r--r--   0 pavel      (501) staff       (20)     3415 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/cli/command_kit_ilias_web.py
+-rw-r--r--   0 pavel      (501) staff       (20)     1199 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/cli/command_kit_ipd.py
+-rw-r--r--   0 pavel      (501) staff       (20)     1688 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/cli/command_local.py
+-rw-r--r--   0 pavel      (501) staff       (20)     7363 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/cli/parser.py
+-rw-r--r--   0 pavel      (501) staff       (20)     6270 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/config.py
+drwxr-xr-x   0 pavel      (501) staff       (20)        0 2024-04-14 10:22:27.678473 pferd-3.5.2/PFERD/crawl/
+-rw-r--r--   0 pavel      (501) staff       (20)     1013 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/crawl/__init__.py
+-rw-r--r--   0 pavel      (501) staff       (20)    12151 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/crawl/crawler.py
+-rw-r--r--   0 pavel      (501) staff       (20)     8191 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/crawl/http_crawler.py
+drwxr-xr-x   0 pavel      (501) staff       (20)        0 2024-04-14 10:22:27.679211 pferd-3.5.2/PFERD/crawl/ilias/
+-rw-r--r--   0 pavel      (501) staff       (20)      144 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/crawl/ilias/__init__.py
+-rw-r--r--   0 pavel      (501) staff       (20)     9052 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/crawl/ilias/file_templates.py
+-rw-r--r--   0 pavel      (501) staff       (20)     2209 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/crawl/ilias/ilias_html_cleaner.py
+-rw-r--r--   0 pavel      (501) staff       (20)    49193 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/crawl/ilias/kit_ilias_html.py
+-rw-r--r--   0 pavel      (501) staff       (20)    47265 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/crawl/ilias/kit_ilias_web_crawler.py
+-rw-r--r--   0 pavel      (501) staff       (20)     5832 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/crawl/kit_ipd_crawler.py
+-rw-r--r--   0 pavel      (501) staff       (20)     3676 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/crawl/local_crawler.py
+-rw-r--r--   0 pavel      (501) staff       (20)     2816 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/deduplicator.py
+-rw-r--r--   0 pavel      (501) staff       (20)     2808 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/limiter.py
+-rw-r--r--   0 pavel      (501) staff       (20)     9320 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/logging.py
+-rw-r--r--   0 pavel      (501) staff       (20)    18050 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/output_dir.py
+-rw-r--r--   0 pavel      (501) staff       (20)     7442 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/pferd.py
+-rw-r--r--   0 pavel      (501) staff       (20)     7944 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/report.py
+-rw-r--r--   0 pavel      (501) staff       (20)    11927 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/transformer.py
+-rw-r--r--   0 pavel      (501) staff       (20)     3858 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/utils.py
+-rw-r--r--   0 pavel      (501) staff       (20)       33 2024-04-14 10:22:21.000000 pferd-3.5.2/PFERD/version.py
+-rw-r--r--   0 pavel      (501) staff       (20)     6597 2024-04-14 10:22:27.680693 pferd-3.5.2/PKG-INFO
+-rw-r--r--   0 pavel      (501) staff       (20)     4654 2024-04-14 10:22:21.000000 pferd-3.5.2/README.md
+drwxr-xr-x   0 pavel      (501) staff       (20)        0 2024-04-14 10:22:27.680350 pferd-3.5.2/pferd.egg-info/
+-rw-r--r--   0 pavel      (501) staff       (20)     6597 2024-04-14 10:22:27.000000 pferd-3.5.2/pferd.egg-info/PKG-INFO
+-rw-r--r--   0 pavel      (501) staff       (20)     1045 2024-04-14 10:22:27.000000 pferd-3.5.2/pferd.egg-info/SOURCES.txt
+-rw-r--r--   0 pavel      (501) staff       (20)        1 2024-04-14 10:22:27.000000 pferd-3.5.2/pferd.egg-info/dependency_links.txt
+-rw-r--r--   0 pavel      (501) staff       (20)       46 2024-04-14 10:22:27.000000 pferd-3.5.2/pferd.egg-info/entry_points.txt
+-rw-r--r--   0 pavel      (501) staff       (20)       86 2024-04-14 10:22:27.000000 pferd-3.5.2/pferd.egg-info/requires.txt
+-rw-r--r--   0 pavel      (501) staff       (20)        6 2024-04-14 10:22:27.000000 pferd-3.5.2/pferd.egg-info/top_level.txt
+-rw-r--r--   0 pavel      (501) staff       (20)      781 2024-04-14 10:22:21.000000 pferd-3.5.2/pyproject.toml
+-rw-r--r--   0 pavel      (501) staff       (20)      395 2024-04-14 10:22:27.681044 pferd-3.5.2/setup.cfg
```

### Comparing `pferd-3.5.1/LICENSE` & `pferd-3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/__main__.py` & `pferd-3.5.2/PFERD/__main__.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/auth/__init__.py` & `pferd-3.5.2/PFERD/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/auth/authenticator.py` & `pferd-3.5.2/PFERD/auth/authenticator.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/auth/credential_file.py` & `pferd-3.5.2/PFERD/auth/credential_file.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/auth/keyring.py` & `pferd-3.5.2/PFERD/auth/keyring.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/auth/pass_.py` & `pferd-3.5.2/PFERD/auth/pass_.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/auth/simple.py` & `pferd-3.5.2/PFERD/auth/simple.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/auth/tfa.py` & `pferd-3.5.2/PFERD/auth/tfa.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/cli/__init__.py` & `pferd-3.5.2/PFERD/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/cli/command_kit_ilias_web.py` & `pferd-3.5.2/PFERD/cli/command_kit_ilias_web.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/cli/command_kit_ipd.py` & `pferd-3.5.2/PFERD/cli/command_kit_ipd.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/cli/command_local.py` & `pferd-3.5.2/PFERD/cli/command_local.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/cli/parser.py` & `pferd-3.5.2/PFERD/cli/parser.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/config.py` & `pferd-3.5.2/PFERD/config.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/crawl/__init__.py` & `pferd-3.5.2/PFERD/crawl/__init__.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/crawl/crawler.py` & `pferd-3.5.2/PFERD/crawl/crawler.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/crawl/http_crawler.py` & `pferd-3.5.2/PFERD/crawl/http_crawler.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/crawl/ilias/file_templates.py` & `pferd-3.5.2/PFERD/crawl/ilias/file_templates.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/crawl/ilias/ilias_html_cleaner.py` & `pferd-3.5.2/PFERD/crawl/ilias/ilias_html_cleaner.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/crawl/ilias/kit_ilias_html.py` & `pferd-3.5.2/PFERD/crawl/ilias/kit_ilias_html.py`

 * *Files 1% similar despite different names*

```diff
@@ -374,14 +374,18 @@
 
         titles: List[Tag] = self._soup.select(".il-item-title")
         for title in titles:
             link = title.find("a")
             name = _sanitize_path_name(link.text.strip())
             url = self._abs_url_from_link(link)
 
+            if "cmd=manage" in url and "cmdClass=ilPDSelectedItemsBlockGUI" in url:
+                # Configure button/link does not have anything interesting
+                continue
+
             type = self._find_type_from_link(name, link, url)
             if not type:
                 _unexpected_html_warning()
                 log.warn_contd(f"Could not extract type for {link}")
                 continue
 
             log.explain(f"Found {name!r}")
@@ -1070,14 +1074,22 @@
             shib_login = soup.find(id="button_shib_login")
             return not login_button and not shib_login
 
         # Personal Desktop
         if soup.find("a", attrs={"href": lambda x: x and "block_type=pditems" in x}):
             return True
 
+        # Empty personal desktop has zero (0) markers. Match on the text...
+        if alert := soup.select_one(".alert-info"):
+            text = alert.getText().lower()
+            if "you have not yet selected any favourites" in text:
+                return True
+            if "sie haben aktuell noch keine favoriten ausgewählt" in text:
+                return True
+
         # Video listing embeds do not have complete ILIAS html. Try to match them by
         # their video listing table
         video_table = soup.find(
             recursive=True,
             name="table",
             attrs={"id": lambda x: x is not None and x.startswith("tbl_xoct")}
         )
```

### Comparing `pferd-3.5.1/PFERD/crawl/ilias/kit_ilias_web_crawler.py` & `pferd-3.5.2/PFERD/crawl/ilias/kit_ilias_web_crawler.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
         root_url = url_set_query_param(
             self._base_url + "/goto.php", "target", f"crs_{course_id}"
         )
 
         await self._crawl_url(root_url, expected_id=course_id)
 
     async def _crawl_desktop(self) -> None:
-        appendix = r"ILIAS\PersonalDesktop\PDMainBarProvider|mm_pd_sel_items"
+        appendix = r"ILIAS\Repository\Provider\RepositoryMainBarProvider|mm_pd_sel_items"
         appendix = appendix.encode("ASCII").hex()
         await self._crawl_url(self._base_url + "/gs_content.php?item=" + appendix)
 
     async def _crawl_url(self, url: str, expected_id: Optional[int] = None) -> None:
         maybe_cl = await self.crawl(PurePath("."))
         if not maybe_cl:
             return
```

### Comparing `pferd-3.5.1/PFERD/crawl/kit_ipd_crawler.py` & `pferd-3.5.2/PFERD/crawl/kit_ipd_crawler.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/crawl/local_crawler.py` & `pferd-3.5.2/PFERD/crawl/local_crawler.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/deduplicator.py` & `pferd-3.5.2/PFERD/deduplicator.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/limiter.py` & `pferd-3.5.2/PFERD/limiter.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/logging.py` & `pferd-3.5.2/PFERD/logging.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/output_dir.py` & `pferd-3.5.2/PFERD/output_dir.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/pferd.py` & `pferd-3.5.2/PFERD/pferd.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/report.py` & `pferd-3.5.2/PFERD/report.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/transformer.py` & `pferd-3.5.2/PFERD/transformer.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PFERD/utils.py` & `pferd-3.5.2/PFERD/utils.py`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/PKG-INFO` & `pferd-3.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pferd
-Version: 3.5.1
+Version: 3.5.2
 Summary: Programm zum Flotten Einfachen Runterladen von Dateien
 Author-email: Garmelon <joscha@plugh.de>
 License: Copyright 2019-2021 Garmelon, I-Al-Istannen, danstooamerican, pavelzw,
                             TheChristophe, Scriptim, thelukasprobst, Toorero,
                             Mr-Pine
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

### Comparing `pferd-3.5.1/README.md` & `pferd-3.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/pferd.egg-info/PKG-INFO` & `pferd-3.5.2/pferd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pferd
-Version: 3.5.1
+Version: 3.5.2
 Summary: Programm zum Flotten Einfachen Runterladen von Dateien
 Author-email: Garmelon <joscha@plugh.de>
 License: Copyright 2019-2021 Garmelon, I-Al-Istannen, danstooamerican, pavelzw,
                             TheChristophe, Scriptim, thelukasprobst, Toorero,
                             Mr-Pine
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

### Comparing `pferd-3.5.1/pferd.egg-info/SOURCES.txt` & `pferd-3.5.2/pferd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pferd-3.5.1/pyproject.toml` & `pferd-3.5.2/pyproject.toml`

 * *Files identical despite different names*

