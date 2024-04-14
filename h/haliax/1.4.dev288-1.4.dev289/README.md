# Comparing `tmp/haliax-1.4.dev288.tar.gz` & `tmp/haliax-1.4.dev289.tar.gz`

## Comparing `haliax-1.4.dev288.tar` & `haliax-1.4.dev289.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 haliax-1.4.dev288/.coveragerc
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 haliax-1.4.dev288/.flake8
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 haliax-1.4.dev288/.pre-commit-config.yaml
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 haliax-1.4.dev288/.readthedocs.yaml
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 haliax-1.4.dev288/CONTRIBUTING.md
--rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 haliax-1.4.dev288/mkdocs.yml
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 haliax-1.4.dev288/.github/workflows/publish_dev.yaml
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 haliax-1.4.dev288/.github/workflows/run_pre_commit.yaml
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 haliax-1.4.dev288/.github/workflows/run_tests.yaml
--rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 haliax-1.4.dev288/docs/api.md
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 haliax-1.4.dev288/docs/broadcasting.md
--rw-r--r--   0        0        0    11861 2020-02-02 00:00:00.000000 haliax-1.4.dev288/docs/cheatsheet.md
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 haliax-1.4.dev288/docs/faq.md
--rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 haliax-1.4.dev288/docs/fp8.md
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 haliax-1.4.dev288/docs/hof.md
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 haliax-1.4.dev288/docs/index.md
--rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 haliax-1.4.dev288/docs/indexing.md
--rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 haliax-1.4.dev288/docs/matmul.md
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 haliax-1.4.dev288/docs/nn.md
--rw-r--r--   0        0        0     5298 2020-02-02 00:00:00.000000 haliax-1.4.dev288/docs/partitioning.md
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 haliax-1.4.dev288/docs/rearrange.ipynb
--rw-r--r--   0        0        0     8230 2020-02-02 00:00:00.000000 haliax-1.4.dev288/docs/rearrange.md
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 haliax-1.4.dev288/docs/requirements.txt
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 haliax-1.4.dev288/docs/tutorial.md
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 haliax-1.4.dev288/docs/css/material.css
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 haliax-1.4.dev288/docs/css/mkdocstrings.css
--rw-r--r--   0        0        0    42926 2020-02-02 00:00:00.000000 haliax-1.4.dev288/docs/figures/data_parallel_mesh.png
--rw-r--r--   0        0        0    50540 2020-02-02 00:00:00.000000 haliax-1.4.dev288/docs/figures/data_parallel_mesh_replicated.png
--rw-r--r--   0        0        0    27854 2020-02-02 00:00:00.000000 haliax-1.4.dev288/docs/figures/device_mesh_1d.png
--rw-r--r--   0        0        0   134942 2020-02-02 00:00:00.000000 haliax-1.4.dev288/docs/figures/device_mesh_1d_zero.png
--rw-r--r--   0        0        0    55907 2020-02-02 00:00:00.000000 haliax-1.4.dev288/docs/figures/device_mesh_2d.png
--rw-r--r--   0        0        0    72933 2020-02-02 00:00:00.000000 haliax-1.4.dev288/docs/figures/device_mesh_2d_batch_partitioned.png
--rw-r--r--   0        0        0    72933 2020-02-02 00:00:00.000000 haliax-1.4.dev288/docs/figures/device_mesh_2d_data_replicated.png
--rw-r--r--   0        0        0   134044 2020-02-02 00:00:00.000000 haliax-1.4.dev288/docs/figures/device_mesh_2d_data_replicated_mlp_partitioned.png
--rw-r--r--   0        0        0   155097 2020-02-02 00:00:00.000000 haliax-1.4.dev288/docs/figures/device_mesh_2d_intermediate_fully_partitioned.png
--rw-r--r--   0        0        0   165402 2020-02-02 00:00:00.000000 haliax-1.4.dev288/docs/figures/device_mesh_2d_zero.png
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/__about__.py
--rw-r--r--   0        0        0    28790 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/__init__.py
--rw-r--r--   0        0        0    17892 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/axis.py
--rw-r--r--   0        0        0    55808 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/core.py
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/debug.py
--rw-r--r--   0        0        0    18205 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/hof.py
--rw-r--r--   0        0        0     6298 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/jax_utils.py
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/ops.py
--rw-r--r--   0        0        0    22548 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/partitioning.py
--rw-r--r--   0        0        0     9442 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/quantization.py
--rw-r--r--   0        0        0    13077 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/random.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/specialized_fns.py
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/tree_util.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/types.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/util.py
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/wrap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/_src/__init__.py
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/_src/compile_utils.py
--rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/_src/dot.py
--rw-r--r--   0        0        0    11696 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/_src/einsum.py
--rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/_src/fp8.py
--rw-r--r--   0        0        0    10691 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/_src/parsing.py
--rw-r--r--   0        0        0    19498 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/_src/rearrange.py
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/_src/util.py
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/nn/__init__.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/nn/activations.py
--rw-r--r--   0        0        0    11718 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/nn/attention.py
--rw-r--r--   0        0        0    15131 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/nn/conv.py
--rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/nn/dropout.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/nn/embedding.py
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/nn/linear.py
--rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/nn/loss.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/nn/mlp.py
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/nn/normalization.py
--rw-r--r--   0        0        0     8513 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/nn/pool.py
--rw-r--r--   0        0        0    10226 2020-02-02 00:00:00.000000 haliax-1.4.dev288/src/haliax/nn/scan.py
--rw-r--r--   0        0        0    30258 2020-02-02 00:00:00.000000 haliax-1.4.dev288/tests/core_test.py
--rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 haliax-1.4.dev288/tests/test_attention.py
--rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 haliax-1.4.dev288/tests/test_axis.py
--rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 haliax-1.4.dev288/tests/test_conv.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 haliax-1.4.dev288/tests/test_debug.py
--rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 haliax-1.4.dev288/tests/test_dot.py
--rw-r--r--   0        0        0     8242 2020-02-02 00:00:00.000000 haliax-1.4.dev288/tests/test_einsum.py
--rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 haliax-1.4.dev288/tests/test_fp8.py
--rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 haliax-1.4.dev288/tests/test_hof.py
--rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 haliax-1.4.dev288/tests/test_nn.py
--rw-r--r--   0        0        0     8078 2020-02-02 00:00:00.000000 haliax-1.4.dev288/tests/test_ops.py
--rw-r--r--   0        0        0     6910 2020-02-02 00:00:00.000000 haliax-1.4.dev288/tests/test_parsing.py
--rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 haliax-1.4.dev288/tests/test_partitioning.py
--rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 haliax-1.4.dev288/tests/test_pool.py
--rw-r--r--   0        0        0    11284 2020-02-02 00:00:00.000000 haliax-1.4.dev288/tests/test_random.py
--rw-r--r--   0        0        0    14465 2020-02-02 00:00:00.000000 haliax-1.4.dev288/tests/test_rearrange.py
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 haliax-1.4.dev288/tests/test_scan.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 haliax-1.4.dev288/tests/test_specialized_fns.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 haliax-1.4.dev288/tests/test_tree_util.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 haliax-1.4.dev288/tests/test_utils.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 haliax-1.4.dev288/.gitignore
--rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 haliax-1.4.dev288/LICENSE
--rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 haliax-1.4.dev288/README.md
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 haliax-1.4.dev288/pyproject.toml
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 haliax-1.4.dev288/PKG-INFO
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 haliax-1.4.dev289/.coveragerc
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 haliax-1.4.dev289/.flake8
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 haliax-1.4.dev289/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 haliax-1.4.dev289/.readthedocs.yaml
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 haliax-1.4.dev289/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 haliax-1.4.dev289/mkdocs.yml
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 haliax-1.4.dev289/.github/workflows/publish_dev.yaml
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 haliax-1.4.dev289/.github/workflows/run_pre_commit.yaml
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 haliax-1.4.dev289/.github/workflows/run_tests.yaml
+-rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 haliax-1.4.dev289/docs/api.md
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 haliax-1.4.dev289/docs/broadcasting.md
+-rw-r--r--   0        0        0    11861 2020-02-02 00:00:00.000000 haliax-1.4.dev289/docs/cheatsheet.md
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 haliax-1.4.dev289/docs/faq.md
+-rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 haliax-1.4.dev289/docs/fp8.md
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 haliax-1.4.dev289/docs/hof.md
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 haliax-1.4.dev289/docs/index.md
+-rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 haliax-1.4.dev289/docs/indexing.md
+-rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 haliax-1.4.dev289/docs/matmul.md
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 haliax-1.4.dev289/docs/nn.md
+-rw-r--r--   0        0        0     5298 2020-02-02 00:00:00.000000 haliax-1.4.dev289/docs/partitioning.md
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 haliax-1.4.dev289/docs/rearrange.ipynb
+-rw-r--r--   0        0        0     8230 2020-02-02 00:00:00.000000 haliax-1.4.dev289/docs/rearrange.md
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 haliax-1.4.dev289/docs/requirements.txt
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 haliax-1.4.dev289/docs/tutorial.md
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 haliax-1.4.dev289/docs/css/material.css
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 haliax-1.4.dev289/docs/css/mkdocstrings.css
+-rw-r--r--   0        0        0    42926 2020-02-02 00:00:00.000000 haliax-1.4.dev289/docs/figures/data_parallel_mesh.png
+-rw-r--r--   0        0        0    50540 2020-02-02 00:00:00.000000 haliax-1.4.dev289/docs/figures/data_parallel_mesh_replicated.png
+-rw-r--r--   0        0        0    27854 2020-02-02 00:00:00.000000 haliax-1.4.dev289/docs/figures/device_mesh_1d.png
+-rw-r--r--   0        0        0   134942 2020-02-02 00:00:00.000000 haliax-1.4.dev289/docs/figures/device_mesh_1d_zero.png
+-rw-r--r--   0        0        0    55907 2020-02-02 00:00:00.000000 haliax-1.4.dev289/docs/figures/device_mesh_2d.png
+-rw-r--r--   0        0        0    72933 2020-02-02 00:00:00.000000 haliax-1.4.dev289/docs/figures/device_mesh_2d_batch_partitioned.png
+-rw-r--r--   0        0        0    72933 2020-02-02 00:00:00.000000 haliax-1.4.dev289/docs/figures/device_mesh_2d_data_replicated.png
+-rw-r--r--   0        0        0   134044 2020-02-02 00:00:00.000000 haliax-1.4.dev289/docs/figures/device_mesh_2d_data_replicated_mlp_partitioned.png
+-rw-r--r--   0        0        0   155097 2020-02-02 00:00:00.000000 haliax-1.4.dev289/docs/figures/device_mesh_2d_intermediate_fully_partitioned.png
+-rw-r--r--   0        0        0   165402 2020-02-02 00:00:00.000000 haliax-1.4.dev289/docs/figures/device_mesh_2d_zero.png
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/__about__.py
+-rw-r--r--   0        0        0    28790 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/__init__.py
+-rw-r--r--   0        0        0    17892 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/axis.py
+-rw-r--r--   0        0        0    55871 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/core.py
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/debug.py
+-rw-r--r--   0        0        0    18205 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/hof.py
+-rw-r--r--   0        0        0     6298 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/jax_utils.py
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/ops.py
+-rw-r--r--   0        0        0    22548 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/partitioning.py
+-rw-r--r--   0        0        0     9442 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/quantization.py
+-rw-r--r--   0        0        0    13077 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/random.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/specialized_fns.py
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/tree_util.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/types.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/util.py
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/wrap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/_src/__init__.py
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/_src/compile_utils.py
+-rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/_src/dot.py
+-rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/_src/einsum.py
+-rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/_src/fp8.py
+-rw-r--r--   0        0        0    11189 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/_src/parsing.py
+-rw-r--r--   0        0        0    19498 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/_src/rearrange.py
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/_src/util.py
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/nn/__init__.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/nn/activations.py
+-rw-r--r--   0        0        0    11718 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/nn/attention.py
+-rw-r--r--   0        0        0    15131 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/nn/conv.py
+-rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/nn/dropout.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/nn/embedding.py
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/nn/linear.py
+-rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/nn/loss.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/nn/mlp.py
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/nn/normalization.py
+-rw-r--r--   0        0        0     8513 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/nn/pool.py
+-rw-r--r--   0        0        0    10226 2020-02-02 00:00:00.000000 haliax-1.4.dev289/src/haliax/nn/scan.py
+-rw-r--r--   0        0        0    30258 2020-02-02 00:00:00.000000 haliax-1.4.dev289/tests/core_test.py
+-rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 haliax-1.4.dev289/tests/test_attention.py
+-rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 haliax-1.4.dev289/tests/test_axis.py
+-rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 haliax-1.4.dev289/tests/test_conv.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 haliax-1.4.dev289/tests/test_debug.py
+-rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 haliax-1.4.dev289/tests/test_dot.py
+-rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 haliax-1.4.dev289/tests/test_einsum.py
+-rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 haliax-1.4.dev289/tests/test_fp8.py
+-rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 haliax-1.4.dev289/tests/test_hof.py
+-rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 haliax-1.4.dev289/tests/test_nn.py
+-rw-r--r--   0        0        0     8078 2020-02-02 00:00:00.000000 haliax-1.4.dev289/tests/test_ops.py
+-rw-r--r--   0        0        0     6910 2020-02-02 00:00:00.000000 haliax-1.4.dev289/tests/test_parsing.py
+-rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 haliax-1.4.dev289/tests/test_partitioning.py
+-rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 haliax-1.4.dev289/tests/test_pool.py
+-rw-r--r--   0        0        0    11284 2020-02-02 00:00:00.000000 haliax-1.4.dev289/tests/test_random.py
+-rw-r--r--   0        0        0    14465 2020-02-02 00:00:00.000000 haliax-1.4.dev289/tests/test_rearrange.py
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 haliax-1.4.dev289/tests/test_scan.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 haliax-1.4.dev289/tests/test_specialized_fns.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 haliax-1.4.dev289/tests/test_tree_util.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 haliax-1.4.dev289/tests/test_utils.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 haliax-1.4.dev289/.gitignore
+-rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 haliax-1.4.dev289/LICENSE
+-rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 haliax-1.4.dev289/README.md
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 haliax-1.4.dev289/pyproject.toml
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 haliax-1.4.dev289/PKG-INFO
```

### Comparing `haliax-1.4.dev288/.pre-commit-config.yaml` & `haliax-1.4.dev289/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/CONTRIBUTING.md` & `haliax-1.4.dev289/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/mkdocs.yml` & `haliax-1.4.dev289/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/.github/workflows/publish_dev.yaml` & `haliax-1.4.dev289/.github/workflows/publish_dev.yaml`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/.github/workflows/run_pre_commit.yaml` & `haliax-1.4.dev289/.github/workflows/run_pre_commit.yaml`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/.github/workflows/run_tests.yaml` & `haliax-1.4.dev289/.github/workflows/run_tests.yaml`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/docs/api.md` & `haliax-1.4.dev289/docs/api.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/docs/broadcasting.md` & `haliax-1.4.dev289/docs/broadcasting.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/docs/cheatsheet.md` & `haliax-1.4.dev289/docs/cheatsheet.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/docs/faq.md` & `haliax-1.4.dev289/docs/faq.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/docs/fp8.md` & `haliax-1.4.dev289/docs/fp8.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/docs/indexing.md` & `haliax-1.4.dev289/docs/indexing.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/docs/matmul.md` & `haliax-1.4.dev289/docs/matmul.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 ## Matrix Multiplication
 
 Haliax has two ways to do matrix multiplication (and tensor contractions more generally):
 [haliax.dot][] and [haliax.einsum][]. [haliax.dot][] and [haliax.einsum][]
 can both express any tensor contraction, though in different situations one or the other may be
-more suitable for expressing a particular contraction.
+more suitable for expressing a particular contraction In general:
+
+- Use [haliax.dot][] when you want to express a simple matrix multiplication over one or a few axes.
+- Use [haliax.einsum][] when you want to express a more complex tensor contraction.
 
 See also the API reference for [haliax.dot][] and [haliax.einsum][] and the
 [cheat sheet section](cheatsheet.md#matrix-multiplication).
 
 ### `haliax.dot`
 
 With [haliax.dot][], you specify the axes to contract over, without needing to write out the
@@ -64,14 +67,17 @@
 it supports long names for axes (like `"batch h w, h w channel -> batch channel"`)
 rather than the compact notation of `numpy.einsum` (like `"bhwc,hwc->bc"`).
 
 Haliax's version of `einsum` comes in three modes: "ordered", "unordered", and "output axes".
 These modes are all accessible through the same function without any flags: the syntax
 of the `einsum` string determines which mode is used.
 
+The syntax for Haliax's `einsum` is similar to [`haliax.rearrange`](rearrange.md), which
+is in turn similar to [einops.rearrange](https://einops.rocks/api/rearrange/).
+
 #### Ordered Mode
 
 Haliax's `einsum` has an "ordered" mode that is similar to `einops.einsum`'s behavior.
 In this mode, the axes in the input arrays are matched to the axes in the `einsum` string in order.
 It supports ellipses in the same way as `einops.einsum`. The names in the einsum string need not
 match the names of the axes in the input arrays, but the order of the axes must match.
 
@@ -115,14 +121,30 @@
 y = hax.einsum("{...} -> ", x)  # shape is ()
 y = hax.einsum("{H ...} -> H", x)  # shape is (H,)
 y = hax.einsum("{H ...} -> ...", x)  # shape is (W, D)
 ```
 
 This mode is most similar to [haliax.dot][]'s behavior, though it's a bit more expressive.
 
