# Comparing `tmp/nonebot_plugin_bilichat-5.4.2.tar.gz` & `tmp/nonebot_plugin_bilichat-5.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-5.4.2.tar", last modified: Thu Apr 11 08:29:41 2024, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-5.5.0.tar", last modified: Sun Apr 14 08:55:27 2024, max compression
```

## Comparing `nonebot_plugin_bilichat-5.4.2.tar` & `nonebot_plugin_bilichat-5.5.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0    34523 2024-04-11 08:29:35.533645 nonebot_plugin_bilichat-5.4.2/LICENSE
--rw-r--r--   0        0        0    17759 2024-04-11 08:29:35.533645 nonebot_plugin_bilichat-5.4.2/README.md
--rw-r--r--   0        0        0     2674 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     1120 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/api/__init__.py
--rw-r--r--   0        0        0      740 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/api/base.py
--rw-r--r--   0        0        0     2232 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/api/bilibili_auth.py
--rw-r--r--   0        0        0     1656 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/api/subs_config.py
--rw-r--r--   0        0        0     2686 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/api/webui.py
--rw-r--r--   0        0        0     7799 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/base_content_parsing.py
--rw-r--r--   0        0        0       60 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/commands/__init__.py
--rw-r--r--   0        0        0     1311 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/commands/auto_delete_subs.py
--rw-r--r--   0        0        0     1063 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/commands/base.py
--rw-r--r--   0        0        0      942 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/commands/functions.py
--rw-r--r--   0        0        0     3895 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/commands/login.py
--rw-r--r--   0        0        0     5230 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/commands/subs.py
--rw-r--r--   0        0        0     4996 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/commands/subs_cfg.py
--rw-r--r--   0        0        0     9273 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0       81 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/content/__init__.py
--rw-r--r--   0        0        0     3166 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/content/column.py
--rw-r--r--   0        0        0     4233 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/content/dynamic.py
--rw-r--r--   0        0        0     3942 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/content/video.py
--rw-r--r--   0        0        0      518 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6192 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0      506 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/bilibili_request/__init__.py
--rw-r--r--   0        0        0     2406 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/bilibili_request/auth.py
--rw-r--r--   0        0        0      966 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py
--rw-r--r--   0        0        0     2653 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py
--rw-r--r--   0        0        0     2657 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/browser.py
--rw-r--r--   0        0        0      456 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/cache/__init__.py
--rw-r--r--   0        0        0      437 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/cache/cache.py
--rw-r--r--   0        0        0      871 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/cache/json_cache.py
--rw-r--r--   0        0        0      531 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/cache/mongo_cache.py
--rw-r--r--   0        0        0      521 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/__init__.py
--rw-r--r--   0        0        0      217 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/column/__init__.py
--rw-r--r--   0        0        0     3262 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py
--rw-r--r--   0        0        0      220 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/dynamic/__init__.py
--rw-r--r--   0        0        0     5145 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py
--rw-r--r--   0        0        0     1160 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py
--rw-r--r--   0        0        0     7333 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/video/__init__.py
--rw-r--r--   0        0        0     6326 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py
--rw-r--r--   0        0        0     3040 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/video/style_blue.py
--rw-r--r--   0        0        0     3796 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/fetch_dynamic.py
--rw-r--r--   0        0        0     3376 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      525 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     3115 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     3329 2024-04-11 08:29:35.553645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/text_to_image.py
--rw-r--r--   0        0        0     1732 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/tools.py
--rw-r--r--   0        0        0     1788 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/uid_extract.py
--rw-r--r--   0        0        0     4033 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      568 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/api/__init__.py
--rw-r--r--   0        0        0      184 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/api/bilibili_auth.py
--rw-r--r--   0        0        0      833 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/api/subs_config.py
--rw-r--r--   0        0        0      341 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     3019 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1326 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/bilibili/live.py
--rw-r--r--   0        0        0     1040 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/bilibili/summary.py
--rw-r--r--   0        0        0     1163 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0      323 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      270 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0     9390 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/browser/mobile_style.js
--rw-r--r--   0        0        0     1187 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/style_blue/assets/business.png
--rw-r--r--   0        0        0     1200 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
--rw-r--r--   0        0        0    93905 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
--rw-r--r--   0        0        0     7545 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/style_blue/video-details.html
--rw-r--r--   0        0        0     5777 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/summary/bilibili.png
--rw-r--r--   0        0        0     2098 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/summary/index.html
--rw-r--r--   0        0        0    47433 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/summary/marked.min.js
--rw-r--r--   0        0        0    59199 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/summary/openai.png
--rw-r--r--   0        0        0     9556 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/upload-webui.html
--rw-r--r--   0        0        0   300664 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/webui.tar.gz
--rw-r--r--   0        0        0     2623 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/subscribe/__init__.py
--rw-r--r--   0        0        0     7217 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/subscribe/dynamic.py
--rw-r--r--   0        0        0     4023 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/subscribe/live.py
--rw-r--r--   0        0        0    15576 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/subscribe/manager.py
--rw-r--r--   0        0        0      478 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     4931 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2268 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1615 2024-04-11 08:29:35.557645 nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/wordcloud.py
--rw-r--r--   0        0        0     1754 2024-04-11 08:29:41.597682 nonebot_plugin_bilichat-5.4.2/pyproject.toml
--rw-r--r--   0        0        0    19454 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-5.4.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-14 08:55:23.747255 nonebot_plugin_bilichat-5.5.0/LICENSE
+-rw-r--r--   0        0        0    17907 2024-04-14 08:55:23.747255 nonebot_plugin_bilichat-5.5.0/README.md
+-rw-r--r--   0        0        0     2674 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     1120 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/api/__init__.py
+-rw-r--r--   0        0        0      740 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/api/base.py
+-rw-r--r--   0        0        0     2232 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/api/bilibili_auth.py
+-rw-r--r--   0        0        0     1656 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/api/subs_config.py
+-rw-r--r--   0        0        0     2686 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/api/webui.py
+-rw-r--r--   0        0        0     8214 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/base_content_parsing.py
+-rw-r--r--   0        0        0       60 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/commands/__init__.py
+-rw-r--r--   0        0        0     1311 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/commands/auto_delete_subs.py
+-rw-r--r--   0        0        0     1063 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/commands/base.py
+-rw-r--r--   0        0        0      942 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/commands/functions.py
+-rw-r--r--   0        0        0     3895 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/commands/login.py
+-rw-r--r--   0        0        0     5230 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/commands/subs.py
+-rw-r--r--   0        0        0     4996 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/commands/subs_cfg.py
+-rw-r--r--   0        0        0     9273 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0       81 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/content/__init__.py
+-rw-r--r--   0        0        0     3166 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/content/column.py
+-rw-r--r--   0        0        0     4233 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/content/dynamic.py
+-rw-r--r--   0        0        0     3942 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/content/video.py
+-rw-r--r--   0        0        0      518 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6192 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0      506 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/bilibili_request/__init__.py
+-rw-r--r--   0        0        0     2406 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/bilibili_request/auth.py
+-rw-r--r--   0        0        0      966 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py
+-rw-r--r--   0        0        0     2653 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py
+-rw-r--r--   0        0        0     2657 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/browser.py
+-rw-r--r--   0        0        0      456 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/cache/__init__.py
+-rw-r--r--   0        0        0      437 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/cache/cache.py
+-rw-r--r--   0        0        0      871 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/cache/json_cache.py
+-rw-r--r--   0        0        0      531 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/cache/mongo_cache.py
+-rw-r--r--   0        0        0      521 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/draw/__init__.py
+-rw-r--r--   0        0        0      217 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/draw/column/__init__.py
+-rw-r--r--   0        0        0     3262 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py
+-rw-r--r--   0        0        0      220 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/draw/dynamic/__init__.py
+-rw-r--r--   0        0        0     5145 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py
+-rw-r--r--   0        0        0     1160 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py
+-rw-r--r--   0        0        0     7333 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/draw/video/__init__.py
+-rw-r--r--   0        0        0     6326 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py
+-rw-r--r--   0        0        0     3040 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/draw/video/style_blue.py
+-rw-r--r--   0        0        0     3796 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/fetch_dynamic.py
+-rw-r--r--   0        0        0     3376 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      525 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     3115 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     3329 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/text_to_image.py
+-rw-r--r--   0        0        0     1732 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/tools.py
+-rw-r--r--   0        0        0     1788 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/uid_extract.py
+-rw-r--r--   0        0        0     4033 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      568 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/model/api/__init__.py
+-rw-r--r--   0        0        0      184 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/model/api/bilibili_auth.py
+-rw-r--r--   0        0        0      833 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/model/api/subs_config.py
+-rw-r--r--   0        0        0      448 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     3019 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1326 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/model/bilibili/live.py
+-rw-r--r--   0        0        0     1040 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/model/bilibili/summary.py
+-rw-r--r--   0        0        0     1163 2024-04-14 08:55:23.767255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0      323 2024-04-14 08:55:23.771255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      270 2024-04-14 08:55:23.771255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0     9390 2024-04-14 08:55:23.771255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/static/browser/mobile_style.js
+-rw-r--r--   0        0        0     1187 2024-04-14 08:55:23.771255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png
+-rw-r--r--   0        0        0     1200 2024-04-14 08:55:23.771255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
+-rw-r--r--   0        0        0    93905 2024-04-14 08:55:23.771255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
+-rw-r--r--   0        0        0     7545 2024-04-14 08:55:23.771255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/static/style_blue/video-details.html
+-rw-r--r--   0        0        0     5777 2024-04-14 08:55:23.771255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/static/summary/bilibili.png
+-rw-r--r--   0        0        0     2098 2024-04-14 08:55:23.771255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/static/summary/index.html
+-rw-r--r--   0        0        0    47433 2024-04-14 08:55:23.771255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/static/summary/marked.min.js
+-rw-r--r--   0        0        0    59199 2024-04-14 08:55:23.771255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/static/summary/openai.png
+-rw-r--r--   0        0        0     9556 2024-04-14 08:55:23.771255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/static/upload-webui.html
+-rw-r--r--   0        0        0   300664 2024-04-14 08:55:23.771255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/static/webui.tar.gz
+-rw-r--r--   0        0        0     2623 2024-04-14 08:55:23.771255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/subscribe/__init__.py
+-rw-r--r--   0        0        0     7217 2024-04-14 08:55:23.771255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/subscribe/dynamic.py
+-rw-r--r--   0        0        0     4023 2024-04-14 08:55:23.771255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/subscribe/live.py
+-rw-r--r--   0        0        0    15576 2024-04-14 08:55:23.771255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/subscribe/manager.py
+-rw-r--r--   0        0        0      478 2024-04-14 08:55:23.771255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     4931 2024-04-14 08:55:23.771255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2268 2024-04-14 08:55:23.771255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1615 2024-04-14 08:55:23.771255 nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/wordcloud.py
+-rw-r--r--   0        0        0     1754 2024-04-14 08:55:27.031237 nonebot_plugin_bilichat-5.5.0/pyproject.toml
+-rw-r--r--   0        0        0    19602 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-5.5.0/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-5.4.2/LICENSE` & `nonebot_plugin_bilichat-5.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/README.md` & `nonebot_plugin_bilichat-5.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -290,21 +290,23 @@
 
 在发送视频时，可以额外添加以下类似 shell 指令的参数，进而对解析流程进行调整。例如
 
 ```shell
 BV12v4y1E7NT --refresh
 BV12v4y1E7NT -r # 可以使用简写
 BV12v4y1E7NT -r --no-cache # 可以多个参数混用
+BV12v4y1E7NT -rn # 可以将简写合并，效果同上一条
 -r BV12v4y1E7NT -n # 虽然不建议，但确实可以把参数放前面
 ```
 
 |    指令    | 简写 |                        说明                        |
 | :--------: | :--: | :------------------------------------------------: |
 | --no-cache |  -n  |     本次总结禁用缓存(不会影响已存在的缓存文件)     |
 | --refresh  |  -r  | 刷新此视频的词云和总结缓存(会覆盖已存在的缓存文件) |
