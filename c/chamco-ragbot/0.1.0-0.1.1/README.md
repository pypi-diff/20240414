# Comparing `tmp/chamco_ragbot-0.1.0.tar.gz` & `tmp/chamco_ragbot-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chamco_ragbot-0.1.0.tar", last modified: Sun Apr 14 04:14:04 2024, max compression
+gzip compressed data, was "chamco_ragbot-0.1.1.tar", last modified: Sun Apr 14 04:48:04 2024, max compression
```

## Comparing `chamco_ragbot-0.1.0.tar` & `chamco_ragbot-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-14 04:14:04.283025 chamco_ragbot-0.1.0/
--rw-r--r--   0 azureuser  (1000) azureuser  (1000)      127 2024-04-14 04:14:04.283025 chamco_ragbot-0.1.0/PKG-INFO
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-14 04:14:04.283025 chamco_ragbot-0.1.0/chamco_ragbot.egg-info/
--rw-r--r--   0 azureuser  (1000) azureuser  (1000)      127 2024-04-14 04:14:04.000000 chamco_ragbot-0.1.0/chamco_ragbot.egg-info/PKG-INFO
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      364 2024-04-14 04:14:04.000000 chamco_ragbot-0.1.0/chamco_ragbot.egg-info/SOURCES.txt
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        1 2024-04-14 04:14:04.000000 chamco_ragbot-0.1.0/chamco_ragbot.egg-info/dependency_links.txt
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       12 2024-04-14 04:14:04.000000 chamco_ragbot-0.1.0/chamco_ragbot.egg-info/top_level.txt
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-14 04:14:04.283025 chamco_ragbot-0.1.0/rag_chatbot/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-04-11 21:28:21.000000 chamco_ragbot-0.1.0/rag_chatbot/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2075 2024-04-13 11:53:51.000000 chamco_ragbot-0.1.0/rag_chatbot/chat.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1680 2024-04-13 13:22:14.000000 chamco_ragbot-0.1.0/rag_chatbot/datasource.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1821 2024-04-13 12:02:27.000000 chamco_ragbot-0.1.0/rag_chatbot/filetransfer.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5968 2024-04-13 13:52:34.000000 chamco_ragbot-0.1.0/rag_chatbot/index.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2276 2024-04-13 13:28:36.000000 chamco_ragbot-0.1.0/rag_chatbot/indexer.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1311 2024-04-13 14:41:11.000000 chamco_ragbot-0.1.0/rag_chatbot/main.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4195 2024-04-13 12:22:44.000000 chamco_ragbot-0.1.0/rag_chatbot/search.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3463 2024-04-13 13:20:43.000000 chamco_ragbot-0.1.0/rag_chatbot/skillset.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       38 2024-04-14 04:14:04.283025 chamco_ragbot-0.1.0/setup.cfg
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      287 2024-04-14 04:10:58.000000 chamco_ragbot-0.1.0/setup.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-14 04:48:04.445161 chamco_ragbot-0.1.1/
+-rw-r--r--   0 azureuser  (1000) azureuser  (1000)      127 2024-04-14 04:48:04.445161 chamco_ragbot-0.1.1/PKG-INFO
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-14 04:48:04.445161 chamco_ragbot-0.1.1/chamco_ragbot/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-04-11 21:28:21.000000 chamco_ragbot-0.1.1/chamco_ragbot/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2075 2024-04-13 11:53:51.000000 chamco_ragbot-0.1.1/chamco_ragbot/chat.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1680 2024-04-13 13:22:14.000000 chamco_ragbot-0.1.1/chamco_ragbot/datasource.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1821 2024-04-13 12:02:27.000000 chamco_ragbot-0.1.1/chamco_ragbot/filetransfer.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     5968 2024-04-13 13:52:34.000000 chamco_ragbot-0.1.1/chamco_ragbot/index.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2276 2024-04-13 13:28:36.000000 chamco_ragbot-0.1.1/chamco_ragbot/indexer.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1311 2024-04-13 14:41:11.000000 chamco_ragbot-0.1.1/chamco_ragbot/main.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4195 2024-04-13 12:22:44.000000 chamco_ragbot-0.1.1/chamco_ragbot/search.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3463 2024-04-13 13:20:43.000000 chamco_ragbot-0.1.1/chamco_ragbot/skillset.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-14 04:48:04.445161 chamco_ragbot-0.1.1/chamco_ragbot.egg-info/
+-rw-r--r--   0 azureuser  (1000) azureuser  (1000)      127 2024-04-14 04:48:04.000000 chamco_ragbot-0.1.1/chamco_ragbot.egg-info/PKG-INFO
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      382 2024-04-14 04:48:04.000000 chamco_ragbot-0.1.1/chamco_ragbot.egg-info/SOURCES.txt
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        1 2024-04-14 04:48:04.000000 chamco_ragbot-0.1.1/chamco_ragbot.egg-info/dependency_links.txt
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       14 2024-04-14 04:48:04.000000 chamco_ragbot-0.1.1/chamco_ragbot.egg-info/top_level.txt
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       38 2024-04-14 04:48:04.445161 chamco_ragbot-0.1.1/setup.cfg
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      287 2024-04-14 04:47:25.000000 chamco_ragbot-0.1.1/setup.py
```

### Comparing `chamco_ragbot-0.1.0/rag_chatbot/chat.py` & `chamco_ragbot-0.1.1/chamco_ragbot/chat.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.0/rag_chatbot/datasource.py` & `chamco_ragbot-0.1.1/chamco_ragbot/datasource.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.0/rag_chatbot/filetransfer.py` & `chamco_ragbot-0.1.1/chamco_ragbot/filetransfer.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.0/rag_chatbot/index.py` & `chamco_ragbot-0.1.1/chamco_ragbot/index.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.0/rag_chatbot/indexer.py` & `chamco_ragbot-0.1.1/chamco_ragbot/indexer.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.0/rag_chatbot/main.py` & `chamco_ragbot-0.1.1/chamco_ragbot/main.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.0/rag_chatbot/search.py` & `chamco_ragbot-0.1.1/chamco_ragbot/search.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.0/rag_chatbot/skillset.py` & `chamco_ragbot-0.1.1/chamco_ragbot/skillset.py`

 * *Files identical despite different names*

