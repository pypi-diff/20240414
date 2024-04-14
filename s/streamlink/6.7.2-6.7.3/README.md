# Comparing `tmp/streamlink-6.7.2.tar.gz` & `tmp/streamlink-6.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlink-6.7.2.tar", last modified: Sat Mar 23 12:22:35 2024, max compression
+gzip compressed data, was "streamlink-6.7.3.tar", last modified: Sun Apr 14 15:40:52 2024, max compression
```

## Comparing `streamlink-6.7.2.tar` & `streamlink-6.7.3.tar`

### file list

```diff
@@ -1,674 +1,674 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:35.018673 streamlink-6.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-23 12:22:01.000000 streamlink-6.7.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    99162 2024-03-23 12:22:01.000000 streamlink-6.7.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-03-23 12:22:01.000000 streamlink-6.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-23 12:22:01.000000 streamlink-6.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-03-23 12:22:35.018673 streamlink-6.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-03-23 12:22:01.000000 streamlink-6.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.910674 streamlink-6.7.2/build_backend/
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-03-23 12:22:01.000000 streamlink-6.7.2/build_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-23 12:22:01.000000 streamlink-6.7.2/build_backend/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-03-23 12:22:01.000000 streamlink-6.7.2/build_backend/onbuild.py
--rw-r--r--   0 runner    (1001) docker     (127)    15908 2024-03-23 12:22:01.000000 streamlink-6.7.2/build_backend/plugins_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-03-23 12:22:01.000000 streamlink-6.7.2/build_backend/test_build_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-03-23 12:22:01.000000 streamlink-6.7.2/build_backend/test_onbuild.py
--rw-r--r--   0 runner    (1001) docker     (127)    37280 2024-03-23 12:22:01.000000 streamlink-6.7.2/build_backend/test_plugins_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.898674 streamlink-6.7.2/completions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.910674 streamlink-6.7.2/completions/bash/
--rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-03-23 12:22:30.000000 streamlink-6.7.2/completions/bash/streamlink
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.910674 streamlink-6.7.2/completions/zsh/
--rw-r--r--   0 runner    (1001) docker     (127)    36671 2024-03-23 12:22:30.000000 streamlink-6.7.2/completions/zsh/_streamlink
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-23 12:22:01.000000 streamlink-6.7.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.914674 streamlink-6.7.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.902674 streamlink-6.7.2/docs/_build/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.914674 streamlink-6.7.2/docs/_build/man/
--rw-r--r--   0 runner    (1001) docker     (127)    41171 2024-03-23 12:22:29.000000 streamlink-6.7.2/docs/_build/man/streamlink.1
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/_man.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.918674 streamlink-6.7.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    12092 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/_static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/_static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/_static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/_static/icon-ffmpeg.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/_static/icon-python.svg
--rw-r--r--   0 runner    (1001) docker     (127)    18593 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/_static/icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15790 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/_static/opengraph-image.png
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/_static/site.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.918674 streamlink-6.7.2/docs/_static/styles/
--rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/_static/styles/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.918674 streamlink-6.7.2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/_templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/_templates/page.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.918674 streamlink-6.7.2/docs/_templates/sidebar/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/_templates/sidebar/brand.html
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/_templates/sidebar/github-buttons.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.918674 streamlink-6.7.2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/api/cache.rst
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/api/options.rst
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/api/plugin.rst
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/api/session.rst
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/api/stream.rst
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/api/streamlink.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/api/validate.rst
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/api/webbrowser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.922674 streamlink-6.7.2/docs/api_guide/
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/api_guide/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)    17250 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/api_guide/validate.rst
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/api_guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/applications.rst
--rw-r--r--   0 runner    (1001) docker     (127)    99162 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.922674 streamlink-6.7.2/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/cli/config.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/cli/metadata.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/cli/plugin-sideloading.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.922674 streamlink-6.7.2/docs/cli/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/cli/plugins/crunchyroll.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10202 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/cli/plugins/twitch.rst
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/cli/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/cli/protocols.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/cli/proxy.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/cli/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    11426 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/deprecations.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/docutils.conf
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/donate.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/ext_argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/ext_github.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/ext_html_template_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/ext_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/ext_releaseref.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    25334 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11739 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/migrations.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/players.rst
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs/thirdparty.rst
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-23 12:22:01.000000 streamlink-6.7.2/docs-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18593 2024-03-23 12:22:01.000000 streamlink-6.7.2/icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-03-23 12:22:35.022673 streamlink-6.7.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.922674 streamlink-6.7.2/script/
--rwxr-xr-x   0 runner    (1001) docker     (127)      802 2024-03-23 12:22:01.000000 streamlink-6.7.2/script/build-shell-completions.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 12:22:35.018673 streamlink-6.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-03-23 12:22:35.022673 streamlink-6.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.902674 streamlink-6.7.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.926674 streamlink-6.7.2/src/streamlink/
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-23 12:22:35.022673 streamlink-6.7.2/src/streamlink/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/buffers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8007 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.926674 streamlink-6.7.2/src/streamlink/packages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/packages/requests_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.926674 streamlink-6.7.2/src/streamlink/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.926674 streamlink-6.7.2/src/streamlink/plugin/api/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugin/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugin/api/http_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugin/api/useragents.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.926674 streamlink-6.7.2/src/streamlink/plugin/api/validate/
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugin/api/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugin/api/validate/_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugin/api/validate/_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    11763 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugin/api/validate/_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)    19460 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugin/api/validate/_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugin/api/websocket.py
--rw-r--r--   0 runner    (1001) docker     (127)    26032 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.954673 streamlink-6.7.2/src/streamlink/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9677 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/abematv.py
--rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/adultswim.py
--rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/afreeca.py
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/albavision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/aloula.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/app17.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/ard_live.py
--rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/ard_mediathek.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/artetv.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/atpchallenger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/atresplayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/bbciplayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/bfmtv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/bigo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/bilibili.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/blazetv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/bloomberg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/booyah.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/brightcove.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/btv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/cbsnews.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/cdnbg.py
--rw-r--r--   0 runner    (1001) docker     (127)     7082 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/ceskatelevize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/cinergroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/clubbingtv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/cmmedia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/cnews.py
--rw-r--r--   0 runner    (1001) docker     (127)    14036 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/crunchyroll.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/dailymotion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/dash.py
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/delfi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/deutschewelle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/dlive.py
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/dogan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/dogus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/drdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/earthcam.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/euronews.py
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/facebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     8421 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/filmon.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/galatasaraytv.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/goltelevision.py
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/goodgame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/googledrive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/gulli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/hiplayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/hls.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/htv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/huajiao.py
--rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/huya.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/idf1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/indihometv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/invintus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/kugou.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/linelive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/livestream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/lnk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/lrt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/ltv_lsm_lv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/mangomolo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/mdstrm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/mediaklikk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/mediavitrina.py
--rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/mildom.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/mitele.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/mixcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/mjunoon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/mrtmk.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/n13tv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/nasaplus.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/nhkworld.py
--rw-r--r--   0 runner    (1001) docker     (127)    10573 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/nicolive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/nimotv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/nos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/nownews.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/nowtvtr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/nrk.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/okru.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/olympicchannel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/oneplusone.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/onetv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/openrectv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/pandalive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/piaulizaportal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/picarto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/piczel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/pixiv.py
--rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/pluto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/pluzz.py
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/radiko.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/radionet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/raiplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/reuters.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/rtpa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/rtpplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/rtve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/rtvs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/ruv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/sbscokr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/showroom.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/sportal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/sportschau.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/ssh101.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/stadium.py
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/steam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/streamable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/streann.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/stv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/svtplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/swisstxt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/telefe.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/telemadrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/tf1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/trovo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/turkuvaz.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/tv360.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/tv3cat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/tv4play.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/tv5monde.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/tv8.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/tv999.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/tvibo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/tviplayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/tvp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/tvrby.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/tvrplus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/tvtoya.py
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/twitcasting.py
--rw-r--r--   0 runner    (1001) docker     (127)    33777 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/twitch.py
--rw-r--r--   0 runner    (1001) docker     (127)    19213 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/ustreamtv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/ustvnow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/vidio.py
--rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/vimeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/vinhlongtv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/vk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/vkplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/vtvgo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/webtv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/welt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/wwenetwork.py
--rw-r--r--   0 runner    (1001) docker     (127)    15401 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/youtube.py
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/yupptv.py
--rw-r--r--   0 runner    (1001) docker     (127)    12860 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/zattoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/zdf_mediathek.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/zeenews.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/zengatv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/plugins/zhanqi.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.958673 streamlink-6.7.2/src/streamlink/session/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/session/http.py
--rw-r--r--   0 runner    (1001) docker     (127)    12151 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/session/http.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19101 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/session/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    13238 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/session/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/session/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.958673 streamlink-6.7.2/src/streamlink/stream/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/stream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.958673 streamlink-6.7.2/src/streamlink/stream/dash/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/stream/dash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14067 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/stream/dash/dash.py
--rw-r--r--   0 runner    (1001) docker     (127)    36858 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/stream/dash/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/stream/dash/segment.py
--rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/stream/ffmpegmux.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/stream/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/stream/filtered.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.958673 streamlink-6.7.2/src/streamlink/stream/hls/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/stream/hls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33983 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/stream/hls/hls.py
--rw-r--r--   0 runner    (1001) docker     (127)    21481 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/stream/hls/m3u8.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/stream/hls/segment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/stream/http.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.958673 streamlink-6.7.2/src/streamlink/stream/segmented/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/stream/segmented/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/stream/segmented/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/stream/segmented/segment.py
--rw-r--r--   0 runner    (1001) docker     (127)     8118 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/stream/segmented/segmented.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/stream/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/user_input.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.962673 streamlink-6.7.2/src/streamlink/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/utils/args.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/utils/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/utils/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/utils/l10n.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/utils/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/utils/named_pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/utils/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/utils/processoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/utils/socket.py
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/utils/times.py
--rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/utils/url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.962673 streamlink-6.7.2/src/streamlink/webbrowser/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/webbrowser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.962673 streamlink-6.7.2/src/streamlink/webbrowser/cdp/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/webbrowser/cdp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/webbrowser/cdp/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13939 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/webbrowser/cdp/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.966673 streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21632 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/browser.py
--rw-r--r--   0 runner    (1001) docker     (127)    49407 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/debugger.py
--rw-r--r--   0 runner    (1001) docker     (127)    61679 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/dom.py
--rw-r--r--   0 runner    (1001) docker     (127)    26084 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/emulation.py
--rw-r--r--   0 runner    (1001) docker     (127)    19534 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)    27632 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/input_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/io.py
--rw-r--r--   0 runner    (1001) docker     (127)   130706 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/network.py
--rw-r--r--   0 runner    (1001) docker     (127)   107521 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/page.py
--rw-r--r--   0 runner    (1001) docker     (127)    62110 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)    17300 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/security.py
--rw-r--r--   0 runner    (1001) docker     (127)    24082 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/target.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/webbrowser/cdp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8564 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/webbrowser/chromium.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/webbrowser/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink/webbrowser/webbrowser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:35.018673 streamlink-6.7.2/src/streamlink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-03-23 12:22:34.000000 streamlink-6.7.2/src/streamlink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19654 2024-03-23 12:22:34.000000 streamlink-6.7.2/src/streamlink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 12:22:34.000000 streamlink-6.7.2/src/streamlink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-23 12:22:34.000000 streamlink-6.7.2/src/streamlink.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-23 12:22:34.000000 streamlink-6.7.2/src/streamlink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-23 12:22:34.000000 streamlink-6.7.2/src/streamlink.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.970673 streamlink-6.7.2/src/streamlink_cli/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink_cli/_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    49425 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink_cli/argparser.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink_cli/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink_cli/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink_cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    31969 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.970673 streamlink-6.7.2/src/streamlink_cli/output/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink_cli/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink_cli/output/abc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink_cli/output/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink_cli/output/http.py
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink_cli/output/player.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink_cli/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink_cli/streamrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.970673 streamlink-6.7.2/src/streamlink_cli/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink_cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink_cli/utils/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink_cli/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink_cli/utils/player.py
--rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink_cli/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-03-23 12:22:01.000000 streamlink-6.7.2/src/streamlink_cli/utils/versioncheck.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.974673 streamlink-6.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.974673 streamlink-6.7.2/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.974673 streamlink-6.7.2/tests/cli/output/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/cli/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/cli/output/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    13144 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/cli/output/test_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/cli/test_argparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/cli/test_cmdline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/cli/test_cmdline_title.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/cli/test_console.py
--rw-r--r--   0 runner    (1001) docker     (127)    18037 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/cli/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/cli/test_main_check_file_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/cli/test_main_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    16038 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/cli/test_main_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/cli/test_main_setup_config_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/cli/test_plugin_args_and_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    23211 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/cli/test_streamrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.978673 streamlink-6.7.2/tests/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/cli/utils/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/cli/utils/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/cli/utils/test_player.py
--rw-r--r--   0 runner    (1001) docker     (127)    15076 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/cli/utils/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/cli/utils/test_versioncheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.978673 streamlink-6.7.2/tests/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/mixins/stream_hls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.978673 streamlink-6.7.2/tests/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.978673 streamlink-6.7.2/tests/plugin/override/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugin/override/testplugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugin/testplugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugin/testplugin_invalid.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugin/testplugin_missing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:35.002673 streamlink-6.7.2/tests/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_abematv.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_adultswim.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_afreeca.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_albavision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_aloula.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_app17.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_ard_live.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_ard_mediathek.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_artetv.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_atpchallenger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_atresplayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_bbciplayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_bfmtv.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_bigo.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_bilibili.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_blazetv.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_bloomberg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_booyah.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_brightcove.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_btv.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_cbsnews.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_cdnbg.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_ceskatelevize.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_cinergroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_clubbingtv.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_cmmedia.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_cnews.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_crunchyroll.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_dailymotion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_dash.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_delfi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_deutschewelle.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_dlive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_dogan.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_dogus.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_drdk.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_earthcam.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_euronews.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_facebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_filmon.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_galatasaraytv.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_goltelevision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_goodgame.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_googledrive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_gulli.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_hiplayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_hls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_http.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_htv.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_huajiao.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_huya.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_idf1.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_indihometv.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_invintus.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_kugou.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_linelive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_livestream.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_lnk.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_lrt.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_ltv_lsm_lv.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_mangomolo.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_mdstrm.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_mediaklikk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_mediavitrina.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_mildom.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_mitele.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_mixcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_mjunoon.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_mrtmk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_n13tv.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_nasaplus.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_nhkworld.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_nicolive.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_nimotv.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_nos.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_nownews.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_nowtvtr.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_nrk.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_okru.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_olympicchannel.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_oneplusone.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_onetv.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_openrectv.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_pandalive.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_piaulizaportal.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_picarto.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_piczel.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_pixiv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_pluto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_pluzz.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_radiko.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_radionet.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_raiplay.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_reuters.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_rtpa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_rtpplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_rtve.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_rtvs.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_ruv.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_sbscokr.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_showroom.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_sportal.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_sportschau.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_ssh101.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_stadium.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_steam.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_streamable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_streann.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_stv.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_svtplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_swisstxt.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_telefe.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_telemadrid.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_tf1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_trovo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_turkuvaz.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_tv360.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_tv3cat.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_tv4play.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_tv5monde.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_tv8.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_tv999.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_tvibo.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_tviplayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_tvp.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_tvrby.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_tvrplus.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_tvtoya.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_twitcasting.py
--rw-r--r--   0 runner    (1001) docker     (127)    35577 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_twitch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_ustreamtv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_ustvnow.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_vidio.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_vimeo.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_vinhlongtv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_vk.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_vkplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_vtvgo.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_webtv.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_welt.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_wwenetwork.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_youtube.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_yupptv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_zattoo.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_zdf_mediathek.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_zeenews.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_zengatv.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/plugins/test_zhanqi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:35.002673 streamlink-6.7.2/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:34.906674 streamlink-6.7.2/tests/resources/cli/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:35.006673 streamlink-6.7.2/tests/resources/cli/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/cli/config/custom
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/cli/config/primary
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/cli/config/primary.testplugin
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/cli/config/secondary
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/cli/config/secondary.testplugin
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:35.010673 streamlink-6.7.2/tests/resources/dash/
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/dash/test_1.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/dash/test_10.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     9187 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/dash/test_11_static.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/dash/test_2.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/dash/test_3.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/dash/test_8.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/dash/test_9.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/dash/test_dynamic_segment_list_no_duration.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/dash/test_dynamic_segment_list_p1.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/dash/test_dynamic_segment_list_p2.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/dash/test_dynamic_segment_list_p3.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/dash/test_dynamic_segment_list_p4.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/dash/test_dynamic_segment_list_p5.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/dash/test_dynamic_timeline_continued_p1.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/dash/test_dynamic_timeline_continued_p2.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/dash/test_nested_baseurls.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/dash/test_no_segment_list_or_template.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/dash/test_segment_list.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/dash/test_segments_byterange.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/dash/test_segments_dynamic_number.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/dash/test_static_no_publish_time.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/dash/test_suggested_presentation_delay.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/dash/test_timeline_ids.mpd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:35.010673 streamlink-6.7.2/tests/resources/hls/
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/hls/test_1.m3u8
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/hls/test_2.m3u8
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/hls/test_date.m3u8
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/hls/test_master.m3u8
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/hls/test_master_twitch_vod.m3u8
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/resources/hls/test_multivariant_bandwidth.m3u8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:35.010673 streamlink-6.7.2/tests/session/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/session/test_http.py
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/session/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    23380 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/session/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/session/test_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:35.010673 streamlink-6.7.2/tests/stream/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/stream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:35.014673 streamlink-6.7.2/tests/stream/dash/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/stream/dash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21720 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/stream/dash/test_dash.py
--rw-r--r--   0 runner    (1001) docker     (127)    29634 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/stream/dash/test_manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:35.014673 streamlink-6.7.2/tests/stream/hls/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/stream/hls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48313 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/stream/hls/test_hls.py
--rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/stream/hls/test_hls_filtered.py
--rw-r--r--   0 runner    (1001) docker     (127)    20206 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/stream/hls/test_m3u8.py
--rw-r--r--   0 runner    (1001) docker     (127)    18343 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/stream/test_ffmpegmux.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/stream/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/stream/test_segmented.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/stream/test_stream_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/stream/test_stream_to_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/stream/test_stream_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)    49553 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/test_api_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/test_api_websocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/test_buffers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    11028 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    18714 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/test_plugin_userinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/test_streamlink_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:35.014673 streamlink-6.7.2/tests/testutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/testutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/testutils/handshake.py
--rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/testutils/test_handshake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:35.014673 streamlink-6.7.2/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7616 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/utils/test_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/utils/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/utils/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/utils/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/utils/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/utils/test_l10n.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/utils/test_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/utils/test_named_pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/utils/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/utils/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/utils/test_processoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/utils/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     9308 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/utils/test_times.py
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/utils/test_url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:35.018673 streamlink-6.7.2/tests/webbrowser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/webbrowser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 12:22:35.018673 streamlink-6.7.2/tests/webbrowser/cdp/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/webbrowser/cdp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/webbrowser/cdp/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    39762 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/webbrowser/cdp/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    31342 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/webbrowser/cdp/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/webbrowser/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/webbrowser/test_chromium.py
--rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-03-23 12:22:01.000000 streamlink-6.7.2/tests/webbrowser/test_webbrowser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.296392 streamlink-6.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-14 15:40:22.000000 streamlink-6.7.3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)   100542 2024-04-14 15:40:22.000000 streamlink-6.7.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-14 15:40:22.000000 streamlink-6.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-14 15:40:22.000000 streamlink-6.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-14 15:40:52.296392 streamlink-6.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-14 15:40:22.000000 streamlink-6.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.204392 streamlink-6.7.3/build_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-14 15:40:22.000000 streamlink-6.7.3/build_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-14 15:40:22.000000 streamlink-6.7.3/build_backend/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-14 15:40:22.000000 streamlink-6.7.3/build_backend/onbuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15908 2024-04-14 15:40:22.000000 streamlink-6.7.3/build_backend/plugins_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-14 15:40:22.000000 streamlink-6.7.3/build_backend/test_build_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-14 15:40:22.000000 streamlink-6.7.3/build_backend/test_onbuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37280 2024-04-14 15:40:22.000000 streamlink-6.7.3/build_backend/test_plugins_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.196392 streamlink-6.7.3/completions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.204392 streamlink-6.7.3/completions/bash/
+-rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-04-14 15:40:47.000000 streamlink-6.7.3/completions/bash/streamlink
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.204392 streamlink-6.7.3/completions/zsh/
+-rw-r--r--   0 runner    (1001) docker     (127)    36671 2024-04-14 15:40:48.000000 streamlink-6.7.3/completions/zsh/_streamlink
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-14 15:40:22.000000 streamlink-6.7.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.208392 streamlink-6.7.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.196392 streamlink-6.7.3/docs/_build/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.208392 streamlink-6.7.3/docs/_build/man/
+-rw-r--r--   0 runner    (1001) docker     (127)    41171 2024-04-14 15:40:46.000000 streamlink-6.7.3/docs/_build/man/streamlink.1
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_man.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.212392 streamlink-6.7.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    12092 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_static/icon-ffmpeg.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_static/icon-python.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    18593 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_static/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15790 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_static/opengraph-image.png
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_static/site.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.212392 streamlink-6.7.3/docs/_static/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_static/styles/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.212392 streamlink-6.7.3/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_templates/page.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.212392 streamlink-6.7.3/docs/_templates/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_templates/sidebar/brand.html
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_templates/sidebar/github-buttons.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.212392 streamlink-6.7.3/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/api/cache.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/api/options.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/api/plugin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/api/session.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/api/stream.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/api/streamlink.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/api/validate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/api/webbrowser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.212392 streamlink-6.7.3/docs/api_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/api_guide/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    17250 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/api_guide/validate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/api_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/applications.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   100542 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.212392 streamlink-6.7.3/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/cli/config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/cli/metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/cli/plugin-sideloading.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.216392 streamlink-6.7.3/docs/cli/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/cli/plugins/crunchyroll.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10202 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/cli/plugins/twitch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/cli/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/cli/protocols.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/cli/proxy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/cli/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11426 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/deprecations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/docutils.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/donate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/ext_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/ext_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/ext_html_template_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/ext_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/ext_releaseref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    25334 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11739 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/migrations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/players.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/thirdparty.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18593 2024-04-14 15:40:22.000000 streamlink-6.7.3/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-14 15:40:52.300392 streamlink-6.7.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.216392 streamlink-6.7.3/script/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      802 2024-04-14 15:40:22.000000 streamlink-6.7.3/script/build-shell-completions.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 15:40:52.296392 streamlink-6.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-14 15:40:52.300392 streamlink-6.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.200392 streamlink-6.7.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.216392 streamlink-6.7.3/src/streamlink/
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-14 15:40:52.300392 streamlink-6.7.3/src/streamlink/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/buffers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8007 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.216392 streamlink-6.7.3/src/streamlink/packages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/packages/requests_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.216392 streamlink-6.7.3/src/streamlink/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.220392 streamlink-6.7.3/src/streamlink/plugin/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugin/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugin/api/http_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugin/api/useragents.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.220392 streamlink-6.7.3/src/streamlink/plugin/api/validate/
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugin/api/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugin/api/validate/_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugin/api/validate/_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11763 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugin/api/validate/_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19587 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugin/api/validate/_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugin/api/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26032 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.240392 streamlink-6.7.3/src/streamlink/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9677 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/abematv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/adultswim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/afreeca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/albavision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/aloula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/app17.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/ard_live.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/ard_mediathek.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/artetv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/atpchallenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/atresplayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/bbciplayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/bfmtv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/bigo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/bilibili.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/blazetv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/bloomberg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/booyah.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/brightcove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/btv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/cbsnews.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/cdnbg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7082 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/ceskatelevize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/cinergroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/clubbingtv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/cmmedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/cnews.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14036 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/crunchyroll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/dailymotion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/delfi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/deutschewelle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/dlive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/dogan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/dogus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/drdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/earthcam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/euronews.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/facebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8421 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/filmon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/galatasaraytv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/goltelevision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/goodgame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/googledrive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/gulli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/hiplayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/hls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/htv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/huajiao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/huya.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/idf1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/indihometv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/invintus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/kugou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/linelive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/livestream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/lnk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/lrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/ltv_lsm_lv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/mangomolo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/mdstrm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/mediaklikk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/mediavitrina.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/mildom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/mitele.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/mixcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/mjunoon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/mrtmk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/n13tv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/nasaplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/nhkworld.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10573 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/nicolive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/nimotv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/nos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/nownews.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/nowtvtr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/nrk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/okru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/olympicchannel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/oneplusone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/onetv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/openrectv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/pandalive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/piaulizaportal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/picarto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/piczel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/pixiv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/pluto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/pluzz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/radiko.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/radionet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/raiplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/reuters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/rtpa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/rtpplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/rtve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/rtvs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/ruv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/sbscokr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/showroom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/sportal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/sportschau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/ssh101.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/stadium.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/steam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/streamable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/streann.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/stv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/svtplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/swisstxt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/telefe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/telemadrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/tf1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/trovo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/turkuvaz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/tv360.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/tv3cat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/tv4play.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/tv5monde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/tv8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/tv999.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/tvibo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/tviplayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/tvp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/tvrby.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/tvrplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/tvtoya.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/twitcasting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33594 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/twitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19213 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/ustreamtv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/ustvnow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/vidio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/vimeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/vinhlongtv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/vk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/vkplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/vtvgo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/webtv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/welt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/wwenetwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15401 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/youtube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/yupptv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12860 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/zattoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/zdf_mediathek.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/zeenews.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/zengatv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/zhanqi.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.244392 streamlink-6.7.3/src/streamlink/session/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/session/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12151 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/session/http.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19101 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/session/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13238 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/session/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/session/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.244392 streamlink-6.7.3/src/streamlink/stream/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.244392 streamlink-6.7.3/src/streamlink/stream/dash/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/dash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14067 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/dash/dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36858 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/dash/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/dash/segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/ffmpegmux.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/filtered.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.244392 streamlink-6.7.3/src/streamlink/stream/hls/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/hls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33983 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/hls/hls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21481 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/hls/m3u8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/hls/segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.244392 streamlink-6.7.3/src/streamlink/stream/segmented/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/segmented/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/segmented/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/segmented/segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8118 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/segmented/segmented.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/user_input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.248392 streamlink-6.7.3/src/streamlink/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/l10n.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/named_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/processoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/times.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.248392 streamlink-6.7.3/src/streamlink/webbrowser/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.248392 streamlink-6.7.3/src/streamlink/webbrowser/cdp/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13939 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.252392 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21632 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49407 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61679 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/dom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26084 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/emulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19534 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27632 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/input_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)   130706 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)   107521 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62110 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17300 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24082 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/target.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8564 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/chromium.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/webbrowser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.296392 streamlink-6.7.3/src/streamlink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-14 15:40:52.000000 streamlink-6.7.3/src/streamlink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19654 2024-04-14 15:40:52.000000 streamlink-6.7.3/src/streamlink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 15:40:52.000000 streamlink-6.7.3/src/streamlink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-14 15:40:52.000000 streamlink-6.7.3/src/streamlink.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-14 15:40:52.000000 streamlink-6.7.3/src/streamlink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-14 15:40:52.000000 streamlink-6.7.3/src/streamlink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.252392 streamlink-6.7.3/src/streamlink_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49425 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31969 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.256392 streamlink-6.7.3/src/streamlink_cli/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/output/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/output/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/output/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/output/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/streamrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.256392 streamlink-6.7.3/src/streamlink_cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/utils/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/utils/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/utils/versioncheck.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.256392 streamlink-6.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.260392 streamlink-6.7.3/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.260392 streamlink-6.7.3/tests/cli/output/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/output/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13144 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/output/test_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/test_argparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/test_cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/test_cmdline_title.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18037 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/test_main_check_file_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/test_main_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16038 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/test_main_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/test_main_setup_config_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/test_plugin_args_and_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23211 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/test_streamrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.260392 streamlink-6.7.3/tests/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/utils/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/utils/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/utils/test_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15076 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/utils/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/utils/test_versioncheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.260392 streamlink-6.7.3/tests/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/mixins/stream_hls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.260392 streamlink-6.7.3/tests/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.260392 streamlink-6.7.3/tests/plugin/override/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugin/override/testplugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugin/testplugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugin/testplugin_invalid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugin/testplugin_missing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.284392 streamlink-6.7.3/tests/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_abematv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_adultswim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_afreeca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_albavision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_aloula.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_app17.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_ard_live.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_ard_mediathek.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_artetv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_atpchallenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_atresplayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_bbciplayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_bfmtv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_bigo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_bilibili.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_blazetv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_bloomberg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_booyah.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_brightcove.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_btv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_cbsnews.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_cdnbg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_ceskatelevize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_cinergroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_clubbingtv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_cmmedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_cnews.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_crunchyroll.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_dailymotion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_delfi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_deutschewelle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_dlive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_dogan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_dogus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_drdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_earthcam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_euronews.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_facebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_filmon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_galatasaraytv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_goltelevision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_goodgame.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_googledrive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_gulli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_hiplayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_hls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_htv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_huajiao.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_huya.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_idf1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_indihometv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_invintus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_kugou.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_linelive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_livestream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_lnk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_lrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_ltv_lsm_lv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_mangomolo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_mdstrm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_mediaklikk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_mediavitrina.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_mildom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_mitele.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_mixcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_mjunoon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_mrtmk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_n13tv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_nasaplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_nhkworld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_nicolive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_nimotv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_nos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_nownews.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_nowtvtr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_nrk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_okru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_olympicchannel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_oneplusone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_onetv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_openrectv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_pandalive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_piaulizaportal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_picarto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_piczel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_pixiv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_pluto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_pluzz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_radiko.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_radionet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_raiplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_reuters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_rtpa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_rtpplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_rtve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_rtvs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_ruv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_sbscokr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_showroom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_sportal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_sportschau.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_ssh101.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_stadium.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_steam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_streamable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_streann.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_stv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_svtplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_swisstxt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_telefe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_telemadrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_tf1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_trovo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_turkuvaz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_tv360.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_tv3cat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_tv4play.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_tv5monde.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_tv8.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_tv999.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_tvibo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_tviplayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_tvp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_tvrby.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_tvrplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_tvtoya.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_twitcasting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35577 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_twitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_ustreamtv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_ustvnow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_vidio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_vimeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_vinhlongtv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_vk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_vkplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_vtvgo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_webtv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_welt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_wwenetwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_youtube.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_yupptv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_zattoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_zdf_mediathek.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_zeenews.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_zengatv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_zhanqi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.284392 streamlink-6.7.3/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.200392 streamlink-6.7.3/tests/resources/cli/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.284392 streamlink-6.7.3/tests/resources/cli/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/cli/config/custom
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/cli/config/primary
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/cli/config/primary.testplugin
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/cli/config/secondary
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/cli/config/secondary.testplugin
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.288392 streamlink-6.7.3/tests/resources/dash/
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_1.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_10.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     9187 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_11_static.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_2.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_3.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_8.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_9.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_dynamic_segment_list_no_duration.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_dynamic_segment_list_p1.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_dynamic_segment_list_p2.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_dynamic_segment_list_p3.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_dynamic_segment_list_p4.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_dynamic_segment_list_p5.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_dynamic_timeline_continued_p1.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_dynamic_timeline_continued_p2.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_nested_baseurls.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_no_segment_list_or_template.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_segment_list.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_segments_byterange.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_segments_dynamic_number.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_static_no_publish_time.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_suggested_presentation_delay.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_timeline_ids.mpd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.288392 streamlink-6.7.3/tests/resources/hls/
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/hls/test_1.m3u8
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/hls/test_2.m3u8
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/hls/test_date.m3u8
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/hls/test_master.m3u8
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/hls/test_master_twitch_vod.m3u8
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/hls/test_multivariant_bandwidth.m3u8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.292392 streamlink-6.7.3/tests/session/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/session/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/session/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23380 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/session/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/session/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.292392 streamlink-6.7.3/tests/stream/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/stream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.292392 streamlink-6.7.3/tests/stream/dash/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/stream/dash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21720 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/stream/dash/test_dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29634 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/stream/dash/test_manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.292392 streamlink-6.7.3/tests/stream/hls/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/stream/hls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48313 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/stream/hls/test_hls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/stream/hls/test_hls_filtered.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20206 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/stream/hls/test_m3u8.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18343 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/stream/test_ffmpegmux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/stream/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/stream/test_segmented.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/stream/test_stream_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/stream/test_stream_to_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/stream/test_stream_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49815 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/test_api_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/test_api_websocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/test_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11028 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18714 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/test_plugin_userinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/test_streamlink_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.292392 streamlink-6.7.3/tests/testutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/testutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/testutils/handshake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/testutils/test_handshake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.296392 streamlink-6.7.3/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7616 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/test_l10n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/test_named_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/test_processoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9308 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/test_times.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/test_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.296392 streamlink-6.7.3/tests/webbrowser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/webbrowser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.296392 streamlink-6.7.3/tests/webbrowser/cdp/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/webbrowser/cdp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/webbrowser/cdp/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39762 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/webbrowser/cdp/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31342 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/webbrowser/cdp/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/webbrowser/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/webbrowser/test_chromium.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6889 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/webbrowser/test_webbrowser.py
```

### Comparing `streamlink-6.7.2/CHANGELOG.md` & `streamlink-6.7.3/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,27 @@
 # Changelog
 
