# Comparing `tmp/AutoRAG-0.1.2.tar.gz` & `tmp/autorag-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoRAG-0.1.2.tar", last modified: Wed Apr 10 04:46:25 2024, max compression
+gzip compressed data, was "autorag-0.1.3.tar", last modified: Sun Apr 14 04:50:14 2024, max compression
```

## Comparing `AutoRAG-0.1.2.tar` & `autorag-0.1.3.tar`

### file list

```diff
@@ -1,456 +1,490 @@
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.222951 AutoRAG-0.1.2/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.066325 AutoRAG-0.1.2/.github/
--rw-r--r--   0 jeffrey    (501) staff       (20)      501 2024-01-13 07:55:28.000000 AutoRAG-0.1.2/.github/dependabot.yml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.066797 AutoRAG-0.1.2/.github/workflows/
--rw-r--r--   0 jeffrey    (501) staff       (20)      818 2024-03-25 06:37:01.000000 AutoRAG-0.1.2/.github/workflows/sphinx.yml
--rw-r--r--   0 jeffrey    (501) staff       (20)      862 2024-04-06 14:23:40.000000 AutoRAG-0.1.2/.github/workflows/test.yml
--rw-r--r--   0 jeffrey    (501) staff       (20)     3088 2024-01-13 07:55:28.000000 AutoRAG-0.1.2/.gitignore
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.222156 AutoRAG-0.1.2/AutoRAG.egg-info/
--rw-r--r--   0 jeffrey    (501) staff       (20)    33191 2024-04-10 04:46:24.000000 AutoRAG-0.1.2/AutoRAG.egg-info/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)    17176 2024-04-10 04:46:25.000000 AutoRAG-0.1.2/AutoRAG.egg-info/SOURCES.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        1 2024-04-10 04:46:24.000000 AutoRAG-0.1.2/AutoRAG.egg-info/dependency_links.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       44 2024-04-10 04:46:24.000000 AutoRAG-0.1.2/AutoRAG.egg-info/entry_points.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      506 2024-04-10 04:46:24.000000 AutoRAG-0.1.2/AutoRAG.egg-info/requires.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        8 2024-04-10 04:46:24.000000 AutoRAG-0.1.2/AutoRAG.egg-info/top_level.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)    11357 2024-01-13 07:55:28.000000 AutoRAG-0.1.2/LICENSE
--rw-r--r--   0 jeffrey    (501) staff       (20)    33191 2024-04-10 04:46:25.222672 AutoRAG-0.1.2/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)    18212 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/README.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.069927 AutoRAG-0.1.2/autorag/
--rw-r--r--   0 jeffrey    (501) staff       (20)        5 2024-04-10 04:41:48.000000 AutoRAG-0.1.2/autorag/VERSION
--rw-r--r--   0 jeffrey    (501) staff       (20)     2686 2024-03-27 16:56:49.000000 AutoRAG-0.1.2/autorag/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4333 2024-03-29 05:05:10.000000 AutoRAG-0.1.2/autorag/cli.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.070195 AutoRAG-0.1.2/autorag/data/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-04-01 09:28:42.000000 AutoRAG-0.1.2/autorag/data/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.070793 AutoRAG-0.1.2/autorag/data/corpus/
--rw-r--r--   0 jeffrey    (501) staff       (20)      134 2024-03-22 04:27:08.000000 AutoRAG-0.1.2/autorag/data/corpus/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1625 2024-03-22 05:41:56.000000 AutoRAG-0.1.2/autorag/data/corpus/langchain.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2834 2024-03-22 04:27:08.000000 AutoRAG-0.1.2/autorag/data/corpus/llama_index.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.072358 AutoRAG-0.1.2/autorag/data/qacreation/
--rw-r--r--   0 jeffrey    (501) staff       (20)      124 2024-03-25 11:47:15.000000 AutoRAG-0.1.2/autorag/data/qacreation/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2754 2024-03-25 11:47:15.000000 AutoRAG-0.1.2/autorag/data/qacreation/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     7107 2024-03-23 03:44:06.000000 AutoRAG-0.1.2/autorag/data/qacreation/llama_index.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3190 2024-03-23 03:44:06.000000 AutoRAG-0.1.2/autorag/data/qacreation/llama_index_default_prompt.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     3289 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/data/qacreation/simple.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.072747 AutoRAG-0.1.2/autorag/data/utils/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/data/utils/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1050 2024-03-22 04:01:20.000000 AutoRAG-0.1.2/autorag/data/utils/util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     8871 2024-03-06 00:03:36.000000 AutoRAG-0.1.2/autorag/deploy.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.084665 AutoRAG-0.1.2/autorag/evaluate/
--rw-r--r--   0 jeffrey    (501) staff       (20)      146 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/evaluate/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2603 2024-04-05 14:53:42.000000 AutoRAG-0.1.2/autorag/evaluate/generation.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.086067 AutoRAG-0.1.2/autorag/evaluate/metric/
--rw-r--r--   0 jeffrey    (501) staff       (20)      252 2024-04-05 14:53:42.000000 AutoRAG-0.1.2/autorag/evaluate/metric/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.087055 AutoRAG-0.1.2/autorag/evaluate/metric/g_eval_prompts/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1186 2024-02-23 11:07:36.000000 AutoRAG-0.1.2/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     1015 2024-02-23 11:07:40.000000 AutoRAG-0.1.2/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      814 2024-02-23 11:07:43.000000 AutoRAG-0.1.2/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     1005 2024-02-23 11:07:46.000000 AutoRAG-0.1.2/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)    11906 2024-04-05 14:53:42.000000 AutoRAG-0.1.2/autorag/evaluate/metric/generation.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1477 2024-02-23 18:16:58.000000 AutoRAG-0.1.2/autorag/evaluate/metric/retrieval.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2131 2024-02-23 18:16:58.000000 AutoRAG-0.1.2/autorag/evaluate/metric/retrieval_contents.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      224 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/evaluate/metric/util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2052 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/evaluate/retrieval.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2099 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/evaluate/retrieval_contents.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1290 2024-02-18 20:58:37.000000 AutoRAG-0.1.2/autorag/evaluate/util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    16846 2024-03-30 16:07:43.000000 AutoRAG-0.1.2/autorag/evaluator.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2248 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/node_line.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.087185 AutoRAG-0.1.2/autorag/nodes/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/nodes/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.088240 AutoRAG-0.1.2/autorag/nodes/generator/
--rw-r--r--   0 jeffrey    (501) staff       (20)       68 2024-03-07 23:12:39.000000 AutoRAG-0.1.2/autorag/nodes/generator/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2215 2024-03-07 22:31:53.000000 AutoRAG-0.1.2/autorag/nodes/generator/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1641 2024-03-30 16:26:48.000000 AutoRAG-0.1.2/autorag/nodes/generator/llama_index_llm.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4532 2024-03-31 04:56:43.000000 AutoRAG-0.1.2/autorag/nodes/generator/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2810 2024-03-08 18:01:40.000000 AutoRAG-0.1.2/autorag/nodes/generator/vllm.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.089279 AutoRAG-0.1.2/autorag/nodes/passagecompressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)       88 2024-02-22 15:32:30.000000 AutoRAG-0.1.2/autorag/nodes/passagecompressor/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2433 2024-03-06 19:11:31.000000 AutoRAG-0.1.2/autorag/nodes/passagecompressor/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      242 2024-02-22 15:32:30.000000 AutoRAG-0.1.2/autorag/nodes/passagecompressor/pass_compressor.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6075 2024-02-15 17:28:32.000000 AutoRAG-0.1.2/autorag/nodes/passagecompressor/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3028 2024-02-14 10:09:21.000000 AutoRAG-0.1.2/autorag/nodes/passagecompressor/tree_summarize.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.095164 AutoRAG-0.1.2/autorag/nodes/passagereranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)      403 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1664 2024-04-05 03:16:26.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3979 2024-03-17 04:13:16.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/cohere.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3625 2024-04-08 12:04:54.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/colbert.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3534 2024-04-10 04:41:53.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/flag_embedding.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3713 2024-04-06 14:23:40.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/jina.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4186 2024-03-06 19:44:35.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/koreranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6838 2024-03-06 19:44:35.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/monot5.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      618 2024-02-22 15:32:30.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/pass_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4712 2024-04-05 03:16:26.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/rankgpt.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4105 2024-04-10 04:41:35.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3889 2024-04-08 08:26:20.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/sentence_transformer.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.096018 AutoRAG-0.1.2/autorag/nodes/passagereranker/tart/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/tart/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4983 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/tart/modeling_enc_t5.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4452 2024-03-06 19:44:35.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/tart/tart.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4201 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     7555 2024-03-06 19:44:35.000000 AutoRAG-0.1.2/autorag/nodes/passagereranker/upr.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.097502 AutoRAG-0.1.2/autorag/nodes/promptmaker/
--rw-r--r--   0 jeffrey    (501) staff       (20)       84 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/autorag/nodes/promptmaker/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1379 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/autorag/nodes/promptmaker/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1162 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/nodes/promptmaker/fstring.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2290 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/autorag/nodes/promptmaker/long_context_reorder.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     8925 2024-03-31 10:20:41.000000 AutoRAG-0.1.2/autorag/nodes/promptmaker/run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.098976 AutoRAG-0.1.2/autorag/nodes/queryexpansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)      123 2024-02-22 15:32:30.000000 AutoRAG-0.1.2/autorag/nodes/queryexpansion/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1663 2024-03-06 19:11:31.000000 AutoRAG-0.1.2/autorag/nodes/queryexpansion/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1572 2024-02-14 10:09:21.000000 AutoRAG-0.1.2/autorag/nodes/queryexpansion/hyde.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      368 2024-02-22 15:32:30.000000 AutoRAG-0.1.2/autorag/nodes/queryexpansion/pass_query_expansion.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3491 2024-02-14 10:09:21.000000 AutoRAG-0.1.2/autorag/nodes/queryexpansion/query_decompose.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     7932 2024-02-15 17:29:26.000000 AutoRAG-0.1.2/autorag/nodes/queryexpansion/run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.100657 AutoRAG-0.1.2/autorag/nodes/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)      155 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/nodes/retrieval/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6415 2024-03-08 17:59:53.000000 AutoRAG-0.1.2/autorag/nodes/retrieval/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5637 2024-03-25 04:14:52.000000 AutoRAG-0.1.2/autorag/nodes/retrieval/bm25.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3122 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/nodes/retrieval/hybrid_cc.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2957 2024-02-13 22:39:30.000000 AutoRAG-0.1.2/autorag/nodes/retrieval/hybrid_rrf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    10751 2024-02-15 17:27:26.000000 AutoRAG-0.1.2/autorag/nodes/retrieval/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4651 2024-03-25 07:44:05.000000 AutoRAG-0.1.2/autorag/nodes/retrieval/vectordb.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.101238 AutoRAG-0.1.2/autorag/schema/
--rw-r--r--   0 jeffrey    (501) staff       (20)       50 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/schema/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      722 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/schema/module.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4158 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/schema/node.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3996 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/strategy.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3102 2024-04-10 04:41:35.000000 AutoRAG-0.1.2/autorag/support.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.101723 AutoRAG-0.1.2/autorag/utils/
--rw-r--r--   0 jeffrey    (501) staff       (20)      161 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/utils/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2611 2024-02-13 20:12:31.000000 AutoRAG-0.1.2/autorag/utils/preprocess.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     9447 2024-04-10 04:41:35.000000 AutoRAG-0.1.2/autorag/utils/util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2563 2024-03-06 00:03:36.000000 AutoRAG-0.1.2/autorag/web.py
--rw-r--r--   0 jeffrey    (501) staff       (20)       58 2024-02-18 10:18:03.000000 AutoRAG-0.1.2/dev_requirements.txt
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.102306 AutoRAG-0.1.2/docs/
--rw-r--r--   0 jeffrey    (501) staff       (20)      638 2024-01-17 16:38:11.000000 AutoRAG-0.1.2/docs/Makefile
--rw-r--r--   0 jeffrey    (501) staff       (20)      804 2024-01-17 11:55:21.000000 AutoRAG-0.1.2/docs/make.bat
--rw-r--r--   0 jeffrey    (501) staff       (20)      110 2024-03-30 16:07:43.000000 AutoRAG-0.1.2/docs/requirements.txt
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.104117 AutoRAG-0.1.2/docs/source/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.112793 AutoRAG-0.1.2/docs/source/_static/
--rw-r--r--   0 jeffrey    (501) staff       (20)    57124 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/_static/data_creation.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    30770 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/_static/data_folder.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    31538 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/_static/node_folder.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    18941 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/_static/node_line_folder.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    42589 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/_static/node_line_summary.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    92939 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/_static/node_lines.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    95669 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/_static/node_summary.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    36728 2024-02-07 10:54:42.000000 AutoRAG-0.1.2/docs/source/_static/project_folder_example.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    19853 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/_static/project_folders.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    22432 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/_static/resources_folder.png
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.117002 AutoRAG-0.1.2/docs/source/_static/roadmap/
--rw-r--r--   0 jeffrey    (501) staff       (20)   159068 2024-02-07 21:45:07.000000 AutoRAG-0.1.2/docs/source/_static/roadmap/RAG_paradigms.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    38568 2024-02-07 21:45:07.000000 AutoRAG-0.1.2/docs/source/_static/roadmap/advanced_RAG.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    62853 2024-02-07 21:45:07.000000 AutoRAG-0.1.2/docs/source/_static/roadmap/cycle.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    75826 2024-02-07 21:45:07.000000 AutoRAG-0.1.2/docs/source/_static/roadmap/merger.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    82200 2024-02-07 21:45:07.000000 AutoRAG-0.1.2/docs/source/_static/roadmap/node_line_modular.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    69999 2024-02-07 21:45:07.000000 AutoRAG-0.1.2/docs/source/_static/roadmap/policy.png
--rw-r--r--   0 jeffrey    (501) staff       (20)   567356 2024-02-07 10:54:42.000000 AutoRAG-0.1.2/docs/source/_static/samsung_sundae.jpeg
--rw-r--r--   0 jeffrey    (501) staff       (20)    37348 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/_static/trial_folder.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    25499 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/_static/trial_json.png
--rw-r--r--   0 jeffrey    (501) staff       (20)   177107 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/_static/trial_summary.png
--rw-r--r--   0 jeffrey    (501) staff       (20)   269046 2024-03-06 00:03:36.000000 AutoRAG-0.1.2/docs/source/_static/web_interface.png
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.124928 AutoRAG-0.1.2/docs/source/api_spec/
--rw-r--r--   0 jeffrey    (501) staff       (20)      563 2024-03-22 04:34:21.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.data.corpus.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      763 2024-03-26 06:03:31.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.data.qacreation.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      287 2024-03-22 04:34:21.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.data.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      358 2024-03-22 04:34:21.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.data.utils.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      984 2024-02-10 14:23:30.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.evaluate.metric.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      962 2024-02-10 14:23:30.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.evaluate.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      941 2024-03-17 04:13:16.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.generator.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1091 2024-02-22 15:32:30.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.passagecompressor.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     2772 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.passagereranker.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      952 2024-02-01 16:32:39.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      995 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.promptmaker.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1254 2024-02-22 15:32:30.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.queryexpansion.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1299 2024-02-03 13:50:08.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.retrieval.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      401 2024-01-17 15:59:52.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1239 2024-03-07 15:58:42.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      486 2024-01-17 15:59:52.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.schema.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      489 2024-01-17 15:59:52.000000 AutoRAG-0.1.2/docs/source/api_spec/autorag.utils.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)       58 2024-01-17 15:59:52.000000 AutoRAG-0.1.2/docs/source/api_spec/modules.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1371 2024-03-30 16:07:43.000000 AutoRAG-0.1.2/docs/source/conf.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.125380 AutoRAG-0.1.2/docs/source/data_creation/
--rw-r--r--   0 jeffrey    (501) staff       (20)     5072 2024-02-18 20:58:37.000000 AutoRAG-0.1.2/docs/source/data_creation/data_format.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     5543 2024-03-25 11:47:15.000000 AutoRAG-0.1.2/docs/source/data_creation/tutorial.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.125872 AutoRAG-0.1.2/docs/source/deploy/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1473 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/deploy/api_endpoint.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      912 2024-03-06 00:03:36.000000 AutoRAG-0.1.2/docs/source/deploy/web.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     4056 2024-03-06 00:03:36.000000 AutoRAG-0.1.2/docs/source/index.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1891 2024-02-15 09:50:25.000000 AutoRAG-0.1.2/docs/source/install.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     6083 2024-02-18 20:58:37.000000 AutoRAG-0.1.2/docs/source/local_model.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.126091 AutoRAG-0.1.2/docs/source/nodes/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.126803 AutoRAG-0.1.2/docs/source/nodes/generator/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2703 2024-04-05 14:53:42.000000 AutoRAG-0.1.2/docs/source/nodes/generator/generator.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1306 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/nodes/generator/llama_index_llm.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1358 2024-03-14 09:00:38.000000 AutoRAG-0.1.2/docs/source/nodes/generator/vllm.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     5062 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/docs/source/nodes/index.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.127235 AutoRAG-0.1.2/docs/source/nodes/passage_compressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3036 2024-02-22 15:32:30.000000 AutoRAG-0.1.2/docs/source/nodes/passage_compressor/passage_compressor.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1252 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/nodes/passage_compressor/tree_summarize.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.129717 AutoRAG-0.1.2/docs/source/nodes/passage_reranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1151 2024-03-17 04:13:16.000000 AutoRAG-0.1.2/docs/source/nodes/passage_reranker/cohere.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      521 2024-04-08 12:04:54.000000 AutoRAG-0.1.2/docs/source/nodes/passage_reranker/colbert.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      647 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/docs/source/nodes/passage_reranker/flag_embedding_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1232 2024-04-06 14:23:40.000000 AutoRAG-0.1.2/docs/source/nodes/passage_reranker/jina_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      366 2024-02-22 16:33:58.000000 AutoRAG-0.1.2/docs/source/nodes/passage_reranker/koreranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1567 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/nodes/passage_reranker/monot5.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2324 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/docs/source/nodes/passage_reranker/passage_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1063 2024-04-05 03:16:26.000000 AutoRAG-0.1.2/docs/source/nodes/passage_reranker/rankgpt.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      645 2024-04-08 08:26:20.000000 AutoRAG-0.1.2/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      515 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/nodes/passage_reranker/tart.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1435 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/nodes/passage_reranker/upr.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.130600 AutoRAG-0.1.2/docs/source/nodes/prompt_maker/
--rw-r--r--   0 jeffrey    (501) staff       (20)      585 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/nodes/prompt_maker/fstring.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      815 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/docs/source/nodes/prompt_maker/long_context_reorder.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2689 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/docs/source/nodes/prompt_maker/prompt_maker.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.131184 AutoRAG-0.1.2/docs/source/nodes/query_expansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1178 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/nodes/query_expansion/hyde.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1330 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/nodes/query_expansion/query_decompose.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     3272 2024-02-22 15:32:30.000000 AutoRAG-0.1.2/docs/source/nodes/query_expansion/query_expansion.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.132161 AutoRAG-0.1.2/docs/source/nodes/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)      625 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/nodes/retrieval/bm25.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2236 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/nodes/retrieval/hybrid_cc.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2073 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/nodes/retrieval/hybrid_rrf.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1881 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/nodes/retrieval/retrieval.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1223 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/nodes/retrieval/vectordb.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.133116 AutoRAG-0.1.2/docs/source/optimization/
--rw-r--r--   0 jeffrey    (501) staff       (20)     4160 2024-02-15 10:23:20.000000 AutoRAG-0.1.2/docs/source/optimization/custom_config.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     3779 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/optimization/folder_structure.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     4596 2024-02-07 21:46:19.000000 AutoRAG-0.1.2/docs/source/optimization/optimization.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2580 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/optimization/sample_full_config.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.133288 AutoRAG-0.1.2/docs/source/roadmap/
--rw-r--r--   0 jeffrey    (501) staff       (20)     6735 2024-02-07 21:45:07.000000 AutoRAG-0.1.2/docs/source/roadmap/modular_rag.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     3032 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/docs/source/structure.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     3121 2024-02-18 20:58:37.000000 AutoRAG-0.1.2/docs/source/troubleshooting.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     8338 2024-03-29 05:05:10.000000 AutoRAG-0.1.2/docs/source/tutorial.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1529 2024-02-18 20:58:37.000000 AutoRAG-0.1.2/pyproject.toml
--rw-r--r--   0 jeffrey    (501) staff       (20)     1101 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/requirements.txt
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.142612 AutoRAG-0.1.2/sample_config/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2101 2024-03-14 09:00:38.000000 AutoRAG-0.1.2/sample_config/compact_local.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     2420 2024-03-17 04:13:16.000000 AutoRAG-0.1.2/sample_config/compact_openai.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     1222 2024-03-17 04:13:16.000000 AutoRAG-0.1.2/sample_config/config_korean.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)      976 2024-03-06 00:03:36.000000 AutoRAG-0.1.2/sample_config/extracted_sample.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     3569 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/sample_config/full.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)      896 2024-03-14 09:00:38.000000 AutoRAG-0.1.2/sample_config/simple_local.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)      863 2024-02-08 11:27:02.000000 AutoRAG-0.1.2/sample_config/simple_openai.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.142819 AutoRAG-0.1.2/sample_dataset/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1404 2024-02-05 20:46:09.000000 AutoRAG-0.1.2/sample_dataset/README.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.143049 AutoRAG-0.1.2/sample_dataset/eli5/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1109 2024-02-05 20:46:09.000000 AutoRAG-0.1.2/sample_dataset/eli5/load_eli5_dataset.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.143231 AutoRAG-0.1.2/sample_dataset/msmarco/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1167 2024-02-05 20:46:09.000000 AutoRAG-0.1.2/sample_dataset/msmarco/load_msmarco_dataset.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.143516 AutoRAG-0.1.2/sample_dataset/triviaqa/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1171 2024-02-07 10:54:45.000000 AutoRAG-0.1.2/sample_dataset/triviaqa/load_triviaqa_dataset.py
--rw-r--r--   0 jeffrey    (501) staff       (20)       38 2024-04-10 04:46:25.223009 AutoRAG-0.1.2/setup.cfg
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.144370 AutoRAG-0.1.2/tests/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.145906 AutoRAG-0.1.2/tests/autorag/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.059939 AutoRAG-0.1.2/tests/autorag/data/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.146627 AutoRAG-0.1.2/tests/autorag/data/corpus/
--rw-r--r--   0 jeffrey    (501) staff       (20)      620 2024-03-22 04:29:06.000000 AutoRAG-0.1.2/tests/autorag/data/corpus/test_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      642 2024-03-22 04:29:59.000000 AutoRAG-0.1.2/tests/autorag/data/corpus/test_langchain.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      977 2024-03-25 07:44:05.000000 AutoRAG-0.1.2/tests/autorag/data/corpus/test_llama_index_corpus.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.147380 AutoRAG-0.1.2/tests/autorag/data/qacreation/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1415 2024-03-25 11:47:15.000000 AutoRAG-0.1.2/tests/autorag/data/qacreation/test_base_qacreation.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2720 2024-03-25 07:44:05.000000 AutoRAG-0.1.2/tests/autorag/data/qacreation/test_llama_index_qacreation.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1931 2024-03-22 03:52:09.000000 AutoRAG-0.1.2/tests/autorag/data/qacreation/test_simple.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.148350 AutoRAG-0.1.2/tests/autorag/evaluate/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.149076 AutoRAG-0.1.2/tests/autorag/evaluate/metric/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3551 2024-04-05 14:53:42.000000 AutoRAG-0.1.2/tests/autorag/evaluate/metric/test_generation_metric.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1578 2024-02-13 20:13:32.000000 AutoRAG-0.1.2/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1375 2024-04-10 04:41:35.000000 AutoRAG-0.1.2/tests/autorag/evaluate/metric/test_retrieval_metric.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1263 2024-03-08 17:59:53.000000 AutoRAG-0.1.2/tests/autorag/evaluate/test_evaluate_util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3191 2024-02-23 12:23:14.000000 AutoRAG-0.1.2/tests/autorag/evaluate/test_generation_evaluate.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1460 2024-02-13 20:13:32.000000 AutoRAG-0.1.2/tests/autorag/evaluate/test_retrieval_contents_evaluate.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2007 2024-02-13 20:13:32.000000 AutoRAG-0.1.2/tests/autorag/evaluate/test_retrieval_evaluate.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.060708 AutoRAG-0.1.2/tests/autorag/nodes/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.149985 AutoRAG-0.1.2/tests/autorag/nodes/generator/
--rw-r--r--   0 jeffrey    (501) staff       (20)      687 2024-03-08 18:01:40.000000 AutoRAG-0.1.2/tests/autorag/nodes/generator/test_generator_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1372 2024-03-08 17:13:58.000000 AutoRAG-0.1.2/tests/autorag/nodes/generator/test_llama_index_llm.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3263 2024-03-31 05:05:12.000000 AutoRAG-0.1.2/tests/autorag/nodes/generator/test_run_generator_node.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1004 2024-03-08 18:15:21.000000 AutoRAG-0.1.2/tests/autorag/nodes/generator/test_vllm.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.150786 AutoRAG-0.1.2/tests/autorag/nodes/passagecompressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)      820 2024-02-22 15:32:30.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagecompressor/test_pass_compressor.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5091 2024-02-22 16:01:50.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2525 2024-02-22 16:08:56.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagecompressor/test_tree_summarize.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.153723 AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)      795 2024-03-17 04:13:16.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_cohere_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1105 2024-04-08 12:04:54.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_colbert_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1078 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_flag_embedding.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1524 2024-04-06 14:23:40.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_jina_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1063 2024-02-22 16:33:58.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_koreranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      991 2024-02-18 20:58:37.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_monot5.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      818 2024-02-22 15:32:30.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_pass_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3337 2024-02-22 16:33:58.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4830 2024-02-18 20:58:37.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1795 2024-04-05 03:16:26.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_rankgpt.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1120 2024-04-08 08:26:20.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_sentence_transformer.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      963 2024-02-18 20:58:37.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_tart.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      956 2024-02-18 20:58:37.000000 AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_upr.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.154364 AutoRAG-0.1.2/tests/autorag/nodes/promptmaker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1373 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/tests/autorag/nodes/promptmaker/test_fstring.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1798 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/tests/autorag/nodes/promptmaker/test_long_context_reorder.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      580 2024-04-09 15:31:49.000000 AutoRAG-0.1.2/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     7998 2024-03-31 10:29:05.000000 AutoRAG-0.1.2/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.160750 AutoRAG-0.1.2/tests/autorag/nodes/queryexpansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)      813 2024-02-22 15:48:12.000000 AutoRAG-0.1.2/tests/autorag/nodes/queryexpansion/test_hyde.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      544 2024-02-22 15:32:30.000000 AutoRAG-0.1.2/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      991 2024-02-22 15:56:28.000000 AutoRAG-0.1.2/tests/autorag/nodes/queryexpansion/test_query_decompose.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1586 2024-02-15 09:47:24.000000 AutoRAG-0.1.2/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6880 2024-02-22 16:17:25.000000 AutoRAG-0.1.2/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.162355 AutoRAG-0.1.2/tests/autorag/nodes/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2906 2024-03-25 03:54:12.000000 AutoRAG-0.1.2/tests/autorag/nodes/retrieval/test_bm25.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3608 2024-02-13 20:13:32.000000 AutoRAG-0.1.2/tests/autorag/nodes/retrieval/test_hybrid_cc.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4997 2024-02-14 10:09:21.000000 AutoRAG-0.1.2/tests/autorag/nodes/retrieval/test_hybrid_rrf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2976 2024-02-13 20:13:32.000000 AutoRAG-0.1.2/tests/autorag/nodes/retrieval/test_retrieval_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    11185 2024-03-23 14:00:14.000000 AutoRAG-0.1.2/tests/autorag/nodes/retrieval/test_run_retrieval_node.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3757 2024-03-25 07:44:05.000000 AutoRAG-0.1.2/tests/autorag/nodes/retrieval/test_vectordb.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.162845 AutoRAG-0.1.2/tests/autorag/schema/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1033 2024-02-13 20:13:32.000000 AutoRAG-0.1.2/tests/autorag/schema/test_module_schema.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5515 2024-02-13 20:13:32.000000 AutoRAG-0.1.2/tests/autorag/schema/test_node_schema.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3118 2024-03-29 05:05:10.000000 AutoRAG-0.1.2/tests/autorag/test_cli.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6871 2024-02-18 20:58:37.000000 AutoRAG-0.1.2/tests/autorag/test_deploy.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    13837 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/autorag/test_evaluator.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2081 2024-02-13 20:13:32.000000 AutoRAG-0.1.2/tests/autorag/test_strategy.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      306 2024-02-13 20:13:32.000000 AutoRAG-0.1.2/tests/autorag/test_support.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      878 2024-03-06 00:03:36.000000 AutoRAG-0.1.2/tests/autorag/test_web.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.163305 AutoRAG-0.1.2/tests/autorag/utils/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2491 2024-02-13 20:13:32.000000 AutoRAG-0.1.2/tests/autorag/utils/test_preprocess.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     9058 2024-03-25 07:44:05.000000 AutoRAG-0.1.2/tests/autorag/utils/test_util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      124 2024-03-23 03:44:06.000000 AutoRAG-0.1.2/tests/conftest.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      672 2024-02-18 20:58:37.000000 AutoRAG-0.1.2/tests/delete_tests.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2641 2024-02-22 16:04:39.000000 AutoRAG-0.1.2/tests/mock.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.165665 AutoRAG-0.1.2/tests/resources/
--rw-r--r--   0 jeffrey    (501) staff       (20)      796 2024-03-23 03:44:06.000000 AutoRAG-0.1.2/tests/resources/README.md
--rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-01-31 17:28:04.000000 AutoRAG-0.1.2/tests/resources/corpus_data_sample.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.061171 AutoRAG-0.1.2/tests/resources/data_creation/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.166517 AutoRAG-0.1.2/tests/resources/data_creation/raw_dir/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3379 2024-02-08 11:27:05.000000 AutoRAG-0.1.2/tests/resources/data_creation/raw_dir/sample1.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     3243 2024-02-08 11:27:05.000000 AutoRAG-0.1.2/tests/resources/data_creation/raw_dir/sample2.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     4563 2024-02-08 11:27:05.000000 AutoRAG-0.1.2/tests/resources/data_creation/raw_dir/sample3.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     3235 2024-03-31 10:20:41.000000 AutoRAG-0.1.2/tests/resources/full.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-01-15 05:15:36.000000 AutoRAG-0.1.2/tests/resources/qa_data_sample.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.167168 AutoRAG-0.1.2/tests/resources/qa_gen_prompts/
--rw-r--r--   0 jeffrey    (501) staff       (20)      198 2024-03-23 03:44:06.000000 AutoRAG-0.1.2/tests/resources/qa_gen_prompts/prompt1.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      186 2024-03-23 03:44:06.000000 AutoRAG-0.1.2/tests/resources/qa_gen_prompts/prompt2.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      202 2024-03-23 03:44:06.000000 AutoRAG-0.1.2/tests/resources/qa_gen_prompts/prompt3.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     5910 2024-02-07 10:54:45.000000 AutoRAG-0.1.2/tests/resources/qa_test_data_sample.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.167971 AutoRAG-0.1.2/tests/resources/result_project/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.168441 AutoRAG-0.1.2/tests/resources/result_project/0/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2297 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/config.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.168652 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.171322 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/
--rw-r--r--   0 jeffrey    (501) staff       (20)    23516 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    26448 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    33716 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14618 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14683 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    13278 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    54234 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     1155 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.172466 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     8548 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     8443 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    41557 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      513 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      368 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.172699 AutoRAG-0.1.2/tests/resources/result_project/0/pre_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.173942 AutoRAG-0.1.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.174081 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.184479 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/passage_compressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    31124 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      340 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/passage_compressor/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.186012 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/passage_reranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.187546 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/retrieval/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      321 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      845 2024-02-18 14:46:34.000000 AutoRAG-0.1.2/tests/resources/result_project/0/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.187774 AutoRAG-0.1.2/tests/resources/result_project/1/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2458 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/config.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.188181 AutoRAG-0.1.2/tests/resources/result_project/1/pre_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.190061 AutoRAG-0.1.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.062922 AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.190219 AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/passage_compressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.191240 AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/passage_reranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.192651 AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/retrieval/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.192886 AutoRAG-0.1.2/tests/resources/result_project/2/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2458 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/config.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.063164 AutoRAG-0.1.2/tests/resources/result_project/2/post_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.193200 AutoRAG-0.1.2/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     8548 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.193498 AutoRAG-0.1.2/tests/resources/result_project/2/pre_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.195168 AutoRAG-0.1.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.205860 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.206481 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/passage_compressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    31124 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      340 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/passage_compressor/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.209149 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/passage_reranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.210946 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/retrieval/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      321 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.211176 AutoRAG-0.1.2/tests/resources/result_project/3/
--rw-r--r--   0 jeffrey    (501) staff       (20)      682 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/3/config.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     2307 2024-03-29 05:05:10.000000 AutoRAG-0.1.2/tests/resources/result_project/best.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.212176 AutoRAG-0.1.2/tests/resources/result_project/data/
--rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/data/corpus.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/data/qa.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.212504 AutoRAG-0.1.2/tests/resources/result_project/resources/
--rw-r--r--   0 jeffrey    (501) staff       (20)   109454 2024-02-03 19:10:47.000000 AutoRAG-0.1.2/tests/resources/result_project/resources/bm25.pkl
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.212813 AutoRAG-0.1.2/tests/resources/result_project/resources/chroma/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.219789 AutoRAG-0.1.2/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/
--rw-r--r--   0 jeffrey    (501) staff       (20)  6284000 2024-02-18 14:41:41.000000 AutoRAG-0.1.2/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin
--rw-r--r--   0 jeffrey    (501) staff       (20)      100 2024-02-18 14:41:00.000000 AutoRAG-0.1.2/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/header.bin
--rw-r--r--   0 jeffrey    (501) staff       (20)     4000 2024-02-18 14:41:41.000000 AutoRAG-0.1.2/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-18 14:41:00.000000 AutoRAG-0.1.2/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/link_lists.bin
--rw-r--r--   0 jeffrey    (501) staff       (20)   352256 2024-02-18 14:41:41.000000 AutoRAG-0.1.2/tests/resources/result_project/resources/chroma/chroma.sqlite3
--rw-r--r--   0 jeffrey    (501) staff       (20)      338 2024-03-25 11:47:36.000000 AutoRAG-0.1.2/tests/resources/result_project/trial.json
--rw-r--r--   0 jeffrey    (501) staff       (20)     8439 2024-03-23 03:44:06.000000 AutoRAG-0.1.2/tests/resources/sample_contents_nqa.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.064433 AutoRAG-0.1.2/tests/resources/sample_project/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.220648 AutoRAG-0.1.2/tests/resources/sample_project/data/
--rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-01-31 17:28:04.000000 AutoRAG-0.1.2/tests/resources/sample_project/data/corpus.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-01-15 05:15:36.000000 AutoRAG-0.1.2/tests/resources/sample_project/data/qa.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-10 04:46:25.221243 AutoRAG-0.1.2/tests/resources/sample_project/resources/
--rw-r--r--   0 jeffrey    (501) staff       (20)   109454 2024-01-13 07:56:04.000000 AutoRAG-0.1.2/tests/resources/sample_project/resources/bm25.pkl
--rw-r--r--   0 jeffrey    (501) staff       (20)      653 2024-02-15 10:23:20.000000 AutoRAG-0.1.2/tests/resources/simple.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)    26773 2024-01-13 07:56:04.000000 AutoRAG-0.1.2/tests/resources/test_bm25_retrieval.pkl
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.211042 autorag-0.1.3/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.097929 autorag-0.1.3/.github/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      501 2024-01-13 07:55:28.000000 autorag-0.1.3/.github/dependabot.yml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.098426 autorag-0.1.3/.github/workflows/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      818 2024-03-25 06:37:01.000000 autorag-0.1.3/.github/workflows/sphinx.yml
+-rw-r--r--   0 jeffrey    (501) staff       (20)      862 2024-04-06 14:23:40.000000 autorag-0.1.3/.github/workflows/test.yml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3088 2024-01-13 07:55:28.000000 autorag-0.1.3/.gitignore
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.210234 autorag-0.1.3/AutoRAG.egg-info/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    24163 2024-04-14 04:50:14.000000 autorag-0.1.3/AutoRAG.egg-info/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)    18745 2024-04-14 04:50:14.000000 autorag-0.1.3/AutoRAG.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        1 2024-04-14 04:50:14.000000 autorag-0.1.3/AutoRAG.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       44 2024-04-14 04:50:14.000000 autorag-0.1.3/AutoRAG.egg-info/entry_points.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      512 2024-04-14 04:50:14.000000 autorag-0.1.3/AutoRAG.egg-info/requires.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        8 2024-04-14 04:50:14.000000 autorag-0.1.3/AutoRAG.egg-info/top_level.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)    11357 2024-01-13 07:55:28.000000 autorag-0.1.3/LICENSE
+-rw-r--r--   0 jeffrey    (501) staff       (20)    24163 2024-04-14 04:50:14.210777 autorag-0.1.3/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9163 2024-04-11 14:29:33.000000 autorag-0.1.3/README.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.101427 autorag-0.1.3/autorag/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        5 2024-04-14 04:47:22.000000 autorag-0.1.3/autorag/VERSION
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2686 2024-03-27 16:56:49.000000 autorag-0.1.3/autorag/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4400 2024-04-12 13:21:50.000000 autorag-0.1.3/autorag/cli.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.101744 autorag-0.1.3/autorag/data/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-04-01 09:28:42.000000 autorag-0.1.3/autorag/data/__init__.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.102675 autorag-0.1.3/autorag/data/corpus/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      134 2024-03-22 04:27:08.000000 autorag-0.1.3/autorag/data/corpus/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1625 2024-03-22 05:41:56.000000 autorag-0.1.3/autorag/data/corpus/langchain.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2834 2024-03-22 04:27:08.000000 autorag-0.1.3/autorag/data/corpus/llama_index.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.104146 autorag-0.1.3/autorag/data/qacreation/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      124 2024-04-11 07:54:19.000000 autorag-0.1.3/autorag/data/qacreation/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2754 2024-04-12 15:53:11.000000 autorag-0.1.3/autorag/data/qacreation/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     7107 2024-03-23 03:44:06.000000 autorag-0.1.3/autorag/data/qacreation/llama_index.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3190 2024-03-23 03:44:06.000000 autorag-0.1.3/autorag/data/qacreation/llama_index_default_prompt.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2924 2024-04-12 13:21:50.000000 autorag-0.1.3/autorag/data/qacreation/ragas.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3289 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/data/qacreation/simple.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.104520 autorag-0.1.3/autorag/data/utils/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/data/utils/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1496 2024-04-12 13:21:50.000000 autorag-0.1.3/autorag/data/utils/util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8871 2024-03-06 00:03:36.000000 autorag-0.1.3/autorag/deploy.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.105953 autorag-0.1.3/autorag/evaluate/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      146 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/evaluate/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2603 2024-04-05 14:53:42.000000 autorag-0.1.3/autorag/evaluate/generation.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.107098 autorag-0.1.3/autorag/evaluate/metric/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      252 2024-04-05 14:53:42.000000 autorag-0.1.3/autorag/evaluate/metric/__init__.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.108088 autorag-0.1.3/autorag/evaluate/metric/g_eval_prompts/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1186 2024-02-23 11:07:36.000000 autorag-0.1.3/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1015 2024-02-23 11:07:40.000000 autorag-0.1.3/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      814 2024-02-23 11:07:43.000000 autorag-0.1.3/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1005 2024-02-23 11:07:46.000000 autorag-0.1.3/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)    11906 2024-04-05 14:53:42.000000 autorag-0.1.3/autorag/evaluate/metric/generation.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1477 2024-02-23 18:16:58.000000 autorag-0.1.3/autorag/evaluate/metric/retrieval.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2131 2024-02-23 18:16:58.000000 autorag-0.1.3/autorag/evaluate/metric/retrieval_contents.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      224 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/evaluate/metric/util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2052 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/evaluate/retrieval.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2099 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/evaluate/retrieval_contents.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1290 2024-02-18 20:58:37.000000 autorag-0.1.3/autorag/evaluate/util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)    17273 2024-04-12 13:21:55.000000 autorag-0.1.3/autorag/evaluator.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2248 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/node_line.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.108276 autorag-0.1.3/autorag/nodes/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/nodes/__init__.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.109530 autorag-0.1.3/autorag/nodes/generator/
+-rw-r--r--   0 jeffrey    (501) staff       (20)       68 2024-03-07 23:12:39.000000 autorag-0.1.3/autorag/nodes/generator/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2215 2024-03-07 22:31:53.000000 autorag-0.1.3/autorag/nodes/generator/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1641 2024-03-30 16:26:48.000000 autorag-0.1.3/autorag/nodes/generator/llama_index_llm.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4532 2024-03-31 04:56:43.000000 autorag-0.1.3/autorag/nodes/generator/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2810 2024-03-08 18:01:40.000000 autorag-0.1.3/autorag/nodes/generator/vllm.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.110831 autorag-0.1.3/autorag/nodes/passagecompressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)       88 2024-02-22 15:32:30.000000 autorag-0.1.3/autorag/nodes/passagecompressor/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2433 2024-03-06 19:11:31.000000 autorag-0.1.3/autorag/nodes/passagecompressor/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      242 2024-02-22 15:32:30.000000 autorag-0.1.3/autorag/nodes/passagecompressor/pass_compressor.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6075 2024-02-15 17:28:32.000000 autorag-0.1.3/autorag/nodes/passagecompressor/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3028 2024-02-14 10:09:21.000000 autorag-0.1.3/autorag/nodes/passagecompressor/tree_summarize.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.112286 autorag-0.1.3/autorag/nodes/passagefilter/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      171 2024-04-12 13:21:50.000000 autorag-0.1.3/autorag/nodes/passagefilter/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1694 2024-04-10 13:46:46.000000 autorag-0.1.3/autorag/nodes/passagefilter/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      417 2024-04-11 14:32:56.000000 autorag-0.1.3/autorag/nodes/passagefilter/pass_passage_filter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3922 2024-04-12 13:21:50.000000 autorag-0.1.3/autorag/nodes/passagefilter/percentile_cutoff.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3955 2024-04-10 13:46:46.000000 autorag-0.1.3/autorag/nodes/passagefilter/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4022 2024-04-12 13:21:50.000000 autorag-0.1.3/autorag/nodes/passagefilter/threshold_cutoff.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.116264 autorag-0.1.3/autorag/nodes/passagereranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      504 2024-04-12 13:21:50.000000 autorag-0.1.3/autorag/nodes/passagereranker/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2236 2024-04-12 13:21:50.000000 autorag-0.1.3/autorag/nodes/passagereranker/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3979 2024-03-17 04:13:16.000000 autorag-0.1.3/autorag/nodes/passagereranker/cohere.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3625 2024-04-08 12:04:54.000000 autorag-0.1.3/autorag/nodes/passagereranker/colbert.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3548 2024-04-11 14:29:33.000000 autorag-0.1.3/autorag/nodes/passagereranker/flag_embedding.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2248 2024-04-11 14:29:33.000000 autorag-0.1.3/autorag/nodes/passagereranker/flag_embedding_llm.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3713 2024-04-06 14:23:40.000000 autorag-0.1.3/autorag/nodes/passagereranker/jina.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4186 2024-03-06 19:44:35.000000 autorag-0.1.3/autorag/nodes/passagereranker/koreranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6838 2024-03-06 19:44:35.000000 autorag-0.1.3/autorag/nodes/passagereranker/monot5.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      618 2024-04-10 15:52:33.000000 autorag-0.1.3/autorag/nodes/passagereranker/pass_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4712 2024-04-05 03:16:26.000000 autorag-0.1.3/autorag/nodes/passagereranker/rankgpt.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4167 2024-04-10 13:46:46.000000 autorag-0.1.3/autorag/nodes/passagereranker/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3889 2024-04-14 04:47:06.000000 autorag-0.1.3/autorag/nodes/passagereranker/sentence_transformer.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.117192 autorag-0.1.3/autorag/nodes/passagereranker/tart/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/nodes/passagereranker/tart/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4983 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/nodes/passagereranker/tart/modeling_enc_t5.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4452 2024-03-06 19:44:35.000000 autorag-0.1.3/autorag/nodes/passagereranker/tart/tart.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4201 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1758 2024-04-12 13:21:50.000000 autorag-0.1.3/autorag/nodes/passagereranker/time_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     7555 2024-03-06 19:44:35.000000 autorag-0.1.3/autorag/nodes/passagereranker/upr.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.119246 autorag-0.1.3/autorag/nodes/promptmaker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)       84 2024-04-09 15:31:49.000000 autorag-0.1.3/autorag/nodes/promptmaker/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1379 2024-04-09 15:31:49.000000 autorag-0.1.3/autorag/nodes/promptmaker/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1162 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/nodes/promptmaker/fstring.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2290 2024-04-09 15:31:49.000000 autorag-0.1.3/autorag/nodes/promptmaker/long_context_reorder.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8925 2024-03-31 10:20:41.000000 autorag-0.1.3/autorag/nodes/promptmaker/run.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.120925 autorag-0.1.3/autorag/nodes/queryexpansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      123 2024-02-22 15:32:30.000000 autorag-0.1.3/autorag/nodes/queryexpansion/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1663 2024-03-06 19:11:31.000000 autorag-0.1.3/autorag/nodes/queryexpansion/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1572 2024-02-14 10:09:21.000000 autorag-0.1.3/autorag/nodes/queryexpansion/hyde.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      368 2024-02-22 15:32:30.000000 autorag-0.1.3/autorag/nodes/queryexpansion/pass_query_expansion.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3491 2024-02-14 10:09:21.000000 autorag-0.1.3/autorag/nodes/queryexpansion/query_decompose.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     7932 2024-02-15 17:29:26.000000 autorag-0.1.3/autorag/nodes/queryexpansion/run.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.123150 autorag-0.1.3/autorag/nodes/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      227 2024-04-11 14:29:33.000000 autorag-0.1.3/autorag/nodes/retrieval/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6444 2024-04-11 14:29:33.000000 autorag-0.1.3/autorag/nodes/retrieval/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5637 2024-03-25 04:14:52.000000 autorag-0.1.3/autorag/nodes/retrieval/bm25.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3122 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/nodes/retrieval/hybrid_cc.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3221 2024-04-11 14:29:33.000000 autorag-0.1.3/autorag/nodes/retrieval/hybrid_dbsf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2957 2024-02-13 22:39:30.000000 autorag-0.1.3/autorag/nodes/retrieval/hybrid_rrf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4148 2024-04-11 14:29:33.000000 autorag-0.1.3/autorag/nodes/retrieval/hybrid_rsf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)    10780 2024-04-11 14:29:33.000000 autorag-0.1.3/autorag/nodes/retrieval/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4651 2024-03-25 07:44:05.000000 autorag-0.1.3/autorag/nodes/retrieval/vectordb.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.123831 autorag-0.1.3/autorag/schema/
+-rw-r--r--   0 jeffrey    (501) staff       (20)       50 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/schema/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      722 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/schema/module.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4158 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/schema/node.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3996 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/strategy.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3826 2024-04-14 04:47:06.000000 autorag-0.1.3/autorag/support.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.124457 autorag-0.1.3/autorag/utils/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      161 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/utils/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2611 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/utils/preprocess.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9737 2024-04-14 04:47:06.000000 autorag-0.1.3/autorag/utils/util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2563 2024-03-06 00:03:36.000000 autorag-0.1.3/autorag/web.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)       58 2024-02-18 10:18:03.000000 autorag-0.1.3/dev_requirements.txt
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.125086 autorag-0.1.3/docs/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      638 2024-01-17 16:38:11.000000 autorag-0.1.3/docs/Makefile
+-rw-r--r--   0 jeffrey    (501) staff       (20)      804 2024-01-17 11:55:21.000000 autorag-0.1.3/docs/make.bat
+-rw-r--r--   0 jeffrey    (501) staff       (20)      110 2024-03-30 16:07:43.000000 autorag-0.1.3/docs/requirements.txt
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.127033 autorag-0.1.3/docs/source/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.134013 autorag-0.1.3/docs/source/_static/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    57124 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/_static/data_creation.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    30770 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/_static/data_folder.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    31538 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/_static/node_folder.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    18941 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/_static/node_line_folder.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    42589 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/_static/node_line_summary.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    92939 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/_static/node_lines.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    95669 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/_static/node_summary.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    36728 2024-02-07 10:54:42.000000 autorag-0.1.3/docs/source/_static/project_folder_example.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    19853 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/_static/project_folders.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    22432 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/_static/resources_folder.png
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.138104 autorag-0.1.3/docs/source/_static/roadmap/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   159068 2024-02-07 21:45:07.000000 autorag-0.1.3/docs/source/_static/roadmap/RAG_paradigms.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    38568 2024-02-07 21:45:07.000000 autorag-0.1.3/docs/source/_static/roadmap/advanced_RAG.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    62853 2024-02-07 21:45:07.000000 autorag-0.1.3/docs/source/_static/roadmap/cycle.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    75826 2024-02-07 21:45:07.000000 autorag-0.1.3/docs/source/_static/roadmap/merger.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    82200 2024-02-07 21:45:07.000000 autorag-0.1.3/docs/source/_static/roadmap/node_line_modular.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    69999 2024-02-07 21:45:07.000000 autorag-0.1.3/docs/source/_static/roadmap/policy.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)   567356 2024-02-07 10:54:42.000000 autorag-0.1.3/docs/source/_static/samsung_sundae.jpeg
+-rw-r--r--   0 jeffrey    (501) staff       (20)    37348 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/_static/trial_folder.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    25499 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/_static/trial_json.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)   177107 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/_static/trial_summary.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)   269046 2024-03-06 00:03:36.000000 autorag-0.1.3/docs/source/_static/web_interface.png
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.140782 autorag-0.1.3/docs/source/api_spec/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      563 2024-03-22 04:34:21.000000 autorag-0.1.3/docs/source/api_spec/autorag.data.corpus.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      939 2024-04-14 04:49:44.000000 autorag-0.1.3/docs/source/api_spec/autorag.data.qacreation.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      287 2024-03-22 04:34:21.000000 autorag-0.1.3/docs/source/api_spec/autorag.data.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      358 2024-03-22 04:34:21.000000 autorag-0.1.3/docs/source/api_spec/autorag.data.utils.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      984 2024-02-10 14:23:30.000000 autorag-0.1.3/docs/source/api_spec/autorag.evaluate.metric.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      962 2024-02-10 14:23:30.000000 autorag-0.1.3/docs/source/api_spec/autorag.evaluate.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      941 2024-03-17 04:13:16.000000 autorag-0.1.3/docs/source/api_spec/autorag.nodes.generator.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1091 2024-02-22 15:32:30.000000 autorag-0.1.3/docs/source/api_spec/autorag.nodes.passagecompressor.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1277 2024-04-14 04:49:44.000000 autorag-0.1.3/docs/source/api_spec/autorag.nodes.passagefilter.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3229 2024-04-12 13:21:50.000000 autorag-0.1.3/docs/source/api_spec/autorag.nodes.passagereranker.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      952 2024-02-01 16:32:39.000000 autorag-0.1.3/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      995 2024-04-09 15:31:49.000000 autorag-0.1.3/docs/source/api_spec/autorag.nodes.promptmaker.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1254 2024-02-22 15:32:30.000000 autorag-0.1.3/docs/source/api_spec/autorag.nodes.queryexpansion.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1688 2024-04-11 14:29:33.000000 autorag-0.1.3/docs/source/api_spec/autorag.nodes.retrieval.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      432 2024-04-10 13:46:46.000000 autorag-0.1.3/docs/source/api_spec/autorag.nodes.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1239 2024-03-07 15:58:42.000000 autorag-0.1.3/docs/source/api_spec/autorag.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      486 2024-01-17 15:59:52.000000 autorag-0.1.3/docs/source/api_spec/autorag.schema.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      489 2024-01-17 15:59:52.000000 autorag-0.1.3/docs/source/api_spec/autorag.utils.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)       58 2024-01-17 15:59:52.000000 autorag-0.1.3/docs/source/api_spec/modules.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1371 2024-03-30 16:07:43.000000 autorag-0.1.3/docs/source/conf.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.141424 autorag-0.1.3/docs/source/data_creation/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5072 2024-02-18 20:58:37.000000 autorag-0.1.3/docs/source/data_creation/data_format.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2206 2024-04-12 13:21:50.000000 autorag-0.1.3/docs/source/data_creation/ragas.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5543 2024-03-25 11:47:15.000000 autorag-0.1.3/docs/source/data_creation/tutorial.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.141910 autorag-0.1.3/docs/source/deploy/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1473 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/deploy/api_endpoint.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      912 2024-03-06 00:03:36.000000 autorag-0.1.3/docs/source/deploy/web.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4124 2024-04-12 13:21:50.000000 autorag-0.1.3/docs/source/index.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1891 2024-02-15 09:50:25.000000 autorag-0.1.3/docs/source/install.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6153 2024-04-12 13:21:50.000000 autorag-0.1.3/docs/source/local_model.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.142136 autorag-0.1.3/docs/source/nodes/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.142796 autorag-0.1.3/docs/source/nodes/generator/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2703 2024-04-05 14:53:42.000000 autorag-0.1.3/docs/source/nodes/generator/generator.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1306 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/nodes/generator/llama_index_llm.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1358 2024-03-14 09:00:38.000000 autorag-0.1.3/docs/source/nodes/generator/vllm.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      172 2024-04-11 14:29:33.000000 autorag-0.1.3/docs/source/nodes/index.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.143247 autorag-0.1.3/docs/source/nodes/passage_compressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3036 2024-02-22 15:32:30.000000 autorag-0.1.3/docs/source/nodes/passage_compressor/passage_compressor.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1252 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/nodes/passage_compressor/tree_summarize.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.143859 autorag-0.1.3/docs/source/nodes/passage_filter/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1747 2024-04-12 13:21:50.000000 autorag-0.1.3/docs/source/nodes/passage_filter/passage_filter.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1028 2024-04-12 13:21:50.000000 autorag-0.1.3/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1085 2024-04-10 13:46:46.000000 autorag-0.1.3/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.147476 autorag-0.1.3/docs/source/nodes/passage_reranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1151 2024-03-17 04:13:16.000000 autorag-0.1.3/docs/source/nodes/passage_reranker/cohere.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      521 2024-04-08 12:04:54.000000 autorag-0.1.3/docs/source/nodes/passage_reranker/colbert.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      675 2024-04-11 14:29:33.000000 autorag-0.1.3/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      654 2024-04-11 14:29:33.000000 autorag-0.1.3/docs/source/nodes/passage_reranker/flag_embedding_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1232 2024-04-06 14:23:40.000000 autorag-0.1.3/docs/source/nodes/passage_reranker/jina_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      366 2024-02-22 16:33:58.000000 autorag-0.1.3/docs/source/nodes/passage_reranker/koreranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1567 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/nodes/passage_reranker/monot5.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2372 2024-04-12 13:21:50.000000 autorag-0.1.3/docs/source/nodes/passage_reranker/passage_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1063 2024-04-05 03:16:26.000000 autorag-0.1.3/docs/source/nodes/passage_reranker/rankgpt.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      645 2024-04-08 08:26:20.000000 autorag-0.1.3/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      515 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/nodes/passage_reranker/tart.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      561 2024-04-12 13:21:50.000000 autorag-0.1.3/docs/source/nodes/passage_reranker/time_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1435 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/nodes/passage_reranker/upr.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.148278 autorag-0.1.3/docs/source/nodes/prompt_maker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      585 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/nodes/prompt_maker/fstring.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      815 2024-04-09 15:31:49.000000 autorag-0.1.3/docs/source/nodes/prompt_maker/long_context_reorder.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2689 2024-04-09 15:31:49.000000 autorag-0.1.3/docs/source/nodes/prompt_maker/prompt_maker.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.148757 autorag-0.1.3/docs/source/nodes/query_expansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1178 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/nodes/query_expansion/hyde.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1330 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/nodes/query_expansion/query_decompose.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3272 2024-02-22 15:32:30.000000 autorag-0.1.3/docs/source/nodes/query_expansion/query_expansion.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.150086 autorag-0.1.3/docs/source/nodes/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      625 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/nodes/retrieval/bm25.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2216 2024-04-10 06:33:52.000000 autorag-0.1.3/docs/source/nodes/retrieval/hybrid_cc.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2294 2024-04-11 14:29:33.000000 autorag-0.1.3/docs/source/nodes/retrieval/hybrid_dbsf.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2053 2024-04-10 06:33:52.000000 autorag-0.1.3/docs/source/nodes/retrieval/hybrid_rrf.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2304 2024-04-10 06:33:52.000000 autorag-0.1.3/docs/source/nodes/retrieval/hybrid_rsf.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1910 2024-04-11 14:29:33.000000 autorag-0.1.3/docs/source/nodes/retrieval/retrieval.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1223 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/nodes/retrieval/vectordb.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.151103 autorag-0.1.3/docs/source/optimization/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4160 2024-02-15 10:23:20.000000 autorag-0.1.3/docs/source/optimization/custom_config.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3779 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/optimization/folder_structure.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4596 2024-02-07 21:46:19.000000 autorag-0.1.3/docs/source/optimization/optimization.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2580 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/optimization/sample_full_config.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.151322 autorag-0.1.3/docs/source/roadmap/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6735 2024-02-07 21:45:07.000000 autorag-0.1.3/docs/source/roadmap/modular_rag.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3032 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/structure.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3121 2024-02-18 20:58:37.000000 autorag-0.1.3/docs/source/troubleshooting.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8338 2024-03-29 05:05:10.000000 autorag-0.1.3/docs/source/tutorial.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1529 2024-02-18 20:58:37.000000 autorag-0.1.3/pyproject.toml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1149 2024-04-12 13:21:50.000000 autorag-0.1.3/requirements.txt
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.152988 autorag-0.1.3/sample_config/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2101 2024-03-14 09:00:38.000000 autorag-0.1.3/sample_config/compact_local.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2420 2024-03-17 04:13:16.000000 autorag-0.1.3/sample_config/compact_openai.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1222 2024-03-17 04:13:16.000000 autorag-0.1.3/sample_config/config_korean.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)      976 2024-03-06 00:03:36.000000 autorag-0.1.3/sample_config/extracted_sample.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4291 2024-04-12 13:21:50.000000 autorag-0.1.3/sample_config/full.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)      896 2024-03-14 09:00:38.000000 autorag-0.1.3/sample_config/simple_local.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)      863 2024-02-08 11:27:02.000000 autorag-0.1.3/sample_config/simple_openai.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.153222 autorag-0.1.3/sample_dataset/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1404 2024-02-05 20:46:09.000000 autorag-0.1.3/sample_dataset/README.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.153545 autorag-0.1.3/sample_dataset/eli5/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1109 2024-02-05 20:46:09.000000 autorag-0.1.3/sample_dataset/eli5/load_eli5_dataset.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.153788 autorag-0.1.3/sample_dataset/msmarco/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1167 2024-02-05 20:46:09.000000 autorag-0.1.3/sample_dataset/msmarco/load_msmarco_dataset.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.154140 autorag-0.1.3/sample_dataset/triviaqa/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1171 2024-02-07 10:54:45.000000 autorag-0.1.3/sample_dataset/triviaqa/load_triviaqa_dataset.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)       38 2024-04-14 04:50:14.211093 autorag-0.1.3/setup.cfg
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.154892 autorag-0.1.3/tests/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.156437 autorag-0.1.3/tests/autorag/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.092163 autorag-0.1.3/tests/autorag/data/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.157572 autorag-0.1.3/tests/autorag/data/corpus/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      620 2024-03-22 04:29:06.000000 autorag-0.1.3/tests/autorag/data/corpus/test_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      642 2024-03-22 04:29:59.000000 autorag-0.1.3/tests/autorag/data/corpus/test_langchain.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      977 2024-03-25 07:44:05.000000 autorag-0.1.3/tests/autorag/data/corpus/test_llama_index_corpus.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.158511 autorag-0.1.3/tests/autorag/data/qacreation/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1415 2024-04-12 15:50:36.000000 autorag-0.1.3/tests/autorag/data/qacreation/test_base_qacreation.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2720 2024-03-25 07:44:05.000000 autorag-0.1.3/tests/autorag/data/qacreation/test_llama_index_qacreation.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      897 2024-04-12 13:21:50.000000 autorag-0.1.3/tests/autorag/data/qacreation/test_ragas_qa_creation.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1931 2024-03-22 03:52:09.000000 autorag-0.1.3/tests/autorag/data/qacreation/test_simple.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.159428 autorag-0.1.3/tests/autorag/evaluate/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.160118 autorag-0.1.3/tests/autorag/evaluate/metric/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3551 2024-04-05 14:53:42.000000 autorag-0.1.3/tests/autorag/evaluate/metric/test_generation_metric.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1578 2024-02-13 20:13:32.000000 autorag-0.1.3/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1569 2024-04-10 13:46:46.000000 autorag-0.1.3/tests/autorag/evaluate/metric/test_retrieval_metric.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1263 2024-03-08 17:59:53.000000 autorag-0.1.3/tests/autorag/evaluate/test_evaluate_util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3191 2024-02-23 12:23:14.000000 autorag-0.1.3/tests/autorag/evaluate/test_generation_evaluate.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1460 2024-02-13 20:13:32.000000 autorag-0.1.3/tests/autorag/evaluate/test_retrieval_contents_evaluate.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2007 2024-02-13 20:13:32.000000 autorag-0.1.3/tests/autorag/evaluate/test_retrieval_evaluate.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.093041 autorag-0.1.3/tests/autorag/nodes/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.161099 autorag-0.1.3/tests/autorag/nodes/generator/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      687 2024-03-08 18:01:40.000000 autorag-0.1.3/tests/autorag/nodes/generator/test_generator_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1372 2024-03-08 17:13:58.000000 autorag-0.1.3/tests/autorag/nodes/generator/test_llama_index_llm.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3263 2024-03-31 05:05:12.000000 autorag-0.1.3/tests/autorag/nodes/generator/test_run_generator_node.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1004 2024-03-08 18:15:21.000000 autorag-0.1.3/tests/autorag/nodes/generator/test_vllm.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.161857 autorag-0.1.3/tests/autorag/nodes/passagecompressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      820 2024-02-22 15:32:30.000000 autorag-0.1.3/tests/autorag/nodes/passagecompressor/test_pass_compressor.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5091 2024-02-22 16:01:50.000000 autorag-0.1.3/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2525 2024-02-22 16:08:56.000000 autorag-0.1.3/tests/autorag/nodes/passagecompressor/test_tree_summarize.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.163053 autorag-0.1.3/tests/autorag/nodes/passagefilter/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      710 2024-04-11 14:32:56.000000 autorag-0.1.3/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2476 2024-04-10 13:46:46.000000 autorag-0.1.3/tests/autorag/nodes/passagefilter/test_passage_filter_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2999 2024-04-10 13:46:46.000000 autorag-0.1.3/tests/autorag/nodes/passagefilter/test_passage_filter_run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      981 2024-04-12 13:21:50.000000 autorag-0.1.3/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      860 2024-04-10 13:46:46.000000 autorag-0.1.3/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.166753 autorag-0.1.3/tests/autorag/nodes/passagereranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      795 2024-03-17 04:13:16.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_cohere_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1105 2024-04-08 12:04:54.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_colbert_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1078 2024-04-09 15:31:49.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_flag_embedding.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1159 2024-04-11 14:29:33.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1524 2024-04-06 14:23:40.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_jina_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1063 2024-02-22 16:33:58.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_koreranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      991 2024-02-18 20:58:37.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_monot5.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      818 2024-02-22 15:32:30.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_pass_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4364 2024-04-12 13:21:50.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4830 2024-02-18 20:58:37.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1795 2024-04-05 03:16:26.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_rankgpt.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1120 2024-04-08 08:26:20.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_sentence_transformer.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      963 2024-02-18 20:58:37.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_tart.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1210 2024-04-12 13:21:50.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_time_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      956 2024-02-18 20:58:37.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_upr.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.167623 autorag-0.1.3/tests/autorag/nodes/promptmaker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1373 2024-04-09 15:31:49.000000 autorag-0.1.3/tests/autorag/nodes/promptmaker/test_fstring.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1798 2024-04-09 15:31:49.000000 autorag-0.1.3/tests/autorag/nodes/promptmaker/test_long_context_reorder.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      580 2024-04-09 15:31:49.000000 autorag-0.1.3/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     7998 2024-03-31 10:29:05.000000 autorag-0.1.3/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.168932 autorag-0.1.3/tests/autorag/nodes/queryexpansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      813 2024-02-22 15:48:12.000000 autorag-0.1.3/tests/autorag/nodes/queryexpansion/test_hyde.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      544 2024-02-22 15:32:30.000000 autorag-0.1.3/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      991 2024-02-22 15:56:28.000000 autorag-0.1.3/tests/autorag/nodes/queryexpansion/test_query_decompose.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1586 2024-02-15 09:47:24.000000 autorag-0.1.3/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6880 2024-02-22 16:17:25.000000 autorag-0.1.3/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.171883 autorag-0.1.3/tests/autorag/nodes/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2906 2024-03-25 03:54:12.000000 autorag-0.1.3/tests/autorag/nodes/retrieval/test_bm25.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4013 2024-04-11 14:29:33.000000 autorag-0.1.3/tests/autorag/nodes/retrieval/test_hybrid_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1525 2024-04-11 14:29:33.000000 autorag-0.1.3/tests/autorag/nodes/retrieval/test_hybrid_cc.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      879 2024-04-11 14:29:33.000000 autorag-0.1.3/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2989 2024-04-10 06:33:52.000000 autorag-0.1.3/tests/autorag/nodes/retrieval/test_hybrid_rrf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      780 2024-04-11 14:29:33.000000 autorag-0.1.3/tests/autorag/nodes/retrieval/test_hybrid_rsf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2976 2024-02-13 20:13:32.000000 autorag-0.1.3/tests/autorag/nodes/retrieval/test_retrieval_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)    11185 2024-03-23 14:00:14.000000 autorag-0.1.3/tests/autorag/nodes/retrieval/test_run_retrieval_node.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3757 2024-03-25 07:44:05.000000 autorag-0.1.3/tests/autorag/nodes/retrieval/test_vectordb.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.172384 autorag-0.1.3/tests/autorag/schema/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1033 2024-02-13 20:13:32.000000 autorag-0.1.3/tests/autorag/schema/test_module_schema.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5515 2024-02-13 20:13:32.000000 autorag-0.1.3/tests/autorag/schema/test_node_schema.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3118 2024-03-29 05:05:10.000000 autorag-0.1.3/tests/autorag/test_cli.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6869 2024-04-10 13:46:46.000000 autorag-0.1.3/tests/autorag/test_deploy.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14194 2024-04-12 16:43:24.000000 autorag-0.1.3/tests/autorag/test_evaluator.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2081 2024-02-13 20:13:32.000000 autorag-0.1.3/tests/autorag/test_strategy.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      306 2024-02-13 20:13:32.000000 autorag-0.1.3/tests/autorag/test_support.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      878 2024-03-06 00:03:36.000000 autorag-0.1.3/tests/autorag/test_web.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.172779 autorag-0.1.3/tests/autorag/utils/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2491 2024-02-13 20:13:32.000000 autorag-0.1.3/tests/autorag/utils/test_preprocess.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9696 2024-04-12 13:21:50.000000 autorag-0.1.3/tests/autorag/utils/test_util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      124 2024-03-23 03:44:06.000000 autorag-0.1.3/tests/conftest.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      672 2024-02-18 20:58:37.000000 autorag-0.1.3/tests/delete_tests.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2641 2024-02-22 16:04:39.000000 autorag-0.1.3/tests/mock.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.175432 autorag-0.1.3/tests/resources/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      796 2024-03-23 03:44:06.000000 autorag-0.1.3/tests/resources/README.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-01-31 17:28:04.000000 autorag-0.1.3/tests/resources/corpus_data_sample.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.093444 autorag-0.1.3/tests/resources/data_creation/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.176645 autorag-0.1.3/tests/resources/data_creation/raw_dir/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3379 2024-02-08 11:27:05.000000 autorag-0.1.3/tests/resources/data_creation/raw_dir/sample1.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3243 2024-02-08 11:27:05.000000 autorag-0.1.3/tests/resources/data_creation/raw_dir/sample2.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4563 2024-02-08 11:27:05.000000 autorag-0.1.3/tests/resources/data_creation/raw_dir/sample3.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3235 2024-04-12 16:43:24.000000 autorag-0.1.3/tests/resources/full.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-01-15 05:15:36.000000 autorag-0.1.3/tests/resources/qa_data_sample.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.177373 autorag-0.1.3/tests/resources/qa_gen_prompts/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      198 2024-03-23 03:44:06.000000 autorag-0.1.3/tests/resources/qa_gen_prompts/prompt1.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      186 2024-03-23 03:44:06.000000 autorag-0.1.3/tests/resources/qa_gen_prompts/prompt2.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      202 2024-03-23 03:44:06.000000 autorag-0.1.3/tests/resources/qa_gen_prompts/prompt3.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5910 2024-02-07 10:54:45.000000 autorag-0.1.3/tests/resources/qa_test_data_sample.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.178179 autorag-0.1.3/tests/resources/result_project/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.178645 autorag-0.1.3/tests/resources/result_project/0/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2297 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/config.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.178850 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.181316 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    23516 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    26448 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    33716 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14618 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14683 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    13278 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    54234 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1155 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.182195 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8548 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8443 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    41557 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      513 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      368 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.182443 autorag-0.1.3/tests/resources/result_project/0/pre_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.183740 autorag-0.1.3/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.183879 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.184700 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    31124 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      340 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/passage_compressor/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.186144 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.187632 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/retrieval/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      321 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      845 2024-02-18 14:46:34.000000 autorag-0.1.3/tests/resources/result_project/0/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.187859 autorag-0.1.3/tests/resources/result_project/1/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2458 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/config.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.188123 autorag-0.1.3/tests/resources/result_project/1/pre_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.189446 autorag-0.1.3/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.095141 autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.189622 autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.190582 autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.192059 autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/retrieval/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.192304 autorag-0.1.3/tests/resources/result_project/2/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2458 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/config.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.095398 autorag-0.1.3/tests/resources/result_project/2/post_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.192575 autorag-0.1.3/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8548 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.193033 autorag-0.1.3/tests/resources/result_project/2/pre_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.195497 autorag-0.1.3/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.195677 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.196559 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    31124 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      340 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/passage_compressor/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.198301 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.200063 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/retrieval/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      321 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.200297 autorag-0.1.3/tests/resources/result_project/3/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      682 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/3/config.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2307 2024-03-29 05:05:10.000000 autorag-0.1.3/tests/resources/result_project/best.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.201331 autorag-0.1.3/tests/resources/result_project/data/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/data/corpus.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/data/qa.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.201634 autorag-0.1.3/tests/resources/result_project/resources/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   109454 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/resources/bm25.pkl
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.201909 autorag-0.1.3/tests/resources/result_project/resources/chroma/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.208141 autorag-0.1.3/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/
+-rw-r--r--   0 jeffrey    (501) staff       (20)  6284000 2024-02-18 14:41:41.000000 autorag-0.1.3/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin
+-rw-r--r--   0 jeffrey    (501) staff       (20)      100 2024-02-18 14:41:00.000000 autorag-0.1.3/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/header.bin
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4000 2024-02-18 14:41:41.000000 autorag-0.1.3/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-18 14:41:00.000000 autorag-0.1.3/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/link_lists.bin
+-rw-r--r--   0 jeffrey    (501) staff       (20)   352256 2024-02-18 14:41:41.000000 autorag-0.1.3/tests/resources/result_project/resources/chroma/chroma.sqlite3
+-rw-r--r--   0 jeffrey    (501) staff       (20)      338 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/trial.json
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8439 2024-03-23 03:44:06.000000 autorag-0.1.3/tests/resources/sample_contents_nqa.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.096489 autorag-0.1.3/tests/resources/sample_project/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.209096 autorag-0.1.3/tests/resources/sample_project/data/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-01-31 17:28:04.000000 autorag-0.1.3/tests/resources/sample_project/data/corpus.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-01-15 05:15:36.000000 autorag-0.1.3/tests/resources/sample_project/data/qa.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.209387 autorag-0.1.3/tests/resources/sample_project/resources/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   109454 2024-01-13 07:56:04.000000 autorag-0.1.3/tests/resources/sample_project/resources/bm25.pkl
+-rw-r--r--   0 jeffrey    (501) staff       (20)      893 2024-04-10 13:46:46.000000 autorag-0.1.3/tests/resources/simple.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)    26773 2024-01-13 07:56:04.000000 autorag-0.1.3/tests/resources/test_bm25_retrieval.pkl
```

### Comparing `AutoRAG-0.1.2/.github/workflows/sphinx.yml` & `autorag-0.1.3/.github/workflows/sphinx.yml`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/.github/workflows/test.yml` & `autorag-0.1.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/.gitignore` & `autorag-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/AutoRAG.egg-info/PKG-INFO` & `autorag-0.1.3/AutoRAG.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoRAG
-Version: 0.1.2
+Version: 0.1.3
 Summary: Automatically Evaluate RAG pipelines with your own data. Find optimal structure for new RAG product.
 Author-email: Marker-Inc <vkehfdl1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -243,14 +243,15 @@
 Requires-Dist: guidance
 Requires-Dist: cohere>=5.0.0a9
 Requires-Dist: tokenlog>=0.0.2
 Requires-Dist: aiohttp
 Requires-Dist: bert_score
 Requires-Dist: sentence-transformers
 Requires-Dist: FlagEmbedding
+Requires-Dist: ragas
 Requires-Dist: llama-index>=0.10.1
 Requires-Dist: llama-index-core>=0.10.1
 Requires-Dist: llama-index-embeddings-openai
 Requires-Dist: llama-index-embeddings-huggingface
 Requires-Dist: llama-index-llms-openai
 Requires-Dist: llama-index-llms-huggingface
 Requires-Dist: llama-index-llms-openai-like
@@ -492,22 +493,18 @@
             model: [ gpt-3.5-turbo-16k, gpt-3.5-turbo-1106 ]
             temperature: [ 0.5, 1.0, 1.5 ]
 
 ```
 
 # ❗Supporting Nodes & modules
 
