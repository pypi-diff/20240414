# Comparing `tmp/jammy-0.1.8.tar.gz` & `tmp/jammy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jammy-0.1.8.tar", max compression
+gzip compressed data, was "jammy-0.1.9.tar", max compression
```

## Comparing `jammy-0.1.8.tar` & `jammy-0.1.9.tar`

### file list

```diff
@@ -1,179 +1,179 @@
--rw-r--r--   0        0        0     2479 2023-07-21 02:38:00.291612 jammy-0.1.8/README.md
--rw-r--r--   0        0        0     1259 2023-07-21 02:38:00.295612 jammy-0.1.8/jammy/__init__.py
--rw-r--r--   0        0        0       70 2023-07-21 02:38:00.295612 jammy-0.1.8/jammy/cli/__init__.py
--rw-r--r--   0        0        0     5682 2023-07-21 02:38:00.295612 jammy-0.1.8/jammy/cli/argument.py
--rw-r--r--   0        0        0     1329 2023-07-21 02:38:00.295612 jammy-0.1.8/jammy/cli/cmd_utils.py
--rw-r--r--   0        0        0     2047 2023-07-21 02:38:00.295612 jammy-0.1.8/jammy/cli/cmdline_viz.py
--rw-r--r--   0        0        0     2403 2023-07-21 02:38:00.295612 jammy-0.1.8/jammy/cli/colors.py
--rw-r--r--   0        0        0     1743 2023-07-21 02:38:00.295612 jammy-0.1.8/jammy/cli/device.py
--rw-r--r--   0        0        0     2754 2023-07-21 02:38:00.295612 jammy-0.1.8/jammy/cli/keyboard.py
--rw-r--r--   0        0        0        0 2023-07-21 02:38:00.339611 jammy-0.1.8/jammy/cli_scripts/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 02:38:00.339611 jammy-0.1.8/jammy/cli_scripts/conf/__init__.py
--rw-r--r--   0        0        0      302 2023-07-21 02:38:00.295612 jammy-0.1.8/jammy/cli_scripts/conf/jamdk.yaml
--rw-r--r--   0        0        0      452 2023-07-21 02:38:00.295612 jammy-0.1.8/jammy/cli_scripts/conf/ngc.yaml
--rw-r--r--   0        0        0     4256 2023-07-21 02:38:00.295612 jammy-0.1.8/jammy/cli_scripts/dk.py
--rw-r--r--   0        0        0     3716 2023-07-21 02:38:00.295612 jammy-0.1.8/jammy/cli_scripts/gpu_sc.py
--rw-r--r--   0        0        0      304 2023-07-21 02:38:00.295612 jammy-0.1.8/jammy/cli_scripts/inspect_file.py
--rw-r--r--   0        0        0     6839 2023-07-21 02:38:00.295612 jammy-0.1.8/jammy/cli_scripts/ngc_debug.py
--rw-r--r--   0        0        0    17767 2023-07-21 02:38:00.296612 jammy-0.1.8/jammy/cli_scripts/shell_executor.py
--rw-r--r--   0        0        0    15458 2023-07-21 02:38:00.296612 jammy-0.1.8/jammy/cli_scripts/sys_info.py
--rw-r--r--   0        0        0       31 2023-07-21 02:38:00.296612 jammy-0.1.8/jammy/collections/__init__.py
--rw-r--r--   0        0        0      312 2023-07-21 02:38:00.296612 jammy-0.1.8/jammy/collections/lazy_dict.py
--rw-r--r--   0        0        0       39 2023-07-21 02:38:00.296612 jammy-0.1.8/jammy/comm/__init__.py
--rw-r--r--   0        0        0     6007 2023-07-21 02:38:00.296612 jammy-0.1.8/jammy/comm/cs.py
--rw-r--r--   0        0        0     1295 2023-07-21 02:38:00.296612 jammy-0.1.8/jammy/comm/utils.py
--rw-r--r--   0        0        0     2521 2023-07-21 02:38:00.296612 jammy-0.1.8/jammy/concurrency/__init__.py
--rw-r--r--   0        0        0     3757 2023-07-21 02:38:00.296612 jammy-0.1.8/jammy/concurrency/packing.py
--rw-r--r--   0        0        0     2533 2023-07-21 02:38:00.296612 jammy-0.1.8/jammy/concurrency/zmq_utils.py
--rw-r--r--   0        0        0       24 2023-07-21 02:38:00.296612 jammy-0.1.8/jammy/event/__init__.py
--rw-r--r--   0        0        0     2990 2023-07-21 02:38:00.296612 jammy-0.1.8/jammy/event/registry.py
--rw-r--r--   0        0        0       66 2023-07-21 02:38:00.296612 jammy-0.1.8/jammy/image/__init__.py
--rw-r--r--   0        0        0     3191 2023-07-21 02:38:00.296612 jammy-0.1.8/jammy/image/backend.py
--rw-r--r--   0        0        0     2139 2023-07-21 02:38:00.296612 jammy-0.1.8/jammy/image/codecs.py
--rw-r--r--   0        0        0     1554 2023-07-21 02:38:00.296612 jammy-0.1.8/jammy/image/imgio.py
--rw-r--r--   0        0        0     5101 2023-07-21 02:38:00.297612 jammy-0.1.8/jammy/image/imgproc.py
--rw-r--r--   0        0        0       84 2023-07-21 02:38:00.297612 jammy-0.1.8/jammy/io/__init__.py
--rw-r--r--   0        0        0     1088 2023-07-21 02:38:00.297612 jammy-0.1.8/jammy/io/common.py
--rw-r--r--   0        0        0    12085 2023-07-21 02:38:00.297612 jammy-0.1.8/jammy/io/fs.py
--rw-r--r--   0        0        0     1342 2023-07-21 02:38:00.297612 jammy-0.1.8/jammy/io/path.py
--rw-r--r--   0        0        0      302 2023-07-21 02:38:00.297612 jammy-0.1.8/jammy/io/tempfile.py
--rw-r--r--   0        0        0       95 2023-07-21 02:38:00.297612 jammy-0.1.8/jammy/logging/__init__.py
--rw-r--r--   0        0        0      489 2023-07-21 02:38:00.297612 jammy-0.1.8/jammy/logging/fake_logger.py
--rw-r--r--   0        0        0     1558 2023-07-21 02:38:00.297612 jammy-0.1.8/jammy/logging/logger.py
--rw-r--r--   0        0        0     5341 2023-07-21 02:38:00.297612 jammy-0.1.8/jammy/logging/wandb_utils.py
--rw-r--r--   0        0        0       44 2023-07-21 02:38:00.297612 jammy-0.1.8/jammy/random/__init__.py
--rw-r--r--   0        0        0     6177 2023-07-21 02:38:00.297612 jammy-0.1.8/jammy/random/_lazy_bind.py
--rw-r--r--   0        0        0     2952 2023-07-21 02:38:00.297612 jammy-0.1.8/jammy/random/rng.py
--rw-r--r--   0        0        0       26 2023-07-21 02:38:00.297612 jammy-0.1.8/jammy/storage/__init__.py
--rw-r--r--   0        0        0     1045 2023-07-21 02:38:00.297612 jammy-0.1.8/jammy/storage/attr_saver.py
--rw-r--r--   0        0        0        0 2023-07-21 02:38:00.340611 jammy-0.1.8/jammy/storage/kv/__init__.py
--rw-r--r--   0        0        0     2437 2023-07-21 02:38:00.297612 jammy-0.1.8/jammy/storage/kv/kv.py
--rw-r--r--   0        0        0     2860 2023-07-21 02:38:00.297612 jammy-0.1.8/jammy/storage/kv/lmdb.py
--rw-r--r--   0        0        0      834 2023-07-21 02:38:00.297612 jammy-0.1.8/jammy/storage/kv/mem.py
--rw-r--r--   0        0        0     2141 2023-07-21 02:38:00.297612 jammy-0.1.8/jammy/storage/kv/memcached.py
--rw-r--r--   0        0        0      188 2023-07-21 02:38:00.298611 jammy-0.1.8/jammy/utils/__init__.py
--rw-r--r--   0        0        0     3739 2023-07-21 02:38:00.298611 jammy-0.1.8/jammy/utils/argument.py
--rw-r--r--   0        0        0     2306 2023-07-21 02:38:00.298611 jammy-0.1.8/jammy/utils/cache.py
--rw-r--r--   0        0        0     1039 2023-07-21 02:38:00.298611 jammy-0.1.8/jammy/utils/cfg.py
--rw-r--r--   0        0        0     1773 2023-07-21 02:38:00.298611 jammy-0.1.8/jammy/utils/cnt.py
--rw-r--r--   0        0        0     1968 2023-07-21 02:38:00.298611 jammy-0.1.8/jammy/utils/colored_tqdm.py
--rw-r--r--   0        0        0     3271 2023-07-21 02:38:00.298611 jammy-0.1.8/jammy/utils/container.py
--rw-r--r--   0        0        0      358 2023-07-21 02:38:00.298611 jammy-0.1.8/jammy/utils/context.py
--rw-r--r--   0        0        0     6104 2023-07-21 02:38:00.298611 jammy-0.1.8/jammy/utils/debug.py
--rw-r--r--   0        0        0     5725 2023-07-21 02:38:00.298611 jammy-0.1.8/jammy/utils/defaults.py
--rw-r--r--   0        0        0      630 2023-07-21 02:38:00.298611 jammy-0.1.8/jammy/utils/deprecated.py
--rw-r--r--   0        0        0     1483 2023-07-21 02:38:00.298611 jammy-0.1.8/jammy/utils/enum.py
--rw-r--r--   0        0        0     1229 2023-07-21 02:38:00.298611 jammy-0.1.8/jammy/utils/env.py
--rw-r--r--   0        0        0     2061 2023-07-21 02:38:00.298611 jammy-0.1.8/jammy/utils/filelock.py
--rw-r--r--   0        0        0     1201 2023-07-21 02:38:00.298611 jammy-0.1.8/jammy/utils/git.py
--rw-r--r--   0        0        0     1581 2023-07-21 02:38:00.298611 jammy-0.1.8/jammy/utils/gpu.py
--rw-r--r--   0        0        0      430 2023-07-21 02:38:00.298611 jammy-0.1.8/jammy/utils/hash.py
--rw-r--r--   0        0        0     3515 2023-07-21 02:38:00.298611 jammy-0.1.8/jammy/utils/hyd.py
--rw-r--r--   0        0        0     2334 2023-07-21 02:38:00.298611 jammy-0.1.8/jammy/utils/imp.py
--rw-r--r--   0        0        0      975 2023-07-21 02:38:00.298611 jammy-0.1.8/jammy/utils/init.py
--rw-r--r--   0        0        0     1930 2023-07-21 02:38:00.298611 jammy-0.1.8/jammy/utils/inspect.py
--rw-r--r--   0        0        0     4034 2023-07-21 02:38:00.298611 jammy-0.1.8/jammy/utils/matching.py
--rw-r--r--   0        0        0     7222 2023-07-21 02:38:00.299612 jammy-0.1.8/jammy/utils/meta.py
--rw-r--r--   0        0        0     2986 2023-07-21 02:38:00.299612 jammy-0.1.8/jammy/utils/meter.py
--rw-r--r--   0        0        0       38 2023-07-21 02:38:00.299612 jammy-0.1.8/jammy/utils/mock.py
--rw-r--r--   0        0        0      797 2023-07-21 02:38:00.299612 jammy-0.1.8/jammy/utils/naming.py
--rw-r--r--   0        0        0     2118 2023-07-21 02:38:00.299612 jammy-0.1.8/jammy/utils/notifier.py
--rw-r--r--   0        0        0      442 2023-07-21 02:38:00.299612 jammy-0.1.8/jammy/utils/num_check.py
--rw-r--r--   0        0        0     9092 2023-07-21 02:38:00.299612 jammy-0.1.8/jammy/utils/printing.py
--rw-r--r--   0        0        0     6380 2023-07-21 02:38:00.299612 jammy-0.1.8/jammy/utils/process.py
--rw-r--r--   0        0        0    17173 2023-07-21 02:38:00.299612 jammy-0.1.8/jammy/utils/profiler.py
--rw-r--r--   0        0        0     4520 2023-07-21 02:38:00.299612 jammy-0.1.8/jammy/utils/registry.py
--rw-r--r--   0        0        0     4694 2023-07-21 02:38:00.299612 jammy-0.1.8/jammy/utils/retry.py
--rw-r--r--   0        0        0     1281 2023-07-21 02:38:00.299612 jammy-0.1.8/jammy/utils/sizeof.py
--rw-r--r--   0        0        0       81 2023-07-21 02:38:00.299612 jammy-0.1.8/jamnp/__init__.py
--rw-r--r--   0        0        0     1193 2023-07-21 02:38:00.299612 jammy-0.1.8/jamnp/buffer_storage.py
--rw-r--r--   0        0        0     1075 2023-07-21 02:38:00.299612 jammy-0.1.8/jamnp/container.py
--rw-r--r--   0        0        0      522 2023-07-21 02:38:00.299612 jammy-0.1.8/jamtorch/__init__.py
--rw-r--r--   0        0        0       22 2023-07-21 02:38:00.299612 jammy-0.1.8/jamtorch/cuda/__init__.py
--rw-r--r--   0        0        0      695 2023-07-21 02:38:00.299612 jammy-0.1.8/jamtorch/cuda/device.py
--rw-r--r--   0        0        0      172 2023-07-21 02:38:00.299612 jammy-0.1.8/jamtorch/cuda/readme.md
--rw-r--r--   0        0        0       64 2023-07-21 02:38:00.300612 jammy-0.1.8/jamtorch/data/__init__.py
--rw-r--r--   0        0        0     1291 2023-07-21 02:38:00.300612 jammy-0.1.8/jamtorch/data/buffer_storage.py
--rw-r--r--   0        0        0      554 2023-07-21 02:38:00.300612 jammy-0.1.8/jamtorch/data/dataset.py
--rw-r--r--   0        0        0     1532 2023-07-21 02:38:00.300612 jammy-0.1.8/jamtorch/data/meta.py
--rw-r--r--   0        0        0      116 2023-07-21 02:38:00.300612 jammy-0.1.8/jamtorch/ddp/__init__.py
--rw-r--r--   0        0        0      471 2023-07-21 02:38:00.300612 jammy-0.1.8/jamtorch/ddp/ddp_template.yaml
--rw-r--r--   0        0        0     2761 2023-07-21 02:38:00.300612 jammy-0.1.8/jamtorch/ddp/ddp_trainer.py
--rw-r--r--   0        0        0     4327 2023-07-21 02:38:00.300612 jammy-0.1.8/jamtorch/ddp/ddp_utils.py
--rw-r--r--   0        0        0      571 2023-07-21 02:38:00.300612 jammy-0.1.8/jamtorch/ddp/ema_trainer.py
--rw-r--r--   0        0        0      543 2023-07-21 02:38:00.300612 jammy-0.1.8/jamtorch/ddp/fns.py
--rw-r--r--   0        0        0      309 2023-07-21 02:38:00.300612 jammy-0.1.8/jamtorch/ddp/readme.md
--rw-r--r--   0        0        0       55 2023-07-21 02:38:00.300612 jammy-0.1.8/jamtorch/distributed/__init__.py
--rw-r--r--   0        0        0     1183 2023-07-21 02:38:00.300612 jammy-0.1.8/jamtorch/distributed/basic.py
--rw-r--r--   0        0        0     2866 2023-07-21 02:38:00.300612 jammy-0.1.8/jamtorch/distributed/filelock.py
--rw-r--r--   0        0        0      255 2023-07-21 02:38:00.300612 jammy-0.1.8/jamtorch/distributions/__init__.py
--rw-r--r--   0        0        0     4576 2023-07-21 02:38:00.300612 jammy-0.1.8/jamtorch/distributions/base.py
--rw-r--r--   0        0        0     2513 2023-07-21 02:38:00.300612 jammy-0.1.8/jamtorch/distributions/discrete.py
--rw-r--r--   0        0        0      403 2023-07-21 02:38:00.300612 jammy-0.1.8/jamtorch/distributions/fns.py
--rw-r--r--   0        0        0     6912 2023-07-21 02:38:00.300612 jammy-0.1.8/jamtorch/distributions/normal.py
--rw-r--r--   0        0        0     3416 2023-07-21 02:38:00.300612 jammy-0.1.8/jamtorch/distributions/uniform.py
--rw-r--r--   0        0        0      108 2023-07-21 02:38:00.300612 jammy-0.1.8/jamtorch/io/__init__.py
--rw-r--r--   0        0        0     5084 2023-07-21 02:38:00.300612 jammy-0.1.8/jamtorch/io/ckpt.py
--rw-r--r--   0        0        0     2798 2023-07-21 02:38:00.301612 jammy-0.1.8/jamtorch/io/ema.py
--rw-r--r--   0        0        0      475 2023-07-21 02:38:00.301612 jammy-0.1.8/jamtorch/io/ema_helper.py
--rw-r--r--   0        0        0      207 2023-07-21 02:38:00.301612 jammy-0.1.8/jamtorch/io/io.py
--rw-r--r--   0        0        0     2391 2023-07-21 02:38:00.301612 jammy-0.1.8/jamtorch/io/param_ema.py
--rw-r--r--   0        0        0        0 2023-07-21 02:38:00.342611 jammy-0.1.8/jamtorch/learn/__init__.py
--rw-r--r--   0        0        0     4248 2023-07-21 02:38:00.301612 jammy-0.1.8/jamtorch/learn/gan/sn_discriminator.py
--rw-r--r--   0        0        0       22 2023-07-21 02:38:00.301612 jammy-0.1.8/jamtorch/logging/__init__.py
--rw-r--r--   0        0        0      451 2023-07-21 02:38:00.301612 jammy-0.1.8/jamtorch/logging/logger.py
--rw-r--r--   0        0        0       76 2023-07-21 02:38:00.301612 jammy-0.1.8/jamtorch/nn/__init__.py
--rw-r--r--   0        0        0     7517 2023-07-21 02:38:00.301612 jammy-0.1.8/jamtorch/nn/base_modules.py
--rw-r--r--   0        0        0     2588 2023-07-21 02:38:00.301612 jammy-0.1.8/jamtorch/nn/fouriermlp.py
--rw-r--r--   0        0        0      186 2023-07-21 02:38:00.301612 jammy-0.1.8/jamtorch/nn/readme.md
--rw-r--r--   0        0        0     4461 2023-07-21 02:38:00.301612 jammy-0.1.8/jamtorch/nn/seq.py
--rw-r--r--   0        0        0      572 2023-07-21 02:38:00.301612 jammy-0.1.8/jamtorch/nn/simple_network.py
--rw-r--r--   0        0        0        0 2023-07-21 02:38:00.343611 jammy-0.1.8/jamtorch/nn/utils/__init__.py
--rw-r--r--   0        0        0    14986 2023-07-21 02:38:00.301612 jammy-0.1.8/jamtorch/nn/utils/spectral_norm.py
--rw-r--r--   0        0        0        0 2023-07-21 02:38:00.343611 jammy-0.1.8/jamtorch/pl_callbacks/__init__.py
--rw-r--r--   0        0        0     1438 2023-07-21 02:38:00.301612 jammy-0.1.8/jamtorch/pl_callbacks/cuda_cb.py
--rw-r--r--   0        0        0      575 2023-07-21 02:38:00.301612 jammy-0.1.8/jamtorch/pl_callbacks/every_n.py
--rw-r--r--   0        0        0      552 2023-07-21 02:38:00.301612 jammy-0.1.8/jamtorch/prototype/__init__.py
--rw-r--r--   0        0        0      185 2023-07-21 02:38:00.302611 jammy-0.1.8/jamtorch/prototype/optim.py
--rw-r--r--   0        0        0     3560 2023-07-21 02:38:00.302611 jammy-0.1.8/jamtorch/prototype/pytorch_util.py
--rw-r--r--   0        0        0      177 2023-07-21 02:38:00.302611 jammy-0.1.8/jamtorch/readme.md
--rw-r--r--   0        0        0      106 2023-07-21 02:38:00.302611 jammy-0.1.8/jamtorch/trainer/__init__.py
--rw-r--r--   0        0        0     3228 2023-07-21 02:38:00.302611 jammy-0.1.8/jamtorch/trainer/amp.py
--rw-r--r--   0        0        0     2956 2023-07-21 02:38:00.302611 jammy-0.1.8/jamtorch/trainer/cfg_trainer.py
--rw-r--r--   0        0        0      413 2023-07-21 02:38:00.302611 jammy-0.1.8/jamtorch/trainer/design_trainer.md
--rw-r--r--   0        0        0      738 2023-07-21 02:38:00.302611 jammy-0.1.8/jamtorch/trainer/ema_trainer.py
--rw-r--r--   0        0        0    10807 2023-07-21 02:38:00.302611 jammy-0.1.8/jamtorch/trainer/genetic_trainer.py
--rw-r--r--   0        0        0      400 2023-07-21 02:38:00.302611 jammy-0.1.8/jamtorch/trainer/hydra_utils.py
--rw-r--r--   0        0        0     2940 2023-07-21 02:38:00.302611 jammy-0.1.8/jamtorch/trainer/monitor.py
--rw-r--r--   0        0        0     3632 2023-07-21 02:38:00.302611 jammy-0.1.8/jamtorch/trainer/progress_fn.py
--rw-r--r--   0        0        0     1070 2023-07-21 02:38:00.302611 jammy-0.1.8/jamtorch/trainer/simple_trainer.py
--rw-r--r--   0        0        0     2489 2023-07-21 02:38:00.302611 jammy-0.1.8/jamtorch/trainer/tb.py
--rw-r--r--   0        0        0     5312 2023-07-21 02:38:00.302611 jammy-0.1.8/jamtorch/trainer/test_trainer.py
--rw-r--r--   0        0        0    10617 2023-07-21 02:38:00.302611 jammy-0.1.8/jamtorch/trainer/trainer.py
--rw-r--r--   0        0        0     2161 2023-07-21 02:38:00.302611 jammy-0.1.8/jamtorch/trainer/trainer_fn.py
--rw-r--r--   0        0        0     1474 2023-07-21 02:38:00.302611 jammy-0.1.8/jamtorch/trainer/trainer_monitor.py
--rw-r--r--   0        0        0     2242 2023-07-21 02:38:00.302611 jammy-0.1.8/jamtorch/trainer/utils.py
--rw-r--r--   0        0        0       69 2023-07-21 02:38:00.302611 jammy-0.1.8/jamtorch/utils/__init__.py
--rw-r--r--   0        0        0      907 2023-07-21 02:38:00.302611 jammy-0.1.8/jamtorch/utils/deep_to.py
--rw-r--r--   0        0        0      239 2023-07-21 02:38:00.302611 jammy-0.1.8/jamtorch/utils/grad.py
--rw-r--r--   0        0        0      523 2023-07-21 02:38:00.302611 jammy-0.1.8/jamtorch/utils/init.py
--rw-r--r--   0        0        0     2324 2023-07-21 02:38:00.303612 jammy-0.1.8/jamtorch/utils/meta.py
--rw-r--r--   0        0        0     2325 2023-07-21 02:38:00.303612 jammy-0.1.8/jamtorch/utils/pytree.py
--rw-r--r--   0        0        0     3217 2023-07-21 02:38:00.303612 jammy-0.1.8/jamtorch/utils/ts_ops.py
--rw-r--r--   0        0        0      129 2023-07-21 02:38:00.303612 jammy-0.1.8/jamviz/README.md
--rw-r--r--   0        0        0       19 2023-07-21 02:38:00.303612 jammy-0.1.8/jamviz/__init__.py
--rw-r--r--   0        0        0     2482 2023-07-21 02:38:00.303612 jammy-0.1.8/jamviz/img.py
--rw-r--r--   0        0        0        0 2023-07-21 02:38:00.344611 jammy-0.1.8/jamviz/jupyter/__init__.py
--rw-r--r--   0        0        0       64 2023-07-21 02:38:00.303612 jammy-0.1.8/jamviz/plt/__init__.py
--rw-r--r--   0        0        0     2297 2023-07-21 02:38:00.303612 jammy-0.1.8/jamviz/plt/color_list.py
--rw-r--r--   0        0        0      613 2023-07-21 02:38:00.303612 jammy-0.1.8/jamviz/plt/img.py
--rw-r--r--   0        0        0     4405 2023-07-21 02:38:00.303612 jammy-0.1.8/jamviz/plt/mstd.py
--rw-r--r--   0        0        0        0 2023-07-21 02:38:00.344611 jammy-0.1.8/jamweb/__init__.py
--rw-r--r--   0        0        0       71 2023-07-21 02:38:00.303612 jammy-0.1.8/jamweb/readme.md
--rw-r--r--   0        0        0        0 2023-07-21 02:38:00.344611 jammy-0.1.8/jamweb/session/__init__.py
--rw-r--r--   0        0        0     2649 2023-07-21 02:38:00.303612 jammy-0.1.8/jamweb/session/memcached.py
--rw-r--r--   0        0        0     1662 2023-07-21 02:38:00.303612 jammy-0.1.8/jamweb/session/session.py
--rw-r--r--   0        0        0       27 2023-07-21 02:38:00.303612 jammy-0.1.8/jamweb/web/__init__.py
--rw-r--r--   0        0        0     5935 2023-07-21 02:38:00.303612 jammy-0.1.8/jamweb/web/application.py
--rw-r--r--   0        0        0     2883 2023-07-21 02:38:01.449600 jammy-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     5073 1970-01-01 00:00:00.000000 jammy-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     2479 2023-08-07 21:45:31.763935 jammy-0.1.9/README.md
+-rw-r--r--   0        0        0     1259 2023-08-07 21:45:31.767935 jammy-0.1.9/jammy/__init__.py
+-rw-r--r--   0        0        0       70 2023-08-07 21:45:31.767935 jammy-0.1.9/jammy/cli/__init__.py
+-rw-r--r--   0        0        0     5682 2023-08-07 21:45:31.768935 jammy-0.1.9/jammy/cli/argument.py
+-rw-r--r--   0        0        0     1329 2023-08-07 21:45:31.768935 jammy-0.1.9/jammy/cli/cmd_utils.py
+-rw-r--r--   0        0        0     2047 2023-08-07 21:45:31.768935 jammy-0.1.9/jammy/cli/cmdline_viz.py
+-rw-r--r--   0        0        0     2403 2023-08-07 21:45:31.768935 jammy-0.1.9/jammy/cli/colors.py
+-rw-r--r--   0        0        0     1743 2023-08-07 21:45:31.768935 jammy-0.1.9/jammy/cli/device.py
+-rw-r--r--   0        0        0     2754 2023-08-07 21:45:31.768935 jammy-0.1.9/jammy/cli/keyboard.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:45:31.814935 jammy-0.1.9/jammy/cli_scripts/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:45:31.814935 jammy-0.1.9/jammy/cli_scripts/conf/__init__.py
+-rw-r--r--   0        0        0      302 2023-08-07 21:45:31.768935 jammy-0.1.9/jammy/cli_scripts/conf/jamdk.yaml
+-rw-r--r--   0        0        0      452 2023-08-07 21:45:31.768935 jammy-0.1.9/jammy/cli_scripts/conf/ngc.yaml
+-rw-r--r--   0        0        0     4309 2023-08-07 21:45:31.768935 jammy-0.1.9/jammy/cli_scripts/dk.py
+-rw-r--r--   0        0        0     3716 2023-08-07 21:45:31.768935 jammy-0.1.9/jammy/cli_scripts/gpu_sc.py
+-rw-r--r--   0        0        0      304 2023-08-07 21:45:31.768935 jammy-0.1.9/jammy/cli_scripts/inspect_file.py
+-rw-r--r--   0        0        0     6839 2023-08-07 21:45:31.768935 jammy-0.1.9/jammy/cli_scripts/ngc_debug.py
+-rw-r--r--   0        0        0    17767 2023-08-07 21:45:31.768935 jammy-0.1.9/jammy/cli_scripts/shell_executor.py
+-rw-r--r--   0        0        0    15458 2023-08-07 21:45:31.768935 jammy-0.1.9/jammy/cli_scripts/sys_info.py
+-rw-r--r--   0        0        0       31 2023-08-07 21:45:31.768935 jammy-0.1.9/jammy/collections/__init__.py
+-rw-r--r--   0        0        0      312 2023-08-07 21:45:31.769935 jammy-0.1.9/jammy/collections/lazy_dict.py
+-rw-r--r--   0        0        0       39 2023-08-07 21:45:31.769935 jammy-0.1.9/jammy/comm/__init__.py
+-rw-r--r--   0        0        0     6007 2023-08-07 21:45:31.769935 jammy-0.1.9/jammy/comm/cs.py
+-rw-r--r--   0        0        0     1295 2023-08-07 21:45:31.769935 jammy-0.1.9/jammy/comm/utils.py
+-rw-r--r--   0        0        0     2521 2023-08-07 21:45:31.769935 jammy-0.1.9/jammy/concurrency/__init__.py
+-rw-r--r--   0        0        0     3757 2023-08-07 21:45:31.769935 jammy-0.1.9/jammy/concurrency/packing.py
+-rw-r--r--   0        0        0     2533 2023-08-07 21:45:31.769935 jammy-0.1.9/jammy/concurrency/zmq_utils.py
+-rw-r--r--   0        0        0       24 2023-08-07 21:45:31.769935 jammy-0.1.9/jammy/event/__init__.py
+-rw-r--r--   0        0        0     2990 2023-08-07 21:45:31.769935 jammy-0.1.9/jammy/event/registry.py
+-rw-r--r--   0        0        0       66 2023-08-07 21:45:31.769935 jammy-0.1.9/jammy/image/__init__.py
+-rw-r--r--   0        0        0     3191 2023-08-07 21:45:31.769935 jammy-0.1.9/jammy/image/backend.py
+-rw-r--r--   0        0        0     2139 2023-08-07 21:45:31.769935 jammy-0.1.9/jammy/image/codecs.py
+-rw-r--r--   0        0        0     1554 2023-08-07 21:45:31.769935 jammy-0.1.9/jammy/image/imgio.py
+-rw-r--r--   0        0        0     5101 2023-08-07 21:45:31.769935 jammy-0.1.9/jammy/image/imgproc.py
+-rw-r--r--   0        0        0       84 2023-08-07 21:45:31.769935 jammy-0.1.9/jammy/io/__init__.py
+-rw-r--r--   0        0        0     1088 2023-08-07 21:45:31.769935 jammy-0.1.9/jammy/io/common.py
+-rw-r--r--   0        0        0    12085 2023-08-07 21:45:31.770935 jammy-0.1.9/jammy/io/fs.py
+-rw-r--r--   0        0        0     1342 2023-08-07 21:45:31.770935 jammy-0.1.9/jammy/io/path.py
+-rw-r--r--   0        0        0      302 2023-08-07 21:45:31.770935 jammy-0.1.9/jammy/io/tempfile.py
+-rw-r--r--   0        0        0       95 2023-08-07 21:45:31.770935 jammy-0.1.9/jammy/logging/__init__.py
+-rw-r--r--   0        0        0      489 2023-08-07 21:45:31.770935 jammy-0.1.9/jammy/logging/fake_logger.py
+-rw-r--r--   0        0        0     1224 2023-08-07 21:45:31.770935 jammy-0.1.9/jammy/logging/logger.py
+-rw-r--r--   0        0        0     5341 2023-08-07 21:45:31.770935 jammy-0.1.9/jammy/logging/wandb_utils.py
+-rw-r--r--   0        0        0       44 2023-08-07 21:45:31.770935 jammy-0.1.9/jammy/random/__init__.py
+-rw-r--r--   0        0        0     6177 2023-08-07 21:45:31.770935 jammy-0.1.9/jammy/random/_lazy_bind.py
+-rw-r--r--   0        0        0     2952 2023-08-07 21:45:31.770935 jammy-0.1.9/jammy/random/rng.py
+-rw-r--r--   0        0        0       26 2023-08-07 21:45:31.770935 jammy-0.1.9/jammy/storage/__init__.py
+-rw-r--r--   0        0        0     1045 2023-08-07 21:45:31.770935 jammy-0.1.9/jammy/storage/attr_saver.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:45:31.815935 jammy-0.1.9/jammy/storage/kv/__init__.py
+-rw-r--r--   0        0        0     2437 2023-08-07 21:45:31.770935 jammy-0.1.9/jammy/storage/kv/kv.py
+-rw-r--r--   0        0        0     2860 2023-08-07 21:45:31.770935 jammy-0.1.9/jammy/storage/kv/lmdb.py
+-rw-r--r--   0        0        0      834 2023-08-07 21:45:31.770935 jammy-0.1.9/jammy/storage/kv/mem.py
+-rw-r--r--   0        0        0     2141 2023-08-07 21:45:31.770935 jammy-0.1.9/jammy/storage/kv/memcached.py
+-rw-r--r--   0        0        0      188 2023-08-07 21:45:31.770935 jammy-0.1.9/jammy/utils/__init__.py
+-rw-r--r--   0        0        0     3739 2023-08-07 21:45:31.770935 jammy-0.1.9/jammy/utils/argument.py
+-rw-r--r--   0        0        0     2306 2023-08-07 21:45:31.770935 jammy-0.1.9/jammy/utils/cache.py
+-rw-r--r--   0        0        0     1039 2023-08-07 21:45:31.771935 jammy-0.1.9/jammy/utils/cfg.py
+-rw-r--r--   0        0        0     1773 2023-08-07 21:45:31.771935 jammy-0.1.9/jammy/utils/cnt.py
+-rw-r--r--   0        0        0     1968 2023-08-07 21:45:31.771935 jammy-0.1.9/jammy/utils/colored_tqdm.py
+-rw-r--r--   0        0        0     3271 2023-08-07 21:45:31.771935 jammy-0.1.9/jammy/utils/container.py
+-rw-r--r--   0        0        0      358 2023-08-07 21:45:31.771935 jammy-0.1.9/jammy/utils/context.py
+-rw-r--r--   0        0        0     6104 2023-08-07 21:45:31.771935 jammy-0.1.9/jammy/utils/debug.py
+-rw-r--r--   0        0        0     5725 2023-08-07 21:45:31.771935 jammy-0.1.9/jammy/utils/defaults.py
+-rw-r--r--   0        0        0      630 2023-08-07 21:45:31.771935 jammy-0.1.9/jammy/utils/deprecated.py
+-rw-r--r--   0        0        0     1483 2023-08-07 21:45:31.771935 jammy-0.1.9/jammy/utils/enum.py
+-rw-r--r--   0        0        0     1229 2023-08-07 21:45:31.771935 jammy-0.1.9/jammy/utils/env.py
+-rw-r--r--   0        0        0     2061 2023-08-07 21:45:31.771935 jammy-0.1.9/jammy/utils/filelock.py
+-rw-r--r--   0        0        0     1201 2023-08-07 21:45:31.771935 jammy-0.1.9/jammy/utils/git.py
+-rw-r--r--   0        0        0     1581 2023-08-07 21:45:31.771935 jammy-0.1.9/jammy/utils/gpu.py
+-rw-r--r--   0        0        0      430 2023-08-07 21:45:31.771935 jammy-0.1.9/jammy/utils/hash.py
+-rw-r--r--   0        0        0     3515 2023-08-07 21:45:31.771935 jammy-0.1.9/jammy/utils/hyd.py
+-rw-r--r--   0        0        0     2334 2023-08-07 21:45:31.771935 jammy-0.1.9/jammy/utils/imp.py
+-rw-r--r--   0        0        0      975 2023-08-07 21:45:31.771935 jammy-0.1.9/jammy/utils/init.py
+-rw-r--r--   0        0        0     1930 2023-08-07 21:45:31.771935 jammy-0.1.9/jammy/utils/inspect.py
+-rw-r--r--   0        0        0     4034 2023-08-07 21:45:31.771935 jammy-0.1.9/jammy/utils/matching.py
+-rw-r--r--   0        0        0     7222 2023-08-07 21:45:31.771935 jammy-0.1.9/jammy/utils/meta.py
+-rw-r--r--   0        0        0     2986 2023-08-07 21:45:31.771935 jammy-0.1.9/jammy/utils/meter.py
+-rw-r--r--   0        0        0       38 2023-08-07 21:45:31.771935 jammy-0.1.9/jammy/utils/mock.py
+-rw-r--r--   0        0        0      797 2023-08-07 21:45:31.772935 jammy-0.1.9/jammy/utils/naming.py
+-rw-r--r--   0        0        0     2118 2023-08-07 21:45:31.772935 jammy-0.1.9/jammy/utils/notifier.py
+-rw-r--r--   0        0        0      442 2023-08-07 21:45:31.772935 jammy-0.1.9/jammy/utils/num_check.py
+-rw-r--r--   0        0        0     9092 2023-08-07 21:45:31.772935 jammy-0.1.9/jammy/utils/printing.py
+-rw-r--r--   0        0        0     6380 2023-08-07 21:45:31.772935 jammy-0.1.9/jammy/utils/process.py
+-rw-r--r--   0        0        0    17173 2023-08-07 21:45:31.772935 jammy-0.1.9/jammy/utils/profiler.py
+-rw-r--r--   0        0        0     4520 2023-08-07 21:45:31.772935 jammy-0.1.9/jammy/utils/registry.py
+-rw-r--r--   0        0        0     4694 2023-08-07 21:45:31.772935 jammy-0.1.9/jammy/utils/retry.py
+-rw-r--r--   0        0        0     1281 2023-08-07 21:45:31.772935 jammy-0.1.9/jammy/utils/sizeof.py
+-rw-r--r--   0        0        0       81 2023-08-07 21:45:31.772935 jammy-0.1.9/jamnp/__init__.py
+-rw-r--r--   0        0        0     1193 2023-08-07 21:45:31.772935 jammy-0.1.9/jamnp/buffer_storage.py
+-rw-r--r--   0        0        0     1075 2023-08-07 21:45:31.772935 jammy-0.1.9/jamnp/container.py
+-rw-r--r--   0        0        0      522 2023-08-07 21:45:31.772935 jammy-0.1.9/jamtorch/__init__.py
+-rw-r--r--   0        0        0       22 2023-08-07 21:45:31.772935 jammy-0.1.9/jamtorch/cuda/__init__.py
+-rw-r--r--   0        0        0      695 2023-08-07 21:45:31.772935 jammy-0.1.9/jamtorch/cuda/device.py
+-rw-r--r--   0        0        0      172 2023-08-07 21:45:31.772935 jammy-0.1.9/jamtorch/cuda/readme.md
+-rw-r--r--   0        0        0       64 2023-08-07 21:45:31.772935 jammy-0.1.9/jamtorch/data/__init__.py
+-rw-r--r--   0        0        0     1291 2023-08-07 21:45:31.772935 jammy-0.1.9/jamtorch/data/buffer_storage.py
+-rw-r--r--   0        0        0      554 2023-08-07 21:45:31.772935 jammy-0.1.9/jamtorch/data/dataset.py
+-rw-r--r--   0        0        0     1532 2023-08-07 21:45:31.773935 jammy-0.1.9/jamtorch/data/meta.py
+-rw-r--r--   0        0        0      116 2023-08-07 21:45:31.773935 jammy-0.1.9/jamtorch/ddp/__init__.py
+-rw-r--r--   0        0        0      471 2023-08-07 21:45:31.773935 jammy-0.1.9/jamtorch/ddp/ddp_template.yaml
+-rw-r--r--   0        0        0     2761 2023-08-07 21:45:31.773935 jammy-0.1.9/jamtorch/ddp/ddp_trainer.py
+-rw-r--r--   0        0        0     4327 2023-08-07 21:45:31.773935 jammy-0.1.9/jamtorch/ddp/ddp_utils.py
+-rw-r--r--   0        0        0      571 2023-08-07 21:45:31.773935 jammy-0.1.9/jamtorch/ddp/ema_trainer.py
+-rw-r--r--   0        0        0      543 2023-08-07 21:45:31.773935 jammy-0.1.9/jamtorch/ddp/fns.py
+-rw-r--r--   0        0        0      309 2023-08-07 21:45:31.773935 jammy-0.1.9/jamtorch/ddp/readme.md
+-rw-r--r--   0        0        0       55 2023-08-07 21:45:31.773935 jammy-0.1.9/jamtorch/distributed/__init__.py
+-rw-r--r--   0        0        0     1183 2023-08-07 21:45:31.773935 jammy-0.1.9/jamtorch/distributed/basic.py
+-rw-r--r--   0        0        0     2866 2023-08-07 21:45:31.773935 jammy-0.1.9/jamtorch/distributed/filelock.py
+-rw-r--r--   0        0        0      255 2023-08-07 21:45:31.773935 jammy-0.1.9/jamtorch/distributions/__init__.py
+-rw-r--r--   0        0        0     4576 2023-08-07 21:45:31.773935 jammy-0.1.9/jamtorch/distributions/base.py
+-rw-r--r--   0        0        0     2513 2023-08-07 21:45:31.773935 jammy-0.1.9/jamtorch/distributions/discrete.py
+-rw-r--r--   0        0        0      403 2023-08-07 21:45:31.773935 jammy-0.1.9/jamtorch/distributions/fns.py
+-rw-r--r--   0        0        0     6912 2023-08-07 21:45:31.773935 jammy-0.1.9/jamtorch/distributions/normal.py
+-rw-r--r--   0        0        0     3416 2023-08-07 21:45:31.773935 jammy-0.1.9/jamtorch/distributions/uniform.py
+-rw-r--r--   0        0        0      108 2023-08-07 21:45:31.773935 jammy-0.1.9/jamtorch/io/__init__.py
+-rw-r--r--   0        0        0     5084 2023-08-07 21:45:31.773935 jammy-0.1.9/jamtorch/io/ckpt.py
+-rw-r--r--   0        0        0     2798 2023-08-07 21:45:31.773935 jammy-0.1.9/jamtorch/io/ema.py
+-rw-r--r--   0        0        0      475 2023-08-07 21:45:31.774935 jammy-0.1.9/jamtorch/io/ema_helper.py
+-rw-r--r--   0        0        0      207 2023-08-07 21:45:31.774935 jammy-0.1.9/jamtorch/io/io.py
+-rw-r--r--   0        0        0     2391 2023-08-07 21:45:31.774935 jammy-0.1.9/jamtorch/io/param_ema.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:45:31.817935 jammy-0.1.9/jamtorch/learn/__init__.py
+-rw-r--r--   0        0        0     4248 2023-08-07 21:45:31.774935 jammy-0.1.9/jamtorch/learn/gan/sn_discriminator.py
+-rw-r--r--   0        0        0       22 2023-08-07 21:45:31.774935 jammy-0.1.9/jamtorch/logging/__init__.py
+-rw-r--r--   0        0        0      451 2023-08-07 21:45:31.774935 jammy-0.1.9/jamtorch/logging/logger.py
+-rw-r--r--   0        0        0       76 2023-08-07 21:45:31.774935 jammy-0.1.9/jamtorch/nn/__init__.py
+-rw-r--r--   0        0        0     7517 2023-08-07 21:45:31.774935 jammy-0.1.9/jamtorch/nn/base_modules.py
+-rw-r--r--   0        0        0     2588 2023-08-07 21:45:31.774935 jammy-0.1.9/jamtorch/nn/fouriermlp.py
+-rw-r--r--   0        0        0      186 2023-08-07 21:45:31.774935 jammy-0.1.9/jamtorch/nn/readme.md
+-rw-r--r--   0        0        0     4461 2023-08-07 21:45:31.774935 jammy-0.1.9/jamtorch/nn/seq.py
+-rw-r--r--   0        0        0      572 2023-08-07 21:45:31.774935 jammy-0.1.9/jamtorch/nn/simple_network.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:45:31.817935 jammy-0.1.9/jamtorch/nn/utils/__init__.py
+-rw-r--r--   0        0        0    14986 2023-08-07 21:45:31.774935 jammy-0.1.9/jamtorch/nn/utils/spectral_norm.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:45:31.817935 jammy-0.1.9/jamtorch/pl_callbacks/__init__.py
+-rw-r--r--   0        0        0     1438 2023-08-07 21:45:31.774935 jammy-0.1.9/jamtorch/pl_callbacks/cuda_cb.py
+-rw-r--r--   0        0        0      575 2023-08-07 21:45:31.774935 jammy-0.1.9/jamtorch/pl_callbacks/every_n.py
+-rw-r--r--   0        0        0      552 2023-08-07 21:45:31.774935 jammy-0.1.9/jamtorch/prototype/__init__.py
+-rw-r--r--   0        0        0      185 2023-08-07 21:45:31.775935 jammy-0.1.9/jamtorch/prototype/optim.py
+-rw-r--r--   0        0        0     3560 2023-08-07 21:45:31.775935 jammy-0.1.9/jamtorch/prototype/pytorch_util.py
+-rw-r--r--   0        0        0      177 2023-08-07 21:45:31.775935 jammy-0.1.9/jamtorch/readme.md
+-rw-r--r--   0        0        0      106 2023-08-07 21:45:31.775935 jammy-0.1.9/jamtorch/trainer/__init__.py
+-rw-r--r--   0        0        0     3228 2023-08-07 21:45:31.775935 jammy-0.1.9/jamtorch/trainer/amp.py
+-rw-r--r--   0        0        0     2956 2023-08-07 21:45:31.775935 jammy-0.1.9/jamtorch/trainer/cfg_trainer.py
+-rw-r--r--   0        0        0      413 2023-08-07 21:45:31.775935 jammy-0.1.9/jamtorch/trainer/design_trainer.md
+-rw-r--r--   0        0        0      738 2023-08-07 21:45:31.775935 jammy-0.1.9/jamtorch/trainer/ema_trainer.py
+-rw-r--r--   0        0        0    10807 2023-08-07 21:45:31.775935 jammy-0.1.9/jamtorch/trainer/genetic_trainer.py
+-rw-r--r--   0        0        0      400 2023-08-07 21:45:31.775935 jammy-0.1.9/jamtorch/trainer/hydra_utils.py
+-rw-r--r--   0        0        0     2940 2023-08-07 21:45:31.775935 jammy-0.1.9/jamtorch/trainer/monitor.py
+-rw-r--r--   0        0        0     3632 2023-08-07 21:45:31.775935 jammy-0.1.9/jamtorch/trainer/progress_fn.py
+-rw-r--r--   0        0        0     1070 2023-08-07 21:45:31.775935 jammy-0.1.9/jamtorch/trainer/simple_trainer.py
+-rw-r--r--   0        0        0     2489 2023-08-07 21:45:31.775935 jammy-0.1.9/jamtorch/trainer/tb.py
+-rw-r--r--   0        0        0     5312 2023-08-07 21:45:31.775935 jammy-0.1.9/jamtorch/trainer/test_trainer.py
+-rw-r--r--   0        0        0    10617 2023-08-07 21:45:31.775935 jammy-0.1.9/jamtorch/trainer/trainer.py
+-rw-r--r--   0        0        0     2161 2023-08-07 21:45:31.775935 jammy-0.1.9/jamtorch/trainer/trainer_fn.py
+-rw-r--r--   0        0        0     1474 2023-08-07 21:45:31.775935 jammy-0.1.9/jamtorch/trainer/trainer_monitor.py
+-rw-r--r--   0        0        0     2242 2023-08-07 21:45:31.775935 jammy-0.1.9/jamtorch/trainer/utils.py
+-rw-r--r--   0        0        0       69 2023-08-07 21:45:31.775935 jammy-0.1.9/jamtorch/utils/__init__.py
+-rw-r--r--   0        0        0      907 2023-08-07 21:45:31.775935 jammy-0.1.9/jamtorch/utils/deep_to.py
+-rw-r--r--   0        0        0      239 2023-08-07 21:45:31.776935 jammy-0.1.9/jamtorch/utils/grad.py
+-rw-r--r--   0        0        0      523 2023-08-07 21:45:31.776935 jammy-0.1.9/jamtorch/utils/init.py
+-rw-r--r--   0        0        0     2324 2023-08-07 21:45:31.776935 jammy-0.1.9/jamtorch/utils/meta.py
+-rw-r--r--   0        0        0     2325 2023-08-07 21:45:31.776935 jammy-0.1.9/jamtorch/utils/pytree.py
+-rw-r--r--   0        0        0     3217 2023-08-07 21:45:31.776935 jammy-0.1.9/jamtorch/utils/ts_ops.py
+-rw-r--r--   0        0        0      129 2023-08-07 21:45:31.776935 jammy-0.1.9/jamviz/README.md
+-rw-r--r--   0        0        0       19 2023-08-07 21:45:31.776935 jammy-0.1.9/jamviz/__init__.py
+-rw-r--r--   0        0        0     2482 2023-08-07 21:45:31.776935 jammy-0.1.9/jamviz/img.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:45:31.818935 jammy-0.1.9/jamviz/jupyter/__init__.py
+-rw-r--r--   0        0        0       64 2023-08-07 21:45:31.776935 jammy-0.1.9/jamviz/plt/__init__.py
+-rw-r--r--   0        0        0     2297 2023-08-07 21:45:31.776935 jammy-0.1.9/jamviz/plt/color_list.py
+-rw-r--r--   0        0        0      613 2023-08-07 21:45:31.776935 jammy-0.1.9/jamviz/plt/img.py
+-rw-r--r--   0        0        0     4405 2023-08-07 21:45:31.776935 jammy-0.1.9/jamviz/plt/mstd.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:45:31.818935 jammy-0.1.9/jamweb/__init__.py
+-rw-r--r--   0        0        0       71 2023-08-07 21:45:31.776935 jammy-0.1.9/jamweb/readme.md
+-rw-r--r--   0        0        0        0 2023-08-07 21:45:31.818935 jammy-0.1.9/jamweb/session/__init__.py
+-rw-r--r--   0        0        0     2649 2023-08-07 21:45:31.776935 jammy-0.1.9/jamweb/session/memcached.py
+-rw-r--r--   0        0        0     1662 2023-08-07 21:45:31.776935 jammy-0.1.9/jamweb/session/session.py
+-rw-r--r--   0        0        0       27 2023-08-07 21:45:31.776935 jammy-0.1.9/jamweb/web/__init__.py
+-rw-r--r--   0        0        0     5935 2023-08-07 21:45:31.776935 jammy-0.1.9/jamweb/web/application.py
+-rw-r--r--   0        0        0     2884 2023-08-07 21:45:32.962933 jammy-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     5074 1970-01-01 00:00:00.000000 jammy-0.1.9/PKG-INFO
```

### Comparing `jammy-0.1.8/README.md` & `jammy-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/__init__.py` & `jammy-0.1.9/jammy/__init__.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/cli/argument.py` & `jammy-0.1.9/jammy/cli/argument.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/cli/cmd_utils.py` & `jammy-0.1.9/jammy/cli/cmd_utils.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/cli/cmdline_viz.py` & `jammy-0.1.9/jammy/cli/cmdline_viz.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/cli/colors.py` & `jammy-0.1.9/jammy/cli/colors.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/cli/device.py` & `jammy-0.1.9/jammy/cli/device.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/cli/keyboard.py` & `jammy-0.1.9/jammy/cli/keyboard.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/cli_scripts/dk.py` & `jammy-0.1.9/jammy/cli_scripts/dk.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from omegaconf import DictConfig, OmegaConf
 
 from jammy.logging import get_logger
 
 logger = get_logger()
 
 jam_dk_wrappers = []
