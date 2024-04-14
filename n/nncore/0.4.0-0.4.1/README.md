# Comparing `tmp/nncore-0.4.0.tar.gz` & `tmp/nncore-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nncore-0.4.0.tar", last modified: Sun Apr  7 04:05:32 2024, max compression
+gzip compressed data, was "nncore-0.4.1.tar", last modified: Sun Apr 14 14:43:50 2024, max compression
```

## Comparing `nncore-0.4.0.tar` & `nncore-0.4.1.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.316973 nncore-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-07 04:05:22.000000 nncore-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-04-07 04:05:32.316973 nncore-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-07 04:05:22.000000 nncore-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.300973 nncore-0.4.0/nncore/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.300973 nncore-0.4.0/nncore/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/dataset/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/dataset/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.300973 nncore-0.4.0/nncore/engine/
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/builder.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9026 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/comm.py
--rw-r--r--   0 runner    (1001) docker     (127)    21687 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.304973 nncore-0.4.0/nncore/engine/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/hooks/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/hooks/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/hooks/closure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/hooks/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/hooks/lr_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/hooks/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/hooks/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/hooks/precise_bn.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/hooks/sampler_seed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/hooks/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11191 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/hooks/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.304973 nncore-0.4.0/nncore/image/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/image/colorspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/image/geometric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/image/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/image/normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.304973 nncore-0.4.0/nncore/io/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.304973 nncore-0.4.0/nncore/io/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/io/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/io/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/io/handlers/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/io/handlers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/io/handlers/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/io/handlers/pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/io/handlers/txt.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/io/handlers/xml.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/io/handlers/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/io/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.308973 nncore-0.4.0/nncore/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.308973 nncore-0.4.0/nncore/nn/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/blocks/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/blocks/conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/blocks/msg_pass.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/blocks/norm.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/blocks/scale.py
--rw-r--r--   0 runner    (1001) docker     (127)    30450 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/blocks/transformer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4505 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.308973 nncore-0.4.0/nncore/nn/bundle/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/bundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/bundle/bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.308973 nncore-0.4.0/nncore/nn/losses/
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/losses/bce.py
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/losses/contrastive.py
--rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/losses/focal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/losses/ghm.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6311 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/losses/lasso.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/losses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.312973 nncore-0.4.0/nncore/nn/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/modules/conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/modules/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/modules/msg_pass.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9821 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.312973 nncore-0.4.0/nncore/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/ops/bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/ops/matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/ops/temporal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.312973 nncore-0.4.0/nncore/optim/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/optim/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/optim/lamb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.312973 nncore-0.4.0/nncore/parallel/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/parallel/collate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/parallel/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/parallel/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.316973 nncore-0.4.0/nncore/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/utils/binder.py
--rw-r--r--   0 runner    (1001) docker     (127)    14654 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/utils/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.316973 nncore-0.4.0/nncore/video/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/video/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.316973 nncore-0.4.0/nncore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-04-07 04:05:32.000000 nncore-0.4.0/nncore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-07 04:05:32.000000 nncore-0.4.0/nncore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 04:05:32.000000 nncore-0.4.0/nncore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-07 04:05:32.000000 nncore-0.4.0/nncore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 04:05:32.000000 nncore-0.4.0/nncore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-07 04:05:32.316973 nncore-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-07 04:05:22.000000 nncore-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.316973 nncore-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-07 04:05:22.000000 nncore-0.4.0/tests/test_binder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-07 04:05:22.000000 nncore-0.4.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-07 04:05:22.000000 nncore-0.4.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-07 04:05:22.000000 nncore-0.4.0/tests/test_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-07 04:05:22.000000 nncore-0.4.0/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-07 04:05:22.000000 nncore-0.4.0/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-07 04:05:22.000000 nncore-0.4.0/tests/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-07 04:05:22.000000 nncore-0.4.0/tests/test_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.131383 nncore-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-14 14:43:42.000000 nncore-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-04-14 14:43:50.131383 nncore-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-04-14 14:43:42.000000 nncore-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.115383 nncore-0.4.1/nncore/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.115383 nncore-0.4.1/nncore/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/dataset/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/dataset/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.115383 nncore-0.4.1/nncore/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/builder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9026 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/comm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21729 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.119383 nncore-0.4.1/nncore/engine/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/hooks/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/hooks/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/hooks/closure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/hooks/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/hooks/lr_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/hooks/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/hooks/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/hooks/precise_bn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/hooks/sampler_seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/hooks/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11191 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/hooks/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.119383 nncore-0.4.1/nncore/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/image/colorspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/image/geometric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/image/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/image/normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.119383 nncore-0.4.1/nncore/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.119383 nncore-0.4.1/nncore/io/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/io/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/io/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/io/handlers/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/io/handlers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/io/handlers/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/io/handlers/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/io/handlers/txt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/io/handlers/xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/io/handlers/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/io/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.123383 nncore-0.4.1/nncore/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.123383 nncore-0.4.1/nncore/nn/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/blocks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/blocks/conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/blocks/msg_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/blocks/norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/blocks/scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30450 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/blocks/transformer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4505 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.123383 nncore-0.4.1/nncore/nn/bundle/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/bundle/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.123383 nncore-0.4.1/nncore/nn/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/losses/bce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/losses/contrastive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/losses/focal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/losses/ghm.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6311 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/losses/lasso.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.123383 nncore-0.4.1/nncore/nn/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/modules/conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/modules/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/modules/msg_pass.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9821 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.123383 nncore-0.4.1/nncore/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/ops/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/ops/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/ops/temporal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.127383 nncore-0.4.1/nncore/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/optim/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/optim/lamb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.127383 nncore-0.4.1/nncore/parallel/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/parallel/collate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/parallel/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/parallel/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.127383 nncore-0.4.1/nncore/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/utils/binder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14654 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/utils/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.127383 nncore-0.4.1/nncore/video/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/video/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.131383 nncore-0.4.1/nncore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-04-14 14:43:50.000000 nncore-0.4.1/nncore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-14 14:43:50.000000 nncore-0.4.1/nncore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 14:43:50.000000 nncore-0.4.1/nncore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-14 14:43:50.000000 nncore-0.4.1/nncore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-14 14:43:50.000000 nncore-0.4.1/nncore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-14 14:43:50.131383 nncore-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-14 14:43:42.000000 nncore-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.131383 nncore-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-14 14:43:42.000000 nncore-0.4.1/tests/test_binder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-14 14:43:42.000000 nncore-0.4.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-14 14:43:42.000000 nncore-0.4.1/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-14 14:43:42.000000 nncore-0.4.1/tests/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-14 14:43:42.000000 nncore-0.4.1/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-14 14:43:42.000000 nncore-0.4.1/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-14 14:43:42.000000 nncore-0.4.1/tests/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-14 14:43:42.000000 nncore-0.4.1/tests/test_registry.py
```

### Comparing `nncore-0.4.0/LICENSE` & `nncore-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/PKG-INFO` & `nncore-0.4.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: nncore
-Version: 0.4.0
+Version: 0.4.1
 Summary: A lightweight machine learning toolkit for researchers.
 Home-page: https://github.com/yeliudev/nncore
 Author: Ye Liu
 Author-email: yeliudev@outlook.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: h5py>=3.1
