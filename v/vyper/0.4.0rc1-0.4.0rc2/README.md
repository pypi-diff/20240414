# Comparing `tmp/vyper-0.4.0rc1.tar.gz` & `tmp/vyper-0.4.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vyper-0.4.0rc1.tar", last modified: Wed Apr 10 17:15:53 2024, max compression
+gzip compressed data, was "vyper-0.4.0rc2.tar", last modified: Sun Apr 14 02:52:25 2024, max compression
```

## Comparing `vyper-0.4.0rc1.tar` & `vyper-0.4.0rc2.tar`

### file list

```diff
@@ -1,585 +1,587 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.889755 vyper-0.4.0rc1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.817755 vyper-0.4.0rc1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.817755 vyper-0.4.0rc1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/.github/ISSUE_TEMPLATE/vip.md
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.817755 vyper-0.4.0rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/.github/workflows/era-tester.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/.github/workflows/ghcr.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/.github/workflows/pull-request.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/.github/workflows/release-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-10 17:15:53.889755 vyper-0.4.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.821755 vyper-0.4.0rc1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.821755 vyper-0.4.0rc1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/_templates/versions.html
--rw-r--r--   0 runner    (1001) docker     (127)    38035 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/built-in-functions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/compiler-exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15660 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/compiling-a-contract.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/constants-and-vars.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13206 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/control-structures.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/deploying-contracts.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/event-logging.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/installing-vyper.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/interfaces.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/natspec.rst
--rw-r--r--   0 runner    (1001) docker     (127)    64067 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/resources.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/scoping-and-declarations.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/statements.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/structure-of-a-contract.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15593 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/style-guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/testing-contracts-brownie.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/testing-contracts-ethtester.rst
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/testing-contracts.rst
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/toctree.rst
--rw-r--r--   0 runner    (1001) docker     (127)    23266 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/types.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/versioning.rst
--rw-r--r--   0 runner    (1001) docker     (127)    29097 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/docs/vyper-by-example.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.821755 vyper-0.4.0rc1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.821755 vyper-0.4.0rc1/examples/auctions/
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/auctions/blind_auction.vy
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/auctions/simple_open_auction.vy
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/crowdfund.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.821755 vyper-0.4.0rc1/examples/factory/
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/factory/Exchange.vy
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/factory/Factory.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.821755 vyper-0.4.0rc1/examples/market_maker/
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/market_maker/on_chain_market_maker.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.821755 vyper-0.4.0rc1/examples/name_registry/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/name_registry/name_registry.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.821755 vyper-0.4.0rc1/examples/safe_remote_purchase/
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/safe_remote_purchase/safe_remote_purchase.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.821755 vyper-0.4.0rc1/examples/stock/
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/stock/company.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.821755 vyper-0.4.0rc1/examples/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/storage/advanced_storage.vy
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/storage/storage.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.825755 vyper-0.4.0rc1/examples/tokens/
--rw-r--r--   0 runner    (1001) docker     (127)    15365 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/tokens/ERC1155ownable.vy
--rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/tokens/ERC20.vy
--rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/tokens/ERC4626.vy
--rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/tokens/ERC721.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.825755 vyper-0.4.0rc1/examples/voting/
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/voting/ballot.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.825755 vyper-0.4.0rc1/examples/wallet/
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/examples/wallet/wallet.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.825755 vyper-0.4.0rc1/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)      265 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/hooks/build
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/make.cmd
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      207 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/quicktest.sh
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-10 17:15:53.889755 vyper-0.4.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.825755 vyper-0.4.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19787 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.825755 vyper-0.4.0rc1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/fixtures/memorymock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.825755 vyper-0.4.0rc1/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.809755 vyper-0.4.0rc1/tests/functional/builtins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.829755 vyper-0.4.0rc1/tests/functional/builtins/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_abi_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)    12235 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_abi_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_addmod.py
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_as_wei_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_bitwise.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_ceil.py
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)    20923 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    19720 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_create_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_ec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_ecrecover.py
--rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_extract32.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_floor.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_is_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_keccak256.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_method_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_minmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_minmax_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_mulmod.py
--rw-r--r--   0 runner    (1001) docker     (127)    16894 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_raw_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_send.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)    14614 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_uint2str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_unary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/codegen/test_unsafe_math.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.829755 vyper-0.4.0rc1/tests/functional/builtins/folding/
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/folding/test_abs.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/folding/test_addmod_mulmod.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/folding/test_bitwise.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/folding/test_epsilon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/folding/test_floor_ceil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/folding/test_fold_as_wei_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/folding/test_keccak_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/folding/test_len.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/folding/test_min_max.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/builtins/folding/test_powmod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.833755 vyper-0.4.0rc1/tests/functional/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.833755 vyper-0.4.0rc1/tests/functional/codegen/calling_convention/
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/calling_convention/test_default_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/calling_convention/test_default_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/calling_convention/test_erc20_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)    59140 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/calling_convention/test_external_contract_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/calling_convention/test_modifiable_external_contract_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)    16771 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/calling_convention/test_return.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/calling_convention/test_self_call_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.833755 vyper-0.4.0rc1/tests/functional/codegen/environment_variables/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/environment_variables/test_block_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/environment_variables/test_blockhash.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/environment_variables/test_tx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.837755 vyper-0.4.0rc1/tests/functional/codegen/features/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.837755 vyper-0.4.0rc1/tests/functional/codegen/features/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/decorators/test_nonreentrant.py
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/decorators/test_payable.py
--rw-r--r--   0 runner    (1001) docker     (127)    14651 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/decorators/test_private.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/decorators/test_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/decorators/test_pure.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/decorators/test_view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.837755 vyper-0.4.0rc1/tests/functional/codegen/features/iteration/
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/iteration/test_break.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/iteration/test_continue.py
--rw-r--r--   0 runner    (1001) docker     (127)    17032 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/iteration/test_for_in_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/iteration/test_for_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/iteration/test_range_in.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_address_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_assert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_assert_unreachable.py
--rw-r--r--   0 runner    (1001) docker     (127)     9726 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_bytes_map_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    16224 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_clampers.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_conditionals.py
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_gas.py
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_immutable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)    15764 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_internal_call.py
--rw-r--r--   0 runner    (1001) docker     (127)    33812 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_logging_bytes_extended.py
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_logging_from_call.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_memory_alloc.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_memory_dealloc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_packing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_reverting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_short_circuiting.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_string_map_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_ternary.py
--rw-r--r--   0 runner    (1001) docker     (127)    12702 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/features/test_transient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.837755 vyper-0.4.0rc1/tests/functional/codegen/integration/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/integration/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/integration/test_crowdfund.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/integration/test_escrow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.841755 vyper-0.4.0rc1/tests/functional/codegen/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/modules/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/modules/test_exports.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/modules/test_flag_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/modules/test_interface_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/modules/test_module_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/modules/test_module_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/modules/test_stateless_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.841755 vyper-0.4.0rc1/tests/functional/codegen/storage_variables/
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/storage_variables/test_getters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/storage_variables/test_setters.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/storage_variables/test_storage_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/test_call_graph_stability.py
--rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    14820 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/test_selector_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/test_selector_table_stability.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.841755 vyper-0.4.0rc1/tests/functional/codegen/types/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.845755 vyper-0.4.0rc1/tests/functional/codegen/types/numbers/
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8450 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_decimals.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_division.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_exponents.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_isqrt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_modulo.py
--rw-r--r--   0 runner    (1001) docker     (127)    10362 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_signed_ints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_sqrt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_unsigned_ints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/test_array_indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/test_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/test_bytes_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/test_bytes_zero_padding.py
--rw-r--r--   0 runner    (1001) docker     (127)    50402 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/test_dynamic_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/test_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/test_identifier_naming.py
--rw-r--r--   0 runner    (1001) docker     (127)    23876 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/test_lists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/test_node_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9422 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/test_string_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/codegen/types/test_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.845755 vyper-0.4.0rc1/tests/functional/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.845755 vyper-0.4.0rc1/tests/functional/examples/auctions/
--rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/auctions/test_blind_auction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/auctions/test_simple_open_auction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.845755 vyper-0.4.0rc1/tests/functional/examples/company/
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/company/test_company.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.845755 vyper-0.4.0rc1/tests/functional/examples/crowdfund/
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/crowdfund/test_crowdfund_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.845755 vyper-0.4.0rc1/tests/functional/examples/factory/
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/factory/test_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.845755 vyper-0.4.0rc1/tests/functional/examples/market_maker/
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/market_maker/test_on_chain_market_maker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.845755 vyper-0.4.0rc1/tests/functional/examples/name_registry/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/name_registry/test_name_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.845755 vyper-0.4.0rc1/tests/functional/examples/safe_remote_purchase/
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/safe_remote_purchase/test_safe_remote_purchase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.845755 vyper-0.4.0rc1/tests/functional/examples/storage/
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/storage/test_advanced_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/storage/test_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.845755 vyper-0.4.0rc1/tests/functional/examples/tokens/
--rw-r--r--   0 runner    (1001) docker     (127)    14162 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/tokens/test_erc1155.py
--rw-r--r--   0 runner    (1001) docker     (127)    14563 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/tokens/test_erc20.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/tokens/test_erc4626.py
--rw-r--r--   0 runner    (1001) docker     (127)    11222 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/tokens/test_erc721.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.845755 vyper-0.4.0rc1/tests/functional/examples/voting/
--rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/voting/test_ballot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.845755 vyper-0.4.0rc1/tests/functional/examples/wallet/
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/examples/wallet/test_wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.845755 vyper-0.4.0rc1/tests/functional/grammar/
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/grammar/test_grammar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.853755 vyper-0.4.0rc1/tests/functional/syntax/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.857755 vyper-0.4.0rc1/tests/functional/syntax/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_argument_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_call_violation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_constancy_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_function_declaration_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_instantiation_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_invalid_literal_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_invalid_payable.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_invalid_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_invalid_type_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_namespace_collision.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_overflow_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_structure_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_syntax_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_type_mismatch_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_undeclared_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_variable_declaration_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_vyper_exception_pos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.857755 vyper-0.4.0rc1/tests/functional/syntax/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/modules/test_deploy_visibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/modules/test_exports.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/modules/test_implements.py
--rw-r--r--   0 runner    (1001) docker     (127)    26589 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/modules/test_initializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.857755 vyper-0.4.0rc1/tests/functional/syntax/names/
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/names/test_event_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/names/test_function_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/names/test_variable_names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.857755 vyper-0.4.0rc1/tests/functional/syntax/signatures/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/signatures/test_invalid_function_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/signatures/test_method_id_conflicts.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_abi_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_abi_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_abs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_addmulmod.py
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_address_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_ann_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_as_uint256.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_as_wei_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_blockscope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_bool.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_bool_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_ceil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_chainid.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_code_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_codehash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_conditionals.py
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_create_with_code_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_dynamic_array.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_epsilon.py
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_external_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_extract32.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_floor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7848 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_for_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_functions_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_immutables.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_invalids.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_keccak256.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_len.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_method_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_minmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_minmax_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_msg_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_nested_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_no_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_powmod.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_print.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_raw_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_return_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_self_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_selfdestruct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_send.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_ternary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_tuple_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_uint2str.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_unary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/functional/syntax/test_unbalanced_return.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.857755 vyper-0.4.0rc1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.857755 vyper-0.4.0rc1/tests/unit/abi_types/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/abi_types/test_invalid_abi_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.861755 vyper-0.4.0rc1/tests/unit/ast/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.861755 vyper-0.4.0rc1/tests/unit/ast/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/nodes/test_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/nodes/test_compare_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/nodes/test_fold_binop_decimal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/nodes/test_fold_binop_int.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/nodes/test_fold_boolop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/nodes/test_fold_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/nodes/test_fold_subscript.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/nodes/test_fold_unaryop.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/nodes/test_from_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/nodes/test_get_children.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/nodes/test_get_descendants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/nodes/test_hex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/test_annotate_and_optimize_ast.py
--rw-r--r--   0 runner    (1001) docker     (127)    68091 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/test_ast_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/test_metadata_journal.py
--rw-r--r--   0 runner    (1001) docker     (127)     8940 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/test_natspec.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/test_pre_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/ast/test_source_annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.809755 vyper-0.4.0rc1/tests/unit/cli/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.861755 vyper-0.4.0rc1/tests/unit/cli/storage_layout/
--rw-r--r--   0 runner    (1001) docker     (127)     9181 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/cli/storage_layout/test_storage_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/cli/storage_layout/test_storage_layout_overrides.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.861755 vyper-0.4.0rc1/tests/unit/cli/vyper_compile/
--rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/cli/vyper_compile/test_compile_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/cli/vyper_compile/test_parse_args.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.865755 vyper-0.4.0rc1/tests/unit/cli/vyper_json/
--rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/cli/vyper_json/test_compile_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/cli/vyper_json/test_get_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/cli/vyper_json/test_get_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/cli/vyper_json/test_output_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/cli/vyper_json/test_parse_args_vyperjson.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.865755 vyper-0.4.0rc1/tests/unit/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.865755 vyper-0.4.0rc1/tests/unit/compiler/asm/
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/asm/test_asm_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.865755 vyper-0.4.0rc1/tests/unit/compiler/ir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/ir/test_calldatacopy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/ir/test_compile_ir.py
--rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/ir/test_optimize_ir.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/ir/test_repeat.py
--rw-r--r--   0 runner    (1001) docker     (127)    13843 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/ir/test_with.py
--rw-r--r--   0 runner    (1001) docker     (127)    14979 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/test_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/test_bytecode_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)    24877 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/test_compile_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/test_default_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     8519 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/test_input_bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/test_opcodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/test_pre_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/test_sha3_32.py
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/test_source_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.865755 vyper-0.4.0rc1/tests/unit/compiler/venom/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/venom/test_convert_basicblock_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/venom/test_dominator_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/venom/test_duplicate_operands.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/venom/test_liveness_simple_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/venom/test_make_ssa.py
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/venom/test_multi_entry_block.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/venom/test_stack_at_external_return.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/compiler/venom/test_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.869755 vyper-0.4.0rc1/tests/unit/semantics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.869755 vyper-0.4.0rc1/tests/unit/semantics/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/semantics/analysis/test_array_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/semantics/analysis/test_cyclic_function_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/semantics/analysis/test_for_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/semantics/analysis/test_potential_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/semantics/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/semantics/test_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/semantics/test_storage_slots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.869755 vyper-0.4.0rc1/tests/unit/semantics/types/
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/semantics/types/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/semantics/types/test_pure_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/semantics/types/test_size_in_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/semantics/types/test_type_from_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/semantics/types/test_type_from_annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.869755 vyper-0.4.0rc1/tests/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/unit/utils/test_keccak256.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.869755 vyper-0.4.0rc1/vyper/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/abi_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.873755 vyper-0.4.0rc1/vyper/ast/
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ast/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ast/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ast/grammar.lark
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ast/grammar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ast/identifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ast/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ast/natspec.py
--rw-r--r--   0 runner    (1001) docker     (127)    45995 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ast/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ast/nodes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17273 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ast/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)    11699 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ast/pre_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ast/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ast/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.873755 vyper-0.4.0rc1/vyper/builtins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/builtins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16822 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/builtins/_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/builtins/_signatures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/builtins/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    91096 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/builtins/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.873755 vyper-0.4.0rc1/vyper/builtins/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/builtins/interfaces/IERC165.vyi
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/builtins/interfaces/IERC20.vyi
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/builtins/interfaces/IERC20Detailed.vyi
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/builtins/interfaces/IERC4626.vyi
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/builtins/interfaces/IERC721.vyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.877755 vyper-0.4.0rc1/vyper/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10533 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/cli/vyper_compile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1886 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/cli/vyper_ir.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15843 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/cli/vyper_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.877755 vyper-0.4.0rc1/vyper/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/abi_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    13044 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    42565 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    30634 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/expr.py
--rw-r--r--   0 runner    (1001) docker     (127)     8195 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/external_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.877755 vyper-0.4.0rc1/vyper/codegen/function_definitions/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/function_definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/function_definitions/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7972 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/function_definitions/external_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/function_definitions/internal_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    23599 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/ir_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/jumptable_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/keccak256_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/memory_allocator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21180 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/return_.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/self_call.py
--rw-r--r--   0 runner    (1001) docker     (127)    13548 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/codegen/stmt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.881755 vyper-0.4.0rc1/vyper/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/compiler/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/compiler/input_bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)    12936 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/compiler/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    11699 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/compiler/phases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/compiler/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/compiler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.881755 vyper-0.4.0rc1/vyper/evm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/evm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/evm/address_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     8431 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/evm/opcodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12713 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.881755 vyper-0.4.0rc1/vyper/ir/
--rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ir/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45834 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ir/compile_ir.py
--rw-r--r--   0 runner    (1001) docker     (127)    24821 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ir/optimizer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1076 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/ir/s_expressions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.881755 vyper-0.4.0rc1/vyper/semantics/
--rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.885755 vyper-0.4.0rc1/vyper/semantics/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/analysis/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/analysis/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/analysis/constant_folding.py
--rw-r--r--   0 runner    (1001) docker     (127)    12043 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/analysis/data_positions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/analysis/getters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/analysis/global_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/analysis/import_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/analysis/levenshtein_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    37194 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/analysis/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    35107 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/analysis/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    23538 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/analysis/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/data_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.885755 vyper-0.4.0rc1/vyper/semantics/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15183 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/types/bytestrings.py
--rw-r--r--   0 runner    (1001) docker     (127)    30776 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/types/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    17439 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/types/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    12439 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/types/primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/types/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/types/subscriptable.py
--rw-r--r--   0 runner    (1001) docker     (127)    14788 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/types/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/semantics/types/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17315 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.885755 vyper-0.4.0rc1/vyper/venom/
--rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    15338 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/basicblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/bb_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/dominators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    19260 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/ir_node_to_venom.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.889755 vyper-0.4.0rc1/vyper/venom/passes/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/passes/base_pass.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/passes/constant_propagation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/passes/dft.py
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/passes/make_ssa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/passes/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/passes/simplify_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/passes/stack_reorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/stack_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    20128 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/venom/venom_to_assembly.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-10 17:15:53.000000 vyper-0.4.0rc1/vyper/version.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 17:15:50.000000 vyper-0.4.0rc1/vyper/vyper_git_commithash.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-10 17:15:41.000000 vyper-0.4.0rc1/vyper/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:15:53.869755 vyper-0.4.0rc1/vyper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-10 17:15:53.000000 vyper-0.4.0rc1/vyper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20300 2024-04-10 17:15:53.000000 vyper-0.4.0rc1/vyper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:15:53.000000 vyper-0.4.0rc1/vyper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-10 17:15:53.000000 vyper-0.4.0rc1/vyper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-10 17:15:53.000000 vyper-0.4.0rc1/vyper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 17:15:53.000000 vyper-0.4.0rc1/vyper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.821169 vyper-0.4.0rc2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.753169 vyper-0.4.0rc2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.753169 vyper-0.4.0rc2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/.github/ISSUE_TEMPLATE/vip.md
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.753169 vyper-0.4.0rc2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/.github/workflows/era-tester.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/.github/workflows/ghcr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/.github/workflows/pull-request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/.github/workflows/release-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-14 02:52:25.821169 vyper-0.4.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.757169 vyper-0.4.0rc2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.757169 vyper-0.4.0rc2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/_templates/versions.html
+-rw-r--r--   0 runner    (1001) docker     (127)    38119 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/built-in-functions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/compiler-exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15660 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/compiling-a-contract.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/constants-and-vars.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13206 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/control-structures.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/deploying-contracts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/event-logging.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/installing-vyper.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/interfaces.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/natspec.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    64067 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/resources.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/scoping-and-declarations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/statements.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/structure-of-a-contract.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15593 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/style-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/testing-contracts-brownie.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/testing-contracts-ethtester.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/testing-contracts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/toctree.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    23266 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/types.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/versioning.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    29097 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/vyper-by-example.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.757169 vyper-0.4.0rc2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.761169 vyper-0.4.0rc2/examples/auctions/
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/auctions/blind_auction.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/auctions/simple_open_auction.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/crowdfund.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.761169 vyper-0.4.0rc2/examples/factory/
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/factory/Exchange.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/factory/Factory.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.761169 vyper-0.4.0rc2/examples/market_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/market_maker/on_chain_market_maker.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.761169 vyper-0.4.0rc2/examples/name_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/name_registry/name_registry.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.761169 vyper-0.4.0rc2/examples/safe_remote_purchase/
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/safe_remote_purchase/safe_remote_purchase.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.761169 vyper-0.4.0rc2/examples/stock/
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/stock/company.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.761169 vyper-0.4.0rc2/examples/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/storage/advanced_storage.vy
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/storage/storage.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.761169 vyper-0.4.0rc2/examples/tokens/
+-rw-r--r--   0 runner    (1001) docker     (127)    15365 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/tokens/ERC1155ownable.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/tokens/ERC20.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/tokens/ERC4626.vy
+-rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/tokens/ERC721.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.761169 vyper-0.4.0rc2/examples/voting/
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/voting/ballot.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.761169 vyper-0.4.0rc2/examples/wallet/
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/wallet/wallet.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.761169 vyper-0.4.0rc2/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      265 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/hooks/build
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/make.cmd
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      207 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/quicktest.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-14 02:52:25.821169 vyper-0.4.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.761169 vyper-0.4.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19787 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.761169 vyper-0.4.0rc2/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/fixtures/memorymock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.761169 vyper-0.4.0rc2/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.745169 vyper-0.4.0rc2/tests/functional/builtins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.765169 vyper-0.4.0rc2/tests/functional/builtins/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_abi_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12235 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_abi_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_addmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_as_wei_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_bitwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_ceil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20923 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19720 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_create_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_ec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_ecrecover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_extract32.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_floor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_is_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_keccak256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_method_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_minmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_minmax_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_mulmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16894 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_raw_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_send.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14614 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_uint2str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_unary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_unsafe_math.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.769169 vyper-0.4.0rc2/tests/functional/builtins/folding/
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/folding/test_abs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/folding/test_addmod_mulmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/folding/test_bitwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/folding/test_epsilon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/folding/test_floor_ceil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/folding/test_fold_as_wei_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/folding/test_keccak_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/folding/test_len.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/folding/test_min_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/folding/test_powmod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.769169 vyper-0.4.0rc2/tests/functional/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.769169 vyper-0.4.0rc2/tests/functional/codegen/calling_convention/
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/calling_convention/test_default_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/calling_convention/test_default_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/calling_convention/test_erc20_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59140 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/calling_convention/test_external_contract_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/calling_convention/test_modifiable_external_contract_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16771 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/calling_convention/test_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/calling_convention/test_self_call_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.769169 vyper-0.4.0rc2/tests/functional/codegen/environment_variables/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/environment_variables/test_block_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/environment_variables/test_blockhash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/environment_variables/test_tx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.773169 vyper-0.4.0rc2/tests/functional/codegen/features/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.773169 vyper-0.4.0rc2/tests/functional/codegen/features/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/decorators/test_nonreentrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/decorators/test_payable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14651 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/decorators/test_private.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/decorators/test_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/decorators/test_pure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/decorators/test_view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.773169 vyper-0.4.0rc2/tests/functional/codegen/features/iteration/
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/iteration/test_break.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/iteration/test_continue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17032 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/iteration/test_for_in_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/iteration/test_for_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/iteration/test_range_in.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_address_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_assert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_assert_unreachable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9726 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_bytes_map_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16224 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_clampers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_conditionals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_gas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_immutable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15764 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_internal_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33812 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_logging_bytes_extended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_logging_from_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_memory_alloc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_memory_dealloc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_reverting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_short_circuiting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_string_map_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_ternary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12702 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_transient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.773169 vyper-0.4.0rc2/tests/functional/codegen/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/integration/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/integration/test_crowdfund.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/integration/test_escrow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.777169 vyper-0.4.0rc2/tests/functional/codegen/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/modules/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/modules/test_exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/modules/test_flag_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/modules/test_interface_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/modules/test_module_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/modules/test_module_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/modules/test_nonreentrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/modules/test_stateless_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.777169 vyper-0.4.0rc2/tests/functional/codegen/storage_variables/
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/storage_variables/test_getters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/storage_variables/test_setters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/storage_variables/test_storage_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/test_call_graph_stability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14820 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/test_selector_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/test_selector_table_stability.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.777169 vyper-0.4.0rc2/tests/functional/codegen/types/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.781169 vyper-0.4.0rc2/tests/functional/codegen/types/numbers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8450 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_decimals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_division.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_exponents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_isqrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_modulo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10362 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_signed_ints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_sqrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_unsigned_ints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/test_array_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/test_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/test_bytes_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/test_bytes_zero_padding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50402 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/test_dynamic_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/test_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/test_identifier_naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23876 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/test_lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/test_node_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9422 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/test_string_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/test_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.781169 vyper-0.4.0rc2/tests/functional/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.781169 vyper-0.4.0rc2/tests/functional/examples/auctions/
+-rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/auctions/test_blind_auction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/auctions/test_simple_open_auction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.781169 vyper-0.4.0rc2/tests/functional/examples/company/
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/company/test_company.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.781169 vyper-0.4.0rc2/tests/functional/examples/crowdfund/
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/crowdfund/test_crowdfund_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.781169 vyper-0.4.0rc2/tests/functional/examples/factory/
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/factory/test_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.781169 vyper-0.4.0rc2/tests/functional/examples/market_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/market_maker/test_on_chain_market_maker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.781169 vyper-0.4.0rc2/tests/functional/examples/name_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/name_registry/test_name_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.781169 vyper-0.4.0rc2/tests/functional/examples/safe_remote_purchase/
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/safe_remote_purchase/test_safe_remote_purchase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.781169 vyper-0.4.0rc2/tests/functional/examples/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/storage/test_advanced_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/storage/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.781169 vyper-0.4.0rc2/tests/functional/examples/tokens/
+-rw-r--r--   0 runner    (1001) docker     (127)    14162 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/tokens/test_erc1155.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14563 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/tokens/test_erc20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/tokens/test_erc4626.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11222 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/tokens/test_erc721.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.781169 vyper-0.4.0rc2/tests/functional/examples/voting/
+-rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/voting/test_ballot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.781169 vyper-0.4.0rc2/tests/functional/examples/wallet/
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/wallet/test_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.781169 vyper-0.4.0rc2/tests/functional/grammar/
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/grammar/test_grammar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.789169 vyper-0.4.0rc2/tests/functional/syntax/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.793169 vyper-0.4.0rc2/tests/functional/syntax/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_argument_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_call_violation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_constancy_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_function_declaration_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_instantiation_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_invalid_literal_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_invalid_payable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_invalid_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_invalid_type_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_namespace_collision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_overflow_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_structure_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_syntax_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_type_mismatch_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_undeclared_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_variable_declaration_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_vyper_exception_pos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.793169 vyper-0.4.0rc2/tests/functional/syntax/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/modules/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/modules/test_deploy_visibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/modules/test_exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/modules/test_implements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28241 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/modules/test_initializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.793169 vyper-0.4.0rc2/tests/functional/syntax/names/
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/names/test_event_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/names/test_function_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/names/test_variable_names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.793169 vyper-0.4.0rc2/tests/functional/syntax/signatures/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/signatures/test_invalid_function_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/signatures/test_method_id_conflicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_abi_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_abi_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_abs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_addmulmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_address_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_ann_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_as_uint256.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_as_wei_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_blockscope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_bool_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_ceil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_chainid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_code_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_codehash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_conditionals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_create_with_code_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_dynamic_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_epsilon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_external_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_extract32.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_floor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7848 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_for_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_functions_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_immutables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_invalids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_keccak256.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_len.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_method_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_minmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_minmax_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_msg_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_nested_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_no_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_powmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_raw_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_return_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_self_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_selfdestruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_send.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_ternary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_tuple_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_uint2str.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_unary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_unbalanced_return.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.793169 vyper-0.4.0rc2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.793169 vyper-0.4.0rc2/tests/unit/abi_types/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/abi_types/test_invalid_abi_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.793169 vyper-0.4.0rc2/tests/unit/ast/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.797169 vyper-0.4.0rc2/tests/unit/ast/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/nodes/test_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/nodes/test_compare_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/nodes/test_fold_binop_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/nodes/test_fold_binop_int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/nodes/test_fold_boolop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/nodes/test_fold_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/nodes/test_fold_subscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/nodes/test_fold_unaryop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/nodes/test_from_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/nodes/test_get_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/nodes/test_get_descendants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/nodes/test_hex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/test_annotate_and_optimize_ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68091 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/test_ast_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/test_metadata_journal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8940 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/test_natspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/test_pre_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/test_source_annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.749169 vyper-0.4.0rc2/tests/unit/cli/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.797169 vyper-0.4.0rc2/tests/unit/cli/storage_layout/
+-rw-r--r--   0 runner    (1001) docker     (127)     9181 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/cli/storage_layout/test_storage_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/cli/storage_layout/test_storage_layout_overrides.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.797169 vyper-0.4.0rc2/tests/unit/cli/vyper_compile/
+-rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/cli/vyper_compile/test_compile_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/cli/vyper_compile/test_parse_args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.797169 vyper-0.4.0rc2/tests/unit/cli/vyper_json/
+-rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/cli/vyper_json/test_compile_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/cli/vyper_json/test_get_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/cli/vyper_json/test_get_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/cli/vyper_json/test_output_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/cli/vyper_json/test_parse_args_vyperjson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.797169 vyper-0.4.0rc2/tests/unit/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.797169 vyper-0.4.0rc2/tests/unit/compiler/asm/
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/asm/test_asm_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.801169 vyper-0.4.0rc2/tests/unit/compiler/ir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/ir/test_calldatacopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/ir/test_compile_ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/ir/test_optimize_ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/ir/test_repeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13843 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/ir/test_with.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14979 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/test_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/test_bytecode_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24877 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/test_compile_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/test_default_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8519 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/test_input_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/test_opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/test_pre_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/test_sha3_32.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/test_source_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.801169 vyper-0.4.0rc2/tests/unit/compiler/venom/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/venom/test_convert_basicblock_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/venom/test_dominator_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/venom/test_duplicate_operands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/venom/test_liveness_simple_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/venom/test_make_ssa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/venom/test_multi_entry_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/venom/test_stack_at_external_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/venom/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.801169 vyper-0.4.0rc2/tests/unit/semantics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.801169 vyper-0.4.0rc2/tests/unit/semantics/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/semantics/analysis/test_array_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/semantics/analysis/test_cyclic_function_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/semantics/analysis/test_for_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/semantics/analysis/test_potential_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/semantics/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/semantics/test_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/semantics/test_storage_slots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.801169 vyper-0.4.0rc2/tests/unit/semantics/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/semantics/types/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/semantics/types/test_pure_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/semantics/types/test_size_in_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/semantics/types/test_type_from_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/semantics/types/test_type_from_annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.801169 vyper-0.4.0rc2/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/utils/test_keccak256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.805169 vyper-0.4.0rc2/vyper/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/abi_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.805169 vyper-0.4.0rc2/vyper/ast/
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ast/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ast/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ast/grammar.lark
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ast/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ast/identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ast/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ast/natspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46130 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ast/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ast/nodes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17273 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ast/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11699 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ast/pre_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ast/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ast/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.809169 vyper-0.4.0rc2/vyper/builtins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/builtins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16822 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/builtins/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/builtins/_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/builtins/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91096 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/builtins/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.809169 vyper-0.4.0rc2/vyper/builtins/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/builtins/interfaces/IERC165.vyi
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/builtins/interfaces/IERC20.vyi
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/builtins/interfaces/IERC20Detailed.vyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/builtins/interfaces/IERC4626.vyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/builtins/interfaces/IERC721.vyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.809169 vyper-0.4.0rc2/vyper/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10533 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/cli/vyper_compile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1886 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/cli/vyper_ir.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15843 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/cli/vyper_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.809169 vyper-0.4.0rc2/vyper/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/abi_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13044 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42565 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30728 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8195 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/external_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.813169 vyper-0.4.0rc2/vyper/codegen/function_definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/function_definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/function_definitions/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7972 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/function_definitions/external_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/function_definitions/internal_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23599 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/ir_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/jumptable_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/keccak256_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/memory_allocator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21180 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/return_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/self_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13548 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/stmt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.813169 vyper-0.4.0rc2/vyper/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/compiler/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/compiler/input_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12936 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/compiler/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11699 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/compiler/phases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/compiler/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/compiler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.813169 vyper-0.4.0rc2/vyper/evm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/evm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/evm/address_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8431 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/evm/opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12713 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.813169 vyper-0.4.0rc2/vyper/ir/
+-rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45834 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ir/compile_ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24821 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ir/optimizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1076 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ir/s_expressions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.813169 vyper-0.4.0rc2/vyper/semantics/
+-rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.817169 vyper-0.4.0rc2/vyper/semantics/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/analysis/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/analysis/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/analysis/constant_folding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12043 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/analysis/data_positions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/analysis/getters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/analysis/global_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/analysis/import_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/analysis/levenshtein_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37264 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/analysis/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36587 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/analysis/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23689 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/analysis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/data_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.817169 vyper-0.4.0rc2/vyper/semantics/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15183 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/types/bytestrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30949 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/types/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17759 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/types/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12439 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/types/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/types/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12174 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/types/subscriptable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14788 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/types/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7392 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/types/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17315 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.817169 vyper-0.4.0rc2/vyper/venom/
+-rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15338 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/basicblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/bb_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/dominators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19260 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/ir_node_to_venom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.821169 vyper-0.4.0rc2/vyper/venom/passes/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/passes/base_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/passes/constant_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/passes/dft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/passes/make_ssa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/passes/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/passes/simplify_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/passes/stack_reorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/stack_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20128 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/venom_to_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-14 02:52:25.000000 vyper-0.4.0rc2/vyper/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-14 02:52:22.000000 vyper-0.4.0rc2/vyper/vyper_git_commithash.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.805169 vyper-0.4.0rc2/vyper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-14 02:52:25.000000 vyper-0.4.0rc2/vyper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20397 2024-04-14 02:52:25.000000 vyper-0.4.0rc2/vyper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 02:52:25.000000 vyper-0.4.0rc2/vyper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-14 02:52:25.000000 vyper-0.4.0rc2/vyper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-14 02:52:25.000000 vyper-0.4.0rc2/vyper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 02:52:25.000000 vyper-0.4.0rc2/vyper.egg-info/top_level.txt
```

### Comparing `vyper-0.4.0rc1/.github/ISSUE_TEMPLATE/bug.md` & `vyper-0.4.0rc2/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/.github/ISSUE_TEMPLATE/vip.md` & `vyper-0.4.0rc2/.github/ISSUE_TEMPLATE/vip.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/.github/workflows/build.yml` & `vyper-0.4.0rc2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/.github/workflows/codeql.yml` & `vyper-0.4.0rc2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/.github/workflows/era-tester.yml` & `vyper-0.4.0rc2/.github/workflows/era-tester.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/.github/workflows/ghcr.yml` & `vyper-0.4.0rc2/.github/workflows/ghcr.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/.github/workflows/pull-request.yaml` & `vyper-0.4.0rc2/.github/workflows/pull-request.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -51,9 +51,7 @@
           subjectPattern: '^(?![A-Z]).+$'
           subjectPatternError: |
             Starts with uppercase letter: '{subject}'
             (Full PR title: '{title}')
           # type[scope]<optional !>: subject
           # use [] instead of () for aesthetics
           headerPattern: '^(\w*)(?:\[([\w$.\-*/ ]*)\])?!?: (.*)$'
