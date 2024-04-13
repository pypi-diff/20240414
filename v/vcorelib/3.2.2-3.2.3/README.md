# Comparing `tmp/vcorelib-3.2.2.tar.gz` & `tmp/vcorelib-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcorelib-3.2.2.tar", last modified: Thu Apr  4 04:10:55 2024, max compression
+gzip compressed data, was "vcorelib-3.2.3.tar", last modified: Sat Apr 13 22:02:19 2024, max compression
```

## Comparing `vcorelib-3.2.2.tar` & `vcorelib-3.2.3.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:10:55.850834 vcorelib-3.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 04:09:24.000000 vcorelib-3.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-04 04:10:55.850834 vcorelib-3.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-04 04:09:24.000000 vcorelib-3.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-04 04:09:24.000000 vcorelib-3.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 04:10:55.850834 vcorelib-3.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-04 04:09:24.000000 vcorelib-3.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:10:55.834834 vcorelib-3.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-04 04:09:24.000000 vcorelib-3.2.2/tests/test_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-04 04:09:24.000000 vcorelib-3.2.2/tests/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:10:55.834834 vcorelib-3.2.2/vcorelib/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:10:55.838834 vcorelib-3.2.2/vcorelib/args/
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/args/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/args/newline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:10:55.838834 vcorelib-3.2.2/vcorelib/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/asyncio/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/asyncio/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/dev_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:10:55.838834 vcorelib-3.2.2/vcorelib/dict/
--rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/dict/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/dict/codec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/dict/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/dict/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:10:55.838834 vcorelib-3.2.2/vcorelib/graph/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7436 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/graph/abc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/graph/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/graph/port.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:10:55.842834 vcorelib-3.2.2/vcorelib/io/
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/io/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:10:55.842834 vcorelib-3.2.2/vcorelib/io/arbiter/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/io/arbiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/io/arbiter/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/io/arbiter/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/io/arbiter/directory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:10:55.842834 vcorelib-3.2.2/vcorelib/io/archive/
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/io/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/io/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/io/decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/io/encode.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/io/fifo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/io/file_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/io/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/io/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:10:55.842834 vcorelib-3.2.2/vcorelib/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/logging/args.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/logging/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:10:55.842834 vcorelib-3.2.2/vcorelib/math/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/math/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:10:55.842834 vcorelib-3.2.2/vcorelib/math/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/math/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/math/analysis/average.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/math/analysis/buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:10:55.842834 vcorelib-3.2.2/vcorelib/math/analysis/rate/
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/math/analysis/rate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/math/analysis/rate/limiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/math/analysis/weighted.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/math/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/math/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/math/unit.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:10:55.842834 vcorelib-3.2.2/vcorelib/namespace/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/namespace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/namespace/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/namespace/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:10:55.846834 vcorelib-3.2.2/vcorelib/paths/
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/paths/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/paths/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/paths/find.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/paths/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/paths/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/paths/info_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:10:55.846834 vcorelib-3.2.2/vcorelib/platform/
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/python.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:10:55.846834 vcorelib-3.2.2/vcorelib/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/schemas/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/schemas/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/schemas/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:10:55.846834 vcorelib-3.2.2/vcorelib/script/
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:10:55.846834 vcorelib-3.2.2/vcorelib/target/
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/target/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/target/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/target/expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/target/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:10:55.846834 vcorelib-3.2.2/vcorelib/task/
--rw-r--r--   0 runner    (1001) docker     (127)    11996 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:10:55.846834 vcorelib-3.2.2/vcorelib/task/dict/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/task/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/task/dict/melder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/task/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:10:55.846834 vcorelib-3.2.2/vcorelib/task/subprocess/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/task/subprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/task/subprocess/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:10:55.846834 vcorelib-3.2.2/vcorelib/task/time/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/task/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-04 04:09:24.000000 vcorelib-3.2.2/vcorelib/task/time/sleep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:10:55.850834 vcorelib-3.2.2/vcorelib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-04 04:10:55.000000 vcorelib-3.2.2/vcorelib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-04 04:10:55.000000 vcorelib-3.2.2/vcorelib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 04:10:55.000000 vcorelib-3.2.2/vcorelib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-04 04:10:55.000000 vcorelib-3.2.2/vcorelib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 04:10:55.000000 vcorelib-3.2.2/vcorelib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.243593 vcorelib-3.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-13 22:00:53.000000 vcorelib-3.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-13 22:02:19.243593 vcorelib-3.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-13 22:00:53.000000 vcorelib-3.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-13 22:00:53.000000 vcorelib-3.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 22:02:19.243593 vcorelib-3.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-13 22:00:53.000000 vcorelib-3.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.227593 vcorelib-3.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-13 22:00:53.000000 vcorelib-3.2.3/tests/test_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-13 22:00:53.000000 vcorelib-3.2.3/tests/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.227593 vcorelib-3.2.3/vcorelib/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.231593 vcorelib-3.2.3/vcorelib/args/
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/args/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/args/newline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.231593 vcorelib-3.2.3/vcorelib/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/asyncio/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/asyncio/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.231593 vcorelib-3.2.3/vcorelib/dict/
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/dict/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/dict/codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/dict/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/dict/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.231593 vcorelib-3.2.3/vcorelib/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7436 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/graph/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/graph/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/graph/port.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.231593 vcorelib-3.2.3/vcorelib/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/io/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.235593 vcorelib-3.2.3/vcorelib/io/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/io/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/io/arbiter/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/io/arbiter/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/io/arbiter/directory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.235593 vcorelib-3.2.3/vcorelib/io/archive/
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/io/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/io/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/io/decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/io/encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/io/fifo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/io/file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/io/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/io/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.235593 vcorelib-3.2.3/vcorelib/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/logging/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/logging/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.235593 vcorelib-3.2.3/vcorelib/math/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/math/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.235593 vcorelib-3.2.3/vcorelib/math/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/math/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/math/analysis/average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/math/analysis/buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.235593 vcorelib-3.2.3/vcorelib/math/analysis/rate/
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/math/analysis/rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/math/analysis/rate/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/math/analysis/weighted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/math/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/math/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/math/unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.235593 vcorelib-3.2.3/vcorelib/namespace/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/namespace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/namespace/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/namespace/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.235593 vcorelib-3.2.3/vcorelib/paths/
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/paths/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/paths/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/paths/find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/paths/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/paths/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/paths/info_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.235593 vcorelib-3.2.3/vcorelib/platform/
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.235593 vcorelib-3.2.3/vcorelib/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/schemas/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/schemas/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/schemas/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.235593 vcorelib-3.2.3/vcorelib/script/
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.239593 vcorelib-3.2.3/vcorelib/target/
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/target/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/target/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/target/expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/target/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.239593 vcorelib-3.2.3/vcorelib/task/
+-rw-r--r--   0 runner    (1001) docker     (127)    11996 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.239593 vcorelib-3.2.3/vcorelib/task/dict/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/task/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/task/dict/melder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/task/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.239593 vcorelib-3.2.3/vcorelib/task/subprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/task/subprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/task/subprocess/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.239593 vcorelib-3.2.3/vcorelib/task/time/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/task/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-13 22:00:53.000000 vcorelib-3.2.3/vcorelib/task/time/sleep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:02:19.239593 vcorelib-3.2.3/vcorelib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-13 22:02:19.000000 vcorelib-3.2.3/vcorelib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-13 22:02:19.000000 vcorelib-3.2.3/vcorelib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 22:02:19.000000 vcorelib-3.2.3/vcorelib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-13 22:02:19.000000 vcorelib-3.2.3/vcorelib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 22:02:19.000000 vcorelib-3.2.3/vcorelib.egg-info/top_level.txt
```

### Comparing `vcorelib-3.2.2/LICENSE` & `vcorelib-3.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/PKG-INFO` & `vcorelib-3.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcorelib
-Version: 3.2.2
+Version: 3.2.3
 Summary: A collection of core Python utilities.
 Home-page: https://github.com/vkottler/vcorelib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -13,20 +13,20 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: ruamel.yaml