+You can also use axis aliases in the `einsum` string, which can be useful for expressing contractions
+in library code or just for shortening the string:
+
+```python
+Height = hax.Axis("Height", 3)
+Width = hax.Axis("Width", 4)
+Depth = hax.Axis("Depth", 5)
+
+x = hax.ones((Height, Width, Depth))
+w = hax.ones((Depth,))
+
+y = hax.einsum("{H W D} -> H W", x, H=Height, W=Width, D=Depth)  # shape is (Height, Width)
+y = hax.einsum("{D} -> ", w, D=Depth)  # shape is (Height, Width)
+```
+
+
 #### Output Axes Mode
 
 In "output axes" mode, you only specify the axes that should be in the output. All other
 axes are implicitly contracted over. This mode is a bit "dangerous" in that it's easy to
 accidentally contract over axes you didn't mean to, but it can be useful for expressing
 certain contractions concisely.
 
@@ -138,7 +160,20 @@
 
 y = hax.einsum("-> H W", x)  # shape is (H, W)
 y = hax.einsum("-> D", w)  # shape is (D,)
 ```
 
 We don't recommend using this mode except in cases when you're sure of the full shape of the input arrays
 or you are sure you don't want to let users implicitly batch over any axes.
+
+Output axes mode also supports axis aliases:
+
+```python
+Height = hax.Axis("Height", 3)
+Width = hax.Axis("Width", 4)
+Depth = hax.Axis("Depth", 5)
+
+x = hax.ones((Height, Width, Depth))
+w = hax.ones((Depth,))
+y = hax.einsum("-> Height Width", x, Height=Height, Width=Width, Depth=Depth)  # shape is (Height, Width)
+y = hax.einsum("-> Depth", w, Depth=Depth)  # shape is (Depth,)
+```
```