-dk_args = ["docker", "run", "-d", "--gpus", "all", "--privileged"]
+dk_args = ["docker", "run", "-d", "--gpus", "all", "--privileged", "-it"]
 print_args = ["\n", "\t".join(dk_args)]
 
 
 def jamdk_wrapper(func):
     global jam_dk_wrappers, dk_args, print_args
 
     @functools.wraps(func)
@@ -65,15 +65,15 @@
             return rtn
     return None
 
 
 @jamdk_wrapper
 def check_memeory(cfg):
     mem_bytes = os.sysconf("SC_PAGE_SIZE") * os.sysconf("SC_PHYS_PAGES")
-    mem_gib = mem_bytes / (1024.0 ** 3)
+    mem_gib = mem_bytes / (1024.0**3)
     if cfg.memory is None:
         cfg.memory = int(mem_gib)
     return ["--shm-size", f"{cfg.memory}G"]
 
 
 @jamdk_wrapper
 def check_x_display(cfg):
@@ -152,14 +152,15 @@
 
 @hydra.main(config_path="conf", config_name="jamdk", version_base="1.1.0")
 def my_app(cfg: DictConfig) -> None:
     OmegaConf.set_struct(cfg, False)
     cfg = read_local_cfg(cfg)
     for item in jam_dk_wrappers:
         item(cfg)