-          validateSingleCommit: true
-          validateSingleCommitMatchesPrTitle: true
```

### Comparing `vyper-0.4.0rc1/.github/workflows/release-pypi.yml` & `vyper-0.4.0rc2/.github/workflows/release-pypi.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/.github/workflows/test.yml` & `vyper-0.4.0rc2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/.pre-commit-config.yaml` & `vyper-0.4.0rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/Dockerfile` & `vyper-0.4.0rc2/Dockerfile`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/LICENSE` & `vyper-0.4.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/Makefile` & `vyper-0.4.0rc2/Makefile`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/PKG-INFO` & `vyper-0.4.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vyper
-Version: 0.4.0rc1
+Version: 0.4.0rc2
 Summary: Vyper: the Pythonic Programming Language for the EVM
 Home-page: https://github.com/vyperlang/vyper
 Author: Vyper Team
 Author-email: 
 License: Apache License 2.0
 Keywords: ethereum evm smart contract language
 Classifier: Intended Audience :: Developers
```

### Comparing `vyper-0.4.0rc1/README.md` & `vyper-0.4.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/SECURITY.md` & `vyper-0.4.0rc2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/Makefile` & `vyper-0.4.0rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/_templates/versions.html` & `vyper-0.4.0rc2/docs/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/built-in-functions.rst` & `vyper-0.4.0rc2/docs/built-in-functions.rst`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 .. py:function:: create_minimal_proxy_to(target: address, value: uint256 = 0, revert_on_failure: bool = True[, salt: bytes32]) -> address
 
     Deploys a small, EIP1167-compliant "minimal proxy contract" that duplicates the logic of the contract at ``target``, but has its own state since every call to ``target`` is made using ``DELEGATECALL`` to ``target``. To the end user, this should be indistinguishable from an independently deployed contract with the same code as ``target``.
 
 
     * ``target``: Address of the contract to proxy to
     * ``value``: The wei value to send to the new contract address (Optional, default 0)
-    * ``revert_on_failure``: If ``False``, instead of reverting when the create operation fails, return the null address.
+    * ``revert_on_failure``: If ``False``, instead of reverting when the create operation fails, return the zero address (Optional, default ``True``)
     * ``salt``: A ``bytes32`` value utilized by the deterministic ``CREATE2`` opcode (Optional, if not supplied, ``CREATE`` is used)
 
     Returns the address of the newly created proxy contract. If the create operation fails (for instance, in the case of a ``CREATE2`` collision), execution will revert.
 
     .. code-block:: vyper
 
         @external
@@ -166,15 +166,15 @@
 
 .. py:function:: create_copy_of(target: address, value: uint256 = 0, revert_on_failure: bool = True[, salt: bytes32]) -> address
 
     Create a physical copy of the runtime code at ``target``. The code at ``target`` is byte-for-byte copied into a newly deployed contract.
 
     * ``target``: Address of the contract to copy
     * ``value``: The wei value to send to the new contract address (Optional, default 0)
-    * ``revert_on_failure``: If ``False``, instead of reverting when the create operation fails, return the null address.
+    * ``revert_on_failure``: If ``False``, instead of reverting when the create operation fails, return the zero address (Optional, default ``True``)
     * ``salt``: A ``bytes32`` value utilized by the deterministic ``CREATE2`` opcode (Optional, if not supplied, ``CREATE`` is used)
 
     Returns the address of the created contract. If the create operation fails (for instance, in the case of a ``CREATE2`` collision), execution will revert. If there is no code at ``target``, execution will revert.
 
     .. code-block:: vyper
 
         @external
@@ -191,15 +191,15 @@
     Copy the code of ``target`` into memory and execute it as initcode. In other words, this operation interprets the code at ``target`` not as regular runtime code, but directly as initcode. The ``*args`` are interpreted as constructor arguments, and are ABI-encoded and included when executing the initcode.
 
     * ``target``: Address of the blueprint to invoke
     * ``*args``: Constructor arguments to forward to the initcode.
     * ``value``: The wei value to send to the new contract address (Optional, default 0)
     * ``raw_args``: If ``True``, ``*args`` must be a single ``Bytes[...]`` argument, which will be interpreted as a raw bytes buffer to forward to the create operation (which is useful for instance, if pre- ABI-encoded data is passed in from elsewhere). (Optional, default ``False``)
     * ``code_offset``: The offset to start the ``EXTCODECOPY`` from (Optional, default 3)
-    * ``revert_on_failure``: If ``False``, instead of reverting when the create operation fails, return the null address.
+    * ``revert_on_failure``: If ``False``, instead of reverting when the create operation fails, return the zero address (Optional, default ``True``)
     * ``salt``: A ``bytes32`` value utilized by the deterministic ``CREATE2`` opcode (Optional, if not supplied, ``CREATE`` is used)
 
     Returns the address of the created contract. If the create operation fails (for instance, in the case of a ``CREATE2`` collision), execution will revert. If ``code_offset >= target.codesize`` (ex. if there is no code at ``target``), execution will revert.
 
     .. code-block:: vyper
 
         @external
```