### Comparing `haliax-1.4.dev288/docs/nn.md` & `haliax-1.4.dev289/docs/nn.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/docs/partitioning.md` & `haliax-1.4.dev289/docs/partitioning.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/docs/rearrange.ipynb` & `haliax-1.4.dev289/docs/rearrange.ipynb`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/docs/rearrange.md` & `haliax-1.4.dev289/docs/rearrange.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/docs/css/material.css` & `haliax-1.4.dev289/docs/css/material.css`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/docs/css/mkdocstrings.css` & `haliax-1.4.dev289/docs/css/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/docs/figures/data_parallel_mesh.png` & `haliax-1.4.dev289/docs/figures/data_parallel_mesh.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/docs/figures/data_parallel_mesh_replicated.png` & `haliax-1.4.dev289/docs/figures/data_parallel_mesh_replicated.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/docs/figures/device_mesh_1d.png` & `haliax-1.4.dev289/docs/figures/device_mesh_1d.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/docs/figures/device_mesh_1d_zero.png` & `haliax-1.4.dev289/docs/figures/device_mesh_1d_zero.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/docs/figures/device_mesh_2d.png` & `haliax-1.4.dev289/docs/figures/device_mesh_2d.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/docs/figures/device_mesh_2d_batch_partitioned.png` & `haliax-1.4.dev289/docs/figures/device_mesh_2d_batch_partitioned.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/docs/figures/device_mesh_2d_data_replicated.png` & `haliax-1.4.dev289/docs/figures/device_mesh_2d_data_replicated.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/docs/figures/device_mesh_2d_data_replicated_mlp_partitioned.png` & `haliax-1.4.dev289/docs/figures/device_mesh_2d_data_replicated_mlp_partitioned.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/docs/figures/device_mesh_2d_intermediate_fully_partitioned.png` & `haliax-1.4.dev289/docs/figures/device_mesh_2d_intermediate_fully_partitioned.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/docs/figures/device_mesh_2d_zero.png` & `haliax-1.4.dev289/docs/figures/device_mesh_2d_zero.png`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/__init__.py` & `haliax-1.4.dev289/src/haliax/__init__.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/axis.py` & `haliax-1.4.dev289/src/haliax/axis.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/core.py` & `haliax-1.4.dev289/src/haliax/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,14 +180,16 @@
     def resolve_axis(self, axis: Sequence[AxisSelector]) -> Tuple[Axis, ...]:  # type: ignore
         ...
 
     def resolve_axis(self, axes: AxisSelection) -> AxisSpec:  # type: ignore
         """
         Returns the axes corresponding to the given axis selection.
         That is, it return the [haliax.Axis][] values themselves, not just their names.
+
+        Raises a ValueError if any of the axes are not found.
         """
         indices = self._lookup_indices(axes)
         if isinstance(indices, int):
             return self.axes[indices]
         elif indices is None:
             raise ValueError(f"Axis {axes} not found")
         else:
```

### Comparing `haliax-1.4.dev288/src/haliax/debug.py` & `haliax-1.4.dev289/src/haliax/debug.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/hof.py` & `haliax-1.4.dev289/src/haliax/hof.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/jax_utils.py` & `haliax-1.4.dev289/src/haliax/jax_utils.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/ops.py` & `haliax-1.4.dev289/src/haliax/ops.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/partitioning.py` & `haliax-1.4.dev289/src/haliax/partitioning.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/quantization.py` & `haliax-1.4.dev289/src/haliax/quantization.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/random.py` & `haliax-1.4.dev289/src/haliax/random.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/specialized_fns.py` & `haliax-1.4.dev289/src/haliax/specialized_fns.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/tree_util.py` & `haliax-1.4.dev289/src/haliax/tree_util.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/types.py` & `haliax-1.4.dev289/src/haliax/types.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/util.py` & `haliax-1.4.dev289/src/haliax/util.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/wrap.py` & `haliax-1.4.dev289/src/haliax/wrap.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/_src/compile_utils.py` & `haliax-1.4.dev289/src/haliax/_src/compile_utils.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/_src/dot.py` & `haliax-1.4.dev289/src/haliax/_src/dot.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/_src/einsum.py` & `haliax-1.4.dev289/src/haliax/_src/einsum.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import functools
 from types import EllipsisType
-from typing import Optional, Sequence, Tuple, Union
+from typing import Optional, Tuple
 
 import jax.lax
-import jax.numpy as jnp
 
 import haliax
 