-Requires-Dist: joblib>=1.1
-Requires-Dist: jsonlines>=2
-Requires-Dist: numpy>=1.19
+Requires-Dist: h5py>=3.10
+Requires-Dist: joblib>=1.3
+Requires-Dist: jsonlines>=4
+Requires-Dist: numpy>=1.26
 Requires-Dist: pyyaml>=6
 Requires-Dist: requests>=2.31
-Requires-Dist: tabulate>=0.8
-Requires-Dist: tensorboard>=2.12
-Requires-Dist: termcolor>=1.1
-Requires-Dist: opencv-python>=4.5
+Requires-Dist: tabulate>=0.9
+Requires-Dist: tensorboard>=2.16
+Requires-Dist: termcolor>=2.4
+Requires-Dist: opencv-python>=4.9
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/yeliudev/nncore/main/.github/logo.svg">
 </p>
 
 <h1 align="center">NNCore</h1>
 
@@ -60,19 +61,19 @@
 
 - Universal I/O APIs
 - Efficient implementations of layers and losses that are not included in PyTorch
 - Extended methods for distributed training
 - More powerful data loading techniques
 - An engine that can take over the whole training and testing process, with all the baby-sitting works (stage control, optimizer configuration, lr scheduling, checkpoint management, metrics & tensorboard writing, etc.) done automatically. See an [example](https://github.com/yeliudev/nncore/blob/main/examples/mnist.py) for details.
 
-Note that some methods in the library work with PyTorch 1.11+, but the installation of PyTorch is not necessary.
+Note that some methods in the library work with PyTorch 2.0+, but the installation of PyTorch is not necessary.
 
 ## Continuous Integration
 
-| Platform / Python Version | 3.8 | 3.9 | 3.10 | 3.11 |
+| Platform / Python Version | 3.9 | 3.10 | 3.11 | 3.12
 | :-: | :-: | :-: | :-: | :-: |
 | Ubuntu 20.04 | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/0?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/1?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/2?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/3?icon=github&cache=300)][link] |
 | Ubuntu 22.04 | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/4?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/5?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/6?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/7?icon=github&cache=300)][link] |
 | macOS 12.x | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/8?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/9?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/10?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/11?icon=github&cache=300)][link] |
 | macOS 13.x | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/12?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/13?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/14?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/15?icon=github&cache=300)][link] |
 | Windows Server 2022 | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/16?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/17?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/18?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/19?icon=github&cache=300)][link] |
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: nncore Version: 0.4.0 Summary: A lightweight
+Metadata-Version: 2.1 Name: nncore Version: 0.4.1 Summary: A lightweight
 machine learning toolkit for researchers. Home-page: https://github.com/
 yeliudev/nncore Author: Ye Liu Author-email: yeliudev@outlook.com License: MIT
 Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Topic :: Utilities Requires-
