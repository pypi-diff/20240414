# Comparing `tmp/python2verilog-0.5.0.tar.gz` & `tmp/python2verilog-0.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python2verilog-0.5.0.tar", last modified: Sun Apr 14 20:43:26 2024, max compression
+gzip compressed data, was "python2verilog-0.5.0rc1.tar", last modified: Tue Apr  9 23:31:20 2024, max compression
```

## Comparing `python2verilog-0.5.0.tar` & `python2verilog-0.5.0rc1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:43:26.711433 python2verilog-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-14 20:43:16.000000 python2verilog-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-14 20:43:26.711433 python2verilog-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-04-14 20:43:16.000000 python2verilog-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-14 20:43:16.000000 python2verilog-0.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:43:26.703433 python2verilog-0.5.0/python2verilog/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:43:26.703433 python2verilog-0.5.0/python2verilog/api/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/api/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/api/exit_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/api/file_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/api/modes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/api/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     7118 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/api/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/api/verilogify.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:43:26.703433 python2verilog-0.5.0/python2verilog/backend/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:43:26.703433 python2verilog-0.5.0/python2verilog/backend/verilog/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/backend/verilog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14011 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/backend/verilog/ast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/backend/verilog/codegen.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/backend/verilog/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/backend/verilog/fsm.py
--rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/backend/verilog/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/backend/verilog/testbench.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:43:26.703433 python2verilog-0.5.0/python2verilog/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:43:26.707433 python2verilog-0.5.0/python2verilog/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32090 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/frontend/function.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:43:26.707433 python2verilog-0.5.0/python2verilog/ir/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11967 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/ir/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     9365 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/ir/expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10545 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/ir/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/ir/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/ir/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:43:26.707433 python2verilog-0.5.0/python2verilog/optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/optimizer/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/optimizer/increase_work.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:43:26.707433 python2verilog-0.5.0/python2verilog/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/simulation/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/simulation/iverilog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:43:26.707433 python2verilog-0.5.0/python2verilog/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/utils/cytoscape.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/utils/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/utils/fifo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/utils/generics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/utils/lines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/utils/mit_license.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/utils/peek_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/utils/typed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-14 20:43:16.000000 python2verilog-0.5.0/python2verilog/utils/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:43:26.707433 python2verilog-0.5.0/python2verilog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-14 20:43:26.000000 python2verilog-0.5.0/python2verilog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-14 20:43:26.000000 python2verilog-0.5.0/python2verilog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 20:43:26.000000 python2verilog-0.5.0/python2verilog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-14 20:43:26.000000 python2verilog-0.5.0/python2verilog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-14 20:43:26.000000 python2verilog-0.5.0/python2verilog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 20:43:26.711433 python2verilog-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:31:20.770576 python2verilog-0.5.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-04-09 23:31:20.770576 python2verilog-0.5.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:31:20.758576 python2verilog-0.5.0rc1/python2verilog/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:31:20.762576 python2verilog-0.5.0rc1/python2verilog/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/api/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/api/exit_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/api/file_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/api/modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/api/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7118 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/api/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/api/verilogify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:31:20.762576 python2verilog-0.5.0rc1/python2verilog/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:31:20.762576 python2verilog-0.5.0rc1/python2verilog/backend/verilog/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/backend/verilog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14011 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/backend/verilog/ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/backend/verilog/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/backend/verilog/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/backend/verilog/fsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/backend/verilog/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/backend/verilog/testbench.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:31:20.762576 python2verilog-0.5.0rc1/python2verilog/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:31:20.762576 python2verilog-0.5.0rc1/python2verilog/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32090 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/frontend/function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:31:20.762576 python2verilog-0.5.0rc1/python2verilog/ir/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11967 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/ir/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9365 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/ir/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10545 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/ir/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/ir/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/ir/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:31:20.766576 python2verilog-0.5.0rc1/python2verilog/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/optimizer/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/optimizer/increase_work.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:31:20.766576 python2verilog-0.5.0rc1/python2verilog/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/simulation/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/simulation/iverilog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:31:20.766576 python2verilog-0.5.0rc1/python2verilog/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/utils/cytoscape.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/utils/fifo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/utils/generics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/utils/lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/utils/mit_license.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/utils/peek_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/utils/typed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-09 23:31:12.000000 python2verilog-0.5.0rc1/python2verilog/utils/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:31:20.766576 python2verilog-0.5.0rc1/python2verilog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-04-09 23:31:20.000000 python2verilog-0.5.0rc1/python2verilog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-09 23:31:20.000000 python2verilog-0.5.0rc1/python2verilog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:31:20.000000 python2verilog-0.5.0rc1/python2verilog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-09 23:31:20.000000 python2verilog-0.5.0rc1/python2verilog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-09 23:31:20.000000 python2verilog-0.5.0rc1/python2verilog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 23:31:20.770576 python2verilog-0.5.0rc1/setup.cfg
```

### Comparing `python2verilog-0.5.0/LICENSE` & `python2verilog-0.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/PKG-INFO` & `python2verilog-0.5.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python2verilog
-Version: 0.5.0
+Version: 0.5.0rc1
 Summary: Converts a subset of python generator functions into synthesizable sequential SystemVerilog
 Author-email: Kerry Wang <kerrywang369@gmail.com>
 Project-URL: Homepage, https://github.com/WorldofKerry/ToHDL/
 Project-URL: Bug Tracker, https://github.com/WorldofKerry/ToHDL/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
