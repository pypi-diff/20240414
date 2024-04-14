# Comparing `tmp/lightning-2.3.0.dev20240407.tar.gz` & `tmp/lightning-2.3.0.dev20240414.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-2.3.0.dev20240407.tar", last modified: Sun Apr  7 00:20:54 2024, max compression
+gzip compressed data, was "lightning-2.3.0.dev20240414.tar", last modified: Sun Apr 14 00:21:35 2024, max compression
```

## Comparing `lightning-2.3.0.dev20240407.tar` & `lightning-2.3.0.dev20240414.tar`

### file list

```diff
@@ -1,681 +1,681 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.256882 lightning-2.3.0.dev20240407/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.164881 lightning-2.3.0.dev20240407/.actions/
--rw-r--r--   0 runner    (1001) docker     (127)    21745 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/.actions/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    24254 2024-04-07 00:20:54.256882 lightning-2.3.0.dev20240407/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22984 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.164881 lightning-2.3.0.dev20240407/requirements/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.164881 lightning-2.3.0.dev20240407/requirements/app/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/requirements/app/app.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/requirements/app/cloud.txt
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/requirements/app/components.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/requirements/app/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/requirements/app/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/requirements/app/ui.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-07 00:20:53.000000 lightning-2.3.0.dev20240407/requirements/base.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.164881 lightning-2.3.0.dev20240407/requirements/fabric/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/requirements/fabric/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/requirements/fabric/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/requirements/fabric/examples.txt
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/requirements/fabric/strategies.txt
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/requirements/fabric/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.164881 lightning-2.3.0.dev20240407/requirements/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/requirements/pytorch/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/requirements/pytorch/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/requirements/pytorch/examples.txt
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/requirements/pytorch/extra.txt
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/requirements/pytorch/strategies.txt
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/requirements/pytorch/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 00:20:54.256882 lightning-2.3.0.dev20240407/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     7935 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.164881 lightning-2.3.0.dev20240407/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.168881 lightning-2.3.0.dev20240407/src/lightning/
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-07 00:20:53.000000 lightning-2.3.0.dev20240407/src/lightning/1714ed7a47b2b85f2b1eebdd05b5f1cc91bf167a3421e0ef
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.168881 lightning-2.3.0.dev20240407/src/lightning/app/
--rw-r--r--   0 runner    (1001) docker     (127)    37365 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.168881 lightning-2.3.0.dev20240407/src/lightning/app/api/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/api/http_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/api/request_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.172881 lightning-2.3.0.dev20240407/src/lightning/app/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.172881 lightning-2.3.0.dev20240407/src/lightning/app/cli/app-template/
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/app-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/app-template/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/app-template/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/app-template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.172881 lightning-2.3.0.dev20240407/src/lightning/app/cli/app-template/placeholdername/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/app-template/placeholdername/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.152881 lightning-2.3.0.dev20240407/src/lightning/app/cli/app-template/placeholdername/components/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.172881 lightning-2.3.0.dev20240407/src/lightning/app/cli/app-template/placeholdername/components/component_a/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/app-template/placeholdername/components/component_a/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/app-template/placeholdername/components/component_a/component_a.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.172881 lightning-2.3.0.dev20240407/src/lightning/app/cli/app-template/placeholdername/components/component_b/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/app-template/placeholdername/components/component_b/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/app-template/placeholdername/components/component_b/component_a.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/app-template/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/app-template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.172881 lightning-2.3.0.dev20240407/src/lightning/app/cli/app-template/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/app-template/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/app-template/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/app-template/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/app-template/tests/test_placeholdername_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/cmd_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/cmd_init.py
--rw-r--r--   0 runner    (1001) docker     (127)    21517 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/cmd_install.py
--rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/cmd_pl_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/cmd_react_ui_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.172881 lightning-2.3.0.dev20240407/src/lightning/app/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/commands/app_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/commands/cd.py
--rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/commands/cp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/commands/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/commands/ls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/commands/pwd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/commands/rm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.176881 lightning-2.3.0.dev20240407/src/lightning/app/cli/component-template/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.152881 lightning-2.3.0.dev20240407/src/lightning/app/cli/component-template/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.176881 lightning-2.3.0.dev20240407/src/lightning/app/cli/component-template/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/component-template/.github/workflows/ci-testing.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/component-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/component-template/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/component-template/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/component-template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.176881 lightning-2.3.0.dev20240407/src/lightning/app/cli/component-template/placeholdername/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/component-template/placeholdername/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/component-template/placeholdername/component.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/component-template/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/component-template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.176881 lightning-2.3.0.dev20240407/src/lightning/app/cli/component-template/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/component-template/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/component-template/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/component-template/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/component-template/tests/test_placeholdername_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.176881 lightning-2.3.0.dev20240407/src/lightning/app/cli/connect/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14428 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/connect/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/connect/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    12669 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/lightning_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/lightning_cli_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/lightning_cli_launch.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/lightning_cli_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.176881 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/.lightningignore
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.176881 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13037 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/core/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.176881 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/core/components/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/core/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.176881 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/core/components/logger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/core/components/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/core/components/logger/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/core/components/logger/weights_and_biases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.180881 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/core/components/script_runner/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/core/components/script_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/core/components/script_runner/script_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/core/state.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.180881 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.180881 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/tests/core/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/tests/test_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.180881 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/craco.config.js
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.180881 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/public/
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/public/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/public/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/public/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/public/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.180881 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/App.tsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.184882 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/components/
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/components/Launcher.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/components/ProgressBar.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/components/Timer.tsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.184882 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/hooks/useLightningState.ts
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/index.css
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/index.tsx
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/lightning-colors.ts
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/react-app-env.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/reportWebVitals.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.184882 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/types/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/types/lightning.ts
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.184882 lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/example_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.184882 lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/ui/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.184882 lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/ui/src/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/ui/src/App.css
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/ui/src/App.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/ui/src/favicon.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.184882 lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/ui/src/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/ui/src/hooks/useLightningState.ts
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/ui/src/index.css
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/ui/src/main.tsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.184882 lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/ui/src/types/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/ui/src/types/lightning.ts
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/ui/src/vite-env.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/ui/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/ui/tsconfig.node.json
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/ui/vite.config.ts
--rw-r--r--   0 runner    (1001) docker     (127)    62319 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/ui/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.184882 lightning-2.3.0.dev20240407/src/lightning/app/components/
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.188881 lightning-2.3.0.dev20240407/src/lightning/app/components/database/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/components/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/components/database/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/components/database/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/components/database/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.188881 lightning-2.3.0.dev20240407/src/lightning/app/components/multi_node/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/components/multi_node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/components/multi_node/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/components/multi_node/fabric.py
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/components/multi_node/pytorch_spawn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/components/multi_node/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.188881 lightning-2.3.0.dev20240407/src/lightning/app/components/python/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/components/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/components/python/popen.py
--rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/components/python/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.188881 lightning-2.3.0.dev20240407/src/lightning/app/components/serve/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/components/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30437 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/components/serve/auto_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)    20105 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/components/serve/catimage.png
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/components/serve/cold_start_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/components/serve/gradio_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    11227 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/components/serve/python_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/components/serve/serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/components/serve/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.188881 lightning-2.3.0.dev20240407/src/lightning/app/components/serve/types/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/components/serve/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/components/serve/types/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/components/serve/types/type.py
--rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/components/training.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.192882 lightning-2.3.0.dev20240407/src/lightning/app/core/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18656 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/core/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    29931 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/core/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    33041 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/core/flow.py
--rw-r--r--   0 runner    (1001) docker     (127)    21814 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/core/queues.py
--rw-r--r--   0 runner    (1001) docker     (127)    31227 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/core/work.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.192882 lightning-2.3.0.dev20240407/src/lightning/app/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/frontend/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.192882 lightning-2.3.0.dev20240407/src/lightning/app/frontend/just_py/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/frontend/just_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/frontend/just_py/just_py.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/frontend/just_py/just_py_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.192882 lightning-2.3.0.dev20240407/src/lightning/app/frontend/panel/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/frontend/panel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/frontend/panel/app_state_comm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/frontend/panel/app_state_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/frontend/panel/panel_frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/frontend/panel/panel_serve_render_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/frontend/stream_lit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/frontend/streamlit_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/frontend/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/frontend/web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.192882 lightning-2.3.0.dev20240407/src/lightning/app/launcher/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/launcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15316 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/launcher/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    21529 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/launcher/lightning_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/launcher/lightning_hybrid_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.192882 lightning-2.3.0.dev20240407/src/lightning/app/pdb/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/pdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/pdb/pdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.192882 lightning-2.3.0.dev20240407/src/lightning/app/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.196882 lightning-2.3.0.dev20240407/src/lightning/app/runners/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/runners/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.196882 lightning-2.3.0.dev20240407/src/lightning/app/runners/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/runners/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/runners/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/runners/backends/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/runners/backends/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/runners/backends/mp_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    47781 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/runners/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/runners/multiprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/runners/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/runners/runtime_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.196882 lightning-2.3.0.dev20240407/src/lightning/app/source_code/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/source_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/source_code/copytree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/source_code/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/source_code/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/source_code/tar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/source_code/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.196882 lightning-2.3.0.dev20240407/src/lightning/app/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/storage/copier.py
--rw-r--r--   0 runner    (1001) docker     (127)    13120 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/storage/drive.py
--rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/storage/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/storage/mount.py
--rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/storage/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)    18320 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/storage/path.py
--rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/storage/payload.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/storage/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.200882 lightning-2.3.0.dev20240407/src/lightning/app/structures/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6224 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/structures/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/structures/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.200882 lightning-2.3.0.dev20240407/src/lightning/app/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/testing/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/testing/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    19345 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/testing/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.200882 lightning-2.3.0.dev20240407/src/lightning/app/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240407/src/lightning/app/ui/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)      747 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240407/src/lightning/app/ui/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.200882 lightning-2.3.0.dev20240407/src/lightning/app/ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.200882 lightning-2.3.0.dev20240407/src/lightning/app/ui/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240407/src/lightning/app/ui/static/css/main.fb7060be.css
--rw-r--r--   0 runner    (1001) docker     (127)      847 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240407/src/lightning/app/ui/static/css/main.fb7060be.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240407/src/lightning/app/ui/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.200882 lightning-2.3.0.dev20240407/src/lightning/app/ui/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240407/src/lightning/app/ui/static/js/787.418637a8.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10281 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240407/src/lightning/app/ui/static/js/787.418637a8.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   503634 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240407/src/lightning/app/ui/static/js/main.c1f02aeb.js
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240407/src/lightning/app/ui/static/js/main.c1f02aeb.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)  2068175 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240407/src/lightning/app/ui/static/js/main.c1f02aeb.js.map
--rw-r--r--   0 runner    (1001) docker     (127)      571 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240407/src/lightning/app/ui/static/lightningState.js
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240407/src/lightning/app/ui/static/manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.204882 lightning-2.3.0.dev20240407/src/lightning/app/ui/static/media/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240407/src/lightning/app/ui/static/media/error.11892047d0183a4723b91dc0fb98cb95.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7931 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240407/src/lightning/app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg
--rw-r--r--   0 runner    (1001) docker     (127)      390 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240407/src/lightning/app/ui/static/media/success.5edae4c5b171e2c1c5a3c54273c47ba8.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240407/src/lightning/app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240407/src/lightning/app/ui/static/robots.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240407/src/lightning/app/ui/version.info
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.212882 lightning-2.3.0.dev20240407/src/lightning/app/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/app_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    19038 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/app_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/app_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/app_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    13146 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/cli_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/clusters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.212882 lightning-2.3.0.dev20240407/src/lightning/app/utilities/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11195 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/dependency_caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)    11489 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    10724 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/load_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/log_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/logs_socket_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    60256 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/name_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7732 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/openapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.212882 lightning-2.3.0.dev20240407/src/lightning/app/utilities/packaging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/packaging/app_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/packaging/build_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/packaging/cloud_compute.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/packaging/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/packaging/lightning_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/packaging/tarfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/port.py
--rw-r--r--   0 runner    (1001) docker     (127)    30254 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/proxies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/safe_pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/tracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/app/utilities/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.212882 lightning-2.3.0.dev20240407/src/lightning/data/
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.216882 lightning-2.3.0.dev20240407/src/lightning/fabric/
--rw-r--r--   0 runner    (1001) docker     (127)    32605 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.216882 lightning-2.3.0.dev20240407/src/lightning/fabric/_graveyard/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/_graveyard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/_graveyard/tpu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.216882 lightning-2.3.0.dev20240407/src/lightning/fabric/accelerators/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/accelerators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/accelerators/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/accelerators/cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)    14380 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/accelerators/cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/accelerators/mps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/accelerators/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/accelerators/xla.py
--rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    27849 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    51595 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/fabric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.216882 lightning-2.3.0.dev20240407/src/lightning/fabric/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/loggers/csv_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    13115 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.216882 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.216882 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/collectives/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/collectives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/collectives/collective.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/collectives/single_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/collectives/torch_collective.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.220882 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/environments/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/environments/cluster_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/environments/kubeflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/environments/lightning.py
--rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/environments/lsf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/environments/mpi.py
--rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/environments/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/environments/torchelastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/environments/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.220882 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/io/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/io/checkpoint_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/io/torch_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/io/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.220882 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/precision/
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/precision/amp.py
--rw-r--r--   0 runner    (1001) docker     (127)    20991 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/precision/bitsandbytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/precision/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/precision/double.py
--rw-r--r--   0 runner    (1001) docker     (127)     7046 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/precision/fsdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/precision/half.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/precision/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/precision/transformer_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/precision/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/precision/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.224882 lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/ddp.py
--rw-r--r--   0 runner    (1001) docker     (127)    41437 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/dp.py
--rw-r--r--   0 runner    (1001) docker     (127)    44312 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/fsdp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.224882 lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/launchers/
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/launchers/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/launchers/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/launchers/subprocess_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/launchers/xla.py
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/single_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/single_xla.py
--rw-r--r--   0 runner    (1001) docker     (127)    18461 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11428 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/xla.py
--rw-r--r--   0 runner    (1001) docker     (127)    30515 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/xla_fsdp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.228882 lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/apply_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/cloud_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/consolidate_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    23129 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/device_dtype_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7343 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/device_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    16775 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/rank_zero.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/seed.py
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/spike.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.228882 lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/testing/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/testing/_runif.py
--rw-r--r--   0 runner    (1001) docker     (127)    27517 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/throughput.py
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    17047 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/fabric/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.228882 lightning-2.3.0.dev20240407/src/lightning/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)   456493 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.228882 lightning-2.3.0.dev20240407/src/lightning/pytorch/_graveyard/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/_graveyard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/_graveyard/_torchmetrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/_graveyard/hpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/_graveyard/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/_graveyard/tpu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.232882 lightning-2.3.0.dev20240407/src/lightning/pytorch/accelerators/
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/accelerators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/accelerators/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/accelerators/cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/accelerators/cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/accelerators/mps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/accelerators/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.236882 lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/batch_size_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11022 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/device_stats_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)    19095 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/finetuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/gradient_accumulation_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/lambda_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15095 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/lr_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    38563 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/model_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/on_exception_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/prediction_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.236882 lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/progress/
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/progress/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)    25511 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/progress/rich_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)    16923 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/progress/tqdm_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/pruning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/rich_model_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/spike.py
--rw-r--r--   0 runner    (1001) docker     (127)    17922 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/stochastic_weight_avg.py
--rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/throughput_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8313 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    38278 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.236882 lightning-2.3.0.dev20240407/src/lightning/pytorch/core/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10827 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/core/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)    26968 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/core/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.236882 lightning-2.3.0.dev20240407/src/lightning/pytorch/core/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/core/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6959 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/core/mixins/hparams_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    70944 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/core/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    18344 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/core/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14588 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/core/saving.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.236882 lightning-2.3.0.dev20240407/src/lightning/pytorch/demos/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/demos/boring_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9243 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/demos/mnist_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7132 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/demos/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.240882 lightning-2.3.0.dev20240407/src/lightning/pytorch/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15743 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/loggers/comet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/loggers/csv_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    14939 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/loggers/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    23271 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/loggers/neptune.py
--rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/loggers/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/loggers/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    24843 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/loggers/wandb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.240882 lightning-2.3.0.dev20240407/src/lightning/pytorch/loops/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/loops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25464 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/loops/evaluation_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/loops/fetchers.py
--rw-r--r--   0 runner    (1001) docker     (127)    19179 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/loops/fit_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/loops/loop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.240882 lightning-2.3.0.dev20240407/src/lightning/pytorch/loops/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/loops/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12681 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/loops/optimization/automatic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/loops/optimization/closure.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/loops/optimization/manual.py
--rw-r--r--   0 runner    (1001) docker     (127)    18682 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/loops/prediction_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/loops/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)    23209 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/loops/training_epoch_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     8589 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/loops/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.240882 lightning-2.3.0.dev20240407/src/lightning/pytorch/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/overrides/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/overrides/distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.240882 lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.240882 lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/environments/
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/environments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.244882 lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/io/
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/io/async_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/io/checkpoint_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/io/torch_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/io/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/io/xla_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/layer_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.244882 lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/precision/
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/precision/amp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/precision/bitsandbytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/precision/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/precision/double.py
--rw-r--r--   0 runner    (1001) docker     (127)     8267 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/precision/fsdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/precision/half.py
--rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/precision/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/precision/transformer_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/precision/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.244882 lightning-2.3.0.dev20240407/src/lightning/pytorch/profilers/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/profilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/profilers/advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/profilers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/profilers/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    23778 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/profilers/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/profilers/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/profilers/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.244882 lightning-2.3.0.dev20240407/src/lightning/pytorch/serve/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/serve/servable_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/serve/servable_module_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.248882 lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19061 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/ddp.py
--rw-r--r--   0 runner    (1001) docker     (127)    40964 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)    30989 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/fsdp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.248882 lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/launchers/
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/launchers/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    14256 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/launchers/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/launchers/subprocess_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/launchers/xla.py
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/single_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/single_xla.py
--rw-r--r--   0 runner    (1001) docker     (127)    25739 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13224 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.248882 lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/call.py
--rw-r--r--   0 runner    (1001) docker     (127)     8589 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/configuration_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.248882 lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31261 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/connectors/accelerator_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    10663 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/connectors/callback_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    24486 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/connectors/checkpoint_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    22488 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/connectors/data_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.252882 lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/connectors/logger_connector/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/connectors/logger_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/connectors/logger_connector/fx_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10305 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/connectors/logger_connector/logger_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    20934 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/connectors/logger_connector/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/connectors/signal_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/states.py
--rw-r--r--   0 runner    (1001) docker     (127)    73372 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.252882 lightning-2.3.0.dev20240407/src/lightning/pytorch/tuner/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/tuner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12868 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/tuner/batch_size_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)    19672 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/tuner/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11471 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/tuner/tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.256882 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/_pytree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    16339 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/combined_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/consolidate_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    16604 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/grads.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.256882 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/migration/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/migration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14537 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/migration/migration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/migration/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/model_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.256882 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/model_summary/
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/model_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18287 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/model_summary/model_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/model_summary/model_summary_deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/parameter_tying.py
--rw-r--r--   0 runner    (1001) docker     (127)    12083 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/rank_zero.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/seed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/signature_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.256882 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/testing/_runif.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/upgrade_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.256882 lightning-2.3.0.dev20240407/src/lightning/store/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/store/store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-07 00:20:34.000000 lightning-2.3.0.dev20240407/src/lightning/store/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-07 00:20:37.000000 lightning-2.3.0.dev20240407/src/lightning/version.info
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:54.168881 lightning-2.3.0.dev20240407/src/lightning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24254 2024-04-07 00:20:54.000000 lightning-2.3.0.dev20240407/src/lightning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26370 2024-04-07 00:20:54.000000 lightning-2.3.0.dev20240407/src/lightning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 00:20:54.000000 lightning-2.3.0.dev20240407/src/lightning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-07 00:20:54.000000 lightning-2.3.0.dev20240407/src/lightning.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 00:20:54.000000 lightning-2.3.0.dev20240407/src/lightning.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-07 00:20:54.000000 lightning-2.3.0.dev20240407/src/lightning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-07 00:20:54.000000 lightning-2.3.0.dev20240407/src/lightning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-07 00:20:37.000000 lightning-2.3.0.dev20240407/src/version.info
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.806678 lightning-2.3.0.dev20240414/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.710678 lightning-2.3.0.dev20240414/.actions/
+-rw-r--r--   0 runner    (1001) docker     (127)    21745 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/.actions/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    24254 2024-04-14 00:21:35.806678 lightning-2.3.0.dev20240414/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22984 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.710678 lightning-2.3.0.dev20240414/requirements/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.710678 lightning-2.3.0.dev20240414/requirements/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/requirements/app/app.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/requirements/app/cloud.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/requirements/app/components.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/requirements/app/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/requirements/app/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/requirements/app/ui.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-14 00:21:34.000000 lightning-2.3.0.dev20240414/requirements/base.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.710678 lightning-2.3.0.dev20240414/requirements/fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/requirements/fabric/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/requirements/fabric/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/requirements/fabric/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/requirements/fabric/strategies.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/requirements/fabric/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.714678 lightning-2.3.0.dev20240414/requirements/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/requirements/pytorch/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/requirements/pytorch/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/requirements/pytorch/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/requirements/pytorch/extra.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/requirements/pytorch/strategies.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/requirements/pytorch/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 00:21:35.806678 lightning-2.3.0.dev20240414/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7935 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.714678 lightning-2.3.0.dev20240414/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.714678 lightning-2.3.0.dev20240414/src/lightning/
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.714678 lightning-2.3.0.dev20240414/src/lightning/app/
+-rw-r--r--   0 runner    (1001) docker     (127)    37365 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.714678 lightning-2.3.0.dev20240414/src/lightning/app/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/api/http_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/api/request_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.718678 lightning-2.3.0.dev20240414/src/lightning/app/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.718678 lightning-2.3.0.dev20240414/src/lightning/app/cli/app-template/
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/app-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/app-template/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/app-template/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/app-template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.718678 lightning-2.3.0.dev20240414/src/lightning/app/cli/app-template/placeholdername/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/app-template/placeholdername/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.698678 lightning-2.3.0.dev20240414/src/lightning/app/cli/app-template/placeholdername/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.718678 lightning-2.3.0.dev20240414/src/lightning/app/cli/app-template/placeholdername/components/component_a/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/app-template/placeholdername/components/component_a/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/app-template/placeholdername/components/component_a/component_a.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.718678 lightning-2.3.0.dev20240414/src/lightning/app/cli/app-template/placeholdername/components/component_b/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/app-template/placeholdername/components/component_b/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/app-template/placeholdername/components/component_b/component_a.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/app-template/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/app-template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.718678 lightning-2.3.0.dev20240414/src/lightning/app/cli/app-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/app-template/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/app-template/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/app-template/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/app-template/tests/test_placeholdername_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/cmd_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/cmd_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21517 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/cmd_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/cmd_pl_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/cmd_react_ui_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.722678 lightning-2.3.0.dev20240414/src/lightning/app/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/commands/app_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/commands/cd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/commands/cp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/commands/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/commands/ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/commands/pwd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/commands/rm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.722678 lightning-2.3.0.dev20240414/src/lightning/app/cli/component-template/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.698678 lightning-2.3.0.dev20240414/src/lightning/app/cli/component-template/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.722678 lightning-2.3.0.dev20240414/src/lightning/app/cli/component-template/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/component-template/.github/workflows/ci-testing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/component-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/component-template/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/component-template/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/component-template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.722678 lightning-2.3.0.dev20240414/src/lightning/app/cli/component-template/placeholdername/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/component-template/placeholdername/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/component-template/placeholdername/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/component-template/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/component-template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.722678 lightning-2.3.0.dev20240414/src/lightning/app/cli/component-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/component-template/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/component-template/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/component-template/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/component-template/tests/test_placeholdername_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.722678 lightning-2.3.0.dev20240414/src/lightning/app/cli/connect/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14428 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/connect/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/connect/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12669 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/lightning_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/lightning_cli_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/lightning_cli_launch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/lightning_cli_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.726678 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/.lightningignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.726678 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13037 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/core/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.726678 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/core/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/core/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.726678 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/core/components/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/core/components/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/core/components/logger/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/core/components/logger/weights_and_biases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.726678 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/core/components/script_runner/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/core/components/script_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/core/components/script_runner/script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.726678 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.726678 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/tests/core/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.726678 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/craco.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.726678 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/public/
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/public/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/public/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/public/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.730678 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/App.tsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.730678 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/components/Launcher.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/components/ProgressBar.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/components/Timer.tsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.730678 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/hooks/useLightningState.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/index.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/lightning-colors.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/react-app-env.d.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/reportWebVitals.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.730678 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/types/lightning.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.730678 lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/example_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.730678 lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/ui/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.734678 lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/ui/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/ui/src/App.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/ui/src/App.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/ui/src/favicon.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.734678 lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/ui/src/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/ui/src/hooks/useLightningState.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/ui/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/ui/src/main.tsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.734678 lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/ui/src/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/ui/src/types/lightning.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/ui/src/vite-env.d.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/ui/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/ui/tsconfig.node.json
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/ui/vite.config.ts
+-rw-r--r--   0 runner    (1001) docker     (127)    62319 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/ui/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.734678 lightning-2.3.0.dev20240414/src/lightning/app/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.734678 lightning-2.3.0.dev20240414/src/lightning/app/components/database/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/components/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/components/database/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/components/database/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/components/database/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.734678 lightning-2.3.0.dev20240414/src/lightning/app/components/multi_node/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/components/multi_node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/components/multi_node/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/components/multi_node/fabric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/components/multi_node/pytorch_spawn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/components/multi_node/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.734678 lightning-2.3.0.dev20240414/src/lightning/app/components/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/components/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/components/python/popen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/components/python/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.738678 lightning-2.3.0.dev20240414/src/lightning/app/components/serve/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/components/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30437 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/components/serve/auto_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20105 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/components/serve/catimage.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/components/serve/cold_start_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/components/serve/gradio_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11227 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/components/serve/python_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/components/serve/serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/components/serve/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.738678 lightning-2.3.0.dev20240414/src/lightning/app/components/serve/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/components/serve/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/components/serve/types/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/components/serve/types/type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/components/training.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.738678 lightning-2.3.0.dev20240414/src/lightning/app/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18656 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29931 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33041 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/core/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21814 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/core/queues.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31227 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/core/work.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.738678 lightning-2.3.0.dev20240414/src/lightning/app/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/frontend/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.738678 lightning-2.3.0.dev20240414/src/lightning/app/frontend/just_py/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/frontend/just_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/frontend/just_py/just_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/frontend/just_py/just_py_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.738678 lightning-2.3.0.dev20240414/src/lightning/app/frontend/panel/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/frontend/panel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/frontend/panel/app_state_comm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/frontend/panel/app_state_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/frontend/panel/panel_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/frontend/panel/panel_serve_render_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/frontend/stream_lit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/frontend/streamlit_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/frontend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/frontend/web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.742678 lightning-2.3.0.dev20240414/src/lightning/app/launcher/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/launcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15316 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/launcher/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21529 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/launcher/lightning_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/launcher/lightning_hybrid_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.742678 lightning-2.3.0.dev20240414/src/lightning/app/pdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/pdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/pdb/pdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.742678 lightning-2.3.0.dev20240414/src/lightning/app/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.742678 lightning-2.3.0.dev20240414/src/lightning/app/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/runners/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.742678 lightning-2.3.0.dev20240414/src/lightning/app/runners/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/runners/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/runners/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/runners/backends/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/runners/backends/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/runners/backends/mp_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47781 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/runners/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/runners/multiprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/runners/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/runners/runtime_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.742678 lightning-2.3.0.dev20240414/src/lightning/app/source_code/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/source_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/source_code/copytree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/source_code/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/source_code/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/source_code/tar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/source_code/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.746678 lightning-2.3.0.dev20240414/src/lightning/app/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/storage/copier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13120 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/storage/drive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/storage/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/storage/mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/storage/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18320 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/storage/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/storage/payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/storage/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.746678 lightning-2.3.0.dev20240414/src/lightning/app/structures/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6224 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/structures/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/structures/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.746678 lightning-2.3.0.dev20240414/src/lightning/app/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/testing/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/testing/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19345 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/testing/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.746678 lightning-2.3.0.dev20240414/src/lightning/app/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240414/src/lightning/app/ui/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240414/src/lightning/app/ui/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.746678 lightning-2.3.0.dev20240414/src/lightning/app/ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.746678 lightning-2.3.0.dev20240414/src/lightning/app/ui/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240414/src/lightning/app/ui/static/css/main.fb7060be.css
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240414/src/lightning/app/ui/static/css/main.fb7060be.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240414/src/lightning/app/ui/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.750678 lightning-2.3.0.dev20240414/src/lightning/app/ui/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240414/src/lightning/app/ui/static/js/787.418637a8.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10281 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240414/src/lightning/app/ui/static/js/787.418637a8.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   503634 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240414/src/lightning/app/ui/static/js/main.c1f02aeb.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240414/src/lightning/app/ui/static/js/main.c1f02aeb.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  2068175 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240414/src/lightning/app/ui/static/js/main.c1f02aeb.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240414/src/lightning/app/ui/static/lightningState.js
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240414/src/lightning/app/ui/static/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.754678 lightning-2.3.0.dev20240414/src/lightning/app/ui/static/media/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240414/src/lightning/app/ui/static/media/error.11892047d0183a4723b91dc0fb98cb95.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240414/src/lightning/app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240414/src/lightning/app/ui/static/media/success.5edae4c5b171e2c1c5a3c54273c47ba8.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240414/src/lightning/app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240414/src/lightning/app/ui/static/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-09-26 19:57:09.000000 lightning-2.3.0.dev20240414/src/lightning/app/ui/version.info
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.758678 lightning-2.3.0.dev20240414/src/lightning/app/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/app_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19038 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/app_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/app_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/app_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13146 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/cli_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/clusters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.758678 lightning-2.3.0.dev20240414/src/lightning/app/utilities/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11195 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/dependency_caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11489 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10724 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/load_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/log_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/logs_socket_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60256 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/name_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7732 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/openapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.762678 lightning-2.3.0.dev20240414/src/lightning/app/utilities/packaging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/packaging/app_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/packaging/build_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/packaging/cloud_compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/packaging/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/packaging/lightning_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/packaging/tarfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/port.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30254 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/safe_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/app/utilities/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.762678 lightning-2.3.0.dev20240414/src/lightning/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-14 00:21:35.000000 lightning-2.3.0.dev20240414/src/lightning/e4e465c6f6642e9f9fc64f431fc44401b9981f6435f96f96
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.762678 lightning-2.3.0.dev20240414/src/lightning/fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)    32758 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.762678 lightning-2.3.0.dev20240414/src/lightning/fabric/_graveyard/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/_graveyard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/_graveyard/tpu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.762678 lightning-2.3.0.dev20240414/src/lightning/fabric/accelerators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/accelerators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/accelerators/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/accelerators/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14380 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/accelerators/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/accelerators/mps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/accelerators/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/accelerators/xla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27849 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51595 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/fabric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.762678 lightning-2.3.0.dev20240414/src/lightning/fabric/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/loggers/csv_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13115 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.762678 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.766678 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/collectives/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/collectives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/collectives/collective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/collectives/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/collectives/torch_collective.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.766678 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/environments/cluster_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/environments/kubeflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/environments/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/environments/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/environments/mpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/environments/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/environments/torchelastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/environments/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.766678 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/io/checkpoint_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/io/torch_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/io/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.770678 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/precision/
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/precision/amp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20991 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/precision/bitsandbytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/precision/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/precision/double.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7046 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/precision/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/precision/half.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/precision/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/precision/transformer_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/precision/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/precision/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.770678 lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41437 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/dp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44312 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/fsdp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.770678 lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/launchers/
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/launchers/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/launchers/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/launchers/subprocess_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/launchers/xla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/single_xla.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18461 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11428 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/xla.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30515 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/xla_fsdp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.774678 lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/apply_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/cloud_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/consolidate_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23129 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/device_dtype_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7343 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/device_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16775 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/rank_zero.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/spike.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.774678 lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/testing/_runif.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27517 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/throughput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17047 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/fabric/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.778678 lightning-2.3.0.dev20240414/src/lightning/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)   456493 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.778678 lightning-2.3.0.dev20240414/src/lightning/pytorch/_graveyard/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/_graveyard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/_graveyard/_torchmetrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/_graveyard/hpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/_graveyard/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/_graveyard/tpu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.778678 lightning-2.3.0.dev20240414/src/lightning/pytorch/accelerators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/accelerators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/accelerators/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/accelerators/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/accelerators/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/accelerators/mps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/accelerators/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.782678 lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/batch_size_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11022 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/device_stats_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19095 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/finetuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/gradient_accumulation_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/lambda_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15095 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/lr_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38563 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/model_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/on_exception_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/prediction_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.782678 lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/progress/
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/progress/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25511 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/progress/rich_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16923 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/progress/tqdm_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/pruning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/rich_model_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/spike.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17922 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/stochastic_weight_avg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/throughput_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8313 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38278 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.782678 lightning-2.3.0.dev20240414/src/lightning/pytorch/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10827 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/core/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26968 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/core/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.782678 lightning-2.3.0.dev20240414/src/lightning/pytorch/core/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/core/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6959 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/core/mixins/hparams_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70944 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/core/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18344 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/core/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14588 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/core/saving.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.786678 lightning-2.3.0.dev20240414/src/lightning/pytorch/demos/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/demos/boring_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9243 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/demos/mnist_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7132 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/demos/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.786678 lightning-2.3.0.dev20240414/src/lightning/pytorch/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15743 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/loggers/comet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/loggers/csv_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14939 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/loggers/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23271 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/loggers/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/loggers/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/loggers/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24843 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/loggers/wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.786678 lightning-2.3.0.dev20240414/src/lightning/pytorch/loops/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/loops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25464 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/loops/evaluation_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/loops/fetchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19179 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/loops/fit_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/loops/loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.786678 lightning-2.3.0.dev20240414/src/lightning/pytorch/loops/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/loops/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12681 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/loops/optimization/automatic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/loops/optimization/closure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/loops/optimization/manual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18682 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/loops/prediction_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/loops/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23209 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/loops/training_epoch_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8589 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/loops/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.790678 lightning-2.3.0.dev20240414/src/lightning/pytorch/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/overrides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/overrides/distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.790678 lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.790678 lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/environments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.790678 lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/io/async_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/io/checkpoint_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/io/torch_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/io/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/io/xla_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/layer_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.790678 lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/precision/
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/precision/amp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/precision/bitsandbytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/precision/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/precision/double.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8267 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/precision/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/precision/half.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/precision/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/precision/transformer_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/precision/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.794678 lightning-2.3.0.dev20240414/src/lightning/pytorch/profilers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/profilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/profilers/advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/profilers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/profilers/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23778 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/profilers/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/profilers/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/profilers/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.794678 lightning-2.3.0.dev20240414/src/lightning/pytorch/serve/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/serve/servable_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/serve/servable_module_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.794678 lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19061 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40964 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30989 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/fsdp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.794678 lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/launchers/
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/launchers/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14256 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/launchers/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/launchers/subprocess_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/launchers/xla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/single_xla.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25739 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13224 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.798678 lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8589 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/configuration_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.798678 lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31261 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/connectors/accelerator_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10663 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/connectors/callback_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24486 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/connectors/checkpoint_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22488 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/connectors/data_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.798678 lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/connectors/logger_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/connectors/logger_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/connectors/logger_connector/fx_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10305 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/connectors/logger_connector/logger_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20934 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/connectors/logger_connector/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/connectors/signal_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73372 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.798678 lightning-2.3.0.dev20240414/src/lightning/pytorch/tuner/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/tuner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12868 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/tuner/batch_size_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19672 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/tuner/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11471 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/tuner/tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.802678 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/_pytree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16339 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/combined_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/consolidate_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16604 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/grads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.802678 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/migration/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/migration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14537 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/migration/migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/migration/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/model_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.802678 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/model_summary/
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/model_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18287 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/model_summary/model_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/model_summary/model_summary_deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/parameter_tying.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12083 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/rank_zero.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/signature_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.802678 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/testing/_runif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/upgrade_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.802678 lightning-2.3.0.dev20240414/src/lightning/store/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/store/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-14 00:21:18.000000 lightning-2.3.0.dev20240414/src/lightning/store/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-14 00:21:21.000000 lightning-2.3.0.dev20240414/src/lightning/version.info
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:21:35.714678 lightning-2.3.0.dev20240414/src/lightning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24254 2024-04-14 00:21:35.000000 lightning-2.3.0.dev20240414/src/lightning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26370 2024-04-14 00:21:35.000000 lightning-2.3.0.dev20240414/src/lightning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 00:21:35.000000 lightning-2.3.0.dev20240414/src/lightning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-14 00:21:35.000000 lightning-2.3.0.dev20240414/src/lightning.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 00:21:35.000000 lightning-2.3.0.dev20240414/src/lightning.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-14 00:21:35.000000 lightning-2.3.0.dev20240414/src/lightning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-14 00:21:35.000000 lightning-2.3.0.dev20240414/src/lightning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-14 00:21:21.000000 lightning-2.3.0.dev20240414/src/version.info
```

### Comparing `lightning-2.3.0.dev20240407/.actions/assistant.py` & `lightning-2.3.0.dev20240414/.actions/assistant.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/CITATION.cff` & `lightning-2.3.0.dev20240414/CITATION.cff`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/LICENSE` & `lightning-2.3.0.dev20240414/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/PKG-INFO` & `lightning-2.3.0.dev20240414/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning
-Version: 2.3.0.dev20240407
+Version: 2.3.0.dev20240414
 Summary: The Deep Learning framework to train, deploy, and ship AI products Lightning fast.
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
@@ -74,15 +74,15 @@
 ______________________________________________________________________
 
 <p align="center">
   <a href="https://lightning.ai/">Lightning.ai</a> •
   <a href="https://lightning.ai/docs/pytorch/stable/">PyTorch Lightning</a> •
   <a href="https://lightning.ai/docs/fabric/stable/">Fabric</a> •
   <a href="https://lightning.ai/docs/app/stable/">Lightning Apps</a> •
-  <a href="https://pytorch-lightning.readthedocs.io/en/2.3.0.dev20240407">Docs</a> •
+  <a href="https://pytorch-lightning.readthedocs.io/en/2.3.0.dev20240414">Docs</a> •
   <a href="#community">Community</a> •
   <a href="https://lightning.ai/docs/pytorch/stable/generated/CONTRIBUTING.html">Contribute</a> •
 </p>
 
 <!-- DO NOT ADD CONDA DOWNLOADS... README CHANGES MUST BE APPROVED BY EDEN OR WILL -->
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytorch-lightning)](https://pypi.org/project/pytorch-lightning/)
@@ -619,15 +619,15 @@
 <details>
   <summary>Current build statuses</summary>
 
 <center>
 
 |       System / PyTorch ver.        | 1.13                                                                                                                                                                                                                            | 2.0                                                                                                                                                                                                                             |                                                                                                               2.1                                                                                                               |
 | :--------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
-|        Linux py3.9 \[GPUs\]        |  |  | [![Build Status](https://dev.azure.com/Lightning-AI/lightning/_apis/build/status%2Fpytorch-lightning%20%28GPUs%29?branchName=refs%2Ftags%2F2.3.0.dev20240407)](https://dev.azure.com/Lightning-AI/lightning/_build/latest?definitionId=24&branchName=master) |
+|        Linux py3.9 \[GPUs\]        |  |  | [![Build Status](https://dev.azure.com/Lightning-AI/lightning/_apis/build/status%2Fpytorch-lightning%20%28GPUs%29?branchName=refs%2Ftags%2F2.3.0.dev20240414)](https://dev.azure.com/Lightning-AI/lightning/_build/latest?definitionId=24&branchName=master) |
 |        Linux py3.9 \[TPUs\]        |                                                                                                                                                                                                                                 |  [![Test PyTorch - TPU](https://github.com/Lightning-AI/lightning/actions/workflows/tpu-tests.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/tpu-tests.yml)     |      |
 |  Linux (multiple Python versions)  | [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                                 | [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                                 |                 [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                 |
 |   OSX (multiple Python versions)   | [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                                 | [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                                 |                 [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                 |
 | Windows (multiple Python versions) | [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                                 | [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                                 |                 [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                 |
 
 </center>
 </details>
```