-Python: >=3.8 Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: h5py>=3.1 Requires-Dist: joblib>=1.1 Requires-Dist: jsonlines>=2
-Requires-Dist: numpy>=1.19 Requires-Dist: pyyaml>=6 Requires-Dist:
-requests>=2.31 Requires-Dist: tabulate>=0.8 Requires-Dist: tensorboard>=2.12
-Requires-Dist: termcolor>=1.1 Requires-Dist: opencv-python>=4.5
+:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Topic :: Utilities Requires-Python: >=3.9
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+h5py>=3.10 Requires-Dist: joblib>=1.3 Requires-Dist: jsonlines>=4 Requires-
+Dist: numpy>=1.26 Requires-Dist: pyyaml>=6 Requires-Dist: requests>=2.31
+Requires-Dist: tabulate>=0.9 Requires-Dist: tensorboard>=2.16 Requires-Dist:
+termcolor>=2.4 Requires-Dist: opencv-python>=4.9
    [https://raw.githubusercontent.com/yeliudev/nncore/main/.github/logo.svg]
                              ************ NNNNCCoorree ************
             AA lliigghhttwweeiigghhtt mmaacchhiinnee lleeaarrnniinngg ttoooollkkiitt ffoorr rreesseeaarrcchheerrss..
   _[_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/_p_y_p_i_/_v_/_n_n_c_o_r_e_?_l_a_b_e_l_=_P_y_P_I_&_c_a_c_h_e_=_3_0_0_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/
 _p_y_p_i_/_d_m_/_n_n_c_o_r_e_?_l_a_b_e_l_=_D_o_w_n_l_o_a_d_s_&_c_o_l_o_r_=_c_y_a_n_&_c_a_c_h_e_=_3_0_0_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/_g_i_t_h_u_b_/
 _l_i_c_e_n_s_e_/_y_e_l_i_u_d_e_v_/_n_n_c_o_r_e_?_l_a_b_e_l_=_L_i_c_e_n_s_e_&_c_a_c_h_e_=_3_0_0_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/_c_o_v_e_r_a_l_l_s_/
   _c_/_g_i_t_h_u_b_/_y_e_l_i_u_d_e_v_/_n_n_c_o_r_e_/_m_a_i_n_?_l_a_b_e_l_=_C_o_v_e_r_a_g_e_&_c_a_c_h_e_=_3_0_0_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/
@@ -26,17 +27,17 @@
 implementations of layers and losses that are not included in PyTorch -
 Extended methods for distributed training - More powerful data loading
 techniques - An engine that can take over the whole training and testing
 process, with all the baby-sitting works (stage control, optimizer
 configuration, lr scheduling, checkpoint management, metrics & tensorboard
 writing, etc.) done automatically. See an [example](https://github.com/
 yeliudev/nncore/blob/main/examples/mnist.py) for details. Note that some
-methods in the library work with PyTorch 1.11+, but the installation of PyTorch
-is not necessary. ## Continuous Integration | Platform / Python Version | 3.8 |
-3.9 | 3.10 | 3.11 | | :-: | :-: | :-: | :-: | :-: | | Ubuntu 20.04 | [![Build]
+methods in the library work with PyTorch 2.0+, but the installation of PyTorch
+is not necessary. ## Continuous Integration | Platform / Python Version | 3.9 |
+3.10 | 3.11 | 3.12 | :-: | :-: | :-: | :-: | :-: | | Ubuntu 20.04 | [![Build]
 (https://badgen.net/runkit/yeliudev/nncore-badge/0?icon=github&cache=300)]
 [link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/
 1?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/
 nncore-badge/2?icon=github&cache=300)][link] | [![Build](https://badgen.net/
 runkit/yeliudev/nncore-badge/3?icon=github&cache=300)][link] | | Ubuntu 22.04 |
 [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/
 4?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/
```

### Comparing `nncore-0.4.0/README.md` & `nncore-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 
 - Universal I/O APIs
 - Efficient implementations of layers and losses that are not included in PyTorch
 - Extended methods for distributed training
 - More powerful data loading techniques
 - An engine that can take over the whole training and testing process, with all the baby-sitting works (stage control, optimizer configuration, lr scheduling, checkpoint management, metrics & tensorboard writing, etc.) done automatically. See an [example](https://github.com/yeliudev/nncore/blob/main/examples/mnist.py) for details.
 
-Note that some methods in the library work with PyTorch 1.11+, but the installation of PyTorch is not necessary.
+Note that some methods in the library work with PyTorch 2.0+, but the installation of PyTorch is not necessary.
 
 ## Continuous Integration
 
-| Platform / Python Version | 3.8 | 3.9 | 3.10 | 3.11 |
+| Platform / Python Version | 3.9 | 3.10 | 3.11 | 3.12
 | :-: | :-: | :-: | :-: | :-: |
 | Ubuntu 20.04 | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/0?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/1?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/2?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/3?icon=github&cache=300)][link] |
 | Ubuntu 22.04 | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/4?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/5?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/6?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/7?icon=github&cache=300)][link] |
 | macOS 12.x | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/8?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/9?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/10?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/11?icon=github&cache=300)][link] |
 | macOS 13.x | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/12?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/13?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/14?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/15?icon=github&cache=300)][link] |
 | Windows Server 2022 | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/16?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/17?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/18?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/19?icon=github&cache=300)][link] |
