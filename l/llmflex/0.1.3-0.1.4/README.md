# Comparing `tmp/llmflex-0.1.3.tar.gz` & `tmp/llmflex-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmflex-0.1.3.tar", last modified: Tue Apr  9 19:26:50 2024, max compression
+gzip compressed data, was "llmflex-0.1.4.tar", last modified: Sun Apr 14 12:29:51 2024, max compression
```

## Comparing `llmflex-0.1.3.tar` & `llmflex-0.1.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.976054 llmflex-0.1.3/
--rw-r--r--   0 nathan95   (501) staff       (20)     1067 2024-01-22 01:35:14.000000 llmflex-0.1.3/LICENSE.md
--rw-r--r--   0 nathan95   (501) staff       (20)     9750 2024-04-09 19:26:50.975682 llmflex-0.1.3/PKG-INFO
--rw-r--r--   0 nathan95   (501) staff       (20)     8569 2024-04-09 19:26:07.000000 llmflex-0.1.3/README.md
--rw-r--r--   0 nathan95   (501) staff       (20)     1196 2024-02-24 22:31:02.000000 llmflex-0.1.3/pyproject.toml
--rw-r--r--   0 nathan95   (501) staff       (20)       38 2024-04-09 19:26:50.976099 llmflex-0.1.3/setup.cfg
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.962074 llmflex-0.1.3/src/
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.963637 llmflex-0.1.3/src/llmflex/
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.964711 llmflex-0.1.3/src/llmflex/Data/
--rw-r--r--   0 nathan95   (501) staff       (20)       43 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Data/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     4919 2024-02-24 22:31:02.000000 llmflex-0.1.3/src/llmflex/Data/sqlite_database.py
--rw-r--r--   0 nathan95   (501) staff       (20)    20029 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Data/vector_database.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.965618 llmflex-0.1.3/src/llmflex/Embeddings/
--rw-r--r--   0 nathan95   (501) staff       (20)      226 2024-02-24 22:31:02.000000 llmflex-0.1.3/src/llmflex/Embeddings/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     4400 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Embeddings/api_embeddings.py
--rw-r--r--   0 nathan95   (501) staff       (20)     4245 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Embeddings/base_embeddings.py
--rw-r--r--   0 nathan95   (501) staff       (20)     2275 2024-03-15 22:38:26.000000 llmflex-0.1.3/src/llmflex/Embeddings/hf_embeddings_server.py
--rw-r--r--   0 nathan95   (501) staff       (20)     3998 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Embeddings/huggingface_embeddings.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.966031 llmflex-0.1.3/src/llmflex/Frontend/
--rw-r--r--   0 nathan95   (501) staff       (20)      102 2024-02-24 22:31:02.000000 llmflex-0.1.3/src/llmflex/Frontend/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    29992 2024-02-24 22:31:02.000000 llmflex-0.1.3/src/llmflex/Frontend/gradio_interface.py
--rw-r--r--   0 nathan95   (501) staff       (20)    37390 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Frontend/streamlit_interface.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.966567 llmflex-0.1.3/src/llmflex/Memory/
--rw-r--r--   0 nathan95   (501) staff       (20)      287 2024-02-24 22:31:02.000000 llmflex-0.1.3/src/llmflex/Memory/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     8298 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Memory/assistant_long_term_memory.py
--rw-r--r--   0 nathan95   (501) staff       (20)     8703 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Memory/base_memory.py
--rw-r--r--   0 nathan95   (501) staff       (20)     7727 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Memory/long_short_memory.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.966695 llmflex-0.1.3/src/llmflex/Models/
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.967574 llmflex-0.1.3/src/llmflex/Models/Cores/
--rw-r--r--   0 nathan95   (501) staff       (20)        0 2024-02-24 22:31:02.000000 llmflex-0.1.3/src/llmflex/Models/Cores/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    14712 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Models/Cores/base_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     7915 2024-02-25 22:17:53.000000 llmflex-0.1.3/src/llmflex/Models/Cores/exllamav2_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     9508 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Models/Cores/huggingface_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     8610 2024-02-25 22:17:53.000000 llmflex-0.1.3/src/llmflex/Models/Cores/llamacpp_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     9239 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Models/Cores/openai_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     7368 2024-02-28 15:01:21.000000 llmflex-0.1.3/src/llmflex/Models/Cores/utils.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.967799 llmflex-0.1.3/src/llmflex/Models/Factory/
--rw-r--r--   0 nathan95   (501) staff       (20)        0 2024-02-24 22:31:02.000000 llmflex-0.1.3/src/llmflex/Models/Factory/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    10725 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Models/Factory/llm_factory.py
--rw-r--r--   0 nathan95   (501) staff       (20)       43 2024-02-24 22:31:02.000000 llmflex-0.1.3/src/llmflex/Models/__init__.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.968030 llmflex-0.1.3/src/llmflex/Prompts/
--rw-r--r--   0 nathan95   (501) staff       (20)       52 2024-02-24 22:31:02.000000 llmflex-0.1.3/src/llmflex/Prompts/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    14910 2024-04-09 19:26:07.000000 llmflex-0.1.3/src/llmflex/Prompts/prompt_template.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.968262 llmflex-0.1.3/src/llmflex/Schemas/
--rw-r--r--   0 nathan95   (501) staff       (20)       31 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Schemas/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)      140 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Schemas/documents.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.968730 llmflex-0.1.3/src/llmflex/TextSplitters/
--rw-r--r--   0 nathan95   (501) staff       (20)      123 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/TextSplitters/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     1526 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/TextSplitters/base_text_splitter.py
--rw-r--r--   0 nathan95   (501) staff       (20)     2709 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/TextSplitters/sentence_token_text_splitter.py
--rw-r--r--   0 nathan95   (501) staff       (20)     1485 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/TextSplitters/token_text_splitter.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.969373 llmflex-0.1.3/src/llmflex/Tools/
--rw-r--r--   0 nathan95   (501) staff       (20)      115 2024-02-24 22:31:02.000000 llmflex-0.1.3/src/llmflex/Tools/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    11795 2024-02-24 22:31:02.000000 llmflex-0.1.3/src/llmflex/Tools/base_tool.py
--rw-r--r--   0 nathan95   (501) staff       (20)     6603 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Tools/tool_selection.py
--rw-r--r--   0 nathan95   (501) staff       (20)    11406 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Tools/web_search_tool.py
--rw-r--r--   0 nathan95   (501) staff       (20)    14418 2024-02-24 22:31:02.000000 llmflex-0.1.3/src/llmflex/Tools/web_search_utils.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.970895 llmflex-0.1.3/src/llmflex/VectorDBs/
--rw-r--r--   0 nathan95   (501) staff       (20)       93 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/VectorDBs/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    23515 2024-04-09 19:26:07.000000 llmflex-0.1.3/src/llmflex/VectorDBs/base_vectordb.py
--rw-r--r--   0 nathan95   (501) staff       (20)     5018 2024-04-09 19:26:07.000000 llmflex-0.1.3/src/llmflex/VectorDBs/faiss_vectordb.py
--rw-r--r--   0 nathan95   (501) staff       (20)      275 2024-04-09 19:26:07.000000 llmflex-0.1.3/src/llmflex/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     4381 2024-02-24 22:31:02.000000 llmflex-0.1.3/src/llmflex/cli.py
--rw-r--r--   0 nathan95   (501) staff       (20)     6178 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/utils.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.971099 llmflex-0.1.3/src/llmflex.egg-info/
--rw-r--r--   0 nathan95   (501) staff       (20)     9750 2024-04-09 19:26:50.000000 llmflex-0.1.3/src/llmflex.egg-info/PKG-INFO
--rw-r--r--   0 nathan95   (501) staff       (20)     1903 2024-04-09 19:26:50.000000 llmflex-0.1.3/src/llmflex.egg-info/SOURCES.txt
--rw-r--r--   0 nathan95   (501) staff       (20)        1 2024-04-09 19:26:50.000000 llmflex-0.1.3/src/llmflex.egg-info/dependency_links.txt
--rw-r--r--   0 nathan95   (501) staff       (20)       44 2024-04-09 19:26:50.000000 llmflex-0.1.3/src/llmflex.egg-info/entry_points.txt
--rw-r--r--   0 nathan95   (501) staff       (20)      323 2024-04-09 19:26:50.000000 llmflex-0.1.3/src/llmflex.egg-info/requires.txt
--rw-r--r--   0 nathan95   (501) staff       (20)        8 2024-04-09 19:26:50.000000 llmflex-0.1.3/src/llmflex.egg-info/top_level.txt
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.553269 llmflex-0.1.4/
+-rw-r--r--   0 nathan95   (501) staff       (20)     1067 2024-01-22 01:35:14.000000 llmflex-0.1.4/LICENSE.md
+-rw-r--r--   0 nathan95   (501) staff       (20)     9757 2024-04-14 12:29:51.553024 llmflex-0.1.4/PKG-INFO
+-rw-r--r--   0 nathan95   (501) staff       (20)     8569 2024-04-09 19:26:07.000000 llmflex-0.1.4/README.md
+-rw-r--r--   0 nathan95   (501) staff       (20)     1203 2024-04-14 12:29:06.000000 llmflex-0.1.4/pyproject.toml
+-rw-r--r--   0 nathan95   (501) staff       (20)       38 2024-04-14 12:29:51.553312 llmflex-0.1.4/setup.cfg
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.543876 llmflex-0.1.4/src/
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.545837 llmflex-0.1.4/src/llmflex/
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.547019 llmflex-0.1.4/src/llmflex/Data/
+-rw-r--r--   0 nathan95   (501) staff       (20)       43 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/Data/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     4919 2024-02-24 22:31:02.000000 llmflex-0.1.4/src/llmflex/Data/sqlite_database.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    20029 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/Data/vector_database.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.547747 llmflex-0.1.4/src/llmflex/Embeddings/
+-rw-r--r--   0 nathan95   (501) staff       (20)      226 2024-02-24 22:31:02.000000 llmflex-0.1.4/src/llmflex/Embeddings/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     4400 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/Embeddings/api_embeddings.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     4245 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/Embeddings/base_embeddings.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     2275 2024-03-15 22:38:26.000000 llmflex-0.1.4/src/llmflex/Embeddings/hf_embeddings_server.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     3998 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/Embeddings/huggingface_embeddings.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.548179 llmflex-0.1.4/src/llmflex/Frontend/
+-rw-r--r--   0 nathan95   (501) staff       (20)      102 2024-02-24 22:31:02.000000 llmflex-0.1.4/src/llmflex/Frontend/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    29992 2024-02-24 22:31:02.000000 llmflex-0.1.4/src/llmflex/Frontend/gradio_interface.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    37412 2024-04-14 12:29:06.000000 llmflex-0.1.4/src/llmflex/Frontend/streamlit_interface.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.548680 llmflex-0.1.4/src/llmflex/Memory/
+-rw-r--r--   0 nathan95   (501) staff       (20)      287 2024-02-24 22:31:02.000000 llmflex-0.1.4/src/llmflex/Memory/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     8298 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/Memory/assistant_long_term_memory.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     8703 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/Memory/base_memory.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     7727 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/Memory/long_short_memory.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.548831 llmflex-0.1.4/src/llmflex/Models/
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.549928 llmflex-0.1.4/src/llmflex/Models/Cores/
+-rw-r--r--   0 nathan95   (501) staff       (20)        0 2024-02-24 22:31:02.000000 llmflex-0.1.4/src/llmflex/Models/Cores/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    14710 2024-04-14 12:29:06.000000 llmflex-0.1.4/src/llmflex/Models/Cores/base_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     7915 2024-02-25 22:17:53.000000 llmflex-0.1.4/src/llmflex/Models/Cores/exllamav2_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     9508 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/Models/Cores/huggingface_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     8610 2024-02-25 22:17:53.000000 llmflex-0.1.4/src/llmflex/Models/Cores/llamacpp_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     9425 2024-04-14 12:29:06.000000 llmflex-0.1.4/src/llmflex/Models/Cores/openai_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     7368 2024-02-28 15:01:21.000000 llmflex-0.1.4/src/llmflex/Models/Cores/utils.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.550168 llmflex-0.1.4/src/llmflex/Models/Factory/
+-rw-r--r--   0 nathan95   (501) staff       (20)        0 2024-02-24 22:31:02.000000 llmflex-0.1.4/src/llmflex/Models/Factory/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    10723 2024-04-14 12:29:06.000000 llmflex-0.1.4/src/llmflex/Models/Factory/llm_factory.py
+-rw-r--r--   0 nathan95   (501) staff       (20)       43 2024-02-24 22:31:02.000000 llmflex-0.1.4/src/llmflex/Models/__init__.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.550433 llmflex-0.1.4/src/llmflex/Prompts/
+-rw-r--r--   0 nathan95   (501) staff       (20)       52 2024-02-24 22:31:02.000000 llmflex-0.1.4/src/llmflex/Prompts/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    14910 2024-04-09 19:26:07.000000 llmflex-0.1.4/src/llmflex/Prompts/prompt_template.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.550681 llmflex-0.1.4/src/llmflex/Schemas/
+-rw-r--r--   0 nathan95   (501) staff       (20)       31 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/Schemas/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)      140 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/Schemas/documents.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.551226 llmflex-0.1.4/src/llmflex/TextSplitters/
+-rw-r--r--   0 nathan95   (501) staff       (20)      123 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/TextSplitters/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     1526 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/TextSplitters/base_text_splitter.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     2709 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/TextSplitters/sentence_token_text_splitter.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     1485 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/TextSplitters/token_text_splitter.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.551822 llmflex-0.1.4/src/llmflex/Tools/
+-rw-r--r--   0 nathan95   (501) staff       (20)      115 2024-02-24 22:31:02.000000 llmflex-0.1.4/src/llmflex/Tools/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    11795 2024-02-24 22:31:02.000000 llmflex-0.1.4/src/llmflex/Tools/base_tool.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     6603 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/Tools/tool_selection.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    11406 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/Tools/web_search_tool.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    14418 2024-02-24 22:31:02.000000 llmflex-0.1.4/src/llmflex/Tools/web_search_utils.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.552226 llmflex-0.1.4/src/llmflex/VectorDBs/
+-rw-r--r--   0 nathan95   (501) staff       (20)       93 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/VectorDBs/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    23515 2024-04-09 19:26:07.000000 llmflex-0.1.4/src/llmflex/VectorDBs/base_vectordb.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     5018 2024-04-09 19:26:07.000000 llmflex-0.1.4/src/llmflex/VectorDBs/faiss_vectordb.py
+-rw-r--r--   0 nathan95   (501) staff       (20)      275 2024-04-14 12:29:06.000000 llmflex-0.1.4/src/llmflex/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     4381 2024-02-24 22:31:02.000000 llmflex-0.1.4/src/llmflex/cli.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     6178 2024-03-11 17:44:28.000000 llmflex-0.1.4/src/llmflex/utils.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-14 12:29:51.552423 llmflex-0.1.4/src/llmflex.egg-info/
+-rw-r--r--   0 nathan95   (501) staff       (20)     9757 2024-04-14 12:29:51.000000 llmflex-0.1.4/src/llmflex.egg-info/PKG-INFO
+-rw-r--r--   0 nathan95   (501) staff       (20)     1903 2024-04-14 12:29:51.000000 llmflex-0.1.4/src/llmflex.egg-info/SOURCES.txt
+-rw-r--r--   0 nathan95   (501) staff       (20)        1 2024-04-14 12:29:51.000000 llmflex-0.1.4/src/llmflex.egg-info/dependency_links.txt
+-rw-r--r--   0 nathan95   (501) staff       (20)       44 2024-04-14 12:29:51.000000 llmflex-0.1.4/src/llmflex.egg-info/entry_points.txt
+-rw-r--r--   0 nathan95   (501) staff       (20)      330 2024-04-14 12:29:51.000000 llmflex-0.1.4/src/llmflex.egg-info/requires.txt
+-rw-r--r--   0 nathan95   (501) staff       (20)        8 2024-04-14 12:29:51.000000 llmflex-0.1.4/src/llmflex.egg-info/top_level.txt
```

### Comparing `llmflex-0.1.3/LICENSE.md` & `llmflex-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.3/PKG-INFO` & `llmflex-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmflex
-Version: 0.1.3
+Version: 0.1.4
 Summary: A python package for developing AI applications with local LLMs.
 Author-email: Nathan Tam <nathan1295@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nath1295/LLMFlex
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -14,15 +14,15 @@
 Requires-Dist: transformers>=4.35.0
 Requires-Dist: accelerate>=0.25.0
 Requires-Dist: sentence-transformers
 Requires-Dist: langchain
 Requires-Dist: faiss-cpu
 Requires-Dist: optimum
 Requires-Dist: gradio>=4.2