### Comparing `vyper-0.4.0rc1/docs/compiler-exceptions.rst` & `vyper-0.4.0rc2/docs/compiler-exceptions.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/compiling-a-contract.rst` & `vyper-0.4.0rc2/docs/compiling-a-contract.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/conf.py` & `vyper-0.4.0rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/constants-and-vars.rst` & `vyper-0.4.0rc2/docs/constants-and-vars.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/contributing.rst` & `vyper-0.4.0rc2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/control-structures.rst` & `vyper-0.4.0rc2/docs/control-structures.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/deploying-contracts.rst` & `vyper-0.4.0rc2/docs/deploying-contracts.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/event-logging.rst` & `vyper-0.4.0rc2/docs/event-logging.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/index.rst` & `vyper-0.4.0rc2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/installing-vyper.rst` & `vyper-0.4.0rc2/docs/installing-vyper.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/interfaces.rst` & `vyper-0.4.0rc2/docs/interfaces.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/logo.svg` & `vyper-0.4.0rc2/docs/logo.svg`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/make.bat` & `vyper-0.4.0rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/natspec.rst` & `vyper-0.4.0rc2/docs/natspec.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/release-notes.rst` & `vyper-0.4.0rc2/docs/release-notes.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/resources.rst` & `vyper-0.4.0rc2/docs/resources.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/scoping-and-declarations.rst` & `vyper-0.4.0rc2/docs/scoping-and-declarations.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/statements.rst` & `vyper-0.4.0rc2/docs/statements.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/structure-of-a-contract.rst` & `vyper-0.4.0rc2/docs/structure-of-a-contract.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/style-guide.rst` & `vyper-0.4.0rc2/docs/style-guide.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/testing-contracts-brownie.rst` & `vyper-0.4.0rc2/docs/testing-contracts-brownie.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/testing-contracts-ethtester.rst` & `vyper-0.4.0rc2/docs/testing-contracts-ethtester.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/testing-contracts.rst` & `vyper-0.4.0rc2/docs/testing-contracts.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/toctree.rst` & `vyper-0.4.0rc2/docs/toctree.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/types.rst` & `vyper-0.4.0rc2/docs/types.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/versioning.rst` & `vyper-0.4.0rc2/docs/versioning.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/docs/vyper-by-example.rst` & `vyper-0.4.0rc2/docs/vyper-by-example.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/examples/auctions/blind_auction.vy` & `vyper-0.4.0rc2/examples/auctions/blind_auction.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/examples/auctions/simple_open_auction.vy` & `vyper-0.4.0rc2/examples/auctions/simple_open_auction.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/examples/crowdfund.vy` & `vyper-0.4.0rc2/examples/crowdfund.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/examples/factory/Exchange.vy` & `vyper-0.4.0rc2/examples/factory/Exchange.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/examples/factory/Factory.vy` & `vyper-0.4.0rc2/examples/factory/Factory.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/examples/market_maker/on_chain_market_maker.vy` & `vyper-0.4.0rc2/examples/market_maker/on_chain_market_maker.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/examples/safe_remote_purchase/safe_remote_purchase.vy` & `vyper-0.4.0rc2/examples/safe_remote_purchase/safe_remote_purchase.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/examples/stock/company.vy` & `vyper-0.4.0rc2/examples/stock/company.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/examples/tokens/ERC1155ownable.vy` & `vyper-0.4.0rc2/examples/tokens/ERC1155ownable.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/examples/tokens/ERC20.vy` & `vyper-0.4.0rc2/examples/tokens/ERC20.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/examples/tokens/ERC4626.vy` & `vyper-0.4.0rc2/examples/tokens/ERC4626.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/examples/tokens/ERC721.vy` & `vyper-0.4.0rc2/examples/tokens/ERC721.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/examples/voting/ballot.vy` & `vyper-0.4.0rc2/examples/voting/ballot.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/examples/wallet/wallet.vy` & `vyper-0.4.0rc2/examples/wallet/wallet.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/make.cmd` & `vyper-0.4.0rc2/make.cmd`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/setup.cfg` & `vyper-0.4.0rc2/setup.cfg`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/setup.py` & `vyper-0.4.0rc2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,15 +99,14 @@
     ],
     setup_requires=["pytest-runner", "setuptools_scm>=7.1.0,<8.0.0"],
     tests_require=extras_require["test"],
     extras_require=extras_require,
     entry_points={
         "console_scripts": [
             "vyper=vyper.cli.vyper_compile:_parse_cli_args",
-            "vyper-serve=vyper.cli.vyper_serve:_parse_cli_args",
             "fang=vyper.cli.vyper_ir:_parse_cli_args",
             "vyper-json=vyper.cli.vyper_json:_parse_cli_args",
         ]
     },
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
```

### Comparing `vyper-0.4.0rc1/tests/conftest.py` & `vyper-0.4.0rc2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/fixtures/memorymock.py` & `vyper-0.4.0rc2/tests/fixtures/memorymock.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_abi_decode.py` & `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_abi_decode.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_abi_encode.py` & `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_abi_encode.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_addmod.py` & `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_addmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_as_wei_value.py` & `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_as_wei_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_bitwise.py` & `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_bitwise.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_ceil.py` & `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_ceil.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_concat.py` & `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_concat.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_convert.py` & `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_convert.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_create_functions.py` & `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_create_functions.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_ec.py` & `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_ec.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_ecrecover.py` & `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_ecrecover.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_empty.py` & `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_empty.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_extract32.py` & `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_extract32.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_floor.py` & `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_floor.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_is_contract.py` & `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_is_contract.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_keccak256.py` & `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_keccak256.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_length.py` & `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_length.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_method_id.py` & `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_method_id.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_minmax.py` & `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_minmax.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_minmax_value.py` & `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_minmax_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_mulmod.py` & `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_mulmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_raw_call.py` & `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_raw_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_send.py` & `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_send.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_sha256.py` & `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_sha256.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_slice.py` & `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_slice.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_uint2str.py` & `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_uint2str.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_unary.py` & `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_unary.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/codegen/test_unsafe_math.py` & `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_unsafe_math.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/folding/test_abs.py` & `vyper-0.4.0rc2/tests/functional/builtins/folding/test_abs.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/folding/test_addmod_mulmod.py` & `vyper-0.4.0rc2/tests/functional/builtins/folding/test_addmod_mulmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/folding/test_bitwise.py` & `vyper-0.4.0rc2/tests/functional/builtins/folding/test_bitwise.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/folding/test_floor_ceil.py` & `vyper-0.4.0rc2/tests/functional/builtins/folding/test_floor_ceil.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/folding/test_fold_as_wei_value.py` & `vyper-0.4.0rc2/tests/functional/builtins/folding/test_fold_as_wei_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/folding/test_keccak_sha.py` & `vyper-0.4.0rc2/tests/functional/builtins/folding/test_keccak_sha.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/folding/test_len.py` & `vyper-0.4.0rc2/tests/functional/builtins/folding/test_len.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/folding/test_min_max.py` & `vyper-0.4.0rc2/tests/functional/builtins/folding/test_min_max.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/builtins/folding/test_powmod.py` & `vyper-0.4.0rc2/tests/functional/builtins/folding/test_powmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/calling_convention/test_default_function.py` & `vyper-0.4.0rc2/tests/functional/codegen/calling_convention/test_default_function.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/calling_convention/test_default_parameters.py` & `vyper-0.4.0rc2/tests/functional/codegen/calling_convention/test_default_parameters.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/calling_convention/test_erc20_abi.py` & `vyper-0.4.0rc2/tests/functional/codegen/calling_convention/test_erc20_abi.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/calling_convention/test_external_contract_calls.py` & `vyper-0.4.0rc2/tests/functional/codegen/calling_convention/test_external_contract_calls.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/calling_convention/test_modifiable_external_contract_calls.py` & `vyper-0.4.0rc2/tests/functional/codegen/calling_convention/test_modifiable_external_contract_calls.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/calling_convention/test_return.py` & `vyper-0.4.0rc2/tests/functional/codegen/calling_convention/test_return.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/calling_convention/test_self_call_struct.py` & `vyper-0.4.0rc2/tests/functional/codegen/calling_convention/test_self_call_struct.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/environment_variables/test_blockhash.py` & `vyper-0.4.0rc2/tests/functional/codegen/environment_variables/test_blockhash.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/decorators/test_nonreentrant.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/decorators/test_nonreentrant.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/decorators/test_payable.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/decorators/test_payable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/decorators/test_private.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/decorators/test_private.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/decorators/test_public.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/decorators/test_public.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/decorators/test_pure.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/decorators/test_pure.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/decorators/test_view.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/decorators/test_view.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/iteration/test_break.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/iteration/test_break.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/iteration/test_continue.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/iteration/test_continue.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/iteration/test_for_in_list.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/iteration/test_for_in_list.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/iteration/test_for_range.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/iteration/test_for_range.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/iteration/test_range_in.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/iteration/test_range_in.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/test_assert.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/test_assert.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/test_assert_unreachable.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/test_assert_unreachable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/test_assignment.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/test_assignment.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/test_bytes_map_keys.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/test_bytes_map_keys.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/test_clampers.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/test_clampers.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/test_comparison.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/test_comparison.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/test_conditionals.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/test_conditionals.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/test_constructor.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/test_constructor.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/test_immutable.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/test_immutable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/test_init.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/test_init.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/test_internal_call.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/test_internal_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/test_logging.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/test_logging.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/test_logging_bytes_extended.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/test_logging_bytes_extended.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/test_logging_from_call.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/test_logging_from_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/test_memory_dealloc.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/test_memory_dealloc.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/test_packing.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/test_packing.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/test_reverting.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/test_reverting.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/test_short_circuiting.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/test_short_circuiting.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/test_string_map_keys.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/test_string_map_keys.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/test_ternary.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/test_ternary.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/features/test_transient.py` & `vyper-0.4.0rc2/tests/functional/codegen/features/test_transient.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/integration/test_crowdfund.py` & `vyper-0.4.0rc2/tests/functional/codegen/integration/test_crowdfund.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/integration/test_escrow.py` & `vyper-0.4.0rc2/tests/functional/codegen/integration/test_escrow.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/modules/test_events.py` & `vyper-0.4.0rc2/tests/functional/codegen/modules/test_events.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/modules/test_flag_imports.py` & `vyper-0.4.0rc2/tests/functional/codegen/modules/test_flag_imports.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/modules/test_interface_imports.py` & `vyper-0.4.0rc2/tests/functional/codegen/modules/test_interface_imports.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/modules/test_module_constants.py` & `vyper-0.4.0rc2/tests/functional/codegen/modules/test_module_constants.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/modules/test_module_variables.py` & `vyper-0.4.0rc2/tests/functional/codegen/modules/test_module_variables.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/modules/test_stateless_functions.py` & `vyper-0.4.0rc2/tests/functional/codegen/modules/test_stateless_functions.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/storage_variables/test_getters.py` & `vyper-0.4.0rc2/tests/functional/codegen/storage_variables/test_getters.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/storage_variables/test_setters.py` & `vyper-0.4.0rc2/tests/functional/codegen/storage_variables/test_setters.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/storage_variables/test_storage_variable.py` & `vyper-0.4.0rc2/tests/functional/codegen/storage_variables/test_storage_variable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/test_call_graph_stability.py` & `vyper-0.4.0rc2/tests/functional/codegen/test_call_graph_stability.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/test_interfaces.py` & `vyper-0.4.0rc2/tests/functional/codegen/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/test_selector_table.py` & `vyper-0.4.0rc2/tests/functional/codegen/test_selector_table.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/test_selector_table_stability.py` & `vyper-0.4.0rc2/tests/functional/codegen/test_selector_table_stability.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_constants.py` & `vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_constants.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_decimals.py` & `vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_decimals.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_division.py` & `vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_division.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_exponents.py` & `vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_exponents.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_isqrt.py` & `vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_isqrt.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_modulo.py` & `vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_modulo.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_signed_ints.py` & `vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_signed_ints.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_sqrt.py` & `vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_sqrt.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/types/numbers/test_unsigned_ints.py` & `vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_unsigned_ints.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/types/test_array_indexing.py` & `vyper-0.4.0rc2/tests/functional/codegen/types/test_array_indexing.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/types/test_bytes.py` & `vyper-0.4.0rc2/tests/functional/codegen/types/test_bytes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/types/test_bytes_literal.py` & `vyper-0.4.0rc2/tests/functional/codegen/types/test_bytes_literal.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/types/test_bytes_zero_padding.py` & `vyper-0.4.0rc2/tests/functional/codegen/types/test_bytes_zero_padding.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/types/test_dynamic_array.py` & `vyper-0.4.0rc2/tests/functional/codegen/types/test_dynamic_array.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/types/test_flag.py` & `vyper-0.4.0rc2/tests/functional/codegen/types/test_flag.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/types/test_identifier_naming.py` & `vyper-0.4.0rc2/tests/functional/codegen/types/test_identifier_naming.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/types/test_lists.py` & `vyper-0.4.0rc2/tests/functional/codegen/types/test_lists.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/types/test_node_types.py` & `vyper-0.4.0rc2/tests/functional/codegen/types/test_node_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/types/test_string.py` & `vyper-0.4.0rc2/tests/functional/codegen/types/test_string.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/types/test_string_literal.py` & `vyper-0.4.0rc2/tests/functional/codegen/types/test_string_literal.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/codegen/types/test_struct.py` & `vyper-0.4.0rc2/tests/functional/codegen/types/test_struct.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/examples/auctions/test_blind_auction.py` & `vyper-0.4.0rc2/tests/functional/examples/auctions/test_blind_auction.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/examples/auctions/test_simple_open_auction.py` & `vyper-0.4.0rc2/tests/functional/examples/auctions/test_simple_open_auction.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/examples/company/test_company.py` & `vyper-0.4.0rc2/tests/functional/examples/company/test_company.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/examples/crowdfund/test_crowdfund_example.py` & `vyper-0.4.0rc2/tests/functional/examples/crowdfund/test_crowdfund_example.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/examples/factory/test_factory.py` & `vyper-0.4.0rc2/tests/functional/examples/factory/test_factory.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/examples/market_maker/test_on_chain_market_maker.py` & `vyper-0.4.0rc2/tests/functional/examples/market_maker/test_on_chain_market_maker.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/examples/safe_remote_purchase/test_safe_remote_purchase.py` & `vyper-0.4.0rc2/tests/functional/examples/safe_remote_purchase/test_safe_remote_purchase.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/examples/storage/test_advanced_storage.py` & `vyper-0.4.0rc2/tests/functional/examples/storage/test_advanced_storage.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/examples/storage/test_storage.py` & `vyper-0.4.0rc2/tests/functional/examples/storage/test_storage.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/examples/tokens/test_erc1155.py` & `vyper-0.4.0rc2/tests/functional/examples/tokens/test_erc1155.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/examples/tokens/test_erc20.py` & `vyper-0.4.0rc2/tests/functional/examples/tokens/test_erc20.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/examples/tokens/test_erc4626.py` & `vyper-0.4.0rc2/tests/functional/examples/tokens/test_erc4626.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/examples/tokens/test_erc721.py` & `vyper-0.4.0rc2/tests/functional/examples/tokens/test_erc721.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/examples/voting/test_ballot.py` & `vyper-0.4.0rc2/tests/functional/examples/voting/test_ballot.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/examples/wallet/test_wallet.py` & `vyper-0.4.0rc2/tests/functional/examples/wallet/test_wallet.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/grammar/test_grammar.py` & `vyper-0.4.0rc2/tests/functional/grammar/test_grammar.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_argument_exception.py` & `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_argument_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_call_violation.py` & `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_call_violation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_constancy_exception.py` & `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_constancy_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_function_declaration_exception.py` & `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_function_declaration_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_instantiation_exception.py` & `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_instantiation_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_invalid_literal_exception.py` & `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_invalid_literal_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_invalid_payable.py` & `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_invalid_payable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_invalid_reference.py` & `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_invalid_reference.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_invalid_type_exception.py` & `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_invalid_type_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_namespace_collision.py` & `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_namespace_collision.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_overflow_exception.py` & `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_overflow_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_structure_exception.py` & `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_structure_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_syntax_exception.py` & `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_syntax_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_type_mismatch_exception.py` & `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_type_mismatch_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_undeclared_definition.py` & `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_undeclared_definition.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_variable_declaration_exception.py` & `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_variable_declaration_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/exceptions/test_vyper_exception_pos.py` & `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_vyper_exception_pos.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/modules/test_deploy_visibility.py` & `vyper-0.4.0rc2/tests/functional/syntax/modules/test_deploy_visibility.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/modules/test_exports.py` & `vyper-0.4.0rc2/tests/functional/syntax/modules/test_exports.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 import pytest
 
 from vyper.compiler import compile_code