+|  --force   |  -f  |             忽略 cd 时间，强制解析视频             |
 
 ### 指令表
 
 指令部分由 `指令前缀` 和 `指令名` 组成，其中 `指令前缀` 包含 `COMMAND_START` `bilichat_cmd_start` `COMMAND_SEP` 三部分，默认的 `指令前缀` 为 `/bilichat.` ，即完整的指令为 `/bilichat.xxx`
 
 `指令前缀` 部分也是可以修改的，例如 .env 中填入如下设置即可实现无 `指令前缀`
```

#### html2text {}

```diff
@@ -138,24 +138,26 @@
 `bilichat_openai_proxy` æå¨å±éæä»£ç 2. ç±äº newbing
 æ¥å£éå¶ä»¥åè½åä¸éï¼ç°å·²ç§»é¤æ¯æ 3.
 å®æ¹æ»ç»ç®åä¸ºåæµç¶æï¼ä¹åæ¥å£éæ¶å¯è½ä¼æååï¼è¯·æ³¨æåæ¶æ´æ°
 ## ð ä½¿ç¨ ç´æ¥åéè§é¢(ä¸æ )é¾æ¥å³å¯ ### åæ°è¡¨
 å¨åéè§é¢æ¶ï¼å¯ä»¥é¢å¤æ·»å ä»¥ä¸ç±»ä¼¼ shell
 æä»¤çåæ°ï¼è¿èå¯¹è§£ææµç¨è¿è¡è°æ´ãä¾å¦ ```shell
 BV12v4y1E7NT --refresh BV12v4y1E7NT -r # å¯ä»¥ä½¿ç¨ç®å BV12v4y1E7NT -r --
-no-cache # å¯ä»¥å¤ä¸ªåæ°æ··ç¨ -r BV12v4y1E7NT -n #
+no-cache # å¯ä»¥å¤ä¸ªåæ°æ··ç¨ BV12v4y1E7NT -rn #
+å¯ä»¥å°ç®ååå¹¶ï¼ææåä¸ä¸æ¡ -r BV12v4y1E7NT -n #
 è½ç¶ä¸å»ºè®®ï¼ä½ç¡®å®å¯ä»¥æåæ°æ¾åé¢ ``` | æä»¤ | ç®å |
 è¯´æ | | :--------: | :--: | :-----------------------------------------------
 -: | | --no-cache | -n | æ¬æ¬¡æ»ç»ç¦ç¨ç¼å­
 (ä¸ä¼å½±åå·²å­å¨çç¼å­æä»¶) | | --refresh | -r |