```

#### html2text {}

```diff
@@ -13,17 +13,17 @@
 implementations of layers and losses that are not included in PyTorch -
 Extended methods for distributed training - More powerful data loading
 techniques - An engine that can take over the whole training and testing
 process, with all the baby-sitting works (stage control, optimizer
 configuration, lr scheduling, checkpoint management, metrics & tensorboard
 writing, etc.) done automatically. See an [example](https://github.com/
 yeliudev/nncore/blob/main/examples/mnist.py) for details. Note that some
-methods in the library work with PyTorch 1.11+, but the installation of PyTorch
-is not necessary. ## Continuous Integration | Platform / Python Version | 3.8 |
-3.9 | 3.10 | 3.11 | | :-: | :-: | :-: | :-: | :-: | | Ubuntu 20.04 | [![Build]
+methods in the library work with PyTorch 2.0+, but the installation of PyTorch
+is not necessary. ## Continuous Integration | Platform / Python Version | 3.9 |
+3.10 | 3.11 | 3.12 | :-: | :-: | :-: | :-: | :-: | | Ubuntu 20.04 | [![Build]
 (https://badgen.net/runkit/yeliudev/nncore-badge/0?icon=github&cache=300)]
 [link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/
 1?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/
 nncore-badge/2?icon=github&cache=300)][link] | [![Build](https://badgen.net/
 runkit/yeliudev/nncore-badge/3?icon=github&cache=300)][link] | | Ubuntu 22.04 |
 [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/
 4?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/
```

### Comparing `nncore-0.4.0/nncore/dataset/builder.py` & `nncore-0.4.1/nncore/dataset/builder.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/dataset/wrapper.py` & `nncore-0.4.1/nncore/dataset/wrapper.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/engine/__init__.py` & `nncore-0.4.1/nncore/engine/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,20 +7,20 @@
                    is_elastic, is_main_process, is_slurm, main_only, sync)
 from .engine import Engine
 from .hooks import (CheckpointHook, ClosureHook, CommandLineWriter,
                     EmptyCacheHook, EvalHook, EventWriterHook, Hook,
                     JSONWriter, LrUpdaterHook, OptimizerHook, PreciseBNHook,
                     SamplerSeedHook, TensorboardWriter, TimerHook, WandbWriter)
 from .utils import (generate_random_seed, get_checkpoint, load_checkpoint,
-                    move_to_device, save_checkpoint, set_random_seed)
+                    save_checkpoint, set_random_seed)
 
 __all__ = [
     'Buffer', 'HOOKS', 'build_dataloader', 'build_hook', 'all_gather',
     'broadcast', 'gather', 'get_dist_info', 'get_launcher', 'get_rank',
     'get_world_size', 'init_dist', 'is_distributed', 'is_elastic',
     'is_main_process', 'is_slurm', 'main_only', 'sync', 'Engine',
     'CheckpointHook', 'ClosureHook', 'CommandLineWriter', 'EmptyCacheHook',
     'EvalHook', 'EventWriterHook', 'Hook', 'JSONWriter', 'LrUpdaterHook',
     'OptimizerHook', 'PreciseBNHook', 'SamplerSeedHook', 'TensorboardWriter',
     'TimerHook', 'WandbWriter', 'generate_random_seed', 'get_checkpoint',
-    'load_checkpoint', 'move_to_device', 'save_checkpoint', 'set_random_seed'
+    'load_checkpoint', 'save_checkpoint', 'set_random_seed'
 ]
```

### Comparing `nncore-0.4.0/nncore/engine/buffer.py` & `nncore-0.4.1/nncore/engine/buffer.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/engine/builder.py` & `nncore-0.4.1/nncore/engine/builder.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/engine/comm.py` & `nncore-0.4.1/nncore/engine/comm.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/engine/engine.py` & `nncore-0.4.1/nncore/engine/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,14 +211,15 @@
                     "types, but got '{}'".format(amp))
             self.amp_cfg = dict(enabled=True, dtype=dtype)
         else:
             self.amp_cfg = dict(enabled=bool(amp))
 
         self.meta = meta
         self.debug = debug
+        self._kwargs = dict()
 
     @property
     def cur_stage(self):
         return self.stages[self._stage]
 
     @property
     def epoch_in_stage(self):
@@ -446,15 +447,14 @@
         for data in self.data_loader:
             self.train_iter(data)
 
         self._call_hook('after_train_epoch')
         self._epoch += 1
 
     def val_epoch(self):
-        self.logger.info('Validating...')
         self._mode = 'val'
         self.model.eval()
         self.buffer.pop('_out', None)
         self.data_loader = self.data_loaders[self._mode]
 
         if callable(getattr(self.data_loader.dataset, 'set_state', None)):
             self.data_loader.dataset.set_state(self._mode)
@@ -463,15 +463,14 @@
 
         for data in nncore.ProgressBar(self.data_loader):
             self.val_iter(data)
 
         self._call_hook('after_val_epoch')
 
     def test_epoch(self):