-from vyper.exceptions import ImmutableViolation, NamespaceCollision, StructureException
+from vyper.exceptions import (
+    ImmutableViolation,
+    InterfaceViolation,
+    NamespaceCollision,
+    StructureException,
+)
+
+from .helpers import NONREENTRANT_NOTE
 
 
 def test_exports_no_uses(make_input_bundle):
     lib1 = """
 counter: uint256
 
 @external
@@ -17,15 +24,15 @@
 import lib1
 exports: lib1.get_counter
     """
     input_bundle = make_input_bundle({"lib1.vy": lib1})
     with pytest.raises(ImmutableViolation) as e:
         compile_code(main, input_bundle=input_bundle)
 
-    assert e.value._message == "Cannot access `lib1` state!"
+    assert e.value._message == "Cannot access `lib1` state!" + NONREENTRANT_NOTE
 
     expected_hint = "add `uses: lib1` or `initializes: lib1` as a "
     expected_hint += "top-level statement to your contract"
     assert e.value.hint == expected_hint
 
 
 def test_exports_no_uses_variable(make_input_bundle):
@@ -36,15 +43,15 @@
 import lib1
 exports: lib1.counter
     """
     input_bundle = make_input_bundle({"lib1.vy": lib1})
     with pytest.raises(ImmutableViolation) as e:
         compile_code(main, input_bundle=input_bundle)
 
-    assert e.value._message == "Cannot access `lib1` state!"
+    assert e.value._message == "Cannot access `lib1` state!" + NONREENTRANT_NOTE
 
     expected_hint = "add `uses: lib1` or `initializes: lib1` as a "
     expected_hint += "top-level statement to your contract"
     assert e.value.hint == expected_hint
 
 
 def test_exports_uses_variable(make_input_bundle):
@@ -303,7 +310,137 @@
     assert e.value.annotations[0].node_source_code == "lib1.foo"
     assert e.value.annotations[0].module_node.path == "main.vy"
 
     assert e.value.prev_decl.lineno == 4
     assert e.value.prev_decl.col_offset == 9
     assert e.value.prev_decl.node_source_code == "lib1.foo"
     assert e.value.prev_decl.module_node.path == "main.vy"
+
+
+def test_interface_export_collision(make_input_bundle):
+    main = """
+import lib1
+
+exports: lib1.__interface__
+exports: lib1.bar
+    """
+    lib1 = """
+@external
+def bar() -> uint256:
+    return 1
+    """
+    input_bundle = make_input_bundle({"lib1.vy": lib1})
+    with pytest.raises(StructureException) as e:
+        compile_code(main, input_bundle=input_bundle)
+    assert e.value._message == "already exported!"
+
+
+def test_no_export_missing_function(make_input_bundle):
+    ifoo = """
+@external
+def do_xyz():
+    ...
+    """
+    lib1 = """
+import ifoo
+
+@external
+@view
+def bar() -> uint256:
+    return 1
+    """
+    main = """
+import lib1
+
+exports: lib1.ifoo
+    """
+    input_bundle = make_input_bundle({"lib1.vy": lib1, "ifoo.vyi": ifoo})
+    with pytest.raises(InterfaceViolation) as e:
+        compile_code(main, input_bundle=input_bundle)
+    assert e.value._message == "requested `lib1.ifoo` but `lib1` does not implement `lib1.ifoo`!"
+
+
+def test_no_export_unimplemented_interface(make_input_bundle):
+    ifoo = """
+@external
+def do_xyz():
+    ...
+    """
+    lib1 = """
+import ifoo
+
+# technically implements ifoo, but missing `implements: ifoo`
+
+@external
+def do_xyz():
+    pass
+    """
+    main = """
+import lib1
+
+exports: lib1.ifoo
+    """
+    input_bundle = make_input_bundle({"lib1.vy": lib1, "ifoo.vyi": ifoo})
+    with pytest.raises(InterfaceViolation) as e:
+        compile_code(main, input_bundle=input_bundle)
+    assert e.value._message == "requested `lib1.ifoo` but `lib1` does not implement `lib1.ifoo`!"
+
+
+def test_export_selector_conflict(make_input_bundle):
+    ifoo = """
+@external
+def gsf():
+    ...
+    """
+    lib1 = """
+import ifoo
+
+@external
+def gsf():
+    pass
+
+@external
+@view
+def tgeo() -> uint256:
+    return 1
+    """
+    main = """
+import lib1
+
+exports: (lib1.ifoo, lib1.tgeo)
+    """
+    input_bundle = make_input_bundle({"lib1.vy": lib1, "ifoo.vyi": ifoo})
+    with pytest.raises(StructureException) as e:
+        compile_code(main, input_bundle=input_bundle)
+    assert e.value._message == "Methods produce colliding method ID `0x67e43e43`: gsf(), tgeo()"
+
+
+def test_export_different_return_type(make_input_bundle):
+    ifoo = """
+@external
+def foo() -> uint256:
+    ...
+    """
+    lib1 = """
+import ifoo
+
+foo: public(int256)
+
+@deploy
+def __init__():
+    self.foo = -1
+    """
+    main = """
+import lib1
+
+initializes: lib1
+
+exports: lib1.ifoo
+
+@deploy
+def __init__():
+    lib1.__init__()
+    """
+    input_bundle = make_input_bundle({"lib1.vy": lib1, "ifoo.vyi": ifoo})
+    with pytest.raises(InterfaceViolation) as e:
+        compile_code(main, input_bundle=input_bundle)
+    assert e.value._message == "requested `lib1.ifoo` but `lib1` does not implement `lib1.ifoo`!"
```

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/modules/test_implements.py` & `vyper-0.4.0rc2/tests/functional/syntax/modules/test_implements.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/modules/test_initializers.py` & `vyper-0.4.0rc2/tests/functional/syntax/modules/test_initializers.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     BorrowException,
     ImmutableViolation,
     InitializerException,
     StructureException,
     UndeclaredDefinition,
 )
 
+from .helpers import NONREENTRANT_NOTE
+
 
 def test_initialize_uses(make_input_bundle):
     lib1 = """
 counter: uint256
 
 @deploy
 def __init__():
