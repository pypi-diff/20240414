# Comparing `tmp/llamabot-0.4.3.tar.gz` & `tmp/llamabot-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamabot-0.4.3.tar", last modified: Fri Apr 12 20:28:54 2024, max compression
+gzip compressed data, was "llamabot-0.4.4.tar", last modified: Sat Apr 13 21:58:50 2024, max compression
```

## Comparing `llamabot-0.4.3.tar` & `llamabot-0.4.4.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:54.545241 llamabot-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-12 20:21:30.000000 llamabot-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13519 2024-04-12 20:28:54.545241 llamabot-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12212 2024-04-12 20:21:30.000000 llamabot-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:54.533242 llamabot-0.4.3/llamabot/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:54.537242 llamabot-0.4.3/llamabot/bot/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/bot/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/bot/imagebot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/bot/kgbot.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/bot/model_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-12 20:28:47.000000 llamabot-0.4.3/llamabot/bot/ollama_model_names.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/bot/qabot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/bot/querybot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/bot/simplebot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:54.537242 llamabot-0.4.3/llamabot/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/cli/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/cli/blog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/cli/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/cli/doc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/cli/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/cli/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/cli/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/cli/serve.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/cli/tutorial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/cli/zotero.py
--rw-r--r--   0 runner    (1001) docker     (127)    14939 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/code_manipulation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:54.541242 llamabot-0.4.3/llamabot/components/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/components/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/components/chatui.py
--rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/components/docstore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/components/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/components/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/components/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/doc_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/file_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:54.541242 llamabot-0.4.3/llamabot/prompt_library/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/prompt_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/prompt_library/blog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/prompt_library/diffbot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/prompt_library/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/prompt_library/output_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/prompt_library/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/prompt_library/sembr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/prompt_library/tutorial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/prompt_library/zotero.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/prompt_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/recorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-12 20:21:36.000000 llamabot-0.4.3/llamabot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:54.541242 llamabot-0.4.3/llamabot/zotero/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/zotero/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/zotero/completer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6042 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/zotero/library.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-12 20:21:30.000000 llamabot-0.4.3/llamabot/zotero/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:54.541242 llamabot-0.4.3/llamabot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13519 2024-04-12 20:28:54.000000 llamabot-0.4.3/llamabot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-12 20:28:54.000000 llamabot-0.4.3/llamabot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 20:28:54.000000 llamabot-0.4.3/llamabot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-12 20:28:54.000000 llamabot-0.4.3/llamabot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-12 20:28:54.000000 llamabot-0.4.3/llamabot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 20:28:54.000000 llamabot-0.4.3/llamabot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-12 20:21:36.000000 llamabot-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 20:28:54.545241 llamabot-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:54.541242 llamabot-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-12 20:21:30.000000 llamabot-0.4.3/tests/test_bot.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-12 20:21:30.000000 llamabot-0.4.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-04-12 20:21:30.000000 llamabot-0.4.3/tests/test_code_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-04-12 20:21:30.000000 llamabot-0.4.3/tests/test_doc_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-12 20:21:30.000000 llamabot-0.4.3/tests/test_file_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-12 20:21:30.000000 llamabot-0.4.3/tests/test_prompt_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-12 20:21:30.000000 llamabot-0.4.3/tests/test_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:58:50.203441 llamabot-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-13 21:55:15.000000 llamabot-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13519 2024-04-13 21:58:50.203441 llamabot-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12212 2024-04-13 21:55:15.000000 llamabot-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:58:50.191441 llamabot-0.4.4/llamabot/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:58:50.195441 llamabot-0.4.4/llamabot/bot/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/bot/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/bot/imagebot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/bot/kgbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/bot/model_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-13 21:58:43.000000 llamabot-0.4.4/llamabot/bot/ollama_model_names.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/bot/qabot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/bot/querybot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/bot/simplebot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:58:50.195441 llamabot-0.4.4/llamabot/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/cli/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/cli/blog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/cli/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/cli/doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/cli/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/cli/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/cli/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/cli/serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/cli/tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/cli/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14939 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/code_manipulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:58:50.199441 llamabot-0.4.4/llamabot/components/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/components/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/components/chatui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/components/docstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/components/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/components/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/components/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/doc_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/file_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:58:50.199441 llamabot-0.4.4/llamabot/prompt_library/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/prompt_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/prompt_library/blog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/prompt_library/diffbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/prompt_library/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/prompt_library/output_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/prompt_library/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/prompt_library/sembr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/prompt_library/tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/prompt_library/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/prompt_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-13 21:55:18.000000 llamabot-0.4.4/llamabot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:58:50.199441 llamabot-0.4.4/llamabot/zotero/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/zotero/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/zotero/completer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6042 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/zotero/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-13 21:55:15.000000 llamabot-0.4.4/llamabot/zotero/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:58:50.199441 llamabot-0.4.4/llamabot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13519 2024-04-13 21:58:50.000000 llamabot-0.4.4/llamabot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-13 21:58:50.000000 llamabot-0.4.4/llamabot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 21:58:50.000000 llamabot-0.4.4/llamabot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-13 21:58:50.000000 llamabot-0.4.4/llamabot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-13 21:58:50.000000 llamabot-0.4.4/llamabot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 21:58:50.000000 llamabot-0.4.4/llamabot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-13 21:55:18.000000 llamabot-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 21:58:50.203441 llamabot-0.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:58:50.199441 llamabot-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-13 21:55:15.000000 llamabot-0.4.4/tests/test_bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-13 21:55:15.000000 llamabot-0.4.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-04-13 21:55:15.000000 llamabot-0.4.4/tests/test_code_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-04-13 21:55:15.000000 llamabot-0.4.4/tests/test_doc_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-13 21:55:15.000000 llamabot-0.4.4/tests/test_file_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-13 21:55:15.000000 llamabot-0.4.4/tests/test_prompt_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-13 21:55:15.000000 llamabot-0.4.4/tests/test_recorder.py
```

### Comparing `llamabot-0.4.3/PKG-INFO` & `llamabot-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: llamabot
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Pythonic interface to LLMs.
 Requires-Python: >3.10
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 Requires-Dist: panel>=1.3.0
 Requires-Dist: jupyter_bokeh
 Requires-Dist: bokeh>=3.1.0
 Requires-Dist: loguru
 Requires-Dist: pyperclip
 Requires-Dist: astor>=0.8.1
 Requires-Dist: python-dotenv