-        self.logger.info('Evaluating...')
         self._mode = 'test'
         self.model.eval()
         self.buffer.pop('_out', None)
         self.data_loader = self.data_loaders[self._mode]
 
         if callable(getattr(self.data_loader.dataset, 'set_state', None)):
             self.data_loader.dataset.set_state(self._mode)
@@ -502,14 +501,15 @@
         for _ in range(self.cur_stage['epochs'] - self.epoch_in_stage):
             self.train_epoch()
             cfg = self.cur_stage.get('validation')
             if (cfg is not None and 'val' in self.data_loaders
                     and cfg.get('interval', 0) > 0
                     and self.epoch_in_stage > cfg.get('offset', 0)
                     and self.epoch_in_stage % cfg.get('interval', 0) == 0):
+                self.logger.info('Validating...')
                 self.val_epoch()
 
         self._call_hook('after_stage')
         self._stage += 1
 
     def evaluate(self):
         """
@@ -545,14 +545,15 @@
         Args:
             eval (bool, optional): Whether to run evaluation only. Default:
                 ``False``.
         """
         self._kwargs = kwargs
 
         if eval:
+            self.logger.info('Evaluating...')
             self.test_epoch()
             output = self.evaluate()
             self.logger.info(
                 'Evaluation results: ' +
                 ', '.join(['{}: {}'.format(k, v) for k, v in output.items()]))
             return output
```

### Comparing `nncore-0.4.0/nncore/engine/hooks/__init__.py` & `nncore-0.4.1/nncore/engine/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/engine/hooks/base.py` & `nncore-0.4.1/nncore/engine/hooks/base.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/engine/hooks/checkpoint.py` & `nncore-0.4.1/nncore/engine/hooks/checkpoint.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/engine/hooks/closure.py` & `nncore-0.4.1/nncore/engine/hooks/closure.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/engine/hooks/eval.py` & `nncore-0.4.1/nncore/engine/hooks/eval.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
     def after_val_epoch(self, engine):
         if (not self.every_n_epochs(engine, self._interval) or
                 not hasattr(engine.data_loaders['test'].dataset, 'evaluate')):
             return
 
         if self._run_test:
+            engine.logger.info('Evaluating...')
             engine.test_epoch()
 
         output = engine.evaluate()
 
         for key, value in output.items():
             engine.buffer.update(key, value)
```

### Comparing `nncore-0.4.0/nncore/engine/hooks/lr_updater.py` & `nncore-0.4.1/nncore/engine/hooks/lr_updater.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/engine/hooks/memory.py` & `nncore-0.4.1/nncore/engine/hooks/memory.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/engine/hooks/optimizer.py` & `nncore-0.4.1/nncore/engine/hooks/optimizer.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/engine/hooks/precise_bn.py` & `nncore-0.4.1/nncore/engine/hooks/precise_bn.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/engine/hooks/timer.py` & `nncore-0.4.1/nncore/engine/hooks/timer.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/engine/hooks/writer.py` & `nncore-0.4.1/nncore/engine/hooks/writer.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/engine/utils.py` & `nncore-0.4.1/nncore/engine/utils.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/image/__init__.py` & `nncore-0.4.1/nncore/image/__init__.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/image/colorspace.py` & `nncore-0.4.1/nncore/image/colorspace.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/image/geometric.py` & `nncore-0.4.1/nncore/image/geometric.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/image/io.py` & `nncore-0.4.1/nncore/image/io.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/image/normalize.py` & `nncore-0.4.1/nncore/image/normalize.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/io/handlers/base.py` & `nncore-0.4.1/nncore/io/handlers/base.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/io/handlers/hdf5.py` & `nncore-0.4.1/nncore/io/handlers/hdf5.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/io/handlers/json.py` & `nncore-0.4.1/nncore/io/handlers/json.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/io/handlers/numpy.py` & `nncore-0.4.1/nncore/io/handlers/numpy.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/io/handlers/pickle.py` & `nncore-0.4.1/nncore/io/handlers/pickle.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/io/handlers/txt.py` & `nncore-0.4.1/nncore/io/handlers/txt.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/io/handlers/xml.py` & `nncore-0.4.1/nncore/io/handlers/xml.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/io/handlers/yaml.py` & `nncore-0.4.1/nncore/io/handlers/yaml.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/io/io.py` & `nncore-0.4.1/nncore/io/io.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/nn/__init__.py` & `nncore-0.4.1/nncore/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/nn/blocks/__init__.py` & `nncore-0.4.1/nncore/nn/blocks/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) Ye Liu. Licensed under the MIT License.
 
 from .activation import Clamp
 from .conv import *  # noqa
 from .msg_pass import GAT, GCN, SGC
 from .norm import DropPath, drop_path