+## streamlink 6.7.3 (2024-04-14)
+
+Patch release:
+
+- Fixed: file output paths being able to exceed max file/directory name length ([#5921](https://github.com/streamlink/streamlink/pull/5921), [#5925](https://github.com/streamlink/streamlink/pull/5925))
+- Fixed: propagation of `KeyboardInterrupt`/`SystemExit` in `streamlink.webbrowser` ([#5930](https://github.com/streamlink/streamlink/pull/5930))
+- Fixed: compatibility with `exceptiongroup<=1.1.1` ([#5930](https://github.com/streamlink/streamlink/pull/5930))
+- Fixed: `plugin.api.validate.parse_qsd` input type validation ([#5932](https://github.com/streamlink/streamlink/pull/5932))
+- Updated plugins:
+  - mangomolo: fixed missing referer header and updated URL matcher ([#5923](https://github.com/streamlink/streamlink/pull/5923), [#5926](https://github.com/streamlink/streamlink/pull/5926))
+  - pluto: rewritten plugin ([#5910](https://github.com/streamlink/streamlink/pull/5910))
+  - showroom: fixed geo-block check preventing stream access ([#5911](https://github.com/streamlink/streamlink/pull/5911))
+  - vkplay: updated URL matcher ([#5908](https://github.com/streamlink/streamlink/pull/5908))
+- Tests: fixed test failure when running tests from the `bdist` build directory ([#5933](https://github.com/streamlink/streamlink/pull/5933))
+
+[Full changelog](https://github.com/streamlink/streamlink/compare/6.7.2...6.7.3)
+
+
 ## streamlink 6.7.2 (2024-03-23)
 
 Patch release:
 
 - Build: reverted `trio` version requirement bump ([#5902](https://github.com/streamlink/streamlink/pull/5902))
 - Build: fixed incorrect `pytest` version requirement ([#5901](https://github.com/streamlink/streamlink/pull/5901))
```

### Comparing `streamlink-6.7.2/LICENSE` & `streamlink-6.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/PKG-INFO` & `streamlink-6.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlink
-Version: 6.7.2
+Version: 6.7.3
 Summary: Streamlink is a command-line utility that extracts streams from various services and pipes them into a video player of choice.
 Author: Streamlink
 Author-email: streamlink@protonmail.com
 License: Simplified BSD
 Project-URL: Homepage, https://github.com/streamlink/streamlink
 Project-URL: Documentation, https://streamlink.github.io/
 Project-URL: Tracker, https://github.com/streamlink/streamlink/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: streamlink Version: 6.7.2 Summary: Streamlink is a
+Metadata-Version: 2.1 Name: streamlink Version: 6.7.3 Summary: Streamlink is a
 command-line utility that extracts streams from various services and pipes them
 into a video player of choice. Author: Streamlink Author-email:
 streamlink@protonmail.com License: Simplified BSD Project-URL: Homepage, https:
 //github.com/streamlink/streamlink Project-URL: Documentation, https://
 streamlink.github.io/ Project-URL: Tracker, https://github.com/streamlink/
 streamlink/issues Project-URL: Source, https://github.com/streamlink/streamlink
 Project-URL: Funding, https://streamlink.github.io/latest/donate.html
```

### Comparing `streamlink-6.7.2/README.md` & `streamlink-6.7.3/README.md`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/build_backend/__init__.py` & `streamlink-6.7.3/build_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/build_backend/commands.py` & `streamlink-6.7.3/build_backend/commands.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/build_backend/onbuild.py` & `streamlink-6.7.3/build_backend/onbuild.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/build_backend/plugins_json.py` & `streamlink-6.7.3/build_backend/plugins_json.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/build_backend/test_build_backend.py` & `streamlink-6.7.3/build_backend/test_build_backend.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/build_backend/test_onbuild.py` & `streamlink-6.7.3/build_backend/test_onbuild.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,21 @@
     param = getattr(request, "param", {})
     is_source = param.get("is_source", True)
     pkg_dir = tmp_path / "src" if is_source else tmp_path
 
     (pkg_dir / "streamlink").mkdir(parents=True)
     shutil.copy(PROJECT_ROOT / "pyproject.toml", tmp_path / "pyproject.toml")
     shutil.copy(PROJECT_ROOT / "setup.py", tmp_path / "setup.py")
-    shutil.copy(PROJECT_ROOT / "src" / "streamlink" / "_version.py", pkg_dir / "streamlink" / "_version.py")
+
+    # Lookup for the path from the root source directory
+    if Path(PROJECT_ROOT / "src" / "streamlink" / "_version.py").exists():
+        shutil.copy(PROJECT_ROOT / "src" / "streamlink" / "_version.py", pkg_dir / "streamlink" / "_version.py")
+    else:  # pragma: no cover
+        # We didn't find it, use the build location
+        shutil.copy(PROJECT_ROOT / "streamlink" / "_version.py", pkg_dir / "streamlink" / "_version.py")
 
     options = dict(
         is_source=is_source,
         template_fields=template_fields,
         params={},
     )
     if _HAS_ONBUILD_FILE_PROVIDER:
```

### Comparing `streamlink-6.7.2/build_backend/test_plugins_json.py` & `streamlink-6.7.3/build_backend/test_plugins_json.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/completions/bash/streamlink` & `streamlink-6.7.3/completions/bash/streamlink`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/completions/zsh/_streamlink` & `streamlink-6.7.3/completions/zsh/_streamlink`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/Makefile` & `streamlink-6.7.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/_build/man/streamlink.1` & `streamlink-6.7.3/docs/_build/man/streamlink.1`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "STREAMLINK" "1" "Mar 23, 2024" "6.7.2" "Streamlink"
+.TH "STREAMLINK" "1" "Apr 14, 2024" "6.7.3" "Streamlink"
 .SH NAME
 streamlink \- extracts streams from various services and pipes them into a video player of choice
 .SH SYNOPSIS
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
```

### Comparing `streamlink-6.7.2/docs/_man.rst` & `streamlink-6.7.3/docs/_man.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/_static/apple-touch-icon.png` & `streamlink-6.7.3/docs/_static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/_static/favicon-16x16.png` & `streamlink-6.7.3/docs/_static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/_static/favicon-32x32.png` & `streamlink-6.7.3/docs/_static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/_static/favicon.ico` & `streamlink-6.7.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/_static/icon-ffmpeg.svg` & `streamlink-6.7.3/docs/_static/icon-ffmpeg.svg`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/_static/icon-python.svg` & `streamlink-6.7.3/docs/_static/icon-python.svg`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/_static/icon.svg` & `streamlink-6.7.3/docs/_static/icon.svg`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/_static/opengraph-image.png` & `streamlink-6.7.3/docs/_static/opengraph-image.png`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/_static/styles/custom.css` & `streamlink-6.7.3/docs/_static/styles/custom.css`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/_templates/base.html` & `streamlink-6.7.3/docs/_templates/base.html`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/_templates/sidebar/brand.html` & `streamlink-6.7.3/docs/_templates/sidebar/brand.html`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/_templates/sidebar/github-buttons.html` & `streamlink-6.7.3/docs/_templates/sidebar/github-buttons.html`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/api/validate.rst` & `streamlink-6.7.3/docs/api/validate.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/api/webbrowser.rst` & `streamlink-6.7.3/docs/api/webbrowser.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/api_guide/quickstart.rst` & `streamlink-6.7.3/docs/api_guide/quickstart.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/api_guide/validate.rst` & `streamlink-6.7.3/docs/api_guide/validate.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/applications.rst` & `streamlink-6.7.3/docs/applications.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/changelog.md` & `streamlink-6.7.3/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,27 @@
 # Changelog
 
+## streamlink 6.7.3 (2024-04-14)
+
+Patch release:
+
+- Fixed: file output paths being able to exceed max file/directory name length ([#5921](https://github.com/streamlink/streamlink/pull/5921), [#5925](https://github.com/streamlink/streamlink/pull/5925))
+- Fixed: propagation of `KeyboardInterrupt`/`SystemExit` in `streamlink.webbrowser` ([#5930](https://github.com/streamlink/streamlink/pull/5930))
+- Fixed: compatibility with `exceptiongroup<=1.1.1` ([#5930](https://github.com/streamlink/streamlink/pull/5930))
+- Fixed: `plugin.api.validate.parse_qsd` input type validation ([#5932](https://github.com/streamlink/streamlink/pull/5932))
+- Updated plugins:
+  - mangomolo: fixed missing referer header and updated URL matcher ([#5923](https://github.com/streamlink/streamlink/pull/5923), [#5926](https://github.com/streamlink/streamlink/pull/5926))
+  - pluto: rewritten plugin ([#5910](https://github.com/streamlink/streamlink/pull/5910))
+  - showroom: fixed geo-block check preventing stream access ([#5911](https://github.com/streamlink/streamlink/pull/5911))
+  - vkplay: updated URL matcher ([#5908](https://github.com/streamlink/streamlink/pull/5908))
+- Tests: fixed test failure when running tests from the `bdist` build directory ([#5933](https://github.com/streamlink/streamlink/pull/5933))
+
+[Full changelog](https://github.com/streamlink/streamlink/compare/6.7.2...6.7.3)
+
+
 ## streamlink 6.7.2 (2024-03-23)
 
 Patch release:
 
 - Build: reverted `trio` version requirement bump ([#5902](https://github.com/streamlink/streamlink/pull/5902))
 - Build: fixed incorrect `pytest` version requirement ([#5901](https://github.com/streamlink/streamlink/pull/5901))
```

### Comparing `streamlink-6.7.2/docs/cli/config.rst` & `streamlink-6.7.3/docs/cli/config.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/cli/metadata.rst` & `streamlink-6.7.3/docs/cli/metadata.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/cli/plugin-sideloading.rst` & `streamlink-6.7.3/docs/cli/plugin-sideloading.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/cli/plugins/crunchyroll.rst` & `streamlink-6.7.3/docs/cli/plugins/crunchyroll.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/cli/plugins/twitch.rst` & `streamlink-6.7.3/docs/cli/plugins/twitch.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/cli/protocols.rst` & `streamlink-6.7.3/docs/cli/protocols.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/cli/proxy.rst` & `streamlink-6.7.3/docs/cli/proxy.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/cli/tutorial.rst` & `streamlink-6.7.3/docs/cli/tutorial.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/cli.rst` & `streamlink-6.7.3/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/conf.py` & `streamlink-6.7.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/deprecations.rst` & `streamlink-6.7.3/docs/deprecations.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/developing.rst` & `streamlink-6.7.3/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/donate.rst` & `streamlink-6.7.3/docs/donate.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/ext_argparse.py` & `streamlink-6.7.3/docs/ext_argparse.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/ext_github.py` & `streamlink-6.7.3/docs/ext_github.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/ext_plugins.py` & `streamlink-6.7.3/docs/ext_plugins.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/ext_releaseref.py` & `streamlink-6.7.3/docs/ext_releaseref.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/index.rst` & `streamlink-6.7.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/install.rst` & `streamlink-6.7.3/docs/install.rst`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,15 @@
       - Sebastian Meyer <mail at bastimeyer.de>
 
 
 Package availability
 --------------------
 
 Packaging is not done by the Streamlink maintainers themselves except for
-the `PyPI package <PyPI package and source code_>`_,
+the `PyPI package <pypi-package-and-source-code_>`_,
 the `Windows installers + portable builds <Windows binaries_>`_,
 and the `Linux AppImages <Linux AppImages_>`_.
 
 If a packaged release of Streamlink is not available for your operating system / distro or your system's architecture,
 or if it's out of date or broken, then please contact the respective package maintainers or package-repository maintainers
 of your operating system / distro, as it's up to them to add, update, or fix those packages.
```

### Comparing `streamlink-6.7.2/docs/migrations.rst` & `streamlink-6.7.3/docs/migrations.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/players.rst` & `streamlink-6.7.3/docs/players.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/plugins.rst` & `streamlink-6.7.3/docs/plugins.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/docs/thirdparty.rst` & `streamlink-6.7.3/docs/thirdparty.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/icon.svg` & `streamlink-6.7.3/icon.svg`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/pyproject.toml` & `streamlink-6.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/script/build-shell-completions.sh` & `streamlink-6.7.3/script/build-shell-completions.sh`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/setup.py` & `streamlink-6.7.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,9 +86,9 @@
         def get_cmdclasses(_):  # type: ignore[misc]
             return _
 
     setup(
         cmdclass=get_cmdclasses(cmdclass),
         entry_points=entry_points,
         data_files=data_files,
-        version="6.7.2",
+        version="6.7.3",
     )
```

### Comparing `streamlink-6.7.2/src/streamlink/__init__.py` & `streamlink-6.7.3/src/streamlink/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/api.py` & `streamlink-6.7.3/src/streamlink/api.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/buffers.py` & `streamlink-6.7.3/src/streamlink/buffers.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/cache.py` & `streamlink-6.7.3/src/streamlink/cache.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/compat.py` & `streamlink-6.7.3/src/streamlink/compat.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/exceptions.py` & `streamlink-6.7.3/src/streamlink/exceptions.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/logger.py` & `streamlink-6.7.3/src/streamlink/logger.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/options.py` & `streamlink-6.7.3/src/streamlink/options.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/packages/requests_file.py` & `streamlink-6.7.3/src/streamlink/packages/requests_file.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugin/__init__.py` & `streamlink-6.7.3/src/streamlink/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugin/api/useragents.py` & `streamlink-6.7.3/src/streamlink/plugin/api/useragents.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-ANDROID = "Mozilla/5.0 (Linux; Android 14) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/122.0.6261.90 Mobile Safari/537.36"
-CHROME = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/122.0.0.0 Safari/537.36"
+ANDROID = "Mozilla/5.0 (Linux; Android 14) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.6312.80 Mobile Safari/537.36"
+CHROME = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36"
 CHROME_OS = "Mozilla/5.0 (X11; CrOS x86_64 15633.69.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/119.0.6045.212 Safari/537.36"
-FIREFOX = "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:123.0) Gecko/20100101 Firefox/123.0"
+FIREFOX = "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:124.0) Gecko/20100101 Firefox/124.0"
 IE_11 = "Mozilla/5.0 (Windows NT 10.0; WOW64; Trident/7.0; rv:11.0) like Gecko"
-IPHONE = "Mozilla/5.0 (iPhone; CPU iPhone OS 17_3_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.3.1 Mobile/15E148 Safari/604.1"
-OPERA = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/122.0.0.0 Safari/537.36 OPR/108.0.0.0"
-SAFARI = "Mozilla/5.0 (Macintosh; Intel Mac OS X 14_3_1) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.3.1 Safari/605.1.15"
+IPHONE = "Mozilla/5.0 (iPhone; CPU iPhone OS 17_4_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.3.1 Mobile/15E148 Safari/604.1"
+OPERA = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36 OPR/109.0.0.0"
+SAFARI = "Mozilla/5.0 (Macintosh; Intel Mac OS X 14_4_1) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.3.1 Safari/605.1.15"
 
 # Backwards compatibility
 EDGE = CHROME
 FIREFOX_MAC = FIREFOX
 IE_6 = IE_7 = IE_8 = IE_9 = IE_11
 IPHONE_6 = IPAD = IPHONE
 SAFARI_7 = SAFARI_8 = SAFARI
```

### Comparing `streamlink-6.7.2/src/streamlink/plugin/api/validate/__init__.py` & `streamlink-6.7.3/src/streamlink/plugin/api/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugin/api/validate/_exception.py` & `streamlink-6.7.3/src/streamlink/plugin/api/validate/_exception.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugin/api/validate/_schemas.py` & `streamlink-6.7.3/src/streamlink/plugin/api/validate/_schemas.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugin/api/validate/_validate.py` & `streamlink-6.7.3/src/streamlink/plugin/api/validate/_validate.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugin/api/validate/_validators.py` & `streamlink-6.7.3/src/streamlink/plugin/api/validate/_validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -647,8 +647,12 @@
         )
         assert schema.validate("a=b&a=c&foo=bar") == {"a": "c", "foo": "bar"}
         schema.validate(123)  # raises ValidationError
 
     :raise ValidationError: On parsing error
     """
 
-    return TransformSchema(_parse_qsd, *args, **kwargs, exception=ValidationError, schema=None)
+    def parser(*_args, **_kwargs):
+        validate(AnySchema(str, bytes), _args[0])
+        return _parse_qsd(*_args, **_kwargs, exception=ValidationError, schema=None)
+
+    return TransformSchema(parser, *args, **kwargs)
```

### Comparing `streamlink-6.7.2/src/streamlink/plugin/api/websocket.py` & `streamlink-6.7.3/src/streamlink/plugin/api/websocket.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugin/plugin.py` & `streamlink-6.7.3/src/streamlink/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/abematv.py` & `streamlink-6.7.3/src/streamlink/plugins/abematv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/adultswim.py` & `streamlink-6.7.3/src/streamlink/plugins/adultswim.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/afreeca.py` & `streamlink-6.7.3/src/streamlink/plugins/afreeca.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/albavision.py` & `streamlink-6.7.3/src/streamlink/plugins/albavision.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/aloula.py` & `streamlink-6.7.3/src/streamlink/plugins/aloula.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/app17.py` & `streamlink-6.7.3/src/streamlink/plugins/app17.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/ard_live.py` & `streamlink-6.7.3/src/streamlink/plugins/ard_live.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/ard_mediathek.py` & `streamlink-6.7.3/src/streamlink/plugins/ard_mediathek.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/artetv.py` & `streamlink-6.7.3/src/streamlink/plugins/artetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/atpchallenger.py` & `streamlink-6.7.3/src/streamlink/plugins/atpchallenger.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/atresplayer.py` & `streamlink-6.7.3/src/streamlink/plugins/atresplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/bbciplayer.py` & `streamlink-6.7.3/src/streamlink/plugins/bbciplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/bfmtv.py` & `streamlink-6.7.3/src/streamlink/plugins/bfmtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/bigo.py` & `streamlink-6.7.3/src/streamlink/plugins/bigo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/bilibili.py` & `streamlink-6.7.3/src/streamlink/plugins/bilibili.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/blazetv.py` & `streamlink-6.7.3/src/streamlink/plugins/blazetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/bloomberg.py` & `streamlink-6.7.3/src/streamlink/plugins/bloomberg.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/booyah.py` & `streamlink-6.7.3/src/streamlink/plugins/booyah.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/brightcove.py` & `streamlink-6.7.3/src/streamlink/plugins/brightcove.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/btv.py` & `streamlink-6.7.3/src/streamlink/plugins/btv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/cbsnews.py` & `streamlink-6.7.3/src/streamlink/plugins/cbsnews.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/cdnbg.py` & `streamlink-6.7.3/src/streamlink/plugins/cdnbg.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/ceskatelevize.py` & `streamlink-6.7.3/src/streamlink/plugins/ceskatelevize.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/cinergroup.py` & `streamlink-6.7.3/src/streamlink/plugins/cinergroup.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/clubbingtv.py` & `streamlink-6.7.3/src/streamlink/plugins/clubbingtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/cmmedia.py` & `streamlink-6.7.3/src/streamlink/plugins/cmmedia.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/cnews.py` & `streamlink-6.7.3/src/streamlink/plugins/cnews.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/crunchyroll.py` & `streamlink-6.7.3/src/streamlink/plugins/crunchyroll.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/dailymotion.py` & `streamlink-6.7.3/src/streamlink/plugins/dailymotion.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/dash.py` & `streamlink-6.7.3/src/streamlink/plugins/dash.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/delfi.py` & `streamlink-6.7.3/src/streamlink/plugins/delfi.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/deutschewelle.py` & `streamlink-6.7.3/src/streamlink/plugins/deutschewelle.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/dlive.py` & `streamlink-6.7.3/src/streamlink/plugins/dlive.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/dogan.py` & `streamlink-6.7.3/src/streamlink/plugins/dogan.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/dogus.py` & `streamlink-6.7.3/src/streamlink/plugins/dogus.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/drdk.py` & `streamlink-6.7.3/src/streamlink/plugins/drdk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/earthcam.py` & `streamlink-6.7.3/src/streamlink/plugins/earthcam.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/euronews.py` & `streamlink-6.7.3/src/streamlink/plugins/euronews.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/facebook.py` & `streamlink-6.7.3/src/streamlink/plugins/facebook.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/filmon.py` & `streamlink-6.7.3/src/streamlink/plugins/filmon.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/galatasaraytv.py` & `streamlink-6.7.3/src/streamlink/plugins/galatasaraytv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/goltelevision.py` & `streamlink-6.7.3/src/streamlink/plugins/goltelevision.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/goodgame.py` & `streamlink-6.7.3/src/streamlink/plugins/goodgame.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/googledrive.py` & `streamlink-6.7.3/src/streamlink/plugins/googledrive.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/gulli.py` & `streamlink-6.7.3/src/streamlink/plugins/gulli.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/hiplayer.py` & `streamlink-6.7.3/src/streamlink/plugins/hiplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/hls.py` & `streamlink-6.7.3/src/streamlink/plugins/hls.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/http.py` & `streamlink-6.7.3/src/streamlink/plugins/http.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/htv.py` & `streamlink-6.7.3/src/streamlink/plugins/htv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/huajiao.py` & `streamlink-6.7.3/src/streamlink/plugins/huajiao.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/huya.py` & `streamlink-6.7.3/src/streamlink/plugins/huya.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/idf1.py` & `streamlink-6.7.3/src/streamlink/plugins/idf1.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/indihometv.py` & `streamlink-6.7.3/src/streamlink/plugins/indihometv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/invintus.py` & `streamlink-6.7.3/src/streamlink/plugins/invintus.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/kugou.py` & `streamlink-6.7.3/src/streamlink/plugins/kugou.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/linelive.py` & `streamlink-6.7.3/src/streamlink/plugins/linelive.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/livestream.py` & `streamlink-6.7.3/src/streamlink/plugins/livestream.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/lnk.py` & `streamlink-6.7.3/src/streamlink/plugins/lnk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/lrt.py` & `streamlink-6.7.3/src/streamlink/plugins/lrt.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/ltv_lsm_lv.py` & `streamlink-6.7.3/src/streamlink/plugins/ltv_lsm_lv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/mangomolo.py` & `streamlink-6.7.3/src/streamlink/plugins/mangomolo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
 $description OTT video platform owned by Alpha Technology Group
+$url player.mangomolo.com
 $url media.gov.kw
 $type live
 """
 
 import logging
 import re
 
@@ -19,33 +20,35 @@
 
 @pluginmatcher(
     name="mangomoloplayer",
     pattern=re.compile(r"https?://player\.mangomolo\.com/v1/"),
 )
 @pluginmatcher(
     name="mediagovkw",
-    pattern=re.compile(r"https?://media\.gov\.kw/"),
+    pattern=re.compile(r"https?://(www\.)?media\.gov\.kw/"),
 )
 class Mangomolo(Plugin):
     def _get_player_url(self):
         player_url = self.session.http.get(self.url, schema=validate.Schema(
             validate.parse_html(),
             validate.xml_xpath_string(".//iframe[contains(@src,'//player.mangomolo.com/v1/')][1]/@src"),
         ))
         if not player_url:
             log.error("Could not find embedded player")
             raise NoStreamsError
 
         self.url = update_scheme("https://", player_url)
 
     def _get_streams(self):
+        headers = {}
         if not self.matches["mangomoloplayer"]:
+            headers["Referer"] = self.url
             self._get_player_url()
 
-        hls_url = self.session.http.get(self.url, schema=validate.Schema(
+        hls_url = self.session.http.get(self.url, headers=headers, schema=validate.Schema(
             re.compile(r"src\s*:\s*(?P<q>[\"'])(?P<url>https?://\S+?\.m3u8\S*?)(?P=q)"),
             validate.none_or_all(validate.get("url")),
         ))
         if hls_url:
             return HLSStream.parse_variant_playlist(self.session, hls_url)
```

### Comparing `streamlink-6.7.2/src/streamlink/plugins/mdstrm.py` & `streamlink-6.7.3/src/streamlink/plugins/mdstrm.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/mediaklikk.py` & `streamlink-6.7.3/src/streamlink/plugins/mediaklikk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/mediavitrina.py` & `streamlink-6.7.3/src/streamlink/plugins/mediavitrina.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/mildom.py` & `streamlink-6.7.3/src/streamlink/plugins/mildom.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/mitele.py` & `streamlink-6.7.3/src/streamlink/plugins/mitele.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/mixcloud.py` & `streamlink-6.7.3/src/streamlink/plugins/mixcloud.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/mjunoon.py` & `streamlink-6.7.3/src/streamlink/plugins/mjunoon.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/mrtmk.py` & `streamlink-6.7.3/src/streamlink/plugins/mrtmk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/n13tv.py` & `streamlink-6.7.3/src/streamlink/plugins/n13tv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/nasaplus.py` & `streamlink-6.7.3/src/streamlink/plugins/nasaplus.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/nhkworld.py` & `streamlink-6.7.3/src/streamlink/plugins/nhkworld.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/nicolive.py` & `streamlink-6.7.3/src/streamlink/plugins/nicolive.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/nimotv.py` & `streamlink-6.7.3/src/streamlink/plugins/nimotv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/nos.py` & `streamlink-6.7.3/src/streamlink/plugins/nos.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/nownews.py` & `streamlink-6.7.3/src/streamlink/plugins/nownews.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/nowtvtr.py` & `streamlink-6.7.3/src/streamlink/plugins/nowtvtr.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/nrk.py` & `streamlink-6.7.3/src/streamlink/plugins/nrk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/okru.py` & `streamlink-6.7.3/src/streamlink/plugins/okru.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/olympicchannel.py` & `streamlink-6.7.3/src/streamlink/plugins/olympicchannel.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/oneplusone.py` & `streamlink-6.7.3/src/streamlink/plugins/oneplusone.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/onetv.py` & `streamlink-6.7.3/src/streamlink/plugins/onetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/openrectv.py` & `streamlink-6.7.3/src/streamlink/plugins/openrectv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/pandalive.py` & `streamlink-6.7.3/src/streamlink/plugins/pandalive.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/piaulizaportal.py` & `streamlink-6.7.3/src/streamlink/plugins/piaulizaportal.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/picarto.py` & `streamlink-6.7.3/src/streamlink/plugins/picarto.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/piczel.py` & `streamlink-6.7.3/src/streamlink/plugins/piczel.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/pixiv.py` & `streamlink-6.7.3/src/streamlink/plugins/pixiv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/pluto.py` & `streamlink-6.7.3/src/streamlink/plugins/pluto.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,181 +9,222 @@
 """
 
 import logging
 import re
 from urllib.parse import parse_qsl, urljoin
 from uuid import uuid4
 
+from streamlink.exceptions import PluginError
 from streamlink.plugin import Plugin, pluginmatcher
-from streamlink.plugin.api import validate
+from streamlink.plugin.api import useragents, validate
 from streamlink.stream.hls import HLSStream, HLSStreamReader, HLSStreamWriter
 from streamlink.utils.url import update_qsd
 
 
 log = logging.getLogger(__name__)
 
 
 class PlutoHLSStreamWriter(HLSStreamWriter):
-    ad_re = re.compile(r"_ad/creative/|dai\.google\.com|Pluto_TV_OandO/.*(Bumper|plutotv_filler)")
+    ad_re = re.compile(r"_ad/creative/|creative/\d+_ad/|dai\.google\.com|Pluto_TV_OandO/.*(Bumper|plutotv_filler)")
 
     def should_filter_segment(self, segment):
         return self.ad_re.search(segment.uri) is not None or super().should_filter_segment(segment)
 
 
 class PlutoHLSStreamReader(HLSStreamReader):
     __writer__ = PlutoHLSStreamWriter
 
 
 class PlutoHLSStream(HLSStream):
     __shortname__ = "hls-pluto"
     __reader__ = PlutoHLSStreamReader
 
 
-@pluginmatcher(re.compile(r"""
-    https?://(?:www\.)?pluto\.tv/(?:\w{2}/)?(?:
-        live-tv/(?P<slug_live>[^/]+)
-        |
-        on-demand/series/(?P<slug_series>[^/]+)(?:/season/\d+)?/episode/(?P<slug_episode>[^/]+)
-        |
-        on-demand/movies/(?P<slug_movies>[^/]+)
-    )/?$
-""", re.VERBOSE))
+@pluginmatcher(
+    name="live",
+    pattern=re.compile(
+        r"https?://(?:www\.)?pluto\.tv/(?:\w{2}/)?live-tv/(?P<id>[^/]+)/?$",
+    ),
+)
+@pluginmatcher(
+    name="series",
+    pattern=re.compile(
+        r"https?://(?:www\.)?pluto\.tv/(?:\w{2}/)?on-demand/series/(?P<id_s>[^/]+)(?:/season/\d+)?/episode/(?P<id_e>[^/]+)/?$",
+    ),
+)
+@pluginmatcher(
+    name="movies",
+    pattern=re.compile(
+        r"https?://(?:www\.)?pluto\.tv/(?:\w{2}/)?on-demand/movies/(?P<id>[^/]+)/?$",
+    ),
+)
 class Pluto(Plugin):
-    def _get_api_data(self, kind, slug, slugfilter=None):
-        log.debug(f"slug={slug}")
-        app_version = self.session.http.get(self.url, schema=validate.Schema(
-            validate.parse_html(),
-            validate.xml_xpath_string(".//head/meta[@name='appVersion']/@content"),
-            validate.any(None, str),
-        ))
-        if not app_version:
-            return
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.session.http.headers.update({"User-Agent": useragents.FIREFOX})
+        self._app_version = None
+        self._device_version = re.search(r"Firefox/(\d+(?:\.\d+)*)", useragents.FIREFOX)[1]
+        self._client_id = str(uuid4())
+
+    @property
+    def app_version(self):
+        if self._app_version:
+            return self._app_version
 
-        log.debug(f"app_version={app_version}")
+        self._app_version = self.session.http.get(
+            self.url,
+            schema=validate.Schema(
+                validate.parse_html(),
+                validate.xml_xpath_string(".//head/meta[@name='appVersion']/@content"),
+                validate.any(None, str),
+            ),
+        )
+        if not self._app_version:
+            raise PluginError("Could not find pluto app version")
+
+        log.debug(f"{self._app_version=}")
+
+        return self._app_version
+
+    def _get_api_data(self, request):
+        log.debug(f"_get_api_data: {request=}")
+
+        schema_paths = validate.any(
+            validate.all(
+                {
+                    "paths": [
+                        validate.all(
+                            {
+                                "type": str,
+                                "path": str,
+                            },
+                            validate.union_get("type", "path"),
+                        ),
+                    ],
+                },
+                validate.get("paths"),
+            ),
+            validate.all(
+                {
+                    "path": str,
+                },
+                validate.transform(lambda obj: [("hls", obj["path"])]),
+            ),
+        )
+        schema_live = [{
+            "name": str,
+            "id": str,
+            "slug": str,
+            "stitched": schema_paths,
+        }]
+        schema_vod = [{
+            "name": str,
+            "id": str,
+            "slug": str,
+            "genre": str,
+            "stitched": validate.any(schema_paths, {}),
+            validate.optional("seasons"): [{
+                "episodes": [{
+                    "name": str,
+                    "_id": str,
+                    "slug": str,
+                    "stitched": schema_paths,
+                }],
+            }],
+        }]
 
         return self.session.http.get(
             "https://boot.pluto.tv/v4/start",
             params={
                 "appName": "web",
-                "appVersion": app_version,
-                "deviceVersion": "94.0.0",
+                "appVersion": self.app_version,
+                "deviceVersion": self._device_version,
                 "deviceModel": "web",
                 "deviceMake": "firefox",
                 "deviceType": "web",
-                "clientID": str(uuid4()),
-                "clientModelNumber": "1.0",
-                kind: slug,
+                "clientID": self._client_id,
+                "clientModelNumber": "1.0.0",
+                **request,
             },
             schema=validate.Schema(
-                validate.parse_json(), {
+                validate.parse_json(),
+                {
                     "servers": {
                         "stitcher": validate.url(),
                     },
-                    validate.optional("EPG"): [{
-                        "name": str,
-                        "id": str,
-                        "slug": str,
-                        "stitched": {
-                            "path": str,
-                        },
-                    }],
-                    validate.optional("VOD"): [{
-                        "name": str,
-                        "id": str,
-                        "slug": str,
-                        "genre": str,
-                        "stitched": {
-                            "path": str,
-                        },
-                        validate.optional("seasons"): [{
-                            "episodes": validate.all(
-                                [{
-                                    "name": str,
-                                    "_id": str,
-                                    "slug": str,
-                                    "stitched": {
-                                        "path": str,
-                                    },
-                                }],
-                                validate.filter(lambda k: slugfilter and k["slug"] == slugfilter),
-                            ),
-                        }],
-                    }],
-                    "sessionToken": str,
                     "stitcherParams": str,
+                    "sessionToken": str,
+                    validate.optional("EPG"): schema_live,
+                    validate.optional("VOD"): schema_vod,
                 },
             ),
         )
 
-    def _get_playlist(self, host, path, params, token):
-        qsd = dict(parse_qsl(params))
-        qsd["jwt"] = token
-
-        url = urljoin(host, path)
-        url = update_qsd(url, qsd)
-
-        return PlutoHLSStream.parse_variant_playlist(self.session, url)
-
-    @staticmethod
-    def _get_media_data(data, key, slug):
-        media = data.get(key)
-        if media and media[0]["slug"] == slug:
-            return media[0]
+    def _get_streams_live(self):
+        data = self._get_api_data({"channelSlug": self.match["id"]})
+        epg = data.get("EPG", [])
+        media = next((e for e in epg if e["id"] == self.match["id"]), None)
+        if not media:
+            return
+
+        self.id = media["id"]
+        self.title = media["name"]
+
+        return data, media["stitched"]
+
+    def _get_streams_series(self):
+        data = self._get_api_data({"seriesIDs": self.match["id_s"]})
+        vod = data.get("VOD", [])
+        media = next((v for v in vod if v["id"] == self.match["id_s"]), None)
+        if not media:
+            return
+        seasons = media.get("seasons", [])
+        episode = next((e for s in seasons for e in s["episodes"] if e["_id"] == self.match["id_e"]), None)
+        if not episode:
+            return
+
+        self.id = episode["_id"]
+        self.author = media["name"]
+        self.category = media["genre"]
+        self.title = episode["name"]
+
+        return data, episode["stitched"]
+
+    def _get_streams_movies(self):
+        data = self._get_api_data({"seriesIDs": self.match["id"]})
+        vod = data.get("VOD", [])
+        media = next((v for v in vod if v["id"] == self.match["id"]), None)
+        if not media:
+            return
+
+        self.id = media["id"]
+        self.category = media["genre"]
+        self.title = media["name"]
+
+        return data, media["stitched"]
 
     def _get_streams(self):
-        m = self.match.groupdict()
-        if m["slug_live"]:
-            data = self._get_api_data("channelSlug", m["slug_live"])
-            media = self._get_media_data(data, "EPG", m["slug_live"])
-            if not media:
-                return
-
-            self.id = media["id"]
-            self.title = media["name"]
-            path = media["stitched"]["path"]
-
-        elif m["slug_series"] and m["slug_episode"]:
-            data = self._get_api_data("episodeSlugs", m["slug_series"], slugfilter=m["slug_episode"])
-            media = self._get_media_data(data, "VOD", m["slug_series"])
-            if not media or "seasons" not in media:
-                return
-
-            for season in media["seasons"]:
-                if season["episodes"]:
-                    episode = season["episodes"][0]
-                    if episode["slug"] == m["slug_episode"]:
-                        break
-            else:
-                return
-
-            self.author = media["name"]
-            self.category = media["genre"]
-            self.id = episode["_id"]
-            self.title = episode["name"]
-            path = episode["stitched"]["path"]
-
-        elif m["slug_movies"]:
-            data = self._get_api_data("episodeSlugs", m["slug_movies"])
-            media = self._get_media_data(data, "VOD", m["slug_movies"])
-            if not media:
-                return
-
-            self.category = media["genre"]
-            self.id = media["id"]
-            self.title = media["name"]
-            path = media["stitched"]["path"]
+        res = None
+        if self.matches["live"]:
+            res = self._get_streams_live()
+        elif self.matches["series"]:
+            res = self._get_streams_series()
+        elif self.matches["movies"]:
+            res = self._get_streams_movies()
 
-        else:
+        if not res:
             return
 
-        log.trace(f"data={data!r}")
-        log.debug(f"path={path}")
+        data, paths = res
+        for mediatype, path in paths:
+            if mediatype != "hls":
+                continue
+
+            params = dict(parse_qsl(data["stitcherParams"]))
+            params["jwt"] = data["sessionToken"]
+            url = urljoin(data["servers"]["stitcher"], path)
+            url = update_qsd(url, params)
 
-        return self._get_playlist(
-            data["servers"]["stitcher"],
-            path,
-            data["stitcherParams"],
-            data["sessionToken"],
-        )
+            return PlutoHLSStream.parse_variant_playlist(self.session, url)
 
 
 __plugin__ = Pluto
```

### Comparing `streamlink-6.7.2/src/streamlink/plugins/pluzz.py` & `streamlink-6.7.3/src/streamlink/plugins/pluzz.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/radiko.py` & `streamlink-6.7.3/src/streamlink/plugins/radiko.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/radionet.py` & `streamlink-6.7.3/src/streamlink/plugins/radionet.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/raiplay.py` & `streamlink-6.7.3/src/streamlink/plugins/raiplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/reuters.py` & `streamlink-6.7.3/src/streamlink/plugins/reuters.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/rtpa.py` & `streamlink-6.7.3/src/streamlink/plugins/rtpa.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/rtpplay.py` & `streamlink-6.7.3/src/streamlink/plugins/rtpplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/rtve.py` & `streamlink-6.7.3/src/streamlink/plugins/rtve.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/rtvs.py` & `streamlink-6.7.3/src/streamlink/plugins/rtvs.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/ruv.py` & `streamlink-6.7.3/src/streamlink/plugins/ruv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/sbscokr.py` & `streamlink-6.7.3/src/streamlink/plugins/sbscokr.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/showroom.py` & `streamlink-6.7.3/src/streamlink/plugins/showroom.py`

 * *Files 12% similar despite different names*

```diff
@@ -80,15 +80,15 @@
                 validate.get("streaming_url_list"),
                 validate.filter(lambda p: p["type"] == "hls_all"),
                 validate.get((0, "url")),
             ),
         )
 
         res = self.session.http.get(url, acceptable_status=(200, 403, 404))
-        if res.headers["Content-Type"] != "application/x-mpegURL":
+        if res.headers["Content-Type"] not in ("application/x-mpegURL", "application/vnd.apple.mpegurl"):
             log.error("This stream is restricted")
             return
 
         return HLSStream.parse_variant_playlist(self.session, url)
 
 
 __plugin__ = Showroom
```

### Comparing `streamlink-6.7.2/src/streamlink/plugins/sportal.py` & `streamlink-6.7.3/src/streamlink/plugins/sportal.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/sportschau.py` & `streamlink-6.7.3/src/streamlink/plugins/sportschau.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/ssh101.py` & `streamlink-6.7.3/src/streamlink/plugins/ssh101.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/stadium.py` & `streamlink-6.7.3/src/streamlink/plugins/stadium.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/steam.py` & `streamlink-6.7.3/src/streamlink/plugins/steam.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/streamable.py` & `streamlink-6.7.3/src/streamlink/plugins/streamable.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/streann.py` & `streamlink-6.7.3/src/streamlink/plugins/streann.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/stv.py` & `streamlink-6.7.3/src/streamlink/plugins/stv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/svtplay.py` & `streamlink-6.7.3/src/streamlink/plugins/svtplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/swisstxt.py` & `streamlink-6.7.3/src/streamlink/plugins/swisstxt.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/telefe.py` & `streamlink-6.7.3/src/streamlink/plugins/telefe.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/telemadrid.py` & `streamlink-6.7.3/src/streamlink/plugins/telemadrid.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/tf1.py` & `streamlink-6.7.3/src/streamlink/plugins/tf1.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/trovo.py` & `streamlink-6.7.3/src/streamlink/plugins/trovo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/turkuvaz.py` & `streamlink-6.7.3/src/streamlink/plugins/turkuvaz.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/tv360.py` & `streamlink-6.7.3/src/streamlink/plugins/tv360.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/tv3cat.py` & `streamlink-6.7.3/src/streamlink/plugins/tv3cat.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/tv4play.py` & `streamlink-6.7.3/src/streamlink/plugins/tv4play.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/tv5monde.py` & `streamlink-6.7.3/src/streamlink/plugins/tv5monde.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/tv8.py` & `streamlink-6.7.3/src/streamlink/plugins/tv8.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/tv999.py` & `streamlink-6.7.3/src/streamlink/plugins/tv999.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/tvibo.py` & `streamlink-6.7.3/src/streamlink/plugins/tvibo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/tviplayer.py` & `streamlink-6.7.3/src/streamlink/plugins/tviplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/tvp.py` & `streamlink-6.7.3/src/streamlink/plugins/tvp.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/tvrby.py` & `streamlink-6.7.3/src/streamlink/plugins/tvrby.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/tvrplus.py` & `streamlink-6.7.3/src/streamlink/plugins/tvrplus.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/tvtoya.py` & `streamlink-6.7.3/src/streamlink/plugins/tvtoya.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/twitcasting.py` & `streamlink-6.7.3/src/streamlink/plugins/twitcasting.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/twitch.py` & `streamlink-6.7.3/src/streamlink/plugins/twitch.py`

 * *Files 1% similar despite different names*

```diff
@@ -537,15 +537,15 @@
     def acquire(
         cls,
         session: Streamlink,
         channel: str,
         headers: Mapping[str, str],
         device_id: str,
     ) -> Optional[Tuple[str, int]]:
-        from exceptiongroup import BaseExceptionGroup, catch  # noqa: PLC0415, I001
+        from exceptiongroup import BaseExceptionGroup  # noqa: PLC0415, I001
         from streamlink.webbrowser.cdp import CDPClient, CDPClientSession, devtools  # noqa: PLC0415
 
         url = f"https://www.twitch.tv/{channel}"
         js_get_integrity_token = cls.JS_INTEGRITY_TOKEN \
             .replace("SCRIPT_SOURCE", cls.URL_P_SCRIPT) \
             .replace("HEADERS", json_dumps(headers)) \
             .replace("DEVICE_ID", device_id)
@@ -561,27 +561,25 @@
             client_session: CDPClientSession
             async with client.session() as client_session:
                 client_session.add_request_handler(on_main, url_pattern=url, on_request=True)
                 async with client_session.navigate(url) as frame_id:
                     await client_session.loaded(frame_id)
                     return await client_session.evaluate(js_get_integrity_token, timeout=eval_timeout)
 
-        def handle_error(exc_grp: BaseExceptionGroup) -> None:
-            for err in exc_grp.exceptions:
-                log.error(f"{type(err).__name__}: {err}")
-
-        with catch({  # type: ignore[dict-item]  # bug in exceptiongroup==1.2.0
-            Exception: handle_error,  # type: ignore[dict-item]  # bug in exceptiongroup==1.2.0
-        }):
+        try:
             client_integrity = CDPClient.launch(
                 session,
                 acquire_client_integrity_token,
                 # headless mode gets detected by Twitch, so we have to disable it regardless the user config
                 headless=False,
             )
+        except BaseExceptionGroup:
+            log.exception("Failed acquiring client integrity token")
+        except Exception as err:
+            log.error(err)
 
         if not client_integrity:
             return None
 
         token, expiration = parse_json(client_integrity, schema=validate.Schema(
             {"token": str, "expiration": int},
             validate.union_get("token", "expiration"),
```

### Comparing `streamlink-6.7.2/src/streamlink/plugins/ustreamtv.py` & `streamlink-6.7.3/src/streamlink/plugins/ustreamtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/ustvnow.py` & `streamlink-6.7.3/src/streamlink/plugins/ustvnow.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/vidio.py` & `streamlink-6.7.3/src/streamlink/plugins/vidio.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/vimeo.py` & `streamlink-6.7.3/src/streamlink/plugins/vimeo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/vinhlongtv.py` & `streamlink-6.7.3/src/streamlink/plugins/vinhlongtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/vk.py` & `streamlink-6.7.3/src/streamlink/plugins/vk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/vkplay.py` & `streamlink-6.7.3/src/streamlink/plugins/vkplay.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 $description Russian live-streaming platform for gaming and esports, owned by VKontakte.
-$url vkplay.live
+$url live.vkplay.ru
 $type live
 $metadata id
 $metadata author
 $metadata category
 $metadata title
 """
 
@@ -16,21 +16,21 @@
 from streamlink.stream.hls import HLSStream
 
 
 log = logging.getLogger(__name__)
 
 
 @pluginmatcher(re.compile(
-    r"https?://vkplay\.live/(?P<channel_name>\w+)/?$",
+    r"https?://(?:live\.vkplay\.ru|vkplay\.live)/(?P<channel_name>\w+)/?$",
 ))
 class VKplay(Plugin):
-    API_URL = "https://api.vkplay.live/v1"
+    API_URL = "https://api.live.vkplay.ru/v1"
 
     def _get_streams(self):
-        self.author = self.match.group("channel_name")
+        self.author = self.match["channel_name"]
         log.debug(f"Channel name: {self.author}")
 
         data = self.session.http.get(
             f"{self.API_URL}/blog/{self.author}/public_video_stream",
             headers={"Referer": self.url},
             acceptable_status=(200, 404),
             schema=validate.Schema(
```

### Comparing `streamlink-6.7.2/src/streamlink/plugins/vtvgo.py` & `streamlink-6.7.3/src/streamlink/plugins/vtvgo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/webtv.py` & `streamlink-6.7.3/src/streamlink/plugins/webtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/welt.py` & `streamlink-6.7.3/src/streamlink/plugins/welt.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/wwenetwork.py` & `streamlink-6.7.3/src/streamlink/plugins/wwenetwork.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/youtube.py` & `streamlink-6.7.3/src/streamlink/plugins/youtube.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/yupptv.py` & `streamlink-6.7.3/src/streamlink/plugins/yupptv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/zattoo.py` & `streamlink-6.7.3/src/streamlink/plugins/zattoo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/zdf_mediathek.py` & `streamlink-6.7.3/src/streamlink/plugins/zdf_mediathek.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/zeenews.py` & `streamlink-6.7.3/src/streamlink/plugins/zeenews.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/zengatv.py` & `streamlink-6.7.3/src/streamlink/plugins/zengatv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/plugins/zhanqi.py` & `streamlink-6.7.3/src/streamlink/plugins/zhanqi.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/session/http.py` & `streamlink-6.7.3/src/streamlink/session/http.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/session/http.pyi` & `streamlink-6.7.3/src/streamlink/session/http.pyi`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/session/options.py` & `streamlink-6.7.3/src/streamlink/session/options.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/session/plugins.py` & `streamlink-6.7.3/src/streamlink/session/plugins.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/session/session.py` & `streamlink-6.7.3/src/streamlink/session/session.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/stream/dash/dash.py` & `streamlink-6.7.3/src/streamlink/stream/dash/dash.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/stream/dash/manifest.py` & `streamlink-6.7.3/src/streamlink/stream/dash/manifest.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/stream/dash/segment.py` & `streamlink-6.7.3/src/streamlink/stream/dash/segment.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/stream/ffmpegmux.py` & `streamlink-6.7.3/src/streamlink/stream/ffmpegmux.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/stream/file.py` & `streamlink-6.7.3/src/streamlink/stream/file.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/stream/filtered.py` & `streamlink-6.7.3/src/streamlink/stream/filtered.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/stream/hls/hls.py` & `streamlink-6.7.3/src/streamlink/stream/hls/hls.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/stream/hls/m3u8.py` & `streamlink-6.7.3/src/streamlink/stream/hls/m3u8.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/stream/hls/segment.py` & `streamlink-6.7.3/src/streamlink/stream/hls/segment.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/stream/http.py` & `streamlink-6.7.3/src/streamlink/stream/http.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/stream/segmented/concurrent.py` & `streamlink-6.7.3/src/streamlink/stream/segmented/concurrent.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/stream/segmented/segmented.py` & `streamlink-6.7.3/src/streamlink/stream/segmented/segmented.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/stream/stream.py` & `streamlink-6.7.3/src/streamlink/stream/stream.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/stream/wrappers.py` & `streamlink-6.7.3/src/streamlink/stream/wrappers.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/user_input.py` & `streamlink-6.7.3/src/streamlink/user_input.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/utils/__init__.py` & `streamlink-6.7.3/src/streamlink/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/utils/args.py` & `streamlink-6.7.3/src/streamlink/utils/args.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/utils/cache.py` & `streamlink-6.7.3/src/streamlink/utils/cache.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/utils/crypto.py` & `streamlink-6.7.3/src/streamlink/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/utils/data.py` & `streamlink-6.7.3/src/streamlink/utils/data.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/utils/formatter.py` & `streamlink-6.7.3/src/streamlink/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/utils/l10n.py` & `streamlink-6.7.3/src/streamlink/utils/l10n.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/utils/module.py` & `streamlink-6.7.3/src/streamlink/utils/module.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/utils/named_pipe.py` & `streamlink-6.7.3/src/streamlink/utils/named_pipe.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/utils/parse.py` & `streamlink-6.7.3/src/streamlink/utils/parse.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/utils/processoutput.py` & `streamlink-6.7.3/src/streamlink/utils/processoutput.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/utils/random.py` & `streamlink-6.7.3/src/streamlink/utils/random.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/utils/socket.py` & `streamlink-6.7.3/src/streamlink/utils/socket.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/utils/times.py` & `streamlink-6.7.3/src/streamlink/utils/times.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/utils/url.py` & `streamlink-6.7.3/src/streamlink/utils/url.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/webbrowser/cdp/client.py` & `streamlink-6.7.3/src/streamlink/webbrowser/cdp/client.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/webbrowser/cdp/connection.py` & `streamlink-6.7.3/src/streamlink/webbrowser/cdp/connection.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/__init__.py` & `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/browser.py` & `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/browser.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/debugger.py` & `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/debugger.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/dom.py` & `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/dom.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/emulation.py` & `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/emulation.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/fetch.py` & `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/fetch.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/input_.py` & `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/input_.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/inspector.py` & `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/inspector.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/io.py` & `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/io.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/network.py` & `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/network.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/page.py` & `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/page.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/runtime.py` & `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/runtime.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/security.py` & `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/security.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/target.py` & `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/target.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/webbrowser/cdp/devtools/util.py` & `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/util.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/webbrowser/chromium.py` & `streamlink-6.7.3/src/streamlink/webbrowser/chromium.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink/webbrowser/webbrowser.py` & `streamlink-6.7.3/src/streamlink/webbrowser/webbrowser.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from contextlib import asynccontextmanager, contextmanager
 from functools import partial
 from pathlib import Path
 from subprocess import DEVNULL
 from typing import AsyncContextManager, AsyncGenerator, Generator, List, Optional, Union
 
 import trio
-from exceptiongroup import BaseExceptionGroup, catch
+from exceptiongroup import BaseExceptionGroup
 
 from streamlink.utils.path import resolve_executable
 from streamlink.webbrowser.exceptions import WebbrowserError
 
 
 log = logging.getLogger(__name__)
 
@@ -76,20 +76,15 @@
         self.executable = executable
         self.arguments = arguments
         self.timeout = timeout
         self._process_ended_early = False
 
     @asynccontextmanager
     async def launch(self) -> AsyncGenerator[trio.Nursery, None]:
-        def handle_baseexception(exc_grp: BaseExceptionGroup) -> None:
-            raise exc_grp.exceptions[0] from exc_grp.exceptions[0].__context__
-
-        with catch({  # type: ignore[dict-item]  # bug in exceptiongroup==1.2.0
-            (KeyboardInterrupt, SystemExit): handle_baseexception,  # type: ignore[dict-item]  # bug in exceptiongroup==1.2.0
-        }):
+        try:
             async with trio.open_nursery() as nursery:
                 log.info(f"Launching web browser: {self.executable}")
                 # the process is run in a separate task
                 run_process = partial(
                     trio.run_process,
                     [self.executable, *self.arguments],
                     check=False,
@@ -109,14 +104,21 @@
                         log.warning("Web browser task group has timed out")
                 finally:
                     # check if the task group hasn't been cancelled yet in the process watcher task
                     if not self._process_ended_early:
                         log.debug("Waiting for web browser process to terminate")
                     # once the application logic is done, cancel the entire task group and terminate/kill the process
                     nursery.cancel_scope.cancel()
+        except BaseExceptionGroup as exc_grp:  # TODO: py310 support end: use except*
+            exc: Union[BaseException, BaseExceptionGroup, None] = exc_grp.subgroup((KeyboardInterrupt, SystemExit))
+            if not exc:  # not a KeyboardInterrupt or SystemExit
+                raise
+            while isinstance(exc, BaseExceptionGroup):  # get the first actual exception in the potentially nested groups
+                exc = exc.exceptions[0]
+            raise exc from exc.__context__
 
     async def _task_process_watcher(self, process: trio.Process, nursery: trio.Nursery) -> None:
         """Task for cancelling the launch task group if the user closes the browser or if it exits early on its own"""
         await process.wait()
         # if the task group hasn't been cancelled yet, then the application logic was still running
         if not nursery.cancel_scope.cancel_called:  # pragma: no branch
             self._process_ended_early = True
```

### Comparing `streamlink-6.7.2/src/streamlink.egg-info/PKG-INFO` & `streamlink-6.7.3/src/streamlink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlink
-Version: 6.7.2
+Version: 6.7.3
 Summary: Streamlink is a command-line utility that extracts streams from various services and pipes them into a video player of choice.
 Author: Streamlink
 Author-email: streamlink@protonmail.com
 License: Simplified BSD
 Project-URL: Homepage, https://github.com/streamlink/streamlink
 Project-URL: Documentation, https://streamlink.github.io/
 Project-URL: Tracker, https://github.com/streamlink/streamlink/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: streamlink Version: 6.7.2 Summary: Streamlink is a
+Metadata-Version: 2.1 Name: streamlink Version: 6.7.3 Summary: Streamlink is a
 command-line utility that extracts streams from various services and pipes them
 into a video player of choice. Author: Streamlink Author-email:
 streamlink@protonmail.com License: Simplified BSD Project-URL: Homepage, https:
 //github.com/streamlink/streamlink Project-URL: Documentation, https://
 streamlink.github.io/ Project-URL: Tracker, https://github.com/streamlink/
 streamlink/issues Project-URL: Source, https://github.com/streamlink/streamlink
 Project-URL: Funding, https://streamlink.github.io/latest/donate.html
```

### Comparing `streamlink-6.7.2/src/streamlink.egg-info/SOURCES.txt` & `streamlink-6.7.3/src/streamlink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink_cli/argparser.py` & `streamlink-6.7.3/src/streamlink_cli/argparser.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink_cli/console.py` & `streamlink-6.7.3/src/streamlink_cli/console.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink_cli/constants.py` & `streamlink-6.7.3/src/streamlink_cli/constants.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink_cli/main.py` & `streamlink-6.7.3/src/streamlink_cli/main.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink_cli/output/abc.py` & `streamlink-6.7.3/src/streamlink_cli/output/abc.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink_cli/output/file.py` & `streamlink-6.7.3/src/streamlink_cli/output/file.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink_cli/output/http.py` & `streamlink-6.7.3/src/streamlink_cli/output/http.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink_cli/output/player.py` & `streamlink-6.7.3/src/streamlink_cli/output/player.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink_cli/streamrunner.py` & `streamlink-6.7.3/src/streamlink_cli/streamrunner.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink_cli/utils/__init__.py` & `streamlink-6.7.3/src/streamlink_cli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink_cli/utils/formatter.py` & `streamlink-6.7.3/src/streamlink_cli/utils/formatter.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from pathlib import Path
 from typing import Optional
 
 from streamlink.utils.formatter import Formatter as _BaseFormatter
-from streamlink_cli.utils.path import replace_chars, replace_path
+from streamlink_cli.utils.path import replace_chars, replace_path, truncate_path
 
 
 class Formatter(_BaseFormatter):
     title = _BaseFormatter.format
 
-    def path(self, pathlike: str, charmap: Optional[str] = None) -> Path:
+    def path(self, pathlike: str, charmap: Optional[str] = None, max_filename_length: int = 255) -> Path:
         def mapper(s):
             return replace_chars(s, charmap)
 
-        def format_part(part):
-            return self._format(part, mapper, {})
+        def format_part(part: str, isfile: bool) -> str:
+            formatted = self._format(part, mapper, {})
+            return truncate_path(formatted, max_filename_length, keep_extension=isfile)
 
         return replace_path(pathlike, format_part)
```

### Comparing `streamlink-6.7.2/src/streamlink_cli/utils/player.py` & `streamlink-6.7.3/src/streamlink_cli/utils/player.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink_cli/utils/progress.py` & `streamlink-6.7.3/src/streamlink_cli/utils/progress.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/src/streamlink_cli/utils/versioncheck.py` & `streamlink-6.7.3/src/streamlink_cli/utils/versioncheck.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/__init__.py` & `streamlink-6.7.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/cli/output/test_file.py` & `streamlink-6.7.3/tests/cli/output/test_file.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/cli/output/test_player.py` & `streamlink-6.7.3/tests/cli/output/test_player.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/cli/test_argparser.py` & `streamlink-6.7.3/tests/cli/test_argparser.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/cli/test_cmdline.py` & `streamlink-6.7.3/tests/cli/test_cmdline.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/cli/test_cmdline_title.py` & `streamlink-6.7.3/tests/cli/test_cmdline_title.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/cli/test_console.py` & `streamlink-6.7.3/tests/cli/test_console.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/cli/test_main.py` & `streamlink-6.7.3/tests/cli/test_main.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/cli/test_main_check_file_output.py` & `streamlink-6.7.3/tests/cli/test_main_check_file_output.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/cli/test_main_formatter.py` & `streamlink-6.7.3/tests/cli/test_main_formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/cli/test_main_logging.py` & `streamlink-6.7.3/tests/cli/test_main_logging.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/cli/test_main_setup_config_args.py` & `streamlink-6.7.3/tests/cli/test_main_setup_config_args.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/cli/test_plugin_args_and_options.py` & `streamlink-6.7.3/tests/cli/test_plugin_args_and_options.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/cli/test_streamrunner.py` & `streamlink-6.7.3/tests/cli/test_streamrunner.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/cli/utils/test_formatter.py` & `streamlink-6.7.3/tests/cli/utils/test_formatter.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from datetime import datetime
 from os.path import sep
 from pathlib import Path
+from string import ascii_letters as alphabet
 from unittest.mock import Mock, call, patch
 
 import pytest
 from freezegun import freeze_time
 
 from streamlink_cli.utils.formatter import Formatter
 
@@ -75,7 +76,23 @@
             "parent": lambda: "..",
             "dots": lambda: "...",
             "separator": lambda: sep,
         })
         path = formatter.path(f"{{current}}{sep}{{parent}}{sep}{{dots}}{sep}{{separator}}{sep}foo{sep}.{sep}..{sep}bar")
         assert path == Path("_", "_", "...", "_", "foo", ".", "..", "bar"), \
             "Formats the path's parts separately and ignores current and parent directories in substitutions only"
+
+    def test_path_truncation_ascii(self, formatter: Formatter):
+        formatter.mapping.update({
+            "dir": lambda: alphabet * 10,
+            "file": lambda: alphabet * 10,
+        })
+        path = formatter.path(f"{{dir}}.fakeext{sep}{{file}}.ext")
+        assert path == Path((alphabet * 10)[:255], f"{(alphabet * 10)[:251]}.ext")
+
+    def test_path_truncation_unicode(self, formatter: Formatter):
+        formatter.mapping.update({
+            "dir": lambda: "🐻" * 512,
+            "file": lambda: "🐻" * 512,
+        })
+        path = formatter.path(f"{{dir}}.fakeext{sep}{{file}}.ext")
+        assert path == Path("🐻" * 63, f"{'🐻' * 62}.ext")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `streamlink-6.7.2/tests/cli/utils/test_player.py` & `streamlink-6.7.3/tests/cli/utils/test_player.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/cli/utils/test_progress.py` & `streamlink-6.7.3/tests/cli/utils/test_progress.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/cli/utils/test_versioncheck.py` & `streamlink-6.7.3/tests/cli/utils/test_versioncheck.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/conftest.py` & `streamlink-6.7.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/mixins/stream_hls.py` & `streamlink-6.7.3/tests/mixins/stream_hls.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugin/testplugin.py` & `streamlink-6.7.3/tests/plugin/testplugin.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/__init__.py` & `streamlink-6.7.3/tests/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/conftest.py` & `streamlink-6.7.3/tests/plugins/conftest.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_abematv.py` & `streamlink-6.7.3/tests/plugins/test_abematv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_adultswim.py` & `streamlink-6.7.3/tests/plugins/test_adultswim.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_afreeca.py` & `streamlink-6.7.3/tests/plugins/test_afreeca.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_albavision.py` & `streamlink-6.7.3/tests/plugins/test_albavision.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_aloula.py` & `streamlink-6.7.3/tests/plugins/test_aloula.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_ard_mediathek.py` & `streamlink-6.7.3/tests/plugins/test_ard_mediathek.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_artetv.py` & `streamlink-6.7.3/tests/plugins/test_artetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_atpchallenger.py` & `streamlink-6.7.3/tests/plugins/test_atpchallenger.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_atresplayer.py` & `streamlink-6.7.3/tests/plugins/test_atresplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_bbciplayer.py` & `streamlink-6.7.3/tests/plugins/test_bbciplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_bfmtv.py` & `streamlink-6.7.3/tests/plugins/test_bfmtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_blazetv.py` & `streamlink-6.7.3/tests/plugins/test_blazetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_bloomberg.py` & `streamlink-6.7.3/tests/plugins/test_bloomberg.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_booyah.py` & `streamlink-6.7.3/tests/plugins/test_booyah.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_cbsnews.py` & `streamlink-6.7.3/tests/plugins/test_cbsnews.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_cdnbg.py` & `streamlink-6.7.3/tests/plugins/test_cdnbg.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_ceskatelevize.py` & `streamlink-6.7.3/tests/plugins/test_ceskatelevize.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_cinergroup.py` & `streamlink-6.7.3/tests/plugins/test_cinergroup.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_cmmedia.py` & `streamlink-6.7.3/tests/plugins/test_cmmedia.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_crunchyroll.py` & `streamlink-6.7.3/tests/plugins/test_crunchyroll.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_dailymotion.py` & `streamlink-6.7.3/tests/plugins/test_dailymotion.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_dash.py` & `streamlink-6.7.3/tests/plugins/test_dash.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_delfi.py` & `streamlink-6.7.3/tests/plugins/test_delfi.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_deutschewelle.py` & `streamlink-6.7.3/tests/plugins/test_deutschewelle.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_dlive.py` & `streamlink-6.7.3/tests/plugins/test_dlive.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_dogan.py` & `streamlink-6.7.3/tests/plugins/test_dogan.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_drdk.py` & `streamlink-6.7.3/tests/plugins/test_drdk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_euronews.py` & `streamlink-6.7.3/tests/plugins/test_euronews.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_facebook.py` & `streamlink-6.7.3/tests/plugins/test_facebook.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_filmon.py` & `streamlink-6.7.3/tests/plugins/test_filmon.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_goltelevision.py` & `streamlink-6.7.3/tests/plugins/test_goltelevision.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_goodgame.py` & `streamlink-6.7.3/tests/plugins/test_goodgame.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_gulli.py` & `streamlink-6.7.3/tests/plugins/test_gulli.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_hls.py` & `streamlink-6.7.3/tests/plugins/test_hls.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_http.py` & `streamlink-6.7.3/tests/plugins/test_http.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_htv.py` & `streamlink-6.7.3/tests/plugins/test_htv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_idf1.py` & `streamlink-6.7.3/tests/plugins/test_idf1.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_invintus.py` & `streamlink-6.7.3/tests/plugins/test_invintus.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_kugou.py` & `streamlink-6.7.3/tests/plugins/test_kugou.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_livestream.py` & `streamlink-6.7.3/tests/plugins/test_livestream.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_lnk.py` & `streamlink-6.7.3/tests/plugins/test_lnk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_lrt.py` & `streamlink-6.7.3/tests/plugins/test_lrt.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_ltv_lsm_lv.py` & `streamlink-6.7.3/tests/plugins/test_ltv_lsm_lv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_mangomolo.py` & `streamlink-6.7.3/tests/plugins/test_mangomolo.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,10 +13,18 @@
         ),
         (
             "mediagovkw",
             "https://media.gov.kw/LiveTV.aspx?PanChannel=KTV1",
         ),
         (
             "mediagovkw",
+            "https://www.media.gov.kw/LiveTV.aspx?PanChannel=KTV1",
+        ),
+        (
+            "mediagovkw",
             "https://media.gov.kw/LiveTV.aspx?PanChannel=KTVSports",
         ),
+        (
+            "mediagovkw",
+            "https://www.media.gov.kw/LiveTV.aspx?PanChannel=KTVSports",
+        ),
     ]
```

### Comparing `streamlink-6.7.2/tests/plugins/test_mdstrm.py` & `streamlink-6.7.3/tests/plugins/test_mdstrm.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_mediaklikk.py` & `streamlink-6.7.3/tests/plugins/test_mediaklikk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_mediavitrina.py` & `streamlink-6.7.3/tests/plugins/test_mediavitrina.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_mitele.py` & `streamlink-6.7.3/tests/plugins/test_mitele.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_mixcloud.py` & `streamlink-6.7.3/tests/plugins/test_mixcloud.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_n13tv.py` & `streamlink-6.7.3/tests/plugins/test_n13tv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_nasaplus.py` & `streamlink-6.7.3/tests/plugins/test_nasaplus.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_nicolive.py` & `streamlink-6.7.3/tests/plugins/test_nicolive.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_nos.py` & `streamlink-6.7.3/tests/plugins/test_nos.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_nrk.py` & `streamlink-6.7.3/tests/plugins/test_nrk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_olympicchannel.py` & `streamlink-6.7.3/tests/plugins/test_olympicchannel.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_oneplusone.py` & `streamlink-6.7.3/tests/plugins/test_oneplusone.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_onetv.py` & `streamlink-6.7.3/tests/plugins/test_onetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_piaulizaportal.py` & `streamlink-6.7.3/tests/plugins/test_piaulizaportal.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_picarto.py` & `streamlink-6.7.3/tests/plugins/test_picarto.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_pluzz.py` & `streamlink-6.7.3/tests/plugins/test_pluzz.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_radionet.py` & `streamlink-6.7.3/tests/plugins/test_radionet.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_raiplay.py` & `streamlink-6.7.3/tests/plugins/test_raiplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_reuters.py` & `streamlink-6.7.3/tests/plugins/test_reuters.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_rtpplay.py` & `streamlink-6.7.3/tests/plugins/test_rtpplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_rtve.py` & `streamlink-6.7.3/tests/plugins/test_rtve.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_rtvs.py` & `streamlink-6.7.3/tests/plugins/test_rtvs.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_ruv.py` & `streamlink-6.7.3/tests/plugins/test_ruv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_sbscokr.py` & `streamlink-6.7.3/tests/plugins/test_sbscokr.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_showroom.py` & `streamlink-6.7.3/tests/plugins/test_showroom.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_steam.py` & `streamlink-6.7.3/tests/plugins/test_steam.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_streann.py` & `streamlink-6.7.3/tests/plugins/test_streann.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_svtplay.py` & `streamlink-6.7.3/tests/plugins/test_svtplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_swisstxt.py` & `streamlink-6.7.3/tests/plugins/test_swisstxt.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_telefe.py` & `streamlink-6.7.3/tests/plugins/test_telefe.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_tf1.py` & `streamlink-6.7.3/tests/plugins/test_tf1.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_trovo.py` & `streamlink-6.7.3/tests/plugins/test_trovo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_turkuvaz.py` & `streamlink-6.7.3/tests/plugins/test_turkuvaz.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_tv3cat.py` & `streamlink-6.7.3/tests/plugins/test_tv3cat.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_tv4play.py` & `streamlink-6.7.3/tests/plugins/test_tv4play.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_tv5monde.py` & `streamlink-6.7.3/tests/plugins/test_tv5monde.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_tvp.py` & `streamlink-6.7.3/tests/plugins/test_tvp.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_tvrby.py` & `streamlink-6.7.3/tests/plugins/test_tvrby.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_tvrplus.py` & `streamlink-6.7.3/tests/plugins/test_tvrplus.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_twitch.py` & `streamlink-6.7.3/tests/plugins/test_twitch.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_ustreamtv.py` & `streamlink-6.7.3/tests/plugins/test_ustreamtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_ustvnow.py` & `streamlink-6.7.3/tests/plugins/test_ustvnow.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_vimeo.py` & `streamlink-6.7.3/tests/plugins/test_vimeo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_vinhlongtv.py` & `streamlink-6.7.3/tests/plugins/test_vinhlongtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_vk.py` & `streamlink-6.7.3/tests/plugins/test_vk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_vtvgo.py` & `streamlink-6.7.3/tests/plugins/test_vtvgo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_webtv.py` & `streamlink-6.7.3/tests/plugins/test_webtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_welt.py` & `streamlink-6.7.3/tests/plugins/test_welt.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_youtube.py` & `streamlink-6.7.3/tests/plugins/test_youtube.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_zattoo.py` & `streamlink-6.7.3/tests/plugins/test_zattoo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_zdf_mediathek.py` & `streamlink-6.7.3/tests/plugins/test_zdf_mediathek.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/plugins/test_zengatv.py` & `streamlink-6.7.3/tests/plugins/test_zengatv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/__init__.py` & `streamlink-6.7.3/tests/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/dash/test_1.mpd` & `streamlink-6.7.3/tests/resources/dash/test_1.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/dash/test_10.mpd` & `streamlink-6.7.3/tests/resources/dash/test_10.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/dash/test_11_static.mpd` & `streamlink-6.7.3/tests/resources/dash/test_11_static.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/dash/test_2.mpd` & `streamlink-6.7.3/tests/resources/dash/test_2.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/dash/test_3.mpd` & `streamlink-6.7.3/tests/resources/dash/test_3.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/dash/test_8.mpd` & `streamlink-6.7.3/tests/resources/dash/test_8.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/dash/test_9.mpd` & `streamlink-6.7.3/tests/resources/dash/test_9.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/dash/test_dynamic_segment_list_no_duration.mpd` & `streamlink-6.7.3/tests/resources/dash/test_dynamic_segment_list_no_duration.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/dash/test_dynamic_segment_list_p1.mpd` & `streamlink-6.7.3/tests/resources/dash/test_dynamic_segment_list_p1.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/dash/test_dynamic_segment_list_p2.mpd` & `streamlink-6.7.3/tests/resources/dash/test_dynamic_segment_list_p2.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/dash/test_dynamic_segment_list_p3.mpd` & `streamlink-6.7.3/tests/resources/dash/test_dynamic_segment_list_p3.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/dash/test_dynamic_segment_list_p4.mpd` & `streamlink-6.7.3/tests/resources/dash/test_dynamic_segment_list_p4.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/dash/test_dynamic_segment_list_p5.mpd` & `streamlink-6.7.3/tests/resources/dash/test_dynamic_segment_list_p5.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/dash/test_dynamic_timeline_continued_p1.mpd` & `streamlink-6.7.3/tests/resources/dash/test_dynamic_timeline_continued_p1.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/dash/test_dynamic_timeline_continued_p2.mpd` & `streamlink-6.7.3/tests/resources/dash/test_dynamic_timeline_continued_p2.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/dash/test_nested_baseurls.mpd` & `streamlink-6.7.3/tests/resources/dash/test_nested_baseurls.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/dash/test_no_segment_list_or_template.mpd` & `streamlink-6.7.3/tests/resources/dash/test_no_segment_list_or_template.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/dash/test_segment_list.mpd` & `streamlink-6.7.3/tests/resources/dash/test_segment_list.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/dash/test_segments_byterange.mpd` & `streamlink-6.7.3/tests/resources/dash/test_segments_byterange.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/dash/test_segments_dynamic_number.mpd` & `streamlink-6.7.3/tests/resources/dash/test_segments_dynamic_number.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/dash/test_static_no_publish_time.mpd` & `streamlink-6.7.3/tests/resources/dash/test_static_no_publish_time.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/dash/test_suggested_presentation_delay.mpd` & `streamlink-6.7.3/tests/resources/dash/test_suggested_presentation_delay.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/dash/test_timeline_ids.mpd` & `streamlink-6.7.3/tests/resources/dash/test_timeline_ids.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/hls/test_1.m3u8` & `streamlink-6.7.3/tests/resources/hls/test_1.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/hls/test_2.m3u8` & `streamlink-6.7.3/tests/resources/hls/test_2.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/hls/test_date.m3u8` & `streamlink-6.7.3/tests/resources/hls/test_date.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/hls/test_master.m3u8` & `streamlink-6.7.3/tests/resources/hls/test_master.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/hls/test_master_twitch_vod.m3u8` & `streamlink-6.7.3/tests/resources/hls/test_master_twitch_vod.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/resources/hls/test_multivariant_bandwidth.m3u8` & `streamlink-6.7.3/tests/resources/hls/test_multivariant_bandwidth.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/session/test_http.py` & `streamlink-6.7.3/tests/session/test_http.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/session/test_options.py` & `streamlink-6.7.3/tests/session/test_options.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/session/test_plugins.py` & `streamlink-6.7.3/tests/session/test_plugins.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/session/test_session.py` & `streamlink-6.7.3/tests/session/test_session.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/stream/dash/test_dash.py` & `streamlink-6.7.3/tests/stream/dash/test_dash.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/stream/dash/test_manifest.py` & `streamlink-6.7.3/tests/stream/dash/test_manifest.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/stream/hls/test_hls.py` & `streamlink-6.7.3/tests/stream/hls/test_hls.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/stream/hls/test_hls_filtered.py` & `streamlink-6.7.3/tests/stream/hls/test_hls_filtered.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/stream/hls/test_m3u8.py` & `streamlink-6.7.3/tests/stream/hls/test_m3u8.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/stream/test_ffmpegmux.py` & `streamlink-6.7.3/tests/stream/test_ffmpegmux.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/stream/test_file.py` & `streamlink-6.7.3/tests/stream/test_file.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/stream/test_stream_json.py` & `streamlink-6.7.3/tests/stream/test_stream_json.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/stream/test_stream_to_url.py` & `streamlink-6.7.3/tests/stream/test_stream_to_url.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/stream/test_stream_wrappers.py` & `streamlink-6.7.3/tests/stream/test_stream_wrappers.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/test_api_validate.py` & `streamlink-6.7.3/tests/test_api_validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1339,21 +1339,28 @@
 
 class TestParseQsdValidator:
     def test_success(self):
         assert validate.validate(
             validate.parse_qsd(),
             "foo=bar&foo=baz&qux=quux",
         ) == {"foo": "baz", "qux": "quux"}
+        assert validate.validate(
+            validate.parse_qsd(),
+            b"foo=bar&foo=baz&qux=quux",
+        ) == {b"foo": b"baz", b"qux": b"quux"}
 
     def test_failure(self):
         with pytest.raises(ValidationError) as cm:
             validate.validate(validate.parse_qsd(), 123)
         assert_validationerror(cm.value, """
-            ValidationError:
-              Unable to parse query string: 'int' object has no attribute 'decode' (123)
+            ValidationError(AnySchema):
+              ValidationError(type):
+                Type of 123 should be str, but is int
+              ValidationError(type):
+                Type of 123 should be bytes, but is int
         """)
 
 
 class TestValidationError:
     def test_subclass(self):
         assert issubclass(ValidationError, ValueError)
```

### Comparing `streamlink-6.7.2/tests/test_api_websocket.py` & `streamlink-6.7.3/tests/test_api_websocket.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/test_buffers.py` & `streamlink-6.7.3/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/test_cache.py` & `streamlink-6.7.3/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/test_compat.py` & `streamlink-6.7.3/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/test_logger.py` & `streamlink-6.7.3/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/test_options.py` & `streamlink-6.7.3/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/test_plugin.py` & `streamlink-6.7.3/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/test_plugin_userinput.py` & `streamlink-6.7.3/tests/test_plugin_userinput.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/test_plugins.py` & `streamlink-6.7.3/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/test_streamlink_api.py` & `streamlink-6.7.3/tests/test_streamlink_api.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/testutils/handshake.py` & `streamlink-6.7.3/tests/testutils/handshake.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/testutils/test_handshake.py` & `streamlink-6.7.3/tests/testutils/test_handshake.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/utils/test_args.py` & `streamlink-6.7.3/tests/utils/test_args.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/utils/test_cache.py` & `streamlink-6.7.3/tests/utils/test_cache.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/utils/test_crypto.py` & `streamlink-6.7.3/tests/utils/test_crypto.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/utils/test_data.py` & `streamlink-6.7.3/tests/utils/test_data.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/utils/test_formatter.py` & `streamlink-6.7.3/tests/utils/test_formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/utils/test_l10n.py` & `streamlink-6.7.3/tests/utils/test_l10n.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/utils/test_module.py` & `streamlink-6.7.3/tests/utils/test_module.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/utils/test_named_pipe.py` & `streamlink-6.7.3/tests/utils/test_named_pipe.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/utils/test_parse.py` & `streamlink-6.7.3/tests/utils/test_parse.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/utils/test_path.py` & `streamlink-6.7.3/tests/utils/test_path.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/utils/test_processoutput.py` & `streamlink-6.7.3/tests/utils/test_processoutput.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/utils/test_random.py` & `streamlink-6.7.3/tests/utils/test_random.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/utils/test_times.py` & `streamlink-6.7.3/tests/utils/test_times.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/utils/test_url.py` & `streamlink-6.7.3/tests/utils/test_url.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/webbrowser/cdp/__init__.py` & `streamlink-6.7.3/tests/webbrowser/cdp/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/webbrowser/cdp/conftest.py` & `streamlink-6.7.3/tests/webbrowser/cdp/conftest.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/webbrowser/cdp/test_client.py` & `streamlink-6.7.3/tests/webbrowser/cdp/test_client.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/webbrowser/cdp/test_connection.py` & `streamlink-6.7.3/tests/webbrowser/cdp/test_connection.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/webbrowser/conftest.py` & `streamlink-6.7.3/tests/webbrowser/conftest.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/webbrowser/test_chromium.py` & `streamlink-6.7.3/tests/webbrowser/test_chromium.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.2/tests/webbrowser/test_webbrowser.py` & `streamlink-6.7.3/tests/webbrowser/test_webbrowser.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from contextlib import AbstractContextManager, nullcontext
 from pathlib import Path
 from signal import SIGTERM
 from typing import List, Optional
 
 import pytest
 import trio
+from exceptiongroup import BaseExceptionGroup
 
 from streamlink.compat import is_win32
 from streamlink.webbrowser.exceptions import WebbrowserError
 from streamlink.webbrowser.webbrowser import Webbrowser
 
 
 class _FakeWebbrowser(Webbrowser):
@@ -94,21 +95,38 @@
         assert [(record.name, record.levelname, record.msg) for record in caplog.records] == [
             ("streamlink.webbrowser.webbrowser", "warning", "Web browser task group has timed out"),
             ("streamlink.webbrowser.webbrowser", "debug", "Waiting for web browser process to terminate"),
         ]
 
     @pytest.mark.trio()
     @pytest.mark.parametrize("exception", [KeyboardInterrupt, SystemExit])
-    async def test_terminate_on_nursery_baseexception(self, caplog: pytest.LogCaptureFixture, webbrowser_launch, exception):
+    async def test_propagate_keyboardinterrupt_systemexit(self, caplog: pytest.LogCaptureFixture, webbrowser_launch, exception):
         process: trio.Process
-        with pytest.raises(exception):  # noqa: PT012
+        with pytest.raises(exception) as excinfo:  # noqa: PT012
             async with webbrowser_launch() as (_nursery, process):
                 assert process.poll() is None, "process is still running"
-                raise exception()
+                async with trio.open_nursery():
+                    raise exception()
 
+        assert isinstance(excinfo.value.__context__, BaseExceptionGroup)
+        assert process.poll() == (1 if is_win32 else -SIGTERM), "Process has been terminated"
+        assert [(record.name, record.levelname, record.msg) for record in caplog.records] == [
+            ("streamlink.webbrowser.webbrowser", "debug", "Waiting for web browser process to terminate"),
+        ]
+
+    @pytest.mark.trio()
+    async def test_terminate_on_exception(self, caplog: pytest.LogCaptureFixture, webbrowser_launch):
+        process: trio.Process
+        with pytest.raises(BaseExceptionGroup) as excinfo:  # noqa: PT012
+            async with webbrowser_launch() as (_nursery, process):
+                assert process.poll() is None, "process is still running"
+                async with trio.open_nursery():
+                    raise ZeroDivisionError()
+
+        assert excinfo.group_contains(ZeroDivisionError)
         assert process.poll() == (1 if is_win32 else -SIGTERM), "Process has been terminated"
         assert [(record.name, record.levelname, record.msg) for record in caplog.records] == [
             ("streamlink.webbrowser.webbrowser", "debug", "Waiting for web browser process to terminate"),
         ]
 
     # don't run on Windows, because of some weird flaky subprocess early-termination issues
     @pytest.mark.posix_only()
```