-Requires-Dist: tomli-w
-Requires-Dist: cerberus
-Requires-Dist: fastjsonschema
 Requires-Dist: tomli
+Requires-Dist: cerberus
 Requires-Dist: importlib-resources
+Requires-Dist: fastjsonschema
+Requires-Dist: ruamel.yaml
+Requires-Dist: tomli-w
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: isort; extra == "test"
@@ -40,19 +40,19 @@
 Requires-Dist: types-setuptools; extra == "test"
 Requires-Dist: uvloop; (sys_platform != "win32" and sys_platform != "cygwin") and extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=a2a4ea5abcd1abefc7a1528728ba2500
+    hash=f8b97332b3af92a47a234fed499d57a3
     =====================================
 -->
 
-# vcorelib ([3.2.2](https://pypi.org/project/vcorelib/))
+# vcorelib ([3.2.3](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-3.2.2/README.md` & `vcorelib-3.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=a2a4ea5abcd1abefc7a1528728ba2500
+    hash=f8b97332b3af92a47a234fed499d57a3
     =====================================
 -->
 
-# vcorelib ([3.2.2](https://pypi.org/project/vcorelib/))
+# vcorelib ([3.2.3](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-3.2.2/pyproject.toml` & `vcorelib-3.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "vcorelib"
-version = "3.2.2"
+version = "3.2.3"
 description = "A collection of core Python utilities."
 readme = "README.md"
 requires-python = ">=3.11"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `vcorelib-3.2.2/setup.py` & `vcorelib-3.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/tests/test_names.py` & `vcorelib-3.2.3/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/args/__init__.py` & `vcorelib-3.2.3/vcorelib/args/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/args/newline.py` & `vcorelib-3.2.3/vcorelib/args/newline.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/asyncio/__init__.py` & `vcorelib-3.2.3/vcorelib/asyncio/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,25 +54,33 @@
     """Log task exception and return the list of tasks that aren't complete."""
 
     for task in tasks:
         log_task_exception(task, logger=logger)
     return [x for x in tasks if not x.done()]
 
 
+def new_eloop(set_current: bool = True) -> _asyncio.AbstractEventLoop:
+    """Get a new event loop."""
+
+    eloop = _asyncio.new_event_loop()
+    if set_current:
+        _asyncio.set_event_loop(eloop)
+    return eloop
+
+
 def normalize_eloop(
     eloop: _asyncio.AbstractEventLoop = None,
 ) -> _asyncio.AbstractEventLoop:
     """Get the active event loop if one isn't provided explicitly."""
 
     if eloop is None:
         try:
             eloop = _asyncio.get_running_loop()
         except RuntimeError:
-            eloop = _asyncio.new_event_loop()
-            _asyncio.set_event_loop(eloop)
+            eloop = new_eloop()
     return eloop
 
 
 def shutdown_loop(
     eloop: _asyncio.AbstractEventLoop = None, logger: _LoggerType = None
 ) -> None:
     """Attempt to shut down an event loop."""
@@ -89,18 +97,18 @@
             # Give all tasks a chance to complete.
             with _suppress(KeyboardInterrupt, _asyncio.CancelledError):
                 eloop.run_until_complete(task)
                 log_task_exception(task, logger=logger)
 
 
 def run_handle_interrupt(
-    to_run: _Awaitable[_Any],
+    to_run: _Awaitable[T],
     eloop: _asyncio.AbstractEventLoop = None,
     enable_uvloop: bool = True,
-) -> _Optional[_Any]:
+) -> _Optional[T]:
     """
     Run a task in an event loop and gracefully handle keyboard interrupts.
 
     Return the result of the awaitable or None if execution was interrupted.
     """
 
     with try_uvloop_runner(eloop=eloop, enable=enable_uvloop) as loop:
```