### Comparing `lightning-2.3.0.dev20240407/README.md` & `lightning-2.3.0.dev20240414/README.md`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/pyproject.toml` & `lightning-2.3.0.dev20240414/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/requirements/app/app.txt` & `lightning-2.3.0.dev20240414/requirements/app/app.txt`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/requirements/fabric/strategies.txt` & `lightning-2.3.0.dev20240414/requirements/fabric/strategies.txt`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/requirements/pytorch/base.txt` & `lightning-2.3.0.dev20240414/requirements/pytorch/base.txt`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/requirements/pytorch/extra.txt` & `lightning-2.3.0.dev20240414/requirements/pytorch/extra.txt`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/requirements/pytorch/test.txt` & `lightning-2.3.0.dev20240414/requirements/pytorch/test.txt`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/setup.py` & `lightning-2.3.0.dev20240414/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/1714ed7a47b2b85f2b1eebdd05b5f1cc91bf167a3421e0ef` & `lightning-2.3.0.dev20240414/src/lightning/e4e465c6f6642e9f9fc64f431fc44401b9981f6435f96f96`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/__about__.py` & `lightning-2.3.0.dev20240414/src/lightning/__about__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/__setup__.py` & `lightning-2.3.0.dev20240414/src/lightning/__setup__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/CHANGELOG.md` & `lightning-2.3.0.dev20240414/src/lightning/app/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/app/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/api/http_methods.py` & `lightning-2.3.0.dev20240414/src/lightning/app/api/http_methods.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/api/request_types.py` & `lightning-2.3.0.dev20240414/src/lightning/app/api/request_types.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/app-template/.gitignore` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/app-template/.gitignore`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/app-template/LICENSE` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/app-template/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/app-template/README.md` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/app-template/README.md`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/app-template/tests/test_placeholdername_app.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/app-template/tests/test_placeholdername_app.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/cmd_apps.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/cmd_apps.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/cmd_init.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/cmd_init.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/cmd_install.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/cmd_install.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/cmd_pl_init.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/cmd_pl_init.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/cmd_react_ui_init.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/cmd_react_ui_init.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/commands/app_commands.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/commands/app_commands.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/commands/cd.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/commands/cd.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/commands/cp.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/commands/cp.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/commands/logs.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/commands/logs.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/commands/ls.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/commands/ls.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/commands/pwd.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/commands/pwd.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/commands/rm.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/commands/rm.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/component-template/.github/workflows/ci-testing.yml` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/component-template/.github/workflows/ci-testing.yml`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/component-template/.gitignore` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/component-template/.gitignore`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/component-template/LICENSE` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/component-template/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/component-template/README.md` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/component-template/README.md`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/connect/app.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/connect/app.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/connect/data.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/connect/data.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/core.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/core.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/lightning_cli.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/lightning_cli.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/lightning_cli_delete.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/lightning_cli_delete.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/lightning_cli_launch.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/lightning_cli_launch.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/lightning_cli_list.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/lightning_cli_list.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/app.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/app.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/core/callbacks.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/core/callbacks.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/core/components/logger/tensorboard.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/core/components/logger/tensorboard.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/core/components/logger/weights_and_biases.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/core/components/logger/weights_and_biases.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/core/components/script_runner/script_runner.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/core/components/script_runner/script_runner.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/core/state.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/core/state.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/setup.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/tests/core/test_callbacks.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/tests/core/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/.prettierrc` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/.prettierrc`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/craco.config.js` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/craco.config.js`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/package.json` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/package.json`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/public/favicon.svg` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/public/index.html` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/public/index.html`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/App.tsx` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/App.tsx`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/components/Launcher.tsx` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/components/Launcher.tsx`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/components/ProgressBar.tsx` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/components/ProgressBar.tsx`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/components/Timer.tsx` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/components/Timer.tsx`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/hooks/useLightningState.ts` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/hooks/useLightningState.ts`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/index.tsx` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/index.tsx`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/src/types/lightning.ts` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/src/types/lightning.ts`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/pl-app-template/ui/tsconfig.json` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/pl-app-template/ui/tsconfig.json`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/README.md` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/README.md`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/example_app.py` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/example_app.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/ui/package.json` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/ui/package.json`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/ui/src/App.tsx` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/ui/src/App.tsx`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/ui/src/favicon.svg` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/ui/src/favicon.svg`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/ui/src/hooks/useLightningState.ts` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/ui/src/hooks/useLightningState.ts`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/ui/src/types/lightning.ts` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/ui/src/types/lightning.ts`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/ui/tsconfig.json` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/ui/tsconfig.json`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/cli/react-ui-template/ui/yarn.lock` & `lightning-2.3.0.dev20240414/src/lightning/app/cli/react-ui-template/ui/yarn.lock`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/components/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/app/components/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/components/database/client.py` & `lightning-2.3.0.dev20240414/src/lightning/app/components/database/client.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/components/database/server.py` & `lightning-2.3.0.dev20240414/src/lightning/app/components/database/server.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/components/database/utilities.py` & `lightning-2.3.0.dev20240414/src/lightning/app/components/database/utilities.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/components/multi_node/base.py` & `lightning-2.3.0.dev20240414/src/lightning/app/components/multi_node/base.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/components/multi_node/fabric.py` & `lightning-2.3.0.dev20240414/src/lightning/app/components/multi_node/fabric.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/components/multi_node/pytorch_spawn.py` & `lightning-2.3.0.dev20240414/src/lightning/app/components/multi_node/pytorch_spawn.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/components/multi_node/trainer.py` & `lightning-2.3.0.dev20240414/src/lightning/app/components/multi_node/trainer.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/components/python/popen.py` & `lightning-2.3.0.dev20240414/src/lightning/app/components/python/popen.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/components/python/tracer.py` & `lightning-2.3.0.dev20240414/src/lightning/app/components/python/tracer.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/components/serve/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/app/components/serve/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/components/serve/auto_scaler.py` & `lightning-2.3.0.dev20240414/src/lightning/app/components/serve/auto_scaler.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/components/serve/catimage.png` & `lightning-2.3.0.dev20240414/src/lightning/app/components/serve/catimage.png`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/components/serve/cold_start_proxy.py` & `lightning-2.3.0.dev20240414/src/lightning/app/components/serve/cold_start_proxy.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/components/serve/gradio_server.py` & `lightning-2.3.0.dev20240414/src/lightning/app/components/serve/gradio_server.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/components/serve/python_server.py` & `lightning-2.3.0.dev20240414/src/lightning/app/components/serve/python_server.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/components/serve/serve.py` & `lightning-2.3.0.dev20240414/src/lightning/app/components/serve/serve.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/components/serve/streamlit.py` & `lightning-2.3.0.dev20240414/src/lightning/app/components/serve/streamlit.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/components/serve/types/image.py` & `lightning-2.3.0.dev20240414/src/lightning/app/components/serve/types/image.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/components/serve/types/type.py` & `lightning-2.3.0.dev20240414/src/lightning/app/components/serve/types/type.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/components/training.py` & `lightning-2.3.0.dev20240414/src/lightning/app/components/training.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/core/api.py` & `lightning-2.3.0.dev20240414/src/lightning/app/core/api.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/core/app.py` & `lightning-2.3.0.dev20240414/src/lightning/app/core/app.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/core/constants.py` & `lightning-2.3.0.dev20240414/src/lightning/app/core/constants.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/core/flow.py` & `lightning-2.3.0.dev20240414/src/lightning/app/core/flow.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/core/queues.py` & `lightning-2.3.0.dev20240414/src/lightning/app/core/queues.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/core/work.py` & `lightning-2.3.0.dev20240414/src/lightning/app/core/work.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/frontend/frontend.py` & `lightning-2.3.0.dev20240414/src/lightning/app/frontend/frontend.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/frontend/just_py/just_py.py` & `lightning-2.3.0.dev20240414/src/lightning/app/frontend/just_py/just_py.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/frontend/just_py/just_py_base.py` & `lightning-2.3.0.dev20240414/src/lightning/app/frontend/just_py/just_py_base.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/frontend/panel/app_state_comm.py` & `lightning-2.3.0.dev20240414/src/lightning/app/frontend/panel/app_state_comm.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/frontend/panel/app_state_watcher.py` & `lightning-2.3.0.dev20240414/src/lightning/app/frontend/panel/app_state_watcher.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/frontend/panel/panel_frontend.py` & `lightning-2.3.0.dev20240414/src/lightning/app/frontend/panel/panel_frontend.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/frontend/panel/panel_serve_render_fn.py` & `lightning-2.3.0.dev20240414/src/lightning/app/frontend/panel/panel_serve_render_fn.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/frontend/stream_lit.py` & `lightning-2.3.0.dev20240414/src/lightning/app/frontend/stream_lit.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/frontend/streamlit_base.py` & `lightning-2.3.0.dev20240414/src/lightning/app/frontend/streamlit_base.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/frontend/utils.py` & `lightning-2.3.0.dev20240414/src/lightning/app/frontend/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/frontend/web.py` & `lightning-2.3.0.dev20240414/src/lightning/app/frontend/web.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/launcher/launcher.py` & `lightning-2.3.0.dev20240414/src/lightning/app/launcher/launcher.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/launcher/lightning_backend.py` & `lightning-2.3.0.dev20240414/src/lightning/app/launcher/lightning_backend.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/launcher/lightning_hybrid_backend.py` & `lightning-2.3.0.dev20240414/src/lightning/app/launcher/lightning_hybrid_backend.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/pdb/pdb.py` & `lightning-2.3.0.dev20240414/src/lightning/app/pdb/pdb.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/plugin/plugin.py` & `lightning-2.3.0.dev20240414/src/lightning/app/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/runners/backends/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/app/runners/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/runners/backends/backend.py` & `lightning-2.3.0.dev20240414/src/lightning/app/runners/backends/backend.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/runners/backends/cloud.py` & `lightning-2.3.0.dev20240414/src/lightning/app/runners/backends/cloud.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/runners/backends/docker.py` & `lightning-2.3.0.dev20240414/src/lightning/app/runners/backends/docker.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/runners/backends/mp_process.py` & `lightning-2.3.0.dev20240414/src/lightning/app/runners/backends/mp_process.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/runners/cloud.py` & `lightning-2.3.0.dev20240414/src/lightning/app/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/runners/multiprocess.py` & `lightning-2.3.0.dev20240414/src/lightning/app/runners/multiprocess.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/runners/runtime.py` & `lightning-2.3.0.dev20240414/src/lightning/app/runners/runtime.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/runners/runtime_type.py` & `lightning-2.3.0.dev20240414/src/lightning/app/runners/runtime_type.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/source_code/copytree.py` & `lightning-2.3.0.dev20240414/src/lightning/app/source_code/copytree.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/source_code/hashing.py` & `lightning-2.3.0.dev20240414/src/lightning/app/source_code/hashing.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/source_code/local.py` & `lightning-2.3.0.dev20240414/src/lightning/app/source_code/local.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/source_code/tar.py` & `lightning-2.3.0.dev20240414/src/lightning/app/source_code/tar.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/source_code/uploader.py` & `lightning-2.3.0.dev20240414/src/lightning/app/source_code/uploader.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/storage/copier.py` & `lightning-2.3.0.dev20240414/src/lightning/app/storage/copier.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/storage/drive.py` & `lightning-2.3.0.dev20240414/src/lightning/app/storage/drive.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/storage/filesystem.py` & `lightning-2.3.0.dev20240414/src/lightning/app/storage/filesystem.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/storage/mount.py` & `lightning-2.3.0.dev20240414/src/lightning/app/storage/mount.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/storage/orchestrator.py` & `lightning-2.3.0.dev20240414/src/lightning/app/storage/orchestrator.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/storage/path.py` & `lightning-2.3.0.dev20240414/src/lightning/app/storage/path.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/storage/payload.py` & `lightning-2.3.0.dev20240414/src/lightning/app/storage/payload.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/storage/requests.py` & `lightning-2.3.0.dev20240414/src/lightning/app/storage/requests.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/structures/dict.py` & `lightning-2.3.0.dev20240414/src/lightning/app/structures/dict.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/structures/list.py` & `lightning-2.3.0.dev20240414/src/lightning/app/structures/list.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/testing/config.py` & `lightning-2.3.0.dev20240414/src/lightning/app/testing/config.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/testing/helpers.py` & `lightning-2.3.0.dev20240414/src/lightning/app/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/testing/testing.py` & `lightning-2.3.0.dev20240414/src/lightning/app/testing/testing.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/ui/asset-manifest.json` & `lightning-2.3.0.dev20240414/src/lightning/app/ui/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/ui/index.html` & `lightning-2.3.0.dev20240414/src/lightning/app/ui/index.html`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/ui/static/css/main.fb7060be.css` & `lightning-2.3.0.dev20240414/src/lightning/app/ui/static/css/main.fb7060be.css`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/ui/static/css/main.fb7060be.css.map` & `lightning-2.3.0.dev20240414/src/lightning/app/ui/static/css/main.fb7060be.css.map`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/ui/static/favicon.ico` & `lightning-2.3.0.dev20240414/src/lightning/app/ui/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/ui/static/js/787.418637a8.chunk.js` & `lightning-2.3.0.dev20240414/src/lightning/app/ui/static/js/787.418637a8.chunk.js`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/ui/static/js/787.418637a8.chunk.js.map` & `lightning-2.3.0.dev20240414/src/lightning/app/ui/static/js/787.418637a8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/ui/static/js/main.c1f02aeb.js` & `lightning-2.3.0.dev20240414/src/lightning/app/ui/static/js/main.c1f02aeb.js`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/ui/static/js/main.c1f02aeb.js.LICENSE.txt` & `lightning-2.3.0.dev20240414/src/lightning/app/ui/static/js/main.c1f02aeb.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/ui/static/js/main.c1f02aeb.js.map` & `lightning-2.3.0.dev20240414/src/lightning/app/ui/static/js/main.c1f02aeb.js.map`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/ui/static/lightningState.js` & `lightning-2.3.0.dev20240414/src/lightning/app/ui/static/lightningState.js`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg` & `lightning-2.3.0.dev20240414/src/lightning/app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg` & `lightning-2.3.0.dev20240414/src/lightning/app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/app_commands.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/app_commands.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/app_helpers.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/app_helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/app_logs.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/app_logs.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/app_status.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/app_status.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/auth.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/auth.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/cli_helpers.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/cli_helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/cloud.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/cloud.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/clusters.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/clusters.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/commands/base.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/commands/base.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/component.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/component.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/data_structures.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/data_structures.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/dependency_caching.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/dependency_caching.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/enum.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/enum.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/exceptions.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/frontend.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/frontend.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/git.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/git.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/imports.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/imports.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/introspection.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/introspection.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/layout.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/layout.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/load_app.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/load_app.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/log.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/log.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/log_helpers.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/log_helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/login.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/login.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/logs_socket_api.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/logs_socket_api.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/name_generator.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/name_generator.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/network.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/network.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/openapi.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/openapi.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/packaging/app_config.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/packaging/app_config.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/packaging/build_config.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/packaging/build_config.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/packaging/cloud_compute.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/packaging/cloud_compute.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/packaging/docker.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/packaging/docker.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/packaging/lightning_utils.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/packaging/lightning_utils.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/packaging/tarfile.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/packaging/tarfile.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/port.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/port.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/proxies.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/proxies.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/redis.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/redis.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/safe_pickle.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/safe_pickle.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/scheduler.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/scheduler.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/secrets.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/secrets.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/state.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/state.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/tracer.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/tracer.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/tree.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/tree.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/types.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/types.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/app/utilities/warnings.py` & `lightning-2.3.0.dev20240414/src/lightning/app/utilities/warnings.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/data/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/data/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/CHANGELOG.md` & `lightning-2.3.0.dev20240414/src/lightning/fabric/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,16 @@
 
 ### Fixed
 
 - Fixed an issue causing a TypeError when using `torch.compile` as a decorator ([#19627](https://github.com/Lightning-AI/pytorch-lightning/pull/19627))
 
 - Fixed issue where some model methods couldn't be monkeypatched after being Fabric wrapped ([#19705](https://github.com/Lightning-AI/pytorch-lightning/pull/19705))
 
--
+- Fixed an issue causing weights to be reset in `Fabric.setup()` when using FSDP ([#19755](https://github.com/Lightning-AI/pytorch-lightning/pull/19755))
+
 
 
 ## [2.2.1] - 2024-03-04
 
 ### Fixed
 
 - Fixed an issue with CSVLogger trying to append to file from a previous run when the version is set manually ([#19446](https://github.com/Lightning-AI/lightning/pull/19446))
```

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/_graveyard/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/_graveyard/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/_graveyard/tpu.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/_graveyard/tpu.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/accelerators/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/accelerators/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/accelerators/accelerator.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/accelerators/accelerator.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/accelerators/cpu.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/accelerators/cpu.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/accelerators/cuda.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/accelerators/cuda.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/accelerators/mps.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/accelerators/mps.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/accelerators/registry.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/accelerators/registry.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/accelerators/xla.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/accelerators/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/cli.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/connector.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/connector.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/fabric.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/fabric.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/loggers/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/loggers/csv_logs.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/loggers/csv_logs.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/loggers/logger.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/loggers/tensorboard.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/collectives/collective.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/collectives/collective.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/collectives/single_device.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/collectives/single_device.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/collectives/torch_collective.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/collectives/torch_collective.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/environments/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/environments/cluster_environment.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/environments/cluster_environment.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/environments/kubeflow.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/environments/kubeflow.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/environments/lightning.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/environments/lightning.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/environments/lsf.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/environments/lsf.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/environments/mpi.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/environments/mpi.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/environments/slurm.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/environments/slurm.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/environments/torchelastic.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/environments/torchelastic.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/environments/xla.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/environments/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/io/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/io/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/io/checkpoint_io.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/io/checkpoint_io.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/io/torch_io.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/io/torch_io.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/io/xla.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/io/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/precision/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/precision/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/precision/amp.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/precision/amp.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/precision/bitsandbytes.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/precision/bitsandbytes.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/precision/deepspeed.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/precision/deepspeed.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/precision/double.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/precision/double.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/precision/fsdp.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/precision/fsdp.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/precision/half.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/precision/half.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/precision/precision.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/precision/precision.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/precision/transformer_engine.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/precision/transformer_engine.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/precision/utils.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/precision/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/plugins/precision/xla.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/plugins/precision/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/ddp.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/ddp.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/deepspeed.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/deepspeed.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/dp.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/dp.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/fsdp.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/fsdp.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/launchers/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/launchers/launcher.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/launchers/launcher.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/launchers/multiprocessing.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/launchers/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/launchers/subprocess_script.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/launchers/subprocess_script.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/launchers/xla.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/launchers/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/parallel.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/parallel.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/registry.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/registry.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/single_device.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/single_device.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/single_xla.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/single_xla.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/strategy.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/xla.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/strategies/xla_fsdp.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/strategies/xla_fsdp.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/apply_func.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/apply_func.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/cloud_io.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/cloud_io.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/consolidate_checkpoint.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/consolidate_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/data.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/data.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/device_dtype_mixin.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/device_dtype_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,18 +105,16 @@
         _update_properties(self, dtype=torch.half)
         return super().half()
 
 
 def _update_properties(
     root: torch.nn.Module, device: Optional[torch.device] = None, dtype: Optional[Union[str, torch.dtype]] = None
 ) -> None:
-    def apply_fn(module: Union[_DeviceDtypeModuleMixin, Module]) -> None:
+    for module in root.modules():
         if not isinstance(module, _DeviceDtypeModuleMixin):
-            return
+            continue
         # cannot use `module.to()` because we don't actually want to move the model in case there are multiple
         # devices types (such as partial meta parameters)
         if device is not None:
             module._device = device
         if dtype is not None:
             module._dtype = dtype
-
-    root.apply(apply_fn)
```

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/device_parser.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/device_parser.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/distributed.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/distributed.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/enums.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/enums.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/exceptions.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/imports.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/imports.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/init.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/init.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/load.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/load.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/logger.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/optimizer.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/optimizer.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/rank_zero.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/rank_zero.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/registry.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/registry.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/seed.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/seed.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/spike.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/spike.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/testing/_runif.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/testing/_runif.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/throughput.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/throughput.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/types.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/types.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/utilities/warnings.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/utilities/warnings.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/fabric/wrappers.py` & `lightning-2.3.0.dev20240414/src/lightning/fabric/wrappers.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/CHANGELOG.md` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/_graveyard/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/_graveyard/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/_graveyard/_torchmetrics.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/_graveyard/_torchmetrics.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/_graveyard/hpu.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/_graveyard/hpu.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/_graveyard/precision.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/_graveyard/precision.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/_graveyard/tpu.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/_graveyard/tpu.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/accelerators/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/accelerators/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/accelerators/accelerator.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/accelerators/accelerator.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/accelerators/cpu.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/accelerators/cpu.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/accelerators/cuda.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/accelerators/cuda.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/accelerators/mps.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/accelerators/mps.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/accelerators/xla.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/accelerators/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/batch_size_finder.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/batch_size_finder.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/callback.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/device_stats_monitor.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/device_stats_monitor.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/early_stopping.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/finetuning.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/finetuning.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/gradient_accumulation_scheduler.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/gradient_accumulation_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/lambda_function.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/lambda_function.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/lr_finder.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/lr_finder.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/lr_monitor.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/lr_monitor.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/model_checkpoint.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/model_summary.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/model_summary.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/on_exception_checkpoint.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/on_exception_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/prediction_writer.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/prediction_writer.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/progress/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/progress/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/progress/progress_bar.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/progress/progress_bar.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/progress/rich_progress.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/progress/rich_progress.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/progress/tqdm_progress.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/progress/tqdm_progress.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/pruning.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/pruning.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/rich_model_summary.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/rich_model_summary.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/spike.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/spike.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/stochastic_weight_avg.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/stochastic_weight_avg.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/throughput_monitor.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/throughput_monitor.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/callbacks/timer.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/callbacks/timer.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/cli.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/core/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/core/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/core/datamodule.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/core/datamodule.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/core/hooks.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/core/hooks.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/core/mixins/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/core/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/core/mixins/hparams_mixin.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/core/mixins/hparams_mixin.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/core/module.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/core/module.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/core/optimizer.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/core/optimizer.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/core/saving.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/core/saving.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/demos/boring_classes.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/demos/boring_classes.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/demos/mnist_datamodule.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/demos/mnist_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/demos/transformer.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/demos/transformer.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/loggers/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/loggers/comet.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/loggers/comet.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/loggers/csv_logs.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/loggers/csv_logs.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/loggers/logger.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/loggers/mlflow.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/loggers/mlflow.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/loggers/neptune.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/loggers/neptune.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/loggers/tensorboard.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/loggers/utilities.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/loggers/utilities.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/loggers/wandb.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/loggers/wandb.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/loops/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/loops/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/loops/evaluation_loop.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/loops/evaluation_loop.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/loops/fetchers.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/loops/fetchers.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/loops/fit_loop.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/loops/fit_loop.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/loops/loop.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/loops/loop.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/loops/optimization/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/loops/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/loops/optimization/automatic.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/loops/optimization/automatic.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/loops/optimization/closure.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/loops/optimization/closure.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/loops/optimization/manual.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/loops/optimization/manual.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/loops/prediction_loop.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/loops/prediction_loop.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/loops/progress.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/loops/progress.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/loops/training_epoch_loop.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/loops/training_epoch_loop.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/loops/utilities.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/loops/utilities.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/overrides/distributed.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/overrides/distributed.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/environments/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/io/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/io/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/io/async_plugin.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/io/async_plugin.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/io/checkpoint_plugin.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/io/checkpoint_plugin.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/io/torch_plugin.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/io/torch_plugin.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/io/wrapper.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/io/wrapper.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/io/xla_plugin.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/io/xla_plugin.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/layer_sync.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/layer_sync.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/precision/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/precision/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/precision/amp.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/precision/amp.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/precision/bitsandbytes.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/precision/bitsandbytes.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/precision/deepspeed.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/precision/deepspeed.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/precision/double.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/precision/double.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/precision/fsdp.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/precision/fsdp.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/precision/half.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/precision/half.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/precision/precision.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/precision/precision.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/precision/transformer_engine.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/precision/transformer_engine.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/plugins/precision/xla.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/plugins/precision/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/profilers/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/profilers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/profilers/advanced.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/profilers/advanced.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/profilers/base.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/profilers/base.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/profilers/profiler.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/profilers/profiler.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/profilers/pytorch.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/profilers/pytorch.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/profilers/simple.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/profilers/simple.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/profilers/xla.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/profilers/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/serve/servable_module.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/serve/servable_module.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/serve/servable_module_validator.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/serve/servable_module_validator.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/ddp.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/ddp.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/deepspeed.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/deepspeed.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/fsdp.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/fsdp.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/launchers/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/launchers/launcher.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/launchers/launcher.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/launchers/multiprocessing.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/launchers/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/launchers/subprocess_script.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/launchers/subprocess_script.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/launchers/xla.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/launchers/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/parallel.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/parallel.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/single_device.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/single_device.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/single_xla.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/single_xla.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/strategy.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/strategies/xla.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/strategies/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/call.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/call.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/configuration_validator.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/configuration_validator.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/connectors/accelerator_connector.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/connectors/accelerator_connector.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/connectors/callback_connector.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/connectors/callback_connector.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/connectors/checkpoint_connector.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/connectors/checkpoint_connector.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/connectors/data_connector.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/connectors/data_connector.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/connectors/logger_connector/fx_validator.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/connectors/logger_connector/fx_validator.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/connectors/logger_connector/logger_connector.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/connectors/logger_connector/logger_connector.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/connectors/logger_connector/result.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/connectors/logger_connector/result.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/connectors/signal_connector.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/connectors/signal_connector.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/setup.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/states.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/states.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/trainer/trainer.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/tuner/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/tuner/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/tuner/batch_size_scaling.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/tuner/batch_size_scaling.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/tuner/lr_finder.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/tuner/lr_finder.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/tuner/tuning.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/tuner/tuning.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/_pytree.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/_pytree.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/argparse.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/argparse.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/combined_loader.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/combined_loader.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/compile.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/compile.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/consolidate_checkpoint.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/consolidate_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/data.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/data.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/deepspeed.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/deepspeed.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/enums.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/enums.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/exceptions.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/grads.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/grads.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/imports.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/imports.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/memory.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/memory.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/migration/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/migration/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/migration/migration.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/migration/migration.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/migration/utils.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/migration/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/model_helpers.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/model_helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/model_summary/__init__.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/model_summary/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/model_summary/model_summary.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/model_summary/model_summary.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/model_summary/model_summary_deepspeed.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/model_summary/model_summary_deepspeed.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/parameter_tying.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/parameter_tying.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/parsing.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/parsing.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/rank_zero.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/rank_zero.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/seed.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/seed.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/signature_utils.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/signature_utils.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/testing/_runif.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/testing/_runif.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/types.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/types.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/upgrade_checkpoint.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/upgrade_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/pytorch/utilities/warnings.py` & `lightning-2.3.0.dev20240414/src/lightning/pytorch/utilities/warnings.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/store/store.py` & `lightning-2.3.0.dev20240414/src/lightning/store/store.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning/store/utils.py` & `lightning-2.3.0.dev20240414/src/lightning/store/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-2.3.0.dev20240407/src/lightning.egg-info/PKG-INFO` & `lightning-2.3.0.dev20240414/src/lightning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning
-Version: 2.3.0.dev20240407
+Version: 2.3.0.dev20240414
 Summary: The Deep Learning framework to train, deploy, and ship AI products Lightning fast.
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
@@ -74,15 +74,15 @@
 ______________________________________________________________________
 
 <p align="center">
   <a href="https://lightning.ai/">Lightning.ai</a> •
   <a href="https://lightning.ai/docs/pytorch/stable/">PyTorch Lightning</a> •
   <a href="https://lightning.ai/docs/fabric/stable/">Fabric</a> •
   <a href="https://lightning.ai/docs/app/stable/">Lightning Apps</a> •
-  <a href="https://pytorch-lightning.readthedocs.io/en/2.3.0.dev20240407">Docs</a> •
+  <a href="https://pytorch-lightning.readthedocs.io/en/2.3.0.dev20240414">Docs</a> •
   <a href="#community">Community</a> •
   <a href="https://lightning.ai/docs/pytorch/stable/generated/CONTRIBUTING.html">Contribute</a> •
 </p>
 
 <!-- DO NOT ADD CONDA DOWNLOADS... README CHANGES MUST BE APPROVED BY EDEN OR WILL -->
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytorch-lightning)](https://pypi.org/project/pytorch-lightning/)
@@ -619,15 +619,15 @@
 <details>
   <summary>Current build statuses</summary>
 
 <center>
 
 |       System / PyTorch ver.        | 1.13                                                                                                                                                                                                                            | 2.0                                                                                                                                                                                                                             |                                                                                                               2.1                                                                                                               |
 | :--------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
-|        Linux py3.9 \[GPUs\]        |  |  | [![Build Status](https://dev.azure.com/Lightning-AI/lightning/_apis/build/status%2Fpytorch-lightning%20%28GPUs%29?branchName=refs%2Ftags%2F2.3.0.dev20240407)](https://dev.azure.com/Lightning-AI/lightning/_build/latest?definitionId=24&branchName=master) |
+|        Linux py3.9 \[GPUs\]        |  |  | [![Build Status](https://dev.azure.com/Lightning-AI/lightning/_apis/build/status%2Fpytorch-lightning%20%28GPUs%29?branchName=refs%2Ftags%2F2.3.0.dev20240414)](https://dev.azure.com/Lightning-AI/lightning/_build/latest?definitionId=24&branchName=master) |
 |        Linux py3.9 \[TPUs\]        |                                                                                                                                                                                                                                 |  [![Test PyTorch - TPU](https://github.com/Lightning-AI/lightning/actions/workflows/tpu-tests.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/tpu-tests.yml)     |      |
 |  Linux (multiple Python versions)  | [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                                 | [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                                 |                 [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                 |
 |   OSX (multiple Python versions)   | [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                                 | [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                                 |                 [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                 |
 | Windows (multiple Python versions) | [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                                 | [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                                 |                 [![Test PyTorch](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml/badge.svg)](https://github.com/Lightning-AI/lightning/actions/workflows/ci-tests-pytorch.yml)                 |
 
 </center>
 </details>
```

### Comparing `lightning-2.3.0.dev20240407/src/lightning.egg-info/SOURCES.txt` & `lightning-2.3.0.dev20240414/src/lightning.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 requirements/pytorch/base.txt
 requirements/pytorch/docs.txt
 requirements/pytorch/examples.txt
 requirements/pytorch/extra.txt
 requirements/pytorch/strategies.txt
 requirements/pytorch/test.txt
 src/version.info
-src/lightning/1714ed7a47b2b85f2b1eebdd05b5f1cc91bf167a3421e0ef
 src/lightning/__about__.py
 src/lightning/__init__.py
 src/lightning/__main__.py
 src/lightning/__setup__.py
 src/lightning/__version__.py
+src/lightning/e4e465c6f6642e9f9fc64f431fc44401b9981f6435f96f96
 src/lightning/py.typed
 src/lightning/version.info
 src/lightning.egg-info/PKG-INFO
 src/lightning.egg-info/SOURCES.txt
 src/lightning.egg-info/dependency_links.txt
 src/lightning.egg-info/entry_points.txt
 src/lightning.egg-info/not-zip-safe
```

### Comparing `lightning-2.3.0.dev20240407/src/lightning.egg-info/requires.txt` & `lightning-2.3.0.dev20240414/src/lightning.egg-info/requires.txt`

 * *Files identical despite different names*