@@ -409,15 +411,15 @@
 initializes: lib1
     """
     input_bundle = make_input_bundle({"lib1.vy": lib1, "lib2.vy": lib2})
 
     with pytest.raises(ImmutableViolation) as e:
         compile_code(main, input_bundle=input_bundle)
 
-    assert e.value._message == "Cannot access `lib1` state!"
+    assert e.value._message == "Cannot access `lib1` state!" + NONREENTRANT_NOTE
 
     expected_hint = "add `uses: lib1` or `initializes: lib1` as a "
     expected_hint += "top-level statement to your contract"
     assert e.value._hint == expected_hint
 
 
 def test_missing_uses_for_read(make_input_bundle):
@@ -446,15 +448,15 @@
     lib1.counter = 100
     """
     input_bundle = make_input_bundle({"lib1.vy": lib1, "lib2.vy": lib2})
 
     with pytest.raises(ImmutableViolation) as e:
         compile_code(main, input_bundle=input_bundle)
 
-    assert e.value._message == "Cannot access `lib1` state!"
+    assert e.value._message == "Cannot access `lib1` state!" + NONREENTRANT_NOTE
 
     expected_hint = "add `uses: lib1` or `initializes: lib1` as a "
     expected_hint += "top-level statement to your contract"
     assert e.value._hint == expected_hint
 
 
 def test_missing_uses_for_read_immutable(make_input_bundle):
@@ -487,15 +489,15 @@
     lib1.counter = 100
     """
     input_bundle = make_input_bundle({"lib1.vy": lib1, "lib2.vy": lib2})
 
     with pytest.raises(ImmutableViolation) as e:
         compile_code(main, input_bundle=input_bundle)
 
-    assert e.value._message == "Cannot access `lib1` state!"
+    assert e.value._message == "Cannot access `lib1` state!" + NONREENTRANT_NOTE
 
     expected_hint = "add `uses: lib1` or `initializes: lib1` as a "
     expected_hint += "top-level statement to your contract"
     assert e.value._hint == expected_hint
 
 
 def test_missing_uses_for_read_inside_call(make_input_bundle):
@@ -532,15 +534,15 @@
     lib1.counter = 100
     """
     input_bundle = make_input_bundle({"lib1.vy": lib1, "lib2.vy": lib2})
 
     with pytest.raises(ImmutableViolation) as e:
         compile_code(main, input_bundle=input_bundle)
 
-    assert e.value._message == "Cannot access `lib1` state!"
+    assert e.value._message == "Cannot access `lib1` state!" + NONREENTRANT_NOTE
 
     expected_hint = "add `uses: lib1` or `initializes: lib1` as a "
     expected_hint += "top-level statement to your contract"
     assert e.value._hint == expected_hint
 
 
 def test_missing_uses_for_hashmap(make_input_bundle):
@@ -567,15 +569,15 @@
     lib1.counter = 100
     """
     input_bundle = make_input_bundle({"lib1.vy": lib1, "lib2.vy": lib2})
 
     with pytest.raises(ImmutableViolation) as e:
         compile_code(main, input_bundle=input_bundle)
 
-    assert e.value._message == "Cannot access `lib1` state!"
+    assert e.value._message == "Cannot access `lib1` state!" + NONREENTRANT_NOTE
 
     expected_hint = "add `uses: lib1` or `initializes: lib1` as a "
     expected_hint += "top-level statement to your contract"
     assert e.value._hint == expected_hint
 
 
 def test_missing_uses_for_tuple(make_input_bundle):
@@ -608,15 +610,15 @@
     lib1.counter = 100
     """
     input_bundle = make_input_bundle({"lib1.vy": lib1, "lib2.vy": lib2})
 
     with pytest.raises(ImmutableViolation) as e:
         compile_code(main, input_bundle=input_bundle)
 
-    assert e.value._message == "Cannot access `lib1` state!"
+    assert e.value._message == "Cannot access `lib1` state!" + NONREENTRANT_NOTE
 
     expected_hint = "add `uses: lib1` or `initializes: lib1` as a "
     expected_hint += "top-level statement to your contract"
     assert e.value._hint == expected_hint
 
 
 def test_missing_uses_for_tuple_function_call(make_input_bundle):
@@ -652,15 +654,15 @@
     lib1.counter = 100
     """
     input_bundle = make_input_bundle({"lib1.vy": lib1, "lib2.vy": lib2})
 
     with pytest.raises(ImmutableViolation) as e:
         compile_code(main, input_bundle=input_bundle)
 
-    assert e.value._message == "Cannot access `lib1` state!"
+    assert e.value._message == "Cannot access `lib1` state!" + NONREENTRANT_NOTE
 
     expected_hint = "add `uses: lib1` or `initializes: lib1` as a "
     expected_hint += "top-level statement to your contract"
     assert e.value._hint == expected_hint
 
 
 def test_missing_uses_function_call(make_input_bundle):
@@ -691,15 +693,15 @@
 initializes: lib1
     """
     input_bundle = make_input_bundle({"lib1.vy": lib1, "lib2.vy": lib2})
 
     with pytest.raises(ImmutableViolation) as e:
         compile_code(main, input_bundle=input_bundle)
 
-    assert e.value._message == "Cannot access `lib1` state!"
+    assert e.value._message == "Cannot access `lib1` state!" + NONREENTRANT_NOTE
 
     expected_hint = "add `uses: lib1` or `initializes: lib1` as a "
     expected_hint += "top-level statement to your contract"
     assert e.value._hint == expected_hint
 
 
 def test_missing_uses_nested_attribute(make_input_bundle):
@@ -730,15 +732,15 @@
     lib2.lib1.counter = new_value
     """
     input_bundle = make_input_bundle({"lib1.vy": lib1, "lib2.vy": lib2})
 
     with pytest.raises(ImmutableViolation) as e:
         compile_code(main, input_bundle=input_bundle)
 
-    assert e.value._message == "Cannot access `lib2` state!"
+    assert e.value._message == "Cannot access `lib2` state!" + NONREENTRANT_NOTE
 
     expected_hint = "add `uses: lib2` or `initializes: lib2` as a "
     expected_hint += "top-level statement to your contract"
     assert e.value._hint == expected_hint
 
 
 def test_missing_uses_subscript(make_input_bundle):
@@ -772,15 +774,15 @@
     lib2.lib1.foos[0].array[1] = new_value
     """
     input_bundle = make_input_bundle({"lib1.vy": lib1, "lib2.vy": lib2})
 
     with pytest.raises(ImmutableViolation) as e:
         compile_code(main, input_bundle=input_bundle)
 
-    assert e.value._message == "Cannot access `lib2` state!"
+    assert e.value._message == "Cannot access `lib2` state!" + NONREENTRANT_NOTE
 
     expected_hint = "add `uses: lib2` or `initializes: lib2` as a "
     expected_hint += "top-level statement to your contract"
     assert e.value._hint == expected_hint
 
 
 def test_missing_uses_nested_attribute_function_call(make_input_bundle):
@@ -815,15 +817,15 @@
     lib2.lib1.update_counter(new_value)
     """
     input_bundle = make_input_bundle({"lib1.vy": lib1, "lib2.vy": lib2})
 
     with pytest.raises(ImmutableViolation) as e:
         compile_code(main, input_bundle=input_bundle)
 
-    assert e.value._message == "Cannot access `lib2` state!"
+    assert e.value._message == "Cannot access `lib2` state!" + NONREENTRANT_NOTE
 
     expected_hint = "add `uses: lib2` or `initializes: lib2` as a "
     expected_hint += "top-level statement to your contract"
     assert e.value._hint == expected_hint
 
 
 def test_uses_skip_import(make_input_bundle):
@@ -849,15 +851,15 @@
     lib2.lib1.counter = new_value
     """
     input_bundle = make_input_bundle({"lib1.vy": lib1, "lib2.vy": lib2})
 
     with pytest.raises(ImmutableViolation) as e:
         compile_code(main, input_bundle=input_bundle)
 
-    assert e.value._message == "Cannot access `lib1` state!"
+    assert e.value._message == "Cannot access `lib1` state!" + NONREENTRANT_NOTE
 
     expected_hint = "add `uses: lib1` or `initializes: lib1` as a "
     expected_hint += "top-level statement to your contract"
     assert e.value._hint == expected_hint
 
 
 def test_uses_skip_import2(make_input_bundle):
@@ -911,15 +913,17 @@
 initializes: lib2[lib1 := lib1]
 initializes: lib1
     """
     input_bundle = make_input_bundle({"lib1.vy": lib1, "lib2.vy": lib2})
 
     with pytest.raises(BorrowException) as e:
         compile_code(main, input_bundle=input_bundle)
-    assert e.value._message == "`lib1` is declared as used, but it is not actually used in lib2.vy!"
+    expected = "`lib1` is declared as used, but its state is not"
+    expected += " actually used in lib2.vy!"
+    assert e.value._message == expected
     assert e.value._hint == "delete `uses: lib1`"
 
 
 def test_invalid_uses2(make_input_bundle, chdir_tmp_path):
     # test a more complicated invalid uses
     lib1 = """
 counter: uint256
@@ -952,15 +956,17 @@
 def foo():
     lib2.foo()
     """
     input_bundle = make_input_bundle({"lib1.vy": lib1, "lib2.vy": lib2})
 
     with pytest.raises(BorrowException) as e:
         compile_code(main, input_bundle=input_bundle)
-    assert e.value._message == "`lib1` is declared as used, but it is not actually used in lib2.vy!"
+    expected = "`lib1` is declared as used, but its state is not "
+    expected += "actually used in lib2.vy!"
+    assert e.value._message == expected
     assert e.value._hint == "delete `uses: lib1`"
 
 
 def test_initializes_uses_conflict(make_input_bundle):
     lib1 = """
 counter: uint256
     """
@@ -1288,7 +1294,58 @@
 initializes: lib2
     """
     input_bundle = make_input_bundle({"lib1.vy": lib1, "lib2.vy": lib2})
     with pytest.raises(InitializerException) as e:
         compile_code(main, input_bundle=input_bundle)
     assert e.value._message == "`lib2` uses `lib1`, but it is not initialized with `lib1`"
     assert e.value._hint == "try importing lib1 first"