-from ..axis import AxisSelector, axis_name, eliminate_axes, rearrange_for_partial_order, union_axes
+from ..axis import Axis, AxisSelector, axis_name, eliminate_axes, rearrange_for_partial_order, union_axes
 from ..core import NamedArray
 from ..jax_utils import _jittable_dg_einsum
 from ..types import DTypeLike, PrecisionLike
 from ..util import ensure_tuple
 from .parsing import AliasTable, parse_einsum, raise_parse_error
 
 
 def einsum(
     equation: str,
     *arrays: NamedArray,
     precision: PrecisionLike = None,
     preferred_element_type: Optional[DTypeLike] = None,
     _dot_general=jax.lax.dot_general,
+    **axis_aliases,
 ) -> NamedArray:
     """Compute the tensor contraction of the input arrays according to Haliax's named variant of the Einstein summation
     convention.
 
     Examples:
        >>> # normal einsum
        >>> import haliax as hax
@@ -34,20 +34,24 @@
        >>> a = hax.zeros((H, W, D))
        >>> b = hax.zeros((D, W, H))
        >>> hax.einsum("h w d, d w h -> h w", a, b)
        >>> # named einsum
        >>> hax.einsum("{H W D} -> H W", a, b)
        >>> hax.einsum("{D} -> ", a, b)  # same as the previous example
        >>> hax.einsum("-> H W", a, b)  # same as the first example
+       >>> # axis aliases, useful for generic code
+       >>> hax.einsum("{x y} -> y", a, b, x=H, y=W)
 
     Args:
        equation: The einsum equation.
        arrays: The input arrays.
        precision: The precision of the computation.
        preferred_element_type: The preferred element type of the computation.
+       _dot_general: The dot_general function to use.
+       axis_aliases: The axis aliases to use.
 
     Returns:
        The result of the einsum.
     """
     lhses, rhs = parse_einsum(equation)
 
     # we have essentially 3 cases:
@@ -55,44 +59,46 @@
     # 2. named einsum where a subset of dims are contracted and the rest are kept
     # 3. named einsum without an lhs, with a specific set of dims to keep on the rhs
     # in each case we need
 
     # NB: we're using JAX's einsum which only supports one letter names for dims
     if len(lhses) == 1 and len(lhses[0].captures) == 0 and lhses[0].is_ordered:
         # case 3: get the output axes, contract the others
-        spec, out_axes = _output_only_named_einsum(equation, arrays, rhs)
+        spec, out_axes = _output_only_named_einsum(equation, arrays, rhs, axis_aliases)
     elif len(lhses) == 1 and not lhses[0].is_ordered:
         # case 2: some axes are named. Those named only on the lhs are contracted, the others are kept
         # subcase: if there's an ellipsis on the lhs, we contract all the axes that are not named on the rhs
-        spec, out_axes = _unordered_einsum(arrays, equation, lhses, rhs)
+        spec, out_axes = _unordered_einsum(arrays, equation, lhses[0], rhs, axis_aliases)
     else:
         # general case: we have a normal einsum. we don't allow unordered axes here
         if any(not lhs.is_ordered for lhs in lhses):
             raise_parse_error("Cannot have multiple unordered axes in an einsum", equation, None)
 
-        spec, out_axes = _positional_einsum_spec(equation, arrays, lhses, rhs)
+        spec, out_axes = _positional_einsum_spec(equation, arrays, lhses, rhs, axis_aliases)
 
     out_raw = _jittable_dg_einsum(
         spec,
         *[a.array for a in arrays],
         precision=precision,
         preferred_element_type=preferred_element_type,
         _dot_general=_dot_general,
     )
 
     out = haliax.named(out_raw, out_axes)
     return haliax.auto_sharded(out)
 
 
-def _unordered_einsum(arrays, equation, lhses, rhs):
-    used_letters: set[str] = set()
-    name_mappings_for_einsum: dict[str, str] = {}
-    lhs = lhses[0]
-    candidate_axes, has_ellipsis_lhs = _captures_to_axis_names(equation, lhs)
-    rhs_axes, has_ellipsis_rhs = _captures_to_axis_names(equation, rhs)
+def _unordered_einsum(arrays, equation, lhs, rhs, axis_aliases):
+    candidate_axes, has_ellipsis_lhs, covered_lhs = _captures_to_axis_names(equation, lhs, axis_aliases)
+    rhs_axes, has_ellipsis_rhs, covered_rhs = _captures_to_axis_names(equation, rhs, axis_aliases)
+
+    for alias_name in axis_aliases:
+        if alias_name not in covered_lhs and alias_name not in covered_rhs:
+            raise_parse_error(f"Axis alias {alias_name} not used in the einsum", equation, None)
+
     all_input_axes = _all_input_axes(arrays)
     if has_ellipsis_rhs:
         out_axes = rearrange_for_partial_order(rhs_axes, all_input_axes)
 
     elif has_ellipsis_lhs:
         # if the lhs has an ellipsis but not the right, we contract all the axes that are not named on the rhs
         out_axes = tuple(rhs_axes)
@@ -101,51 +107,81 @@
         # if neither has an ellipsis, we contract the axes that are named on the lhs but not on the rhs
         almost_out_axes = eliminate_axes(all_input_axes, named_on_left_but_not_right)  # type: ignore
         # we now need to rearrange to be consistent with the rhs order.
         # since there's no ellipsis on the rhs, we arbitrarily insert one at the beginning which is usually
         # what people expect
         rhs_axes = [Ellipsis] + rhs_axes  # type: ignore
         out_axes = rearrange_for_partial_order(rhs_axes, almost_out_axes)
-    spec = _make_einsum_spec(name_mappings_for_einsum, used_letters, arrays, out_axes)
+    spec = _make_einsum_spec(arrays, out_axes)
     return spec, out_axes
 
 
-def _output_only_named_einsum(equation, arrays, rhs):
-    used_letters: set[str] = set()
-    name_mappings_for_einsum: dict[str, str] = {}
-
+def _output_only_named_einsum(equation, arrays, rhs, axis_aliases):
     out_axes = []