### Comparing `vcorelib-3.2.2/vcorelib/asyncio/cli.py` & `vcorelib-3.2.3/vcorelib/asyncio/cli.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/asyncio/subprocess.py` & `vcorelib-3.2.3/vcorelib/asyncio/subprocess.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/dict/__init__.py` & `vcorelib-3.2.3/vcorelib/dict/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/dict/cache.py` & `vcorelib-3.2.3/vcorelib/dict/cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/dict/codec.py` & `vcorelib-3.2.3/vcorelib/dict/codec.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/dict/config.py` & `vcorelib-3.2.3/vcorelib/dict/config.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/dict/env.py` & `vcorelib-3.2.3/vcorelib/dict/env.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/graph/__init__.py` & `vcorelib-3.2.3/vcorelib/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/graph/abc.py` & `vcorelib-3.2.3/vcorelib/graph/abc.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/graph/edge.py` & `vcorelib-3.2.3/vcorelib/graph/edge.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/graph/node.py` & `vcorelib-3.2.3/vcorelib/graph/node.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/graph/port.py` & `vcorelib-3.2.3/vcorelib/graph/port.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/io/__init__.py` & `vcorelib-3.2.3/vcorelib/io/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/io/abc.py` & `vcorelib-3.2.3/vcorelib/io/abc.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/io/arbiter/base.py` & `vcorelib-3.2.3/vcorelib/io/arbiter/base.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/io/arbiter/context.py` & `vcorelib-3.2.3/vcorelib/io/arbiter/context.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/io/arbiter/directory.py` & `vcorelib-3.2.3/vcorelib/io/arbiter/directory.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/io/archive/__init__.py` & `vcorelib-3.2.3/vcorelib/io/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/io/cache.py` & `vcorelib-3.2.3/vcorelib/io/cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/io/decode.py` & `vcorelib-3.2.3/vcorelib/io/decode.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/io/encode.py` & `vcorelib-3.2.3/vcorelib/io/encode.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/io/fifo.py` & `vcorelib-3.2.3/vcorelib/io/fifo.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/io/file_writer.py` & `vcorelib-3.2.3/vcorelib/io/file_writer.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/io/mapping.py` & `vcorelib-3.2.3/vcorelib/io/mapping.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/io/types.py` & `vcorelib-3.2.3/vcorelib/io/types.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/logging/__init__.py` & `vcorelib-3.2.3/vcorelib/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/logging/args.py` & `vcorelib-3.2.3/vcorelib/logging/args.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/logging/time.py` & `vcorelib-3.2.3/vcorelib/logging/time.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/math/__init__.py` & `vcorelib-3.2.3/vcorelib/math/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/math/analysis/average.py` & `vcorelib-3.2.3/vcorelib/math/analysis/average.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/math/analysis/buffer.py` & `vcorelib-3.2.3/vcorelib/math/analysis/buffer.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/math/analysis/rate/__init__.py` & `vcorelib-3.2.3/vcorelib/math/analysis/rate/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/math/analysis/rate/limiter.py` & `vcorelib-3.2.3/vcorelib/math/analysis/rate/limiter.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/math/analysis/weighted.py` & `vcorelib-3.2.3/vcorelib/math/analysis/weighted.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/math/time.py` & `vcorelib-3.2.3/vcorelib/math/time.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/math/unit.py` & `vcorelib-3.2.3/vcorelib/math/unit.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/names.py` & `vcorelib-3.2.3/vcorelib/names.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/namespace/base.py` & `vcorelib-3.2.3/vcorelib/namespace/base.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/namespace/mixin.py` & `vcorelib-3.2.3/vcorelib/namespace/mixin.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/paths/__init__.py` & `vcorelib-3.2.3/vcorelib/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/paths/base.py` & `vcorelib-3.2.3/vcorelib/paths/base.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/paths/context.py` & `vcorelib-3.2.3/vcorelib/paths/context.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/paths/find.py` & `vcorelib-3.2.3/vcorelib/paths/find.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/paths/hashing.py` & `vcorelib-3.2.3/vcorelib/paths/hashing.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/paths/info.py` & `vcorelib-3.2.3/vcorelib/paths/info.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/paths/info_cache.py` & `vcorelib-3.2.3/vcorelib/paths/info_cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/platform/__init__.py` & `vcorelib-3.2.3/vcorelib/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/python.py` & `vcorelib-3.2.3/vcorelib/python.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/schemas/__init__.py` & `vcorelib-3.2.3/vcorelib/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/schemas/base.py` & `vcorelib-3.2.3/vcorelib/schemas/base.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/schemas/json.py` & `vcorelib-3.2.3/vcorelib/schemas/json.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/schemas/mixins.py` & `vcorelib-3.2.3/vcorelib/schemas/mixins.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/script/__init__.py` & `vcorelib-3.2.3/vcorelib/script/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/target/__init__.py` & `vcorelib-3.2.3/vcorelib/target/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/target/evaluation.py` & `vcorelib-3.2.3/vcorelib/target/evaluation.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/target/expression.py` & `vcorelib-3.2.3/vcorelib/target/expression.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/target/resolver.py` & `vcorelib-3.2.3/vcorelib/target/resolver.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/task/__init__.py` & `vcorelib-3.2.3/vcorelib/task/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/task/dict/melder.py` & `vcorelib-3.2.3/vcorelib/task/dict/melder.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/task/manager.py` & `vcorelib-3.2.3/vcorelib/task/manager.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/task/subprocess/run.py` & `vcorelib-3.2.3/vcorelib/task/subprocess/run.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib/task/time/sleep.py` & `vcorelib-3.2.3/vcorelib/task/time/sleep.py`

 * *Files identical despite different names*