-Requires-Dist: typer>=0.4.3
+Requires-Dist: typer>=0.4.4
 Requires-Dist: gitpython
 Requires-Dist: pyprojroot
 Requires-Dist: frozenlist
 Requires-Dist: beautifulsoup4
 Requires-Dist: rich
 Requires-Dist: pyzotero
 Requires-Dist: case-converter
```

### Comparing `llamabot-0.4.3/README.md` & `llamabot-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/bot/chatbot.py` & `llamabot-0.4.4/llamabot/bot/chatbot.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/bot/imagebot.py` & `llamabot-0.4.4/llamabot/bot/imagebot.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/bot/kgbot.py` & `llamabot-0.4.4/llamabot/bot/kgbot.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/bot/model_tokens.py` & `llamabot-0.4.4/llamabot/bot/model_tokens.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/bot/ollama_model_names.txt` & `llamabot-0.4.4/llamabot/bot/ollama_model_names.txt`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/bot/qabot.py` & `llamabot-0.4.4/llamabot/bot/qabot.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/bot/querybot.py` & `llamabot-0.4.4/llamabot/bot/querybot.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/bot/simplebot.py` & `llamabot-0.4.4/llamabot/bot/simplebot.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/cli/__init__.py` & `llamabot-0.4.4/llamabot/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/cli/apps.py` & `llamabot-0.4.4/llamabot/cli/apps.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/cli/blog.py` & `llamabot-0.4.4/llamabot/cli/blog.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/cli/configure.py` & `llamabot-0.4.4/llamabot/cli/configure.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/cli/doc.py` & `llamabot-0.4.4/llamabot/cli/doc.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,21 +16,25 @@
         "mistral/mistral-medium", help="Name of the LLM to use."
     ),
     initial_message: str = typer.Option(..., help="Initial message for the bot."),
     panel: bool = typer.Option(True, help="Whether to use Panel or not."),
     doc_path: Path = typer.Argument(
         "", help="Path to the document you wish to chat with."
     ),
+    address: str = typer.Option("0.0.0.0", help="Host to serve the API on."),
+    port: int = typer.Option(6363, help="Port to serve the API on."),
 ):
     """Chat with your document.
 
     :param model_name: Name of the LLM to use.
     :param panel: Whether to use Panel or not. If not, we default to using CLI chat.
     :param initial_message: The initial message to send to the user.
     :param doc_path: Path to the document you wish to chat with.
+    :param address: Host to serve the API on.
+    :param port: Port to serve the API on.
     """
     stream_target = "stdout"
     if panel:
         stream_target = "panel"
 
     bot = QueryBot(
         system_prompt=(
@@ -50,15 +54,15 @@
             "Ask me anything! "
             "Otherwise, type 'exit' or 'quit' at anytime to exit."
         )
     )
 
     if panel:
         print("Serving your document in a panel...")
-        bot.serve()
+        bot.serve(address=address, port=port, websocket_origin=["*"])
 
     else:
         while True:
             query = uniform_prompt()
             exit_if_asked(query)
             bot(query)
             typer.echo("\n\n")
```