-Requires-Dist: duckduckgo-search
+Requires-Dist: duckduckgo-search>=5.2.2
 Requires-Dist: fake-useragent
 Requires-Dist: openai>=1.0.0
 Requires-Dist: tiktoken
 Requires-Dist: protobuf
 Requires-Dist: beautifulsoup4
 Requires-Dist: streamlit
 Requires-Dist: watchdog
```

### Comparing `llmflex-0.1.3/README.md` & `llmflex-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.3/pyproject.toml` & `llmflex-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "transformers>=4.35.0",
     "accelerate>=0.25.0",
     "sentence-transformers",
     "langchain",
     "faiss-cpu",
     "optimum",
     "gradio>=4.2",
-    "duckduckgo-search",
+    "duckduckgo-search>=5.2.2",
     "fake-useragent",
     "openai>=1.0.0",
     "tiktoken",
     "protobuf",
     "beautifulsoup4",
     "streamlit",
     "watchdog",
```

### Comparing `llmflex-0.1.3/src/llmflex/Data/sqlite_database.py` & `llmflex-0.1.4/src/llmflex/Data/sqlite_database.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.3/src/llmflex/Data/vector_database.py` & `llmflex-0.1.4/src/llmflex/Data/vector_database.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.3/src/llmflex/Embeddings/api_embeddings.py` & `llmflex-0.1.4/src/llmflex/Embeddings/api_embeddings.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.3/src/llmflex/Embeddings/base_embeddings.py` & `llmflex-0.1.4/src/llmflex/Embeddings/base_embeddings.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.3/src/llmflex/Embeddings/hf_embeddings_server.py` & `llmflex-0.1.4/src/llmflex/Embeddings/hf_embeddings_server.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.3/src/llmflex/Embeddings/huggingface_embeddings.py` & `llmflex-0.1.4/src/llmflex/Embeddings/huggingface_embeddings.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.3/src/llmflex/Frontend/gradio_interface.py` & `llmflex-0.1.4/src/llmflex/Frontend/gradio_interface.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.3/src/llmflex/Frontend/streamlit_interface.py` & `llmflex-0.1.4/src/llmflex/Frontend/streamlit_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         from ..Prompts.prompt_template import DEFAULT_SYSTEM_MESSAGE
         self.model = model
         self.embeddings = embeddings
         self.text_splitter = SentenceTokenTextSplitter(count_token_fn=model().get_num_tokens, chunk_size=200, chunk_overlap=40)
         self.memory = AssistantLongTermChatMemory(title='Untitled 0', embeddings=self.embeddings, text_splitter=self.text_splitter, from_exist=False)
         self.system = DEFAULT_SYSTEM_MESSAGE
         self.template = self.model.prompt_template