+    dk_args.extend("tail -f /dev/null".split())
     logger.debug(dk_args)
     logger.info(f"stating {cfg.name}" + "\n".join(print_args))
     Popen(dk_args)  # pylint: disable=consider-using-with
 
 
 if __name__ == "__main__":
     my_app()  # pylint: disable=no-value-for-parameter
```

### Comparing `jammy-0.1.8/jammy/cli_scripts/gpu_sc.py` & `jammy-0.1.9/jammy/cli_scripts/gpu_sc.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/cli_scripts/ngc_debug.py` & `jammy-0.1.9/jammy/cli_scripts/ngc_debug.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/cli_scripts/shell_executor.py` & `jammy-0.1.9/jammy/cli_scripts/shell_executor.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/cli_scripts/sys_info.py` & `jammy-0.1.9/jammy/cli_scripts/sys_info.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/comm/cs.py` & `jammy-0.1.9/jammy/comm/cs.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/comm/utils.py` & `jammy-0.1.9/jammy/comm/utils.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/concurrency/__init__.py` & `jammy-0.1.9/jammy/concurrency/__init__.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/concurrency/packing.py` & `jammy-0.1.9/jammy/concurrency/packing.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/concurrency/zmq_utils.py` & `jammy-0.1.9/jammy/concurrency/zmq_utils.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/event/registry.py` & `jammy-0.1.9/jammy/event/registry.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/image/backend.py` & `jammy-0.1.9/jammy/image/backend.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/image/codecs.py` & `jammy-0.1.9/jammy/image/codecs.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/image/imgio.py` & `jammy-0.1.9/jammy/image/imgio.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/image/imgproc.py` & `jammy-0.1.9/jammy/image/imgproc.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/io/common.py` & `jammy-0.1.9/jammy/io/common.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/io/fs.py` & `jammy-0.1.9/jammy/io/fs.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/io/path.py` & `jammy-0.1.9/jammy/io/path.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/logging/logger.py` & `jammy-0.1.9/jammy/logging/logger.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,25 @@
-import os
 import sys
 
 from loguru import logger
 
 __all__ = [
     "get_logger",
-    "add_relative_path",
     "LOG_FORMAT",
 ]
 
 logger.remove()
 
 logger_sink = {}
 LOG_FORMAT = (
     "[<green>{time:MM-DD HH:mm:ss}</green>|"
-    "<red>[{process.name}]</red>|"
+    "<red>{process.name}</red>|"
     "<level>{level: <8}</level>|"
-    "<cyan>{extra[relative_path]}:{line}:{function}</cyan>]<level>{message}</level>"
-)
-
-
-def add_relative_path(record):
-    start = os.getcwd()
-    record["extra"]["relative_path"] = os.path.relpath(record["file"].path, start)
-
-
-*options, _, extra = logger._options  # pylint: disable=protected-access
-logger._options = tuple(  # pylint: disable=protected-access
-    [*options, add_relative_path, extra]
+    "<cyan>{file.path}</cyan>:<cyan>{line}</cyan>:<cyan>{function}</cyan>]"
+    "<level>{message}</level>"
 )
 
 
 def get_logger(file_name=None, clear=False, **kwargs):
     global logger_sink  # pylint: disable=global-statement,global-variable-not-assigned
     if clear:
         logger.remove()