### Comparing `llamabot-0.4.3/llamabot/cli/git.py` & `llamabot-0.4.4/llamabot/cli/git.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/cli/python.py` & `llamabot-0.4.4/llamabot/cli/python.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/cli/repo.py` & `llamabot-0.4.4/llamabot/cli/repo.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/cli/serve.py` & `llamabot-0.4.4/llamabot/cli/serve.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/cli/tutorial.py` & `llamabot-0.4.4/llamabot/cli/tutorial.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/cli/utils.py` & `llamabot-0.4.4/llamabot/cli/utils.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/cli/zotero.py` & `llamabot-0.4.4/llamabot/cli/zotero.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/code_manipulation.py` & `llamabot-0.4.4/llamabot/code_manipulation.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/components/api.py` & `llamabot-0.4.4/llamabot/components/api.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/components/chatui.py` & `llamabot-0.4.4/llamabot/components/chatui.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,13 +26,13 @@
     def servable(self):
         """Return the chat interface as a Panel servable object.
 
         :returns: The chat interface as a Panel servable object.
         """
         return self.chat_interface.servable()
 
-    def serve(self):
+    def serve(self, **kwargs):
         """Serve the chat interface.
 
         :returns: None
         """
-        self.chat_interface.show()
+        self.chat_interface.show(**kwargs)
```

### Comparing `llamabot-0.4.3/llamabot/components/docstore.py` & `llamabot-0.4.4/llamabot/components/docstore.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/components/history.py` & `llamabot-0.4.4/llamabot/components/history.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/components/messages.py` & `llamabot-0.4.4/llamabot/components/messages.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/components/tools.py` & `llamabot-0.4.4/llamabot/components/tools.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/doc_processor.py` & `llamabot-0.4.4/llamabot/doc_processor.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/dummy.py` & `llamabot-0.4.4/llamabot/dummy.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/file_finder.py` & `llamabot-0.4.4/llamabot/file_finder.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/prompt_library/blog.py` & `llamabot-0.4.4/llamabot/prompt_library/blog.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/prompt_library/diffbot.py` & `llamabot-0.4.4/llamabot/prompt_library/diffbot.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/prompt_library/git.py` & `llamabot-0.4.4/llamabot/prompt_library/git.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/prompt_library/output_formatter.py` & `llamabot-0.4.4/llamabot/prompt_library/output_formatter.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/prompt_library/python.py` & `llamabot-0.4.4/llamabot/prompt_library/python.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/prompt_library/sembr.py` & `llamabot-0.4.4/llamabot/prompt_library/sembr.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/prompt_library/tutorial.py` & `llamabot-0.4.4/llamabot/prompt_library/tutorial.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/prompt_library/zotero.py` & `llamabot-0.4.4/llamabot/prompt_library/zotero.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/prompt_manager.py` & `llamabot-0.4.4/llamabot/prompt_manager.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/recorder.py` & `llamabot-0.4.4/llamabot/recorder.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/zotero/completer.py` & `llamabot-0.4.4/llamabot/zotero/completer.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot/zotero/library.py` & `llamabot-0.4.4/llamabot/zotero/library.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/llamabot.egg-info/PKG-INFO` & `llamabot-0.4.4/llamabot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: llamabot
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Pythonic interface to LLMs.
 Requires-Python: >3.10
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 Requires-Dist: panel>=1.3.0
 Requires-Dist: jupyter_bokeh
 Requires-Dist: bokeh>=3.1.0
 Requires-Dist: loguru
 Requires-Dist: pyperclip
 Requires-Dist: astor>=0.8.1
 Requires-Dist: python-dotenv
-Requires-Dist: typer>=0.4.3
+Requires-Dist: typer>=0.4.4
 Requires-Dist: gitpython
 Requires-Dist: pyprojroot
 Requires-Dist: frozenlist
 Requires-Dist: beautifulsoup4
 Requires-Dist: rich
 Requires-Dist: pyzotero
 Requires-Dist: case-converter
```

### Comparing `llamabot-0.4.3/llamabot.egg-info/SOURCES.txt` & `llamabot-0.4.4/llamabot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/pyproject.toml` & `llamabot-0.4.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -58,25 +58,25 @@
 
 [tool.setuptools.packages.find]
 where = ["."]
 namespaces = false
 
 [project]
 name = "llamabot"
-version = "0.4.3"
+version = "0.4.4"
 dependencies = [
     "openai",
     "panel>=1.3.0",
     "jupyter_bokeh",
     "bokeh>=3.1.0",
     "loguru",
     "pyperclip",
     "astor>=0.8.1",
     "python-dotenv",
-    "typer>=0.4.3",
+    "typer>=0.4.4",
     "gitpython",
     "pyprojroot",
     "frozenlist",
     "beautifulsoup4",
     "rich",
     "pyzotero",
     "case-converter",
```

### Comparing `llamabot-0.4.3/tests/test_code_manipulation.py` & `llamabot-0.4.4/tests/test_code_manipulation.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/tests/test_doc_processor.py` & `llamabot-0.4.4/tests/test_doc_processor.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/tests/test_file_finder.py` & `llamabot-0.4.4/tests/test_file_finder.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/tests/test_prompt_manager.py` & `llamabot-0.4.4/tests/test_prompt_manager.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.3/tests/test_recorder.py` & `llamabot-0.4.4/tests/test_recorder.py`

 * *Files identical despite different names*