-        self.llm = self.model(stop=self.template.stop + ['#####'])
+        self.llm = self.model(stop=self.template.stop + ['#####'], max_new_tokens=1024)
         self.short_limit = 600
         self.long_limit = 500
         self.score_threshold = 0.5
         self.tool_selector = ToolSelector(tools, model=self.model, embeddings=self.embeddings) if len(tools) > 0 else None
 
     @property
     def titles(self) -> List[str]:
@@ -499,15 +499,15 @@
         """System prompt settings."""
         self.system_text = st.text_area(label='System message', height=250, key='system_msg',label_visibility='collapsed', value=self.backend.system, disabled=self.generating)
         st.markdown(f'System message token count: {self.backend.llm.get_num_tokens(self.backend.system)}')
         st.button(label=':floppy_disk:', key='system_save', disabled=self.generating, use_container_width=True, on_click=self.set_system_message, kwargs=dict(system=self.system_text))
 
     def memory_settings(self) -> None:
         """Memory token limit settings."""
-        self.short_limit_slidder = st.slider('Short term memory token limit', min_value=0, max_value=6000, step=1, value=self.backend.short_limit, disabled=self.generating)
+        self.short_limit_slidder = st.slider('Short term memory token limit', min_value=0, max_value=10000, step=1, value=self.backend.short_limit, disabled=self.generating)
         self.long_limit_slidder = st.slider('Long term memory token limit', min_value=0, max_value=6000, step=1, value=self.backend.long_limit, disabled=self.generating)
         self.score_threshold_slidder = st.slider('Score threshold for long term memory', min_value=0.0, max_value=1.0, step=0.01, value=self.backend.score_threshold, disabled=self.generating)
         summary = [
             'Current settings:',
             f'Short term memory token limit: {self.backend.short_limit}',
             f'Long term memory token limit: {self.backend.long_limit}',
             f'Score threshold: {self.backend.score_threshold}'
```

### Comparing `llmflex-0.1.3/src/llmflex/Memory/assistant_long_term_memory.py` & `llmflex-0.1.4/src/llmflex/Memory/assistant_long_term_memory.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.3/src/llmflex/Memory/base_memory.py` & `llmflex-0.1.4/src/llmflex/Memory/base_memory.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.3/src/llmflex/Memory/long_short_memory.py` & `llmflex-0.1.4/src/llmflex/Memory/long_short_memory.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.3/src/llmflex/Models/Cores/base_core.py` & `llmflex-0.1.4/src/llmflex/Models/Cores/base_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,22 +303,22 @@
 class GenericLLM(BaseLLM):
     """Generic LLM class, using the LLM class from langchain.
     """
     core: BaseCore
     generation_config: Dict[str, Any]
     stop: List[str]
 
-    def __init__(self, core: Type[BaseCore], temperature: float = 0, max_new_tokens: int = 2048, top_p: float = 0.95, top_k: int = 40, 
+    def __init__(self, core: Type[BaseCore], temperature: float = 0, max_new_tokens: int = 256, top_p: float = 0.95, top_k: int = 40, 
                  repetition_penalty: float = 1.1, stop: Optional[List[str]] = None, stop_newline_version: bool = True, **kwargs) -> None:
         """Initialising the LLM.
 
         Args:
             core (Type[BaseCore]): The LLM model core.
             temperature (float, optional): Set how "creative" the model is, the smaller it is, the more static of the output. Defaults to 0.
-            max_new_tokens (int, optional): Maximum number of tokens to generate by the llm. Defaults to 2048.
+            max_new_tokens (int, optional): Maximum number of tokens to generate by the llm. Defaults to 256.
             top_p (float, optional): While sampling the next token, only consider the tokens above this p value. Defaults to 0.95.
             top_k (int, optional): While sampling the next token, only consider the top "top_k" tokens. Defaults to 40.
             repetition_penalty (float, optional): The value to penalise the model for generating repetitive text. Defaults to 1.1.
             stop (Optional[List[str]], optional): List of strings to stop the generation of the llm. Defaults to None.
             stop_newline_version (bool, optional): Whether to add duplicates of the list of stop words starting with a new line character. Defaults to True.
         """
         from .utils import get_stop_words
```

### Comparing `llmflex-0.1.3/src/llmflex/Models/Cores/exllamav2_core.py` & `llmflex-0.1.4/src/llmflex/Models/Cores/exllamav2_core.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.3/src/llmflex/Models/Cores/huggingface_core.py` & `llmflex-0.1.4/src/llmflex/Models/Cores/huggingface_core.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.3/src/llmflex/Models/Cores/llamacpp_core.py` & `llmflex-0.1.4/src/llmflex/Models/Cores/llamacpp_core.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.3/src/llmflex/Models/Cores/openai_core.py` & `llmflex-0.1.4/src/llmflex/Models/Cores/openai_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,19 +156,23 @@
             gen_config['stream'] = True
             def generate():
                 for i in self.model.completions.create(
                     model=self.model_id,
                     prompt=prompt,
                     **gen_config
                 ):
-                    yield i.choices[0].text
+                    if i.choices is None:
+                        yield i.content
+                    else:
+                        yield i.choices[0].text
             return textgen_iterator(generate(), stop=stop)
         else:
             from langchain.llms.utils import enforce_stop_tokens
             gen_config['stream'] = False
             output = self.model.completions.create(
                 model=self.model_id,
                 prompt=prompt,
                 **gen_config
-            ).choices[0].text
+            )
+            output = output.content if output.choices is None else output.choices[0].text
             output = enforce_stop_tokens(output, stop=stop)
             return output
```

### Comparing `llmflex-0.1.3/src/llmflex/Models/Cores/utils.py` & `llmflex-0.1.4/src/llmflex/Models/Cores/utils.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.3/src/llmflex/Models/Factory/llm_factory.py` & `llmflex-0.1.4/src/llmflex/Models/Factory/llm_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,22 +142,22 @@
         """Default prompt template for the model.
 
         Returns:
             PromptTemplate: Default prompt template for the model.
         """
         return self.core.prompt_template
     
-    def __call__(self, temperature: float = 0.8, max_new_tokens: int = 2048, top_p: float = 0.95,
+    def __call__(self, temperature: float = 0.8, max_new_tokens: int = 256, top_p: float = 0.95,
                 top_k: int = 40, repetition_penalty: float = 1.1, stop: Optional[List[str]] = None, 
                 newline=True, **kwargs: Dict[str, Any]) -> BaseLLM:
         """Calling the object will create a langchain format llm with the generation configurations passed from the arguments. 
 
         Args:
             temperature (float, optional): Set how "creative" the model is, the samller it is, the more static of the output. Defaults to 0.8.
-            max_new_tokens (int, optional): Maximum number of tokens to generate by the llm. Defaults to 2048.
+            max_new_tokens (int, optional): Maximum number of tokens to generate by the llm. Defaults to 256.
             top_p (float, optional): While sampling the next token, only consider the tokens above this p value. Defaults to 0.95.
             top_k (int, optional): While sampling the next token, only consider the top "top_k" tokens. Defaults to 40.
             repetition_penalty (float, optional): The value to penalise the model for generating repetitive text. Defaults to 1.1.
             stop (Optional[List[str]], optional): List of strings to stop the generation of the llm. Defaults to None.
             newline (bool, optional): Whether to add a newline character to the beginning of the "stop" list provided. Defaults to True.
 
         Returns:
```

### Comparing `llmflex-0.1.3/src/llmflex/Prompts/prompt_template.py` & `llmflex-0.1.4/src/llmflex/Prompts/prompt_template.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.3/src/llmflex/TextSplitters/base_text_splitter.py` & `llmflex-0.1.4/src/llmflex/TextSplitters/base_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.3/src/llmflex/TextSplitters/sentence_token_text_splitter.py` & `llmflex-0.1.4/src/llmflex/TextSplitters/sentence_token_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.3/src/llmflex/TextSplitters/token_text_splitter.py` & `llmflex-0.1.4/src/llmflex/TextSplitters/token_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.3/src/llmflex/Tools/base_tool.py` & `llmflex-0.1.4/src/llmflex/Tools/base_tool.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.3/src/llmflex/Tools/tool_selection.py` & `llmflex-0.1.4/src/llmflex/Tools/tool_selection.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.3/src/llmflex/Tools/web_search_tool.py` & `llmflex-0.1.4/src/llmflex/Tools/web_search_tool.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.3/src/llmflex/Tools/web_search_utils.py` & `llmflex-0.1.4/src/llmflex/Tools/web_search_utils.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.3/src/llmflex/VectorDBs/base_vectordb.py` & `llmflex-0.1.4/src/llmflex/VectorDBs/base_vectordb.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.3/src/llmflex/VectorDBs/faiss_vectordb.py` & `llmflex-0.1.4/src/llmflex/VectorDBs/faiss_vectordb.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.3/src/llmflex/cli.py` & `llmflex-0.1.4/src/llmflex/cli.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.3/src/llmflex/utils.py` & `llmflex-0.1.4/src/llmflex/utils.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.3/src/llmflex.egg-info/PKG-INFO` & `llmflex-0.1.4/src/llmflex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmflex
-Version: 0.1.3
+Version: 0.1.4
 Summary: A python package for developing AI applications with local LLMs.
 Author-email: Nathan Tam <nathan1295@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nath1295/LLMFlex
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -14,15 +14,15 @@
 Requires-Dist: transformers>=4.35.0
 Requires-Dist: accelerate>=0.25.0
 Requires-Dist: sentence-transformers
 Requires-Dist: langchain
 Requires-Dist: faiss-cpu
 Requires-Dist: optimum
 Requires-Dist: gradio>=4.2
-Requires-Dist: duckduckgo-search
+Requires-Dist: duckduckgo-search>=5.2.2
 Requires-Dist: fake-useragent
 Requires-Dist: openai>=1.0.0
 Requires-Dist: tiktoken
 Requires-Dist: protobuf
 Requires-Dist: beautifulsoup4
 Requires-Dist: streamlit
 Requires-Dist: watchdog
```

### Comparing `llmflex-0.1.3/src/llmflex.egg-info/SOURCES.txt` & `llmflex-0.1.4/src/llmflex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