+
+
+def test_nonreentrant_exports(make_input_bundle):
+    lib1 = """
+# lib1.vy
+@external
+@nonreentrant
+def bar():
+    pass
+    """
+    main = """
+import lib1
+
+exports: lib1.bar  # line 4
+
+@external
+def foo():
+    pass
+    """
+    input_bundle = make_input_bundle({"lib1.vy": lib1})
+    with pytest.raises(ImmutableViolation) as e:
+        compile_code(main, input_bundle=input_bundle)
+    assert e.value._message == "Cannot access `lib1` state!" + NONREENTRANT_NOTE
+    hint = "add `uses: lib1` or `initializes: lib1` as a top-level statement to your contract"
+    assert e.value._hint == hint
+    assert e.value.annotations[0].lineno == 4
+
+
+def test_internal_nonreentrant_import(make_input_bundle):
+    lib1 = """
+# lib1.vy
+@internal
+@nonreentrant
+def bar():
+    pass
+    """
+    main = """
+import lib1
+
+@external
+def foo():
+    lib1.bar()  # line 6
+    """
+    input_bundle = make_input_bundle({"lib1.vy": lib1})
+    with pytest.raises(ImmutableViolation) as e:
+        compile_code(main, input_bundle=input_bundle)
+    assert e.value._message == "Cannot access `lib1` state!" + NONREENTRANT_NOTE
+
+    hint = "add `uses: lib1` or `initializes: lib1` as a top-level statement to your contract"
+    assert e.value._hint == hint
+    assert e.value.annotations[0].lineno == 6
```

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/names/test_event_names.py` & `vyper-0.4.0rc2/tests/functional/syntax/names/test_event_names.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/names/test_function_names.py` & `vyper-0.4.0rc2/tests/functional/syntax/names/test_function_names.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/names/test_variable_names.py` & `vyper-0.4.0rc2/tests/functional/syntax/names/test_variable_names.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/signatures/test_invalid_function_decorators.py` & `vyper-0.4.0rc2/tests/functional/syntax/signatures/test_invalid_function_decorators.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/signatures/test_method_id_conflicts.py` & `vyper-0.4.0rc2/tests/functional/syntax/signatures/test_method_id_conflicts.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_abi_decode.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_abi_decode.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_abi_encode.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_abi_encode.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_abs.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_abs.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_addmulmod.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_addmulmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_address_code.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_address_code.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_ann_assign.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_ann_assign.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_as_uint256.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_as_uint256.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_as_wei_value.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_as_wei_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_block.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_block.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_blockscope.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_blockscope.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_bool.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_bool.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_bool_ops.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_bool_ops.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_bytes.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_bytes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_chainid.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_chainid.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_code_size.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_code_size.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_codehash.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_codehash.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_concat.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_concat.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_constants.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_constants.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_create_with_code_of.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_create_with_code_of.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_dynamic_array.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_dynamic_array.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_external_calls.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_external_calls.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_extract32.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_extract32.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_flag.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_flag.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_for_range.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_for_range.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_functions_call.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_functions_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_immutables.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_immutables.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_init.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_init.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_interfaces.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_invalids.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_invalids.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_keccak256.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_keccak256.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_len.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_len.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_list.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_list.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_logging.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_logging.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_method_id.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_method_id.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_minmax.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_minmax.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_minmax_value.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_minmax_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_msg_data.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_msg_data.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_nested_list.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_nested_list.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_no_none.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_no_none.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_powmod.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_powmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_print.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_print.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_public.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_public.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_raw_call.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_raw_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_return_tuple.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_return_tuple.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_self_balance.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_self_balance.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_selfdestruct.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_selfdestruct.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_send.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_send.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_slice.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_slice.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_string.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_string.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_structs.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_structs.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_ternary.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_ternary.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_tuple_assign.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_tuple_assign.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/functional/syntax/test_unbalanced_return.py` & `vyper-0.4.0rc2/tests/functional/syntax/test_unbalanced_return.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/abi_types/test_invalid_abi_types.py` & `vyper-0.4.0rc2/tests/unit/abi_types/test_invalid_abi_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/ast/nodes/test_compare_nodes.py` & `vyper-0.4.0rc2/tests/unit/ast/nodes/test_compare_nodes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/ast/nodes/test_fold_binop_decimal.py` & `vyper-0.4.0rc2/tests/unit/ast/nodes/test_fold_binop_decimal.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/ast/nodes/test_fold_binop_int.py` & `vyper-0.4.0rc2/tests/unit/ast/nodes/test_fold_binop_int.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/ast/nodes/test_fold_boolop.py` & `vyper-0.4.0rc2/tests/unit/ast/nodes/test_fold_boolop.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/ast/nodes/test_fold_compare.py` & `vyper-0.4.0rc2/tests/unit/ast/nodes/test_fold_compare.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/ast/nodes/test_fold_unaryop.py` & `vyper-0.4.0rc2/tests/unit/ast/nodes/test_fold_unaryop.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/ast/nodes/test_from_node.py` & `vyper-0.4.0rc2/tests/unit/ast/nodes/test_from_node.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/ast/nodes/test_get_children.py` & `vyper-0.4.0rc2/tests/unit/ast/nodes/test_get_children.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/ast/nodes/test_get_descendants.py` & `vyper-0.4.0rc2/tests/unit/ast/nodes/test_get_descendants.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/ast/nodes/test_hex.py` & `vyper-0.4.0rc2/tests/unit/ast/nodes/test_hex.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/ast/test_annotate_and_optimize_ast.py` & `vyper-0.4.0rc2/tests/unit/ast/test_annotate_and_optimize_ast.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/ast/test_ast_dict.py` & `vyper-0.4.0rc2/tests/unit/ast/test_ast_dict.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/ast/test_metadata_journal.py` & `vyper-0.4.0rc2/tests/unit/ast/test_metadata_journal.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/ast/test_natspec.py` & `vyper-0.4.0rc2/tests/unit/ast/test_natspec.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/ast/test_parser.py` & `vyper-0.4.0rc2/tests/unit/ast/test_parser.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/ast/test_pre_parser.py` & `vyper-0.4.0rc2/tests/unit/ast/test_pre_parser.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/ast/test_source_annotation.py` & `vyper-0.4.0rc2/tests/unit/ast/test_source_annotation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/cli/storage_layout/test_storage_layout.py` & `vyper-0.4.0rc2/tests/unit/cli/storage_layout/test_storage_layout.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/cli/storage_layout/test_storage_layout_overrides.py` & `vyper-0.4.0rc2/tests/unit/cli/storage_layout/test_storage_layout_overrides.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/cli/vyper_compile/test_compile_files.py` & `vyper-0.4.0rc2/tests/unit/cli/vyper_compile/test_compile_files.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/cli/vyper_compile/test_parse_args.py` & `vyper-0.4.0rc2/tests/unit/cli/vyper_compile/test_parse_args.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/cli/vyper_json/test_compile_json.py` & `vyper-0.4.0rc2/tests/unit/cli/vyper_json/test_compile_json.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/cli/vyper_json/test_get_inputs.py` & `vyper-0.4.0rc2/tests/unit/cli/vyper_json/test_get_inputs.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/cli/vyper_json/test_get_settings.py` & `vyper-0.4.0rc2/tests/unit/cli/vyper_json/test_get_settings.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/cli/vyper_json/test_output_selection.py` & `vyper-0.4.0rc2/tests/unit/cli/vyper_json/test_output_selection.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/cli/vyper_json/test_parse_args_vyperjson.py` & `vyper-0.4.0rc2/tests/unit/cli/vyper_json/test_parse_args_vyperjson.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/compiler/asm/test_asm_optimizer.py` & `vyper-0.4.0rc2/tests/unit/compiler/asm/test_asm_optimizer.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/compiler/ir/test_compile_ir.py` & `vyper-0.4.0rc2/tests/unit/compiler/ir/test_compile_ir.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/compiler/ir/test_optimize_ir.py` & `vyper-0.4.0rc2/tests/unit/compiler/ir/test_optimize_ir.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/compiler/ir/test_with.py` & `vyper-0.4.0rc2/tests/unit/compiler/ir/test_with.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/compiler/test_abi.py` & `vyper-0.4.0rc2/tests/unit/compiler/test_abi.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/compiler/test_bytecode_runtime.py` & `vyper-0.4.0rc2/tests/unit/compiler/test_bytecode_runtime.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/compiler/test_compile_code.py` & `vyper-0.4.0rc2/tests/unit/compiler/test_compile_code.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/compiler/test_default_settings.py` & `vyper-0.4.0rc2/tests/unit/compiler/test_default_settings.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/compiler/test_input_bundle.py` & `vyper-0.4.0rc2/tests/unit/compiler/test_input_bundle.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/compiler/test_opcodes.py` & `vyper-0.4.0rc2/tests/unit/compiler/test_opcodes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/compiler/test_pre_parser.py` & `vyper-0.4.0rc2/tests/unit/compiler/test_pre_parser.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/compiler/test_sha3_32.py` & `vyper-0.4.0rc2/tests/unit/compiler/test_sha3_32.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/compiler/test_source_map.py` & `vyper-0.4.0rc2/tests/unit/compiler/test_source_map.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/compiler/venom/test_convert_basicblock_simple.py` & `vyper-0.4.0rc2/tests/unit/compiler/venom/test_convert_basicblock_simple.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/compiler/venom/test_dominator_tree.py` & `vyper-0.4.0rc2/tests/unit/compiler/venom/test_dominator_tree.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/compiler/venom/test_duplicate_operands.py` & `vyper-0.4.0rc2/tests/unit/compiler/venom/test_duplicate_operands.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/compiler/venom/test_make_ssa.py` & `vyper-0.4.0rc2/tests/unit/compiler/venom/test_make_ssa.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/compiler/venom/test_multi_entry_block.py` & `vyper-0.4.0rc2/tests/unit/compiler/venom/test_multi_entry_block.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/semantics/analysis/test_array_index.py` & `vyper-0.4.0rc2/tests/unit/semantics/analysis/test_array_index.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/semantics/analysis/test_cyclic_function_calls.py` & `vyper-0.4.0rc2/tests/unit/semantics/analysis/test_cyclic_function_calls.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/semantics/analysis/test_for_loop.py` & `vyper-0.4.0rc2/tests/unit/semantics/analysis/test_for_loop.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/semantics/analysis/test_potential_types.py` & `vyper-0.4.0rc2/tests/unit/semantics/analysis/test_potential_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/semantics/conftest.py` & `vyper-0.4.0rc2/tests/unit/semantics/conftest.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/semantics/test_namespace.py` & `vyper-0.4.0rc2/tests/unit/semantics/test_namespace.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/semantics/test_storage_slots.py` & `vyper-0.4.0rc2/tests/unit/semantics/test_storage_slots.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/semantics/types/test_event.py` & `vyper-0.4.0rc2/tests/unit/semantics/types/test_event.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/semantics/types/test_pure_types.py` & `vyper-0.4.0rc2/tests/unit/semantics/types/test_pure_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/semantics/types/test_size_in_bytes.py` & `vyper-0.4.0rc2/tests/unit/semantics/types/test_size_in_bytes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/semantics/types/test_type_from_abi.py` & `vyper-0.4.0rc2/tests/unit/semantics/types/test_type_from_abi.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/unit/semantics/types/test_type_from_annotation.py` & `vyper-0.4.0rc2/tests/unit/semantics/types/test_type_from_annotation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/tests/utils.py` & `vyper-0.4.0rc2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/__init__.py` & `vyper-0.4.0rc2/vyper/__init__.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/__main__.py` & `vyper-0.4.0rc2/vyper/__main__.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/abi_types.py` & `vyper-0.4.0rc2/vyper/abi_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/ast/README.md` & `vyper-0.4.0rc2/vyper/ast/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/ast/grammar.lark` & `vyper-0.4.0rc2/vyper/ast/grammar.lark`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/ast/grammar.py` & `vyper-0.4.0rc2/vyper/ast/grammar.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/ast/identifiers.py` & `vyper-0.4.0rc2/vyper/ast/identifiers.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/ast/metadata.py` & `vyper-0.4.0rc2/vyper/ast/metadata.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/ast/natspec.py` & `vyper-0.4.0rc2/vyper/ast/natspec.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/ast/nodes.py` & `vyper-0.4.0rc2/vyper/ast/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,14 +417,19 @@
         is not foldable.
         """
         try:
             return self._metadata["folded_value"]
         except KeyError:
             raise UnfoldableNode("not foldable", self)
 
+    def reduced(self) -> "ExprNode":
+        if self.has_folded_value:
+            return self.get_folded_value()
+        return self
+
     def _set_folded_value(self, node: "VyperNode") -> None:
         # sanity check this is only called once
         assert "folded_value" not in self._metadata
 
         # set the "original node" so that exceptions can point to the original
         # node and not the folded node
         cls = node.__class__
```

### Comparing `vyper-0.4.0rc1/vyper/ast/nodes.pyi` & `vyper-0.4.0rc2/vyper/ast/nodes.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     def has_folded_value(self): ...
     @property
     def parent(self): ...
     @classmethod
     def get_fields(cls: Any) -> set: ...
     def set_parent(self, parent: VyperNode) -> VyperNode: ...
     def get_folded_value(self) -> ExprNode: ...
+    def reduced(self) -> ExprNode: ...
     def _set_folded_value(self, node: ExprNode) -> None: ...
     @classmethod
     def from_node(cls, node: VyperNode, **kwargs: Any) -> Any: ...
     def to_dict(self) -> dict: ...
     def get_children(
         self,
         node_type: Union[Type[VyperNode], Sequence[Type[VyperNode]], None] = ...,
```

### Comparing `vyper-0.4.0rc1/vyper/ast/parse.py` & `vyper-0.4.0rc2/vyper/ast/parse.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/ast/pre_parser.py` & `vyper-0.4.0rc2/vyper/ast/pre_parser.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/ast/utils.py` & `vyper-0.4.0rc2/vyper/ast/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/ast/validation.py` & `vyper-0.4.0rc2/vyper/ast/validation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/builtins/_convert.py` & `vyper-0.4.0rc2/vyper/builtins/_convert.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/builtins/_signatures.py` & `vyper-0.4.0rc2/vyper/builtins/_signatures.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/builtins/_utils.py` & `vyper-0.4.0rc2/vyper/builtins/_utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/builtins/functions.py` & `vyper-0.4.0rc2/vyper/builtins/functions.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/builtins/interfaces/IERC20.vyi` & `vyper-0.4.0rc2/vyper/builtins/interfaces/IERC20.vyi`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/builtins/interfaces/IERC4626.vyi` & `vyper-0.4.0rc2/vyper/builtins/interfaces/IERC4626.vyi`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/builtins/interfaces/IERC721.vyi` & `vyper-0.4.0rc2/vyper/builtins/interfaces/IERC721.vyi`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/cli/vyper_compile.py` & `vyper-0.4.0rc2/vyper/cli/vyper_compile.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/cli/vyper_ir.py` & `vyper-0.4.0rc2/vyper/cli/vyper_ir.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/cli/vyper_json.py` & `vyper-0.4.0rc2/vyper/cli/vyper_json.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/codegen/abi_encoder.py` & `vyper-0.4.0rc2/vyper/codegen/abi_encoder.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/codegen/arithmetic.py` & `vyper-0.4.0rc2/vyper/codegen/arithmetic.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/codegen/context.py` & `vyper-0.4.0rc2/vyper/codegen/context.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/codegen/core.py` & `vyper-0.4.0rc2/vyper/codegen/core.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/codegen/events.py` & `vyper-0.4.0rc2/vyper/codegen/events.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/codegen/expr.py` & `vyper-0.4.0rc2/vyper/codegen/expr.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,16 +67,15 @@
 
 
 class Expr:
     # TODO: Once other refactors are made reevaluate all inline imports
 
     def __init__(self, node, context, is_stmt=False):
         assert isinstance(node, vy_ast.VyperNode)
-        if node.has_folded_value:
-            node = node.get_folded_value()
+        node = node.reduced()
 
         self.expr = node
         self.context = context
         self.is_stmt = is_stmt  # this came from an Expr node
 
         fn_name = f"parse_{type(node).__name__}"
         with tag_exceptions(node, fallback_exception_type=CodegenPanic, note=fn_name):
@@ -343,15 +342,17 @@
                 # we have to hash the key to get a storage location
                 index = keccak256_helper(index, self.context)
 
         elif is_array_like(sub.typ):
             index = Expr.parse_value_expr(self.expr.slice, self.context)
 
         elif is_tuple_like(sub.typ):
-            index = self.expr.slice.n
+            # should we annotate expr.slice in the frontend with the
+            # folded value instead of calling reduced() here?
+            index = self.expr.slice.reduced().n
             # note: this check should also happen in get_element_ptr
             if not 0 <= index < len(sub.typ.member_types):
                 raise TypeCheckFailure("unreachable")
         else:
             raise TypeCheckFailure("unreachable")
 
         ir_node = get_element_ptr(sub, index)
```

### Comparing `vyper-0.4.0rc1/vyper/codegen/external_call.py` & `vyper-0.4.0rc2/vyper/codegen/external_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/codegen/function_definitions/common.py` & `vyper-0.4.0rc2/vyper/codegen/function_definitions/common.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/codegen/function_definitions/external_function.py` & `vyper-0.4.0rc2/vyper/codegen/function_definitions/external_function.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/codegen/function_definitions/internal_function.py` & `vyper-0.4.0rc2/vyper/codegen/function_definitions/internal_function.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/codegen/ir_node.py` & `vyper-0.4.0rc2/vyper/codegen/ir_node.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/codegen/jumptable_utils.py` & `vyper-0.4.0rc2/vyper/codegen/jumptable_utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/codegen/keccak256_helper.py` & `vyper-0.4.0rc2/vyper/codegen/keccak256_helper.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/codegen/memory_allocator.py` & `vyper-0.4.0rc2/vyper/codegen/memory_allocator.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/codegen/module.py` & `vyper-0.4.0rc2/vyper/codegen/module.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/codegen/return_.py` & `vyper-0.4.0rc2/vyper/codegen/return_.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/codegen/self_call.py` & `vyper-0.4.0rc2/vyper/codegen/self_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/codegen/stmt.py` & `vyper-0.4.0rc2/vyper/codegen/stmt.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/compiler/README.md` & `vyper-0.4.0rc2/vyper/compiler/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/compiler/__init__.py` & `vyper-0.4.0rc2/vyper/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/compiler/input_bundle.py` & `vyper-0.4.0rc2/vyper/compiler/input_bundle.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/compiler/output.py` & `vyper-0.4.0rc2/vyper/compiler/output.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/compiler/phases.py` & `vyper-0.4.0rc2/vyper/compiler/phases.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/compiler/settings.py` & `vyper-0.4.0rc2/vyper/compiler/settings.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/compiler/utils.py` & `vyper-0.4.0rc2/vyper/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/evm/address_space.py` & `vyper-0.4.0rc2/vyper/evm/address_space.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/evm/opcodes.py` & `vyper-0.4.0rc2/vyper/evm/opcodes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/exceptions.py` & `vyper-0.4.0rc2/vyper/exceptions.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/ir/README.md` & `vyper-0.4.0rc2/vyper/ir/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/ir/compile_ir.py` & `vyper-0.4.0rc2/vyper/ir/compile_ir.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/ir/optimizer.py` & `vyper-0.4.0rc2/vyper/ir/optimizer.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/ir/s_expressions.py` & `vyper-0.4.0rc2/vyper/ir/s_expressions.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/semantics/README.md` & `vyper-0.4.0rc2/vyper/semantics/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/semantics/analysis/base.py` & `vyper-0.4.0rc2/vyper/semantics/analysis/base.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/semantics/analysis/common.py` & `vyper-0.4.0rc2/vyper/semantics/analysis/common.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/semantics/analysis/constant_folding.py` & `vyper-0.4.0rc2/vyper/semantics/analysis/constant_folding.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/semantics/analysis/data_positions.py` & `vyper-0.4.0rc2/vyper/semantics/analysis/data_positions.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/semantics/analysis/getters.py` & `vyper-0.4.0rc2/vyper/semantics/analysis/getters.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/semantics/analysis/global_.py` & `vyper-0.4.0rc2/vyper/semantics/analysis/global_.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/semantics/analysis/import_graph.py` & `vyper-0.4.0rc2/vyper/semantics/analysis/import_graph.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/semantics/analysis/levenshtein_utils.py` & `vyper-0.4.0rc2/vyper/semantics/analysis/levenshtein_utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/semantics/analysis/local.py` & `vyper-0.4.0rc2/vyper/semantics/analysis/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# CMC 2024-02-03 TODO: split me into function.py and expr.py
+# CMC 2024-02-03 TODO: rename me to function.py
 
 import contextlib
 from typing import Optional
 
 from vyper import ast as vy_ast
 from vyper.ast.validation import validate_call_args
 from vyper.exceptions import (
@@ -31,14 +31,15 @@
 )
 from vyper.semantics.analysis.common import VyperNodeVisitorBase
 from vyper.semantics.analysis.utils import (
     get_common_types,
     get_exact_type_from_node,
     get_expr_info,
     get_possible_types_from_node,
+    uses_state,
     validate_expected_type,
 )
 from vyper.semantics.data_locations import DataLocation
 from vyper.semantics.environment import CONSTANT_ENVIRONMENT_VARS
 from vyper.semantics.namespace import get_namespace
 from vyper.semantics.types import (
     TYPE_T,
@@ -60,38 +61,38 @@
     is_type_t,
     map_void,
 )
 from vyper.semantics.types.function import ContractFunctionT, MemberFunctionT, StateMutability
 from vyper.semantics.types.utils import type_from_annotation
 
 
-def validate_functions(vy_module: vy_ast.Module) -> None:
+def analyze_functions(vy_module: vy_ast.Module) -> None:
     """Analyzes a vyper ast and validates the function bodies"""
     err_list = ExceptionList()
 
     for node in vy_module.get_children(vy_ast.FunctionDef):
-        _validate_function_r(vy_module, node, err_list)
+        _analyze_function_r(vy_module, node, err_list)
 
     for node in vy_module.get_children(vy_ast.VariableDecl):
         if not node.is_public:
             continue
-        _validate_function_r(vy_module, node._expanded_getter, err_list)
+        _analyze_function_r(vy_module, node._expanded_getter, err_list)
 
     err_list.raise_if_not_empty()
 
 
-def _validate_function_r(
+def _analyze_function_r(
     vy_module: vy_ast.Module, node: vy_ast.FunctionDef, err_list: ExceptionList
 ):
     func_t = node._metadata["func_type"]
 
     for call_t in func_t.called_functions:
         if isinstance(call_t, ContractFunctionT):
             assert isinstance(call_t.ast_def, vy_ast.FunctionDef)  # help mypy
-            _validate_function_r(vy_module, call_t.ast_def, err_list)
+            _analyze_function_r(vy_module, call_t.ast_def, err_list)
 
     namespace = get_namespace()
 
     try:
         with namespace.enter_scope():
             analyzer = FunctionAnalyzer(vy_module, node, namespace)
             analyzer.analyze()
@@ -263,15 +264,22 @@
     module_infos = _get_module_chain(node)
 
     if len(module_infos) == 0:
         return None
 
     for module_info in module_infos:
         if module_info.ownership < ModuleOwnership.USES:
-            msg = f"Cannot access `{module_info.alias}` state!"
+            msg = f"Cannot access `{module_info.alias}` state!\n  note that"
+            # CMC 2024-04-12 add UX note about nonreentrant. might be nice
+            # in the future to be more specific about exactly which state is
+            # used, although that requires threading a bit more context into
+            # this function.
+            msg += " use of the `@nonreentrant` decorator is also considered"
+            msg += " state access"
+
             hint = f"add `uses: {module_info.alias}` or "
             hint += f"`initializes: {module_info.alias}` as "
             hint += "a top-level statement to your contract"
             raise ImmutableViolation(msg, hint=hint)
 
     # the leftmost- referenced module
     root_module_info = module_infos[0]
@@ -439,18 +447,15 @@
             raise ImmutableViolation("Constant value cannot be written to.")
 
         var_access = _get_variable_access(target)
         assert var_access is not None
 
         info._writes.add(var_access)
 
-    def _handle_module_access(self, var_access: VarAccess, target: vy_ast.ExprNode):
-        if not var_access.variable.is_state_variable():
-            return
-
+    def _handle_module_access(self, target: vy_ast.ExprNode):
         root_module_info = check_module_uses(target)
 
         if root_module_info is not None:
             # log the access
             self.func.mark_used_module(root_module_info)
 
     def visit_Assign(self, node):
@@ -523,17 +528,15 @@
         args = iter_node.args
         kwargs = [s.value for s in iter_node.keywords]
         for arg in (*args, *kwargs):
             self.expr_visitor.visit(arg, target_type)
 
     def _analyse_list_iter(self, iter_node, target_type):
         # iteration over a variable or literal list
-        iter_val = iter_node
-        if iter_val.has_folded_value:
-            iter_val = iter_val.get_folded_value()
+        iter_val = iter_node.reduced()
 
         if isinstance(iter_val, vy_ast.List):
             len_ = len(iter_val.elements)
             if len_ == 0:
                 raise StructureException("For loop must have at least 1 iteration", iter_node)
             iter_type = SArrayT(target_type, len_)
         else:
@@ -680,17 +683,17 @@
 
                         msg = "Cannot modify loop variable"
                         var = s.variable
                         if var.decl_node is not None:
                             msg += f" `{var.decl_node.target.id}`"
                         raise ImmutableViolation(msg, var.decl_node, node)
 
-                variable_accesses = info._writes | info._reads
-                for s in variable_accesses:
-                    self.function_analyzer._handle_module_access(s, node)
+                var_accesses = info._writes | info._reads
+                if uses_state(var_accesses):
+                    self.function_analyzer._handle_module_access(node)
 
                 self.func.mark_variable_writes(info._writes)
                 self.func.mark_variable_reads(info._reads)
 
         # validate and annotate folded value
         if node.has_folded_value:
             folded_node = node.get_folded_value()
@@ -785,16 +788,16 @@
                 for s in func_type.get_variable_reads():
                     if s.variable.is_state_variable():
                         func_info._reads.add(s)
 
             if self.function_analyzer:
                 self._check_call_mutability(func_type.mutability)
 
-                for s in func_type.get_variable_accesses():
-                    self.function_analyzer._handle_module_access(s, node.func)
+                if func_type.uses_state():
+                    self.function_analyzer._handle_module_access(node.func)
 
                 if func_type.is_deploy and not self.func.is_deploy:
                     raise CallViolation(
                         f"Cannot call an @{func_type.visibility} function from "
                         f"an @{self.func.visibility} function!",
                         node,
                     )
@@ -942,20 +945,18 @@
     :param node: call to range()
     :return: None
     """
     assert node.func.get("id") == "range"
     validate_call_args(node, (1, 2), kwargs=["bound"])
     kwargs = {s.arg: s.value for s in node.keywords or []}
     start, end = (vy_ast.Int(value=0), node.args[0]) if len(node.args) == 1 else node.args