+    used_axes = set()
+    used_aliases = set()
+
+    input_axis_names = set(ax.name for ax in _all_input_axes(arrays))
+
     for capture in rhs.captures:
         if capture is Ellipsis:
             raise_parse_error("Can't use ellipsis on the rhs of an einsum without an lhs", equation, None)
         elif capture.binding is None or len(capture.axes) > 1:
             raise_parse_error(
                 "Parenthesized axes are not currently supported in the output of an einsum",
                 equation,
                 capture.char_range,
             )
         else:
             name = capture.binding
+            used_aliases.add(name)
+
+            if name in axis_aliases:
+                # this could be axis or a name. if an axis, need to assert the size
+                axis = axis_aliases[name]
+                if isinstance(axis, Axis):
+                    _check_axis_size_consistency(arrays, axis, name)
+                ax_name = axis_name(axis)
+
+                if ax_name in used_axes:
+                    raise_parse_error(
+                        f"Axis {name} occurs multiple times on the rhs. Probably because of multiple aliasing?",
+                        equation,
+                        capture.char_range,
+                    )
+
+                name = ax_name
+                used_axes.add(name)
 
             if name in out_axes:
-                raise_parse_error(f"Axis name {name} occurs multiple times on the rhs", equation, capture.char_range)
+                raise_parse_error(
+                    f"Axis capture {name} occurs multiple times on the rhs", equation, capture.char_range
+                )
+
+            if name not in input_axis_names:
+                raise_parse_error(f"Axis {name} not found in any of the input arrays", equation, capture.char_range)
 
             out_axes.append(name)
 
-    spec = _make_einsum_spec(name_mappings_for_einsum, used_letters, arrays, out_axes)
+    _check_for_unused_aliases(axis_aliases, used_aliases, equation)
+
+    spec = _make_einsum_spec(arrays, out_axes)
     return spec, out_axes
 
 
-def _positional_einsum_spec(equation, arrays, lhses, rhs):
+def _positional_einsum_spec(equation, arrays, lhses, rhs, axis_aliases):
     used_letters: set[str] = set()
     name_mappings_for_einsum: dict[str, str] = {}
+    used_aliases = set()
 
     if len(lhses) != len(arrays):
         raise ValueError(f"Number of lhses ({len(lhses)}) does not match number of arrays ({len(arrays)})")
-    table = AliasTable()
+
+    # For this function, axis_aliases exists entirely for checking axis sizes against what's in the arrays
+    table = AliasTable(axis_aliases)
     # ok, we're going to lead pretty heavily on einsum here. We just need to figure out the names of the axes
     # and do any error checking (that there are no mismatched names)
     # once we do that, we can pass a slightly modified spec to einsum (namely that we shorten the names of the axes)
     # and we're good to go
     spec = ""
     for lhs, a in zip(lhses, arrays):
         if len(spec):
@@ -160,14 +196,17 @@
                 spec += "..."
                 axis_off += 1
                 break
             elif capture.binding is None or len(capture.axes) > 1:
                 raise_parse_error("Parenthesized axes are not currently supported", equation, capture.char_range)
             else:
                 name = capture.binding
+                if name in axis_aliases:
+                    used_aliases.add(name)
+
                 if axis_off >= len(a.axes):
                     raise ValueError("Mismatched number of axes in einsum")
                 table.bind_alias(name, a.axes[axis_off], equation, capture.char_range)
                 letter = _assign_letter_to_name(name, name_mappings_for_einsum, used_letters)
                 spec += letter
                 axis_off += 1
 
@@ -180,14 +219,17 @@
 
             axis_off = len(a.axes) - 1
             for capture in reversed(lhs.captures):
                 if capture is Ellipsis:
                     break
                 else:
                     name = capture.binding
+                    if name in axis_aliases:
+                        used_aliases.add(name)
+
                     if axis_off < final_lhs_axis_off:
                         raise ValueError("Mismatched number of axes in einsum")
                     table.bind_alias(name, a.axes[axis_off], equation, capture.char_range)
                     letter = _assign_letter_to_name(name, name_mappings_for_einsum, used_letters)
                     spec += letter
                     axis_off -= 1
         else:
@@ -226,44 +268,53 @@
                 )
 
             named_on_left_but_not_right.discard(letter)
 
             spec += letter
             out_axes.append(axis)
 
+    _check_for_unused_aliases(axis_aliases, used_aliases, equation)
+
     if has_ellipsis_rhs:
         all_input_axes = _all_input_axes(arrays)
         # eliminate the axes that are contracted
         unmentioned = tuple(table.dealias_binding(name) for name in named_on_left_but_not_right)
         out = eliminate_axes(all_input_axes, unmentioned)  # type: ignore
         return spec, out
     else:
         return spec, out_axes
 
 
 def _all_input_axes(arrays):
     return ensure_tuple(functools.reduce(union_axes, (a.axes for a in arrays), ()))  # type: ignore
 
 
-def _captures_to_axis_names(equation, lhs) -> Tuple[list[str | EllipsisType], bool]:
+def _captures_to_axis_names(equation, lhs, aliases) -> Tuple[list[str | EllipsisType], bool, set[str]]:
+    covered_aliases = set()
     candidate_axes: list[str | EllipsisType] = []
     has_ellipsis = False
     for capture in lhs.captures:
         if capture is Ellipsis:
             has_ellipsis = True
             candidate_axes.append(Ellipsis)
         elif capture.binding is None or len(capture.axes) > 1:
             raise_parse_error("Parenthesized axes are not currently supported", equation, capture.char_range)
         else:
             name = capture.binding
+            if name in aliases:
+                covered_aliases.add(name)
+                axis = aliases[name]
+                name = axis_name(axis)
             candidate_axes.append(name)
-    return candidate_axes, has_ellipsis
+    return candidate_axes, has_ellipsis, covered_aliases
 
 
-def _make_einsum_spec(name_mappings_for_einsum, used_letters, arrays, out_axes):
+def _make_einsum_spec(arrays, out_axes):
+    name_mappings_for_einsum: dict[str, str] = {}
+    used_letters: set[str] = set()
     spec = ""
     for operand in arrays:
         if len(spec):
             spec += ","
         for axis in operand.axes:
             letter = _assign_letter_to_name(axis.name, name_mappings_for_einsum, used_letters)
             spec += letter