-from .scale import Scale, Gate
+from .scale import Gate, Scale
 from .transformer import (CrossAttentionLayer, FeedForwardNetwork,
                           MultiHeadAttention, PositionalEncoding,
                           TransformerDecoderLayer, TransformerEncoderLayer)
 
 __all__ = [
     'Clamp', 'GAT', 'GCN', 'SGC', 'DropPath', 'drop_path', 'Scale', 'Gate',
     'CrossAttentionLayer', 'FeedForwardNetwork', 'MultiHeadAttention',
```

### Comparing `nncore-0.4.0/nncore/nn/blocks/activation.py` & `nncore-0.4.1/nncore/nn/blocks/activation.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/nn/blocks/conv.py` & `nncore-0.4.1/nncore/nn/blocks/conv.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/nn/blocks/msg_pass.py` & `nncore-0.4.1/nncore/nn/blocks/msg_pass.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/nn/blocks/norm.py` & `nncore-0.4.1/nncore/nn/blocks/norm.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/nn/blocks/scale.py` & `nncore-0.4.1/nncore/nn/blocks/scale.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/nn/blocks/transformer.py` & `nncore-0.4.1/nncore/nn/blocks/transformer.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/nn/builder.py` & `nncore-0.4.1/nncore/nn/builder.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/nn/bundle/bundle.py` & `nncore-0.4.1/nncore/nn/bundle/bundle.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/nn/init.py` & `nncore-0.4.1/nncore/nn/init.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/nn/losses/__init__.py` & `nncore-0.4.1/nncore/nn/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/nn/losses/bce.py` & `nncore-0.4.1/nncore/nn/losses/bce.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,21 +30,29 @@
         self._pos_weight = pos_weight
         self._loss_weight = loss_weight
 
     def extra_repr(self):
         return "reduction='{}', pos_weight={}, loss_weight={}".format(
             self._reduction, self._pos_weight, self._loss_weight)
 
-    def forward(self, pred, target, weight=None):
+    def forward(self, pred, target, weight=None, avg_factor=None):
         if self._pos_weight is not None:
             pos_weight = pred.new_tensor([self._pos_weight] * pred.size(1))
         else:
             pos_weight = None
 
+        if avg_factor is not None:
+            assert self._reduction == 'mean'
+            reduction = 'sum'
+        else:
+            reduction = self._reduction
+            avg_factor = 1
+
         loss = F.binary_cross_entropy_with_logits(
             pred,
             target,
             weight=weight,
-            reduction=self._reduction,
+            reduction=reduction,
             pos_weight=pos_weight)
+        loss = loss / avg_factor
 
         return loss * self._loss_weight
```

### Comparing `nncore-0.4.0/nncore/nn/losses/contrastive.py` & `nncore-0.4.1/nncore/nn/losses/contrastive.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/nn/losses/focal.py` & `nncore-0.4.1/nncore/nn/losses/focal.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/nn/losses/ghm.py` & `nncore-0.4.1/nncore/nn/losses/ghm.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/nn/losses/lasso.py` & `nncore-0.4.1/nncore/nn/losses/lasso.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/nn/losses/utils.py` & `nncore-0.4.1/nncore/nn/losses/utils.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/nn/modules/conv.py` & `nncore-0.4.1/nncore/nn/modules/conv.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/nn/modules/linear.py` & `nncore-0.4.1/nncore/nn/modules/linear.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/nn/modules/msg_pass.py` & `nncore-0.4.1/nncore/nn/modules/msg_pass.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/nn/utils.py` & `nncore-0.4.1/nncore/nn/utils.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/ops/__init__.py` & `nncore-0.4.1/nncore/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/ops/bbox.py` & `nncore-0.4.1/nncore/ops/bbox.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/ops/matrix.py` & `nncore-0.4.1/nncore/ops/matrix.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/ops/temporal.py` & `nncore-0.4.1/nncore/ops/temporal.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/optim/builder.py` & `nncore-0.4.1/nncore/optim/builder.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/optim/lamb.py` & `nncore-0.4.1/nncore/optim/lamb.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/parallel/collate.py` & `nncore-0.4.1/nncore/parallel/collate.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/parallel/container.py` & `nncore-0.4.1/nncore/parallel/container.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/parallel/parallel.py` & `nncore-0.4.1/nncore/parallel/parallel.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/utils/__init__.py` & `nncore-0.4.1/nncore/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/utils/binder.py` & `nncore-0.4.1/nncore/utils/binder.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/utils/config.py` & `nncore-0.4.1/nncore/utils/config.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/utils/data.py` & `nncore-0.4.1/nncore/utils/data.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/utils/env.py` & `nncore-0.4.1/nncore/utils/env.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/utils/logger.py` & `nncore-0.4.1/nncore/utils/logger.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/utils/misc.py` & `nncore-0.4.1/nncore/utils/misc.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/utils/network.py` & `nncore-0.4.1/nncore/utils/network.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/utils/path.py` & `nncore-0.4.1/nncore/utils/path.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/utils/progress.py` & `nncore-0.4.1/nncore/utils/progress.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 
             if self._num_tasks is not None:
                 perc = self._completed / self._num_tasks
                 eta = int(ela * (1 - perc) / perc + 0.5)
                 eta_str = self._get_time_str(math.ceil(eta))
                 end_str = '\n' if self._num_tasks == self._completed else ''
                 if self._percentage:
-                    msg = self._pb.format(f'{round(perc*100,1)}%', ela_str,
+                    msg = self._pb.format(f'{round(perc*100, 1)}%', ela_str,
                                           eta_str, end_str)
                 else:
                     msg = self._wb.format(self._completed, self._num_tasks,
                                           fps, ela_str, eta_str, end_str)
                 bar_width = self._get_bar_width(msg)
                 mark_width = int(bar_width * perc)
                 chars = '>' * mark_width + ' ' * (bar_width - mark_width)
```

### Comparing `nncore-0.4.0/nncore/utils/registry.py` & `nncore-0.4.1/nncore/utils/registry.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/utils/timer.py` & `nncore-0.4.1/nncore/utils/timer.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore/video/io.py` & `nncore-0.4.1/nncore/video/io.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/nncore.egg-info/PKG-INFO` & `nncore-0.4.1/nncore.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: nncore
-Version: 0.4.0
+Version: 0.4.1
 Summary: A lightweight machine learning toolkit for researchers.
 Home-page: https://github.com/yeliudev/nncore
 Author: Ye Liu
 Author-email: yeliudev@outlook.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: h5py>=3.1
-Requires-Dist: joblib>=1.1
-Requires-Dist: jsonlines>=2
-Requires-Dist: numpy>=1.19
+Requires-Dist: h5py>=3.10
+Requires-Dist: joblib>=1.3
+Requires-Dist: jsonlines>=4
+Requires-Dist: numpy>=1.26
 Requires-Dist: pyyaml>=6
 Requires-Dist: requests>=2.31
-Requires-Dist: tabulate>=0.8
-Requires-Dist: tensorboard>=2.12
-Requires-Dist: termcolor>=1.1
-Requires-Dist: opencv-python>=4.5
+Requires-Dist: tabulate>=0.9
+Requires-Dist: tensorboard>=2.16
+Requires-Dist: termcolor>=2.4
+Requires-Dist: opencv-python>=4.9
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/yeliudev/nncore/main/.github/logo.svg">
 </p>
 
 <h1 align="center">NNCore</h1>
 
@@ -60,19 +61,19 @@
 
 - Universal I/O APIs
 - Efficient implementations of layers and losses that are not included in PyTorch
 - Extended methods for distributed training
 - More powerful data loading techniques
 - An engine that can take over the whole training and testing process, with all the baby-sitting works (stage control, optimizer configuration, lr scheduling, checkpoint management, metrics & tensorboard writing, etc.) done automatically. See an [example](https://github.com/yeliudev/nncore/blob/main/examples/mnist.py) for details.
 
-Note that some methods in the library work with PyTorch 1.11+, but the installation of PyTorch is not necessary.
+Note that some methods in the library work with PyTorch 2.0+, but the installation of PyTorch is not necessary.
 
 ## Continuous Integration
 
-| Platform / Python Version | 3.8 | 3.9 | 3.10 | 3.11 |
+| Platform / Python Version | 3.9 | 3.10 | 3.11 | 3.12
 | :-: | :-: | :-: | :-: | :-: |
 | Ubuntu 20.04 | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/0?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/1?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/2?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/3?icon=github&cache=300)][link] |
 | Ubuntu 22.04 | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/4?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/5?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/6?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/7?icon=github&cache=300)][link] |
 | macOS 12.x | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/8?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/9?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/10?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/11?icon=github&cache=300)][link] |
 | macOS 13.x | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/12?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/13?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/14?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/15?icon=github&cache=300)][link] |
 | Windows Server 2022 | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/16?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/17?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/18?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/19?icon=github&cache=300)][link] |
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: nncore Version: 0.4.0 Summary: A lightweight
+Metadata-Version: 2.1 Name: nncore Version: 0.4.1 Summary: A lightweight
 machine learning toolkit for researchers. Home-page: https://github.com/
 yeliudev/nncore Author: Ye Liu Author-email: yeliudev@outlook.com License: MIT
 Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Topic :: Utilities Requires-