-    start, end = [i.get_folded_value() if i.has_folded_value else i for i in (start, end)]
+    start, end = [i.reduced() for i in (start, end)]
 
     if "bound" in kwargs:
-        bound = kwargs["bound"]
-        if bound.has_folded_value:
-            bound = bound.get_folded_value()
+        bound = kwargs["bound"].reduced()
         if not isinstance(bound, vy_ast.Int):
             raise StructureException("Bound must be a literal integer", bound)
         if bound.value <= 0:
             raise StructureException("Bound must be at least 1", bound)
         if isinstance(start, vy_ast.Int) and isinstance(end, vy_ast.Int):
             error = "Please remove the `bound=` kwarg when using range with constants"
             raise StructureException(error, bound)
```

### Comparing `vyper-0.4.0rc1/vyper/semantics/analysis/module.py` & `vyper-0.4.0rc2/vyper/semantics/analysis/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     BorrowException,
     CallViolation,
     DuplicateImport,
     EvmVersionException,
     ExceptionList,
     ImmutableViolation,
     InitializerException,
+    InterfaceViolation,
     InvalidLiteral,
     InvalidType,
     ModuleNotFound,
     StateAccessViolation,
     StructureException,
     UndeclaredDefinition,
     VyperException,
@@ -39,15 +40,15 @@
     UsesInfo,
     VarInfo,
 )
 from vyper.semantics.analysis.common import VyperNodeVisitorBase
 from vyper.semantics.analysis.constant_folding import constant_fold
 from vyper.semantics.analysis.getters import generate_public_variable_getters
 from vyper.semantics.analysis.import_graph import ImportGraph
-from vyper.semantics.analysis.local import ExprVisitor, check_module_uses, validate_functions
+from vyper.semantics.analysis.local import ExprVisitor, analyze_functions, check_module_uses
 from vyper.semantics.analysis.utils import (
     check_modifiability,
     get_exact_type_from_node,
     get_expr_info,
 )
 from vyper.semantics.data_locations import DataLocation
 from vyper.semantics.namespace import Namespace, get_namespace, override_global_namespace
@@ -98,15 +99,15 @@
 
         ret = ModuleT(module_ast)
         module_ast._metadata["type"] = ret
 
         # if this is an interface, the function is already validated
         # in `ContractFunction.from_vyi()`
         if not is_interface:
-            validate_functions(module_ast)
+            analyze_functions(module_ast)
             analyzer.validate_initialized_modules()
             analyzer.validate_used_modules()
 
     return ret
 
 
 def _analyze_call_graph(module_ast: vy_ast.Module):
@@ -311,15 +312,15 @@
             if used_module in should_use:
                 del should_use[used_module]
 
         if len(should_use) > 0:
             err_list = ExceptionList()
             for used_module_info, uses_info in should_use.values():
                 msg = f"`{used_module_info.alias}` is declared as used, but "
-                msg += f"it is not actually used in {module_t}!"
+                msg += f"its state is not actually used in {module_t}!"
                 hint = f"delete `uses: {used_module_info.alias}`"
                 err_list.append(BorrowException(msg, uses_info.node, hint=hint))
 
             err_list.raise_if_not_empty()
 
     def validate_initialized_modules(self):
         # check all `initializes:` modules have `__init__()` called exactly once
@@ -526,60 +527,93 @@
         # note: try to refactor. not a huge fan of mutating the
         # ModuleInfo after it's constructed
         module_info.set_ownership(ModuleOwnership.INITIALIZES, node)
         node._metadata["initializes_info"] = InitializesInfo(module_info, dependencies, node)
 
     def visit_ExportsDecl(self, node):
         items = vy_ast.as_tuple(node.annotation)
-        funcs = []
+        exported_funcs = []
         used_modules = OrderedSet()
 
+        # CMC 2024-04-13 TODO: reduce nesting in this function
+
         for item in items:
             # set is_callable=True to give better error messages for imported
             # types, e.g. exports: some_module.MyEvent
             info = get_expr_info(item, is_callable=True)
+
             if info.var_info is not None:
-                decl_node = info.var_info.decl_node
+                decl = info.var_info.decl_node
                 if not info.var_info.is_public:
-                    raise StructureException("not a public variable!", decl_node, item)
-                func_t = decl_node._expanded_getter._metadata["func_type"]
-
-            else:
+                    raise StructureException("not a public variable!", decl, item)
+                funcs = [decl._expanded_getter._metadata["func_type"]]
+            elif isinstance(info.typ, ContractFunctionT):
                 # regular function