@@ -285,7 +336,34 @@
             if letter not in used_letters:
                 break
         else:
             raise ValueError("Too many axes to contract")
     name_mappings_for_einsum[name] = letter
     used_letters.add(letter)
     return letter
+
+
+def _check_axis_size_consistency(arrays, axis, name_in_spec):
+    # ensure the size is correct and the axis is present
+    found = False
+    ax_name = axis_name(axis)
+    for array_index, array in enumerate(arrays):
+        try:
+            resolved = array.resolve_axis(ax_name)
+        except ValueError:
+            pass
+        else:
+            found = True
+            if resolved.size != axis.size:
+                raise ValueError(
+                    f"Size mismatch for axis {ax_name}. In array {array_index},"
+                    f" {axis} has size {resolved.size} but expected {axis.size},"
+                    f"because of the alias {name_in_spec}={axis}"
+                )
+    if not found:
+        raise ValueError(f"Axis {ax_name} not found in any of the input arrays")
+
+
+def _check_for_unused_aliases(axis_aliases, used_aliases, equation):
+    if any(alias not in used_aliases for alias in axis_aliases):
+        unused_aliases_str = ", ".join([alias for alias in axis_aliases if alias not in used_aliases])
+        raise_parse_error(f"Unused aliases from kwargs: {unused_aliases_str}", equation, None)
```

### Comparing `haliax-1.4.dev288/src/haliax/_src/fp8.py` & `haliax-1.4.dev289/src/haliax/_src/fp8.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/_src/parsing.py` & `haliax-1.4.dev289/src/haliax/_src/parsing.py`

 * *Files 4% similar despite different names*

```diff
@@ -221,24 +221,34 @@
 
 
 class AliasTable:
     bindings: dict[str, AxisSelector]  # names in the string to axes
 
     def __init__(self, bindings=None):
         if bindings is None:
-            bindings = {}
-        self.bindings = bindings
+            self.bindings = {}
+        else:
+            self.bindings = {**bindings}
 
     def dealias_binding(self, binding: str) -> Optional[AxisSelector]:
         return self.bindings.get(binding, None)
 
     def bind_alias(self, alias: str, axis: Axis, expr, char_range):
         if axis.name in self.bindings:
             if self.bindings[alias] != axis:
                 raise_parse_error(f"Alias {alias} is assigned to more than one axis", expr, char_range)
+        elif alias in self.bindings:
+            current = self.bindings[alias]
+            if isinstance(current, Axis):
+                if current != axis:
+                    raise_parse_error(f"Alias {alias} is assigned to more than one axis", expr, char_range)
+            elif current != axis.name:
+                raise_parse_error(f"Alias {alias} is assigned to more than one axis", expr, char_range)
+            else:
+                self.bindings[alias] = axis
         else:
             self.bindings[alias] = axis
 
 
 def _resolve_bindings(array, bindings: Mapping[str, Axis | str | int]) -> AliasTable:
     b: dict[str, AxisSelector] = {}
     for name, selector in bindings.items():
```

### Comparing `haliax-1.4.dev288/src/haliax/_src/rearrange.py` & `haliax-1.4.dev289/src/haliax/_src/rearrange.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/_src/util.py` & `haliax-1.4.dev289/src/haliax/_src/util.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/nn/__init__.py` & `haliax-1.4.dev289/src/haliax/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/nn/activations.py` & `haliax-1.4.dev289/src/haliax/nn/activations.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/nn/attention.py` & `haliax-1.4.dev289/src/haliax/nn/attention.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/nn/conv.py` & `haliax-1.4.dev289/src/haliax/nn/conv.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/nn/dropout.py` & `haliax-1.4.dev289/src/haliax/nn/dropout.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/nn/embedding.py` & `haliax-1.4.dev289/src/haliax/nn/embedding.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/nn/linear.py` & `haliax-1.4.dev289/src/haliax/nn/linear.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/nn/loss.py` & `haliax-1.4.dev289/src/haliax/nn/loss.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/nn/mlp.py` & `haliax-1.4.dev289/src/haliax/nn/mlp.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/nn/normalization.py` & `haliax-1.4.dev289/src/haliax/nn/normalization.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/nn/pool.py` & `haliax-1.4.dev289/src/haliax/nn/pool.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/src/haliax/nn/scan.py` & `haliax-1.4.dev289/src/haliax/nn/scan.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/tests/core_test.py` & `haliax-1.4.dev289/tests/core_test.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/tests/test_attention.py` & `haliax-1.4.dev289/tests/test_attention.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/tests/test_axis.py` & `haliax-1.4.dev289/tests/test_axis.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/tests/test_conv.py` & `haliax-1.4.dev289/tests/test_conv.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/tests/test_debug.py` & `haliax-1.4.dev289/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/tests/test_dot.py` & `haliax-1.4.dev289/tests/test_dot.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/tests/test_einsum.py` & `haliax-1.4.dev289/tests/test_einsum.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,14 +33,36 @@
         jnp.equal(
             einsum("i j k,k j i->", m1, m2).array,
             jnp.einsum("ijk,kji->", m1.array, m2.array),
         )
     )
 
 
+def test_einsum_positional_aliases():
+    Height = Axis("Height", 2)
+    Width = Axis("Width", 3)
+    Depth = Axis("Depth", 4)
+
+    m1 = NamedArray(jnp.ones((Height.size, Width.size, Depth.size)), (Height, Width, Depth))
+    m2 = NamedArray(jnp.ones((Depth.size, Width.size, Height.size)), (Depth, Width, Height))
+
+    assert jnp.all(
+        jnp.equal(einsum("i j k,k j i-> j k", m1, m2, i=Height).array, jnp.einsum("ijk,kji->jk", m1.array, m2.array))
+    )
+
+    with pytest.raises(ValueError):
+        einsum("i j k,k j i-> j k", m1, m2, i=Width)
+
+    with pytest.raises(ValueError):
+        einsum("i j k,q j i-> j k", m1, m2, i=Height, q=Height)
+
+    with pytest.raises(ValueError):
+        einsum("i j k,k j i-> j k", m1, m2, i=Height, q=Height)
+
+
 def test_einsum_basic_named():
     Height = Axis("Height", 2)
     Width = Axis("Width", 3)
     Depth = Axis("Depth", 4)
 
     m1 = hax.ones((Height, Width, Depth))
     m2 = hax.ones((Depth, Width, Height))