```

### Comparing `jammy-0.1.8/jammy/logging/wandb_utils.py` & `jammy-0.1.9/jammy/logging/wandb_utils.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/random/_lazy_bind.py` & `jammy-0.1.9/jammy/random/_lazy_bind.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/random/rng.py` & `jammy-0.1.9/jammy/random/rng.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/storage/attr_saver.py` & `jammy-0.1.9/jammy/storage/attr_saver.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/storage/kv/kv.py` & `jammy-0.1.9/jammy/storage/kv/kv.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/storage/kv/lmdb.py` & `jammy-0.1.9/jammy/storage/kv/lmdb.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/storage/kv/mem.py` & `jammy-0.1.9/jammy/storage/kv/mem.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/storage/kv/memcached.py` & `jammy-0.1.9/jammy/storage/kv/memcached.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/argument.py` & `jammy-0.1.9/jammy/utils/argument.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/cache.py` & `jammy-0.1.9/jammy/utils/cache.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/cfg.py` & `jammy-0.1.9/jammy/utils/cfg.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/cnt.py` & `jammy-0.1.9/jammy/utils/cnt.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/colored_tqdm.py` & `jammy-0.1.9/jammy/utils/colored_tqdm.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/container.py` & `jammy-0.1.9/jammy/utils/container.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/debug.py` & `jammy-0.1.9/jammy/utils/debug.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/defaults.py` & `jammy-0.1.9/jammy/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/deprecated.py` & `jammy-0.1.9/jammy/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/enum.py` & `jammy-0.1.9/jammy/utils/enum.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/env.py` & `jammy-0.1.9/jammy/utils/env.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/filelock.py` & `jammy-0.1.9/jammy/utils/filelock.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/git.py` & `jammy-0.1.9/jammy/utils/git.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/gpu.py` & `jammy-0.1.9/jammy/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/hyd.py` & `jammy-0.1.9/jammy/utils/hyd.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/imp.py` & `jammy-0.1.9/jammy/utils/imp.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/init.py` & `jammy-0.1.9/jammy/utils/init.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/inspect.py` & `jammy-0.1.9/jammy/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/matching.py` & `jammy-0.1.9/jammy/utils/matching.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/meta.py` & `jammy-0.1.9/jammy/utils/meta.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/meter.py` & `jammy-0.1.9/jammy/utils/meter.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/naming.py` & `jammy-0.1.9/jammy/utils/naming.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/notifier.py` & `jammy-0.1.9/jammy/utils/notifier.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/printing.py` & `jammy-0.1.9/jammy/utils/printing.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/process.py` & `jammy-0.1.9/jammy/utils/process.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/profiler.py` & `jammy-0.1.9/jammy/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/registry.py` & `jammy-0.1.9/jammy/utils/registry.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/retry.py` & `jammy-0.1.9/jammy/utils/retry.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jammy/utils/sizeof.py` & `jammy-0.1.9/jammy/utils/sizeof.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamnp/buffer_storage.py` & `jammy-0.1.9/jamnp/buffer_storage.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamnp/container.py` & `jammy-0.1.9/jamnp/container.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/__init__.py` & `jammy-0.1.9/jamtorch/__init__.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/cuda/device.py` & `jammy-0.1.9/jamtorch/cuda/device.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/data/buffer_storage.py` & `jammy-0.1.9/jamtorch/data/buffer_storage.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/data/dataset.py` & `jammy-0.1.9/jamtorch/data/dataset.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/data/meta.py` & `jammy-0.1.9/jamtorch/data/meta.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/ddp/ddp_trainer.py` & `jammy-0.1.9/jamtorch/ddp/ddp_trainer.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/ddp/ddp_utils.py` & `jammy-0.1.9/jamtorch/ddp/ddp_utils.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/ddp/ema_trainer.py` & `jammy-0.1.9/jamtorch/ddp/ema_trainer.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/ddp/fns.py` & `jammy-0.1.9/jamtorch/ddp/fns.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/distributed/basic.py` & `jammy-0.1.9/jamtorch/distributed/basic.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/distributed/filelock.py` & `jammy-0.1.9/jamtorch/distributed/filelock.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/distributions/base.py` & `jammy-0.1.9/jamtorch/distributions/base.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/distributions/discrete.py` & `jammy-0.1.9/jamtorch/distributions/discrete.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/distributions/normal.py` & `jammy-0.1.9/jamtorch/distributions/normal.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/distributions/uniform.py` & `jammy-0.1.9/jamtorch/distributions/uniform.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/io/ckpt.py` & `jammy-0.1.9/jamtorch/io/ckpt.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/io/ema.py` & `jammy-0.1.9/jamtorch/io/ema.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/io/param_ema.py` & `jammy-0.1.9/jamtorch/io/param_ema.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/learn/gan/sn_discriminator.py` & `jammy-0.1.9/jamtorch/learn/gan/sn_discriminator.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/nn/base_modules.py` & `jammy-0.1.9/jamtorch/nn/base_modules.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/nn/fouriermlp.py` & `jammy-0.1.9/jamtorch/nn/fouriermlp.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/nn/seq.py` & `jammy-0.1.9/jamtorch/nn/seq.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/nn/simple_network.py` & `jammy-0.1.9/jamtorch/nn/simple_network.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/nn/utils/spectral_norm.py` & `jammy-0.1.9/jamtorch/nn/utils/spectral_norm.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/pl_callbacks/cuda_cb.py` & `jammy-0.1.9/jamtorch/pl_callbacks/cuda_cb.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/pl_callbacks/every_n.py` & `jammy-0.1.9/jamtorch/pl_callbacks/every_n.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/prototype/__init__.py` & `jammy-0.1.9/jamtorch/prototype/__init__.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/prototype/pytorch_util.py` & `jammy-0.1.9/jamtorch/prototype/pytorch_util.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/trainer/amp.py` & `jammy-0.1.9/jamtorch/trainer/amp.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/trainer/cfg_trainer.py` & `jammy-0.1.9/jamtorch/trainer/cfg_trainer.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/trainer/ema_trainer.py` & `jammy-0.1.9/jamtorch/trainer/ema_trainer.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/trainer/genetic_trainer.py` & `jammy-0.1.9/jamtorch/trainer/genetic_trainer.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/trainer/monitor.py` & `jammy-0.1.9/jamtorch/trainer/monitor.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/trainer/progress_fn.py` & `jammy-0.1.9/jamtorch/trainer/progress_fn.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/trainer/simple_trainer.py` & `jammy-0.1.9/jamtorch/trainer/simple_trainer.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/trainer/tb.py` & `jammy-0.1.9/jamtorch/trainer/tb.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/trainer/test_trainer.py` & `jammy-0.1.9/jamtorch/trainer/test_trainer.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/trainer/trainer.py` & `jammy-0.1.9/jamtorch/trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/trainer/trainer_fn.py` & `jammy-0.1.9/jamtorch/trainer/trainer_fn.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/trainer/trainer_monitor.py` & `jammy-0.1.9/jamtorch/trainer/trainer_monitor.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/trainer/utils.py` & `jammy-0.1.9/jamtorch/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/utils/deep_to.py` & `jammy-0.1.9/jamtorch/utils/deep_to.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/utils/init.py` & `jammy-0.1.9/jamtorch/utils/init.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/utils/meta.py` & `jammy-0.1.9/jamtorch/utils/meta.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/utils/pytree.py` & `jammy-0.1.9/jamtorch/utils/pytree.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamtorch/utils/ts_ops.py` & `jammy-0.1.9/jamtorch/utils/ts_ops.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamviz/img.py` & `jammy-0.1.9/jamviz/img.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamviz/plt/color_list.py` & `jammy-0.1.9/jamviz/plt/color_list.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamviz/plt/img.py` & `jammy-0.1.9/jamviz/plt/img.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamviz/plt/mstd.py` & `jammy-0.1.9/jamviz/plt/mstd.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamweb/session/memcached.py` & `jammy-0.1.9/jamweb/session/memcached.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamweb/session/session.py` & `jammy-0.1.9/jamweb/session/session.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/jamweb/web/application.py` & `jammy-0.1.9/jamweb/web/application.py`

 * *Files identical despite different names*

### Comparing `jammy-0.1.8/pyproject.toml` & `jammy-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jammy"
-version = "0.1.8"
+version = "0.1.9"
 description = "A Versatile ToolBox"
 authors = ["Qin <qsh.zh27@gmail.com>"]
 license = "MIT"
 packages = [
     { include="jammy" },
     { include="jamtorch" },
     { include="jamnp" },
@@ -13,22 +13,22 @@
 ]
 
 readme = "README.md"
 documentation = "https://jammy.readthedocs.io/en/latest/"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-numpy = "^1.20.3"