-                func_t = info.typ
-                decl_node = func_t.decl_node
+                funcs = [info.typ]
+            elif isinstance(info.typ, InterfaceT):
+                if not isinstance(item, vy_ast.Attribute):
+                    raise StructureException(
+                        "invalid export",
+                        hint="exports should look like <module>.<function | interface>",
+                    )
+
+                module_info = get_expr_info(item.value).module_info
+                if module_info is None:
+                    raise StructureException("not a valid module!", item.value)
+
+                if info.typ not in module_info.typ.implemented_interfaces:
+                    iface_str = item.node_source_code
+                    module_str = item.value.node_source_code
+                    msg = f"requested `{iface_str}` but `{module_str}`"
+                    msg += f" does not implement `{iface_str}`!"
+                    raise InterfaceViolation(msg, item)
+
+                module_exposed_fns = {fn.name: fn for fn in module_info.typ.exposed_functions}
+                # find the specific implementation of the function in the module
+                funcs = [
+                    module_exposed_fns[fn.name]
+                    for fn in info.typ.functions.values()
+                    if fn.is_external
+                ]
+            else:
+                raise StructureException(
+                    f"not a function or interface: `{info.typ}`", info.typ.decl_node, item
+                )
+
+            for func_t in funcs:
+                if not func_t.is_external:
+                    raise StructureException(
+                        "can't export non-external functions!", func_t.decl_node, item
+                    )
+
+                self._add_exposed_function(func_t, item, relax=False)
+                with tag_exceptions(item):  # tag exceptions with specific item
+                    self._self_t.typ.add_member(func_t.name, func_t)
+
+                    exported_funcs.append(func_t)
+
+                    # check module uses
+                    if func_t.uses_state():
+                        module_info = check_module_uses(item)
+
+                        # guaranteed by above checks:
+                        assert module_info is not None
 
-            if not isinstance(func_t, ContractFunctionT):
-                raise StructureException(f"not a function: `{func_t}`", decl_node, item)
-            if not func_t.is_external:
-                raise StructureException("can't export non-external functions!", decl_node, item)
-
-            self._add_exposed_function(func_t, item, relax=False)
-            with tag_exceptions(item):  # tag with specific item
-                self._self_t.typ.add_member(func_t.name, func_t)
-
-            funcs.append(func_t)
-
-            # check module uses
-            var_accesses = func_t.get_variable_accesses()
-            if any(s.variable.is_state_variable() for s in var_accesses):
-                module_info = check_module_uses(item)
-                assert module_info is not None  # guaranteed by above checks
-                used_modules.add(module_info)
+                        used_modules.add(module_info)
 
-        node._metadata["exports_info"] = ExportsInfo(funcs, used_modules)
+        node._metadata["exports_info"] = ExportsInfo(exported_funcs, used_modules)
 
     @property
     def _self_t(self):
         return self.namespace["self"]
 
     def _add_exposed_function(self, func_t, node, relax=True):
         # call this before self._self_t.typ.add_member() for exception raising
         # priority
-        if (prev_decl := self._exposed_functions.get(func_t)) is not None:
+        if not relax and (prev_decl := self._exposed_functions.get(func_t)) is not None:
             raise StructureException("already exported!", node, prev_decl=prev_decl)
 
         self._exposed_functions[func_t] = node
 
     def visit_VariableDecl(self, node):
         # postcondition of VariableDecl.validate
         assert isinstance(node.target, vy_ast.Name)
```

### Comparing `vyper-0.4.0rc1/vyper/semantics/analysis/utils.py` & `vyper-0.4.0rc2/vyper/semantics/analysis/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import itertools
-from typing import Callable, List
+from typing import Callable, Iterable, List
 
 from vyper import ast as vy_ast
 from vyper.exceptions import (
     CompilerPanic,
     InvalidLiteral,
     InvalidOperation,
     InvalidReference,
@@ -13,15 +13,15 @@
     TypeMismatch,
     UndeclaredDefinition,
     UnknownAttribute,
     VyperException,
     ZeroDivisionException,
 )
 from vyper.semantics import types
-from vyper.semantics.analysis.base import ExprInfo, Modifiability, ModuleInfo, VarInfo
+from vyper.semantics.analysis.base import ExprInfo, Modifiability, ModuleInfo, VarAccess, VarInfo
 from vyper.semantics.analysis.levenshtein_utils import get_levenshtein_error_suggestions
 from vyper.semantics.namespace import get_namespace
 from vyper.semantics.types.base import TYPE_T, VyperType
 from vyper.semantics.types.bytestrings import BytesT, StringT
 from vyper.semantics.types.primitives import AddressT, BoolT, BytesM_T, IntegerT
 from vyper.semantics.types.subscriptable import DArrayT, SArrayT, TupleT
 from vyper.utils import checksum_encode, int_to_fourbytes
@@ -44,14 +44,18 @@
 
     if ret:
         return ret
 
     raise err_list[0]
 
 
+def uses_state(var_accesses: Iterable[VarAccess]) -> bool:
+    return any(s.variable.is_state_variable() for s in var_accesses)
+
+
 class _ExprAnalyser:
     """
     Node type-checker class.
 
     Type-check logic is implemented in `type_from_<NODE_CLASS>` methods, organized
     according to the Vyper ast node class. Calls to `get_exact_type_from_node` and
     `get_possible_types_from_node` are forwarded to this class, where the node
```

### Comparing `vyper-0.4.0rc1/vyper/semantics/environment.py` & `vyper-0.4.0rc2/vyper/semantics/environment.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/semantics/namespace.py` & `vyper-0.4.0rc2/vyper/semantics/namespace.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/semantics/types/__init__.py` & `vyper-0.4.0rc2/vyper/semantics/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/semantics/types/base.py` & `vyper-0.4.0rc2/vyper/semantics/types/base.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/semantics/types/bytestrings.py` & `vyper-0.4.0rc2/vyper/semantics/types/bytestrings.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/semantics/types/function.py` & `vyper-0.4.0rc2/vyper/semantics/types/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     StateMutability,
     VarAccess,
     VarOffset,
 )
 from vyper.semantics.analysis.utils import (
     check_modifiability,
     get_exact_type_from_node,
+    uses_state,
     validate_expected_type,
 )
 from vyper.semantics.data_locations import DataLocation
 from vyper.semantics.types.base import KwargSettings, VyperType
 from vyper.semantics.types.primitives import BoolT
 from vyper.semantics.types.shortcuts import UINT256_T
 from vyper.semantics.types.subscriptable import TupleT
@@ -159,15 +160,19 @@
 
     def get_variable_writes(self):
         return self._variable_writes
 
     def get_variable_accesses(self):
         return self._variable_reads | self._variable_writes
 
+    def uses_state(self):
+        return self.nonreentrant or uses_state(self.get_variable_accesses())
+
     def get_used_modules(self):
+        # _used_modules is populated during analysis
         return self._used_modules
 
     def mark_used_module(self, module_info):
         self._used_modules.add(module_info)
 
     def mark_variable_writes(self, var_infos):
         self._variable_writes.update(var_infos)
```

### Comparing `vyper-0.4.0rc1/vyper/semantics/types/module.py` & `vyper-0.4.0rc2/vyper/semantics/types/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -327,14 +327,16 @@
             if hasattr(import_info.typ, "module_t"):
                 self._helper.add_member(import_info.alias, TYPE_T(import_info.typ))
 
         for name, interface_t in self.interfaces.items():
             # can access interfaces in type position
             self._helper.add_member(name, TYPE_T(interface_t))
 
+        self.add_member("__interface__", self.interface)
+
     # __eq__ is very strict on ModuleT - object equality! this is because we
     # don't want to reason about where a module came from (i.e. input bundle,
     # search path, symlinked vs normalized path, etc.)
     def __eq__(self, other):
         return self is other
 
     def __hash__(self):
@@ -368,14 +370,23 @@
         return self._module.get_children(vy_ast.InterfaceDef)
 
     @cached_property
     def implements_decls(self):
         return self._module.get_children(vy_ast.ImplementsDecl)
 
     @cached_property
+    def implemented_interfaces(self):
+        ret = [node._metadata["interface_type"] for node in self.implements_decls]
+
+        # a module implicitly implements module.__interface__.
+        ret.append(self.interface)
+
+        return ret
+
+    @cached_property
     def interfaces(self) -> dict[str, InterfaceT]:
         ret = {}
         for i in self.interface_defs:
             assert i.name not in ret  # precondition
             ret[i.name] = i._metadata["interface_type"]
 
         for i in self.import_stmts:
```

### Comparing `vyper-0.4.0rc1/vyper/semantics/types/primitives.py` & `vyper-0.4.0rc2/vyper/semantics/types/primitives.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/semantics/types/subscriptable.py` & `vyper-0.4.0rc2/vyper/semantics/types/subscriptable.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,16 @@
         """
         return self.length
 
     def validate_index_type(self, node):
         # TODO break this cycle
         from vyper.semantics.analysis.utils import validate_expected_type
 
+        node = node.reduced()
+
         if isinstance(node, vy_ast.Int):
             if node.value < 0:
                 raise ArrayIndexException("Vyper does not support negative indexing", node)
             if node.value >= self.length:
                 raise ArrayIndexException("Index out of range", node)
 
         validate_expected_type(node, IntegerT.any())
@@ -286,17 +288,15 @@
 
         if not isinstance(node, vy_ast.Subscript):
             raise StructureException(err_msg, node)
 
         if not isinstance(node.slice, vy_ast.Tuple) or len(node.slice.elements) != 2:
             raise StructureException(err_msg, node.slice)
 
-        length_node = node.slice.elements[1]
-        if length_node.has_folded_value:
-            length_node = length_node.get_folded_value()
+        length_node = node.slice.elements[1].reduced()
 
         if not isinstance(length_node, vy_ast.Int):
             raise StructureException(err_msg, length_node)
 
         length = length_node.value
 
         value_node = node.slice.elements[0]
@@ -363,22 +363,25 @@
         return {"name": name, "type": "tuple", "components": components}
 
     @property
     def size_in_bytes(self):
         return sum(i.size_in_bytes for i in self.member_types)
 
     def validate_index_type(self, node):
+        node = node.reduced()
+
         if not isinstance(node, vy_ast.Int):
             raise InvalidType("Tuple indexes must be literals", node)
         if node.value < 0:
             raise ArrayIndexException("Vyper does not support negative indexing", node)
         if node.value >= self.length:
             raise ArrayIndexException("Index out of range", node)
 
     def get_subscripted_type(self, node):
+        node = node.reduced()
         return self.member_types[node.value]
 
     def compare_type(self, other):
         if not isinstance(self, type(other)):
             return False
         if self.length != other.length:
             return False
```

### Comparing `vyper-0.4.0rc1/vyper/semantics/types/user.py` & `vyper-0.4.0rc2/vyper/semantics/types/user.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/semantics/types/utils.py` & `vyper-0.4.0rc2/vyper/semantics/types/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,16 +191,15 @@
         Literal integer value.
         In the future, will return `None` if the subscript is an Ellipsis
     """
     # this is imported to improve error messages
     # TODO: revisit this!
     from vyper.semantics.analysis.utils import get_possible_types_from_node
 
-    if node.has_folded_value:
-        node = node.get_folded_value()
+    node = node.reduced()
 
     if not isinstance(node, vy_ast.Int):
         # even though the subscript is an invalid type, first check if it's a valid _something_
         # this gives a more accurate error in case of e.g. a typo in a constant variable name
         try:
             get_possible_types_from_node(node)
         except StructureException:
```

### Comparing `vyper-0.4.0rc1/vyper/utils.py` & `vyper-0.4.0rc2/vyper/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/venom/README.md` & `vyper-0.4.0rc2/vyper/venom/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/venom/__init__.py` & `vyper-0.4.0rc2/vyper/venom/__init__.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/venom/analysis.py` & `vyper-0.4.0rc2/vyper/venom/analysis.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/venom/basicblock.py` & `vyper-0.4.0rc2/vyper/venom/basicblock.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/venom/bb_optimizer.py` & `vyper-0.4.0rc2/vyper/venom/bb_optimizer.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/venom/dominators.py` & `vyper-0.4.0rc2/vyper/venom/dominators.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/venom/function.py` & `vyper-0.4.0rc2/vyper/venom/function.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/venom/ir_node_to_venom.py` & `vyper-0.4.0rc2/vyper/venom/ir_node_to_venom.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/venom/passes/base_pass.py` & `vyper-0.4.0rc2/vyper/venom/passes/base_pass.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/venom/passes/dft.py` & `vyper-0.4.0rc2/vyper/venom/passes/dft.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/venom/passes/make_ssa.py` & `vyper-0.4.0rc2/vyper/venom/passes/make_ssa.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/venom/passes/normalization.py` & `vyper-0.4.0rc2/vyper/venom/passes/normalization.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/venom/passes/simplify_cfg.py` & `vyper-0.4.0rc2/vyper/venom/passes/simplify_cfg.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/venom/passes/stack_reorder.py` & `vyper-0.4.0rc2/vyper/venom/passes/stack_reorder.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/venom/stack_model.py` & `vyper-0.4.0rc2/vyper/venom/stack_model.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper/venom/venom_to_assembly.py` & `vyper-0.4.0rc2/vyper/venom/venom_to_assembly.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc1/vyper.egg-info/PKG-INFO` & `vyper-0.4.0rc2/vyper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vyper
-Version: 0.4.0rc1
+Version: 0.4.0rc2
 Summary: Vyper: the Pythonic Programming Language for the EVM
 Home-page: https://github.com/vyperlang/vyper
 Author: Vyper Team
 Author-email: 
 License: Apache License 2.0
 Keywords: ethereum evm smart contract language
 Classifier: Intended Audience :: Developers
```

### Comparing `vyper-0.4.0rc1/vyper.egg-info/SOURCES.txt` & `vyper-0.4.0rc2/vyper.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -173,14 +173,15 @@
 tests/functional/codegen/modules/__init__.py
 tests/functional/codegen/modules/test_events.py
 tests/functional/codegen/modules/test_exports.py
 tests/functional/codegen/modules/test_flag_imports.py
 tests/functional/codegen/modules/test_interface_imports.py
 tests/functional/codegen/modules/test_module_constants.py
 tests/functional/codegen/modules/test_module_variables.py
+tests/functional/codegen/modules/test_nonreentrant.py
 tests/functional/codegen/modules/test_stateless_functions.py
 tests/functional/codegen/storage_variables/test_getters.py
 tests/functional/codegen/storage_variables/test_setters.py
 tests/functional/codegen/storage_variables/test_storage_variable.py
 tests/functional/codegen/types/test_array_indexing.py
 tests/functional/codegen/types/test_bytes.py
 tests/functional/codegen/types/test_bytes_literal.py
@@ -294,14 +295,15 @@
 tests/functional/syntax/exceptions/test_structure_exception.py
 tests/functional/syntax/exceptions/test_syntax_exception.py
 tests/functional/syntax/exceptions/test_type_mismatch_exception.py
 tests/functional/syntax/exceptions/test_undeclared_definition.py
 tests/functional/syntax/exceptions/test_variable_declaration_exception.py
 tests/functional/syntax/exceptions/test_vyper_exception_pos.py
 tests/functional/syntax/modules/__init__.py
+tests/functional/syntax/modules/helpers.py
 tests/functional/syntax/modules/test_deploy_visibility.py
 tests/functional/syntax/modules/test_exports.py
 tests/functional/syntax/modules/test_implements.py
 tests/functional/syntax/modules/test_initializers.py
 tests/functional/syntax/names/test_event_names.py
 tests/functional/syntax/names/test_function_names.py
 tests/functional/syntax/names/test_variable_names.py
```

### Comparing `vyper-0.4.0rc1/vyper.egg-info/requires.txt` & `vyper-0.4.0rc2/vyper.egg-info/requires.txt`

 * *Files identical despite different names*