### Comparing `vcorelib-3.2.2/vcorelib.egg-info/PKG-INFO` & `vcorelib-3.2.3/vcorelib.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcorelib
-Version: 3.2.2
+Version: 3.2.3
 Summary: A collection of core Python utilities.
 Home-page: https://github.com/vkottler/vcorelib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -13,20 +13,20 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: ruamel.yaml
-Requires-Dist: tomli-w
-Requires-Dist: cerberus
-Requires-Dist: fastjsonschema
 Requires-Dist: tomli
+Requires-Dist: cerberus
 Requires-Dist: importlib-resources
+Requires-Dist: fastjsonschema
+Requires-Dist: ruamel.yaml
+Requires-Dist: tomli-w
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: isort; extra == "test"
@@ -40,19 +40,19 @@
 Requires-Dist: types-setuptools; extra == "test"
 Requires-Dist: uvloop; (sys_platform != "win32" and sys_platform != "cygwin") and extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=a2a4ea5abcd1abefc7a1528728ba2500
+    hash=f8b97332b3af92a47a234fed499d57a3
     =====================================
 -->
 
-# vcorelib ([3.2.2](https://pypi.org/project/vcorelib/))
+# vcorelib ([3.2.3](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-3.2.2/vcorelib.egg-info/SOURCES.txt` & `vcorelib-3.2.3/vcorelib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