-|                                                       Nodes                                                       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Modules                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
-|:-----------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
-|     [Query_Expansion](https://marker-inc-korea.github.io/AutoRAG/nodes/query_expansion/query_expansion.html)      |                                                                                                                                                                                                                                                                                                                                                                                                                                    [Query_Decompose](https://marker-inc-korea.github.io/AutoRAG/nodes/query_expansion/query_decompose.html)<br/>[HyDE](https://marker-inc-korea.github.io/AutoRAG/nodes/query_expansion/hyde.html)                                                                                                                                                                                                                                                                                                                                                                                                                                    |
-|              [Retrieval](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/retrieval.html)               |                                                                                                                                                                                                                                                                                                            [BM25](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/bm25.html)<br/>[VectorDB (choose embedding model)](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/vectordb.html)<br/>[Hybrid with rrf (reciprocal rank fusion)](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/hybrid_rrf.html)<br/>[Hybrid with cc (convex combination)](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/hybrid_cc.html)                                                                                                                                                                                                                                                                                                             |
-|    [Passage_Reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/passage_reranker.html)    | [UPR](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/upr.html)<br/>[Tart](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/tart.html)<br/>[MonoT5](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/monot5.html)<br/>[Ko-reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/koreranker.html)<br/>[cohere_reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/cohere.html)<br/>[RankGPT](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/rankgpt.html)<br/>[Jina Reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/jina_reranker.html)<br/>[Sentence Transformer Reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/setence_transformer_reranker.html)<br/>[Colbert Reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/colbert.html)<br/>[Flag Embedding Reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/flag_embedding_reranker.html) |
-| [Passage_Compressor](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_compressor/passage_compressor.html) |                                                                                                                                                                                                                                                                                                                                                                                                                  [Tree Summarize](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_compressor/tree_summarize.html)<br/>[Long Context Reorder](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_compressor/long_context_reorder.html)                                                                                                                                                                                                                                                                                                                                                                                                                  |
-|          [Prompt Maker](https://marker-inc-korea.github.io/AutoRAG/nodes/prompt_maker/prompt_maker.html)          |                                                                                                                                                                                                                                                                                                                                                                                                                                                                             [Default Prompt Maker (f-string)](https://marker-inc-korea.github.io/AutoRAG/nodes/prompt_maker/fstring.html)                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
-|              [Generator](https://marker-inc-korea.github.io/AutoRAG/nodes/generator/generator.html)               |                                                                                                                                                                                                                                                                                                                                                                                                                                          [llama_index llm](https://marker-inc-korea.github.io/AutoRAG/nodes/generator/llama_index_llm.html)<br/>[vllm](https://marker-inc-korea.github.io/AutoRAG/nodes/generator/vllm.html)                                                                                                                                                                                                                                                                                                                                                                                                                                          |
+You can check our all supporting Nodes & modules
+at [here](https://edai.notion.site/Supporting-Nodes-modules-0ebc7810649f4e41aead472a92976be4?pvs=4)
+
+
 
 # 🛣Roadmap
 
 - [ ] Policy Module for modular RAG pipeline
 - [ ] Visualize evaluation result
 - [ ] Visualize config yaml file
 - [ ] More RAG modules support
```

### Comparing `AutoRAG-0.1.2/AutoRAG.egg-info/SOURCES.txt` & `autorag-0.1.3/AutoRAG.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 autorag/data/corpus/__init__.py
 autorag/data/corpus/langchain.py
 autorag/data/corpus/llama_index.py
 autorag/data/qacreation/__init__.py
 autorag/data/qacreation/base.py
 autorag/data/qacreation/llama_index.py
 autorag/data/qacreation/llama_index_default_prompt.txt
+autorag/data/qacreation/ragas.py
 autorag/data/qacreation/simple.py
 autorag/data/utils/__init__.py
 autorag/data/utils/util.py
 autorag/evaluate/__init__.py
 autorag/evaluate/generation.py
 autorag/evaluate/retrieval.py
 autorag/evaluate/retrieval_contents.py
@@ -54,26 +55,34 @@
 autorag/nodes/generator/run.py
 autorag/nodes/generator/vllm.py
 autorag/nodes/passagecompressor/__init__.py
 autorag/nodes/passagecompressor/base.py
 autorag/nodes/passagecompressor/pass_compressor.py
 autorag/nodes/passagecompressor/run.py
 autorag/nodes/passagecompressor/tree_summarize.py
+autorag/nodes/passagefilter/__init__.py
+autorag/nodes/passagefilter/base.py
+autorag/nodes/passagefilter/pass_passage_filter.py
+autorag/nodes/passagefilter/percentile_cutoff.py
+autorag/nodes/passagefilter/run.py
+autorag/nodes/passagefilter/threshold_cutoff.py
 autorag/nodes/passagereranker/__init__.py
 autorag/nodes/passagereranker/base.py
 autorag/nodes/passagereranker/cohere.py
 autorag/nodes/passagereranker/colbert.py
 autorag/nodes/passagereranker/flag_embedding.py
+autorag/nodes/passagereranker/flag_embedding_llm.py
 autorag/nodes/passagereranker/jina.py
 autorag/nodes/passagereranker/koreranker.py
 autorag/nodes/passagereranker/monot5.py
 autorag/nodes/passagereranker/pass_reranker.py
 autorag/nodes/passagereranker/rankgpt.py
 autorag/nodes/passagereranker/run.py
 autorag/nodes/passagereranker/sentence_transformer.py
+autorag/nodes/passagereranker/time_reranker.py
 autorag/nodes/passagereranker/upr.py
 autorag/nodes/passagereranker/tart/__init__.py
 autorag/nodes/passagereranker/tart/modeling_enc_t5.py
 autorag/nodes/passagereranker/tart/tart.py
 autorag/nodes/passagereranker/tart/tokenization_enc_t5.py
 autorag/nodes/promptmaker/__init__.py
 autorag/nodes/promptmaker/base.py
@@ -86,15 +95,17 @@
 autorag/nodes/queryexpansion/pass_query_expansion.py
 autorag/nodes/queryexpansion/query_decompose.py
 autorag/nodes/queryexpansion/run.py
 autorag/nodes/retrieval/__init__.py
 autorag/nodes/retrieval/base.py
 autorag/nodes/retrieval/bm25.py
 autorag/nodes/retrieval/hybrid_cc.py
+autorag/nodes/retrieval/hybrid_dbsf.py
 autorag/nodes/retrieval/hybrid_rrf.py
+autorag/nodes/retrieval/hybrid_rsf.py
 autorag/nodes/retrieval/run.py
 autorag/nodes/retrieval/vectordb.py
 autorag/schema/__init__.py
 autorag/schema/module.py
 autorag/schema/node.py
 autorag/utils/__init__.py
 autorag/utils/preprocess.py
@@ -134,54 +145,63 @@
 docs/source/api_spec/autorag.data.qacreation.rst
 docs/source/api_spec/autorag.data.rst
 docs/source/api_spec/autorag.data.utils.rst
 docs/source/api_spec/autorag.evaluate.metric.rst
 docs/source/api_spec/autorag.evaluate.rst
 docs/source/api_spec/autorag.nodes.generator.rst
 docs/source/api_spec/autorag.nodes.passagecompressor.rst
+docs/source/api_spec/autorag.nodes.passagefilter.rst
 docs/source/api_spec/autorag.nodes.passagereranker.rst
 docs/source/api_spec/autorag.nodes.passagereranker.tart.rst
 docs/source/api_spec/autorag.nodes.promptmaker.rst
 docs/source/api_spec/autorag.nodes.queryexpansion.rst
 docs/source/api_spec/autorag.nodes.retrieval.rst
 docs/source/api_spec/autorag.nodes.rst
 docs/source/api_spec/autorag.rst
 docs/source/api_spec/autorag.schema.rst
 docs/source/api_spec/autorag.utils.rst
 docs/source/api_spec/modules.rst
 docs/source/data_creation/data_format.md
+docs/source/data_creation/ragas.md
 docs/source/data_creation/tutorial.md
 docs/source/deploy/api_endpoint.md
 docs/source/deploy/web.md
 docs/source/nodes/index.md
 docs/source/nodes/generator/generator.md
 docs/source/nodes/generator/llama_index_llm.md
 docs/source/nodes/generator/vllm.md
 docs/source/nodes/passage_compressor/passage_compressor.md
 docs/source/nodes/passage_compressor/tree_summarize.md
+docs/source/nodes/passage_filter/passage_filter.md
+docs/source/nodes/passage_filter/similarity_percentile_cutoff.md
+docs/source/nodes/passage_filter/similarity_threshold_cutoff.md
 docs/source/nodes/passage_reranker/cohere.md
 docs/source/nodes/passage_reranker/colbert.md
+docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md
 docs/source/nodes/passage_reranker/flag_embedding_reranker.md
 docs/source/nodes/passage_reranker/jina_reranker.md
 docs/source/nodes/passage_reranker/koreranker.md
 docs/source/nodes/passage_reranker/monot5.md
 docs/source/nodes/passage_reranker/passage_reranker.md
 docs/source/nodes/passage_reranker/rankgpt.md
 docs/source/nodes/passage_reranker/sentence_transformer_reranker.md
 docs/source/nodes/passage_reranker/tart.md
+docs/source/nodes/passage_reranker/time_reranker.md
 docs/source/nodes/passage_reranker/upr.md
 docs/source/nodes/prompt_maker/fstring.md
 docs/source/nodes/prompt_maker/long_context_reorder.md
 docs/source/nodes/prompt_maker/prompt_maker.md
 docs/source/nodes/query_expansion/hyde.md
 docs/source/nodes/query_expansion/query_decompose.md
 docs/source/nodes/query_expansion/query_expansion.md
 docs/source/nodes/retrieval/bm25.md
 docs/source/nodes/retrieval/hybrid_cc.md
+docs/source/nodes/retrieval/hybrid_dbsf.md
 docs/source/nodes/retrieval/hybrid_rrf.md
+docs/source/nodes/retrieval/hybrid_rsf.md
 docs/source/nodes/retrieval/retrieval.md
 docs/source/nodes/retrieval/vectordb.md
 docs/source/optimization/custom_config.md
 docs/source/optimization/folder_structure.md
 docs/source/optimization/optimization.md
 docs/source/optimization/sample_full_config.yaml
 docs/source/roadmap/modular_rag.md
@@ -206,14 +226,15 @@
 tests/autorag/test_support.py
 tests/autorag/test_web.py
 tests/autorag/data/corpus/test_base.py
 tests/autorag/data/corpus/test_langchain.py
 tests/autorag/data/corpus/test_llama_index_corpus.py
 tests/autorag/data/qacreation/test_base_qacreation.py
 tests/autorag/data/qacreation/test_llama_index_qacreation.py
+tests/autorag/data/qacreation/test_ragas_qa_creation.py
 tests/autorag/data/qacreation/test_simple.py
 tests/autorag/evaluate/test_evaluate_util.py
 tests/autorag/evaluate/test_generation_evaluate.py
 tests/autorag/evaluate/test_retrieval_contents_evaluate.py
 tests/autorag/evaluate/test_retrieval_evaluate.py
 tests/autorag/evaluate/metric/test_generation_metric.py
 tests/autorag/evaluate/metric/test_retrieval_contents_metric.py
@@ -221,39 +242,49 @@
 tests/autorag/nodes/generator/test_generator_base.py
 tests/autorag/nodes/generator/test_llama_index_llm.py
 tests/autorag/nodes/generator/test_run_generator_node.py
 tests/autorag/nodes/generator/test_vllm.py
 tests/autorag/nodes/passagecompressor/test_pass_compressor.py
 tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py
 tests/autorag/nodes/passagecompressor/test_tree_summarize.py
+tests/autorag/nodes/passagefilter/test_pass_passage_filter.py
+tests/autorag/nodes/passagefilter/test_passage_filter_base.py
+tests/autorag/nodes/passagefilter/test_passage_filter_run.py
+tests/autorag/nodes/passagefilter/test_percentile_cutoff.py
+tests/autorag/nodes/passagefilter/test_threshold_cutoff.py
 tests/autorag/nodes/passagereranker/test_cohere_reranker.py
 tests/autorag/nodes/passagereranker/test_colbert_reranker.py
 tests/autorag/nodes/passagereranker/test_flag_embedding.py
+tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py
 tests/autorag/nodes/passagereranker/test_jina_reranker.py
 tests/autorag/nodes/passagereranker/test_koreranker.py
 tests/autorag/nodes/passagereranker/test_monot5.py
 tests/autorag/nodes/passagereranker/test_pass_reranker.py
 tests/autorag/nodes/passagereranker/test_passage_reranker_base.py
 tests/autorag/nodes/passagereranker/test_passage_reranker_run.py
 tests/autorag/nodes/passagereranker/test_rankgpt.py
 tests/autorag/nodes/passagereranker/test_sentence_transformer.py
 tests/autorag/nodes/passagereranker/test_tart.py
+tests/autorag/nodes/passagereranker/test_time_reranker.py
 tests/autorag/nodes/passagereranker/test_upr.py
 tests/autorag/nodes/promptmaker/test_fstring.py
 tests/autorag/nodes/promptmaker/test_long_context_reorder.py
 tests/autorag/nodes/promptmaker/test_prompt_maker_base.py
 tests/autorag/nodes/promptmaker/test_prompt_maker_run.py
 tests/autorag/nodes/queryexpansion/test_hyde.py
 tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py
 tests/autorag/nodes/queryexpansion/test_query_decompose.py
 tests/autorag/nodes/queryexpansion/test_query_expansion_base.py
 tests/autorag/nodes/queryexpansion/test_query_expansion_run.py
 tests/autorag/nodes/retrieval/test_bm25.py
+tests/autorag/nodes/retrieval/test_hybrid_base.py
 tests/autorag/nodes/retrieval/test_hybrid_cc.py
+tests/autorag/nodes/retrieval/test_hybrid_dbsf.py
 tests/autorag/nodes/retrieval/test_hybrid_rrf.py
+tests/autorag/nodes/retrieval/test_hybrid_rsf.py
 tests/autorag/nodes/retrieval/test_retrieval_base.py
 tests/autorag/nodes/retrieval/test_run_retrieval_node.py
 tests/autorag/nodes/retrieval/test_vectordb.py
 tests/autorag/schema/test_module_schema.py
 tests/autorag/schema/test_node_schema.py
 tests/autorag/utils/test_preprocess.py
 tests/autorag/utils/test_util.py
```

### Comparing `AutoRAG-0.1.2/LICENSE` & `autorag-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/PKG-INFO` & `autorag-0.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoRAG
-Version: 0.1.2
+Version: 0.1.3
 Summary: Automatically Evaluate RAG pipelines with your own data. Find optimal structure for new RAG product.
 Author-email: Marker-Inc <vkehfdl1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -243,14 +243,15 @@
 Requires-Dist: guidance
 Requires-Dist: cohere>=5.0.0a9
 Requires-Dist: tokenlog>=0.0.2
 Requires-Dist: aiohttp
 Requires-Dist: bert_score
 Requires-Dist: sentence-transformers
 Requires-Dist: FlagEmbedding
+Requires-Dist: ragas
 Requires-Dist: llama-index>=0.10.1
 Requires-Dist: llama-index-core>=0.10.1
 Requires-Dist: llama-index-embeddings-openai
 Requires-Dist: llama-index-embeddings-huggingface
 Requires-Dist: llama-index-llms-openai
 Requires-Dist: llama-index-llms-huggingface
 Requires-Dist: llama-index-llms-openai-like
@@ -492,22 +493,18 @@
             model: [ gpt-3.5-turbo-16k, gpt-3.5-turbo-1106 ]
             temperature: [ 0.5, 1.0, 1.5 ]
 
 ```
 
 # ❗Supporting Nodes & modules
 
-|                                                       Nodes                                                       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Modules                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
-|:-----------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
-|     [Query_Expansion](https://marker-inc-korea.github.io/AutoRAG/nodes/query_expansion/query_expansion.html)      |                                                                                                                                                                                                                                                                                                                                                                                                                                    [Query_Decompose](https://marker-inc-korea.github.io/AutoRAG/nodes/query_expansion/query_decompose.html)<br/>[HyDE](https://marker-inc-korea.github.io/AutoRAG/nodes/query_expansion/hyde.html)                                                                                                                                                                                                                                                                                                                                                                                                                                    |
-|              [Retrieval](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/retrieval.html)               |                                                                                                                                                                                                                                                                                                            [BM25](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/bm25.html)<br/>[VectorDB (choose embedding model)](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/vectordb.html)<br/>[Hybrid with rrf (reciprocal rank fusion)](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/hybrid_rrf.html)<br/>[Hybrid with cc (convex combination)](https://marker-inc-korea.github.io/AutoRAG/nodes/retrieval/hybrid_cc.html)                                                                                                                                                                                                                                                                                                             |
-|    [Passage_Reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/passage_reranker.html)    | [UPR](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/upr.html)<br/>[Tart](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/tart.html)<br/>[MonoT5](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/monot5.html)<br/>[Ko-reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/koreranker.html)<br/>[cohere_reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/cohere.html)<br/>[RankGPT](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/rankgpt.html)<br/>[Jina Reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/jina_reranker.html)<br/>[Sentence Transformer Reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/setence_transformer_reranker.html)<br/>[Colbert Reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/colbert.html)<br/>[Flag Embedding Reranker](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_reranker/flag_embedding_reranker.html) |
-| [Passage_Compressor](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_compressor/passage_compressor.html) |                                                                                                                                                                                                                                                                                                                                                                                                                  [Tree Summarize](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_compressor/tree_summarize.html)<br/>[Long Context Reorder](https://marker-inc-korea.github.io/AutoRAG/nodes/passage_compressor/long_context_reorder.html)                                                                                                                                                                                                                                                                                                                                                                                                                  |
-|          [Prompt Maker](https://marker-inc-korea.github.io/AutoRAG/nodes/prompt_maker/prompt_maker.html)          |                                                                                                                                                                                                                                                                                                                                                                                                                                                                             [Default Prompt Maker (f-string)](https://marker-inc-korea.github.io/AutoRAG/nodes/prompt_maker/fstring.html)                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
-|              [Generator](https://marker-inc-korea.github.io/AutoRAG/nodes/generator/generator.html)               |                                                                                                                                                                                                                                                                                                                                                                                                                                          [llama_index llm](https://marker-inc-korea.github.io/AutoRAG/nodes/generator/llama_index_llm.html)<br/>[vllm](https://marker-inc-korea.github.io/AutoRAG/nodes/generator/vllm.html)                                                                                                                                                                                                                                                                                                                                                                                                                                          |
+You can check our all supporting Nodes & modules
+at [here](https://edai.notion.site/Supporting-Nodes-modules-0ebc7810649f4e41aead472a92976be4?pvs=4)
+
+
 
 # 🛣Roadmap
 
 - [ ] Policy Module for modular RAG pipeline
 - [ ] Visualize evaluation result
 - [ ] Visualize config yaml file
 - [ ] More RAG modules support
```

### Comparing `AutoRAG-0.1.2/autorag/__init__.py` & `autorag-0.1.3/autorag/__init__.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/cli.py` & `autorag-0.1.3/autorag/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import importlib.resources
 import logging
 import os
 import pathlib
 import subprocess
+from pathlib import Path
 from typing import Optional
 
 import click
 
 from autorag.deploy import Runner
 from autorag.deploy import extract_best_config as original_extract_best_config
 from autorag.evaluator import Evaluator
@@ -42,17 +43,17 @@
 def run_api(config_path, host, port, project_dir):
     runner = Runner.from_yaml(config_path, project_dir=project_dir)
     logger.info(f"Running API server at {host}:{port}...")
     runner.run_api_server(host, port)
 
 
 @click.command()
-@click.option('--yaml_path', type=click.Path(), help='Path to the YAML file.')
-@click.option('--project_dir', type=click.Path(), help='Path to the project directory.')
-@click.option('--trial_path', type=click.Path(), help='Path to the trial directory.')
+@click.option('--yaml_path', type=click.Path(path_type=Path), help='Path to the YAML file.')
+@click.option('--project_dir', type=click.Path(path_type=Path), help='Path to the project directory.')
+@click.option('--trial_path', type=click.Path(path_type=Path), help='Path to the trial directory.')
 def run_web(yaml_path: Optional[str], project_dir: Optional[str], trial_path: Optional[str]):
     try:
         with importlib.resources.path('autorag', 'web.py') as web_path:
             web_py_path = str(web_path)
     except ImportError:
         raise ImportError("Could not locate the web.py file within the autorag package."
                           " Please ensure that autorag is correctly installed.")
```

### Comparing `AutoRAG-0.1.2/autorag/data/corpus/langchain.py` & `autorag-0.1.3/autorag/data/corpus/langchain.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/data/corpus/llama_index.py` & `autorag-0.1.3/autorag/data/corpus/llama_index.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/data/qacreation/base.py` & `autorag-0.1.3/autorag/data/qacreation/base.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/data/qacreation/llama_index.py` & `autorag-0.1.3/autorag/data/qacreation/llama_index.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/data/qacreation/llama_index_default_prompt.txt` & `autorag-0.1.3/autorag/data/qacreation/llama_index_default_prompt.txt`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/data/qacreation/simple.py` & `autorag-0.1.3/autorag/data/qacreation/simple.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/deploy.py` & `autorag-0.1.3/autorag/deploy.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/evaluate/generation.py` & `autorag-0.1.3/autorag/evaluate/generation.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt` & `autorag-0.1.3/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt` & `autorag-0.1.3/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt` & `autorag-0.1.3/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt` & `autorag-0.1.3/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/evaluate/metric/generation.py` & `autorag-0.1.3/autorag/evaluate/metric/generation.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/evaluate/metric/retrieval.py` & `autorag-0.1.3/autorag/evaluate/metric/retrieval.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/evaluate/metric/retrieval_contents.py` & `autorag-0.1.3/autorag/evaluate/metric/retrieval_contents.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/evaluate/retrieval.py` & `autorag-0.1.3/autorag/evaluate/retrieval.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/evaluate/retrieval_contents.py` & `autorag-0.1.3/autorag/evaluate/retrieval_contents.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/evaluate/util.py` & `autorag-0.1.3/autorag/evaluate/util.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/evaluator.py` & `autorag-0.1.3/autorag/evaluator.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,24 @@
 from autorag.schema import Node
 from autorag.schema.node import module_type_exists, extract_values_from_nodes
 from autorag.utils import cast_qa_dataset, cast_corpus_dataset
 from autorag.utils.util import load_summary_file, convert_string_to_tuple_in_dict, convert_env_in_dict, explode
 
 logger = logging.getLogger("AutoRAG")
 
+ascii_art = """
+                _        _____            _____ 
+     /\        | |      |  __ \     /\   / ____|
+    /  \  _   _| |_ ___ | |__) |   /  \ | |  __ 
+   / /\ \| | | | __/ _ \|  _  /   / /\ \| | |_ |
+  / ____ \ |_| | || (_) | | \ \  / ____ \ |__| |
+ /_/    \_\__,_|\__\___/|_|  \_\/_/    \_\_____|
+                                                
+"""
+
 
 class Evaluator:
     def __init__(self, qa_data_path: str, corpus_data_path: str, project_dir: Optional[str] = None):
         """
         Initialize an Evaluator object.
 
         :param qa_data_path: The path to the QA dataset.
@@ -60,14 +70,16 @@
         if not os.path.exists(qa_path_in_project):
             self.qa_data.to_parquet(qa_path_in_project, index=False)
         corpus_path_in_project = os.path.join(self.project_dir, 'data', 'corpus.parquet')
         if not os.path.exists(corpus_path_in_project):
             self.corpus_data.to_parquet(corpus_path_in_project, index=False)
 
     def start_trial(self, yaml_path: str):
+        logger.info(ascii_art)
+
         trial_name = self.__get_new_trial_name()
         self.__make_trial_dir(trial_name)
 
         # copy yaml file to trial directory
         shutil.copy(yaml_path, os.path.join(self.project_dir, trial_name, 'config.yaml'))
         node_lines = self._load_node_lines(yaml_path)
         self.__embed(node_lines)
@@ -170,14 +182,15 @@
         node_line_dict = {}
         for node_line in node_lines:
             node_line_dict[node_line['node_line_name']] = list(
                 map(lambda node: Node.from_dict(node), node_line['nodes']))
         return node_line_dict
 
     def restart_trial(self, trial_path: str):
+        logger.info(ascii_art)
         # Check if trial_path exists
         if not os.path.exists(trial_path):
             raise ValueError(f"Trial path {trial_path} does not exist.")
         # Check if trial is completed
         if os.path.exists(os.path.join(trial_path, 'summary.csv')):
             raise ValueError(f"Trial path {trial_path} is already completed.")
```

### Comparing `AutoRAG-0.1.2/autorag/node_line.py` & `autorag-0.1.3/autorag/node_line.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/generator/base.py` & `autorag-0.1.3/autorag/nodes/generator/base.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/generator/llama_index_llm.py` & `autorag-0.1.3/autorag/nodes/generator/llama_index_llm.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/generator/run.py` & `autorag-0.1.3/autorag/nodes/generator/run.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/generator/vllm.py` & `autorag-0.1.3/autorag/nodes/generator/vllm.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/passagecompressor/base.py` & `autorag-0.1.3/autorag/nodes/passagecompressor/base.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/passagecompressor/run.py` & `autorag-0.1.3/autorag/nodes/passagecompressor/run.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/passagecompressor/tree_summarize.py` & `autorag-0.1.3/autorag/nodes/passagecompressor/tree_summarize.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/passagereranker/base.py` & `autorag-0.1.3/autorag/nodes/passagefilter/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import functools
-import logging
 from pathlib import Path
-from typing import List, Union, Tuple
+from typing import Union, Tuple, List
 
 import pandas as pd
 
 from autorag.utils import result_to_dataframe, validate_qa_dataset
 
-logger = logging.getLogger("AutoRAG")
 
-
-def passage_reranker_node(func):
+# same with passage filter from now
+def passage_filter_node(func):
     @functools.wraps(func)
-    @result_to_dataframe(["retrieved_contents", "retrieved_ids", "retrieve_scores"])
+    @result_to_dataframe(['retrieved_contents', 'retrieved_ids', 'retrieve_scores'])
     def wrapper(
             project_dir: Union[str, Path],
             previous_result: pd.DataFrame,
             *args, **kwargs) -> Tuple[List[List[str]], List[List[str]], List[List[float]]]:
         validate_qa_dataset(previous_result)
 
         # find queries columns
@@ -31,13 +29,13 @@
         assert "retrieve_scores" in previous_result.columns, "previous_result must have retrieve_scores column."
         scores = previous_result["retrieve_scores"].tolist()
 
         # find ids columns
         assert "retrieved_ids" in previous_result.columns, "previous_result must have retrieved_ids column."
         ids = previous_result["retrieved_ids"].tolist()
 
-        reranked_contents, reranked_ids, reranked_scores \
-            = func(queries=queries, contents_list=contents, scores_list=scores, ids_list=ids, *args, **kwargs)
+        filtered_contents, filtered_ids, filtered_scores = func(queries=queries, contents_list=contents,
+                                                                scores_list=scores, ids_list=ids, *args, **kwargs)
 
-        return reranked_contents, reranked_ids, reranked_scores
+        return filtered_contents, filtered_ids, filtered_scores
 
     return wrapper
```

### Comparing `AutoRAG-0.1.2/autorag/nodes/passagereranker/cohere.py` & `autorag-0.1.3/autorag/nodes/passagereranker/cohere.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/passagereranker/colbert.py` & `autorag-0.1.3/autorag/nodes/passagereranker/colbert.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/passagereranker/flag_embedding.py` & `autorag-0.1.3/autorag/nodes/passagereranker/flag_embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 @passage_reranker_node
 def flag_embedding_reranker(queries: List[str], contents_list: List[List[str]],
                             scores_list: List[List[float]], ids_list: List[List[str]],
                             top_k: int, batch: int = 64, use_fp16: bool = False,
                             model_name: str = "BAAI/bge-reranker-large",
                             ) -> Tuple[List[List[str]], List[List[str]], List[List[float]]]:
     """
-    Rerank a list of contents based on their relevance to a query using BAAI Reranker model.
+    Rerank a list of contents based on their relevance to a query using BAAI normal-Reranker model.
 
     :param queries: The list of queries to use for reranking
     :param contents_list: The list of lists of contents to rerank
     :param scores_list: The list of lists of scores retrieved from the initial ranking
     :param ids_list: The list of lists of ids retrieved from the initial ranking
     :param top_k: The number of passages to be retrieved
     :param batch: The number of queries to be processed in a batch
     :param use_fp16: Whether to use fp16 for inference
-    :param model_name: The name of the BAAI Reranker model name.
+    :param model_name: The name of the BAAI Reranker normal-model name.
         Default is "BAAI/bge-reranker-large"
     :return: tuple of lists containing the reranked contents, ids, and scores
     """
     model = FlagReranker(
         model_name_or_path=model_name, use_fp16=use_fp16
     )
     tasks = [flag_embedding_reranker_pure(query, contents, scores, top_k, ids, model)
```

### Comparing `AutoRAG-0.1.2/autorag/nodes/passagereranker/jina.py` & `autorag-0.1.3/autorag/nodes/passagereranker/jina.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/passagereranker/koreranker.py` & `autorag-0.1.3/autorag/nodes/passagereranker/koreranker.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/passagereranker/monot5.py` & `autorag-0.1.3/autorag/nodes/passagereranker/monot5.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/passagereranker/pass_reranker.py` & `autorag-0.1.3/autorag/nodes/passagereranker/pass_reranker.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/passagereranker/rankgpt.py` & `autorag-0.1.3/autorag/nodes/passagereranker/rankgpt.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/passagereranker/run.py` & `autorag-0.1.3/autorag/nodes/passagereranker/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     :param modules: Passage reranker modules to run.
     :param module_params: Passage reranker module parameters.
     :param previous_result: Previous result dataframe.
         Could be retrieval, reranker modules result.
         It means it must contain 'query', 'retrieved_contents', 'retrieved_ids', 'retrieve_scores' columns.
     :param node_line_dir: This node line's directory.
     :param strategies: Strategies for passage reranker node.
-        In this node, we use
+        In this node, we use 'retrieval_f1', 'retrieval_recall' and 'retrieval_precision'.
         You can skip evaluation when you use only one module and a module parameter.
     :return: The best result dataframe with previous result columns.
     """
     if not os.path.exists(node_line_dir):
         os.makedirs(node_line_dir)
     project_dir = pathlib.PurePath(node_line_dir).parent.parent
     retrieval_gt = pd.read_parquet(os.path.join(project_dir, "data", "qa.parquet"))['retrieval_gt'].tolist()
```

### Comparing `AutoRAG-0.1.2/autorag/nodes/passagereranker/sentence_transformer.py` & `autorag-0.1.3/autorag/nodes/passagereranker/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/passagereranker/tart/modeling_enc_t5.py` & `autorag-0.1.3/autorag/nodes/passagereranker/tart/modeling_enc_t5.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/passagereranker/tart/tart.py` & `autorag-0.1.3/autorag/nodes/passagereranker/tart/tart.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py` & `autorag-0.1.3/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/passagereranker/upr.py` & `autorag-0.1.3/autorag/nodes/passagereranker/upr.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/promptmaker/base.py` & `autorag-0.1.3/autorag/nodes/promptmaker/base.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/promptmaker/fstring.py` & `autorag-0.1.3/autorag/nodes/promptmaker/fstring.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/promptmaker/long_context_reorder.py` & `autorag-0.1.3/autorag/nodes/promptmaker/long_context_reorder.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/promptmaker/run.py` & `autorag-0.1.3/autorag/nodes/promptmaker/run.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/queryexpansion/base.py` & `autorag-0.1.3/autorag/nodes/queryexpansion/base.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/queryexpansion/hyde.py` & `autorag-0.1.3/autorag/nodes/queryexpansion/hyde.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/queryexpansion/query_decompose.py` & `autorag-0.1.3/autorag/nodes/queryexpansion/query_decompose.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/queryexpansion/run.py` & `autorag-0.1.3/autorag/nodes/queryexpansion/run.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/retrieval/base.py` & `autorag-0.1.3/autorag/nodes/retrieval/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
                 logger.error(f"embedding_model_str {embedding_model_str} does not exist.")
                 raise KeyError(f"embedding_model_str {embedding_model_str} does not exist.")
             ids, scores = func(queries=queries, collection=chroma_collection,
                                embedding_model=embedding_model, **kwargs)
             del embedding_model
             if torch.cuda.is_available():
                 torch.cuda.empty_cache()
-        elif func.__name__ in ["hybrid_rrf", "hybrid_cc"]:
+        elif func.__name__ in ["hybrid_rrf", "hybrid_cc", "hybrid_rsf", "hybrid_dbsf"]:
             if 'ids' in kwargs and 'scores' in kwargs:
                 ids, scores = func(**kwargs)
             else:
                 if not ('target_modules' in kwargs and 'target_module_params' in kwargs):
                     raise ValueError(
                         f"If there are no ids and scores specified, target_modules and target_module_params must be specified for using {func.__name__}.")
                 target_modules = kwargs.pop('target_modules')
```

### Comparing `AutoRAG-0.1.2/autorag/nodes/retrieval/bm25.py` & `autorag-0.1.3/autorag/nodes/retrieval/bm25.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/retrieval/hybrid_cc.py` & `autorag-0.1.3/autorag/nodes/retrieval/hybrid_cc.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/retrieval/hybrid_rrf.py` & `autorag-0.1.3/autorag/nodes/retrieval/hybrid_rrf.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/nodes/retrieval/run.py` & `autorag-0.1.3/autorag/nodes/retrieval/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             **{metric: list(map(lambda result: result[metric].mean(), result)) for metric in
                strategies.get('metrics')},
         })
         summary_df.to_csv(os.path.join(save_dir, 'summary.csv'), index=False)
         return result, average_times, summary_df
 
     # run retrieval modules except hybrid
-    hybrid_module_names = ['hybrid_rrf', 'hybrid_cc']
+    hybrid_module_names = ['hybrid_rrf', 'hybrid_cc', 'hybrid_rsf', 'hybrid_dbsf']
     filename_first = 0
     if any([module.__name__ not in hybrid_module_names for module in modules]):
         non_hybrid_modules, non_hybrid_module_params = zip(*filter(lambda x: x[0].__name__ not in hybrid_module_names,
                                                                    zip(modules, module_params)))
         non_hybrid_results, non_hybrid_times, non_hybrid_summary_df = run_and_save(non_hybrid_modules,
                                                                                    non_hybrid_module_params, filename_first)
         filename_first += len(non_hybrid_modules)
```

### Comparing `AutoRAG-0.1.2/autorag/nodes/retrieval/vectordb.py` & `autorag-0.1.3/autorag/nodes/retrieval/vectordb.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/schema/module.py` & `autorag-0.1.3/autorag/schema/module.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/schema/node.py` & `autorag-0.1.3/autorag/schema/node.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/strategy.py` & `autorag-0.1.3/autorag/strategy.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/support.py` & `autorag-0.1.3/autorag/support.py`

 * *Files 23% similar despite different names*

```diff
@@ -19,26 +19,34 @@
         'hyde': ('autorag.nodes.queryexpansion', 'hyde'),
         'pass_query_expansion': ('autorag.nodes.queryexpansion', 'pass_query_expansion'),
         # retrieval
         'bm25': ('autorag.nodes.retrieval', 'bm25'),
         'vectordb': ('autorag.nodes.retrieval', 'vectordb'),
         'hybrid_rrf': ('autorag.nodes.retrieval', 'hybrid_rrf'),
         'hybrid_cc': ('autorag.nodes.retrieval', 'hybrid_cc'),
+        'hybrid_rsf': ('autorag.nodes.retrieval', 'hybrid_rsf'),
+        'hybrid_dbsf': ('autorag.nodes.retrieval', 'hybrid_dbsf'),
         # passage_reranker
         'monot5': ('autorag.nodes.passagereranker', 'monot5'),
         'tart': ('autorag.nodes.passagereranker', 'tart'),
         'upr': ('autorag.nodes.passagereranker', 'upr'),
         'koreranker': ('autorag.nodes.passagereranker', 'koreranker'),
         'pass_reranker': ('autorag.nodes.passagereranker', 'pass_reranker'),
         'cohere_reranker': ('autorag.nodes.passagereranker', 'cohere_reranker'),
         'rankgpt': ('autorag.nodes.passagereranker', 'rankgpt'),
         'jina_reranker': ('autorag.nodes.passagereranker', 'jina_reranker'),
         'colbert_reranker': ('autorag.nodes.passagereranker', 'colbert_reranker'),
         'sentence_transformer_reranker': ('autorag.nodes.passagereranker', 'sentence_transformer_reranker'),
         'flag_embedding_reranker': ('autorag.nodes.passagereranker', 'flag_embedding_reranker'),
+        'flag_embedding_llm_reranker': ('autorag.nodes.passagereranker', 'flag_embedding_llm_reranker'),
+        'time_reranker': ('autorag.nodes.passagereranker', 'time_reranker'),
+        # passage_filter
+        'pass_passage_filter': ('autorag.nodes.passagefilter', 'pass_passage_filter'),
+        'similarity_threshold_cutoff': ('autorag.nodes.passagefilter', 'similarity_threshold_cutoff'),
+        'similarity_percentile_cutoff': ('autorag.nodes.passagefilter', 'similarity_percentile_cutoff'),
         # passage_compressor
         'tree_summarize': ('autorag.nodes.passagecompressor', 'tree_summarize'),
         'pass_compressor': ('autorag.nodes.passagecompressor', 'pass_compressor'),
         # prompt_maker
         'fstring': ('autorag.nodes.promptmaker', 'fstring'),
         'long_context_reorder': ('autorag.nodes.promptmaker', 'long_context_reorder'),
         # generator
@@ -50,11 +58,12 @@
 
 def get_support_nodes(node_name: str) -> Callable:
     support_nodes = {
         'query_expansion': ('autorag.nodes.queryexpansion.run', 'run_query_expansion_node'),
         'retrieval': ('autorag.nodes.retrieval.run', 'run_retrieval_node'),
         'generator': ('autorag.nodes.generator.run', 'run_generator_node'),
         'prompt_maker': ('autorag.nodes.promptmaker.run', 'run_prompt_maker_node'),
+        'passage_filter': ('autorag.nodes.passagefilter.run', 'run_passage_filter_node'),
         'passage_compressor': ('autorag.nodes.passagecompressor.run', 'run_passage_compressor_node'),
         'passage_reranker': ('autorag.nodes.passagereranker.run', 'run_passage_reranker_node'),
     }
     return dynamically_find_function(node_name, support_nodes)
```

### Comparing `AutoRAG-0.1.2/autorag/utils/preprocess.py` & `autorag-0.1.3/autorag/utils/preprocess.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/autorag/utils/util.py` & `autorag-0.1.3/autorag/utils/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 
 import pandas as pd
 import tiktoken
 
 logger = logging.getLogger("AutoRAG")
 
 
-def fetch_contents(corpus_data: pd.DataFrame, ids: List[List[str]]) -> List[List[str]]:
+def fetch_contents(corpus_data: pd.DataFrame, ids: List[List[str]],
+                   column_name: str = 'contents') -> List[List[Any]]:
     flat_ids = itertools.chain.from_iterable(ids)
-    contents = list(map(lambda x: corpus_data.loc[lambda row: row['doc_id'] == x]['contents'].values[0], flat_ids))
+    contents = list(map(lambda x: corpus_data.loc[lambda row: row['doc_id'] == x][column_name].values[0], flat_ids))
 
     result = []
     idx = 0
     for sublist in ids:
         result.append(contents[idx:idx + len(sublist)])
         idx += len(sublist)
 
@@ -262,7 +263,16 @@
         tokens = tokenizer.encode(text)
         if len(tokens) <= limit:
             return text
         truncated_text = tokenizer.decode(tokens[:limit])
         return truncated_text
 
     return list(map(lambda x: truncate_text(x, token_limit, tokenizer), texts))
+
+
+def reconstruct_list(flat_list: List[Any], lengths: List[int]) -> List[List[Any]]:
+    result = []
+    start = 0
+    for length in lengths:
+        result.append(flat_list[start:start + length])
+        start += length
+    return result
```

### Comparing `AutoRAG-0.1.2/autorag/web.py` & `autorag-0.1.3/autorag/web.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/Makefile` & `autorag-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/make.bat` & `autorag-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/_static/data_creation.png` & `autorag-0.1.3/docs/source/_static/data_creation.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/_static/data_folder.png` & `autorag-0.1.3/docs/source/_static/data_folder.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/_static/node_folder.png` & `autorag-0.1.3/docs/source/_static/node_folder.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/_static/node_line_folder.png` & `autorag-0.1.3/docs/source/_static/node_line_folder.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/_static/node_line_summary.png` & `autorag-0.1.3/docs/source/_static/node_line_summary.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/_static/node_lines.png` & `autorag-0.1.3/docs/source/_static/node_lines.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/_static/node_summary.png` & `autorag-0.1.3/docs/source/_static/node_summary.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/_static/project_folder_example.png` & `autorag-0.1.3/docs/source/_static/project_folder_example.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/_static/project_folders.png` & `autorag-0.1.3/docs/source/_static/project_folders.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/_static/resources_folder.png` & `autorag-0.1.3/docs/source/_static/resources_folder.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/_static/roadmap/RAG_paradigms.png` & `autorag-0.1.3/docs/source/_static/roadmap/RAG_paradigms.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/_static/roadmap/advanced_RAG.png` & `autorag-0.1.3/docs/source/_static/roadmap/advanced_RAG.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/_static/roadmap/cycle.png` & `autorag-0.1.3/docs/source/_static/roadmap/cycle.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/_static/roadmap/merger.png` & `autorag-0.1.3/docs/source/_static/roadmap/merger.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/_static/roadmap/node_line_modular.png` & `autorag-0.1.3/docs/source/_static/roadmap/node_line_modular.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/_static/roadmap/policy.png` & `autorag-0.1.3/docs/source/_static/roadmap/policy.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/_static/samsung_sundae.jpeg` & `autorag-0.1.3/docs/source/_static/samsung_sundae.jpeg`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/_static/trial_folder.png` & `autorag-0.1.3/docs/source/_static/trial_folder.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/_static/trial_json.png` & `autorag-0.1.3/docs/source/_static/trial_json.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/_static/trial_summary.png` & `autorag-0.1.3/docs/source/_static/trial_summary.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/_static/web_interface.png` & `autorag-0.1.3/docs/source/_static/web_interface.png`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/api_spec/autorag.data.corpus.rst` & `autorag-0.1.3/docs/source/api_spec/autorag.data.corpus.rst`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/api_spec/autorag.data.qacreation.rst` & `autorag-0.1.3/docs/source/api_spec/autorag.data.qacreation.rst`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,22 @@
 -------------------------------------------
 
 .. automodule:: autorag.data.qacreation.llama_index
    :members:
    :undoc-members:
    :show-inheritance:
 
+autorag.data.qacreation.ragas module
+------------------------------------
+
+.. automodule:: autorag.data.qacreation.ragas
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 autorag.data.qacreation.simple module
 -------------------------------------
 
 .. automodule:: autorag.data.qacreation.simple
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `AutoRAG-0.1.2/docs/source/api_spec/autorag.evaluate.metric.rst` & `autorag-0.1.3/docs/source/api_spec/autorag.evaluate.metric.rst`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/api_spec/autorag.evaluate.rst` & `autorag-0.1.3/docs/source/api_spec/autorag.evaluate.rst`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.generator.rst` & `autorag-0.1.3/docs/source/api_spec/autorag.nodes.generator.rst`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.passagecompressor.rst` & `autorag-0.1.3/docs/source/api_spec/autorag.nodes.passagecompressor.rst`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.passagereranker.rst` & `autorag-0.1.3/docs/source/api_spec/autorag.nodes.passagereranker.rst`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,22 @@
 ----------------------------------------------------
 
 .. automodule:: autorag.nodes.passagereranker.flag_embedding
    :members:
    :undoc-members:
    :show-inheritance:
 
+autorag.nodes.passagereranker.flag\_embedding\_llm module
+---------------------------------------------------------
+
+.. automodule:: autorag.nodes.passagereranker.flag_embedding_llm
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 autorag.nodes.passagereranker.jina module
 -----------------------------------------
 
 .. automodule:: autorag.nodes.passagereranker.jina
    :members:
    :undoc-members:
    :show-inheritance:
@@ -96,14 +104,22 @@
 ----------------------------------------------------------
 
 .. automodule:: autorag.nodes.passagereranker.sentence_transformer
    :members:
    :undoc-members:
    :show-inheritance:
 
+autorag.nodes.passagereranker.time\_reranker module
+---------------------------------------------------
+
+.. automodule:: autorag.nodes.passagereranker.time_reranker
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 autorag.nodes.passagereranker.upr module
 ----------------------------------------
 
 .. automodule:: autorag.nodes.passagereranker.upr
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst` & `autorag-0.1.3/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.promptmaker.rst` & `autorag-0.1.3/docs/source/api_spec/autorag.nodes.promptmaker.rst`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.queryexpansion.rst` & `autorag-0.1.3/docs/source/api_spec/autorag.nodes.queryexpansion.rst`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/api_spec/autorag.nodes.retrieval.rst` & `autorag-0.1.3/docs/source/api_spec/autorag.nodes.retrieval.rst`

 * *Files 2% similar despite different names*

```diff
@@ -24,22 +24,38 @@
 -----------------------------------------
 
 .. automodule:: autorag.nodes.retrieval.hybrid_cc
    :members:
    :undoc-members:
    :show-inheritance:
 
+autorag.nodes.retrieval.hybrid\_dbsf module
+-------------------------------------------
+
+.. automodule:: autorag.nodes.retrieval.hybrid_dbsf
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 autorag.nodes.retrieval.hybrid\_rrf module
 ------------------------------------------
 
 .. automodule:: autorag.nodes.retrieval.hybrid_rrf
    :members:
    :undoc-members:
    :show-inheritance:
 
+autorag.nodes.retrieval.hybrid\_rsf module
+------------------------------------------
+
+.. automodule:: autorag.nodes.retrieval.hybrid_rsf
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 autorag.nodes.retrieval.run module
 ----------------------------------
 
 .. automodule:: autorag.nodes.retrieval.run
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `AutoRAG-0.1.2/docs/source/api_spec/autorag.rst` & `autorag-0.1.3/docs/source/api_spec/autorag.rst`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/conf.py` & `autorag-0.1.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/data_creation/data_format.md` & `autorag-0.1.3/docs/source/data_creation/data_format.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/data_creation/tutorial.md` & `autorag-0.1.3/docs/source/data_creation/tutorial.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/deploy/api_endpoint.md` & `autorag-0.1.3/docs/source/deploy/api_endpoint.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/deploy/web.md` & `autorag-0.1.3/docs/source/deploy/web.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/index.rst` & `autorag-0.1.3/docs/source/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 .. toctree::
    :maxdepth: 2
    :caption: Data Creation
    :hidden:
 
    data_creation/tutorial.md
    data_creation/data_format.md
+   data_creation/ragas.md
 
 
 .. toctree::
    :maxdepth: 2
    :caption: Optimization
    :hidden:
 
@@ -97,14 +98,15 @@
    nodes/index.md
    nodes/query_expansion/query_expansion.md
    nodes/retrieval/retrieval.md
    nodes/passage_reranker/passage_reranker.md
    nodes/passage_compressor/passage_compressor.md
    nodes/prompt_maker/prompt_maker.md
    nodes/generator/generator.md
+   nodes/passage_filter/passage_filter.md
 
 .. toctree::
    :maxdepth: 2
    :caption: Deploy
    :hidden:
 
    deploy/api_endpoint.md
```

### Comparing `AutoRAG-0.1.2/docs/source/install.md` & `autorag-0.1.3/docs/source/install.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/local_model.md` & `autorag-0.1.3/docs/source/local_model.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,16 @@
   - node_line_name: node_line_1
     nodes:
       - node_type: generator
         modules:
           - module_type: llama_index_llm
             llm: openailike
             model: mistralai/Mistral-7B-Instruct-v0.2
+            api_base: your_api_base
+            api_key: your_api_key
 ```
 
 At the above example, you can see `model` parameter.
 This is the parameter for the LLM model.
 You can set the model parameter for LlamaIndex LLM initialization.
 The most frequently used parameters are `model`, `max_token`, and `temperature`.
 Please check what you can set for the model parameter
```

### Comparing `AutoRAG-0.1.2/docs/source/nodes/generator/generator.md` & `autorag-0.1.3/docs/source/nodes/generator/generator.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/nodes/generator/llama_index_llm.md` & `autorag-0.1.3/docs/source/nodes/generator/llama_index_llm.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/nodes/generator/vllm.md` & `autorag-0.1.3/docs/source/nodes/generator/vllm.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/nodes/passage_compressor/passage_compressor.md` & `autorag-0.1.3/docs/source/nodes/passage_compressor/passage_compressor.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/nodes/passage_compressor/tree_summarize.md` & `autorag-0.1.3/docs/source/nodes/passage_compressor/tree_summarize.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/nodes/passage_reranker/cohere.md` & `autorag-0.1.3/docs/source/nodes/passage_reranker/cohere.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/nodes/passage_reranker/colbert.md` & `autorag-0.1.3/docs/source/nodes/passage_reranker/colbert.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/nodes/passage_reranker/flag_embedding_reranker.md` & `autorag-0.1.3/docs/source/nodes/passage_reranker/flag_embedding_reranker.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Flag Embedding Reranker
 
-The `flag embedding reranker` module is a reranker using BAAI Reranker model for
+The `flag embedding reranker` module is a reranker using BAAI normal-Reranker model for
 passage reranking.
 
 ## **Module Parameters**
 
 - **batch** : The size of batch. If you have limited CUDA memory, decrease the size of the batch. (default: 64)
 - **model_name** : The type of model you want to use for reranking. Default is "BAAI/bge-reranker-large".
     - you can check model list at [here](https://github.com/FlagOpen/FlagEmbedding)
```

### Comparing `AutoRAG-0.1.2/docs/source/nodes/passage_reranker/jina_reranker.md` & `autorag-0.1.3/docs/source/nodes/passage_reranker/jina_reranker.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/nodes/passage_reranker/monot5.md` & `autorag-0.1.3/docs/source/nodes/passage_reranker/monot5.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/nodes/passage_reranker/passage_reranker.md` & `autorag-0.1.3/docs/source/nodes/passage_reranker/passage_reranker.md`

 * *Files 3% similar despite different names*

```diff
@@ -55,8 +55,10 @@
 koreranker.md
 cohere.md
 rankgpt.md
 jina_reranker.md
 colbert.md
 sentence_transformer_reranker.md
 flag_embedding_reranker.md
+time_reranker.md
+flag_embedding_llm_reranker.md
 ```
```

### Comparing `AutoRAG-0.1.2/docs/source/nodes/passage_reranker/rankgpt.md` & `autorag-0.1.3/docs/source/nodes/passage_reranker/rankgpt.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md` & `autorag-0.1.3/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/nodes/passage_reranker/tart.md` & `autorag-0.1.3/docs/source/nodes/passage_reranker/tart.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/nodes/passage_reranker/upr.md` & `autorag-0.1.3/docs/source/nodes/passage_reranker/upr.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/nodes/prompt_maker/fstring.md` & `autorag-0.1.3/docs/source/nodes/prompt_maker/fstring.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/nodes/prompt_maker/long_context_reorder.md` & `autorag-0.1.3/docs/source/nodes/prompt_maker/long_context_reorder.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/nodes/prompt_maker/prompt_maker.md` & `autorag-0.1.3/docs/source/nodes/prompt_maker/prompt_maker.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/nodes/query_expansion/hyde.md` & `autorag-0.1.3/docs/source/nodes/query_expansion/hyde.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/nodes/query_expansion/query_decompose.md` & `autorag-0.1.3/docs/source/nodes/query_expansion/query_decompose.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/nodes/query_expansion/query_expansion.md` & `autorag-0.1.3/docs/source/nodes/query_expansion/query_expansion.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/nodes/retrieval/bm25.md` & `autorag-0.1.3/docs/source/nodes/retrieval/bm25.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/nodes/retrieval/hybrid_cc.md` & `autorag-0.1.3/docs/source/nodes/retrieval/hybrid_cc.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 The `hybrid-cc` module is designed to retrieve passages from multiple retrievals. Similar to the `hybrid-rrf` module, the `hybrid-cc` module is also aimed at retrieving information from multiple sources.
 
 However, it distinguishes itself by using the Convex Combination (CC) algorithm. 
 This algorithm allows for the calculation of scores with varying weights between each retrieval, offering a flexible approach to combining retrieval scores.
 
 ## ❗️Hybird additional explanation
-By default, `hybrid_rrf` and `hybrid_cc` are designed to be used without writing target_module_params. Other modules listed in target_modules must be included in the config file, and hybrid is calculated based on the best of the results from those modules.
+
+By default, `hybrid` is designed to be used without writing target_module_params. Other modules listed in target_modules
+must be included in the config file, and hybrid is calculated based on the best of the results from those modules.
 
 Once evaluated to find the optimal pipeline, extracting the pipeline creates a parameter called target_module_params. This helps the hybrid work even if you don't include other modules, which is useful in test dataset evaluation and deployment situations.
 
 Also, target_modules and target_module_params must be in the form of a tuple. By default, tuples don't work in yaml files, but AutoRAG specifically uses them. In the AutoRAG config yaml file, a tuple is a tuple of parameters, as opposed to a List, which is a list of options for a parameter that you can try for optimization. Note that because we are using `ast.literal_eval()`, we have to write tuples as if we were writing them in python.
 
 So something like `('bm25', 'vectordb')` with quotes will work.
```

### Comparing `AutoRAG-0.1.2/docs/source/nodes/retrieval/hybrid_rrf.md` & `autorag-0.1.3/docs/source/nodes/retrieval/hybrid_rrf.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Hybrid - rrf
 
 The `hybrid_rrf` module is designed to retrieve passages from multiple retrievals. 
 The `hybrid_rrf` module is tailored for retrieving passages from multiple sources of information. It utilizes the Reciprocal Rank Fusion (RRF) algorithm to calculate final similarity scores. This calculation is based on the ranking of passages in each retrieval, effectively combining retrieval scores from different sources.
 
 ## ❗ Hybird additional explanation
-By default, `hybrid_rrf` and `hybrid_cc` are designed to be used without writing target_module_params. Other modules listed in target_modules must be included in the config YAML file, and hybrid is calculated based on the best of the results from those modules.
+
+By default, `hybrid` is designed to be used without writing target_module_params. Other modules listed in target_modules
+must be included in the config YAML file, and hybrid is calculated based on the best of the results from those modules.
 
 Once evaluated to find the optimal pipeline, extracting the pipeline creates a parameter called target_module_params. This helps the hybrid work even if you don't include other modules, which is useful in test dataset evaluation and deployment situations.
 
 Also, target_modules and target_module_params must be in the form of a tuple. By default, tuples don't work in yaml files, but AutoRAG specifically uses them. In the AutoRAG config YAML file, a tuple is a tuple of parameters, as opposed to a List, which is a list of options for a parameter that you can try for optimization. Note that because we are using `ast.literal_eval()`, we have to write tuples as if we were writing them in python.
 
 So something like `('bm25', 'vectordb')` with quotes will work.
```

### Comparing `AutoRAG-0.1.2/docs/source/nodes/retrieval/retrieval.md` & `autorag-0.1.3/docs/source/nodes/retrieval/retrieval.md`

 * *Files 3% similar despite different names*

```diff
@@ -52,8 +52,10 @@
 ---
 maxdepth: 1
 ---
 bm25.md
 vectordb.md
 hybrid_rrf.md
 hybrid_cc.md
+hybrid_rsf.md
+hybrid_dbsf.md
 ```
```

### Comparing `AutoRAG-0.1.2/docs/source/nodes/retrieval/vectordb.md` & `autorag-0.1.3/docs/source/nodes/retrieval/vectordb.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/optimization/custom_config.md` & `autorag-0.1.3/docs/source/optimization/custom_config.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/optimization/folder_structure.md` & `autorag-0.1.3/docs/source/optimization/folder_structure.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/optimization/optimization.md` & `autorag-0.1.3/docs/source/optimization/optimization.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/optimization/sample_full_config.yaml` & `autorag-0.1.3/docs/source/optimization/sample_full_config.yaml`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/roadmap/modular_rag.md` & `autorag-0.1.3/docs/source/roadmap/modular_rag.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/structure.md` & `autorag-0.1.3/docs/source/structure.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/troubleshooting.md` & `autorag-0.1.3/docs/source/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/docs/source/tutorial.md` & `autorag-0.1.3/docs/source/tutorial.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/pyproject.toml` & `autorag-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/requirements.txt` & `autorag-0.1.3/requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 guidance # for qa data creation
 cohere>=5.0.0a9 # for cohere services
 tokenlog>=0.0.2 # for token logging
 aiohttp # for async http requests
 bert_score # for bert score
 sentence-transformers # for sentence transformer reranker
 FlagEmbedding # for flag embedding reranker
+ragas # evaluation data generation & evaluation
 
 ### LlamaIndex ###
 llama-index>=0.10.1
 llama-index-core>=0.10.1
 # Embeddings
 llama-index-embeddings-openai
 llama-index-embeddings-huggingface
```

### Comparing `AutoRAG-0.1.2/sample_config/compact_local.yaml` & `autorag-0.1.3/sample_config/compact_local.yaml`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/sample_config/compact_openai.yaml` & `autorag-0.1.3/sample_config/compact_openai.yaml`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/sample_config/config_korean.yaml` & `autorag-0.1.3/sample_config/config_korean.yaml`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/sample_config/extracted_sample.yaml` & `autorag-0.1.3/sample_config/extracted_sample.yaml`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/sample_config/full.yaml` & `autorag-0.1.3/tests/resources/full.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -43,21 +43,14 @@
         metrics: [retrieval_f1, retrieval_recall, retrieval_precision]
         speed_threshold: 10
       top_k: 5
       modules:
         - module_type: pass_reranker
         - module_type: tart
         - module_type: monot5
-        - module_type: upr
-        - module_type: cohere_reranker
-        - module_type: rankgpt
-        - module_type: jina_reranker
-        - module_type: colbert_reranker
-        - module_type: sentence_transformer_reranker
-        - module_type: flag_embedding_reranker
     - node_type: passage_compressor
       strategy:
         metrics: [retrieval_token_f1, retrieval_token_recall, retrieval_token_precision]
         speed_threshold: 10
       modules:
         - module_type: pass_compressor
         - module_type: tree_summarize
@@ -65,39 +58,42 @@
           model: gpt-3.5-turbo-16k
 - node_line_name: post_retrieve_node_line  # Arbitrary node line name
   nodes:
     - node_type: prompt_maker
       strategy:
         metrics:
           - metric_name: bleu
+            lowercase: true
           - metric_name: meteor
           - metric_name: rouge
           - metric_name: sem_score
             embedding_model: openai
           - metric_name: g_eval
+            model: gpt-3.5-turbo
         speed_threshold: 10
+        token_threshold: 8000
+        tokenizer: gpt-3.5-turbo
         generator_modules:
           - module_type: llama_index_llm
             llm: openai
             model: [gpt-3.5-turbo-16k, gpt-3.5-turbo-1106]
       modules:
         - module_type: fstring
           prompt: ["Tell me something about the question: {query} \n\n {retrieved_contents}",
                    "Question: {query} \n Something to read: {retrieved_contents} \n What's your answer?"]
-        - module_type: long_context_reorder
-          prompt: [ "Tell me something about the question: {query} \n\n {retrieved_contents}",
-                    "Question: {query} \n Something to read: {retrieved_contents} \n What's your answer?" ]
     - node_type: generator
       strategy:
         metrics:
           - metric_name: bleu
           - metric_name: meteor
           - metric_name: rouge
           - metric_name: sem_score
             embedding_model: openai
           - metric_name: g_eval
+            model: gpt-3.5-turbo
         speed_threshold: 10
+        token_threshold: 2048
       modules:
         - module_type: llama_index_llm
           llm: [openai]
           model: [gpt-3.5-turbo-16k, gpt-3.5-turbo-1106]
           temperature: [0.5, 1.0, 1.5]
```

### Comparing `AutoRAG-0.1.2/sample_config/simple_local.yaml` & `autorag-0.1.3/sample_config/simple_local.yaml`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/sample_config/simple_openai.yaml` & `autorag-0.1.3/sample_config/simple_openai.yaml`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/sample_dataset/README.md` & `autorag-0.1.3/sample_dataset/README.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/sample_dataset/eli5/load_eli5_dataset.py` & `autorag-0.1.3/sample_dataset/eli5/load_eli5_dataset.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/sample_dataset/msmarco/load_msmarco_dataset.py` & `autorag-0.1.3/sample_dataset/msmarco/load_msmarco_dataset.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/sample_dataset/triviaqa/load_triviaqa_dataset.py` & `autorag-0.1.3/sample_dataset/triviaqa/load_triviaqa_dataset.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/data/corpus/test_base.py` & `autorag-0.1.3/tests/autorag/data/corpus/test_base.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/data/corpus/test_langchain.py` & `autorag-0.1.3/tests/autorag/data/corpus/test_langchain.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/data/corpus/test_llama_index_corpus.py` & `autorag-0.1.3/tests/autorag/data/corpus/test_llama_index_corpus.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/data/qacreation/test_base_qacreation.py` & `autorag-0.1.3/tests/autorag/data/qacreation/test_base_qacreation.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/data/qacreation/test_llama_index_qacreation.py` & `autorag-0.1.3/tests/autorag/data/qacreation/test_llama_index_qacreation.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/data/qacreation/test_simple.py` & `autorag-0.1.3/tests/autorag/data/qacreation/test_simple.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/evaluate/metric/test_generation_metric.py` & `autorag-0.1.3/tests/autorag/evaluate/metric/test_generation_metric.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py` & `autorag-0.1.3/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/evaluate/metric/test_retrieval_metric.py` & `autorag-0.1.3/tests/autorag/evaluate/metric/test_retrieval_metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,37 +4,41 @@
 
 from autorag.evaluate.metric import retrieval_f1, retrieval_precision, retrieval_recall
 
 retrieval_gt = [
     [['test-1', 'test-2'], ['test-3']],
     [['test-4', 'test-5'], ['test-6', 'test-7'], ['test-8']],
     [['test-9', 'test-10']],
-    [['test-11'], ['test-12'], ['test-13']]
+    [['test-11'], ['test-12'], ['test-13']],
+    [['test-14']],
+    [['test-15']],
 ]
 
 pred = [
     ['test-1', 'pred-1', 'test-2', 'pred-3'],  # recall: 0.5, precision: 0.5, f1: 0.5
     ['test-6', 'pred-5', 'pred-6', 'pred-7'],  # recall: 1/3, precision: 0.25, f1: 2/7
     ['test-9', 'pred-0', 'pred-8', 'pred-9'],  # recall: 1.0, precision: 0.25, f1: 2/5
     ['test-13', 'test-12', 'pred-10', 'pred-11'],  # recall: 2/3, precision: 0.5, f1: 4/7
+    ['test-14', 'pred-12'],  # recall: 1.0, precision: 0.5, f1: 2/3
+    ['pred-13'],  # recall: 0.0, precision: 0.0, f1: 0.0
 ]
 
 
 def test_retrieval_f1():
-    solution = [0.5, 2 / 7, 2 / 5, 4 / 7]
+    solution = [0.5, 2 / 7, 2 / 5, 4 / 7, 2 / 3, 0.0]
     result = retrieval_f1(retrieval_gt=retrieval_gt, pred_ids=pred)
     for gt, res in zip(solution, result):
         assert math.isclose(gt, res, rel_tol=1e-4)
 
 
 def test_retrieval_recall():
-    solution = [0.5, 1 / 3, 1, 2 / 3]
+    solution = [0.5, 1 / 3, 1, 2 / 3, 1, 0.0]
     result = retrieval_recall(retrieval_gt=retrieval_gt, pred_ids=pred)
     for gt, res in zip(solution, result):
         assert gt == pytest.approx(res, rel=1e-4)
 
 
 def test_retrieval_precision():
-    solution = [0.5, 0.25, 0.25, 0.5]
+    solution = [0.5, 0.25, 0.25, 0.5, 0.5, 0.0]
     result = retrieval_precision(retrieval_gt=retrieval_gt, pred_ids=pred)
     for gt, res in zip(solution, result):
         assert gt == pytest.approx(res, rel=1e-4)
```

### Comparing `AutoRAG-0.1.2/tests/autorag/evaluate/test_evaluate_util.py` & `autorag-0.1.3/tests/autorag/evaluate/test_evaluate_util.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/evaluate/test_generation_evaluate.py` & `autorag-0.1.3/tests/autorag/evaluate/test_generation_evaluate.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/evaluate/test_retrieval_contents_evaluate.py` & `autorag-0.1.3/tests/autorag/evaluate/test_retrieval_contents_evaluate.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/evaluate/test_retrieval_evaluate.py` & `autorag-0.1.3/tests/autorag/evaluate/test_retrieval_evaluate.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/generator/test_generator_base.py` & `autorag-0.1.3/tests/autorag/nodes/generator/test_generator_base.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/generator/test_llama_index_llm.py` & `autorag-0.1.3/tests/autorag/nodes/generator/test_llama_index_llm.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/generator/test_run_generator_node.py` & `autorag-0.1.3/tests/autorag/nodes/generator/test_run_generator_node.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/generator/test_vllm.py` & `autorag-0.1.3/tests/autorag/nodes/generator/test_vllm.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/passagecompressor/test_pass_compressor.py` & `autorag-0.1.3/tests/autorag/nodes/passagecompressor/test_pass_compressor.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py` & `autorag-0.1.3/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/passagecompressor/test_tree_summarize.py` & `autorag-0.1.3/tests/autorag/nodes/passagecompressor/test_tree_summarize.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_cohere_reranker.py` & `autorag-0.1.3/tests/autorag/nodes/passagereranker/test_cohere_reranker.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_colbert_reranker.py` & `autorag-0.1.3/tests/autorag/nodes/passagereranker/test_colbert_reranker.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_flag_embedding.py` & `autorag-0.1.3/tests/autorag/nodes/passagereranker/test_flag_embedding.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_jina_reranker.py` & `autorag-0.1.3/tests/autorag/nodes/passagereranker/test_jina_reranker.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_koreranker.py` & `autorag-0.1.3/tests/autorag/nodes/passagereranker/test_koreranker.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_monot5.py` & `autorag-0.1.3/tests/autorag/nodes/passagereranker/test_monot5.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_pass_reranker.py` & `autorag-0.1.3/tests/autorag/nodes/passagereranker/test_pass_reranker.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py` & `autorag-0.1.3/tests/autorag/nodes/retrieval/test_retrieval_base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,69 @@
 import os
 import pathlib
-from uuid import uuid4
+
+from datetime import datetime
 
 import pandas as pd
 
+from autorag.nodes.retrieval.base import evenly_distribute_passages
+
+queries = [
+    ["What is Visconde structure?", "What are Visconde structure?"],
+    ["What is the structure of StrategyQA dataset in this paper?"],
+    ["What's your favorite source of RAG framework?",
+     "What is your source of RAG framework?",
+     "Is RAG framework have source?"],
+]
+
 root_dir = pathlib.PurePath(os.path.dirname(os.path.realpath(__file__))).parent.parent.parent
 project_dir = os.path.join(root_dir, "resources", "sample_project")
 qa_data = pd.read_parquet(os.path.join(project_dir, "data", "qa.parquet"))
 corpus_data = pd.read_parquet(os.path.join(project_dir, "data", "corpus.parquet"))
-previous_result = qa_data.sample(2)
+previous_result = qa_data.sample(5)
 
-queries_example = ["What is the capital of France?",
-                   "How many members are in Newjeans?"]
-contents_example = [["NomaDamas is Great Team", "Paris is the capital of France.", "havertz is suck at soccer"],
-                    ["i am hungry", "LA is a country in the United States.", "Newjeans has 5 members."]]
-ko_queries_example = ["프랑스의 수도는 어디인가요?",
-                      "뉴진스의 멤버는 몇 명인가요?"]
-ko_contents_example = [["마커AI는 멋진 회사입니다.", "프랑스의 수도는 파리 입니다.", "아스날은 축구를 못합니다."],
-                        ["배고파요", "LA는 미국의 도시입니다.", "뉴진스의 멤버는 5명 입니다."]]
-ids_example = [[str(uuid4()) for _ in range(len(contents_example[0]))],
-               [str(uuid4()) for _ in range(len(contents_example[1]))]]
-scores_example = [[0.1, 0.8, 0.1], [0.1, 0.2, 0.7]]
-f1_example = [0.4, 0.4]
-recall_example = [1.0, 1.0]
-
-previous_result['query'] = queries_example
-previous_result['retrieved_contents'] = contents_example
-previous_result['retrieved_ids'] = ids_example
-previous_result['retrieve_scores'] = scores_example
-previous_result['retrieval_f1'] = f1_example
-previous_result['retrieval_recall'] = recall_example
-
-ko_previous_result = previous_result.copy(deep=True)
-ko_previous_result['query'] = ko_queries_example
-ko_previous_result['retrieved_contents'] = ko_contents_example
-
-
-def base_reranker_test(contents, ids, scores, top_k, use_ko=False):
-    assert len(contents) == len(ids) == len(scores) == 2
-    assert len(contents[0]) == len(ids[0]) == len(scores[0]) == top_k
-    for content_list, id_list, score_list in zip(contents, ids, scores):
-        assert isinstance(content_list, list)
+doc_id = ["doc1", "doc2", "doc3", "doc4", "doc5"]
+contents = ["This is a test document 1.", "This is a test document 2.", "This is a test document 3.",
+            "This is a test document 4.", "This is a test document 5."]
+metadata = [{'datetime': datetime.now()} for _ in range(5)]
+corpus_df = pd.DataFrame({"doc_id": doc_id, "contents": contents, "metadata": metadata})
+
+
+def base_retrieval_test(id_result, score_result, top_k):
+    assert len(id_result) == len(score_result) == 3
+    for id_list, score_list in zip(id_result, score_result):
         assert isinstance(id_list, list)
         assert isinstance(score_list, list)
-        for content, _id, score in zip(content_list, id_list, score_list):
-            assert isinstance(content, str)
+        assert len(id_list) == len(score_list) == top_k
+        for _id, score in zip(id_list, score_list):
             assert isinstance(_id, str)
             assert isinstance(score, float)
         for i in range(1, len(score_list)):
             assert score_list[i - 1] >= score_list[i]
-    if use_ko is True:
-        assert contents[0][0] == "프랑스의 수도는 파리 입니다."
-        assert ids[0][0] in ids_example[0][1]
-        assert contents[1][0] == "뉴진스의 멤버는 5명 입니다."
-        assert ids[1][0] in ids_example[1][2]
-    else:
-        assert contents[0][0] == "Paris is the capital of France."
-        assert ids[0][0] in ids_example[0][1]
-        assert contents[1][0] == "Newjeans has 5 members."
-        assert ids[1][0] in ids_example[1][2]
 
 
-def base_reranker_node_test(result_df, top_k, use_ko=False):
+def base_retrieval_node_test(result_df):
     contents = result_df["retrieved_contents"].tolist()
     ids = result_df["retrieved_ids"].tolist()
     scores = result_df["retrieve_scores"].tolist()
-    base_reranker_test(contents, ids, scores, top_k, use_ko)
+    assert len(contents) == len(ids) == len(scores) == 5
+    assert len(contents[0]) == len(ids[0]) == len(scores[0]) == 4
+    # id is matching with corpus.parquet
+    for content_list, id_list, score_list in zip(contents, ids, scores):
+        for i, (content, _id, score) in enumerate(zip(content_list, id_list, score_list)):
+            assert isinstance(content, str)
+            assert isinstance(_id, str)
+            assert isinstance(score, float)
+            assert _id in corpus_data["doc_id"].tolist()
+            assert content == corpus_data[corpus_data["doc_id"] == _id]["contents"].values[0]
+            if i >= 1:
+                assert score_list[i - 1] >= score_list[i]
+
+
+def test_evenly_distribute_passages():
+    ids = [[f'test-{i}-{j}' for i in range(10)] for j in range(3)]
+    scores = [[i for i in range(10)] for _ in range(3)]
+    top_k = 10
+    new_ids, new_scores = evenly_distribute_passages(ids, scores, top_k)
+    assert len(new_ids) == top_k
+    assert len(new_scores) == top_k
+    assert new_scores == [0, 1, 2, 3, 0, 1, 2, 0, 1, 2]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py` & `autorag-0.1.3/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_rankgpt.py` & `autorag-0.1.3/tests/autorag/nodes/passagereranker/test_rankgpt.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_sentence_transformer.py` & `autorag-0.1.3/tests/autorag/nodes/passagereranker/test_sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_tart.py` & `autorag-0.1.3/tests/autorag/nodes/passagereranker/test_tart.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/passagereranker/test_upr.py` & `autorag-0.1.3/tests/autorag/nodes/passagereranker/test_upr.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/promptmaker/test_fstring.py` & `autorag-0.1.3/tests/autorag/nodes/promptmaker/test_fstring.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/promptmaker/test_long_context_reorder.py` & `autorag-0.1.3/tests/autorag/nodes/promptmaker/test_long_context_reorder.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py` & `autorag-0.1.3/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py` & `autorag-0.1.3/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/queryexpansion/test_hyde.py` & `autorag-0.1.3/tests/autorag/nodes/queryexpansion/test_hyde.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py` & `autorag-0.1.3/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/queryexpansion/test_query_decompose.py` & `autorag-0.1.3/tests/autorag/nodes/queryexpansion/test_query_decompose.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py` & `autorag-0.1.3/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py` & `autorag-0.1.3/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/retrieval/test_bm25.py` & `autorag-0.1.3/tests/autorag/nodes/retrieval/test_bm25.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/retrieval/test_hybrid_rrf.py` & `autorag-0.1.3/tests/autorag/nodes/retrieval/test_hybrid_base.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,52 +3,79 @@
 from datetime import datetime
 
 import chromadb
 import pandas as pd
 import pytest
 from llama_index.embeddings.openai import OpenAIEmbedding
 
-from autorag.nodes.retrieval import hybrid_rrf
 from autorag.nodes.retrieval.bm25 import bm25_ingest
-from autorag.nodes.retrieval.hybrid_rrf import rrf_pure
 from autorag.nodes.retrieval.vectordb import vectordb_ingest
 
+sample_ids = ([
+                  ['id-1', 'id-2', 'id-3'],
+                  ['id-2', 'id-3', 'id-4']
+              ], [
+                  ['id-1', 'id-4', 'id-3'],
+                  ['id-2', 'id-5', 'id-4']
+              ])
+sample_scores = ([
+                     [1, 3, 5],
+                     [2, 4, 6]
+                 ], [
+                     [4, 2, 6],
+                     [5, 3, 7]
+                 ])
+sample_ids_2 = (['id-1', 'id-2', 'id-3', 'id-4', 'id-5'],
+                ['id-1', 'id-4', 'id-3', 'id-5', 'id-2'])
+sample_scores_2 = ([5, 3, 1, 0.4, 0.2], [6, 2, 1, 0.5, 0.1])
+
+sample_ids_3 = ([
+                    ['id-1', 'id-2', 'id-3', 'id-4', 'id-5'],
+                    ['id-2', 'id-3', 'id-4', 'id-5', 'id-6']
+                ], [
+                    ['id-1', 'id-4', 'id-3', 'id-5', 'id-2'],
+                    ['id-2', 'id-5', 'id-4', 'id-6', 'id-3']
+                ])
+sample_scores_3 = ([
+                       [5, 3, 1, 0.4, 0.2],
+                       [6, 4, 2, 1.4, 1.2]
+                   ], [
+                       [6, 2, 1, 0.5, 0.1],
+                       [7, 3, 2, 1.5, 1.1],
+                   ])
 
-def test_hybrid_rrf():
-    sample_ids = ([
-                      ['id-1', 'id-2', 'id-3'],
-                      ['id-2', 'id-3', 'id-4']
-                  ], [
-                      ['id-1', 'id-4', 'id-3'],
-                      ['id-2', 'id-5', 'id-4']
-                  ])
-    sample_scores = ([
-                         [1, 3, 5],
-                         [2, 4, 6]
-                     ], [
-                         [4, 2, 6],
-                         [5, 3, 7]
-                     ])
-    result_id, result_scores = hybrid_rrf.__wrapped__(sample_ids, sample_scores, top_k=3, rrf_k=1)
-    assert result_id == [
-        ['id-3', 'id-1', 'id-2'],
-        ['id-4', 'id-2', 'id-3']
-    ]
-    assert result_scores[0] == pytest.approx([1.0, (1 / 4) + (1 / 3), (1 / 3)])
-    assert result_scores[1] == pytest.approx([1.0, (1 / 4) + (1 / 3), (1 / 3)])
+sample_ids_non_overlap = (['id-1', 'id-2', 'id-3', 'id-4', 'id-5'],
+                          ['id-6', 'id-4', 'id-3', 'id-7', 'id-2'])
 
+previous_result = pd.DataFrame({
+    'qid': ['query-1', 'query-2', 'query-3'],
+    'query': ['query-1', 'query-2', 'query-3'],
+    'retrieval_gt': [
+        [['id-1'], ['id-2'], ['id-3']],
+        [['id-1'], ['id-2'], ['id-3']],
+        [['id-1'], ['id-2'], ['id-3']]
+    ],
+    'generation_gt': [
+        ['gen-1', 'gen-2'],
+        ['gen-1', 'gen-2'],
+        ['gen-1', 'gen-2']
+    ]
+})
 
-def test_rrf_pure():
-    sample_ids = (['id-1', 'id-2', 'id-3'],
-                  ['id-1', 'id-4', 'id-3'])
-    sample_scores = ([1, 3, 5], [4, 2, 6])
-    result_id, result_scores = rrf_pure(sample_ids, sample_scores,
-                                        rrf_k=1, top_k=3)
-    assert result_scores == pytest.approx([1.0, (1 / 4) + (1 / 3), (1 / 3)])
-    assert result_id == ['id-3', 'id-1', 'id-2']
+modules_with_weights = {
+    'ids': ([['id-1', 'id-2', 'id-3', 'id-4', 'id-5'],
+             ['id-1', 'id-2', 'id-3', 'id-4', 'id-5']],
+            [['id-1', 'id-4', 'id-3', 'id-5', 'id-2'],
+             ['id-1', 'id-4', 'id-3', 'id-5', 'id-2']]
+            ),
+    'scores': ([[5, 3, 1, 0.4, 0.2], [5, 3, 1, 0.4, 0.2]],
+               [[6, 2, 1, 0.5, 0.1], [6, 2, 1, 0.5, 0.1]]),
+    'top_k': 3,
+    'weights': (0.3, 0.7)
+}
 
 
 @pytest.fixture
 def pseudo_project_dir():
     with tempfile.TemporaryDirectory() as project_dir:
         corpus_df = pd.DataFrame({
             'doc_id': ['id-1', 'id-2', 'id-3', 'id-4', 'id-5', 'id-6', 'id-7', 'id-8', 'id-9'],
@@ -62,69 +89,16 @@
         bm25_ingest(os.path.join(resource_dir, 'bm25.pkl'), corpus_df)
         chroma_path = os.path.join(resource_dir, 'chroma')
         db = chromadb.PersistentClient(path=chroma_path)
         collection = db.create_collection(name="openai", metadata={"hnsw:space": "cosine"})
         vectordb_ingest(collection, corpus_df, OpenAIEmbedding())
         yield project_dir
 
-previous_result = pd.DataFrame({
-        'qid': ['query-1', 'query-2', 'query-3'],
-        'query': ['query-1', 'query-2', 'query-3'],
-        'retrieval_gt': [
-            [['id-1'], ['id-2'], ['id-3']],
-            [['id-1'], ['id-2'], ['id-3']],
-            [['id-1'], ['id-2'], ['id-3']]
-        ],
-        'generation_gt': [
-            ['gen-1', 'gen-2'],
-            ['gen-1', 'gen-2'],
-            ['gen-1', 'gen-2']
-        ]
-    })
-
-
-def test_hybrid_rrf_node(pseudo_project_dir):
-    modules = {
-        'ids': ([['id-1', 'id-2', 'id-3'],
-                 ['id-1', 'id-2', 'id-3'],
-                 ['id-1', 'id-2', 'id-3']],
-                [['id-7', 'id-8', 'id-9'],
-                ['id-7', 'id-8', 'id-9'],
-                ['id-7', 'id-8', 'id-9']]),
-        'scores': ([
-            [0.1, 0.2, 0.3],
-            [0.1, 0.2, 0.3],
-            [0.1, 0.2, 0.3]
-        ],[
-            [0.5, 0.6, 0.7],
-            [0.5, 0.6, 0.7],
-            [0.5, 0.6, 0.7]
-        ]),
-        'top_k': 3,
-        'rrf_k': 1,
-    }
-    result_df = hybrid_rrf(project_dir=pseudo_project_dir, previous_result=previous_result, **modules)
-    assert len(result_df) == 3
-    assert isinstance(result_df, pd.DataFrame)
-    assert set(result_df.columns) == {'retrieved_contents', 'retrieved_ids', 'retrieve_scores'}
-    assert set(result_df['retrieved_ids'].tolist()[0]) == {'id-9', 'id-3', 'id-2'}
-    assert result_df['retrieve_scores'].tolist()[0] == pytest.approx([0.5, 0.5, 1 / 3])
-    assert set(result_df['retrieved_contents'].tolist()[0]) == {'doc-9', 'doc-3', 'doc-2'}
-
-
-def test_hybrid_rrf_node_deploy(pseudo_project_dir):
-    modules = {
-        'target_modules': ('bm25', 'vectordb'),
-        'target_module_params': [
-            {'top_k': 3},
-            {'embedding_model': 'openai', 'top_k': 3}
-        ],
-        'top_k': 3,
-        'rrf_k': 1,
-    }
-    result_df = hybrid_rrf(project_dir=pseudo_project_dir, previous_result=previous_result, **modules)
-    assert len(result_df) == 3
-    assert isinstance(result_df, pd.DataFrame)
-    assert set(result_df.columns) == {'retrieved_contents', 'retrieved_ids', 'retrieve_scores'}
-    assert len(result_df['retrieved_ids'].tolist()[0]) == 3
-    assert len(result_df['retrieve_scores'].tolist()[0]) == 3
-    assert len(result_df['retrieved_contents'].tolist()[0]) == 3
+
+def base_hybrid_weights_node_test(hybrid_func, pseudo_project_dir, retrieve_scores):
+    result = hybrid_func(project_dir=pseudo_project_dir, previous_result=previous_result, **modules_with_weights)
+    assert len(result) == 2
+    assert isinstance(result, pd.DataFrame)
+    assert set(result.columns) == {'retrieved_contents', 'retrieved_ids', 'retrieve_scores'}
+    assert result['retrieved_ids'].tolist()[0] == ['id-1', 'id-4', 'id-2']
+    assert result['retrieve_scores'].tolist()[0] == pytest.approx(retrieve_scores)
+    assert result['retrieved_contents'].tolist()[0] == ['doc-1', 'doc-4', 'doc-2']
```

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/retrieval/test_run_retrieval_node.py` & `autorag-0.1.3/tests/autorag/nodes/retrieval/test_run_retrieval_node.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/nodes/retrieval/test_vectordb.py` & `autorag-0.1.3/tests/autorag/nodes/retrieval/test_vectordb.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/schema/test_module_schema.py` & `autorag-0.1.3/tests/autorag/schema/test_module_schema.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/schema/test_node_schema.py` & `autorag-0.1.3/tests/autorag/schema/test_node_schema.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/test_cli.py` & `autorag-0.1.3/tests/autorag/test_cli.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/test_deploy.py` & `autorag-0.1.3/tests/autorag/test_deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     os.environ['BM25'] = 'bm25'
     evaluator.start_trial(os.path.join(resource_dir, 'simple.yaml'))
     project_dir = evaluator.project_dir
 
     def runner_test(runner: Runner):
         answer = runner.run('What is the best movie in Korea? Have Korea movie ever won Oscar?',
                             'retrieved_contents')
-        assert len(answer) == 10
+        assert len(answer) == 1
         assert isinstance(answer, list)
         assert isinstance(answer[0], str)
 
     runner = Runner.from_trial_folder(os.path.join(project_dir, '0'))
     runner_test(runner)
     runner_test(runner)
 
@@ -184,10 +184,10 @@
     response = client.post('/run', json={
         'query': 'What is the best movie in Korea? Have Korea movie ever won Oscar?',
         'result_column': 'retrieved_contents'
     })
     assert response.status_code == 200
     assert 'retrieved_contents' in response.json()
     retrieved_contents = response.json()['retrieved_contents']
-    assert len(retrieved_contents) == 10
+    assert len(retrieved_contents) == 1
     assert isinstance(retrieved_contents, list)
     assert isinstance(retrieved_contents[0], str)
```

### Comparing `AutoRAG-0.1.2/tests/autorag/test_evaluator.py` & `autorag-0.1.3/tests/autorag/test_evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 def test_load_node_line(evaluator):
     node_lines = Evaluator._load_node_lines(os.path.join(resource_dir, 'simple.yaml'))
     assert 'retrieve_node_line' in list(node_lines.keys())
     assert node_lines['retrieve_node_line'] is not None
     nodes = node_lines['retrieve_node_line']
     assert isinstance(nodes, list)
-    assert len(nodes) == 1
+    assert len(nodes) == 2
     node = nodes[0]
     assert isinstance(node, Node)
     assert node.node_type == 'retrieval'
     assert node.run_node == run_retrieval_node
     assert node.strategy['metrics'] == ['retrieval_f1', 'retrieval_recall']
     assert node.modules[0].module_type == 'bm25'
     assert node.modules[1].module_type == 'vectordb'
@@ -66,26 +66,28 @@
     assert node.modules[1].module == vectordb
     assert node.modules[2].module == hybrid_rrf
     assert node.modules[0].module_param == {}
     assert node.modules[1].module_param == {'embedding_model': ['openai', 'openai']}
     assert node.modules[2].module_param == {
         'rrf_k': 5, 'target_modules': ('bm25', 'vectordb')
     }
+    assert nodes[1].node_type == 'passage_filter'
 
 
 def test_start_trial(evaluator):
     evaluator.start_trial(os.path.join(resource_dir, 'simple.yaml'))
     project_dir = evaluator.project_dir
     assert os.path.exists(os.path.join(project_dir, '0'))
     assert os.path.exists(os.path.join(project_dir, 'data'))
     assert os.path.exists(os.path.join(project_dir, 'resources'))
     assert os.path.exists(os.path.join(project_dir, 'trial.json'))
     assert os.path.exists(os.path.join(project_dir, '0', 'config.yaml'))
     assert os.path.exists(os.path.join(project_dir, '0', 'retrieve_node_line'))
     assert os.path.exists(os.path.join(project_dir, '0', 'retrieve_node_line', 'retrieval'))
+    assert os.path.exists(os.path.join(project_dir, '0', 'retrieve_node_line', 'passage_filter'))
     assert os.path.exists(os.path.join(project_dir, '0', 'retrieve_node_line', 'retrieval', '0.parquet'))
     assert os.path.exists(os.path.join(project_dir, '0', 'retrieve_node_line', 'retrieval', '1.parquet'))
     expect_each_result_columns = ['retrieved_contents', 'retrieved_ids', 'retrieve_scores', 'retrieval_f1',
                                   'retrieval_recall']
     each_result_bm25 = pd.read_parquet(
         os.path.join(project_dir, '0', 'retrieve_node_line', 'retrieval', '0.parquet'))
     each_result_vectordb = pd.read_parquet(
@@ -98,28 +100,28 @@
     best_result = pd.read_parquet(os.path.join(project_dir, '0', 'retrieve_node_line', 'retrieval', 'best_0.parquet'))
     assert all([expect_column in best_result.columns for expect_column in expect_best_result_columns])
 
     # test node line summary
     node_line_summary_path = os.path.join(project_dir, '0', 'retrieve_node_line', 'summary.csv')
     assert os.path.exists(node_line_summary_path)
     node_line_summary_df = load_summary_file(node_line_summary_path, ["best_module_params"])
-    assert len(node_line_summary_df) == 1
+    assert len(node_line_summary_df) == 2
     assert set(node_line_summary_df.columns) == {'node_type', 'best_module_filename',
                                                  'best_module_name', 'best_module_params', 'best_execution_time'}
     assert node_line_summary_df['node_type'][0] == 'retrieval'
     assert node_line_summary_df['best_module_filename'][0] == '0.parquet'
     assert node_line_summary_df['best_module_name'][0] == 'bm25'
     assert node_line_summary_df['best_module_params'][0] == {'top_k': 10}
     assert node_line_summary_df['best_execution_time'][0] > 0
 
     # test trial summary
     trial_summary_path = os.path.join(project_dir, '0', 'summary.csv')
     assert os.path.exists(trial_summary_path)
     trial_summary_df = load_summary_file(trial_summary_path, ["best_module_params"])
-    assert len(trial_summary_df) == 1
+    assert len(trial_summary_df) == 2
     assert set(trial_summary_df.columns) == {'node_line_name', 'node_type', 'best_module_filename',
                                              'best_module_name', 'best_module_params', 'best_execution_time'}
     assert trial_summary_df['node_line_name'][0] == 'retrieve_node_line'
     assert trial_summary_df['node_type'][0] == 'retrieval'
     assert trial_summary_df['best_module_filename'][0] == '0.parquet'
     assert trial_summary_df['best_module_name'][0] == 'bm25'
     assert trial_summary_df['best_module_params'][0] == {'top_k': 10}
@@ -151,14 +153,16 @@
     retrieval_node_path = os.path.join(retrieval_node_line_path, 'retrieval')
     assert os.path.exists(retrieval_node_path)
     assert all([os.path.exists(os.path.join(retrieval_node_path, f'{i}.parquet')) for i in range(8)])
     assert os.path.exists(os.path.join(project_dir, '0', 'retrieve_node_line', 'passage_reranker'))
     assert os.path.exists(os.path.join(project_dir, '0', 'retrieve_node_line', 'passage_reranker', '0.parquet'))
     assert os.path.exists(os.path.join(project_dir, '0', 'retrieve_node_line', 'passage_reranker', '1.parquet'))
     assert os.path.exists(os.path.join(project_dir, '0', 'retrieve_node_line', 'passage_reranker', '2.parquet'))
+    assert os.path.exists(os.path.join(project_dir, '0', 'retrieve_node_line', 'passage_filter'))
+    assert os.path.exists(os.path.join(project_dir, '0', 'retrieve_node_line', 'passage_filter', '0.parquet'))
     assert os.path.exists(os.path.join(project_dir, '0', 'retrieve_node_line', 'passage_compressor'))
     assert os.path.exists(os.path.join(project_dir, '0', 'retrieve_node_line', 'passage_compressor', '0.parquet'))
     assert os.path.exists(os.path.join(project_dir, '0', 'retrieve_node_line', 'passage_compressor', '1.parquet'))
     # 3. post_retrieve_node_line
     assert os.path.exists(os.path.join(project_dir, '0', 'post_retrieve_node_line'))
     assert os.path.exists(os.path.join(project_dir, '0', 'post_retrieve_node_line', 'prompt_maker'))
     assert os.path.exists(os.path.join(project_dir, '0', 'post_retrieve_node_line', 'prompt_maker', '0.parquet'))
```

### Comparing `AutoRAG-0.1.2/tests/autorag/test_strategy.py` & `autorag-0.1.3/tests/autorag/test_strategy.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/test_web.py` & `autorag-0.1.3/tests/autorag/test_web.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/utils/test_preprocess.py` & `autorag-0.1.3/tests/autorag/utils/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/autorag/utils/test_util.py` & `autorag-0.1.3/tests/autorag/utils/test_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 import itertools
 import os
 import pathlib
 import tempfile
+from datetime import datetime
 
 import pandas as pd
 import pytest
 import tiktoken
 from llama_index.core.llms import CompletionResponse
 
 from autorag.utils import fetch_contents
@@ -52,19 +53,27 @@
     find_contents = fetch_contents(corpus_data, list(map(lambda x: [x], search_rows['doc_id'].tolist())))
     assert len(find_contents) == len(search_rows)
     assert list(itertools.chain.from_iterable(find_contents)) == search_rows['contents'].tolist()
 
     corpus_data = pd.DataFrame({
         'doc_id': ['doc1', 'doc2', 'doc3'],
         'contents': ['apple', 'banana', 'cherry'],
+        'metadata': [{'last_modified_datetime': datetime(2022, 1, 1, 0, 0, 0)},
+                     {'last_modified_datetime': datetime(2022, 1, 2, 0, 0, 0)},
+                     {'last_modified_datetime': datetime(2022, 1, 3, 0, 0, 0)}]
     })
     find_contents = fetch_contents(corpus_data, [['doc3', 'doc1'], ['doc2']])
     assert find_contents[0] == ['cherry', 'apple']
     assert find_contents[1] == ['banana']
 
+    find_metadatas = fetch_contents(corpus_data, [['doc3', 'doc1'], ['doc2']], 'metadata')
+    assert find_metadatas[0] == [{'last_modified_datetime': datetime(2022, 1, 3, 0, 0, 0)},
+                                 {'last_modified_datetime': datetime(2022, 1, 1, 0, 0, 0)}]
+    assert find_metadatas[1] == [{'last_modified_datetime': datetime(2022, 1, 2, 0, 0, 0)}]
+
 
 def test_load_summary_file(summary_path):
     with pytest.raises(ValueError):
         load_summary_file(summary_path)
     df = load_summary_file(summary_path, ['best_module_params'])
     assert df.equals(summary_df)
```

### Comparing `AutoRAG-0.1.2/tests/delete_tests.py` & `autorag-0.1.3/tests/delete_tests.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/mock.py` & `autorag-0.1.3/tests/mock.py`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/README.md` & `autorag-0.1.3/tests/resources/README.md`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/corpus_data_sample.parquet` & `autorag-0.1.3/tests/resources/corpus_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/data_creation/raw_dir/sample1.txt` & `autorag-0.1.3/tests/resources/data_creation/raw_dir/sample1.txt`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/data_creation/raw_dir/sample2.txt` & `autorag-0.1.3/tests/resources/data_creation/raw_dir/sample2.txt`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/data_creation/raw_dir/sample3.txt` & `autorag-0.1.3/tests/resources/data_creation/raw_dir/sample3.txt`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/full.yaml` & `autorag-0.1.3/tests/resources/result_project/1/config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,99 +1,69 @@
 node_lines:
-- node_line_name: pre_retrieve_node_line  # Arbitrary node line name
-  nodes:
-    - node_type: query_expansion
-      strategy:
-        metrics: [retrieval_f1, retrieval_recall, retrieval_precision]
-        speed_threshold: 10
+  - node_line_name: pre_retrieve_node_line  # Arbitrary node line name
+    nodes:
+      - node_type: query_expansion
+        strategy:
+          metrics: [ retrieval_f1, retrieval_recall, retrieval_precision ]
+          speed_threshold: 10
+          top_k: 10
+          retrieval_modules:
+            - module_type: bm25
+            - module_type: vectordb
+              embedding_model: openai
+        modules:
+          - module_type: query_decompose
+            llm: openai
+            temperature: [ 0.2, 1.0 ]
+          - module_type: hyde
+            llm: openai
+            max_token: 64
+  - node_line_name: retrieve_node_line  # Arbitrary node line name
+    nodes:
+      - node_type: retrieval
+        strategy:
+          metrics: [ retrieval_f1, retrieval_recall, retrieval_precision ]
+          speed_threshold: 10
         top_k: 10
-        retrieval_modules:
+        modules:
           - module_type: bm25
           - module_type: vectordb
             embedding_model: openai
-      modules:
-        - module_type: pass_query_expansion
-        - module_type: query_decompose
-          llm: openai
-          temperature: [0.2, 1.0]
-        - module_type: hyde
-          llm: openai
-          max_token: 64
-- node_line_name: retrieve_node_line  # Arbitrary node line name
-  nodes:
-    - node_type: retrieval
-      strategy:
-        metrics: [retrieval_f1, retrieval_recall, retrieval_precision]
-        speed_threshold: 10
-      top_k: 10
-      modules:
-        - module_type: bm25
-        - module_type: vectordb
-          embedding_model: openai
-        - module_type: hybrid_rrf
-          target_modules: ('bm25', 'vectordb')
-          rrf_k: [3, 5, 10]
-        - module_type: hybrid_cc
-          target_modules: ('bm25', 'vectordb')
-          weights:
-            - (0.5, 0.5)
-            - (0.3, 0.7)
-            - (0.7, 0.3)
-    - node_type: passage_reranker
-      strategy:
-        metrics: [retrieval_f1, retrieval_recall, retrieval_precision]
-        speed_threshold: 10
-      top_k: 5
-      modules:
-        - module_type: pass_reranker
-        - module_type: tart
-        - module_type: monot5
-    - node_type: passage_compressor
-      strategy:
-        metrics: [retrieval_token_f1, retrieval_token_recall, retrieval_token_precision]
-        speed_threshold: 10
-      modules:
-        - module_type: pass_compressor
-        - module_type: tree_summarize
-          llm: openai
-          model: gpt-3.5-turbo-16k
-- node_line_name: post_retrieve_node_line  # Arbitrary node line name
-  nodes:
-    - node_type: prompt_maker
-      strategy:
-        metrics:
-          - metric_name: bleu
-            lowercase: true
-          - metric_name: meteor
-          - metric_name: rouge
-          - metric_name: sem_score
-            embedding_model: openai
-          - metric_name: g_eval
-            model: gpt-3.5-turbo
-        speed_threshold: 10
-        token_threshold: 8000
-        tokenizer: gpt-3.5-turbo
-        generator_modules:
-          - module_type: llama_index_llm
+      - node_type: passage_reranker
+        strategy:
+          metrics: [ retrieval_f1, retrieval_recall, retrieval_precision ]
+          speed_threshold: 10
+        top_k: 5
+        modules:
+          - module_type: tart
+          - module_type: monot5
+      - node_type: passage_compressor
+        strategy:
+          metrics: [ retrieval_token_f1, retrieval_token_recall, retrieval_token_precision ]
+          speed_threshold: 10
+        modules:
+          - module_type: tree_summarize
             llm: openai
-            model: [gpt-3.5-turbo-16k, gpt-3.5-turbo-1106]
-      modules:
-        - module_type: fstring
-          prompt: ["Tell me something about the question: {query} \n\n {retrieved_contents}",
-                   "Question: {query} \n Something to read: {retrieved_contents} \n What's your answer?"]
-    - node_type: generator
-      strategy:
-        metrics:
-          - metric_name: bleu
-          - metric_name: meteor
-          - metric_name: rouge
-          - metric_name: sem_score
-            embedding_model: openai
-          - metric_name: g_eval
-            model: gpt-3.5-turbo
-        speed_threshold: 10
-        token_threshold: 2048
-      modules:
-        - module_type: llama_index_llm
-          llm: [openai]
-          model: [gpt-3.5-turbo-16k, gpt-3.5-turbo-1106]
-          temperature: [0.5, 1.0, 1.5]
+            model: gpt-3.5-turbo-16k
+  - node_line_name: post_retrieve_node_line  # Arbitrary node line name
+    nodes:
+      - node_type: prompt_maker
+        strategy:
+          metrics: [ bleu, meteor, rouge ]
+          speed_threshold: 10
+          generator_modules:
+            - module_type: llama_index_llm
+              llm: openai
+              model: [ gpt-3.5-turbo-16k, gpt-3.5-turbo-1106 ]
+        modules:
+          - module_type: fstring
+            prompt: [ "Tell me something about the question: {query} \n\n {retrieved_contents}",
+                      "Question: {query} \n Something to read: {retrieved_contents} \n What's your answer?" ]
+      - node_type: generator
+        strategy:
+          metrics: [ bleu, meteor, rouge ]
+          speed_threshold: 10
+        modules:
+          - module_type: llama_index_llm
+            llm: [ openai ]
+            model: [ gpt-3.5-turbo-16k, gpt-3.5-turbo-1106 ]
+            temperature: [ 0.5, 1.0, 1.5 ]
```

### Comparing `AutoRAG-0.1.2/tests/resources/qa_data_sample.parquet` & `autorag-0.1.3/tests/resources/qa_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/qa_test_data_sample.parquet` & `autorag-0.1.3/tests/resources/qa_test_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/0/config.yaml` & `autorag-0.1.3/tests/resources/result_project/0/config.yaml`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet` & `autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet` & `autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet` & `autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet` & `autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet` & `autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet` & `autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet` & `autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv` & `autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet` & `autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet` & `autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet` & `autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv` & `autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.1.3/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.1.3/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.1.3/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.1.3/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet` & `autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet` & `autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet` & `autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet` & `autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/0/summary.csv` & `autorag-0.1.3/tests/resources/result_project/0/summary.csv`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/1/config.yaml` & `autorag-0.1.3/tests/resources/result_project/2/config.yaml`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.1.3/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.1.3/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.1.3/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.1.3/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet` & `autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet` & `autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet` & `autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet` & `autorag-0.1.3/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.1.3/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.1.3/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.1.3/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.1.3/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet` & `autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet` & `autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet` & `autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet` & `autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/3/config.yaml` & `autorag-0.1.3/tests/resources/result_project/3/config.yaml`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/best.yaml` & `autorag-0.1.3/tests/resources/result_project/best.yaml`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/data/corpus.parquet` & `autorag-0.1.3/tests/resources/result_project/data/corpus.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/data/qa.parquet` & `autorag-0.1.3/tests/resources/result_project/data/qa.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/resources/bm25.pkl` & `autorag-0.1.3/tests/resources/result_project/resources/bm25.pkl`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin` & `autorag-0.1.3/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin` & `autorag-0.1.3/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/result_project/resources/chroma/chroma.sqlite3` & `autorag-0.1.3/tests/resources/result_project/resources/chroma/chroma.sqlite3`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/sample_contents_nqa.csv` & `autorag-0.1.3/tests/resources/sample_contents_nqa.csv`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/sample_project/data/corpus.parquet` & `autorag-0.1.3/tests/resources/sample_project/data/corpus.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/sample_project/data/qa.parquet` & `autorag-0.1.3/tests/resources/sample_project/data/qa.parquet`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/sample_project/resources/bm25.pkl` & `autorag-0.1.3/tests/resources/sample_project/resources/bm25.pkl`

 * *Files identical despite different names*

### Comparing `AutoRAG-0.1.2/tests/resources/test_bm25_retrieval.pkl` & `autorag-0.1.3/tests/resources/test_bm25_retrieval.pkl`

 * *Files identical despite different names*