-scipy = "^1.6.3"
-loguru = "^0.6.0"
-einops = "^0.3.0"
+numpy = "^1.24.1"
+scipy = "^1.10.1"
+loguru = "^0.7.0"
+einops = "^0.6.0"
 hydra-core = "^1.1.0"
 GitPython = "^3.1.17"
 ipdb = "^0.13.8"
-matplotlib = "^3.3.0"
+matplotlib = "^3.7.1"
 gpustat = "^0.6.0"
 tqdm = "^4.11.0"
 attrs = "^20.3.0"
 
 # learn
 wandb = { version = "^0.10.31", optional = true }
```

### Comparing `jammy-0.1.8/PKG-INFO` & `jammy-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jammy
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Versatile ToolBox
 License: MIT
 Author: Qin
 Author-email: qsh.zh27@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,34 +15,34 @@
 Provides-Extra: all
 Provides-Extra: pro
 Provides-Extra: storage
 Provides-Extra: torch
 Provides-Extra: web
 Requires-Dist: GitPython (>=3.1.17,<4.0.0)
 Requires-Dist: attrs (>=20.3.0,<21.0.0)
-Requires-Dist: einops (>=0.3.0,<0.4.0)
+Requires-Dist: einops (>=0.6.0,<0.7.0)
 Requires-Dist: filelock (>=3.8.0,<4.0.0)
 Requires-Dist: gpustat (>=0.6.0,<0.7.0)
 Requires-Dist: h5py (>=3.4.0,<4.0.0) ; extra == "storage" or extra == "all"
 Requires-Dist: hydra-core (>=1.1.0,<2.0.0)
 Requires-Dist: ipdb (>=0.13.8,<0.14.0)
 Requires-Dist: line-profiler (>=3.3.1,<4.0.0) ; extra == "pro" or extra == "all"
 Requires-Dist: lmdb (>=1.2.1,<2.0.0) ; extra == "storage" or extra == "all"