@@ -144,14 +166,40 @@
         jnp.equal(
             einsum("{Depth} -> ... Depth ...", m1, m2).array,
             jnp.einsum("ijk,kji->ijk", m1.array, m2.array),
         )
     )
 
 
+def test_einsum_unordered_aliases():
+    Height = Axis("Height", 2)
+    Width = Axis("Width", 3)
+    Depth = Axis("Depth", 4)
+
+    m1 = hax.ones((Height, Width, Depth))
+    m2 = hax.ones((Depth, Width, Height))
+
+    assert jnp.all(
+        jnp.equal(
+            einsum("{h w d} -> h w", m1, m2, h=Height, w=Width, d=Depth).array,
+            jnp.einsum("ijk,kji->ij", m1.array, m2.array),
+        )
+    )
+
+    # test error cases:
+
+    # Missing alias
+    with pytest.raises(ValueError, match="Axis d not present"):
+        einsum("{h w d} -> h w", m1, m2, h=Height, w=Width)
+
+    # Extra alias
+    with pytest.raises(ValueError, match="Axis alias d not used"):
+        einsum("{h w} -> h w", m1, m2, h=Height, w=Width, d=Depth)
+
+
 def test_einsum_ordered_ellipsis():
     Height = Axis("Height", 2)
     Width = Axis("Width", 3)
     Depth = Axis("Depth", 4)
 
     m1 = hax.ones((Height, Width, Depth))
     m2 = hax.ones((Depth, Width, Height))
@@ -268,7 +316,39 @@
     hax_out = hax.einsum("{...} -> ...", hax_im, hax_w2)
     jnp_out = jnp.einsum("bhwc,ce -> bhwce", im, w2)
     assert jnp.all(jnp.equal(hax_out.array, jnp_out))
 
     hax_out = hax.einsum("{...} -> ", hax_im, hax_w2)
     jnp_out = jnp.einsum("bhwc,ce -> ", im, w2)
     assert jnp.all(jnp.equal(hax_out.array, jnp_out))
+
+
+def test_einsum_output_only_mode():
+    # tests "-> out axes"
+    Height = Axis("Height", 2)
+    Width = Axis("Width", 3)
+    Depth = Axis("Depth", 4)
+
+    m1 = hax.ones((Height, Width, Depth))
+    m2 = hax.ones((Depth, Width, Height))
+    m3 = hax.ones((Height, Depth))
+
+    assert jnp.all(jnp.equal(einsum("-> Height Width", m1, m2).array, jnp.einsum("ijk,kji->ij", m1.array, m2.array)))
+    assert jnp.all(jnp.equal(einsum("-> Height", m1).array, jnp.einsum("ijk->i", m1.array)))
+
+    with pytest.raises(ValueError):
+        einsum("-> Q Width", m1)
+
+    with pytest.raises(ValueError, match=".*Unused aliases from kwargs: Q$"):
+        einsum("-> Height Width", m1, m2, Q=Axis("Q", 2))
+
+    assert jnp.all(jnp.equal(einsum("-> h w", m1, h=Height, w=Width).array, jnp.einsum("ijk->ij", m1.array)))
+
+    assert jnp.all(
+        jnp.equal(einsum("-> h w", m1, m3, h=Height, w=Width).array, jnp.einsum("ijk,ik->ij", m1.array, m3.array))
+    )
+
+    with pytest.raises(ValueError, match=".*Size mismatch.*"):
+        einsum("-> h w", m1, h=Height.resize(4), w=Width)
+
+    with pytest.raises(ValueError, match=".*not found in any of the input arrays.*"):
+        einsum("-> h w", m3, h=Height, w=Width.resize(4))
```

### Comparing `haliax-1.4.dev288/tests/test_fp8.py` & `haliax-1.4.dev289/tests/test_fp8.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/tests/test_hof.py` & `haliax-1.4.dev289/tests/test_hof.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/tests/test_nn.py` & `haliax-1.4.dev289/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/tests/test_ops.py` & `haliax-1.4.dev289/tests/test_ops.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/tests/test_parsing.py` & `haliax-1.4.dev289/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/tests/test_partitioning.py` & `haliax-1.4.dev289/tests/test_partitioning.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/tests/test_pool.py` & `haliax-1.4.dev289/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/tests/test_random.py` & `haliax-1.4.dev289/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/tests/test_rearrange.py` & `haliax-1.4.dev289/tests/test_rearrange.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/tests/test_scan.py` & `haliax-1.4.dev289/tests/test_scan.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/tests/test_specialized_fns.py` & `haliax-1.4.dev289/tests/test_specialized_fns.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/tests/test_tree_util.py` & `haliax-1.4.dev289/tests/test_tree_util.py`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/.gitignore` & `haliax-1.4.dev289/.gitignore`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/LICENSE` & `haliax-1.4.dev289/LICENSE`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/README.md` & `haliax-1.4.dev289/README.md`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/pyproject.toml` & `haliax-1.4.dev289/pyproject.toml`

 * *Files identical despite different names*

### Comparing `haliax-1.4.dev288/PKG-INFO` & `haliax-1.4.dev289/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: haliax
-Version: 1.4.dev288
+Version: 1.4.dev289
 Summary: Named Tensors for Legible Deep Learning in JAX
 Project-URL: Homepage, https://github.com/stanford-crfm/haliax
 Project-URL: Bug Tracker, https://github.com/stanford-crfm/haliax/issues/
 Author-email: David Hall <dlwh@cs.stanford.edu>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