-Python: >=3.8 Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: h5py>=3.1 Requires-Dist: joblib>=1.1 Requires-Dist: jsonlines>=2
-Requires-Dist: numpy>=1.19 Requires-Dist: pyyaml>=6 Requires-Dist:
-requests>=2.31 Requires-Dist: tabulate>=0.8 Requires-Dist: tensorboard>=2.12
-Requires-Dist: termcolor>=1.1 Requires-Dist: opencv-python>=4.5
+:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Topic :: Utilities Requires-Python: >=3.9
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+h5py>=3.10 Requires-Dist: joblib>=1.3 Requires-Dist: jsonlines>=4 Requires-
+Dist: numpy>=1.26 Requires-Dist: pyyaml>=6 Requires-Dist: requests>=2.31
+Requires-Dist: tabulate>=0.9 Requires-Dist: tensorboard>=2.16 Requires-Dist:
+termcolor>=2.4 Requires-Dist: opencv-python>=4.9
    [https://raw.githubusercontent.com/yeliudev/nncore/main/.github/logo.svg]
                              ************ NNNNCCoorree ************
             AA lliigghhttwweeiigghhtt mmaacchhiinnee lleeaarrnniinngg ttoooollkkiitt ffoorr rreesseeaarrcchheerrss..
   _[_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/_p_y_p_i_/_v_/_n_n_c_o_r_e_?_l_a_b_e_l_=_P_y_P_I_&_c_a_c_h_e_=_3_0_0_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/
 _p_y_p_i_/_d_m_/_n_n_c_o_r_e_?_l_a_b_e_l_=_D_o_w_n_l_o_a_d_s_&_c_o_l_o_r_=_c_y_a_n_&_c_a_c_h_e_=_3_0_0_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/_g_i_t_h_u_b_/
 _l_i_c_e_n_s_e_/_y_e_l_i_u_d_e_v_/_n_n_c_o_r_e_?_l_a_b_e_l_=_L_i_c_e_n_s_e_&_c_a_c_h_e_=_3_0_0_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/_c_o_v_e_r_a_l_l_s_/
   _c_/_g_i_t_h_u_b_/_y_e_l_i_u_d_e_v_/_n_n_c_o_r_e_/_m_a_i_n_?_l_a_b_e_l_=_C_o_v_e_r_a_g_e_&_c_a_c_h_e_=_3_0_0_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/
@@ -26,17 +27,17 @@
 implementations of layers and losses that are not included in PyTorch -
 Extended methods for distributed training - More powerful data loading
 techniques - An engine that can take over the whole training and testing
 process, with all the baby-sitting works (stage control, optimizer
 configuration, lr scheduling, checkpoint management, metrics & tensorboard
 writing, etc.) done automatically. See an [example](https://github.com/
 yeliudev/nncore/blob/main/examples/mnist.py) for details. Note that some
-methods in the library work with PyTorch 1.11+, but the installation of PyTorch
-is not necessary. ## Continuous Integration | Platform / Python Version | 3.8 |
-3.9 | 3.10 | 3.11 | | :-: | :-: | :-: | :-: | :-: | | Ubuntu 20.04 | [![Build]
+methods in the library work with PyTorch 2.0+, but the installation of PyTorch
+is not necessary. ## Continuous Integration | Platform / Python Version | 3.9 |
+3.10 | 3.11 | 3.12 | :-: | :-: | :-: | :-: | :-: | | Ubuntu 20.04 | [![Build]
 (https://badgen.net/runkit/yeliudev/nncore-badge/0?icon=github&cache=300)]
 [link] | [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/
 1?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/
 nncore-badge/2?icon=github&cache=300)][link] | [![Build](https://badgen.net/
 runkit/yeliudev/nncore-badge/3?icon=github&cache=300)][link] | | Ubuntu 22.04 |
 [![Build](https://badgen.net/runkit/yeliudev/nncore-badge/
 4?icon=github&cache=300)][link] | [![Build](https://badgen.net/runkit/yeliudev/
```

### Comparing `nncore-0.4.0/nncore.egg-info/SOURCES.txt` & `nncore-0.4.1/nncore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/setup.cfg` & `nncore-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/setup.py` & `nncore-0.4.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 import re
 from platform import system
 
 from pkg_resources import DistributionNotFound, get_distribution
 from setuptools import find_packages, setup
 
 INSTALL_REQUIRES = [
-    'h5py>=3.1', 'joblib>=1.1', 'jsonlines>=2', 'numpy>=1.19', 'pyyaml>=6',
-    'requests>=2.31', 'tabulate>=0.8', 'tensorboard>=2.12', 'termcolor>=1.1'
+    'h5py>=3.10', 'joblib>=1.3', 'jsonlines>=4', 'numpy>=1.26', 'pyyaml>=6',
+    'requests>=2.31', 'tabulate>=0.9', 'tensorboard>=2.16', 'termcolor>=2.4'
 ]
 
-OPENCV_INSTALL_REQUIRES = 'opencv-python-headless>=4.5', 'opencv-python>=4.5'
+OPENCV_INSTALL_REQUIRES = 'opencv-python-headless>=4.9', 'opencv-python>=4.9'
 
 
 def get_version():
     version_file = os.path.join('nncore', '__init__.py')
     with open(version_file, encoding='utf-8') as f:
         lines = f.readlines()
     for line in lines:
@@ -56,17 +56,18 @@
     long_description=get_readme(),
     long_description_content_type='text/markdown',
     classifiers=[
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Topic :: Utilities',
     ],
-    python_requires='>=3.8',
+    python_requires='>=3.9',
     setup_requires=['pytest-runner'],
     tests_require=['pytest'],
     install_requires=get_install_requires(),
     packages=find_packages(exclude=('.github', 'docs', 'examples', 'tests')))
```

### Comparing `nncore-0.4.0/tests/test_config.py` & `nncore-0.4.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/tests/test_data.py` & `nncore-0.4.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/tests/test_io.py` & `nncore-0.4.1/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/tests/test_logger.py` & `nncore-0.4.1/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/tests/test_path.py` & `nncore-0.4.1/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.0/tests/test_registry.py` & `nncore-0.4.1/tests/test_registry.py`

 * *Files identical despite different names*