-Requires-Dist: loguru (>=0.6.0,<0.7.0)
-Requires-Dist: matplotlib (>=3.3.0,<4.0.0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: msgpack (>=1.0.2,<2.0.0) ; extra == "storage" or extra == "all"
 Requires-Dist: msgpack-numpy (>=0.4.7,<0.5.0) ; extra == "storage" or extra == "all"
-Requires-Dist: numpy (>=1.20.3,<2.0.0)
+Requires-Dist: numpy (>=1.24.1,<2.0.0)
 Requires-Dist: parse (>=1.19.0,<2.0.0) ; extra == "pro" or extra == "all"
 Requires-Dist: pudb (>=2022.1,<2023.0) ; extra == "pro" or extra == "all"
 Requires-Dist: pyarrow (>=6.0.0,<7.0.0) ; extra == "storage" or extra == "all"
 Requires-Dist: python-memcached (>=1.59,<2.0) ; extra == "storage" or extra == "all"
 Requires-Dist: pytorch-lightning (>=1.5.10,<2.0.0) ; extra == "torch" or extra == "all"
 Requires-Dist: pyzmq (>=22.3.0,<23.0.0) ; extra == "web" or extra == "all"
-Requires-Dist: scipy (>=1.6.3,<2.0.0)
+Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: stackprinter (>=0.2.10,<0.3.0)
 Requires-Dist: timeout-decorator (>=0.5.0,<0.6.0)
 Requires-Dist: torch (>=1.10.0,<2.0.0) ; extra == "torch" or extra == "all"
 Requires-Dist: torchinfo (>=1.5.3,<2.0.0) ; extra == "torch" or extra == "all"
 Requires-Dist: torchvision (>=0.11.0,<0.12.0) ; extra == "torch" or extra == "all"
 Requires-Dist: tornado (>=6.1,<7.0) ; extra == "web" or extra == "all"
 Requires-Dist: tqdm (>=4.11.0,<5.0.0)
```

#### html2text {}

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1 Name: jammy Version: 0.1.8 Summary: A Versatile ToolBox
+Metadata-Version: 2.1 Name: jammy Version: 0.1.9 Summary: A Versatile ToolBox
 License: MIT Author: Qin Author-email: qsh.zh27@gmail.com Requires-Python:
 >=3.8,<3.12 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Provides-Extra: all Provides-Extra: pro Provides-Extra: storage
 Provides-Extra: torch Provides-Extra: web Requires-Dist: GitPython
 (>=3.1.17,<4.0.0) Requires-Dist: attrs (>=20.3.0,<21.0.0) Requires-Dist: einops
-(>=0.3.0,<0.4.0) Requires-Dist: filelock (>=3.8.0,<4.0.0) Requires-Dist:
+(>=0.6.0,<0.7.0) Requires-Dist: filelock (>=3.8.0,<4.0.0) Requires-Dist:
 gpustat (>=0.6.0,<0.7.0) Requires-Dist: h5py (>=3.4.0,<4.0.0) ; extra ==
 "storage" or extra == "all" Requires-Dist: hydra-core (>=1.1.0,<2.0.0)
 Requires-Dist: ipdb (>=0.13.8,<0.14.0) Requires-Dist: line-profiler
 (>=3.3.1,<4.0.0) ; extra == "pro" or extra == "all" Requires-Dist: lmdb
 (>=1.2.1,<2.0.0) ; extra == "storage" or extra == "all" Requires-Dist: loguru
-(>=0.6.0,<0.7.0) Requires-Dist: matplotlib (>=3.3.0,<4.0.0) Requires-Dist:
+(>=0.7.0,<0.8.0) Requires-Dist: matplotlib (>=3.7.1,<4.0.0) Requires-Dist:
 msgpack (>=1.0.2,<2.0.0) ; extra == "storage" or extra == "all" Requires-Dist:
 msgpack-numpy (>=0.4.7,<0.5.0) ; extra == "storage" or extra == "all" Requires-
-Dist: numpy (>=1.20.3,<2.0.0) Requires-Dist: parse (>=1.19.0,<2.0.0) ; extra ==
+Dist: numpy (>=1.24.1,<2.0.0) Requires-Dist: parse (>=1.19.0,<2.0.0) ; extra ==
 "pro" or extra == "all" Requires-Dist: pudb (>=2022.1,<2023.0) ; extra == "pro"
 or extra == "all" Requires-Dist: pyarrow (>=6.0.0,<7.0.0) ; extra == "storage"
 or extra == "all" Requires-Dist: python-memcached (>=1.59,<2.0) ; extra ==
 "storage" or extra == "all" Requires-Dist: pytorch-lightning (>=1.5.10,<2.0.0)
 ; extra == "torch" or extra == "all" Requires-Dist: pyzmq (>=22.3.0,<23.0.0) ;
-extra == "web" or extra == "all" Requires-Dist: scipy (>=1.6.3,<2.0.0)
+extra == "web" or extra == "all" Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: stackprinter (>=0.2.10,<0.3.0) Requires-Dist: timeout-decorator
 (>=0.5.0,<0.6.0) Requires-Dist: torch (>=1.10.0,<2.0.0) ; extra == "torch" or
 extra == "all" Requires-Dist: torchinfo (>=1.5.3,<2.0.0) ; extra == "torch" or
 extra == "all" Requires-Dist: torchvision (>=0.11.0,<0.12.0) ; extra == "torch"
 or extra == "all" Requires-Dist: tornado (>=6.1,<7.0) ; extra == "web" or extra
 == "all" Requires-Dist: tqdm (>=4.11.0,<5.0.0) Requires-Dist: ubelt
 (>=0.10.2,<0.11.0) ; extra == "pro" or extra == "all" Requires-Dist: wandb
```