-å·æ°æ­¤è§é¢çè¯äºåæ»ç»ç¼å­(ä¼è¦çå·²å­å¨çç¼å­æä»¶) |
-### æä»¤è¡¨ æä»¤é¨åç± `æä»¤åç¼` å `æä»¤å` ç»æï¼å¶ä¸­
-`æä»¤åç¼` åå« `COMMAND_START` `bilichat_cmd_start` `COMMAND_SEP`
-ä¸é¨åï¼é»è®¤ç `æä»¤åç¼` ä¸º `/bilichat.` ï¼å³å®æ´çæä»¤ä¸º
-`/bilichat.xxx` `æä»¤åç¼` é¨åä¹æ¯å¯ä»¥ä¿®æ¹çï¼ä¾å¦ .env
+å·æ°æ­¤è§é¢çè¯äºåæ»ç»ç¼å­(ä¼è¦çå·²å­å¨çç¼å­æä»¶) | |
+--force | -f | å¿½ç¥ cd æ¶é´ï¼å¼ºå¶è§£æè§é¢ | ### æä»¤è¡¨
+æä»¤é¨åç± `æä»¤åç¼` å `æä»¤å` ç»æï¼å¶ä¸­ `æä»¤åç¼`
+åå« `COMMAND_START` `bilichat_cmd_start` `COMMAND_SEP` ä¸é¨åï¼é»è®¤ç
+`æä»¤åç¼` ä¸º `/bilichat.` ï¼å³å®æ´çæä»¤ä¸º `/bilichat.xxx`
+`æä»¤åç¼` é¨åä¹æ¯å¯ä»¥ä¿®æ¹çï¼ä¾å¦ .env
 ä¸­å¡«å¥å¦ä¸è®¾ç½®å³å¯å®ç°æ  `æä»¤åç¼` ```dotenv COMMAND_SEP=[""]
 COMMAND_START=[""] bilichat_cmd_start="" ``` `æä»¤å`
 å¦ä¸è¡¨æç¤ºï¼å¶ä¸­é¤ç»å½ç¸å³çæä»¤åå¯èªå®ä¹ï¼å¯åèä¸æç
 [æä»¤åè®¢ééç½®é¡¹](#æä»¤åè®¢ééç½®é¡¹) | æä»¤ | æé |
 èå´ | åæ° | è¯´æ | | :----------: | :----: | :----: | :----------------
 --------------------: | :--------------------------------------: | | sub |
 ä¸»äºº | ç¾¤è | UP ä¸»çæµç§°æ UID | æ·»å è®¢é | | unsub | ä¸»äºº |
```

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/api/__init__.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/api/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/api/base.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/api/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/api/bilibili_auth.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/api/bilibili_auth.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/api/subs_config.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/api/subs_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/api/webui.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/api/webui.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/base_content_parsing.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/base_content_parsing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import re
+import shlex
 import time
 from typing import Dict, Union
 
 from nonebot.adapters import Bot, Event
 from nonebot.exception import FinishedException
 from nonebot.log import logger
 from nonebot.plugin import on_message
@@ -11,15 +12,15 @@
 from nonebot.typing import T_State
 from nonebot_plugin_alconna.uniseg import Hyper, Image, MsgTarget, Reply, Text, UniMessage, UniMsg
 
 from .config import plugin_config
 from .content import Column, Dynamic, Video
 from .lib.b23_extract import b23_extract
 from .lib.text_to_image import t2i
-from .model.arguments import Options
+from .model.arguments import Options, parser
 from .model.exception import AbortError, ProssesError
 from .optional import capture_exception
 
 if plugin_config.bilichat_openai_token:
     from .summary import summarization
 
 if plugin_config.bilichat_word_cloud:
@@ -75,23 +76,23 @@
     if plugin_config.bilichat_only_to_me and not event.is_tome():
         return False
     state["_uid_"] = target.id
     return plugin_config.verify_permission(target.id)
 
 
 async def _bili_check(state: T_State, event: Event, bot: Bot, msg: UniMsg) -> bool:
-    # 检查并提取 raw_bililink
-    try:
-        if plugin_config.bilichat_enable_self and str(event.get_user_id()) == str(bot.self_id) and (Reply in msg):
-            # 是自身消息的情况下，检查是否是回复，是的话则取被回复的消息
-            _msgs = UniMessage(msg[Reply, 0].msg) or msg
-        else:
-            _msgs = msg
-    except Exception:
-        _msgs = msg
+    _msgs = msg.copy()
+    if Reply in msg and (
+        (plugin_config.bilichat_enable_self and str(event.get_user_id()) == str(bot.self_id)) or event.is_tome()
+    ):
+        # 如果是回复消息
+        # 1. 如果是自身消息且允许自身消息
+        # 2. 如果被回复消息中包含对自身的at
+        # 满足上述任一条件，则将被回复的消息的内容添加到待解析的内容中
+        _msgs.append(Text(str(msg[Reply, 0].msg)))
 
     bililink = None
     for _msg in _msgs[Text] + _msgs[Hyper]:
         # b23 格式的链接
         _msg_str = _msg.__repr__()
         if "b23" in _msg_str:
             if b23 := re.search(r"b23.(tv|wtf)[\\/]+(\w+)", _msg_str):  # type: ignore
@@ -103,15 +104,15 @@
                 bililink = _msg_str
                 break
 
     if not bililink:
         return False
 
     content: Union[Column, Video, Dynamic, None] = None
-    options = Options()
+    options: Options = state["_options_"]
 
     try:
         ## video handle
         if matched := re.search(r"av(\d{1,15})|BV(1[A-Za-z0-9]{2}4.1.7[A-Za-z0-9]{2})", bililink):
             _id = matched.group()
             logger.info(f"video id: {_id}")
             content = await Video.from_id(_id, options)
@@ -127,28 +128,36 @@
             matched := re.search(r"(dynamic|opus|t.bilibili.com)/(\d{1,128})", bililink)
         ):
             _id = matched.group()
             logger.info(f"dynamic id: {_id}")
             content = await Dynamic.from_id(_id)
 
         if content:
-            check_cd(f"{state['_uid_']}_-_{content.id}")
+            check_cd(f"{state['_uid_']}_-_{content.id}", check=not options.force)
             state["_content_"] = content
         else:
             raise AbortError(f"查询 {bililink} 返回内容为空")
 
         return True
     except AbortError as e:
         logger.info(e)
         return False
     except FinishedException:
         return False
 
 
+def set_options(state: T_State, msg: UniMsg):
+    options = parser.parse_known_args(args=shlex.split(msg.extract_plain_text()), namespace=Options())[0]
+    state["_options_"] = options
+    if options:
+        logger.info(f"已设置参数: {options}")
+
+
 async def _pre_check(state: T_State, event: Event, bot: Bot, msg: UniMsg, target: MsgTarget):
+    set_options(state, msg)
     return await _permission_check(bot, event, target, state) and await _bili_check(state, event, bot, msg)
 
 
 bilichat = on_message(
     block=plugin_config.bilichat_block,
     priority=1,
     rule=Rule(_pre_check),
```

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/commands/auto_delete_subs.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/commands/auto_delete_subs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/commands/base.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/commands/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/commands/functions.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/commands/functions.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/commands/login.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/commands/login.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/commands/subs.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/commands/subs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/commands/subs_cfg.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/commands/subs_cfg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/content/column.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/content/column.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/content/dynamic.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/content/dynamic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/content/video.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/content/video.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/bilibili_request/auth.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/bilibili_request/auth.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/browser.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/browser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/cache/json_cache.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/cache/json_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/cache/mongo_cache.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/cache/mongo_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/__init__.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/draw/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/video/__init__.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/draw/video/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/draw/video/style_blue.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/draw/video/style_blue.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/fetch_dynamic.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/fetch_dynamic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/store.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/text_to_image.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/tools.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/tools.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/uid_extract.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/uid_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/api/__init__.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/model/api/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/api/subs_config.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/model/api/subs_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/bilibili/live.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/model/bilibili/live.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/bilibili/summary.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/model/bilibili/summary.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/model/exception.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/model/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/browser/mobile_style.js` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/static/browser/mobile_style.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/style_blue/assets/business.png` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/style_blue/assets/personal.png` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/style_blue/video-details.html` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/static/style_blue/video-details.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/summary/bilibili.png` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/static/summary/bilibili.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/summary/index.html` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/static/summary/index.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/summary/marked.min.js` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/static/summary/marked.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/summary/openai.png` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/static/summary/openai.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/upload-webui.html` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/static/upload-webui.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/static/webui.tar.gz` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/static/webui.tar.gz`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/subscribe/__init__.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/subscribe/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/subscribe/dynamic.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/subscribe/dynamic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/subscribe/live.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/subscribe/live.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/subscribe/manager.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/subscribe/manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/nonebot_plugin_bilichat/wordcloud.py` & `nonebot_plugin_bilichat-5.5.0/nonebot_plugin_bilichat/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.4.2/pyproject.toml` & `nonebot_plugin_bilichat-5.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-bilichat"
-version = "5.4.2"
+version = "5.5.0"
 description = "多种B站链接解析，视频词云，AI总结，你想要的都在 bilichat"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "bilireq>=0.2.8",
```

### Comparing `nonebot_plugin_bilichat-5.4.2/PKG-INFO` & `nonebot_plugin_bilichat-5.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 5.4.2
+Version: 5.5.0
 Summary: 多种B站链接解析，视频词云，AI总结，你想要的都在 bilichat
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: bilireq>=0.2.8
 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0
@@ -330,21 +330,23 @@
 
 在发送视频时，可以额外添加以下类似 shell 指令的参数，进而对解析流程进行调整。例如
 
 ```shell
 BV12v4y1E7NT --refresh
 BV12v4y1E7NT -r # 可以使用简写
 BV12v4y1E7NT -r --no-cache # 可以多个参数混用
+BV12v4y1E7NT -rn # 可以将简写合并，效果同上一条
 -r BV12v4y1E7NT -n # 虽然不建议，但确实可以把参数放前面
 ```
 
 |    指令    | 简写 |                        说明                        |
 | :--------: | :--: | :------------------------------------------------: |
 | --no-cache |  -n  |     本次总结禁用缓存(不会影响已存在的缓存文件)     |
 | --refresh  |  -r  | 刷新此视频的词云和总结缓存(会覆盖已存在的缓存文件) |
+|  --force   |  -f  |             忽略 cd 时间，强制解析视频             |
 
 ### 指令表
 
 指令部分由 `指令前缀` 和 `指令名` 组成，其中 `指令前缀` 包含 `COMMAND_START` `bilichat_cmd_start` `COMMAND_SEP` 三部分，默认的 `指令前缀` 为 `/bilichat.` ，即完整的指令为 `/bilichat.xxx`
 
 `指令前缀` 部分也是可以修改的，例如 .env 中填入如下设置即可实现无 `指令前缀`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 5.4.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 5.5.0 Summary:
 å¤ç§Bç«é¾æ¥è§£æï¼è§é¢è¯äºï¼AIæ»ç»ï¼ä½ æ³è¦çé½å¨ bilichat
 Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 bilireq>=0.2.8 Requires-Dist: qrcode>=7.4.2 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot2[fastapi,websockets]>=2.0.0 Requires-Dist: httpx>=0.24.1
@@ -162,24 +162,26 @@
 `bilichat_openai_proxy` æå¨å±éæä»£ç 2. ç±äº newbing
 æ¥å£éå¶ä»¥åè½åä¸éï¼ç°å·²ç§»é¤æ¯æ 3.
 å®æ¹æ»ç»ç®åä¸ºåæµç¶æï¼ä¹åæ¥å£éæ¶å¯è½ä¼æååï¼è¯·æ³¨æåæ¶æ´æ°
 ## ð ä½¿ç¨ ç´æ¥åéè§é¢(ä¸æ )é¾æ¥å³å¯ ### åæ°è¡¨
 å¨åéè§é¢æ¶ï¼å¯ä»¥é¢å¤æ·»å ä»¥ä¸ç±»ä¼¼ shell
 æä»¤çåæ°ï¼è¿èå¯¹è§£ææµç¨è¿è¡è°æ´ãä¾å¦ ```shell
 BV12v4y1E7NT --refresh BV12v4y1E7NT -r # å¯ä»¥ä½¿ç¨ç®å BV12v4y1E7NT -r --
-no-cache # å¯ä»¥å¤ä¸ªåæ°æ··ç¨ -r BV12v4y1E7NT -n #
+no-cache # å¯ä»¥å¤ä¸ªåæ°æ··ç¨ BV12v4y1E7NT -rn #
+å¯ä»¥å°ç®ååå¹¶ï¼ææåä¸ä¸æ¡ -r BV12v4y1E7NT -n #
 è½ç¶ä¸å»ºè®®ï¼ä½ç¡®å®å¯ä»¥æåæ°æ¾åé¢ ``` | æä»¤ | ç®å |
 è¯´æ | | :--------: | :--: | :-----------------------------------------------
 -: | | --no-cache | -n | æ¬æ¬¡æ»ç»ç¦ç¨ç¼å­
 (ä¸ä¼å½±åå·²å­å¨çç¼å­æä»¶) | | --refresh | -r |
-å·æ°æ­¤è§é¢çè¯äºåæ»ç»ç¼å­(ä¼è¦çå·²å­å¨çç¼å­æä»¶) |
-### æä»¤è¡¨ æä»¤é¨åç± `æä»¤åç¼` å `æä»¤å` ç»æï¼å¶ä¸­
-`æä»¤åç¼` åå« `COMMAND_START` `bilichat_cmd_start` `COMMAND_SEP`
-ä¸é¨åï¼é»è®¤ç `æä»¤åç¼` ä¸º `/bilichat.` ï¼å³å®æ´çæä»¤ä¸º
-`/bilichat.xxx` `æä»¤åç¼` é¨åä¹æ¯å¯ä»¥ä¿®æ¹çï¼ä¾å¦ .env
+å·æ°æ­¤è§é¢çè¯äºåæ»ç»ç¼å­(ä¼è¦çå·²å­å¨çç¼å­æä»¶) | |
+--force | -f | å¿½ç¥ cd æ¶é´ï¼å¼ºå¶è§£æè§é¢ | ### æä»¤è¡¨
+æä»¤é¨åç± `æä»¤åç¼` å `æä»¤å` ç»æï¼å¶ä¸­ `æä»¤åç¼`
+åå« `COMMAND_START` `bilichat_cmd_start` `COMMAND_SEP` ä¸é¨åï¼é»è®¤ç
+`æä»¤åç¼` ä¸º `/bilichat.` ï¼å³å®æ´çæä»¤ä¸º `/bilichat.xxx`
+`æä»¤åç¼` é¨åä¹æ¯å¯ä»¥ä¿®æ¹çï¼ä¾å¦ .env
 ä¸­å¡«å¥å¦ä¸è®¾ç½®å³å¯å®ç°æ  `æä»¤åç¼` ```dotenv COMMAND_SEP=[""]
 COMMAND_START=[""] bilichat_cmd_start="" ``` `æä»¤å`
 å¦ä¸è¡¨æç¤ºï¼å¶ä¸­é¤ç»å½ç¸å³çæä»¤åå¯èªå®ä¹ï¼å¯åèä¸æç
 [æä»¤åè®¢ééç½®é¡¹](#æä»¤åè®¢ééç½®é¡¹) | æä»¤ | æé |
 èå´ | åæ° | è¯´æ | | :----------: | :----: | :----: | :----------------
 --------------------: | :--------------------------------------: | | sub |
 ä¸»äºº | ç¾¤è | UP ä¸»çæµç§°æ UID | æ·»å è®¢é | | unsub | ä¸»äºº |
```