@@ -130,17 +130,13 @@
     - On Ubuntu run `sudo apt install build-essential`
 - /usr/bin/ld: cannot find -lpython3.10: No such file or directory
     - On Ubuntu 22.04 run `sudo apt install libpython3.10-dev`
 
 ## Flamegraph
 
 ```bash
-cargo install flamegraph
-
 sudo apt install linux-tools-common linux-tools-generic linux-tools-`uname -r`
 
 sudo sysctl kernel.perf_event_paranoid=0
 
-CARGO_PROFILE_RELEASE_DEBUG=true cargo flamegraph --unit-test tohdl-tests -- verilog::module::test::odd_fib
-CARGO_PROFILE_RELEASE_DEBUG=true cargo flamegraph --test loops
+CARGO_PROFILE_RELEASE_DEBUG=true cargo flamegraph --unit-test tohdl-codegen -- verilog::module::test::odd_fib
 ```
-Will need to set PERF env var for `flamegraph` if running in WSL from [this stackoverflow answer](https://stackoverflow.com/a/65276025).
```

### Comparing `python2verilog-0.5.0/README.md` & `python2verilog-0.5.0rc1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -96,17 +96,13 @@
     - On Ubuntu run `sudo apt install build-essential`
 - /usr/bin/ld: cannot find -lpython3.10: No such file or directory
     - On Ubuntu 22.04 run `sudo apt install libpython3.10-dev`
 
 ## Flamegraph
 
 ```bash
-cargo install flamegraph
-
 sudo apt install linux-tools-common linux-tools-generic linux-tools-`uname -r`
 
 sudo sysctl kernel.perf_event_paranoid=0
 
-CARGO_PROFILE_RELEASE_DEBUG=true cargo flamegraph --unit-test tohdl-tests -- verilog::module::test::odd_fib
-CARGO_PROFILE_RELEASE_DEBUG=true cargo flamegraph --test loops
+CARGO_PROFILE_RELEASE_DEBUG=true cargo flamegraph --unit-test tohdl-codegen -- verilog::module::test::odd_fib
 ```
-Will need to set PERF env var for `flamegraph` if running in WSL from [this stackoverflow answer](https://stackoverflow.com/a/65276025).
```

### Comparing `python2verilog-0.5.0/pyproject.toml` & `python2verilog-0.5.0rc1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python2verilog"
-version = "0.5.0"
+version = "0.5.0rc1"
 authors = [{ name = "Kerry Wang", email = "kerrywang369@gmail.com" }]
 description = "Converts a subset of python generator functions into synthesizable sequential SystemVerilog"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `python2verilog-0.5.0/python2verilog/__main__.py` & `python2verilog-0.5.0rc1/python2verilog/__main__.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/api/context.py` & `python2verilog-0.5.0rc1/python2verilog/api/context.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,44 +42,39 @@
     """
     Converts a context to a verilog module and testbench
 
     :return: (module, testbench)
     """
     typed(context, ir.Context)
     ver_code_gen, _ = context_to_codegen(context)
-    logging.debug("context_to_verilog")
 
-    try:
-        assert context.is_generator, "Not generator function"
-        assert (
-            context.optimization_level == 0
-        ), "No real optimization exists for Rust backend"
-        generators = []
-        for v in context.namespace.values():
-            if v.is_generator:
-                generators.append(v.name)
-        assert (
-            len(generators) == 1
-        ), f"Only one generator function allowed in namespace {generators}"
-        assert len(context.namespace) <= 4, "Only small namespaces allowed"
-        functions = {
-            k: textwrap.dedent(v.py_string or "") for k, v in context.namespace.items()
-        }
-        module_str = pytohdl.translate(  # pylint: disable=no-member
-            pytohdl.PyContext(context.name, functions)  # pylint: disable=no-member
-        )
-    except AssertionError:
-        module_str = ver_code_gen.get_module_str()
-    except BaseException as e:  # pylint: disable=broad-exception-caught
-        assert "pyo3_runtime" in str(e.__class__), str(e)
+    if context.is_generator and context.optimization_level == 0:
+        try:
+            assert all(
+                v.name == context.name or not v.is_generator
+                for v in context.namespace.values()
+            ), "Only function or generator calling other functions supported"
+
+            functions = {
+                k: textwrap.dedent(v.py_string or "")
+                for k, v in context.namespace.items()
+            }
+            module_str = pytohdl.translate(  # pylint: disable=no-member
+                pytohdl.PyContext(context.name, functions)  # pylint: disable=no-member
+            )
+            # logging.error("Path 1")
+        except BaseException as e:  # pylint: disable=broad-exception-caught
+            module_str = ver_code_gen.get_module_str()
+            logging.info(
+                "Failed to use Rust backend, falling back to Python backend with error: %s",
+                e,
+            )
+    else:
         module_str = ver_code_gen.get_module_str()
-        logging.info(
-            "Failed to use Rust backend, falling back to Python backend with error: %s",
-            e,
-        )
+        # logging.warning("Path 3")
 
     tb_str = ver_code_gen.get_testbench_str(config)
     return module_str, tb_str
 
 
 def context_to_verilog_and_dump(context: ir.Context) -> tuple[str, str, str]:
     """
```

### Comparing `python2verilog-0.5.0/python2verilog/api/exit_handler.py` & `python2verilog-0.5.0rc1/python2verilog/api/exit_handler.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/api/modes.py` & `python2verilog-0.5.0rc1/python2verilog/api/modes.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/api/namespace.py` & `python2verilog-0.5.0rc1/python2verilog/api/namespace.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/api/python.py` & `python2verilog-0.5.0rc1/python2verilog/api/python.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/api/verilogify.py` & `python2verilog-0.5.0rc1/python2verilog/api/verilogify.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/backend/verilog/ast.py` & `python2verilog-0.5.0rc1/python2verilog/backend/verilog/ast.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/backend/verilog/codegen.py` & `python2verilog-0.5.0rc1/python2verilog/backend/verilog/codegen.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/backend/verilog/config.py` & `python2verilog-0.5.0rc1/python2verilog/backend/verilog/config.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/backend/verilog/fsm.py` & `python2verilog-0.5.0rc1/python2verilog/backend/verilog/fsm.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/backend/verilog/module.py` & `python2verilog-0.5.0rc1/python2verilog/backend/verilog/module.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/backend/verilog/testbench.py` & `python2verilog-0.5.0rc1/python2verilog/backend/verilog/testbench.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/exceptions/__init__.py` & `python2verilog-0.5.0rc1/python2verilog/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/frontend/function.py` & `python2verilog-0.5.0rc1/python2verilog/frontend/function.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/ir/__init__.py` & `python2verilog-0.5.0rc1/python2verilog/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/ir/context.py` & `python2verilog-0.5.0rc1/python2verilog/ir/context.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/ir/expressions.py` & `python2verilog-0.5.0rc1/python2verilog/ir/expressions.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/ir/graph.py` & `python2verilog-0.5.0rc1/python2verilog/ir/graph.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/ir/instance.py` & `python2verilog-0.5.0rc1/python2verilog/ir/instance.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/ir/signals.py` & `python2verilog-0.5.0rc1/python2verilog/ir/signals.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/optimizer/helpers.py` & `python2verilog-0.5.0rc1/python2verilog/optimizer/helpers.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/optimizer/increase_work.py` & `python2verilog-0.5.0rc1/python2verilog/optimizer/increase_work.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/simulation/display.py` & `python2verilog-0.5.0rc1/python2verilog/simulation/display.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/simulation/iverilog.py` & `python2verilog-0.5.0rc1/python2verilog/simulation/iverilog.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/utils/cytoscape.py` & `python2verilog-0.5.0rc1/python2verilog/utils/cytoscape.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/utils/decorator.py` & `python2verilog-0.5.0rc1/python2verilog/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/utils/env.py` & `python2verilog-0.5.0rc1/python2verilog/utils/env.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/utils/generics.py` & `python2verilog-0.5.0rc1/python2verilog/utils/generics.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/utils/lines.py` & `python2verilog-0.5.0rc1/python2verilog/utils/lines.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/utils/mit_license.py` & `python2verilog-0.5.0rc1/python2verilog/utils/mit_license.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/utils/peek_counter.py` & `python2verilog-0.5.0rc1/python2verilog/utils/peek_counter.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/utils/typed.py` & `python2verilog-0.5.0rc1/python2verilog/utils/typed.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog/utils/visualization.py` & `python2verilog-0.5.0rc1/python2verilog/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `python2verilog-0.5.0/python2verilog.egg-info/PKG-INFO` & `python2verilog-0.5.0rc1/python2verilog.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python2verilog
-Version: 0.5.0
+Version: 0.5.0rc1
 Summary: Converts a subset of python generator functions into synthesizable sequential SystemVerilog
 Author-email: Kerry Wang <kerrywang369@gmail.com>
 Project-URL: Homepage, https://github.com/WorldofKerry/ToHDL/
 Project-URL: Bug Tracker, https://github.com/WorldofKerry/ToHDL/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
@@ -130,17 +130,13 @@
     - On Ubuntu run `sudo apt install build-essential`
 - /usr/bin/ld: cannot find -lpython3.10: No such file or directory
     - On Ubuntu 22.04 run `sudo apt install libpython3.10-dev`
 
 ## Flamegraph
 
 ```bash
-cargo install flamegraph
-
 sudo apt install linux-tools-common linux-tools-generic linux-tools-`uname -r`
 
 sudo sysctl kernel.perf_event_paranoid=0
 
-CARGO_PROFILE_RELEASE_DEBUG=true cargo flamegraph --unit-test tohdl-tests -- verilog::module::test::odd_fib
-CARGO_PROFILE_RELEASE_DEBUG=true cargo flamegraph --test loops
+CARGO_PROFILE_RELEASE_DEBUG=true cargo flamegraph --unit-test tohdl-codegen -- verilog::module::test::odd_fib
 ```
-Will need to set PERF env var for `flamegraph` if running in WSL from [this stackoverflow answer](https://stackoverflow.com/a/65276025).
```

### Comparing `python2verilog-0.5.0/python2verilog.egg-info/SOURCES.txt` & `python2verilog-0.5.0rc1/python2verilog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

