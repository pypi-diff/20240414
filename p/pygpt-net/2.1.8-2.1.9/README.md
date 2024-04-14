# Comparing `tmp/pygpt_net-2.1.8.tar.gz` & `tmp/pygpt_net-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygpt_net-2.1.8.tar", max compression
+gzip compressed data, was "pygpt_net-2.1.9.tar", max compression
```

## Comparing `pygpt_net-2.1.8.tar` & `pygpt_net-2.1.9.tar`

### file list

```diff
@@ -1,707 +1,707 @@
--rwxr-xr-x   0        0        0    42812 2024-03-03 21:57:00.409626 pygpt_net-2.1.8/CHANGELOG.md
--rwxr-xr-x   0        0        0     1077 2024-02-01 17:53:56.362106 pygpt_net-2.1.8/LICENSE
--rwxr-xr-x   0        0        0   124092 2024-03-03 22:16:49.133827 pygpt_net-2.1.8/README.md
--rwxr-xr-x   0        0        0    13970 2024-02-19 21:38:20.920806 pygpt_net-2.1.8/icon.png
--rw-r--r--   0        0        0     2798 2024-03-03 21:58:41.681931 pygpt_net-2.1.8/pyproject.toml
--rwxr-xr-x   0        0        0    41850 2024-03-03 21:57:13.137670 pygpt_net-2.1.8/src/pygpt_net/CHANGELOG.txt
--rwxr-xr-x   0        0        0     1146 2024-02-01 17:53:56.366106 pygpt_net-2.1.8/src/pygpt_net/LICENSE
--rwxr-xr-x   0        0        0      983 2024-03-03 21:59:57.518102 pygpt_net-2.1.8/src/pygpt_net/__init__.py
--rwxr-xr-x   0        0        0    13698 2024-03-03 03:52:54.350656 pygpt_net-2.1.8/src/pygpt_net/app.py
--rwxr-xr-x   0        0        0    11599 2024-02-28 03:58:59.305445 pygpt_net-2.1.8/src/pygpt_net/config.py
--rwxr-xr-x   0        0        0     3350 2024-02-24 01:55:58.445111 pygpt_net-2.1.8/src/pygpt_net/container.py
--rwxr-xr-x   0        0        0     4314 2024-02-15 05:07:04.118540 pygpt_net-2.1.8/src/pygpt_net/controller/__init__.py
--rw-r--r--   0        0        0     4662 2024-02-25 05:32:34.229344 pygpt_net-2.1.8/src/pygpt_net/controller/agent/__init__.py
--rw-r--r--   0        0        0     6569 2024-02-16 04:01:43.038864 pygpt_net-2.1.8/src/pygpt_net/controller/agent/flow.py
--rw-r--r--   0        0        0    10190 2024-02-21 19:09:37.240983 pygpt_net-2.1.8/src/pygpt_net/controller/assistant/__init__.py
--rw-r--r--   0        0        0     9873 2024-02-18 06:49:52.490113 pygpt_net-2.1.8/src/pygpt_net/controller/assistant/editor.py
--rw-r--r--   0        0        0    14478 2024-02-22 03:36:30.096422 pygpt_net-2.1.8/src/pygpt_net/controller/assistant/files.py
--rw-r--r--   0        0        0    12751 2024-02-22 03:36:30.096422 pygpt_net-2.1.8/src/pygpt_net/controller/assistant/threads.py
--rwxr-xr-x   0        0        0    14495 2024-02-22 03:36:30.096422 pygpt_net-2.1.8/src/pygpt_net/controller/attachment.py
--rwxr-xr-x   0        0        0     5234 2024-02-28 03:58:59.305445 pygpt_net-2.1.8/src/pygpt_net/controller/audio.py
--rw-r--r--   0        0        0     4498 2024-03-01 03:17:53.453929 pygpt_net-2.1.8/src/pygpt_net/controller/calendar/__init__.py
--rw-r--r--   0        0        0     7349 2024-03-01 03:17:53.453929 pygpt_net-2.1.8/src/pygpt_net/controller/calendar/note.py
--rwxr-xr-x   0        0        0    12787 2024-02-29 03:07:51.274132 pygpt_net-2.1.8/src/pygpt_net/controller/camera.py
--rw-r--r--   0        0        0     1436 2024-01-13 16:28:42.715718 pygpt_net-2.1.8/src/pygpt_net/controller/chat/__init__.py
--rwxr-xr-x   0        0        0     9758 2024-02-16 04:01:43.038864 pygpt_net-2.1.8/src/pygpt_net/controller/chat/common.py
--rw-r--r--   0        0        0     2149 2024-01-30 20:56:32.772879 pygpt_net-2.1.8/src/pygpt_net/controller/chat/files.py
--rwxr-xr-x   0        0        0     8583 2024-01-31 15:19:17.738030 pygpt_net-2.1.8/src/pygpt_net/controller/chat/image.py
--rwxr-xr-x   0        0        0     8575 2024-02-25 05:32:34.229344 pygpt_net-2.1.8/src/pygpt_net/controller/chat/input.py
--rwxr-xr-x   0        0        0    10083 2024-02-16 04:01:43.038864 pygpt_net-2.1.8/src/pygpt_net/controller/chat/output.py
--rwxr-xr-x   0        0        0     3647 2024-02-17 21:22:47.341663 pygpt_net-2.1.8/src/pygpt_net/controller/chat/render.py
--rw-r--r--   0        0        0    10770 2024-03-03 03:52:54.350656 pygpt_net-2.1.8/src/pygpt_net/controller/chat/text.py
--rw-r--r--   0        0        0     3054 2024-01-30 20:56:32.772879 pygpt_net-2.1.8/src/pygpt_net/controller/chat/vision.py
--rw-r--r--   0        0        0     4408 2024-01-31 21:39:19.384967 pygpt_net-2.1.8/src/pygpt_net/controller/command.py
--rw-r--r--   0        0        0     3885 2024-01-10 11:56:03.088017 pygpt_net-2.1.8/src/pygpt_net/controller/config/__init__.py
--rw-r--r--   0        0        0        0 2024-01-08 20:36:28.054492 pygpt_net-2.1.8/src/pygpt_net/controller/config/field/__init__.py
--rwxr-xr-x   0        0        0     2422 2024-01-30 20:56:32.772879 pygpt_net-2.1.8/src/pygpt_net/controller/config/field/checkbox.py
--rw-r--r--   0        0        0     2335 2024-01-30 20:56:32.772879 pygpt_net-2.1.8/src/pygpt_net/controller/config/field/combo.py
--rw-r--r--   0        0        0     6531 2024-02-25 00:27:02.858945 pygpt_net-2.1.8/src/pygpt_net/controller/config/field/dictionary.py
--rw-r--r--   0        0        0     3312 2024-01-30 20:56:32.772879 pygpt_net-2.1.8/src/pygpt_net/controller/config/field/input.py
--rw-r--r--   0        0        0     4582 2024-01-30 20:56:32.772879 pygpt_net-2.1.8/src/pygpt_net/controller/config/field/slider.py
--rw-r--r--   0        0        0     2281 2024-01-30 20:56:32.772879 pygpt_net-2.1.8/src/pygpt_net/controller/config/field/textarea.py
--rw-r--r--   0        0        0     5219 2024-03-01 17:40:19.825274 pygpt_net-2.1.8/src/pygpt_net/controller/config/placeholder.py
--rw-r--r--   0        0        0    15990 2024-02-27 05:21:39.767084 pygpt_net-2.1.8/src/pygpt_net/controller/ctx/__init__.py
--rw-r--r--   0        0        0     5692 2024-02-23 01:50:39.602419 pygpt_net-2.1.8/src/pygpt_net/controller/ctx/common.py
--rw-r--r--   0        0        0     2552 2024-01-25 22:43:11.543975 pygpt_net-2.1.8/src/pygpt_net/controller/ctx/summarizer.py
--rwxr-xr-x   0        0        0     6527 2024-02-28 03:58:59.305445 pygpt_net-2.1.8/src/pygpt_net/controller/debug.py
--rw-r--r--   0        0        0     1008 2023-12-31 03:09:04.107766 pygpt_net-2.1.8/src/pygpt_net/controller/dialogs/__init__.py
--rwxr-xr-x   0        0        0     6768 2024-02-23 02:31:25.633179 pygpt_net-2.1.8/src/pygpt_net/controller/dialogs/confirm.py
--rw-r--r--   0        0        0     5570 2024-02-25 22:01:41.690831 pygpt_net-2.1.8/src/pygpt_net/controller/dialogs/debug.py
--rwxr-xr-x   0        0        0     2471 2024-02-01 17:53:56.366106 pygpt_net-2.1.8/src/pygpt_net/controller/dialogs/info.py
--rwxr-xr-x   0        0        0    15200 2024-02-16 15:47:42.083541 pygpt_net-2.1.8/src/pygpt_net/controller/files.py
--rw-r--r--   0        0        0     5926 2024-02-23 01:50:39.602419 pygpt_net-2.1.8/src/pygpt_net/controller/idx/__init__.py
--rw-r--r--   0        0        0     2605 2024-02-29 03:07:51.274132 pygpt_net-2.1.8/src/pygpt_net/controller/idx/common.py
--rw-r--r--   0        0        0    17677 2024-02-29 03:07:51.274132 pygpt_net-2.1.8/src/pygpt_net/controller/idx/indexer.py
--rw-r--r--   0        0        0     7789 2024-03-03 03:52:54.350656 pygpt_net-2.1.8/src/pygpt_net/controller/idx/settings.py
--rw-r--r--   0        0        0     2971 2024-01-30 20:56:32.772879 pygpt_net-2.1.8/src/pygpt_net/controller/lang/__init__.py
--rw-r--r--   0        0        0     4016 2024-02-16 20:38:22.742568 pygpt_net-2.1.8/src/pygpt_net/controller/lang/custom.py
--rw-r--r--   0        0        0    13219 2024-02-29 03:07:51.274132 pygpt_net-2.1.8/src/pygpt_net/controller/lang/mapping.py
--rw-r--r--   0        0        0     3879 2024-01-15 13:47:55.919633 pygpt_net-2.1.8/src/pygpt_net/controller/lang/plugins.py
--rw-r--r--   0        0        0     2634 2024-01-22 12:10:21.917245 pygpt_net-2.1.8/src/pygpt_net/controller/lang/settings.py
--rwxr-xr-x   0        0        0     1566 2024-01-04 07:51:17.999390 pygpt_net-2.1.8/src/pygpt_net/controller/launcher.py
--rwxr-xr-x   0        0        0     8825 2024-02-24 01:55:58.445111 pygpt_net-2.1.8/src/pygpt_net/controller/layout.py
--rw-r--r--   0        0        0     6387 2024-02-18 20:56:31.559530 pygpt_net-2.1.8/src/pygpt_net/controller/mode.py
--rw-r--r--   0        0        0     4656 2024-01-30 20:56:32.772879 pygpt_net-2.1.8/src/pygpt_net/controller/model/__init__.py
--rw-r--r--   0        0        0    12599 2024-02-22 03:36:30.096422 pygpt_net-2.1.8/src/pygpt_net/controller/model/editor.py
--rwxr-xr-x   0        0        0     9567 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/controller/notepad.py
--rw-r--r--   0        0        0     2081 2024-02-15 05:07:04.118540 pygpt_net-2.1.8/src/pygpt_net/controller/painter/__init__.py
--rw-r--r--   0        0        0     4461 2024-01-23 23:46:30.495197 pygpt_net-2.1.8/src/pygpt_net/controller/painter/capture.py
--rw-r--r--   0        0        0     6292 2024-02-17 21:22:47.341663 pygpt_net-2.1.8/src/pygpt_net/controller/painter/common.py
--rw-r--r--   0        0        0    12925 2024-02-28 03:58:59.305445 pygpt_net-2.1.8/src/pygpt_net/controller/plugins/__init__.py
--rw-r--r--   0        0        0     5907 2024-02-03 15:51:10.611289 pygpt_net-2.1.8/src/pygpt_net/controller/plugins/settings.py
--rwxr-xr-x   0        0        0    14286 2024-02-18 20:56:31.559530 pygpt_net-2.1.8/src/pygpt_net/controller/presets/__init__.py
--rwxr-xr-x   0        0        0    14915 2024-02-18 20:56:31.559530 pygpt_net-2.1.8/src/pygpt_net/controller/presets/editor.py
--rw-r--r--   0        0        0     6564 2024-02-17 21:22:47.341663 pygpt_net-2.1.8/src/pygpt_net/controller/settings/__init__.py
--rw-r--r--   0        0        0    12750 2024-03-03 03:52:54.350656 pygpt_net-2.1.8/src/pygpt_net/controller/settings/editor.py
--rw-r--r--   0        0        0     5133 2024-01-23 23:46:30.499197 pygpt_net-2.1.8/src/pygpt_net/controller/theme/__init__.py
--rwxr-xr-x   0        0        0     5329 2024-01-27 21:42:30.960980 pygpt_net-2.1.8/src/pygpt_net/controller/theme/common.py
--rw-r--r--   0        0        0     4939 2024-01-23 20:16:03.144694 pygpt_net-2.1.8/src/pygpt_net/controller/theme/markdown.py
--rw-r--r--   0        0        0     3178 2024-01-23 23:46:30.499197 pygpt_net-2.1.8/src/pygpt_net/controller/theme/menu.py
--rw-r--r--   0        0        0     3357 2024-01-27 21:42:30.960980 pygpt_net-2.1.8/src/pygpt_net/controller/theme/nodes.py
--rw-r--r--   0        0        0     4585 2024-01-31 11:15:00.681079 pygpt_net-2.1.8/src/pygpt_net/controller/ui/__init__.py
--rw-r--r--   0        0        0     4936 2024-02-29 03:07:51.274132 pygpt_net-2.1.8/src/pygpt_net/controller/ui/mode.py
--rw-r--r--   0        0        0     1902 2024-01-23 23:46:30.499197 pygpt_net-2.1.8/src/pygpt_net/controller/ui/vision.py
--rw-r--r--   0        0        0        0 2024-01-26 16:05:36.561120 pygpt_net-2.1.8/src/pygpt_net/core/__init__.py
--rw-r--r--   0        0        0     7728 2024-02-21 19:09:37.240983 pygpt_net-2.1.8/src/pygpt_net/core/assistants/__init__.py
--rwxr-xr-x   0        0        0    10240 2024-01-31 15:19:17.738030 pygpt_net-2.1.8/src/pygpt_net/core/attachments.py
--rw-r--r--   0        0        0     2708 2024-02-24 01:55:58.445111 pygpt_net-2.1.8/src/pygpt_net/core/audio.py
--rw-r--r--   0        0        0     3354 2024-01-31 15:19:17.742029 pygpt_net-2.1.8/src/pygpt_net/core/bridge.py
--rw-r--r--   0        0        0     6646 2024-02-02 19:26:46.615683 pygpt_net-2.1.8/src/pygpt_net/core/calendar/__init__.py
--rwxr-xr-x   0        0        0     4034 2024-02-21 16:18:39.952987 pygpt_net-2.1.8/src/pygpt_net/core/camera.py
--rw-r--r--   0        0        0     3130 2024-01-27 01:08:27.560991 pygpt_net-2.1.8/src/pygpt_net/core/chain/__init__.py
--rw-r--r--   0        0        0     4656 2024-01-27 01:08:27.560991 pygpt_net-2.1.8/src/pygpt_net/core/chain/chat.py
--rw-r--r--   0        0        0     5089 2024-01-27 01:08:27.560991 pygpt_net-2.1.8/src/pygpt_net/core/chain/completion.py
--rwxr-xr-x   0        0        0     9759 2024-02-16 04:01:43.038864 pygpt_net-2.1.8/src/pygpt_net/core/command.py
--rw-r--r--   0        0        0    22242 2024-02-27 05:21:39.767084 pygpt_net-2.1.8/src/pygpt_net/core/ctx/__init__.py
--rw-r--r--   0        0        0     7709 2024-02-27 05:21:39.767084 pygpt_net-2.1.8/src/pygpt_net/core/ctx/idx.py
--rw-r--r--   0        0        0     6519 2024-01-23 23:46:30.499197 pygpt_net-2.1.8/src/pygpt_net/core/db/__init__.py
--rwxr-xr-x   0        0        0     7586 2024-02-22 03:36:30.096422 pygpt_net-2.1.8/src/pygpt_net/core/debug/__init__.py
--rw-r--r--   0        0        0     1467 2024-02-25 18:06:16.205368 pygpt_net-2.1.8/src/pygpt_net/core/debug/agent.py
--rwxr-xr-x   0        0        0     2259 2024-02-25 22:01:41.690831 pygpt_net-2.1.8/src/pygpt_net/core/debug/assistants.py
--rwxr-xr-x   0        0        0     1626 2024-02-25 22:01:41.690831 pygpt_net-2.1.8/src/pygpt_net/core/debug/attachments.py
--rwxr-xr-x   0        0        0     1458 2024-02-25 22:01:41.690831 pygpt_net-2.1.8/src/pygpt_net/core/debug/config.py
--rwxr-xr-x   0        0        0     5314 2024-02-28 03:58:59.309445 pygpt_net-2.1.8/src/pygpt_net/core/debug/context.py
--rw-r--r--   0        0        0     3377 2024-02-27 05:21:39.767084 pygpt_net-2.1.8/src/pygpt_net/core/debug/indexes.py
--rwxr-xr-x   0        0        0     1848 2024-02-25 22:01:41.690831 pygpt_net-2.1.8/src/pygpt_net/core/debug/models.py
--rwxr-xr-x   0        0        0     1258 2024-02-25 22:01:41.690831 pygpt_net-2.1.8/src/pygpt_net/core/debug/plugins.py
--rwxr-xr-x   0        0        0     1994 2024-02-25 22:01:41.690831 pygpt_net-2.1.8/src/pygpt_net/core/debug/presets.py
--rwxr-xr-x   0        0        0     2666 2024-02-25 22:01:41.690831 pygpt_net-2.1.8/src/pygpt_net/core/debug/ui.py
--rwxr-xr-x   0        0        0     7384 2024-03-03 21:20:56.988059 pygpt_net-2.1.8/src/pygpt_net/core/dispatcher.py
--rw-r--r--   0        0        0     7678 2024-02-21 19:09:37.240983 pygpt_net-2.1.8/src/pygpt_net/core/filesystem.py
--rwxr-xr-x   0        0        0     3092 2024-01-23 23:46:30.499197 pygpt_net-2.1.8/src/pygpt_net/core/history.py
--rwxr-xr-x   0        0        0    14729 2024-03-01 17:40:19.825274 pygpt_net-2.1.8/src/pygpt_net/core/idx/__init__.py
--rwxr-xr-x   0        0        0     9660 2024-03-03 21:20:56.980059 pygpt_net-2.1.8/src/pygpt_net/core/idx/chat.py
--rw-r--r--   0        0        0     2226 2024-02-28 03:58:59.309445 pygpt_net-2.1.8/src/pygpt_net/core/idx/context.py
--rwxr-xr-x   0        0        0    24729 2024-03-03 21:20:57.028059 pygpt_net-2.1.8/src/pygpt_net/core/idx/indexing.py
--rw-r--r--   0        0        0     2656 2024-02-28 03:58:59.309445 pygpt_net-2.1.8/src/pygpt_net/core/idx/llm.py
--rw-r--r--   0        0        0        0 2024-02-27 05:21:39.767084 pygpt_net-2.1.8/src/pygpt_net/core/idx/types/__init__.py
--rw-r--r--   0        0        0     3113 2024-02-27 05:21:39.767084 pygpt_net-2.1.8/src/pygpt_net/core/idx/types/ctx.py
--rw-r--r--   0        0        0     4722 2024-02-27 05:21:39.767084 pygpt_net-2.1.8/src/pygpt_net/core/idx/types/external.py
--rw-r--r--   0        0        0     3733 2024-02-27 05:21:39.771084 pygpt_net-2.1.8/src/pygpt_net/core/idx/types/files.py
--rw-r--r--   0        0        0     2766 2024-02-28 03:58:59.309445 pygpt_net-2.1.8/src/pygpt_net/core/idx/worker.py
--rwxr-xr-x   0        0        0     4629 2024-02-22 03:36:30.096422 pygpt_net-2.1.8/src/pygpt_net/core/image.py
--rwxr-xr-x   0        0        0      829 2023-12-31 03:18:56.426282 pygpt_net-2.1.8/src/pygpt_net/core/info.py
--rw-r--r--   0        0        0     2040 2024-01-11 15:56:53.273343 pygpt_net-2.1.8/src/pygpt_net/core/installer.py
--rw-r--r--   0        0        0     1168 2024-01-14 15:51:20.622630 pygpt_net-2.1.8/src/pygpt_net/core/llm/__init__.py
--rwxr-xr-x   0        0        0     4814 2024-01-23 23:46:30.499197 pygpt_net-2.1.8/src/pygpt_net/core/locale.py
--rw-r--r--   0        0        0     7573 2024-01-27 21:42:30.960980 pygpt_net-2.1.8/src/pygpt_net/core/models.py
--rw-r--r--   0        0        0     1913 2024-01-23 23:46:30.499197 pygpt_net-2.1.8/src/pygpt_net/core/modes.py
--rwxr-xr-x   0        0        0     3270 2024-01-27 21:42:30.960980 pygpt_net-2.1.8/src/pygpt_net/core/notepad.py
--rwxr-xr-x   0        0        0     4214 2024-01-23 23:46:30.499197 pygpt_net-2.1.8/src/pygpt_net/core/platforms.py
--rwxr-xr-x   0        0        0     8576 2024-02-24 01:55:58.445111 pygpt_net-2.1.8/src/pygpt_net/core/plugins.py
--rw-r--r--   0        0        0     9286 2024-02-01 18:18:38.554891 pygpt_net-2.1.8/src/pygpt_net/core/presets.py
--rw-r--r--   0        0        0     2167 2024-02-27 03:03:23.430567 pygpt_net-2.1.8/src/pygpt_net/core/prompt.py
--rw-r--r--   0        0        0      489 2024-01-05 12:12:41.797675 pygpt_net-2.1.8/src/pygpt_net/core/render/__init__.py
--rw-r--r--   0        0        0     2454 2024-02-17 21:22:47.341663 pygpt_net-2.1.8/src/pygpt_net/core/render/base.py
--rw-r--r--   0        0        0      489 2024-01-05 12:12:41.797675 pygpt_net-2.1.8/src/pygpt_net/core/render/markdown/__init__.py
--rwxr-xr-x   0        0        0     3111 2024-02-22 04:14:57.246812 pygpt_net-2.1.8/src/pygpt_net/core/render/markdown/parser.py
--rwxr-xr-x   0        0        0    14959 2024-02-21 19:09:37.240983 pygpt_net-2.1.8/src/pygpt_net/core/render/markdown/renderer.py
--rw-r--r--   0        0        0      489 2024-01-05 13:07:04.262555 pygpt_net-2.1.8/src/pygpt_net/core/render/plain/__init__.py
--rw-r--r--   0        0        0    12471 2024-02-17 21:22:47.341663 pygpt_net-2.1.8/src/pygpt_net/core/render/plain/renderer.py
--rwxr-xr-x   0        0        0     6333 2024-02-17 21:22:47.341663 pygpt_net-2.1.8/src/pygpt_net/core/settings.py
--rwxr-xr-x   0        0        0    14040 2024-02-25 18:06:16.205368 pygpt_net-2.1.8/src/pygpt_net/core/tokens.py
--rw-r--r--   0        0        0    13722 2024-02-21 19:09:37.240983 pygpt_net-2.1.8/src/pygpt_net/core/updater/__init__.py
--rw-r--r--   0        0        0     2343 2024-02-24 01:55:58.445111 pygpt_net-2.1.8/src/pygpt_net/core/web.py
--rw-r--r--   0        0        0      901 2024-01-25 22:43:11.543975 pygpt_net-2.1.8/src/pygpt_net/core/worker.py
--rwxr-xr-x   0        0        0     7554 2024-03-03 21:59:28.970043 pygpt_net-2.1.8/src/pygpt_net/data/config/config.json
--rwxr-xr-x   0        0        0    14349 2024-03-03 21:59:25.190035 pygpt_net-2.1.8/src/pygpt_net/data/config/models.json
--rw-r--r--   0        0        0     1440 2024-03-03 21:59:22.502029 pygpt_net-2.1.8/src/pygpt_net/data/config/modes.json
--rwxr-xr-x   0        0        0      459 2024-01-13 13:04:53.113674 pygpt_net-2.1.8/src/pygpt_net/data/config/presets/batman_and_joker.json
--rw-r--r--   0        0        0     2702 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/config/presets/current.agent.json
--rwxr-xr-x   0        0        0      368 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/config/presets/current.assistant.json
--rwxr-xr-x   0        0        0      396 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/config/presets/current.chat.json
--rwxr-xr-x   0        0        0      385 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/config/presets/current.completion.json
--rwxr-xr-x   0        0        0      368 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/config/presets/current.img.json
--rwxr-xr-x   0        0        0      382 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/config/presets/current.langchain.json
--rw-r--r--   0        0        0      368 2024-03-03 02:59:46.037803 pygpt_net-2.1.8/src/pygpt_net/data/config/presets/current.llama_index.json
--rwxr-xr-x   0        0        0      392 2024-03-03 03:52:54.350656 pygpt_net-2.1.8/src/pygpt_net/data/config/presets/current.vision.json
--rwxr-xr-x   0        0        0      501 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/config/presets/dalle_white_cat.json
--rwxr-xr-x   0        0        0    23013 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/data/config/settings.json
--rw-r--r--   0        0        0      736 2024-02-01 17:53:56.366106 pygpt_net-2.1.8/src/pygpt_net/data/config/settings_section.json
--rw-r--r--   0        0        0      664 2024-01-20 12:18:41.475899 pygpt_net-2.1.8/src/pygpt_net/data/css/fix_windows.css
--rw-r--r--   0        0        0      489 2024-01-04 08:28:16.417936 pygpt_net-2.1.8/src/pygpt_net/data/css/markdown.css
--rw-r--r--   0        0        0      516 2024-01-23 23:46:30.499197 pygpt_net-2.1.8/src/pygpt_net/data/css/markdown.dark.css
--rw-r--r--   0        0        0      461 2024-01-23 23:46:30.499197 pygpt_net-2.1.8/src/pygpt_net/data/css/markdown.light.css
--rw-r--r--   0        0        0      400 2024-01-12 03:59:56.290336 pygpt_net-2.1.8/src/pygpt_net/data/css/style.css
--rw-r--r--   0        0        0      559 2024-01-27 21:42:30.960980 pygpt_net-2.1.8/src/pygpt_net/data/css/style.dark.css
--rw-r--r--   0        0        0     1157 2024-01-27 21:42:30.960980 pygpt_net-2.1.8/src/pygpt_net/data/css/style.light.css
--rwxr-xr-x   0        0        0    69484 2023-12-08 15:03:16.000000 pygpt_net-2.1.8/src/pygpt_net/data/fonts/Lato/Lato-Black.ttf
--rwxr-xr-x   0        0        0    71948 2023-12-08 15:03:16.000000 pygpt_net-2.1.8/src/pygpt_net/data/fonts/Lato/Lato-BlackItalic.ttf
--rwxr-xr-x   0        0        0    73316 2023-12-08 15:03:16.000000 pygpt_net-2.1.8/src/pygpt_net/data/fonts/Lato/Lato-Bold.ttf
--rwxr-xr-x   0        0        0    77680 2023-12-08 15:03:16.000000 pygpt_net-2.1.8/src/pygpt_net/data/fonts/Lato/Lato-BoldItalic.ttf
--rwxr-xr-x   0        0        0    75744 2023-12-08 15:03:16.000000 pygpt_net-2.1.8/src/pygpt_net/data/fonts/Lato/Lato-Italic.ttf
--rwxr-xr-x   0        0        0    77192 2023-12-08 15:03:16.000000 pygpt_net-2.1.8/src/pygpt_net/data/fonts/Lato/Lato-Light.ttf
--rwxr-xr-x   0        0        0    49064 2023-12-08 15:03:16.000000 pygpt_net-2.1.8/src/pygpt_net/data/fonts/Lato/Lato-LightItalic.ttf
--rwxr-xr-x   0        0        0    75136 2023-12-08 15:03:16.000000 pygpt_net-2.1.8/src/pygpt_net/data/fonts/Lato/Lato-Regular.ttf
--rwxr-xr-x   0        0        0    69968 2023-12-08 15:03:16.000000 pygpt_net-2.1.8/src/pygpt_net/data/fonts/Lato/Lato-Thin.ttf
--rwxr-xr-x   0        0        0    48848 2023-12-08 15:03:16.000000 pygpt_net-2.1.8/src/pygpt_net/data/fonts/Lato/Lato-ThinItalic.ttf
--rwxr-xr-x   0        0        0     4500 2023-12-08 15:03:16.000000 pygpt_net-2.1.8/src/pygpt_net/data/fonts/Lato/OFL.txt
--rwxr-xr-x   0        0        0     3461 2023-04-14 00:10:28.000000 pygpt_net-2.1.8/src/pygpt_net/data/icon.ico
--rwxr-xr-x   0        0        0    13970 2023-04-14 00:10:28.000000 pygpt_net-2.1.8/src/pygpt_net/data/icon.png
--rw-r--r--   0        0        0     5471 2024-01-29 18:11:38.035830 pygpt_net-2.1.8/src/pygpt_net/data/icon_tray_busy.ico
--rw-r--r--   0        0        0    14837 2024-01-29 18:11:38.035830 pygpt_net-2.1.8/src/pygpt_net/data/icon_tray_error.ico
--rw-r--r--   0        0        0     4209 2024-01-29 18:11:38.035830 pygpt_net-2.1.8/src/pygpt_net/data/icon_tray_idle.ico
--rw-r--r--   0        0        0      538 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/abc.svg
--rw-r--r--   0        0        0      178 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/add.svg
--rw-r--r--   0        0        0      463 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/add_circle.svg
--rw-r--r--   0        0        0      348 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/add_folder.svg
--rw-r--r--   0        0        0      391 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/add_library.svg
--rw-r--r--   0        0        0      558 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/alarm.svg
--rw-r--r--   0        0        0     1027 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/apps.svg
--rw-r--r--   0        0        0      267 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/asterisk.svg
--rw-r--r--   0        0        0      429 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/attachment.svg
--rw-r--r--   0        0        0      422 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/attachments.svg
--rw-r--r--   0        0        0      185 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/back.svg
--rw-r--r--   0        0        0      395 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/backspace.svg
--rw-r--r--   0        0        0      472 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/block.svg
--rw-r--r--   0        0        0      255 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/bookmark.svg
--rw-r--r--   0        0        0      423 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/brush.svg
--rw-r--r--   0        0        0      523 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/build.svg
--rw-r--r--   0        0        0      927 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/calendar.svg
--rw-r--r--   0        0        0      496 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/camera.svg
--rw-r--r--   0        0        0      336 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/chat.svg
--rw-r--r--   0        0        0      174 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/check.svg
--rw-r--r--   0        0        0      459 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/check_circle.svg
--rw-r--r--   0        0        0      265 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/checklist.svg
--rw-r--r--   0        0        0      406 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/circle.svg
--rw-r--r--   0        0        0      191 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/clear.svg
--rw-r--r--   0        0        0      411 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/clock.svg
--rw-r--r--   0        0        0      218 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/close.svg
--rw-r--r--   0        0        0      503 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/close_circle.svg
--rw-r--r--   0        0        0      224 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/code.svg
--rw-r--r--   0        0        0      298 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/computer.svg
--rw-r--r--   0        0        0      336 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/copy.svg
--rw-r--r--   0        0        0      264 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/crop.svg
--rw-r--r--   0        0        0      666 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/cut.svg
--rw-r--r--   0        0        0      725 2024-01-30 17:23:19.885579 pygpt_net-2.1.8/src/pygpt_net/data/icons/db.svg
--rw-r--r--   0        0        0      271 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/delete.svg
--rw-r--r--   0        0        0      174 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/done.svg
--rw-r--r--   0        0        0      274 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/download.svg
--rw-r--r--   0        0        0      283 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/draft.svg
--rw-r--r--   0        0        0      323 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/drag.svg
--rw-r--r--   0        0        0      325 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/edit.svg
--rw-r--r--   0        0        0      497 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/emergency.svg
--rw-r--r--   0        0        0      195 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/equalizer.svg
--rw-r--r--   0        0        0      533 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/error.svg
--rw-r--r--   0        0        0      372 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/event_available.svg
--rw-r--r--   0        0        0      174 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/expand.svg
--rw-r--r--   0        0        0      247 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/fast_forward.svg
--rw-r--r--   0        0        0      250 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/fast_rewind.svg
--rw-r--r--   0        0        0      504 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/favorite.svg
--rw-r--r--   0        0        0      297 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/folder.svg
--rw-r--r--   0        0        0      249 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/folder_filled.svg
--rw-r--r--   0        0        0      186 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/forward.svg
--rw-r--r--   0        0        0      194 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/full.svg
--rw-r--r--   0        0        0      249 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/fullscreen.svg
--rw-r--r--   0        0        0      459 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/grid.svg
--rw-r--r--   0        0        0      602 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/hearing.svg
--rw-r--r--   0        0        0      691 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/help.svg
--rw-r--r--   0        0        0      440 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/history.svg
--rw-r--r--   0        0        0      239 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/home.svg
--rw-r--r--   0        0        0      176 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/home_filled.svg
--rw-r--r--   0        0        0      323 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/image.svg
--rw-r--r--   0        0        0      531 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/info.svg
--rw-r--r--   0        0        0      337 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/input.svg
--rw-r--r--   0        0        0      541 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/key.svg
--rw-r--r--   0        0        0      517 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/keyboard.svg
--rw-r--r--   0        0        0      972 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/language.svg
--rw-r--r--   0        0        0      491 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/list.svg
--rw-r--r--   0        0        0      495 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/lock.svg
--rw-r--r--   0        0        0      273 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/logout.svg
--rw-r--r--   0        0        0      392 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/map.svg
--rw-r--r--   0        0        0      431 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/memory.svg
--rw-r--r--   0        0        0      189 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/menu.svg
--rw-r--r--   0        0        0      447 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/mic.svg
--rw-r--r--   0        0        0      485 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/mic_off.svg
--rw-r--r--   0        0        0      423 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/more_horizontal.svg
--rw-r--r--   0        0        0      491 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/mute.svg
--rw-r--r--   0        0        0      296 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/open_tab.svg
--rw-r--r--   0        0        0      846 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/palette.svg
--rw-r--r--   0        0        0      431 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/paste.svg
--rw-r--r--   0        0        0      250 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/pause.svg
--rw-r--r--   0        0        0      454 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/pause_circle.svg
--rw-r--r--   0        0        0      377 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/photos.svg
--rw-r--r--   0        0        0      441 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/pin.svg
--rw-r--r--   0        0        0      186 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/play.svg
--rw-r--r--   0        0        0      197 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/play_pause.svg
--rw-r--r--   0        0        0      246 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/playlist_add.svg
--rw-r--r--   0        0        0      318 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/power.svg
--rw-r--r--   0        0        0      478 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/print.svg
--rw-r--r--   0        0        0      598 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/public_filled.svg
--rw-r--r--   0        0        0      283 2024-01-30 20:56:32.772879 pygpt_net-2.1.8/src/pygpt_net/data/icons/redo.svg
--rw-r--r--   0        0        0      329 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/reload.svg
--rw-r--r--   0        0        0      260 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/repeat.svg
--rw-r--r--   0        0        0      400 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/replay.svg
--rw-r--r--   0        0        0      401 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/resize.svg
--rw-r--r--   0        0        0      615 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/robot.svg
--rw-r--r--   0        0        0      807 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/router.svg
--rw-r--r--   0        0        0      384 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/save.svg
--rw-r--r--   0        0        0      469 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/schedule.svg
--rw-r--r--   0        0        0      396 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/screenshot.svg
--rw-r--r--   0        0        0      372 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/search.svg
--rw-r--r--   0        0        0      274 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/security.svg
--rw-r--r--   0        0        0      660 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/sensors.svg
--rw-r--r--   0        0        0      767 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/settings.svg
--rw-r--r--   0        0        0      475 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/settings_filled.svg
--rw-r--r--   0        0        0      792 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/share.svg
--rw-r--r--   0        0        0      469 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/shedule.svg
--rw-r--r--   0        0        0      189 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/sort.svg
--rw-r--r--   0        0        0      386 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/stack.svg
--rw-r--r--   0        0        0      306 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/stacks.svg
--rw-r--r--   0        0        0      291 2024-01-30 17:23:19.889579 pygpt_net-2.1.8/src/pygpt_net/data/icons/star.svg
--rw-r--r--   0        0        0      188 2024-01-30 17:23:19.893578 pygpt_net-2.1.8/src/pygpt_net/data/icons/stop.svg
--rw-r--r--   0        0        0      432 2024-01-30 17:23:19.893578 pygpt_net-2.1.8/src/pygpt_net/data/icons/stop_circle.svg
--rw-r--r--   0        0        0      381 2024-01-30 17:23:19.893578 pygpt_net-2.1.8/src/pygpt_net/data/icons/sync.svg
--rw-r--r--   0        0        0      317 2024-01-30 17:23:19.893578 pygpt_net-2.1.8/src/pygpt_net/data/icons/tag.svg
--rw-r--r--   0        0        0      334 2024-01-30 17:23:19.893578 pygpt_net-2.1.8/src/pygpt_net/data/icons/task.svg
--rw-r--r--   0        0        0      336 2024-01-30 17:23:19.893578 pygpt_net-2.1.8/src/pygpt_net/data/icons/terminal.svg
--rw-r--r--   0        0        0      204 2024-01-30 17:23:19.893578 pygpt_net-2.1.8/src/pygpt_net/data/icons/text.svg
--rw-r--r--   0        0        0      329 2024-01-30 17:23:19.893578 pygpt_net-2.1.8/src/pygpt_net/data/icons/textfile.svg
--rw-r--r--   0        0        0      479 2024-01-30 17:23:19.893578 pygpt_net-2.1.8/src/pygpt_net/data/icons/timer.svg
--rw-r--r--   0        0        0      321 2024-01-30 17:23:19.893578 pygpt_net-2.1.8/src/pygpt_net/data/icons/today.svg
--rw-r--r--   0        0        0      308 2024-01-30 17:23:19.893578 pygpt_net-2.1.8/src/pygpt_net/data/icons/tune.svg
--rw-r--r--   0        0        0      282 2024-01-30 17:23:19.893578 pygpt_net-2.1.8/src/pygpt_net/data/icons/undo.svg
--rw-r--r--   0        0        0      444 2024-01-30 17:23:19.893578 pygpt_net-2.1.8/src/pygpt_net/data/icons/update.svg
--rw-r--r--   0        0        0      392 2024-01-30 17:23:19.893578 pygpt_net-2.1.8/src/pygpt_net/data/icons/updater.svg
--rw-r--r--   0        0        0      276 2024-01-30 17:23:19.893578 pygpt_net-2.1.8/src/pygpt_net/data/icons/upload.svg
--rw-r--r--   0        0        0      339 2024-01-30 17:23:19.893578 pygpt_net-2.1.8/src/pygpt_net/data/icons/video.svg
--rw-r--r--   0        0        0      550 2024-01-30 17:23:19.893578 pygpt_net-2.1.8/src/pygpt_net/data/icons/view.svg
--rw-r--r--   0        0        0      736 2024-01-30 17:23:19.893578 pygpt_net-2.1.8/src/pygpt_net/data/icons/voice.svg
--rw-r--r--   0        0        0      374 2024-01-30 17:23:19.893578 pygpt_net-2.1.8/src/pygpt_net/data/icons/volume.svg
--rw-r--r--   0        0        0      310 2024-01-30 17:23:19.893578 pygpt_net-2.1.8/src/pygpt_net/data/icons/warning.svg
--rw-r--r--   0        0        0      300 2024-01-30 17:23:19.893578 pygpt_net-2.1.8/src/pygpt_net/data/icons/webcam.svg
--rw-r--r--   0        0        0      375 2024-02-29 03:07:51.274132 pygpt_net-2.1.8/src/pygpt_net/data/icons/webcam_off.svg
--rw-r--r--   0        0        0      325 2024-01-30 17:23:19.893578 pygpt_net-2.1.8/src/pygpt_net/data/icons/width.svg
--rw-r--r--   0        0        0      336 2024-01-30 17:23:19.893578 pygpt_net-2.1.8/src/pygpt_net/data/icons/window.svg
--rw-r--r--   0        0        0      365 2024-01-30 17:23:19.893578 pygpt_net-2.1.8/src/pygpt_net/data/icons/work.svg
--rw-r--r--   0        0        0      422 2024-01-30 17:23:19.893578 pygpt_net-2.1.8/src/pygpt_net/data/icons/zoom_in.svg
--rw-r--r--   0        0        0      396 2024-01-30 17:23:19.893578 pygpt_net-2.1.8/src/pygpt_net/data/icons/zoom_out.svg
--rwxr-xr-x   0        0        0    29134 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/data/locale/locale.de.ini
--rwxr-xr-x   0        0        0    34612 2024-03-02 19:51:00.168984 pygpt_net-2.1.8/src/pygpt_net/data/locale/locale.en.ini
--rwxr-xr-x   0        0        0    29222 2024-03-01 17:40:19.825274 pygpt_net-2.1.8/src/pygpt_net/data/locale/locale.es.ini
--rwxr-xr-x   0        0        0    30122 2024-03-01 17:40:19.825274 pygpt_net-2.1.8/src/pygpt_net/data/locale/locale.fr.ini
--rwxr-xr-x   0        0        0    28666 2024-03-01 17:40:19.825274 pygpt_net-2.1.8/src/pygpt_net/data/locale/locale.it.ini
--rwxr-xr-x   0        0        0    28477 2024-03-01 17:40:19.825274 pygpt_net-2.1.8/src/pygpt_net/data/locale/locale.pl.ini
--rwxr-xr-x   0        0        0    40413 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/data/locale/locale.ua.ini
--rwxr-xr-x   0        0        0     1532 2024-02-25 05:32:34.229344 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.agent.en.ini
--rwxr-xr-x   0        0        0     1713 2024-02-25 05:32:34.229344 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.agent.pl.ini
--rwxr-xr-x   0        0        0     8006 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.audio_input.en.ini
--rwxr-xr-x   0        0        0     7599 2024-02-28 03:58:59.309445 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.audio_input.pl.ini
--rwxr-xr-x   0        0        0     2293 2024-02-25 00:27:02.862945 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.audio_output.en.ini
--rwxr-xr-x   0        0        0     1390 2024-02-24 01:55:58.445111 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.audio_output.pl.ini
--rw-r--r--   0        0        0      766 2024-02-25 05:32:34.229344 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.cmd_api.en.ini
--rw-r--r--   0        0        0      850 2024-02-26 21:30:35.305131 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.cmd_api.pl.ini
--rwxr-xr-x   0        0        0     2353 2024-02-16 20:38:22.746568 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.en.ini
--rwxr-xr-x   0        0        0     2573 2024-02-16 20:38:22.746568 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.pl.ini
--rwxr-xr-x   0        0        0      455 2024-02-25 05:32:34.229344 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.cmd_custom.en.ini
--rwxr-xr-x   0        0        0      527 2024-01-30 20:56:32.776879 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.cmd_custom.pl.ini
--rwxr-xr-x   0        0        0     7909 2024-03-03 20:35:02.756782 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.cmd_files.en.ini
--rwxr-xr-x   0        0        0     7492 2024-02-25 05:32:34.229344 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.cmd_files.pl.ini
--rw-r--r--   0        0        0     3998 2024-02-15 05:07:04.118540 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.cmd_history.en.ini
--rw-r--r--   0        0        0     4450 2024-02-04 17:46:05.314114 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.cmd_history.pl.ini
--rw-r--r--   0        0        0     1992 2024-01-30 20:56:32.776879 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.cmd_serial.en.ini
--rw-r--r--   0        0        0     2186 2024-01-30 20:56:32.776879 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.cmd_serial.pl.ini
--rwxr-xr-x   0        0        0     5863 2024-03-01 17:40:19.825274 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.cmd_web.en.ini
--rwxr-xr-x   0        0        0     6485 2024-03-01 17:40:19.825274 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.cmd_web.pl.ini
--rw-r--r--   0        0        0      888 2024-02-01 23:02:10.688691 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.crontab.en.ini
--rw-r--r--   0        0        0     1014 2024-02-01 23:02:10.688691 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.crontab.pl.ini
--rw-r--r--   0        0        0      409 2024-01-30 20:56:32.776879 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.extra_prompt.en.ini
--rw-r--r--   0        0        0      474 2024-01-30 20:56:32.776879 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.extra_prompt.pl.ini
--rw-r--r--   0        0        0     2407 2024-03-03 05:47:23.540140 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.idx_llama_index.en.ini
--rw-r--r--   0        0        0     1090 2024-01-30 20:56:32.776879 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.idx_llama_index.pl.ini
--rw-r--r--   0        0        0      592 2024-01-30 20:56:32.776879 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.openai_dalle.en.ini
--rw-r--r--   0        0        0      609 2024-01-30 20:56:32.776879 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.openai_dalle.pl.ini
--rw-r--r--   0        0        0     1576 2024-02-15 05:07:04.118540 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.openai_vision.en.ini
--rw-r--r--   0        0        0     1764 2024-01-30 20:56:32.776879 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.openai_vision.pl.ini
--rwxr-xr-x   0        0        0      631 2024-01-30 20:56:32.776879 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.real_time.en.ini
--rwxr-xr-x   0        0        0      752 2024-01-30 20:56:32.776879 pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.real_time.pl.ini
--rwxr-xr-x   0        0        0    19418 2023-12-14 19:08:45.000000 pygpt_net-2.1.8/src/pygpt_net/data/logo.png
--rwxr-xr-x   0        0        0    31708 2024-02-20 19:10:03.189314 pygpt_net-2.1.8/src/pygpt_net/data/win32/README.rtf
--rwxr-xr-x   0        0        0     1633 2023-04-14 00:10:28.000000 pygpt_net-2.1.8/src/pygpt_net/data/win32/USER-LICENSE.rtf
--rwxr-xr-x   0        0        0    87160 2023-04-14 00:10:28.000000 pygpt_net-2.1.8/src/pygpt_net/data/win32/pygpt.aip
--rwxr-xr-x   0        0        0       45 2023-12-19 15:40:13.000000 pygpt_net-2.1.8/src/pygpt_net/data/win32/qt.conf
--rw-r--r--   0        0        0    21736 2024-03-02 20:04:01.386329 pygpt_net-2.1.8/src/pygpt_net/icons.qrc
--rw-r--r--   0        0        0    90430 2024-03-02 20:05:43.048414 pygpt_net-2.1.8/src/pygpt_net/icons_rc.py
--rw-r--r--   0        0        0      488 2023-12-31 03:12:36.955235 pygpt_net-2.1.8/src/pygpt_net/item/__init__.py
--rw-r--r--   0        0        0     5063 2024-02-21 00:32:47.130497 pygpt_net-2.1.8/src/pygpt_net/item/assistant.py
--rw-r--r--   0        0        0     1816 2024-01-27 21:42:30.960980 pygpt_net-2.1.8/src/pygpt_net/item/attachment.py
--rw-r--r--   0        0        0     2108 2024-01-27 21:42:30.960980 pygpt_net-2.1.8/src/pygpt_net/item/calendar_note.py
--rw-r--r--   0        0        0     9629 2024-03-03 21:20:56.984059 pygpt_net-2.1.8/src/pygpt_net/item/ctx.py
--rw-r--r--   0        0        0     1681 2024-01-27 21:42:30.960980 pygpt_net-2.1.8/src/pygpt_net/item/index.py
--rw-r--r--   0        0        0      600 2023-12-31 03:12:34.283242 pygpt_net-2.1.8/src/pygpt_net/item/mode.py
--rw-r--r--   0        0        0     6208 2024-01-27 21:42:30.960980 pygpt_net-2.1.8/src/pygpt_net/item/model.py
--rw-r--r--   0        0        0     1508 2024-01-27 21:42:30.960980 pygpt_net-2.1.8/src/pygpt_net/item/notepad.py
--rw-r--r--   0        0        0     4052 2024-02-15 05:07:04.122540 pygpt_net-2.1.8/src/pygpt_net/item/preset.py
--rwxr-xr-x   0        0        0     6616 2024-02-24 01:55:58.445111 pygpt_net-2.1.8/src/pygpt_net/launcher.py
--rw-r--r--   0        0        0     2849 2023-12-28 02:55:13.572642 pygpt_net-2.1.8/src/pygpt_net/migrations/Version20231227152900.py
--rw-r--r--   0        0        0      906 2023-12-30 08:47:37.360628 pygpt_net-2.1.8/src/pygpt_net/migrations/Version20231230095000.py
--rw-r--r--   0        0        0      901 2024-01-01 00:17:57.553256 pygpt_net-2.1.8/src/pygpt_net/migrations/Version20231231230000.py
--rw-r--r--   0        0        0     1303 2024-01-06 06:27:36.351928 pygpt_net-2.1.8/src/pygpt_net/migrations/Version20240106060000.py
--rw-r--r--   0        0        0      865 2024-01-07 09:35:02.638810 pygpt_net-2.1.8/src/pygpt_net/migrations/Version20240107060000.py
--rw-r--r--   0        0        0     1756 2024-02-23 01:50:39.602419 pygpt_net-2.1.8/src/pygpt_net/migrations/Version20240222160000.py
--rw-r--r--   0        0        0     1099 2024-02-23 06:06:25.510176 pygpt_net-2.1.8/src/pygpt_net/migrations/Version20240223050000.py
--rw-r--r--   0        0        0      847 2024-03-03 21:20:56.972059 pygpt_net-2.1.8/src/pygpt_net/migrations/Version20240303190000.py
--rw-r--r--   0        0        0     1635 2024-03-03 21:20:57.064058 pygpt_net-2.1.8/src/pygpt_net/migrations/__init__.py
--rw-r--r--   0        0        0      614 2023-12-28 02:55:13.572642 pygpt_net-2.1.8/src/pygpt_net/migrations/base.py
--rwxr-xr-x   0        0        0      488 2023-12-25 22:13:46.802302 pygpt_net-2.1.8/src/pygpt_net/plugin/__init__.py
--rwxr-xr-x   0        0        0    14479 2024-02-25 05:32:34.229344 pygpt_net-2.1.8/src/pygpt_net/plugin/agent/__init__.py
--rwxr-xr-x   0        0        0    22052 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/plugin/audio_input/__init__.py
--rw-r--r--   0        0        0     3787 2024-02-28 03:58:59.309445 pygpt_net-2.1.8/src/pygpt_net/plugin/audio_input/simple.py
--rw-r--r--   0        0        0     9606 2024-02-28 03:58:59.309445 pygpt_net-2.1.8/src/pygpt_net/plugin/audio_input/worker.py
--rwxr-xr-x   0        0        0     6589 2024-02-24 01:55:58.445111 pygpt_net-2.1.8/src/pygpt_net/plugin/audio_output/__init__.py
--rw-r--r--   0        0        0     1759 2024-02-24 01:55:58.445111 pygpt_net-2.1.8/src/pygpt_net/plugin/audio_output/worker.py
--rwxr-xr-x   0        0        0     9046 2024-03-03 21:20:57.032059 pygpt_net-2.1.8/src/pygpt_net/plugin/base.py
--rwxr-xr-x   0        0        0    11627 2024-02-25 05:32:34.229344 pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_api/__init__.py
--rw-r--r--   0        0        0     6823 2024-02-25 00:58:54.512534 pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_api/worker.py
--rwxr-xr-x   0        0        0     7757 2024-02-18 06:49:52.494117 pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_code_interpreter/__init__.py
--rw-r--r--   0        0        0    10352 2024-03-03 21:20:57.048059 pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_code_interpreter/runner.py
--rw-r--r--   0        0        0     4749 2024-03-03 21:20:57.052059 pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_code_interpreter/worker.py
--rwxr-xr-x   0        0        0     5717 2024-02-25 00:27:02.862945 pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_custom/__init__.py
--rw-r--r--   0        0        0     4409 2024-02-25 00:27:02.862945 pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_custom/worker.py
--rwxr-xr-x   0        0        0    16853 2024-03-03 21:20:57.040059 pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_files/__init__.py
--rw-r--r--   0        0        0    32180 2024-03-03 21:29:10.322943 pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_files/worker.py
--rwxr-xr-x   0        0        0    23473 2024-02-15 05:07:04.122540 pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_history/__init__.py
--rwxr-xr-x   0        0        0     6969 2024-02-18 06:49:52.494117 pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_serial/__init__.py
--rw-r--r--   0        0        0     8680 2024-01-30 17:23:19.897578 pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_serial/worker.py
--rwxr-xr-x   0        0        0    19314 2024-03-01 17:40:19.825274 pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_web/__init__.py
--rwxr-xr-x   0        0        0    12576 2024-02-24 01:55:58.445111 pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_web/websearch.py
--rw-r--r--   0        0        0     7762 2024-03-01 17:40:19.825274 pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_web/worker.py
--rwxr-xr-x   0        0        0     8158 2024-02-15 05:07:04.122540 pygpt_net-2.1.8/src/pygpt_net/plugin/crontab/__init__.py
--rwxr-xr-x   0        0        0     2831 2024-02-18 01:14:49.758062 pygpt_net-2.1.8/src/pygpt_net/plugin/extra_prompt/__init__.py
--rwxr-xr-x   0        0        0    13103 2024-03-03 21:20:56.964059 pygpt_net-2.1.8/src/pygpt_net/plugin/idx_llama_index/__init__.py
--rwxr-xr-x   0        0        0     6330 2024-02-15 05:07:04.122540 pygpt_net-2.1.8/src/pygpt_net/plugin/openai_dalle/__init__.py
--rwxr-xr-x   0        0        0    11455 2024-02-15 05:07:04.122540 pygpt_net-2.1.8/src/pygpt_net/plugin/openai_vision/__init__.py
--rwxr-xr-x   0        0        0     4029 2024-02-04 17:46:05.314114 pygpt_net-2.1.8/src/pygpt_net/plugin/real_time/__init__.py
--rw-r--r--   0        0        0      488 2023-12-25 22:13:46.802302 pygpt_net-2.1.8/src/pygpt_net/provider/__init__.py
--rw-r--r--   0        0        0      488 2024-02-24 01:55:58.445111 pygpt_net-2.1.8/src/pygpt_net/provider/audio_input/__init__.py
--rw-r--r--   0        0        0     1819 2024-02-27 05:21:39.771084 pygpt_net-2.1.8/src/pygpt_net/provider/audio_input/base.py
--rw-r--r--   0        0        0     2818 2024-02-27 05:21:39.771084 pygpt_net-2.1.8/src/pygpt_net/provider/audio_input/bing_speech_recognition.py
--rw-r--r--   0        0        0     2904 2024-02-27 05:21:39.771084 pygpt_net-2.1.8/src/pygpt_net/provider/audio_input/google_cloud_speech_recognition.py
--rw-r--r--   0        0        0     2840 2024-02-27 05:21:39.771084 pygpt_net-2.1.8/src/pygpt_net/provider/audio_input/google_speech_recognition.py
--rw-r--r--   0        0        0     2244 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/provider/audio_input/openai_whisper.py
--rw-r--r--   0        0        0     3129 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/provider/audio_input/openai_whisper_local.py
--rw-r--r--   0        0        0      488 2024-02-24 01:55:58.449111 pygpt_net-2.1.8/src/pygpt_net/provider/audio_output/__init__.py
--rw-r--r--   0        0        0     1995 2024-02-27 05:21:39.771084 pygpt_net-2.1.8/src/pygpt_net/provider/audio_output/base.py
--rw-r--r--   0        0        0     4231 2024-02-25 00:27:02.862945 pygpt_net-2.1.8/src/pygpt_net/provider/audio_output/eleven_labs.py
--rw-r--r--   0        0        0     4286 2024-02-25 00:27:02.862945 pygpt_net-2.1.8/src/pygpt_net/provider/audio_output/google_tts.py
--rw-r--r--   0        0        0     4960 2024-02-24 01:55:58.449111 pygpt_net-2.1.8/src/pygpt_net/provider/audio_output/ms_azure_tts.py
--rw-r--r--   0        0        0     3056 2024-02-24 01:55:58.449111 pygpt_net-2.1.8/src/pygpt_net/provider/audio_output/openai_tts.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.1.8/src/pygpt_net/provider/core/__init__.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.1.8/src/pygpt_net/provider/core/assistant/__init__.py
--rw-r--r--   0        0        0     1186 2024-01-23 23:46:30.499197 pygpt_net-2.1.8/src/pygpt_net/provider/core/assistant/base.py
--rw-r--r--   0        0        0     5926 2024-01-23 23:46:30.499197 pygpt_net-2.1.8/src/pygpt_net/provider/core/assistant/json_file.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.1.8/src/pygpt_net/provider/core/attachment/__init__.py
--rw-r--r--   0        0        0     1204 2024-01-23 23:46:30.499197 pygpt_net-2.1.8/src/pygpt_net/provider/core/attachment/base.py
--rw-r--r--   0        0        0     5236 2024-01-23 23:46:30.499197 pygpt_net-2.1.8/src/pygpt_net/provider/core/attachment/json_file.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.1.8/src/pygpt_net/provider/core/calendar/__init__.py
--rw-r--r--   0        0        0     1322 2024-01-23 23:46:30.499197 pygpt_net-2.1.8/src/pygpt_net/provider/core/calendar/base.py
--rw-r--r--   0        0        0     3832 2024-02-02 19:26:46.619683 pygpt_net-2.1.8/src/pygpt_net/provider/core/calendar/db_sqlite/__init__.py
--rw-r--r--   0        0        0      837 2024-01-23 23:46:30.499197 pygpt_net-2.1.8/src/pygpt_net/provider/core/calendar/db_sqlite/patch.py
--rw-r--r--   0        0        0    10959 2024-01-23 23:46:30.499197 pygpt_net-2.1.8/src/pygpt_net/provider/core/calendar/db_sqlite/storage.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.1.8/src/pygpt_net/provider/core/config/__init__.py
--rw-r--r--   0        0        0     1235 2024-01-23 23:46:30.499197 pygpt_net-2.1.8/src/pygpt_net/provider/core/config/base.py
--rwxr-xr-x   0        0        0     5017 2024-01-23 23:46:30.499197 pygpt_net-2.1.8/src/pygpt_net/provider/core/config/json_file.py
--rwxr-xr-x   0        0        0    57082 2024-03-03 21:20:57.012059 pygpt_net-2.1.8/src/pygpt_net/provider/core/config/patch.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.1.8/src/pygpt_net/provider/core/ctx/__init__.py
--rw-r--r--   0        0        0     2085 2024-02-23 01:50:39.602419 pygpt_net-2.1.8/src/pygpt_net/provider/core/ctx/base.py
--rw-r--r--   0        0        0     7059 2024-02-23 01:50:39.602419 pygpt_net-2.1.8/src/pygpt_net/provider/core/ctx/db_sqlite/__init__.py
--rw-r--r--   0        0        0     3101 2024-01-23 23:46:30.499197 pygpt_net-2.1.8/src/pygpt_net/provider/core/ctx/db_sqlite/patch.py
--rw-r--r--   0        0        0    23675 2024-03-03 21:20:57.000059 pygpt_net-2.1.8/src/pygpt_net/provider/core/ctx/db_sqlite/storage.py
--rw-r--r--   0        0        0     6888 2024-03-03 21:20:57.036059 pygpt_net-2.1.8/src/pygpt_net/provider/core/ctx/db_sqlite/utils.py
--rw-r--r--   0        0        0    11665 2024-01-23 23:46:30.503197 pygpt_net-2.1.8/src/pygpt_net/provider/core/ctx/json_file.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.1.8/src/pygpt_net/provider/core/history/__init__.py
--rw-r--r--   0        0        0      863 2024-01-23 23:46:30.503197 pygpt_net-2.1.8/src/pygpt_net/provider/core/history/base.py
--rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.1.8/src/pygpt_net/provider/core/history/patch.py
--rw-r--r--   0        0        0     2969 2024-01-23 23:46:30.503197 pygpt_net-2.1.8/src/pygpt_net/provider/core/history/txt_file.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.1.8/src/pygpt_net/provider/core/index/__init__.py
--rw-r--r--   0        0        0     2814 2024-02-23 06:06:25.510176 pygpt_net-2.1.8/src/pygpt_net/provider/core/index/base.py
--rw-r--r--   0        0        0     8217 2024-02-23 06:06:25.510176 pygpt_net-2.1.8/src/pygpt_net/provider/core/index/db_sqlite/__init__.py
--rw-r--r--   0        0        0     2972 2024-02-23 06:06:25.510176 pygpt_net-2.1.8/src/pygpt_net/provider/core/index/db_sqlite/patch.py
--rw-r--r--   0        0        0    16519 2024-02-23 06:06:25.510176 pygpt_net-2.1.8/src/pygpt_net/provider/core/index/db_sqlite/storage.py
--rw-r--r--   0        0        0      870 2024-02-23 01:50:39.606418 pygpt_net-2.1.8/src/pygpt_net/provider/core/index/db_sqlite/utils.py
--rw-r--r--   0        0        0     6615 2024-02-23 01:50:39.606418 pygpt_net-2.1.8/src/pygpt_net/provider/core/index/json_file.py
--rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.1.8/src/pygpt_net/provider/core/index/patch.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.1.8/src/pygpt_net/provider/core/mode/__init__.py
--rw-r--r--   0        0        0     1062 2024-01-23 23:46:30.503197 pygpt_net-2.1.8/src/pygpt_net/provider/core/mode/base.py
--rw-r--r--   0        0        0     4142 2024-01-23 23:46:30.503197 pygpt_net-2.1.8/src/pygpt_net/provider/core/mode/json_file.py
--rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.1.8/src/pygpt_net/provider/core/mode/patch.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.1.8/src/pygpt_net/provider/core/model/__init__.py
--rw-r--r--   0        0        0     1246 2024-01-23 23:46:30.503197 pygpt_net-2.1.8/src/pygpt_net/provider/core/model/base.py
--rw-r--r--   0        0        0     6231 2024-01-23 23:46:30.503197 pygpt_net-2.1.8/src/pygpt_net/provider/core/model/json_file.py
--rw-r--r--   0        0        0     7363 2024-01-30 21:49:30.562821 pygpt_net-2.1.8/src/pygpt_net/provider/core/model/patch.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.1.8/src/pygpt_net/provider/core/notepad/__init__.py
--rw-r--r--   0        0        0     1262 2024-01-23 23:46:30.503197 pygpt_net-2.1.8/src/pygpt_net/provider/core/notepad/base.py
--rw-r--r--   0        0        0     3044 2024-01-23 23:46:30.503197 pygpt_net-2.1.8/src/pygpt_net/provider/core/notepad/db_sqlite/__init__.py
--rw-r--r--   0        0        0     2805 2024-01-23 23:46:30.503197 pygpt_net-2.1.8/src/pygpt_net/provider/core/notepad/db_sqlite/patch.py
--rw-r--r--   0        0        0     7263 2024-01-23 23:46:30.503197 pygpt_net-2.1.8/src/pygpt_net/provider/core/notepad/db_sqlite/storage.py
--rw-r--r--   0        0        0     7555 2024-01-23 23:46:30.503197 pygpt_net-2.1.8/src/pygpt_net/provider/core/notepad/json_file.py
--rwxr-xr-x   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.1.8/src/pygpt_net/provider/core/preset/__init__.py
--rwxr-xr-x   0        0        0     1300 2024-02-01 01:48:09.374583 pygpt_net-2.1.8/src/pygpt_net/provider/core/preset/base.py
--rwxr-xr-x   0        0        0     7887 2024-02-15 05:07:04.122540 pygpt_net-2.1.8/src/pygpt_net/provider/core/preset/json_file.py
--rw-r--r--   0        0        0     3166 2024-01-23 23:46:30.503197 pygpt_net-2.1.8/src/pygpt_net/provider/core/preset/patch.py
--rw-r--r--   0        0        0     6739 2024-02-21 03:55:24.484309 pygpt_net-2.1.8/src/pygpt_net/provider/gpt/__init__.py
--rw-r--r--   0        0        0    13251 2024-02-21 19:09:37.240983 pygpt_net-2.1.8/src/pygpt_net/provider/gpt/assistants.py
--rw-r--r--   0        0        0     5763 2024-02-15 05:07:04.122540 pygpt_net-2.1.8/src/pygpt_net/provider/gpt/chat.py
--rw-r--r--   0        0        0     5169 2024-01-27 01:08:27.560991 pygpt_net-2.1.8/src/pygpt_net/provider/gpt/completion.py
--rw-r--r--   0        0        0     7904 2024-02-18 06:49:52.494117 pygpt_net-2.1.8/src/pygpt_net/provider/gpt/image.py
--rw-r--r--   0        0        0     2681 2024-01-27 01:08:27.560991 pygpt_net-2.1.8/src/pygpt_net/provider/gpt/summarizer.py
--rw-r--r--   0        0        0     7079 2024-02-16 04:34:22.756884 pygpt_net-2.1.8/src/pygpt_net/provider/gpt/vision.py
--rw-r--r--   0        0        0        0 2024-02-20 19:10:03.189314 pygpt_net-2.1.8/src/pygpt_net/provider/gpt/worker/__init__.py
--rw-r--r--   0        0        0     5916 2024-02-21 00:32:47.130497 pygpt_net-2.1.8/src/pygpt_net/provider/gpt/worker/assistants.py
--rw-r--r--   0        0        0     4665 2024-02-21 19:09:37.240983 pygpt_net-2.1.8/src/pygpt_net/provider/gpt/worker/importer.py
--rwxr-xr-x   0        0        0        0 2024-01-27 21:42:30.960980 pygpt_net-2.1.8/src/pygpt_net/provider/llms/__init__.py
--rwxr-xr-x   0        0        0     1641 2024-01-27 21:42:30.960980 pygpt_net-2.1.8/src/pygpt_net/provider/llms/anthropic.py
--rwxr-xr-x   0        0        0     1633 2024-02-28 03:58:59.309445 pygpt_net-2.1.8/src/pygpt_net/provider/llms/azure_openai.py
--rw-r--r--   0        0        0     2694 2024-01-27 21:42:30.960980 pygpt_net-2.1.8/src/pygpt_net/provider/llms/base.py
--rwxr-xr-x   0        0        0     1535 2024-01-27 21:42:30.960980 pygpt_net-2.1.8/src/pygpt_net/provider/llms/hugging_face.py
--rwxr-xr-x   0        0        0     1643 2024-01-27 21:42:30.960980 pygpt_net-2.1.8/src/pygpt_net/provider/llms/llama.py
--rwxr-xr-x   0        0        0     1517 2024-01-27 21:42:30.960980 pygpt_net-2.1.8/src/pygpt_net/provider/llms/ollama.py
--rwxr-xr-x   0        0        0     2048 2024-02-28 03:58:59.309445 pygpt_net-2.1.8/src/pygpt_net/provider/llms/openai.py
--rw-r--r--   0        0        0        0 2024-01-23 23:46:30.503197 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/__init__.py
--rw-r--r--   0        0        0     2481 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/base.py
--rw-r--r--   0        0        0     1149 2024-02-29 03:07:51.278132 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/file_csv.py
--rw-r--r--   0        0        0     1032 2024-02-29 03:07:51.278132 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/file_docx.py
--rw-r--r--   0        0        0     1022 2024-02-29 03:07:51.278132 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/file_epub.py
--rw-r--r--   0        0        0     1032 2024-02-28 03:58:59.309445 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/file_excel.py
--rw-r--r--   0        0        0     1163 2024-02-29 03:07:51.278132 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/file_html.py
--rw-r--r--   0        0        0     1680 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/file_image_vision.py
--rw-r--r--   0        0        0     1169 2024-02-29 03:07:51.278132 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/file_ipynb.py
--rw-r--r--   0        0        0      996 2024-02-28 03:58:59.309445 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/file_json.py
--rw-r--r--   0        0        0     1171 2024-02-29 03:07:51.278132 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/file_markdown.py
--rw-r--r--   0        0        0     1127 2024-02-29 03:07:51.278132 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/file_pdf.py
--rw-r--r--   0        0        0     1720 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/file_video_audio.py
--rw-r--r--   0        0        0     1114 2024-02-29 03:07:51.278132 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/file_xml.py
--rw-r--r--   0        0        0        0 2024-01-27 21:42:30.960980 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/__init__.py
--rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/bitbucket/__init__.py
--rw-r--r--   0        0        0     6194 2024-03-01 17:40:19.825274 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/bitbucket/repo.py
--rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/__init__.py
--rw-r--r--   0        0        0     2460 2024-03-01 17:40:19.825274 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/base.py
--rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/database/__init__.py
--rw-r--r--   0        0        0     4228 2024-03-01 17:40:19.825274 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/database/base.py
--rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/github/__init__.py
--rw-r--r--   0        0        0     4204 2024-03-01 17:40:19.825274 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/github/issues.py
--rw-r--r--   0        0        0     3550 2024-03-01 17:40:19.825274 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/github/repo.py
--rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/google/__init__.py
--rw-r--r--   0        0        0     2658 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/google/calendar.py
--rw-r--r--   0        0        0     5370 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/google/docs.py
--rw-r--r--   0        0        0     6772 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/google/gmail.py
--rw-r--r--   0        0        0     1633 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/google/keep.py
--rw-r--r--   0        0        0     5282 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/google/sheets.py
--rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/image_vision/__init__.py
--rw-r--r--   0        0        0     6940 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/image_vision/base.py
--rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/json/__init__.py
--rw-r--r--   0        0        0     3862 2024-02-29 03:07:51.278132 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/json/base.py
--rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/pandas_excel/__init__.py
--rw-r--r--   0        0        0     3940 2024-02-29 03:07:51.278132 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/pandas_excel/base.py
--rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/simple_csv/__init__.py
--rw-r--r--   0        0        0     1481 2024-02-29 03:07:51.278132 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/simple_csv/base.py
--rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/video_audio/__init__.py
--rw-r--r--   0        0        0     4960 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/video_audio/base.py
--rw-r--r--   0        0        0        0 2024-02-27 05:21:39.771084 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/web_page/__init__.py
--rw-r--r--   0        0        0      556 2024-02-29 03:07:51.278132 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/web_page/base.py
--rw-r--r--   0        0        0        0 2024-02-27 05:21:39.771084 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/yt/__init__.py
--rw-r--r--   0        0        0     2427 2024-02-29 03:07:51.278132 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/yt/base.py
--rw-r--r--   0        0        0      545 2024-02-27 05:21:39.771084 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/yt/utils.py
--rw-r--r--   0        0        0     3078 2024-03-01 17:40:19.825274 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_bitbucket.py
--rw-r--r--   0        0        0     2280 2024-03-01 17:40:19.825274 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_chatgpt_retrieval.py
--rw-r--r--   0        0        0     2392 2024-03-01 17:40:19.825274 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_database.py
--rw-r--r--   0        0        0     3223 2024-03-01 17:40:19.825274 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_github_issues.py
--rw-r--r--   0        0        0     3556 2024-03-01 17:40:19.825274 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_github_repo.py
--rw-r--r--   0        0        0     2499 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_google_calendar.py
--rw-r--r--   0        0        0     2236 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_google_docs.py
--rw-r--r--   0        0        0     3180 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_google_drive.py
--rw-r--r--   0        0        0     2319 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_google_gmail.py
--rw-r--r--   0        0        0     2201 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_google_keep.py
--rw-r--r--   0        0        0     2313 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_google_sheets.py
--rw-r--r--   0        0        0     3443 2024-03-01 17:40:19.825274 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_microsoft_onedrive.py
--rw-r--r--   0        0        0     1399 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_page.py
--rw-r--r--   0        0        0     1404 2024-03-01 03:17:53.457929 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_rss.py
--rw-r--r--   0        0        0     1575 2024-03-01 03:17:53.461929 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_sitemap.py
--rw-r--r--   0        0        0     2512 2024-03-03 03:52:54.350656 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_twitter.py
--rw-r--r--   0        0        0     1442 2024-03-01 03:17:53.461929 pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_yt.py
--rw-r--r--   0        0        0     5396 2024-03-03 21:20:56.944060 pygpt_net-2.1.8/src/pygpt_net/provider/vector_stores/__init__.py
--rw-r--r--   0        0        0     3112 2024-02-28 03:58:59.313445 pygpt_net-2.1.8/src/pygpt_net/provider/vector_stores/base.py
--rwxr-xr-x   0        0        0     3169 2024-03-03 03:52:54.350656 pygpt_net-2.1.8/src/pygpt_net/provider/vector_stores/chroma.py
--rw-r--r--   0        0        0     3152 2024-02-28 03:58:59.313445 pygpt_net-2.1.8/src/pygpt_net/provider/vector_stores/elasticsearch.py
--rw-r--r--   0        0        0     5177 2024-02-28 03:58:59.313445 pygpt_net-2.1.8/src/pygpt_net/provider/vector_stores/pinecode.py
--rw-r--r--   0        0        0     3183 2024-02-28 03:58:59.313445 pygpt_net-2.1.8/src/pygpt_net/provider/vector_stores/redis.py
--rw-r--r--   0        0        0     2524 2024-02-28 03:58:59.313445 pygpt_net-2.1.8/src/pygpt_net/provider/vector_stores/simple.py
--rw-r--r--   0        0        0     3923 2024-03-03 21:20:57.016059 pygpt_net-2.1.8/src/pygpt_net/provider/vector_stores/temp.py
--rw-r--r--   0        0        0      488 2024-02-24 01:55:58.449111 pygpt_net-2.1.8/src/pygpt_net/provider/web/__init__.py
--rw-r--r--   0        0        0     1994 2024-02-27 05:21:39.771084 pygpt_net-2.1.8/src/pygpt_net/provider/web/base.py
--rw-r--r--   0        0        0     4646 2024-02-25 00:27:02.862945 pygpt_net-2.1.8/src/pygpt_net/provider/web/google_custom_search.py
--rw-r--r--   0        0        0     4104 2024-02-25 00:27:02.862945 pygpt_net-2.1.8/src/pygpt_net/provider/web/microsoft_bing.py
--rwxr-xr-x   0        0        0     5680 2024-01-29 18:11:38.035830 pygpt_net-2.1.8/src/pygpt_net/ui/__init__.py
--rw-r--r--   0        0        0        0 2024-01-08 20:36:28.054492 pygpt_net-2.1.8/src/pygpt_net/ui/base/__init__.py
--rw-r--r--   0        0        0     9209 2024-02-27 05:21:39.771084 pygpt_net-2.1.8/src/pygpt_net/ui/base/config_dialog.py
--rwxr-xr-x   0        0        0      488 2023-12-28 18:11:19.000000 pygpt_net-2.1.8/src/pygpt_net/ui/dialog/__init__.py
--rwxr-xr-x   0        0        0     5579 2024-02-28 03:58:59.313445 pygpt_net-2.1.8/src/pygpt_net/ui/dialog/about.py
--rwxr-xr-x   0        0        0     4722 2024-02-15 05:07:04.122540 pygpt_net-2.1.8/src/pygpt_net/ui/dialog/applog.py
--rwxr-xr-x   0        0        0     6534 2024-02-15 05:07:04.122540 pygpt_net-2.1.8/src/pygpt_net/ui/dialog/assistant.py
--rwxr-xr-x   0        0        0     1765 2024-02-01 17:53:56.370106 pygpt_net-2.1.8/src/pygpt_net/ui/dialog/changelog.py
--rw-r--r--   0        0        0      973 2024-01-28 19:32:28.495073 pygpt_net-2.1.8/src/pygpt_net/ui/dialog/create.py
--rwxr-xr-x   0        0        0     1798 2024-02-26 21:30:35.305131 pygpt_net-2.1.8/src/pygpt_net/ui/dialog/debug.py
--rw-r--r--   0        0        0     5490 2024-01-31 21:39:19.388967 pygpt_net-2.1.8/src/pygpt_net/ui/dialog/dictionary.py
--rwxr-xr-x   0        0        0     2382 2024-01-27 21:42:30.964980 pygpt_net-2.1.8/src/pygpt_net/ui/dialog/editor.py
--rwxr-xr-x   0        0        0     2867 2024-01-19 21:21:41.774598 pygpt_net-2.1.8/src/pygpt_net/ui/dialog/image.py
--rwxr-xr-x   0        0        0     2272 2024-02-01 17:53:56.370106 pygpt_net-2.1.8/src/pygpt_net/ui/dialog/license.py
--rwxr-xr-x   0        0        0     1706 2024-01-27 21:42:30.964980 pygpt_net-2.1.8/src/pygpt_net/ui/dialog/logger.py
--rw-r--r--   0        0        0    12634 2024-02-15 05:07:04.122540 pygpt_net-2.1.8/src/pygpt_net/ui/dialog/models.py
--rwxr-xr-x   0        0        0    19464 2024-03-02 19:51:00.168984 pygpt_net-2.1.8/src/pygpt_net/ui/dialog/plugins.py
--rwxr-xr-x   0        0        0     6644 2024-02-15 05:07:04.122540 pygpt_net-2.1.8/src/pygpt_net/ui/dialog/preset.py
--rwxr-xr-x   0        0        0      973 2024-01-28 19:32:28.495073 pygpt_net-2.1.8/src/pygpt_net/ui/dialog/rename.py
--rwxr-xr-x   0        0        0    14557 2024-02-29 03:07:51.278132 pygpt_net-2.1.8/src/pygpt_net/ui/dialog/settings.py
--rw-r--r--   0        0        0      954 2024-02-26 22:26:37.124323 pygpt_net-2.1.8/src/pygpt_net/ui/dialog/snap.py
--rwxr-xr-x   0        0        0     2436 2024-02-25 05:55:37.513980 pygpt_net-2.1.8/src/pygpt_net/ui/dialog/start.py
--rwxr-xr-x   0        0        0      842 2023-12-28 18:11:19.000000 pygpt_net-2.1.8/src/pygpt_net/ui/dialog/update.py
--rwxr-xr-x   0        0        0     7005 2024-02-28 03:58:59.313445 pygpt_net-2.1.8/src/pygpt_net/ui/dialogs.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.1.8/src/pygpt_net/ui/layout/__init__.py
--rwxr-xr-x   0        0        0     1535 2023-12-29 00:18:50.793125 pygpt_net-2.1.8/src/pygpt_net/ui/layout/chat/__init__.py
--rwxr-xr-x   0        0        0     5149 2024-01-28 22:32:36.115407 pygpt_net-2.1.8/src/pygpt_net/ui/layout/chat/attachments.py
--rwxr-xr-x   0        0        0     4376 2024-01-27 21:42:30.964980 pygpt_net-2.1.8/src/pygpt_net/ui/layout/chat/attachments_uploaded.py
--rw-r--r--   0        0        0     5118 2024-02-23 01:50:39.606418 pygpt_net-2.1.8/src/pygpt_net/ui/layout/chat/calendar.py
--rwxr-xr-x   0        0        0     9051 2024-02-26 21:30:35.305131 pygpt_net-2.1.8/src/pygpt_net/ui/layout/chat/input.py
--rwxr-xr-x   0        0        0    18656 2024-01-01 00:17:57.553256 pygpt_net-2.1.8/src/pygpt_net/ui/layout/chat/markdown.py
--rwxr-xr-x   0        0        0     9142 2024-02-29 03:07:51.278132 pygpt_net-2.1.8/src/pygpt_net/ui/layout/chat/output.py
--rw-r--r--   0        0        0     5199 2024-02-17 21:22:47.345663 pygpt_net-2.1.8/src/pygpt_net/ui/layout/chat/painter.py
--rwxr-xr-x   0        0        0     1697 2024-01-27 21:42:30.964980 pygpt_net-2.1.8/src/pygpt_net/ui/layout/ctx/__init__.py
--rwxr-xr-x   0        0        0     4902 2024-02-02 19:26:46.619683 pygpt_net-2.1.8/src/pygpt_net/ui/layout/ctx/ctx_list.py
--rwxr-xr-x   0        0        0     1441 2024-01-07 09:35:02.638810 pygpt_net-2.1.8/src/pygpt_net/ui/layout/ctx/search_input.py
--rwxr-xr-x   0        0        0     1068 2023-12-31 01:26:09.880264 pygpt_net-2.1.8/src/pygpt_net/ui/layout/ctx/video.py
--rwxr-xr-x   0        0        0     1405 2024-01-31 15:19:17.742029 pygpt_net-2.1.8/src/pygpt_net/ui/layout/status.py
--rwxr-xr-x   0        0        0     3475 2024-01-27 21:42:30.964980 pygpt_net-2.1.8/src/pygpt_net/ui/layout/toolbox/__init__.py
--rw-r--r--   0        0        0     2378 2024-01-30 17:23:19.901578 pygpt_net-2.1.8/src/pygpt_net/ui/layout/toolbox/agent.py
--rwxr-xr-x   0        0        0     4414 2024-01-27 21:42:30.964980 pygpt_net-2.1.8/src/pygpt_net/ui/layout/toolbox/assistants.py
--rwxr-xr-x   0        0        0     4254 2024-02-29 03:07:51.278132 pygpt_net-2.1.8/src/pygpt_net/ui/layout/toolbox/footer.py
--rwxr-xr-x   0        0        0     2382 2024-01-21 16:42:14.672394 pygpt_net-2.1.8/src/pygpt_net/ui/layout/toolbox/image.py
--rw-r--r--   0        0        0     5075 2024-01-27 21:42:30.964980 pygpt_net-2.1.8/src/pygpt_net/ui/layout/toolbox/indexes.py
--rwxr-xr-x   0        0        0     3169 2024-02-21 03:55:24.484309 pygpt_net-2.1.8/src/pygpt_net/ui/layout/toolbox/mode.py
--rwxr-xr-x   0        0        0     3067 2024-02-21 03:55:24.484309 pygpt_net-2.1.8/src/pygpt_net/ui/layout/toolbox/model.py
--rwxr-xr-x   0        0        0     4127 2024-02-01 00:24:56.153509 pygpt_net-2.1.8/src/pygpt_net/ui/layout/toolbox/presets.py
--rwxr-xr-x   0        0        0     3502 2024-02-01 13:33:50.646121 pygpt_net-2.1.8/src/pygpt_net/ui/layout/toolbox/prompt.py
--rwxr-xr-x   0        0        0     2447 2023-12-31 01:26:09.000000 pygpt_net-2.1.8/src/pygpt_net/ui/layout/toolbox/vision.py
--rw-r--r--   0        0        0     7682 2024-02-24 01:55:58.449111 pygpt_net-2.1.8/src/pygpt_net/ui/main.py
--rw-r--r--   0        0        0     1618 2024-02-29 03:07:51.278132 pygpt_net-2.1.8/src/pygpt_net/ui/menu/__init__.py
--rw-r--r--   0        0        0     4667 2024-02-16 20:38:22.746568 pygpt_net-2.1.8/src/pygpt_net/ui/menu/about.py
--rw-r--r--   0        0        0     1654 2024-02-28 03:58:59.313445 pygpt_net-2.1.8/src/pygpt_net/ui/menu/audio.py
--rw-r--r--   0        0        0     5142 2024-02-16 20:38:22.746568 pygpt_net-2.1.8/src/pygpt_net/ui/menu/config.py
--rw-r--r--   0        0        0     4875 2024-02-25 18:06:16.209368 pygpt_net-2.1.8/src/pygpt_net/ui/menu/debug.py
--rw-r--r--   0        0        0     2014 2024-02-16 20:38:22.746568 pygpt_net-2.1.8/src/pygpt_net/ui/menu/file.py
--rw-r--r--   0        0        0      897 2024-01-27 21:42:30.964980 pygpt_net-2.1.8/src/pygpt_net/ui/menu/lang.py
--rw-r--r--   0        0        0     1549 2024-02-16 20:38:22.746568 pygpt_net-2.1.8/src/pygpt_net/ui/menu/plugins.py
--rw-r--r--   0        0        0     2685 2024-02-16 20:38:22.746568 pygpt_net-2.1.8/src/pygpt_net/ui/menu/theme.py
--rw-r--r--   0        0        0     2026 2024-02-29 03:07:51.278132 pygpt_net-2.1.8/src/pygpt_net/ui/menu/video.py
--rw-r--r--   0        0        0     6672 2024-02-01 23:02:10.688691 pygpt_net-2.1.8/src/pygpt_net/ui/tray.py
--rwxr-xr-x   0        0        0      488 2023-12-28 18:11:19.000000 pygpt_net-2.1.8/src/pygpt_net/ui/widget/__init__.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.1.8/src/pygpt_net/ui/widget/audio/__init__.py
--rwxr-xr-x   0        0        0     1721 2023-12-28 21:20:40.362230 pygpt_net-2.1.8/src/pygpt_net/ui/widget/audio/input.py
--rw-r--r--   0        0        0     2198 2024-02-29 03:07:51.278132 pygpt_net-2.1.8/src/pygpt_net/ui/widget/audio/input_button.py
--rwxr-xr-x   0        0        0     1586 2023-12-28 21:20:40.362230 pygpt_net-2.1.8/src/pygpt_net/ui/widget/audio/output.py
--rw-r--r--   0        0        0        0 2024-01-06 03:25:04.270157 pygpt_net-2.1.8/src/pygpt_net/ui/widget/calendar/__init__.py
--rw-r--r--   0        0        0     8116 2024-02-17 21:22:47.345663 pygpt_net-2.1.8/src/pygpt_net/ui/widget/calendar/select.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/__init__.py
--rwxr-xr-x   0        0        0     1308 2024-02-16 17:50:31.993013 pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/alert.py
--rw-r--r--   0        0        0     1502 2024-02-17 21:22:47.345663 pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/applog.py
--rw-r--r--   0        0        0     3163 2024-02-28 03:58:59.313445 pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/base.py
--rwxr-xr-x   0        0        0     1977 2024-01-24 15:53:01.386042 pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/confirm.py
--rw-r--r--   0        0        0     2191 2024-01-28 19:32:28.495073 pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/create.py
--rwxr-xr-x   0        0        0     1572 2024-02-21 16:35:35.211671 pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/debug.py
--rwxr-xr-x   0        0        0     1749 2024-02-17 21:22:47.345663 pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/editor.py
--rwxr-xr-x   0        0        0     1638 2024-02-17 21:22:47.345663 pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/editor_file.py
--rwxr-xr-x   0        0        0      816 2024-02-17 21:22:47.345663 pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/image.py
--rwxr-xr-x   0        0        0     1568 2024-02-17 21:22:47.345663 pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/info.py
--rw-r--r--   0        0        0     1717 2024-02-17 21:22:47.345663 pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/license.py
--rwxr-xr-x   0        0        0     1627 2024-02-17 21:22:47.345663 pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/logger.py
--rw-r--r--   0        0        0     1625 2024-02-17 21:22:47.345663 pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/model.py
--rwxr-xr-x   0        0        0     2191 2024-01-28 19:32:28.495073 pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/rename.py
--rwxr-xr-x   0        0        0     1614 2024-02-17 21:22:47.345663 pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/settings.py
--rwxr-xr-x   0        0        0     1696 2024-02-17 21:22:47.345663 pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/settings_plugin.py
--rw-r--r--   0        0        0     2724 2024-02-26 22:26:37.124323 pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/snap.py
--rwxr-xr-x   0        0        0     6789 2024-02-17 21:22:47.345663 pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/update.py
--rwxr-xr-x   0        0        0      488 2024-01-11 15:56:53.277343 pygpt_net-2.1.8/src/pygpt_net/ui/widget/draw/__init__.py
--rw-r--r--   0        0        0     9057 2024-03-01 17:40:19.825274 pygpt_net-2.1.8/src/pygpt_net/ui/widget/draw/painter.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.1.8/src/pygpt_net/ui/widget/element/__init__.py
--rw-r--r--   0        0        0      947 2024-01-13 00:42:12.107250 pygpt_net-2.1.8/src/pygpt_net/ui/widget/element/button.py
--rwxr-xr-x   0        0        0     2559 2024-01-27 21:42:30.964980 pygpt_net-2.1.8/src/pygpt_net/ui/widget/element/group.py
--rw-r--r--   0        0        0     3789 2024-02-28 03:58:59.313445 pygpt_net-2.1.8/src/pygpt_net/ui/widget/element/labels.py
--rwxr-xr-x   0        0        0        0 2023-12-28 21:20:40.362230 pygpt_net-2.1.8/src/pygpt_net/ui/widget/filesystem/__init__.py
--rwxr-xr-x   0        0        0    21480 2024-03-02 19:51:00.168984 pygpt_net-2.1.8/src/pygpt_net/ui/widget/filesystem/explorer.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.1.8/src/pygpt_net/ui/widget/image/__init__.py
--rwxr-xr-x   0        0        0     2823 2024-01-29 13:41:53.379769 pygpt_net-2.1.8/src/pygpt_net/ui/widget/image/display.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.1.8/src/pygpt_net/ui/widget/lists/__init__.py
--rwxr-xr-x   0        0        0     2682 2024-01-29 13:41:53.379769 pygpt_net-2.1.8/src/pygpt_net/ui/widget/lists/assistant.py
--rwxr-xr-x   0        0        0     4750 2024-01-29 13:41:53.379769 pygpt_net-2.1.8/src/pygpt_net/ui/widget/lists/attachment.py
--rwxr-xr-x   0        0        0     2446 2023-12-28 21:20:40.362230 pygpt_net-2.1.8/src/pygpt_net/ui/widget/lists/base.py
--rwxr-xr-x   0        0        0    11603 2024-02-25 00:27:02.862945 pygpt_net-2.1.8/src/pygpt_net/ui/widget/lists/context.py
--rw-r--r--   0        0        0     3653 2024-02-25 22:01:41.690831 pygpt_net-2.1.8/src/pygpt_net/ui/widget/lists/debug.py
--rw-r--r--   0        0        0     4821 2024-01-31 21:39:19.388967 pygpt_net-2.1.8/src/pygpt_net/ui/widget/lists/index.py
--rwxr-xr-x   0        0        0     1080 2023-12-28 21:20:40.362230 pygpt_net-2.1.8/src/pygpt_net/ui/widget/lists/mode.py
--rwxr-xr-x   0        0        0     1912 2024-01-29 13:41:53.379769 pygpt_net-2.1.8/src/pygpt_net/ui/widget/lists/model.py
--rw-r--r--   0        0        0     1919 2024-01-29 13:41:53.379769 pygpt_net-2.1.8/src/pygpt_net/ui/widget/lists/model_editor.py
--rwxr-xr-x   0        0        0     1028 2024-01-12 09:25:47.589375 pygpt_net-2.1.8/src/pygpt_net/ui/widget/lists/plugin.py
--rwxr-xr-x   0        0        0     4071 2024-02-01 01:48:09.378583 pygpt_net-2.1.8/src/pygpt_net/ui/widget/lists/preset.py
--rw-r--r--   0        0        0     1052 2024-01-12 09:25:47.589375 pygpt_net-2.1.8/src/pygpt_net/ui/widget/lists/settings.py
--rwxr-xr-x   0        0        0     4002 2024-01-29 13:41:53.379769 pygpt_net-2.1.8/src/pygpt_net/ui/widget/lists/uploaded.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.1.8/src/pygpt_net/ui/widget/option/__init__.py
--rwxr-xr-x   0        0        0     2068 2024-01-19 21:21:41.774598 pygpt_net-2.1.8/src/pygpt_net/ui/widget/option/checkbox.py
--rw-r--r--   0        0        0     2797 2024-03-03 03:52:54.350656 pygpt_net-2.1.8/src/pygpt_net/ui/widget/option/combo.py
--rwxr-xr-x   0        0        0    12690 2024-01-30 01:28:33.748573 pygpt_net-2.1.8/src/pygpt_net/ui/widget/option/dictionary.py
--rwxr-xr-x   0        0        0     5968 2024-02-16 20:38:22.746568 pygpt_net-2.1.8/src/pygpt_net/ui/widget/option/input.py
--rwxr-xr-x   0        0        0     3569 2024-01-08 20:36:28.058493 pygpt_net-2.1.8/src/pygpt_net/ui/widget/option/slider.py
--rwxr-xr-x   0        0        0     2077 2024-02-18 20:56:31.563530 pygpt_net-2.1.8/src/pygpt_net/ui/widget/option/textarea.py
--rw-r--r--   0        0        0     1668 2024-01-29 13:41:53.379769 pygpt_net-2.1.8/src/pygpt_net/ui/widget/tabs/Input.py
--rw-r--r--   0        0        0      488 2023-12-30 09:04:29.205425 pygpt_net-2.1.8/src/pygpt_net/ui/widget/tabs/__init__.py
--rw-r--r--   0        0        0     2781 2024-02-16 20:38:22.746568 pygpt_net-2.1.8/src/pygpt_net/ui/widget/tabs/output.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.366230 pygpt_net-2.1.8/src/pygpt_net/ui/widget/textarea/__init__.py
--rw-r--r--   0        0        0     4216 2024-01-30 17:23:19.901578 pygpt_net-2.1.8/src/pygpt_net/ui/widget/textarea/calendar_note.py
--rw-r--r--   0        0        0     1358 2024-01-28 19:32:28.495073 pygpt_net-2.1.8/src/pygpt_net/ui/widget/textarea/create.py
--rwxr-xr-x   0        0        0     4894 2024-02-25 00:27:02.862945 pygpt_net-2.1.8/src/pygpt_net/ui/widget/textarea/input.py
--rwxr-xr-x   0        0        0     1132 2024-01-27 21:42:30.964980 pygpt_net-2.1.8/src/pygpt_net/ui/widget/textarea/name.py
--rwxr-xr-x   0        0        0     5736 2024-02-25 00:27:02.862945 pygpt_net-2.1.8/src/pygpt_net/ui/widget/textarea/notepad.py
--rwxr-xr-x   0        0        0     5241 2024-02-25 00:27:02.862945 pygpt_net-2.1.8/src/pygpt_net/ui/widget/textarea/output.py
--rwxr-xr-x   0        0        0     1358 2024-01-28 19:32:28.495073 pygpt_net-2.1.8/src/pygpt_net/ui/widget/textarea/rename.py
--rwxr-xr-x   0        0        0     1659 2024-02-03 15:51:10.611289 pygpt_net-2.1.8/src/pygpt_net/ui/widget/textarea/search_input.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.366230 pygpt_net-2.1.8/src/pygpt_net/ui/widget/vision/__init__.py
--rwxr-xr-x   0        0        0     2584 2023-12-28 21:20:40.366230 pygpt_net-2.1.8/src/pygpt_net/ui/widget/vision/camera.py
--rwxr-xr-x   0        0        0     3581 2024-02-28 03:58:59.313445 pygpt_net-2.1.8/src/pygpt_net/utils.py
--rw-r--r--   0        0        0   127542 1970-01-01 00:00:00.000000 pygpt_net-2.1.8/PKG-INFO
+-rwxr-xr-x   0        0        0    43210 2024-03-04 20:11:18.535086 pygpt_net-2.1.9/CHANGELOG.md
+-rwxr-xr-x   0        0        0     1077 2024-02-01 17:53:56.362106 pygpt_net-2.1.9/LICENSE
+-rwxr-xr-x   0        0        0   124933 2024-03-04 20:11:13.503159 pygpt_net-2.1.9/README.md
+-rwxr-xr-x   0        0        0    13970 2024-02-19 21:38:20.920806 pygpt_net-2.1.9/icon.png
+-rw-r--r--   0        0        0     2798 2024-03-04 19:32:05.116881 pygpt_net-2.1.9/pyproject.toml
+-rwxr-xr-x   0        0        0    42246 2024-03-04 20:11:25.894979 pygpt_net-2.1.9/src/pygpt_net/CHANGELOG.txt
+-rwxr-xr-x   0        0        0     1146 2024-02-01 17:53:56.366106 pygpt_net-2.1.9/src/pygpt_net/LICENSE
+-rwxr-xr-x   0        0        0      983 2024-03-04 19:33:21.748663 pygpt_net-2.1.9/src/pygpt_net/__init__.py
+-rwxr-xr-x   0        0        0    13698 2024-03-03 03:52:54.350656 pygpt_net-2.1.9/src/pygpt_net/app.py
+-rwxr-xr-x   0        0        0    11573 2024-03-04 20:31:17.344277 pygpt_net-2.1.9/src/pygpt_net/config.py
+-rwxr-xr-x   0        0        0     3350 2024-02-24 01:55:58.445111 pygpt_net-2.1.9/src/pygpt_net/container.py
+-rwxr-xr-x   0        0        0     4314 2024-02-15 05:07:04.118540 pygpt_net-2.1.9/src/pygpt_net/controller/__init__.py
+-rw-r--r--   0        0        0     4662 2024-02-25 05:32:34.229344 pygpt_net-2.1.9/src/pygpt_net/controller/agent/__init__.py
+-rw-r--r--   0        0        0     6569 2024-02-16 04:01:43.038864 pygpt_net-2.1.9/src/pygpt_net/controller/agent/flow.py
+-rw-r--r--   0        0        0    10190 2024-02-21 19:09:37.240983 pygpt_net-2.1.9/src/pygpt_net/controller/assistant/__init__.py
+-rw-r--r--   0        0        0     9873 2024-02-18 06:49:52.490113 pygpt_net-2.1.9/src/pygpt_net/controller/assistant/editor.py
+-rw-r--r--   0        0        0    14478 2024-02-22 03:36:30.096422 pygpt_net-2.1.9/src/pygpt_net/controller/assistant/files.py
+-rw-r--r--   0        0        0    12751 2024-02-22 03:36:30.096422 pygpt_net-2.1.9/src/pygpt_net/controller/assistant/threads.py
+-rwxr-xr-x   0        0        0    14495 2024-02-22 03:36:30.096422 pygpt_net-2.1.9/src/pygpt_net/controller/attachment.py
+-rwxr-xr-x   0        0        0     5234 2024-02-28 03:58:59.305445 pygpt_net-2.1.9/src/pygpt_net/controller/audio.py
+-rw-r--r--   0        0        0     4498 2024-03-01 03:17:53.453929 pygpt_net-2.1.9/src/pygpt_net/controller/calendar/__init__.py
+-rw-r--r--   0        0        0     7349 2024-03-01 03:17:53.453929 pygpt_net-2.1.9/src/pygpt_net/controller/calendar/note.py
+-rwxr-xr-x   0        0        0    12787 2024-02-29 03:07:51.274132 pygpt_net-2.1.9/src/pygpt_net/controller/camera.py
+-rw-r--r--   0        0        0     1436 2024-01-13 16:28:42.715718 pygpt_net-2.1.9/src/pygpt_net/controller/chat/__init__.py
+-rwxr-xr-x   0        0        0     9758 2024-02-16 04:01:43.038864 pygpt_net-2.1.9/src/pygpt_net/controller/chat/common.py
+-rw-r--r--   0        0        0     2149 2024-01-30 20:56:32.772879 pygpt_net-2.1.9/src/pygpt_net/controller/chat/files.py
+-rwxr-xr-x   0        0        0     8583 2024-01-31 15:19:17.738030 pygpt_net-2.1.9/src/pygpt_net/controller/chat/image.py
+-rwxr-xr-x   0        0        0     8575 2024-02-25 05:32:34.229344 pygpt_net-2.1.9/src/pygpt_net/controller/chat/input.py
+-rwxr-xr-x   0        0        0    10083 2024-02-16 04:01:43.038864 pygpt_net-2.1.9/src/pygpt_net/controller/chat/output.py
+-rwxr-xr-x   0        0        0     3647 2024-02-17 21:22:47.341663 pygpt_net-2.1.9/src/pygpt_net/controller/chat/render.py
+-rw-r--r--   0        0        0    10821 2024-03-04 20:15:23.083974 pygpt_net-2.1.9/src/pygpt_net/controller/chat/text.py
+-rw-r--r--   0        0        0     3054 2024-01-30 20:56:32.772879 pygpt_net-2.1.9/src/pygpt_net/controller/chat/vision.py
+-rw-r--r--   0        0        0     4408 2024-01-31 21:39:19.384967 pygpt_net-2.1.9/src/pygpt_net/controller/command.py
+-rw-r--r--   0        0        0     3885 2024-01-10 11:56:03.088017 pygpt_net-2.1.9/src/pygpt_net/controller/config/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-08 20:36:28.054492 pygpt_net-2.1.9/src/pygpt_net/controller/config/field/__init__.py
+-rwxr-xr-x   0        0        0     2422 2024-01-30 20:56:32.772879 pygpt_net-2.1.9/src/pygpt_net/controller/config/field/checkbox.py
+-rw-r--r--   0        0        0     2335 2024-01-30 20:56:32.772879 pygpt_net-2.1.9/src/pygpt_net/controller/config/field/combo.py
+-rw-r--r--   0        0        0     6531 2024-02-25 00:27:02.858945 pygpt_net-2.1.9/src/pygpt_net/controller/config/field/dictionary.py
+-rw-r--r--   0        0        0     3312 2024-01-30 20:56:32.772879 pygpt_net-2.1.9/src/pygpt_net/controller/config/field/input.py
+-rw-r--r--   0        0        0     4582 2024-01-30 20:56:32.772879 pygpt_net-2.1.9/src/pygpt_net/controller/config/field/slider.py
+-rw-r--r--   0        0        0     2281 2024-01-30 20:56:32.772879 pygpt_net-2.1.9/src/pygpt_net/controller/config/field/textarea.py
+-rw-r--r--   0        0        0     5219 2024-03-01 17:40:19.825274 pygpt_net-2.1.9/src/pygpt_net/controller/config/placeholder.py
+-rw-r--r--   0        0        0    15990 2024-02-27 05:21:39.767084 pygpt_net-2.1.9/src/pygpt_net/controller/ctx/__init__.py
+-rw-r--r--   0        0        0     5692 2024-02-23 01:50:39.602419 pygpt_net-2.1.9/src/pygpt_net/controller/ctx/common.py
+-rw-r--r--   0        0        0     2552 2024-01-25 22:43:11.543975 pygpt_net-2.1.9/src/pygpt_net/controller/ctx/summarizer.py
+-rwxr-xr-x   0        0        0     6527 2024-02-28 03:58:59.305445 pygpt_net-2.1.9/src/pygpt_net/controller/debug.py
+-rw-r--r--   0        0        0     1008 2023-12-31 03:09:04.107766 pygpt_net-2.1.9/src/pygpt_net/controller/dialogs/__init__.py
+-rwxr-xr-x   0        0        0     6768 2024-02-23 02:31:25.633179 pygpt_net-2.1.9/src/pygpt_net/controller/dialogs/confirm.py
+-rw-r--r--   0        0        0     5570 2024-02-25 22:01:41.690831 pygpt_net-2.1.9/src/pygpt_net/controller/dialogs/debug.py
+-rwxr-xr-x   0        0        0     2471 2024-02-01 17:53:56.366106 pygpt_net-2.1.9/src/pygpt_net/controller/dialogs/info.py
+-rwxr-xr-x   0        0        0    15200 2024-02-16 15:47:42.083541 pygpt_net-2.1.9/src/pygpt_net/controller/files.py
+-rw-r--r--   0        0        0     5926 2024-02-23 01:50:39.602419 pygpt_net-2.1.9/src/pygpt_net/controller/idx/__init__.py
+-rw-r--r--   0        0        0     2605 2024-02-29 03:07:51.274132 pygpt_net-2.1.9/src/pygpt_net/controller/idx/common.py
+-rw-r--r--   0        0        0    17677 2024-02-29 03:07:51.274132 pygpt_net-2.1.9/src/pygpt_net/controller/idx/indexer.py
+-rw-r--r--   0        0        0     7789 2024-03-03 03:52:54.350656 pygpt_net-2.1.9/src/pygpt_net/controller/idx/settings.py
+-rw-r--r--   0        0        0     2971 2024-01-30 20:56:32.772879 pygpt_net-2.1.9/src/pygpt_net/controller/lang/__init__.py
+-rw-r--r--   0        0        0     4016 2024-02-16 20:38:22.742568 pygpt_net-2.1.9/src/pygpt_net/controller/lang/custom.py
+-rw-r--r--   0        0        0    13219 2024-02-29 03:07:51.274132 pygpt_net-2.1.9/src/pygpt_net/controller/lang/mapping.py
+-rw-r--r--   0        0        0     3879 2024-01-15 13:47:55.919633 pygpt_net-2.1.9/src/pygpt_net/controller/lang/plugins.py
+-rw-r--r--   0        0        0     2634 2024-01-22 12:10:21.917245 pygpt_net-2.1.9/src/pygpt_net/controller/lang/settings.py
+-rwxr-xr-x   0        0        0     1566 2024-01-04 07:51:17.999390 pygpt_net-2.1.9/src/pygpt_net/controller/launcher.py
+-rwxr-xr-x   0        0        0     8825 2024-02-24 01:55:58.445111 pygpt_net-2.1.9/src/pygpt_net/controller/layout.py
+-rw-r--r--   0        0        0     6387 2024-02-18 20:56:31.559530 pygpt_net-2.1.9/src/pygpt_net/controller/mode.py
+-rw-r--r--   0        0        0     4656 2024-01-30 20:56:32.772879 pygpt_net-2.1.9/src/pygpt_net/controller/model/__init__.py
+-rw-r--r--   0        0        0    12599 2024-02-22 03:36:30.096422 pygpt_net-2.1.9/src/pygpt_net/controller/model/editor.py
+-rwxr-xr-x   0        0        0     9567 2024-03-01 03:17:53.457929 pygpt_net-2.1.9/src/pygpt_net/controller/notepad.py
+-rw-r--r--   0        0        0     2081 2024-02-15 05:07:04.118540 pygpt_net-2.1.9/src/pygpt_net/controller/painter/__init__.py
+-rw-r--r--   0        0        0     4461 2024-01-23 23:46:30.495197 pygpt_net-2.1.9/src/pygpt_net/controller/painter/capture.py
+-rw-r--r--   0        0        0     6292 2024-02-17 21:22:47.341663 pygpt_net-2.1.9/src/pygpt_net/controller/painter/common.py
+-rw-r--r--   0        0        0    12925 2024-02-28 03:58:59.305445 pygpt_net-2.1.9/src/pygpt_net/controller/plugins/__init__.py
+-rw-r--r--   0        0        0     5907 2024-02-03 15:51:10.611289 pygpt_net-2.1.9/src/pygpt_net/controller/plugins/settings.py
+-rwxr-xr-x   0        0        0    14286 2024-02-18 20:56:31.559530 pygpt_net-2.1.9/src/pygpt_net/controller/presets/__init__.py
+-rwxr-xr-x   0        0        0    14915 2024-02-18 20:56:31.559530 pygpt_net-2.1.9/src/pygpt_net/controller/presets/editor.py
+-rw-r--r--   0        0        0     6564 2024-02-17 21:22:47.341663 pygpt_net-2.1.9/src/pygpt_net/controller/settings/__init__.py
+-rw-r--r--   0        0        0    12750 2024-03-03 03:52:54.350656 pygpt_net-2.1.9/src/pygpt_net/controller/settings/editor.py
+-rw-r--r--   0        0        0     5133 2024-01-23 23:46:30.499197 pygpt_net-2.1.9/src/pygpt_net/controller/theme/__init__.py
+-rwxr-xr-x   0        0        0     5329 2024-01-27 21:42:30.960980 pygpt_net-2.1.9/src/pygpt_net/controller/theme/common.py
+-rw-r--r--   0        0        0     4939 2024-01-23 20:16:03.144694 pygpt_net-2.1.9/src/pygpt_net/controller/theme/markdown.py
+-rw-r--r--   0        0        0     3178 2024-01-23 23:46:30.499197 pygpt_net-2.1.9/src/pygpt_net/controller/theme/menu.py
+-rw-r--r--   0        0        0     3357 2024-01-27 21:42:30.960980 pygpt_net-2.1.9/src/pygpt_net/controller/theme/nodes.py
+-rw-r--r--   0        0        0     4585 2024-01-31 11:15:00.681079 pygpt_net-2.1.9/src/pygpt_net/controller/ui/__init__.py
+-rw-r--r--   0        0        0     4936 2024-02-29 03:07:51.274132 pygpt_net-2.1.9/src/pygpt_net/controller/ui/mode.py
+-rw-r--r--   0        0        0     1902 2024-01-23 23:46:30.499197 pygpt_net-2.1.9/src/pygpt_net/controller/ui/vision.py
+-rw-r--r--   0        0        0        0 2024-01-26 16:05:36.561120 pygpt_net-2.1.9/src/pygpt_net/core/__init__.py
+-rw-r--r--   0        0        0     7728 2024-02-21 19:09:37.240983 pygpt_net-2.1.9/src/pygpt_net/core/assistants/__init__.py
+-rwxr-xr-x   0        0        0    10240 2024-01-31 15:19:17.738030 pygpt_net-2.1.9/src/pygpt_net/core/attachments.py
+-rw-r--r--   0        0        0     2708 2024-02-24 01:55:58.445111 pygpt_net-2.1.9/src/pygpt_net/core/audio.py
+-rw-r--r--   0        0        0     3354 2024-01-31 15:19:17.742029 pygpt_net-2.1.9/src/pygpt_net/core/bridge.py
+-rw-r--r--   0        0        0     6646 2024-02-02 19:26:46.615683 pygpt_net-2.1.9/src/pygpt_net/core/calendar/__init__.py
+-rwxr-xr-x   0        0        0     4034 2024-02-21 16:18:39.952987 pygpt_net-2.1.9/src/pygpt_net/core/camera.py
+-rw-r--r--   0        0        0     3130 2024-01-27 01:08:27.560991 pygpt_net-2.1.9/src/pygpt_net/core/chain/__init__.py
+-rw-r--r--   0        0        0     4656 2024-01-27 01:08:27.560991 pygpt_net-2.1.9/src/pygpt_net/core/chain/chat.py
+-rw-r--r--   0        0        0     5089 2024-01-27 01:08:27.560991 pygpt_net-2.1.9/src/pygpt_net/core/chain/completion.py
+-rwxr-xr-x   0        0        0     9759 2024-02-16 04:01:43.038864 pygpt_net-2.1.9/src/pygpt_net/core/command.py
+-rw-r--r--   0        0        0    22242 2024-02-27 05:21:39.767084 pygpt_net-2.1.9/src/pygpt_net/core/ctx/__init__.py
+-rw-r--r--   0        0        0     7709 2024-02-27 05:21:39.767084 pygpt_net-2.1.9/src/pygpt_net/core/ctx/idx.py
+-rw-r--r--   0        0        0     6519 2024-01-23 23:46:30.499197 pygpt_net-2.1.9/src/pygpt_net/core/db/__init__.py
+-rwxr-xr-x   0        0        0     7586 2024-02-22 03:36:30.096422 pygpt_net-2.1.9/src/pygpt_net/core/debug/__init__.py
+-rw-r--r--   0        0        0     1467 2024-02-25 18:06:16.205368 pygpt_net-2.1.9/src/pygpt_net/core/debug/agent.py
+-rwxr-xr-x   0        0        0     2259 2024-02-25 22:01:41.690831 pygpt_net-2.1.9/src/pygpt_net/core/debug/assistants.py
+-rwxr-xr-x   0        0        0     1626 2024-02-25 22:01:41.690831 pygpt_net-2.1.9/src/pygpt_net/core/debug/attachments.py
+-rwxr-xr-x   0        0        0     1458 2024-02-25 22:01:41.690831 pygpt_net-2.1.9/src/pygpt_net/core/debug/config.py
+-rwxr-xr-x   0        0        0     2958 2024-03-04 19:53:48.502024 pygpt_net-2.1.9/src/pygpt_net/core/debug/context.py
+-rw-r--r--   0        0        0     3377 2024-02-27 05:21:39.767084 pygpt_net-2.1.9/src/pygpt_net/core/debug/indexes.py
+-rwxr-xr-x   0        0        0     1848 2024-02-25 22:01:41.690831 pygpt_net-2.1.9/src/pygpt_net/core/debug/models.py
+-rwxr-xr-x   0        0        0     1258 2024-02-25 22:01:41.690831 pygpt_net-2.1.9/src/pygpt_net/core/debug/plugins.py
+-rwxr-xr-x   0        0        0     1994 2024-02-25 22:01:41.690831 pygpt_net-2.1.9/src/pygpt_net/core/debug/presets.py
+-rwxr-xr-x   0        0        0     2666 2024-02-25 22:01:41.690831 pygpt_net-2.1.9/src/pygpt_net/core/debug/ui.py
+-rwxr-xr-x   0        0        0     7695 2024-03-04 21:11:59.595845 pygpt_net-2.1.9/src/pygpt_net/core/dispatcher.py
+-rw-r--r--   0        0        0     7678 2024-02-21 19:09:37.240983 pygpt_net-2.1.9/src/pygpt_net/core/filesystem.py
+-rwxr-xr-x   0        0        0     3092 2024-01-23 23:46:30.499197 pygpt_net-2.1.9/src/pygpt_net/core/history.py
+-rwxr-xr-x   0        0        0    14729 2024-03-01 17:40:19.825274 pygpt_net-2.1.9/src/pygpt_net/core/idx/__init__.py
+-rwxr-xr-x   0        0        0    11006 2024-03-04 19:26:42.821732 pygpt_net-2.1.9/src/pygpt_net/core/idx/chat.py
+-rw-r--r--   0        0        0     2226 2024-02-28 03:58:59.309445 pygpt_net-2.1.9/src/pygpt_net/core/idx/context.py
+-rwxr-xr-x   0        0        0    25008 2024-03-04 19:26:20.277786 pygpt_net-2.1.9/src/pygpt_net/core/idx/indexing.py
+-rw-r--r--   0        0        0     2656 2024-02-28 03:58:59.309445 pygpt_net-2.1.9/src/pygpt_net/core/idx/llm.py
+-rw-r--r--   0        0        0        0 2024-02-27 05:21:39.767084 pygpt_net-2.1.9/src/pygpt_net/core/idx/types/__init__.py
+-rw-r--r--   0        0        0     3113 2024-02-27 05:21:39.767084 pygpt_net-2.1.9/src/pygpt_net/core/idx/types/ctx.py
+-rw-r--r--   0        0        0     4722 2024-02-27 05:21:39.767084 pygpt_net-2.1.9/src/pygpt_net/core/idx/types/external.py
+-rw-r--r--   0        0        0     3733 2024-02-27 05:21:39.771084 pygpt_net-2.1.9/src/pygpt_net/core/idx/types/files.py
+-rw-r--r--   0        0        0     2766 2024-02-28 03:58:59.309445 pygpt_net-2.1.9/src/pygpt_net/core/idx/worker.py
+-rwxr-xr-x   0        0        0     4629 2024-02-22 03:36:30.096422 pygpt_net-2.1.9/src/pygpt_net/core/image.py
+-rwxr-xr-x   0        0        0      829 2023-12-31 03:18:56.426282 pygpt_net-2.1.9/src/pygpt_net/core/info.py
+-rw-r--r--   0        0        0     2040 2024-01-11 15:56:53.273343 pygpt_net-2.1.9/src/pygpt_net/core/installer.py
+-rw-r--r--   0        0        0     1168 2024-01-14 15:51:20.622630 pygpt_net-2.1.9/src/pygpt_net/core/llm/__init__.py
+-rwxr-xr-x   0        0        0     4814 2024-01-23 23:46:30.499197 pygpt_net-2.1.9/src/pygpt_net/core/locale.py
+-rw-r--r--   0        0        0     7573 2024-01-27 21:42:30.960980 pygpt_net-2.1.9/src/pygpt_net/core/models.py
+-rw-r--r--   0        0        0     1913 2024-01-23 23:46:30.499197 pygpt_net-2.1.9/src/pygpt_net/core/modes.py
+-rwxr-xr-x   0        0        0     3270 2024-01-27 21:42:30.960980 pygpt_net-2.1.9/src/pygpt_net/core/notepad.py
+-rwxr-xr-x   0        0        0     4214 2024-01-23 23:46:30.499197 pygpt_net-2.1.9/src/pygpt_net/core/platforms.py
+-rwxr-xr-x   0        0        0     8576 2024-02-24 01:55:58.445111 pygpt_net-2.1.9/src/pygpt_net/core/plugins.py
+-rw-r--r--   0        0        0     9286 2024-02-01 18:18:38.554891 pygpt_net-2.1.9/src/pygpt_net/core/presets.py
+-rw-r--r--   0        0        0     2167 2024-02-27 03:03:23.430567 pygpt_net-2.1.9/src/pygpt_net/core/prompt.py
+-rw-r--r--   0        0        0      489 2024-01-05 12:12:41.797675 pygpt_net-2.1.9/src/pygpt_net/core/render/__init__.py
+-rw-r--r--   0        0        0     2454 2024-02-17 21:22:47.341663 pygpt_net-2.1.9/src/pygpt_net/core/render/base.py
+-rw-r--r--   0        0        0      489 2024-01-05 12:12:41.797675 pygpt_net-2.1.9/src/pygpt_net/core/render/markdown/__init__.py
+-rwxr-xr-x   0        0        0     3111 2024-02-22 04:14:57.246812 pygpt_net-2.1.9/src/pygpt_net/core/render/markdown/parser.py
+-rwxr-xr-x   0        0        0    14959 2024-02-21 19:09:37.240983 pygpt_net-2.1.9/src/pygpt_net/core/render/markdown/renderer.py
+-rw-r--r--   0        0        0      489 2024-01-05 13:07:04.262555 pygpt_net-2.1.9/src/pygpt_net/core/render/plain/__init__.py
+-rw-r--r--   0        0        0    12471 2024-02-17 21:22:47.341663 pygpt_net-2.1.9/src/pygpt_net/core/render/plain/renderer.py
+-rwxr-xr-x   0        0        0     6333 2024-02-17 21:22:47.341663 pygpt_net-2.1.9/src/pygpt_net/core/settings.py
+-rwxr-xr-x   0        0        0    14040 2024-02-25 18:06:16.205368 pygpt_net-2.1.9/src/pygpt_net/core/tokens.py
+-rw-r--r--   0        0        0    13722 2024-02-21 19:09:37.240983 pygpt_net-2.1.9/src/pygpt_net/core/updater/__init__.py
+-rw-r--r--   0        0        0     2343 2024-02-24 01:55:58.445111 pygpt_net-2.1.9/src/pygpt_net/core/web.py
+-rw-r--r--   0        0        0      901 2024-01-25 22:43:11.543975 pygpt_net-2.1.9/src/pygpt_net/core/worker.py
+-rwxr-xr-x   0        0        0     7577 2024-03-04 20:18:09.982252 pygpt_net-2.1.9/src/pygpt_net/data/config/config.json
+-rwxr-xr-x   0        0        0    14349 2024-03-04 19:33:01.244722 pygpt_net-2.1.9/src/pygpt_net/data/config/models.json
+-rw-r--r--   0        0        0     1440 2024-03-04 19:32:57.500732 pygpt_net-2.1.9/src/pygpt_net/data/config/modes.json
+-rwxr-xr-x   0        0        0      459 2024-01-13 13:04:53.113674 pygpt_net-2.1.9/src/pygpt_net/data/config/presets/batman_and_joker.json
+-rw-r--r--   0        0        0     2702 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/config/presets/current.agent.json
+-rwxr-xr-x   0        0        0      368 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/config/presets/current.assistant.json
+-rwxr-xr-x   0        0        0      396 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/config/presets/current.chat.json
+-rwxr-xr-x   0        0        0      385 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/config/presets/current.completion.json
+-rwxr-xr-x   0        0        0      368 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/config/presets/current.img.json
+-rwxr-xr-x   0        0        0      382 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/config/presets/current.langchain.json
+-rw-r--r--   0        0        0      368 2024-03-03 02:59:46.037803 pygpt_net-2.1.9/src/pygpt_net/data/config/presets/current.llama_index.json
+-rwxr-xr-x   0        0        0      392 2024-03-03 03:52:54.350656 pygpt_net-2.1.9/src/pygpt_net/data/config/presets/current.vision.json
+-rwxr-xr-x   0        0        0      501 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/config/presets/dalle_white_cat.json
+-rwxr-xr-x   0        0        0    23304 2024-03-04 20:18:14.602208 pygpt_net-2.1.9/src/pygpt_net/data/config/settings.json
+-rw-r--r--   0        0        0      736 2024-02-01 17:53:56.366106 pygpt_net-2.1.9/src/pygpt_net/data/config/settings_section.json
+-rw-r--r--   0        0        0      664 2024-01-20 12:18:41.475899 pygpt_net-2.1.9/src/pygpt_net/data/css/fix_windows.css
+-rw-r--r--   0        0        0      489 2024-01-04 08:28:16.417936 pygpt_net-2.1.9/src/pygpt_net/data/css/markdown.css
+-rw-r--r--   0        0        0      516 2024-01-23 23:46:30.499197 pygpt_net-2.1.9/src/pygpt_net/data/css/markdown.dark.css
+-rw-r--r--   0        0        0      461 2024-01-23 23:46:30.499197 pygpt_net-2.1.9/src/pygpt_net/data/css/markdown.light.css
+-rw-r--r--   0        0        0      400 2024-01-12 03:59:56.290336 pygpt_net-2.1.9/src/pygpt_net/data/css/style.css
+-rw-r--r--   0        0        0      559 2024-01-27 21:42:30.960980 pygpt_net-2.1.9/src/pygpt_net/data/css/style.dark.css
+-rw-r--r--   0        0        0     1157 2024-01-27 21:42:30.960980 pygpt_net-2.1.9/src/pygpt_net/data/css/style.light.css
+-rwxr-xr-x   0        0        0    69484 2023-12-08 15:03:16.000000 pygpt_net-2.1.9/src/pygpt_net/data/fonts/Lato/Lato-Black.ttf
+-rwxr-xr-x   0        0        0    71948 2023-12-08 15:03:16.000000 pygpt_net-2.1.9/src/pygpt_net/data/fonts/Lato/Lato-BlackItalic.ttf
+-rwxr-xr-x   0        0        0    73316 2023-12-08 15:03:16.000000 pygpt_net-2.1.9/src/pygpt_net/data/fonts/Lato/Lato-Bold.ttf
+-rwxr-xr-x   0        0        0    77680 2023-12-08 15:03:16.000000 pygpt_net-2.1.9/src/pygpt_net/data/fonts/Lato/Lato-BoldItalic.ttf
+-rwxr-xr-x   0        0        0    75744 2023-12-08 15:03:16.000000 pygpt_net-2.1.9/src/pygpt_net/data/fonts/Lato/Lato-Italic.ttf
+-rwxr-xr-x   0        0        0    77192 2023-12-08 15:03:16.000000 pygpt_net-2.1.9/src/pygpt_net/data/fonts/Lato/Lato-Light.ttf
+-rwxr-xr-x   0        0        0    49064 2023-12-08 15:03:16.000000 pygpt_net-2.1.9/src/pygpt_net/data/fonts/Lato/Lato-LightItalic.ttf
+-rwxr-xr-x   0        0        0    75136 2023-12-08 15:03:16.000000 pygpt_net-2.1.9/src/pygpt_net/data/fonts/Lato/Lato-Regular.ttf
+-rwxr-xr-x   0        0        0    69968 2023-12-08 15:03:16.000000 pygpt_net-2.1.9/src/pygpt_net/data/fonts/Lato/Lato-Thin.ttf
+-rwxr-xr-x   0        0        0    48848 2023-12-08 15:03:16.000000 pygpt_net-2.1.9/src/pygpt_net/data/fonts/Lato/Lato-ThinItalic.ttf
+-rwxr-xr-x   0        0        0     4500 2023-12-08 15:03:16.000000 pygpt_net-2.1.9/src/pygpt_net/data/fonts/Lato/OFL.txt
+-rwxr-xr-x   0        0        0     3461 2023-04-14 00:10:28.000000 pygpt_net-2.1.9/src/pygpt_net/data/icon.ico
+-rwxr-xr-x   0        0        0    13970 2023-04-14 00:10:28.000000 pygpt_net-2.1.9/src/pygpt_net/data/icon.png
+-rw-r--r--   0        0        0     5471 2024-01-29 18:11:38.035830 pygpt_net-2.1.9/src/pygpt_net/data/icon_tray_busy.ico
+-rw-r--r--   0        0        0    14837 2024-01-29 18:11:38.035830 pygpt_net-2.1.9/src/pygpt_net/data/icon_tray_error.ico
+-rw-r--r--   0        0        0     4209 2024-01-29 18:11:38.035830 pygpt_net-2.1.9/src/pygpt_net/data/icon_tray_idle.ico
+-rw-r--r--   0        0        0      538 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/abc.svg
+-rw-r--r--   0        0        0      178 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/add.svg
+-rw-r--r--   0        0        0      463 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/add_circle.svg
+-rw-r--r--   0        0        0      348 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/add_folder.svg
+-rw-r--r--   0        0        0      391 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/add_library.svg
+-rw-r--r--   0        0        0      558 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/alarm.svg
+-rw-r--r--   0        0        0     1027 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/apps.svg
+-rw-r--r--   0        0        0      267 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/asterisk.svg
+-rw-r--r--   0        0        0      429 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/attachment.svg
+-rw-r--r--   0        0        0      422 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/attachments.svg
+-rw-r--r--   0        0        0      185 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/back.svg
+-rw-r--r--   0        0        0      395 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/backspace.svg
+-rw-r--r--   0        0        0      472 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/block.svg
+-rw-r--r--   0        0        0      255 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/bookmark.svg
+-rw-r--r--   0        0        0      423 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/brush.svg
+-rw-r--r--   0        0        0      523 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/build.svg
+-rw-r--r--   0        0        0      927 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/calendar.svg
+-rw-r--r--   0        0        0      496 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/camera.svg
+-rw-r--r--   0        0        0      336 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/chat.svg
+-rw-r--r--   0        0        0      174 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/check.svg
+-rw-r--r--   0        0        0      459 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/check_circle.svg
+-rw-r--r--   0        0        0      265 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/checklist.svg
+-rw-r--r--   0        0        0      406 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/circle.svg
+-rw-r--r--   0        0        0      191 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/clear.svg
+-rw-r--r--   0        0        0      411 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/clock.svg
+-rw-r--r--   0        0        0      218 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/close.svg
+-rw-r--r--   0        0        0      503 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/close_circle.svg
+-rw-r--r--   0        0        0      224 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/code.svg
+-rw-r--r--   0        0        0      298 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/computer.svg
+-rw-r--r--   0        0        0      336 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/copy.svg
+-rw-r--r--   0        0        0      264 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/crop.svg
+-rw-r--r--   0        0        0      666 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/cut.svg
+-rw-r--r--   0        0        0      725 2024-01-30 17:23:19.885579 pygpt_net-2.1.9/src/pygpt_net/data/icons/db.svg
+-rw-r--r--   0        0        0      271 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/delete.svg
+-rw-r--r--   0        0        0      174 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/done.svg
+-rw-r--r--   0        0        0      274 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/download.svg
+-rw-r--r--   0        0        0      283 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/draft.svg
+-rw-r--r--   0        0        0      323 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/drag.svg
+-rw-r--r--   0        0        0      325 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/edit.svg
+-rw-r--r--   0        0        0      497 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/emergency.svg
+-rw-r--r--   0        0        0      195 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/equalizer.svg
+-rw-r--r--   0        0        0      533 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/error.svg
+-rw-r--r--   0        0        0      372 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/event_available.svg
+-rw-r--r--   0        0        0      174 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/expand.svg
+-rw-r--r--   0        0        0      247 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/fast_forward.svg
+-rw-r--r--   0        0        0      250 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/fast_rewind.svg
+-rw-r--r--   0        0        0      504 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/favorite.svg
+-rw-r--r--   0        0        0      297 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/folder.svg
+-rw-r--r--   0        0        0      249 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/folder_filled.svg
+-rw-r--r--   0        0        0      186 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/forward.svg
+-rw-r--r--   0        0        0      194 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/full.svg
+-rw-r--r--   0        0        0      249 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/fullscreen.svg
+-rw-r--r--   0        0        0      459 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/grid.svg
+-rw-r--r--   0        0        0      602 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/hearing.svg
+-rw-r--r--   0        0        0      691 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/help.svg
+-rw-r--r--   0        0        0      440 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/history.svg
+-rw-r--r--   0        0        0      239 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/home.svg
+-rw-r--r--   0        0        0      176 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/home_filled.svg
+-rw-r--r--   0        0        0      323 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/image.svg
+-rw-r--r--   0        0        0      531 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/info.svg
+-rw-r--r--   0        0        0      337 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/input.svg
+-rw-r--r--   0        0        0      541 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/key.svg
+-rw-r--r--   0        0        0      517 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/keyboard.svg
+-rw-r--r--   0        0        0      972 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/language.svg
+-rw-r--r--   0        0        0      491 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/list.svg
+-rw-r--r--   0        0        0      495 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/lock.svg
+-rw-r--r--   0        0        0      273 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/logout.svg
+-rw-r--r--   0        0        0      392 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/map.svg
+-rw-r--r--   0        0        0      431 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/memory.svg
+-rw-r--r--   0        0        0      189 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/menu.svg
+-rw-r--r--   0        0        0      447 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/mic.svg
+-rw-r--r--   0        0        0      485 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/mic_off.svg
+-rw-r--r--   0        0        0      423 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/more_horizontal.svg
+-rw-r--r--   0        0        0      491 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/mute.svg
+-rw-r--r--   0        0        0      296 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/open_tab.svg
+-rw-r--r--   0        0        0      846 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/palette.svg
+-rw-r--r--   0        0        0      431 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/paste.svg
+-rw-r--r--   0        0        0      250 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/pause.svg
+-rw-r--r--   0        0        0      454 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/pause_circle.svg
+-rw-r--r--   0        0        0      377 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/photos.svg
+-rw-r--r--   0        0        0      441 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/pin.svg
+-rw-r--r--   0        0        0      186 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/play.svg
+-rw-r--r--   0        0        0      197 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/play_pause.svg
+-rw-r--r--   0        0        0      246 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/playlist_add.svg
+-rw-r--r--   0        0        0      318 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/power.svg
+-rw-r--r--   0        0        0      478 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/print.svg
+-rw-r--r--   0        0        0      598 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/public_filled.svg
+-rw-r--r--   0        0        0      283 2024-01-30 20:56:32.772879 pygpt_net-2.1.9/src/pygpt_net/data/icons/redo.svg
+-rw-r--r--   0        0        0      329 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/reload.svg
+-rw-r--r--   0        0        0      260 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/repeat.svg
+-rw-r--r--   0        0        0      400 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/replay.svg
+-rw-r--r--   0        0        0      401 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/resize.svg
+-rw-r--r--   0        0        0      615 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/robot.svg
+-rw-r--r--   0        0        0      807 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/router.svg
+-rw-r--r--   0        0        0      384 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/save.svg
+-rw-r--r--   0        0        0      469 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/schedule.svg
+-rw-r--r--   0        0        0      396 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/screenshot.svg
+-rw-r--r--   0        0        0      372 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/search.svg
+-rw-r--r--   0        0        0      274 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/security.svg
+-rw-r--r--   0        0        0      660 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/sensors.svg
+-rw-r--r--   0        0        0      767 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/settings.svg
+-rw-r--r--   0        0        0      475 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/settings_filled.svg
+-rw-r--r--   0        0        0      792 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/share.svg
+-rw-r--r--   0        0        0      469 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/shedule.svg
+-rw-r--r--   0        0        0      189 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/sort.svg
+-rw-r--r--   0        0        0      386 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/stack.svg
+-rw-r--r--   0        0        0      306 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/stacks.svg
+-rw-r--r--   0        0        0      291 2024-01-30 17:23:19.889579 pygpt_net-2.1.9/src/pygpt_net/data/icons/star.svg
+-rw-r--r--   0        0        0      188 2024-01-30 17:23:19.893578 pygpt_net-2.1.9/src/pygpt_net/data/icons/stop.svg
+-rw-r--r--   0        0        0      432 2024-01-30 17:23:19.893578 pygpt_net-2.1.9/src/pygpt_net/data/icons/stop_circle.svg
+-rw-r--r--   0        0        0      381 2024-01-30 17:23:19.893578 pygpt_net-2.1.9/src/pygpt_net/data/icons/sync.svg
+-rw-r--r--   0        0        0      317 2024-01-30 17:23:19.893578 pygpt_net-2.1.9/src/pygpt_net/data/icons/tag.svg
+-rw-r--r--   0        0        0      334 2024-01-30 17:23:19.893578 pygpt_net-2.1.9/src/pygpt_net/data/icons/task.svg
+-rw-r--r--   0        0        0      336 2024-01-30 17:23:19.893578 pygpt_net-2.1.9/src/pygpt_net/data/icons/terminal.svg
+-rw-r--r--   0        0        0      204 2024-01-30 17:23:19.893578 pygpt_net-2.1.9/src/pygpt_net/data/icons/text.svg
+-rw-r--r--   0        0        0      329 2024-01-30 17:23:19.893578 pygpt_net-2.1.9/src/pygpt_net/data/icons/textfile.svg
+-rw-r--r--   0        0        0      479 2024-01-30 17:23:19.893578 pygpt_net-2.1.9/src/pygpt_net/data/icons/timer.svg
+-rw-r--r--   0        0        0      321 2024-01-30 17:23:19.893578 pygpt_net-2.1.9/src/pygpt_net/data/icons/today.svg
+-rw-r--r--   0        0        0      308 2024-01-30 17:23:19.893578 pygpt_net-2.1.9/src/pygpt_net/data/icons/tune.svg
+-rw-r--r--   0        0        0      282 2024-01-30 17:23:19.893578 pygpt_net-2.1.9/src/pygpt_net/data/icons/undo.svg
+-rw-r--r--   0        0        0      444 2024-01-30 17:23:19.893578 pygpt_net-2.1.9/src/pygpt_net/data/icons/update.svg
+-rw-r--r--   0        0        0      392 2024-01-30 17:23:19.893578 pygpt_net-2.1.9/src/pygpt_net/data/icons/updater.svg
+-rw-r--r--   0        0        0      276 2024-01-30 17:23:19.893578 pygpt_net-2.1.9/src/pygpt_net/data/icons/upload.svg
+-rw-r--r--   0        0        0      339 2024-01-30 17:23:19.893578 pygpt_net-2.1.9/src/pygpt_net/data/icons/video.svg
+-rw-r--r--   0        0        0      550 2024-01-30 17:23:19.893578 pygpt_net-2.1.9/src/pygpt_net/data/icons/view.svg
+-rw-r--r--   0        0        0      736 2024-01-30 17:23:19.893578 pygpt_net-2.1.9/src/pygpt_net/data/icons/voice.svg
+-rw-r--r--   0        0        0      374 2024-01-30 17:23:19.893578 pygpt_net-2.1.9/src/pygpt_net/data/icons/volume.svg
+-rw-r--r--   0        0        0      310 2024-01-30 17:23:19.893578 pygpt_net-2.1.9/src/pygpt_net/data/icons/warning.svg
+-rw-r--r--   0        0        0      300 2024-01-30 17:23:19.893578 pygpt_net-2.1.9/src/pygpt_net/data/icons/webcam.svg
+-rw-r--r--   0        0        0      375 2024-02-29 03:07:51.274132 pygpt_net-2.1.9/src/pygpt_net/data/icons/webcam_off.svg
+-rw-r--r--   0        0        0      325 2024-01-30 17:23:19.893578 pygpt_net-2.1.9/src/pygpt_net/data/icons/width.svg
+-rw-r--r--   0        0        0      336 2024-01-30 17:23:19.893578 pygpt_net-2.1.9/src/pygpt_net/data/icons/window.svg
+-rw-r--r--   0        0        0      365 2024-01-30 17:23:19.893578 pygpt_net-2.1.9/src/pygpt_net/data/icons/work.svg
+-rw-r--r--   0        0        0      422 2024-01-30 17:23:19.893578 pygpt_net-2.1.9/src/pygpt_net/data/icons/zoom_in.svg
+-rw-r--r--   0        0        0      396 2024-01-30 17:23:19.893578 pygpt_net-2.1.9/src/pygpt_net/data/icons/zoom_out.svg
+-rwxr-xr-x   0        0        0    29134 2024-03-01 03:17:53.457929 pygpt_net-2.1.9/src/pygpt_net/data/locale/locale.de.ini
+-rwxr-xr-x   0        0        0    34612 2024-03-02 19:51:00.168984 pygpt_net-2.1.9/src/pygpt_net/data/locale/locale.en.ini
+-rwxr-xr-x   0        0        0    29222 2024-03-01 17:40:19.825274 pygpt_net-2.1.9/src/pygpt_net/data/locale/locale.es.ini
+-rwxr-xr-x   0        0        0    30122 2024-03-01 17:40:19.825274 pygpt_net-2.1.9/src/pygpt_net/data/locale/locale.fr.ini
+-rwxr-xr-x   0        0        0    28666 2024-03-01 17:40:19.825274 pygpt_net-2.1.9/src/pygpt_net/data/locale/locale.it.ini
+-rwxr-xr-x   0        0        0    28477 2024-03-01 17:40:19.825274 pygpt_net-2.1.9/src/pygpt_net/data/locale/locale.pl.ini
+-rwxr-xr-x   0        0        0    40413 2024-03-01 03:17:53.457929 pygpt_net-2.1.9/src/pygpt_net/data/locale/locale.ua.ini
+-rwxr-xr-x   0        0        0     1532 2024-02-25 05:32:34.229344 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.agent.en.ini
+-rwxr-xr-x   0        0        0     1713 2024-02-25 05:32:34.229344 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.agent.pl.ini
+-rwxr-xr-x   0        0        0     8006 2024-03-01 03:17:53.457929 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.audio_input.en.ini
+-rwxr-xr-x   0        0        0     7599 2024-02-28 03:58:59.309445 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.audio_input.pl.ini
+-rwxr-xr-x   0        0        0     2293 2024-02-25 00:27:02.862945 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.audio_output.en.ini
+-rwxr-xr-x   0        0        0     1390 2024-02-24 01:55:58.445111 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.audio_output.pl.ini
+-rw-r--r--   0        0        0      766 2024-02-25 05:32:34.229344 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.cmd_api.en.ini
+-rw-r--r--   0        0        0      850 2024-02-26 21:30:35.305131 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.cmd_api.pl.ini
+-rwxr-xr-x   0        0        0     2353 2024-02-16 20:38:22.746568 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.en.ini
+-rwxr-xr-x   0        0        0     2573 2024-02-16 20:38:22.746568 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.pl.ini
+-rwxr-xr-x   0        0        0      455 2024-02-25 05:32:34.229344 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.cmd_custom.en.ini
+-rwxr-xr-x   0        0        0      527 2024-01-30 20:56:32.776879 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.cmd_custom.pl.ini
+-rwxr-xr-x   0        0        0     7909 2024-03-03 22:43:17.403437 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.cmd_files.en.ini
+-rwxr-xr-x   0        0        0     7492 2024-02-25 05:32:34.229344 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.cmd_files.pl.ini
+-rw-r--r--   0        0        0     3998 2024-02-15 05:07:04.118540 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.cmd_history.en.ini
+-rw-r--r--   0        0        0     4450 2024-02-04 17:46:05.314114 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.cmd_history.pl.ini
+-rw-r--r--   0        0        0     1992 2024-01-30 20:56:32.776879 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.cmd_serial.en.ini
+-rw-r--r--   0        0        0     2186 2024-01-30 20:56:32.776879 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.cmd_serial.pl.ini
+-rwxr-xr-x   0        0        0     6548 2024-03-04 19:44:09.848653 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.cmd_web.en.ini
+-rwxr-xr-x   0        0        0     6485 2024-03-01 17:40:19.825274 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.cmd_web.pl.ini
+-rw-r--r--   0        0        0      888 2024-02-01 23:02:10.688691 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.crontab.en.ini
+-rw-r--r--   0        0        0     1014 2024-02-01 23:02:10.688691 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.crontab.pl.ini
+-rw-r--r--   0        0        0      409 2024-01-30 20:56:32.776879 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.extra_prompt.en.ini
+-rw-r--r--   0        0        0      474 2024-01-30 20:56:32.776879 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.extra_prompt.pl.ini
+-rw-r--r--   0        0        0     2407 2024-03-03 05:47:23.540140 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.idx_llama_index.en.ini
+-rw-r--r--   0        0        0     1090 2024-01-30 20:56:32.776879 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.idx_llama_index.pl.ini
+-rw-r--r--   0        0        0      592 2024-01-30 20:56:32.776879 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.openai_dalle.en.ini
+-rw-r--r--   0        0        0      609 2024-01-30 20:56:32.776879 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.openai_dalle.pl.ini
+-rw-r--r--   0        0        0     1576 2024-02-15 05:07:04.118540 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.openai_vision.en.ini
+-rw-r--r--   0        0        0     1764 2024-01-30 20:56:32.776879 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.openai_vision.pl.ini
+-rwxr-xr-x   0        0        0      631 2024-01-30 20:56:32.776879 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.real_time.en.ini
+-rwxr-xr-x   0        0        0      752 2024-01-30 20:56:32.776879 pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.real_time.pl.ini
+-rwxr-xr-x   0        0        0    19418 2023-12-14 19:08:45.000000 pygpt_net-2.1.9/src/pygpt_net/data/logo.png
+-rwxr-xr-x   0        0        0    31708 2024-02-20 19:10:03.189314 pygpt_net-2.1.9/src/pygpt_net/data/win32/README.rtf
+-rwxr-xr-x   0        0        0     1633 2023-04-14 00:10:28.000000 pygpt_net-2.1.9/src/pygpt_net/data/win32/USER-LICENSE.rtf
+-rwxr-xr-x   0        0        0    87160 2023-04-14 00:10:28.000000 pygpt_net-2.1.9/src/pygpt_net/data/win32/pygpt.aip
+-rwxr-xr-x   0        0        0       45 2023-12-19 15:40:13.000000 pygpt_net-2.1.9/src/pygpt_net/data/win32/qt.conf
+-rw-r--r--   0        0        0    21736 2024-03-02 20:04:01.386329 pygpt_net-2.1.9/src/pygpt_net/icons.qrc
+-rw-r--r--   0        0        0    90430 2024-03-02 20:05:43.048414 pygpt_net-2.1.9/src/pygpt_net/icons_rc.py
+-rw-r--r--   0        0        0      488 2023-12-31 03:12:36.955235 pygpt_net-2.1.9/src/pygpt_net/item/__init__.py
+-rw-r--r--   0        0        0     5063 2024-02-21 00:32:47.130497 pygpt_net-2.1.9/src/pygpt_net/item/assistant.py
+-rw-r--r--   0        0        0     1816 2024-01-27 21:42:30.960980 pygpt_net-2.1.9/src/pygpt_net/item/attachment.py
+-rw-r--r--   0        0        0     2108 2024-01-27 21:42:30.960980 pygpt_net-2.1.9/src/pygpt_net/item/calendar_note.py
+-rw-r--r--   0        0        0     9754 2024-03-04 21:08:00.701350 pygpt_net-2.1.9/src/pygpt_net/item/ctx.py
+-rw-r--r--   0        0        0     1681 2024-01-27 21:42:30.960980 pygpt_net-2.1.9/src/pygpt_net/item/index.py
+-rw-r--r--   0        0        0      600 2023-12-31 03:12:34.283242 pygpt_net-2.1.9/src/pygpt_net/item/mode.py
+-rw-r--r--   0        0        0     6208 2024-01-27 21:42:30.960980 pygpt_net-2.1.9/src/pygpt_net/item/model.py
+-rw-r--r--   0        0        0     1508 2024-01-27 21:42:30.960980 pygpt_net-2.1.9/src/pygpt_net/item/notepad.py
+-rw-r--r--   0        0        0     4052 2024-02-15 05:07:04.122540 pygpt_net-2.1.9/src/pygpt_net/item/preset.py
+-rwxr-xr-x   0        0        0     6616 2024-02-24 01:55:58.445111 pygpt_net-2.1.9/src/pygpt_net/launcher.py
+-rw-r--r--   0        0        0     2849 2023-12-28 02:55:13.572642 pygpt_net-2.1.9/src/pygpt_net/migrations/Version20231227152900.py
+-rw-r--r--   0        0        0      906 2023-12-30 08:47:37.360628 pygpt_net-2.1.9/src/pygpt_net/migrations/Version20231230095000.py
+-rw-r--r--   0        0        0      901 2024-01-01 00:17:57.553256 pygpt_net-2.1.9/src/pygpt_net/migrations/Version20231231230000.py
+-rw-r--r--   0        0        0     1303 2024-01-06 06:27:36.351928 pygpt_net-2.1.9/src/pygpt_net/migrations/Version20240106060000.py
+-rw-r--r--   0        0        0      865 2024-01-07 09:35:02.638810 pygpt_net-2.1.9/src/pygpt_net/migrations/Version20240107060000.py
+-rw-r--r--   0        0        0     1756 2024-02-23 01:50:39.602419 pygpt_net-2.1.9/src/pygpt_net/migrations/Version20240222160000.py
+-rw-r--r--   0        0        0     1099 2024-02-23 06:06:25.510176 pygpt_net-2.1.9/src/pygpt_net/migrations/Version20240223050000.py
+-rw-r--r--   0        0        0      847 2024-03-03 22:43:17.403437 pygpt_net-2.1.9/src/pygpt_net/migrations/Version20240303190000.py
+-rw-r--r--   0        0        0     1635 2024-03-03 22:43:17.403437 pygpt_net-2.1.9/src/pygpt_net/migrations/__init__.py
+-rw-r--r--   0        0        0      614 2023-12-28 02:55:13.572642 pygpt_net-2.1.9/src/pygpt_net/migrations/base.py
+-rwxr-xr-x   0        0        0      488 2023-12-25 22:13:46.802302 pygpt_net-2.1.9/src/pygpt_net/plugin/__init__.py
+-rwxr-xr-x   0        0        0    14479 2024-02-25 05:32:34.229344 pygpt_net-2.1.9/src/pygpt_net/plugin/agent/__init__.py
+-rwxr-xr-x   0        0        0    22052 2024-03-01 03:17:53.457929 pygpt_net-2.1.9/src/pygpt_net/plugin/audio_input/__init__.py
+-rw-r--r--   0        0        0     3787 2024-02-28 03:58:59.309445 pygpt_net-2.1.9/src/pygpt_net/plugin/audio_input/simple.py
+-rw-r--r--   0        0        0     9606 2024-02-28 03:58:59.309445 pygpt_net-2.1.9/src/pygpt_net/plugin/audio_input/worker.py
+-rwxr-xr-x   0        0        0     6589 2024-02-24 01:55:58.445111 pygpt_net-2.1.9/src/pygpt_net/plugin/audio_output/__init__.py
+-rw-r--r--   0        0        0     1763 2024-03-04 20:35:51.194582 pygpt_net-2.1.9/src/pygpt_net/plugin/audio_output/worker.py
+-rwxr-xr-x   0        0        0     9091 2024-03-04 21:10:30.303098 pygpt_net-2.1.9/src/pygpt_net/plugin/base.py
+-rwxr-xr-x   0        0        0    11627 2024-02-25 05:32:34.229344 pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_api/__init__.py
+-rw-r--r--   0        0        0     6823 2024-02-25 00:58:54.512534 pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_api/worker.py
+-rwxr-xr-x   0        0        0     7757 2024-02-18 06:49:52.494117 pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_code_interpreter/__init__.py
+-rw-r--r--   0        0        0    10352 2024-03-03 22:43:17.403437 pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_code_interpreter/runner.py
+-rw-r--r--   0        0        0     4749 2024-03-03 22:43:17.403437 pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_code_interpreter/worker.py
+-rwxr-xr-x   0        0        0     5717 2024-02-25 00:27:02.862945 pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_custom/__init__.py
+-rw-r--r--   0        0        0     4409 2024-02-25 00:27:02.862945 pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_custom/worker.py
+-rwxr-xr-x   0        0        0    16896 2024-03-04 19:26:20.301786 pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_files/__init__.py
+-rw-r--r--   0        0        0    32458 2024-03-04 19:26:20.257786 pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_files/worker.py
+-rwxr-xr-x   0        0        0    23473 2024-02-15 05:07:04.122540 pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_history/__init__.py
+-rwxr-xr-x   0        0        0     6969 2024-02-18 06:49:52.494117 pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_serial/__init__.py
+-rw-r--r--   0        0        0     8680 2024-01-30 17:23:19.897578 pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_serial/worker.py
+-rwxr-xr-x   0        0        0    20351 2024-03-04 19:45:01.492395 pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_web/__init__.py
+-rwxr-xr-x   0        0        0    12576 2024-02-24 01:55:58.445111 pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_web/websearch.py
+-rw-r--r--   0        0        0    10601 2024-03-04 19:26:20.297786 pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_web/worker.py
+-rwxr-xr-x   0        0        0     8158 2024-02-15 05:07:04.122540 pygpt_net-2.1.9/src/pygpt_net/plugin/crontab/__init__.py
+-rwxr-xr-x   0        0        0     2831 2024-02-18 01:14:49.758062 pygpt_net-2.1.9/src/pygpt_net/plugin/extra_prompt/__init__.py
+-rwxr-xr-x   0        0        0    13103 2024-03-03 22:43:17.403437 pygpt_net-2.1.9/src/pygpt_net/plugin/idx_llama_index/__init__.py
+-rwxr-xr-x   0        0        0     6330 2024-02-15 05:07:04.122540 pygpt_net-2.1.9/src/pygpt_net/plugin/openai_dalle/__init__.py
+-rwxr-xr-x   0        0        0    11455 2024-02-15 05:07:04.122540 pygpt_net-2.1.9/src/pygpt_net/plugin/openai_vision/__init__.py
+-rwxr-xr-x   0        0        0     4029 2024-02-04 17:46:05.314114 pygpt_net-2.1.9/src/pygpt_net/plugin/real_time/__init__.py
+-rw-r--r--   0        0        0      488 2023-12-25 22:13:46.802302 pygpt_net-2.1.9/src/pygpt_net/provider/__init__.py
+-rw-r--r--   0        0        0      488 2024-02-24 01:55:58.445111 pygpt_net-2.1.9/src/pygpt_net/provider/audio_input/__init__.py
+-rw-r--r--   0        0        0     1819 2024-02-27 05:21:39.771084 pygpt_net-2.1.9/src/pygpt_net/provider/audio_input/base.py
+-rw-r--r--   0        0        0     2818 2024-02-27 05:21:39.771084 pygpt_net-2.1.9/src/pygpt_net/provider/audio_input/bing_speech_recognition.py
+-rw-r--r--   0        0        0     2904 2024-02-27 05:21:39.771084 pygpt_net-2.1.9/src/pygpt_net/provider/audio_input/google_cloud_speech_recognition.py
+-rw-r--r--   0        0        0     2840 2024-02-27 05:21:39.771084 pygpt_net-2.1.9/src/pygpt_net/provider/audio_input/google_speech_recognition.py
+-rw-r--r--   0        0        0     2244 2024-03-01 03:17:53.457929 pygpt_net-2.1.9/src/pygpt_net/provider/audio_input/openai_whisper.py
+-rw-r--r--   0        0        0     3129 2024-03-01 03:17:53.457929 pygpt_net-2.1.9/src/pygpt_net/provider/audio_input/openai_whisper_local.py
+-rw-r--r--   0        0        0      488 2024-02-24 01:55:58.449111 pygpt_net-2.1.9/src/pygpt_net/provider/audio_output/__init__.py
+-rw-r--r--   0        0        0     1995 2024-02-27 05:21:39.771084 pygpt_net-2.1.9/src/pygpt_net/provider/audio_output/base.py
+-rw-r--r--   0        0        0     4231 2024-02-25 00:27:02.862945 pygpt_net-2.1.9/src/pygpt_net/provider/audio_output/eleven_labs.py
+-rw-r--r--   0        0        0     4286 2024-02-25 00:27:02.862945 pygpt_net-2.1.9/src/pygpt_net/provider/audio_output/google_tts.py
+-rw-r--r--   0        0        0     4960 2024-02-24 01:55:58.449111 pygpt_net-2.1.9/src/pygpt_net/provider/audio_output/ms_azure_tts.py
+-rw-r--r--   0        0        0     3056 2024-02-24 01:55:58.449111 pygpt_net-2.1.9/src/pygpt_net/provider/audio_output/openai_tts.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.1.9/src/pygpt_net/provider/core/__init__.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.1.9/src/pygpt_net/provider/core/assistant/__init__.py
+-rw-r--r--   0        0        0     1186 2024-01-23 23:46:30.499197 pygpt_net-2.1.9/src/pygpt_net/provider/core/assistant/base.py
+-rw-r--r--   0        0        0     5926 2024-01-23 23:46:30.499197 pygpt_net-2.1.9/src/pygpt_net/provider/core/assistant/json_file.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.1.9/src/pygpt_net/provider/core/attachment/__init__.py
+-rw-r--r--   0        0        0     1204 2024-01-23 23:46:30.499197 pygpt_net-2.1.9/src/pygpt_net/provider/core/attachment/base.py
+-rw-r--r--   0        0        0     5236 2024-01-23 23:46:30.499197 pygpt_net-2.1.9/src/pygpt_net/provider/core/attachment/json_file.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.1.9/src/pygpt_net/provider/core/calendar/__init__.py
+-rw-r--r--   0        0        0     1322 2024-01-23 23:46:30.499197 pygpt_net-2.1.9/src/pygpt_net/provider/core/calendar/base.py
+-rw-r--r--   0        0        0     3832 2024-02-02 19:26:46.619683 pygpt_net-2.1.9/src/pygpt_net/provider/core/calendar/db_sqlite/__init__.py
+-rw-r--r--   0        0        0      837 2024-01-23 23:46:30.499197 pygpt_net-2.1.9/src/pygpt_net/provider/core/calendar/db_sqlite/patch.py
+-rw-r--r--   0        0        0    10959 2024-01-23 23:46:30.499197 pygpt_net-2.1.9/src/pygpt_net/provider/core/calendar/db_sqlite/storage.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.1.9/src/pygpt_net/provider/core/config/__init__.py
+-rw-r--r--   0        0        0     1235 2024-01-23 23:46:30.499197 pygpt_net-2.1.9/src/pygpt_net/provider/core/config/base.py
+-rwxr-xr-x   0        0        0     5017 2024-01-23 23:46:30.499197 pygpt_net-2.1.9/src/pygpt_net/provider/core/config/json_file.py
+-rwxr-xr-x   0        0        0    57620 2024-03-04 20:18:37.601991 pygpt_net-2.1.9/src/pygpt_net/provider/core/config/patch.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.1.9/src/pygpt_net/provider/core/ctx/__init__.py
+-rw-r--r--   0        0        0     2085 2024-02-23 01:50:39.602419 pygpt_net-2.1.9/src/pygpt_net/provider/core/ctx/base.py
+-rw-r--r--   0        0        0     7059 2024-02-23 01:50:39.602419 pygpt_net-2.1.9/src/pygpt_net/provider/core/ctx/db_sqlite/__init__.py
+-rw-r--r--   0        0        0     3101 2024-01-23 23:46:30.499197 pygpt_net-2.1.9/src/pygpt_net/provider/core/ctx/db_sqlite/patch.py
+-rw-r--r--   0        0        0    23675 2024-03-03 22:43:17.403437 pygpt_net-2.1.9/src/pygpt_net/provider/core/ctx/db_sqlite/storage.py
+-rw-r--r--   0        0        0     6888 2024-03-03 22:43:17.403437 pygpt_net-2.1.9/src/pygpt_net/provider/core/ctx/db_sqlite/utils.py
+-rw-r--r--   0        0        0    11665 2024-01-23 23:46:30.503197 pygpt_net-2.1.9/src/pygpt_net/provider/core/ctx/json_file.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.1.9/src/pygpt_net/provider/core/history/__init__.py
+-rw-r--r--   0        0        0      863 2024-01-23 23:46:30.503197 pygpt_net-2.1.9/src/pygpt_net/provider/core/history/base.py
+-rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.1.9/src/pygpt_net/provider/core/history/patch.py
+-rw-r--r--   0        0        0     2969 2024-01-23 23:46:30.503197 pygpt_net-2.1.9/src/pygpt_net/provider/core/history/txt_file.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.1.9/src/pygpt_net/provider/core/index/__init__.py
+-rw-r--r--   0        0        0     2814 2024-02-23 06:06:25.510176 pygpt_net-2.1.9/src/pygpt_net/provider/core/index/base.py
+-rw-r--r--   0        0        0     8217 2024-02-23 06:06:25.510176 pygpt_net-2.1.9/src/pygpt_net/provider/core/index/db_sqlite/__init__.py
+-rw-r--r--   0        0        0     2972 2024-02-23 06:06:25.510176 pygpt_net-2.1.9/src/pygpt_net/provider/core/index/db_sqlite/patch.py
+-rw-r--r--   0        0        0    16519 2024-02-23 06:06:25.510176 pygpt_net-2.1.9/src/pygpt_net/provider/core/index/db_sqlite/storage.py
+-rw-r--r--   0        0        0      870 2024-02-23 01:50:39.606418 pygpt_net-2.1.9/src/pygpt_net/provider/core/index/db_sqlite/utils.py
+-rw-r--r--   0        0        0     6615 2024-02-23 01:50:39.606418 pygpt_net-2.1.9/src/pygpt_net/provider/core/index/json_file.py
+-rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.1.9/src/pygpt_net/provider/core/index/patch.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.1.9/src/pygpt_net/provider/core/mode/__init__.py
+-rw-r--r--   0        0        0     1062 2024-01-23 23:46:30.503197 pygpt_net-2.1.9/src/pygpt_net/provider/core/mode/base.py
+-rw-r--r--   0        0        0     4142 2024-01-23 23:46:30.503197 pygpt_net-2.1.9/src/pygpt_net/provider/core/mode/json_file.py
+-rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.1.9/src/pygpt_net/provider/core/mode/patch.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.1.9/src/pygpt_net/provider/core/model/__init__.py
+-rw-r--r--   0        0        0     1246 2024-01-23 23:46:30.503197 pygpt_net-2.1.9/src/pygpt_net/provider/core/model/base.py
+-rw-r--r--   0        0        0     6231 2024-01-23 23:46:30.503197 pygpt_net-2.1.9/src/pygpt_net/provider/core/model/json_file.py
+-rw-r--r--   0        0        0     7363 2024-01-30 21:49:30.562821 pygpt_net-2.1.9/src/pygpt_net/provider/core/model/patch.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.1.9/src/pygpt_net/provider/core/notepad/__init__.py
+-rw-r--r--   0        0        0     1262 2024-01-23 23:46:30.503197 pygpt_net-2.1.9/src/pygpt_net/provider/core/notepad/base.py
+-rw-r--r--   0        0        0     3044 2024-01-23 23:46:30.503197 pygpt_net-2.1.9/src/pygpt_net/provider/core/notepad/db_sqlite/__init__.py
+-rw-r--r--   0        0        0     2805 2024-01-23 23:46:30.503197 pygpt_net-2.1.9/src/pygpt_net/provider/core/notepad/db_sqlite/patch.py
+-rw-r--r--   0        0        0     7263 2024-01-23 23:46:30.503197 pygpt_net-2.1.9/src/pygpt_net/provider/core/notepad/db_sqlite/storage.py
+-rw-r--r--   0        0        0     7555 2024-01-23 23:46:30.503197 pygpt_net-2.1.9/src/pygpt_net/provider/core/notepad/json_file.py
+-rwxr-xr-x   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.1.9/src/pygpt_net/provider/core/preset/__init__.py
+-rwxr-xr-x   0        0        0     1300 2024-02-01 01:48:09.374583 pygpt_net-2.1.9/src/pygpt_net/provider/core/preset/base.py
+-rwxr-xr-x   0        0        0     7887 2024-02-15 05:07:04.122540 pygpt_net-2.1.9/src/pygpt_net/provider/core/preset/json_file.py
+-rw-r--r--   0        0        0     3166 2024-01-23 23:46:30.503197 pygpt_net-2.1.9/src/pygpt_net/provider/core/preset/patch.py
+-rw-r--r--   0        0        0     6739 2024-02-21 03:55:24.484309 pygpt_net-2.1.9/src/pygpt_net/provider/gpt/__init__.py
+-rw-r--r--   0        0        0    13251 2024-02-21 19:09:37.240983 pygpt_net-2.1.9/src/pygpt_net/provider/gpt/assistants.py
+-rw-r--r--   0        0        0     5763 2024-02-15 05:07:04.122540 pygpt_net-2.1.9/src/pygpt_net/provider/gpt/chat.py
+-rw-r--r--   0        0        0     5169 2024-01-27 01:08:27.560991 pygpt_net-2.1.9/src/pygpt_net/provider/gpt/completion.py
+-rw-r--r--   0        0        0     7904 2024-02-18 06:49:52.494117 pygpt_net-2.1.9/src/pygpt_net/provider/gpt/image.py
+-rw-r--r--   0        0        0     2681 2024-01-27 01:08:27.560991 pygpt_net-2.1.9/src/pygpt_net/provider/gpt/summarizer.py
+-rw-r--r--   0        0        0     7079 2024-02-16 04:34:22.756884 pygpt_net-2.1.9/src/pygpt_net/provider/gpt/vision.py
+-rw-r--r--   0        0        0        0 2024-02-20 19:10:03.189314 pygpt_net-2.1.9/src/pygpt_net/provider/gpt/worker/__init__.py
+-rw-r--r--   0        0        0     5916 2024-02-21 00:32:47.130497 pygpt_net-2.1.9/src/pygpt_net/provider/gpt/worker/assistants.py
+-rw-r--r--   0        0        0     4665 2024-02-21 19:09:37.240983 pygpt_net-2.1.9/src/pygpt_net/provider/gpt/worker/importer.py
+-rwxr-xr-x   0        0        0        0 2024-01-27 21:42:30.960980 pygpt_net-2.1.9/src/pygpt_net/provider/llms/__init__.py
+-rwxr-xr-x   0        0        0     1641 2024-01-27 21:42:30.960980 pygpt_net-2.1.9/src/pygpt_net/provider/llms/anthropic.py
+-rwxr-xr-x   0        0        0     1633 2024-02-28 03:58:59.309445 pygpt_net-2.1.9/src/pygpt_net/provider/llms/azure_openai.py
+-rw-r--r--   0        0        0     2694 2024-01-27 21:42:30.960980 pygpt_net-2.1.9/src/pygpt_net/provider/llms/base.py
+-rwxr-xr-x   0        0        0     1535 2024-01-27 21:42:30.960980 pygpt_net-2.1.9/src/pygpt_net/provider/llms/hugging_face.py
+-rwxr-xr-x   0        0        0     1643 2024-01-27 21:42:30.960980 pygpt_net-2.1.9/src/pygpt_net/provider/llms/llama.py
+-rwxr-xr-x   0        0        0     1517 2024-01-27 21:42:30.960980 pygpt_net-2.1.9/src/pygpt_net/provider/llms/ollama.py
+-rwxr-xr-x   0        0        0     2048 2024-02-28 03:58:59.309445 pygpt_net-2.1.9/src/pygpt_net/provider/llms/openai.py
+-rw-r--r--   0        0        0        0 2024-01-23 23:46:30.503197 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/__init__.py
+-rw-r--r--   0        0        0     2481 2024-03-01 03:17:53.457929 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/base.py
+-rw-r--r--   0        0        0     1149 2024-02-29 03:07:51.278132 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/file_csv.py
+-rw-r--r--   0        0        0     1032 2024-02-29 03:07:51.278132 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/file_docx.py
+-rw-r--r--   0        0        0     1022 2024-02-29 03:07:51.278132 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/file_epub.py
+-rw-r--r--   0        0        0     1032 2024-02-28 03:58:59.309445 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/file_excel.py
+-rw-r--r--   0        0        0     1163 2024-02-29 03:07:51.278132 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/file_html.py
+-rw-r--r--   0        0        0     1680 2024-03-01 03:17:53.457929 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/file_image_vision.py
+-rw-r--r--   0        0        0     1169 2024-02-29 03:07:51.278132 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/file_ipynb.py
+-rw-r--r--   0        0        0      996 2024-02-28 03:58:59.309445 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/file_json.py
+-rw-r--r--   0        0        0     1171 2024-02-29 03:07:51.278132 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/file_markdown.py
+-rw-r--r--   0        0        0     1127 2024-02-29 03:07:51.278132 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/file_pdf.py
+-rw-r--r--   0        0        0     1720 2024-03-01 03:17:53.457929 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/file_video_audio.py
+-rw-r--r--   0        0        0     1114 2024-02-29 03:07:51.278132 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/file_xml.py
+-rw-r--r--   0        0        0        0 2024-01-27 21:42:30.960980 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/bitbucket/__init__.py
+-rw-r--r--   0        0        0     6194 2024-03-01 17:40:19.825274 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/bitbucket/repo.py
+-rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/__init__.py
+-rw-r--r--   0        0        0     2460 2024-03-01 17:40:19.825274 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/base.py
+-rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/database/__init__.py
+-rw-r--r--   0        0        0     4228 2024-03-01 17:40:19.825274 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/database/base.py
+-rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/github/__init__.py
+-rw-r--r--   0        0        0     4204 2024-03-01 17:40:19.825274 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/github/issues.py
+-rw-r--r--   0        0        0     3550 2024-03-01 17:40:19.825274 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/github/repo.py
+-rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/google/__init__.py
+-rw-r--r--   0        0        0     2658 2024-03-01 03:17:53.457929 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/google/calendar.py
+-rw-r--r--   0        0        0     5370 2024-03-01 03:17:53.457929 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/google/docs.py
+-rw-r--r--   0        0        0     6772 2024-03-01 03:17:53.457929 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/google/gmail.py
+-rw-r--r--   0        0        0     1633 2024-03-01 03:17:53.457929 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/google/keep.py
+-rw-r--r--   0        0        0     5282 2024-03-01 03:17:53.457929 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/google/sheets.py
+-rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/image_vision/__init__.py
+-rw-r--r--   0        0        0     6940 2024-03-01 03:17:53.457929 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/image_vision/base.py
+-rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/json/__init__.py
+-rw-r--r--   0        0        0     3862 2024-02-29 03:07:51.278132 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/json/base.py
+-rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/pandas_excel/__init__.py
+-rw-r--r--   0        0        0     3940 2024-02-29 03:07:51.278132 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/pandas_excel/base.py
+-rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/simple_csv/__init__.py
+-rw-r--r--   0        0        0     1481 2024-02-29 03:07:51.278132 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/simple_csv/base.py
+-rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/video_audio/__init__.py
+-rw-r--r--   0        0        0     4960 2024-03-01 03:17:53.457929 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/video_audio/base.py
+-rw-r--r--   0        0        0        0 2024-02-27 05:21:39.771084 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/web_page/__init__.py
+-rw-r--r--   0        0        0      556 2024-02-29 03:07:51.278132 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/web_page/base.py
+-rw-r--r--   0        0        0        0 2024-02-27 05:21:39.771084 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/yt/__init__.py
+-rw-r--r--   0        0        0     2427 2024-02-29 03:07:51.278132 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/yt/base.py
+-rw-r--r--   0        0        0      545 2024-02-27 05:21:39.771084 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/yt/utils.py
+-rw-r--r--   0        0        0     3078 2024-03-01 17:40:19.825274 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_bitbucket.py
+-rw-r--r--   0        0        0     2280 2024-03-01 17:40:19.825274 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_chatgpt_retrieval.py
+-rw-r--r--   0        0        0     2392 2024-03-01 17:40:19.825274 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_database.py
+-rw-r--r--   0        0        0     3223 2024-03-01 17:40:19.825274 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_github_issues.py
+-rw-r--r--   0        0        0     3556 2024-03-01 17:40:19.825274 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_github_repo.py
+-rw-r--r--   0        0        0     2499 2024-03-01 03:17:53.457929 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_google_calendar.py
+-rw-r--r--   0        0        0     2236 2024-03-01 03:17:53.457929 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_google_docs.py
+-rw-r--r--   0        0        0     3180 2024-03-01 03:17:53.457929 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_google_drive.py
+-rw-r--r--   0        0        0     2319 2024-03-01 03:17:53.457929 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_google_gmail.py
+-rw-r--r--   0        0        0     2201 2024-03-01 03:17:53.457929 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_google_keep.py
+-rw-r--r--   0        0        0     2313 2024-03-01 03:17:53.457929 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_google_sheets.py
+-rw-r--r--   0        0        0     3443 2024-03-01 17:40:19.825274 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_microsoft_onedrive.py
+-rw-r--r--   0        0        0     1399 2024-03-01 03:17:53.457929 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_page.py
+-rw-r--r--   0        0        0     1404 2024-03-01 03:17:53.457929 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_rss.py
+-rw-r--r--   0        0        0     1575 2024-03-01 03:17:53.461929 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_sitemap.py
+-rw-r--r--   0        0        0     2512 2024-03-03 03:52:54.350656 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_twitter.py
+-rw-r--r--   0        0        0     1442 2024-03-01 03:17:53.461929 pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_yt.py
+-rw-r--r--   0        0        0     5396 2024-03-03 22:43:17.403437 pygpt_net-2.1.9/src/pygpt_net/provider/vector_stores/__init__.py
+-rw-r--r--   0        0        0     3112 2024-02-28 03:58:59.313445 pygpt_net-2.1.9/src/pygpt_net/provider/vector_stores/base.py
+-rwxr-xr-x   0        0        0     3169 2024-03-03 03:52:54.350656 pygpt_net-2.1.9/src/pygpt_net/provider/vector_stores/chroma.py
+-rw-r--r--   0        0        0     3152 2024-02-28 03:58:59.313445 pygpt_net-2.1.9/src/pygpt_net/provider/vector_stores/elasticsearch.py
+-rw-r--r--   0        0        0     5177 2024-02-28 03:58:59.313445 pygpt_net-2.1.9/src/pygpt_net/provider/vector_stores/pinecode.py
+-rw-r--r--   0        0        0     3183 2024-02-28 03:58:59.313445 pygpt_net-2.1.9/src/pygpt_net/provider/vector_stores/redis.py
+-rw-r--r--   0        0        0     2524 2024-02-28 03:58:59.313445 pygpt_net-2.1.9/src/pygpt_net/provider/vector_stores/simple.py
+-rw-r--r--   0        0        0     3923 2024-03-03 22:43:17.403437 pygpt_net-2.1.9/src/pygpt_net/provider/vector_stores/temp.py
+-rw-r--r--   0        0        0      488 2024-02-24 01:55:58.449111 pygpt_net-2.1.9/src/pygpt_net/provider/web/__init__.py
+-rw-r--r--   0        0        0     1994 2024-02-27 05:21:39.771084 pygpt_net-2.1.9/src/pygpt_net/provider/web/base.py
+-rw-r--r--   0        0        0     4646 2024-02-25 00:27:02.862945 pygpt_net-2.1.9/src/pygpt_net/provider/web/google_custom_search.py
+-rw-r--r--   0        0        0     4104 2024-02-25 00:27:02.862945 pygpt_net-2.1.9/src/pygpt_net/provider/web/microsoft_bing.py
+-rwxr-xr-x   0        0        0     5680 2024-01-29 18:11:38.035830 pygpt_net-2.1.9/src/pygpt_net/ui/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-08 20:36:28.054492 pygpt_net-2.1.9/src/pygpt_net/ui/base/__init__.py
+-rw-r--r--   0        0        0     9209 2024-02-27 05:21:39.771084 pygpt_net-2.1.9/src/pygpt_net/ui/base/config_dialog.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 18:11:19.000000 pygpt_net-2.1.9/src/pygpt_net/ui/dialog/__init__.py
+-rwxr-xr-x   0        0        0     5579 2024-02-28 03:58:59.313445 pygpt_net-2.1.9/src/pygpt_net/ui/dialog/about.py
+-rwxr-xr-x   0        0        0     4722 2024-02-15 05:07:04.122540 pygpt_net-2.1.9/src/pygpt_net/ui/dialog/applog.py
+-rwxr-xr-x   0        0        0     6534 2024-02-15 05:07:04.122540 pygpt_net-2.1.9/src/pygpt_net/ui/dialog/assistant.py
+-rwxr-xr-x   0        0        0     1765 2024-02-01 17:53:56.370106 pygpt_net-2.1.9/src/pygpt_net/ui/dialog/changelog.py
+-rw-r--r--   0        0        0      973 2024-01-28 19:32:28.495073 pygpt_net-2.1.9/src/pygpt_net/ui/dialog/create.py
+-rwxr-xr-x   0        0        0     1798 2024-02-26 21:30:35.305131 pygpt_net-2.1.9/src/pygpt_net/ui/dialog/debug.py
+-rw-r--r--   0        0        0     5490 2024-01-31 21:39:19.388967 pygpt_net-2.1.9/src/pygpt_net/ui/dialog/dictionary.py
+-rwxr-xr-x   0        0        0     2382 2024-01-27 21:42:30.964980 pygpt_net-2.1.9/src/pygpt_net/ui/dialog/editor.py
+-rwxr-xr-x   0        0        0     2867 2024-01-19 21:21:41.774598 pygpt_net-2.1.9/src/pygpt_net/ui/dialog/image.py
+-rwxr-xr-x   0        0        0     2272 2024-02-01 17:53:56.370106 pygpt_net-2.1.9/src/pygpt_net/ui/dialog/license.py
+-rwxr-xr-x   0        0        0     1706 2024-01-27 21:42:30.964980 pygpt_net-2.1.9/src/pygpt_net/ui/dialog/logger.py
+-rw-r--r--   0        0        0    12634 2024-02-15 05:07:04.122540 pygpt_net-2.1.9/src/pygpt_net/ui/dialog/models.py
+-rwxr-xr-x   0        0        0    19464 2024-03-02 19:51:00.168984 pygpt_net-2.1.9/src/pygpt_net/ui/dialog/plugins.py
+-rwxr-xr-x   0        0        0     6644 2024-02-15 05:07:04.122540 pygpt_net-2.1.9/src/pygpt_net/ui/dialog/preset.py
+-rwxr-xr-x   0        0        0      973 2024-01-28 19:32:28.495073 pygpt_net-2.1.9/src/pygpt_net/ui/dialog/rename.py
+-rwxr-xr-x   0        0        0    14557 2024-02-29 03:07:51.278132 pygpt_net-2.1.9/src/pygpt_net/ui/dialog/settings.py
+-rw-r--r--   0        0        0      954 2024-02-26 22:26:37.124323 pygpt_net-2.1.9/src/pygpt_net/ui/dialog/snap.py
+-rwxr-xr-x   0        0        0     2436 2024-02-25 05:55:37.513980 pygpt_net-2.1.9/src/pygpt_net/ui/dialog/start.py
+-rwxr-xr-x   0        0        0      842 2023-12-28 18:11:19.000000 pygpt_net-2.1.9/src/pygpt_net/ui/dialog/update.py
+-rwxr-xr-x   0        0        0     7005 2024-02-28 03:58:59.313445 pygpt_net-2.1.9/src/pygpt_net/ui/dialogs.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.1.9/src/pygpt_net/ui/layout/__init__.py
+-rwxr-xr-x   0        0        0     1535 2023-12-29 00:18:50.793125 pygpt_net-2.1.9/src/pygpt_net/ui/layout/chat/__init__.py
+-rwxr-xr-x   0        0        0     5149 2024-01-28 22:32:36.115407 pygpt_net-2.1.9/src/pygpt_net/ui/layout/chat/attachments.py
+-rwxr-xr-x   0        0        0     4376 2024-01-27 21:42:30.964980 pygpt_net-2.1.9/src/pygpt_net/ui/layout/chat/attachments_uploaded.py
+-rw-r--r--   0        0        0     5118 2024-02-23 01:50:39.606418 pygpt_net-2.1.9/src/pygpt_net/ui/layout/chat/calendar.py
+-rwxr-xr-x   0        0        0     9051 2024-02-26 21:30:35.305131 pygpt_net-2.1.9/src/pygpt_net/ui/layout/chat/input.py
+-rwxr-xr-x   0        0        0    18656 2024-01-01 00:17:57.553256 pygpt_net-2.1.9/src/pygpt_net/ui/layout/chat/markdown.py
+-rwxr-xr-x   0        0        0     9142 2024-02-29 03:07:51.278132 pygpt_net-2.1.9/src/pygpt_net/ui/layout/chat/output.py
+-rw-r--r--   0        0        0     5199 2024-02-17 21:22:47.345663 pygpt_net-2.1.9/src/pygpt_net/ui/layout/chat/painter.py
+-rwxr-xr-x   0        0        0     1697 2024-01-27 21:42:30.964980 pygpt_net-2.1.9/src/pygpt_net/ui/layout/ctx/__init__.py
+-rwxr-xr-x   0        0        0     4902 2024-02-02 19:26:46.619683 pygpt_net-2.1.9/src/pygpt_net/ui/layout/ctx/ctx_list.py
+-rwxr-xr-x   0        0        0     1441 2024-01-07 09:35:02.638810 pygpt_net-2.1.9/src/pygpt_net/ui/layout/ctx/search_input.py
+-rwxr-xr-x   0        0        0     1068 2023-12-31 01:26:09.880264 pygpt_net-2.1.9/src/pygpt_net/ui/layout/ctx/video.py
+-rwxr-xr-x   0        0        0     1405 2024-01-31 15:19:17.742029 pygpt_net-2.1.9/src/pygpt_net/ui/layout/status.py
+-rwxr-xr-x   0        0        0     3475 2024-01-27 21:42:30.964980 pygpt_net-2.1.9/src/pygpt_net/ui/layout/toolbox/__init__.py
+-rw-r--r--   0        0        0     2378 2024-01-30 17:23:19.901578 pygpt_net-2.1.9/src/pygpt_net/ui/layout/toolbox/agent.py
+-rwxr-xr-x   0        0        0     4414 2024-01-27 21:42:30.964980 pygpt_net-2.1.9/src/pygpt_net/ui/layout/toolbox/assistants.py
+-rwxr-xr-x   0        0        0     4254 2024-02-29 03:07:51.278132 pygpt_net-2.1.9/src/pygpt_net/ui/layout/toolbox/footer.py
+-rwxr-xr-x   0        0        0     2382 2024-01-21 16:42:14.672394 pygpt_net-2.1.9/src/pygpt_net/ui/layout/toolbox/image.py
+-rw-r--r--   0        0        0     5075 2024-01-27 21:42:30.964980 pygpt_net-2.1.9/src/pygpt_net/ui/layout/toolbox/indexes.py
+-rwxr-xr-x   0        0        0     3169 2024-02-21 03:55:24.484309 pygpt_net-2.1.9/src/pygpt_net/ui/layout/toolbox/mode.py
+-rwxr-xr-x   0        0        0     3067 2024-02-21 03:55:24.484309 pygpt_net-2.1.9/src/pygpt_net/ui/layout/toolbox/model.py
+-rwxr-xr-x   0        0        0     4127 2024-02-01 00:24:56.153509 pygpt_net-2.1.9/src/pygpt_net/ui/layout/toolbox/presets.py
+-rwxr-xr-x   0        0        0     3502 2024-02-01 13:33:50.646121 pygpt_net-2.1.9/src/pygpt_net/ui/layout/toolbox/prompt.py
+-rwxr-xr-x   0        0        0     2447 2023-12-31 01:26:09.000000 pygpt_net-2.1.9/src/pygpt_net/ui/layout/toolbox/vision.py
+-rw-r--r--   0        0        0     7682 2024-02-24 01:55:58.449111 pygpt_net-2.1.9/src/pygpt_net/ui/main.py
+-rw-r--r--   0        0        0     1618 2024-02-29 03:07:51.278132 pygpt_net-2.1.9/src/pygpt_net/ui/menu/__init__.py
+-rw-r--r--   0        0        0     4667 2024-02-16 20:38:22.746568 pygpt_net-2.1.9/src/pygpt_net/ui/menu/about.py
+-rw-r--r--   0        0        0     1654 2024-02-28 03:58:59.313445 pygpt_net-2.1.9/src/pygpt_net/ui/menu/audio.py
+-rw-r--r--   0        0        0     5142 2024-02-16 20:38:22.746568 pygpt_net-2.1.9/src/pygpt_net/ui/menu/config.py
+-rw-r--r--   0        0        0     4875 2024-02-25 18:06:16.209368 pygpt_net-2.1.9/src/pygpt_net/ui/menu/debug.py
+-rw-r--r--   0        0        0     2014 2024-02-16 20:38:22.746568 pygpt_net-2.1.9/src/pygpt_net/ui/menu/file.py
+-rw-r--r--   0        0        0      897 2024-01-27 21:42:30.964980 pygpt_net-2.1.9/src/pygpt_net/ui/menu/lang.py
+-rw-r--r--   0        0        0     1549 2024-02-16 20:38:22.746568 pygpt_net-2.1.9/src/pygpt_net/ui/menu/plugins.py
+-rw-r--r--   0        0        0     2685 2024-02-16 20:38:22.746568 pygpt_net-2.1.9/src/pygpt_net/ui/menu/theme.py
+-rw-r--r--   0        0        0     2026 2024-02-29 03:07:51.278132 pygpt_net-2.1.9/src/pygpt_net/ui/menu/video.py
+-rw-r--r--   0        0        0     6672 2024-02-01 23:02:10.688691 pygpt_net-2.1.9/src/pygpt_net/ui/tray.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 18:11:19.000000 pygpt_net-2.1.9/src/pygpt_net/ui/widget/__init__.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.1.9/src/pygpt_net/ui/widget/audio/__init__.py
+-rwxr-xr-x   0        0        0     1721 2023-12-28 21:20:40.362230 pygpt_net-2.1.9/src/pygpt_net/ui/widget/audio/input.py
+-rw-r--r--   0        0        0     2198 2024-02-29 03:07:51.278132 pygpt_net-2.1.9/src/pygpt_net/ui/widget/audio/input_button.py
+-rwxr-xr-x   0        0        0     1586 2023-12-28 21:20:40.362230 pygpt_net-2.1.9/src/pygpt_net/ui/widget/audio/output.py
+-rw-r--r--   0        0        0        0 2024-01-06 03:25:04.270157 pygpt_net-2.1.9/src/pygpt_net/ui/widget/calendar/__init__.py
+-rw-r--r--   0        0        0     8116 2024-02-17 21:22:47.345663 pygpt_net-2.1.9/src/pygpt_net/ui/widget/calendar/select.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/__init__.py
+-rwxr-xr-x   0        0        0     1308 2024-02-16 17:50:31.993013 pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/alert.py
+-rw-r--r--   0        0        0     1502 2024-02-17 21:22:47.345663 pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/applog.py
+-rw-r--r--   0        0        0     3163 2024-02-28 03:58:59.313445 pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/base.py
+-rwxr-xr-x   0        0        0     1977 2024-01-24 15:53:01.386042 pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/confirm.py
+-rw-r--r--   0        0        0     2191 2024-01-28 19:32:28.495073 pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/create.py
+-rwxr-xr-x   0        0        0     1572 2024-02-21 16:35:35.211671 pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/debug.py
+-rwxr-xr-x   0        0        0     1749 2024-02-17 21:22:47.345663 pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/editor.py
+-rwxr-xr-x   0        0        0     1638 2024-02-17 21:22:47.345663 pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/editor_file.py
+-rwxr-xr-x   0        0        0      816 2024-02-17 21:22:47.345663 pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/image.py
+-rwxr-xr-x   0        0        0     1568 2024-02-17 21:22:47.345663 pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/info.py
+-rw-r--r--   0        0        0     1717 2024-02-17 21:22:47.345663 pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/license.py
+-rwxr-xr-x   0        0        0     1627 2024-02-17 21:22:47.345663 pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/logger.py
+-rw-r--r--   0        0        0     1625 2024-02-17 21:22:47.345663 pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/model.py
+-rwxr-xr-x   0        0        0     2191 2024-01-28 19:32:28.495073 pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/rename.py
+-rwxr-xr-x   0        0        0     1614 2024-02-17 21:22:47.345663 pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/settings.py
+-rwxr-xr-x   0        0        0     1696 2024-02-17 21:22:47.345663 pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/settings_plugin.py
+-rw-r--r--   0        0        0     2724 2024-02-26 22:26:37.124323 pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/snap.py
+-rwxr-xr-x   0        0        0     6789 2024-02-17 21:22:47.345663 pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/update.py
+-rwxr-xr-x   0        0        0      488 2024-01-11 15:56:53.277343 pygpt_net-2.1.9/src/pygpt_net/ui/widget/draw/__init__.py
+-rw-r--r--   0        0        0     9057 2024-03-01 17:40:19.825274 pygpt_net-2.1.9/src/pygpt_net/ui/widget/draw/painter.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.1.9/src/pygpt_net/ui/widget/element/__init__.py
+-rw-r--r--   0        0        0      947 2024-01-13 00:42:12.107250 pygpt_net-2.1.9/src/pygpt_net/ui/widget/element/button.py
+-rwxr-xr-x   0        0        0     2559 2024-01-27 21:42:30.964980 pygpt_net-2.1.9/src/pygpt_net/ui/widget/element/group.py
+-rw-r--r--   0        0        0     3789 2024-02-28 03:58:59.313445 pygpt_net-2.1.9/src/pygpt_net/ui/widget/element/labels.py
+-rwxr-xr-x   0        0        0        0 2023-12-28 21:20:40.362230 pygpt_net-2.1.9/src/pygpt_net/ui/widget/filesystem/__init__.py
+-rwxr-xr-x   0        0        0    21480 2024-03-02 19:51:00.168984 pygpt_net-2.1.9/src/pygpt_net/ui/widget/filesystem/explorer.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.1.9/src/pygpt_net/ui/widget/image/__init__.py
+-rwxr-xr-x   0        0        0     2823 2024-01-29 13:41:53.379769 pygpt_net-2.1.9/src/pygpt_net/ui/widget/image/display.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.1.9/src/pygpt_net/ui/widget/lists/__init__.py
+-rwxr-xr-x   0        0        0     2682 2024-01-29 13:41:53.379769 pygpt_net-2.1.9/src/pygpt_net/ui/widget/lists/assistant.py
+-rwxr-xr-x   0        0        0     4750 2024-01-29 13:41:53.379769 pygpt_net-2.1.9/src/pygpt_net/ui/widget/lists/attachment.py
+-rwxr-xr-x   0        0        0     2446 2023-12-28 21:20:40.362230 pygpt_net-2.1.9/src/pygpt_net/ui/widget/lists/base.py
+-rwxr-xr-x   0        0        0    11603 2024-02-25 00:27:02.862945 pygpt_net-2.1.9/src/pygpt_net/ui/widget/lists/context.py
+-rw-r--r--   0        0        0     3653 2024-02-25 22:01:41.690831 pygpt_net-2.1.9/src/pygpt_net/ui/widget/lists/debug.py
+-rw-r--r--   0        0        0     4821 2024-01-31 21:39:19.388967 pygpt_net-2.1.9/src/pygpt_net/ui/widget/lists/index.py
+-rwxr-xr-x   0        0        0     1080 2023-12-28 21:20:40.362230 pygpt_net-2.1.9/src/pygpt_net/ui/widget/lists/mode.py
+-rwxr-xr-x   0        0        0     1912 2024-01-29 13:41:53.379769 pygpt_net-2.1.9/src/pygpt_net/ui/widget/lists/model.py
+-rw-r--r--   0        0        0     1919 2024-01-29 13:41:53.379769 pygpt_net-2.1.9/src/pygpt_net/ui/widget/lists/model_editor.py
+-rwxr-xr-x   0        0        0     1028 2024-01-12 09:25:47.589375 pygpt_net-2.1.9/src/pygpt_net/ui/widget/lists/plugin.py
+-rwxr-xr-x   0        0        0     4071 2024-02-01 01:48:09.378583 pygpt_net-2.1.9/src/pygpt_net/ui/widget/lists/preset.py
+-rw-r--r--   0        0        0     1052 2024-01-12 09:25:47.589375 pygpt_net-2.1.9/src/pygpt_net/ui/widget/lists/settings.py
+-rwxr-xr-x   0        0        0     4002 2024-01-29 13:41:53.379769 pygpt_net-2.1.9/src/pygpt_net/ui/widget/lists/uploaded.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.1.9/src/pygpt_net/ui/widget/option/__init__.py
+-rwxr-xr-x   0        0        0     2068 2024-01-19 21:21:41.774598 pygpt_net-2.1.9/src/pygpt_net/ui/widget/option/checkbox.py
+-rw-r--r--   0        0        0     2797 2024-03-03 03:52:54.350656 pygpt_net-2.1.9/src/pygpt_net/ui/widget/option/combo.py
+-rwxr-xr-x   0        0        0    12690 2024-01-30 01:28:33.748573 pygpt_net-2.1.9/src/pygpt_net/ui/widget/option/dictionary.py
+-rwxr-xr-x   0        0        0     5968 2024-02-16 20:38:22.746568 pygpt_net-2.1.9/src/pygpt_net/ui/widget/option/input.py
+-rwxr-xr-x   0        0        0     3569 2024-01-08 20:36:28.058493 pygpt_net-2.1.9/src/pygpt_net/ui/widget/option/slider.py
+-rwxr-xr-x   0        0        0     2077 2024-02-18 20:56:31.563530 pygpt_net-2.1.9/src/pygpt_net/ui/widget/option/textarea.py
+-rw-r--r--   0        0        0     1668 2024-01-29 13:41:53.379769 pygpt_net-2.1.9/src/pygpt_net/ui/widget/tabs/Input.py
+-rw-r--r--   0        0        0      488 2023-12-30 09:04:29.205425 pygpt_net-2.1.9/src/pygpt_net/ui/widget/tabs/__init__.py
+-rw-r--r--   0        0        0     2781 2024-02-16 20:38:22.746568 pygpt_net-2.1.9/src/pygpt_net/ui/widget/tabs/output.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.366230 pygpt_net-2.1.9/src/pygpt_net/ui/widget/textarea/__init__.py
+-rw-r--r--   0        0        0     4216 2024-01-30 17:23:19.901578 pygpt_net-2.1.9/src/pygpt_net/ui/widget/textarea/calendar_note.py
+-rw-r--r--   0        0        0     1358 2024-01-28 19:32:28.495073 pygpt_net-2.1.9/src/pygpt_net/ui/widget/textarea/create.py
+-rwxr-xr-x   0        0        0     4894 2024-02-25 00:27:02.862945 pygpt_net-2.1.9/src/pygpt_net/ui/widget/textarea/input.py
+-rwxr-xr-x   0        0        0     1132 2024-01-27 21:42:30.964980 pygpt_net-2.1.9/src/pygpt_net/ui/widget/textarea/name.py
+-rwxr-xr-x   0        0        0     5736 2024-02-25 00:27:02.862945 pygpt_net-2.1.9/src/pygpt_net/ui/widget/textarea/notepad.py
+-rwxr-xr-x   0        0        0     5241 2024-02-25 00:27:02.862945 pygpt_net-2.1.9/src/pygpt_net/ui/widget/textarea/output.py
+-rwxr-xr-x   0        0        0     1358 2024-01-28 19:32:28.495073 pygpt_net-2.1.9/src/pygpt_net/ui/widget/textarea/rename.py
+-rwxr-xr-x   0        0        0     1659 2024-02-03 15:51:10.611289 pygpt_net-2.1.9/src/pygpt_net/ui/widget/textarea/search_input.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.366230 pygpt_net-2.1.9/src/pygpt_net/ui/widget/vision/__init__.py
+-rwxr-xr-x   0        0        0     2584 2023-12-28 21:20:40.366230 pygpt_net-2.1.9/src/pygpt_net/ui/widget/vision/camera.py
+-rwxr-xr-x   0        0        0     3581 2024-02-28 03:58:59.313445 pygpt_net-2.1.9/src/pygpt_net/utils.py
+-rw-r--r--   0        0        0   128383 1970-01-01 00:00:00.000000 pygpt_net-2.1.9/PKG-INFO
```

### Comparing `pygpt_net-2.1.8/CHANGELOG.md` & `pygpt_net-2.1.9/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # CHANGELOG
 
+# 2.1.9 (2024-03-04)
+
+- A new option has been added to the `Web Search` plugin: `web_index_query`, which allows for indexing a web and external content in a temporary index (in memory) and quickly querying its content. Works similar to `query_file` command.
+- The `read_file` command has been expanded to handle multiple files at once.
+- Added `Log and debug events` option to Developer settings.
+
 # 2.1.8 (2024-03-03)
 
 - A new option has been added to the `Files I/O` plugin: `query_file`, which allows for indexing a file in a temporary index (in memory) and quickly querying its content. This enables the use of Llama-index for fast querying or adding context from individual files. From now on, you can ask questions about individual files without indexing them to the main vector store. See the "Querying single files" in "Modes -> Chat with files" section in a README for more info.
 - The `read_file` command has been expanded to return just the exact file content, without wrapping it in JSON.
 - Improved prompt for preparing queries in the Chat with files plugin.
 - Updated docs.
```

### Comparing `pygpt_net-2.1.8/LICENSE` & `pygpt_net-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/README.md` & `pygpt_net-2.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # PyGPT - Desktop AI Assistant
 
 [![pygpt](https://snapcraft.io/pygpt/badge.svg)](https://snapcraft.io/pygpt)
 
-Release: **2.1.8** | build: **2024.03.03** | Python: **>=3.10, <3.12**
+Release: **2.1.9** | build: **2024.03.04** | Python: **>=3.10, <3.12**
 
 Official website: https://pygpt.net | Documentation: https://pygpt.readthedocs.io
 
 Snap Store: https://snapcraft.io/pygpt | PyPi: https://pypi.org/project/pygpt-net
 
 Compiled version for Linux (`tar.gz`) and Windows 10/11 (`msi`) 64-bit: https://pygpt.net/#download
 
@@ -412,15 +412,15 @@
 ##  Chat with files (Llama-index)
 
 This mode enables chat interaction with your documents and entire context history through conversation. 
 It seamlessly incorporates `Llama-index` into the chat interface, allowing for immediate querying of your indexed documents.
 
 **Querying single files**
 
-From version `2.1.8`, you can also query individual files "on the fly" using the `query_file` command from the `Files I/O` plugin. This allows you to query any file by simply asking a question about that file. A temporary index will be created in memory for the file being queried, and an answer will be returned from it. 
+From version `2.1.8`, you can also query individual files "on the fly" using the `query_file` command from the `Files I/O` plugin. This allows you to query any file by simply asking a question about that file. A temporary index will be created in memory for the file being queried, and an answer will be returned from it. From version `2.1.9` similar command is available for querying web and external content: `Directly query web content with Llama-index`.
 
 For example:
 
 If you have a file: `data/my_cars.txt` with content `My car is red.`
 
 You can ask for: `Query the file my_cars.txt about what color my car is.`
 
@@ -1721,15 +1721,15 @@
 
 - `Enable: Read file` *cmd_read_file*
 
 Allows `read_file` command execution. *Default:* `True`
 
 - `Enable: Query file with Llama-index` *cmd_query_file*
 
-Allows `query_file` command execution *Default:* `True`
+Allows `query_file` command execution  (temporary index, on the fly) *Default:* `True`
 
 - `Enable: Append to file` *cmd_append_file*
 
 Allows `append_file` command execution. *Default:* `True`
 
 - `Enable: Save file` *cmd_save_file*
 
@@ -1914,27 +1914,29 @@
 
 If enabled, model will be able to open specified URL and get raw content
 
 - `Enable: "web_urls" command` *cmd_web_urls*
 
 If enabled, model will be able to search the Web and get founded URLs list
 
-If enabled, model will be able to search the Web and get founded URLs list
-
 - `Enable: "web_index" command` *cmd_web_index*
 
-If enabled, model will be able to index web pages using Llama-index
+If enabled, model will be able to index (on the fly) web pages using Llama-index (persistent index)
+
+- `Enable: "web_index_query" command - quick query the web content with Llama-index` *cmd_web_index_query*
+
+If enabled, model will be able to index and query web content using Llama-index (temporary index, on the fly)
 
 - `Auto-index all used URLs using Llama-index` *auto_index*
 
-If enabled, every URL used by the model will be automatically indexed using Llama-index
+If enabled, every URL used by the model will be automatically indexed using Llama-index (persistent index)
 
 - `Index to use` *idx*
 
-ID of index to use for web page indexing
+ID of index to use for web page indexing (persistent index)
 
 - `Model used for web page summarize` *summary_model*
 
 Model used for web page summarize, default: gpt-3.5-turbo-1106
 
 - `Summarize prompt` *prompt_summarize*
 
@@ -2729,15 +2731,17 @@
 
 - `Check for updates on start`: Enables checking for updates on start. Default: True.
 
 - `Check for updates in background`: Enables checking for updates in background (checking every 5 minutes). Default: True.
 
 **Developer**
 
-- `Show debug menu`: enables debug (developer) menu
+- `Show debug menu`: enables debug (developer) menu.
+
+- `Log and debug events`: Enables logging of events dispatch.
 
 - `Log plugin usage to console`: Enables logging of plugin usage to console.
 
 - `Log DALL-E usage to console`: Enables logging of DALL-E usage to console.
 
 - `Log Llama-index usage to console`: Enables logging of Llama-index usage to console.
 
@@ -2876,14 +2880,20 @@
 
 ---
 
 # CHANGELOG
 
 ## Recent changes:
 
+# 2.1.9 (2024-03-04)
+
+- A new option has been added to the `Web Search` plugin: `web_index_query`, which allows for indexing a web and external content in a temporary index (in memory) and quickly querying its content. Works similar to `query_file` command.
+- The `read_file` command has been expanded to handle multiple files at once.
+- Added `Log and debug events` option to Developer settings.
+
 # 2.1.8 (2024-03-03)
 
 - A new option has been added to the `Files I/O` plugin: `query_file`, which allows for indexing a file in a temporary index (in memory) and quickly querying its content. This enables the use of Llama-index for fast querying or adding context from individual files. From now on, you can ask questions about individual files without indexing them to the main vector store. See the "Querying single files" in "Modes -> Chat with files" section in a README for more info.
 - The `read_file` command has been expanded to return just the exact file content, without wrapping it in JSON.
 - Improved prompt for preparing queries in the Chat with files plugin.
 - Updated docs.
```

### Comparing `pygpt_net-2.1.8/icon.png` & `pygpt_net-2.1.9/icon.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/pyproject.toml` & `pygpt_net-2.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygpt-net"
-version = "2.1.8"
+version = "2.1.9"
 description = "Desktop AI Assistant powered by GPT-4, GPT-4V, GPT-3.5, DALL-E 3, Langchain LLMs, Llama-index, Whisper with chatbot, assistant, text completion, vision and image generation, internet access, chat with files, commands and code execution, file upload and download and more"
 authors = ["Marcin Szczyglinski <info@pygpt.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/szczyglis-dev/py-gpt"
 repository = "https://github.com/szczyglis-dev/py-gpt"
 documentation = "https://pygpt.readthedocs.io/"
```

### Comparing `pygpt_net-2.1.8/src/pygpt_net/CHANGELOG.txt` & `pygpt_net-2.1.9/src/pygpt_net/CHANGELOG.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+2.1.9 (2024-03-04)
+
+- A new option has been added to the "Web Search" plugin: "web_index_query", which allows for indexing a web and external content in a temporary index (in memory) and quickly querying its content. Works similar to "query_file" command.
+- The "read_file" command has been expanded to handle multiple files at once.
+- Added `Log and debug events` option to Developer settings.
+
 2.1.8 (2024-03-03)
 
 - A new option has been added to the "Files I/O" plugin: "query_file", which allows for indexing a file in a temporary index (in memory) and quickly querying its content. This enables the use of Llama-index for fast querying or adding context from individual files. From now on, you can ask questions about individual files without indexing them to the main vector store. See the "Querying single files" in "Modes -> Chat with files" section in a README for more info.
 - The "read_file" command has been expanded to return just the exact file content, without wrapping it in JSON.
 - Improved prompt for preparing queries in the Chat with files plugin.
 - Updated docs.
```

### Comparing `pygpt_net-2.1.8/src/pygpt_net/LICENSE` & `pygpt_net-2.1.9/src/pygpt_net/LICENSE`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.03.03 22:00:00                  #
+# Updated Date: 2024.03.04 20:00:00                  #
 # ================================================== #
 
 __author__ = "Marcin Szczygliński"
 __copyright__ = "Copyright 2024, Marcin Szczygliński"
 __credits__ = ["Marcin Szczygliński"]
 __license__ = "MIT"
-__version__ = "2.1.8"
-__build__ = "2024.03.03"
+__version__ = "2.1.9"
+__build__ = "2024.03.04"
 __maintainer__ = "Marcin Szczygliński"
 __github__ = "https://github.com/szczyglis-dev/py-gpt"
 __website__ = "https://pygpt.net"
 __pypi__ = "https://pypi.org/project/pygpt-net"
 __snap__ = "https://snapcraft.io/pygpt"
 __documentation__ = "https://pygpt.readthedocs.io"
 __email__ = "info@pygpt.net"
```

### Comparing `pygpt_net-2.1.8/src/pygpt_net/app.py` & `pygpt_net-2.1.9/src/pygpt_net/app.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/config.py` & `pygpt_net-2.1.9/src/pygpt_net/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.02.28 02:00:00                  #
+# Updated Date: 2024.03.04 22:00:00                  #
 # ================================================== #
 
 import copy
 import datetime
 import os
 import re
 from pathlib import Path
@@ -135,15 +135,14 @@
         if not self.initialized:
 
             # if app initialization
             if all:
                 v = self.get_version()
                 os = self.window.core.platforms.get_os()
                 architecture = self.window.core.platforms.get_architecture()
-                print("")
                 print("PyGPT v{} ({}, {})".format(v, os, architecture))
                 print("Author: Marcin Szczyglinski")
                 print("GitHub: https://github.com/szczyglis-dev/py-gpt")
                 print("WWW: https://pygpt.net")
                 print("Email: info@pygpt.net")
                 print("")
                 print("Initializing...")
```

### Comparing `pygpt_net-2.1.8/src/pygpt_net/container.py` & `pygpt_net-2.1.9/src/pygpt_net/container.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/agent/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/agent/flow.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/agent/flow.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/assistant/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/assistant/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/assistant/editor.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/assistant/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/assistant/files.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/assistant/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/assistant/threads.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/assistant/threads.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/attachment.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/attachment.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/audio.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/audio.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/calendar/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/calendar/note.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/calendar/note.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/camera.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/camera.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/chat/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/chat/common.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/chat/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/chat/files.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/chat/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/chat/image.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/chat/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/chat/input.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/chat/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/chat/output.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/chat/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/chat/render.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/chat/render.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/chat/text.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/chat/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         # get mode
         mode = self.window.core.config.get('mode')
         model = self.window.core.config.get('model')
         model_data = self.window.core.models.get(model)
 
         # create ctx item
         ctx = CtxItem()
+        ctx.meta_id = self.window.core.ctx.current
         ctx.internal = internal
         ctx.current = True  # mark as current context item
         ctx.mode = mode  # store current selected mode (not inline changed)
         ctx.model = model  # store model list key, not real model id
         ctx.set_input(text, user_name)
         ctx.set_output(None, ai_name)
```

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/chat/vision.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/chat/vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/command.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/command.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/config/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/config/field/checkbox.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/config/field/checkbox.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/config/field/combo.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/config/field/combo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/config/field/dictionary.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/config/field/dictionary.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/config/field/input.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/config/field/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/config/field/slider.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/config/field/slider.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/config/field/textarea.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/config/field/textarea.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/config/placeholder.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/config/placeholder.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/ctx/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/ctx/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/ctx/common.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/ctx/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/ctx/summarizer.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/ctx/summarizer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/debug.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/dialogs/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/dialogs/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/dialogs/confirm.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/dialogs/confirm.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/dialogs/debug.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/dialogs/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/dialogs/info.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/dialogs/info.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/files.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/idx/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/idx/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/idx/common.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/idx/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/idx/indexer.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/idx/indexer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/idx/settings.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/idx/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/lang/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/lang/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/lang/custom.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/lang/custom.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/lang/mapping.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/lang/mapping.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/lang/plugins.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/lang/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/lang/settings.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/lang/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/launcher.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/launcher.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/layout.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/layout.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/mode.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/model/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/model/editor.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/model/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/notepad.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/notepad.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/painter/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/painter/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/painter/capture.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/painter/capture.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/painter/common.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/painter/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/plugins/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/plugins/settings.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/plugins/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/presets/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/presets/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/presets/editor.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/presets/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/settings/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/settings/editor.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/settings/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/theme/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/theme/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/theme/common.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/theme/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/theme/markdown.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/theme/markdown.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/theme/menu.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/theme/menu.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/theme/nodes.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/theme/nodes.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/ui/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/ui/mode.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/ui/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/controller/ui/vision.py` & `pygpt_net-2.1.9/src/pygpt_net/controller/ui/vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/assistants/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/core/assistants/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/attachments.py` & `pygpt_net-2.1.9/src/pygpt_net/core/attachments.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/audio.py` & `pygpt_net-2.1.9/src/pygpt_net/core/audio.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/bridge.py` & `pygpt_net-2.1.9/src/pygpt_net/core/bridge.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/calendar/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/core/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/camera.py` & `pygpt_net-2.1.9/src/pygpt_net/core/camera.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/chain/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/core/chain/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/chain/chat.py` & `pygpt_net-2.1.9/src/pygpt_net/core/chain/chat.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/chain/completion.py` & `pygpt_net-2.1.9/src/pygpt_net/core/chain/completion.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/command.py` & `pygpt_net-2.1.9/src/pygpt_net/core/command.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/ctx/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/core/ctx/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/ctx/idx.py` & `pygpt_net-2.1.9/src/pygpt_net/core/ctx/idx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/db/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/core/db/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/debug/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/core/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/debug/agent.py` & `pygpt_net-2.1.9/src/pygpt_net/core/debug/agent.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/debug/assistants.py` & `pygpt_net-2.1.9/src/pygpt_net/core/debug/assistants.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/debug/attachments.py` & `pygpt_net-2.1.9/src/pygpt_net/core/debug/attachments.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/debug/config.py` & `pygpt_net-2.1.9/src/pygpt_net/core/debug/config.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/debug/indexes.py` & `pygpt_net-2.1.9/src/pygpt_net/core/debug/indexes.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/debug/models.py` & `pygpt_net-2.1.9/src/pygpt_net/core/debug/models.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/debug/plugins.py` & `pygpt_net-2.1.9/src/pygpt_net/core/debug/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/debug/presets.py` & `pygpt_net-2.1.9/src/pygpt_net/core/debug/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/debug/ui.py` & `pygpt_net-2.1.9/src/pygpt_net/core/debug/ui.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/dispatcher.py` & `pygpt_net-2.1.9/src/pygpt_net/core/dispatcher.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.03.03 22:00:00                  #
+# Updated Date: 2024.03.04 20:00:00                  #
 # ================================================== #
 
 import json
 
 from PySide6.QtWidgets import QApplication
 
 from pygpt_net.item.ctx import CtxItem
@@ -117,19 +117,33 @@
         Check if event can be logged
 
         :param event: event object
         :return: true if can be logged
         """
         if event.name in self.nolog_events:
             return False
+        if not self.is_log_display():
+            return False
         data = event.data
         if data is not None and "silent" in data and data["silent"]:
             return False
         return True
 
+    def is_log_display(self) -> bool:
+        """
+        Check if event can be logged
+
+        :return: true if can be logged
+        """
+        is_log = False
+        if self.window.core.config.has("log.events") \
+                and self.window.core.config.get("log.events"):
+            is_log = True
+        return is_log
+
     def async_allowed(self, ctx: CtxItem) -> bool:
         """
         Check if async execution are allowed
 
         :param ctx: context item
         :return: True if async commands are allowed
         """
@@ -197,32 +211,30 @@
         """
         Send reply from plugins to model
 
         :param ctx: context object
         """
         if ctx is not None:
             self.window.core.debug.info("Reply...")
-            if self.window.core.debug.enabled():
+            if self.window.core.debug.enabled() and self.is_log_display():
                 self.window.core.debug.debug("CTX REPLY: " + str(ctx))
 
             self.window.ui.status("")  # clear status
             if ctx.reply:
-
                 # if agent mode is enabled, add +1 run if sending reply
                 if ctx.internal:
                     if self.window.controller.agent.enabled():
                         self.window.controller.agent.add_run()
                         self.window.controller.agent.update()
                         QApplication.processEvents()
 
                 # prepare data to send
                 data = json.dumps(ctx.results)
-                if ctx.output is not None and ctx.output != "":
-                    data = ctx.output  # if output is set, use it as data (additional context, etc.)
-                    ctx.output = ""  # clear output before sending
+                if ctx.extra_ctx:
+                    data = ctx.extra_ctx  # if extra content is set, use it as data to send
 
                 self.window.core.ctx.update_item(ctx)  # update context in db
                 self.window.ui.status('...')
                 self.window.controller.chat.input.send(
                     data,
                     force=True,
                     reply=True,
```

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/filesystem.py` & `pygpt_net-2.1.9/src/pygpt_net/core/filesystem.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/history.py` & `pygpt_net-2.1.9/src/pygpt_net/core/history.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/idx/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/core/idx/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/idx/chat.py` & `pygpt_net-2.1.9/src/pygpt_net/core/idx/chat.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.03.03 22:00:00                  #
+# Updated Date: 2024.03.04 20:00:00                  #
 # ================================================== #
 
+import json
+
 from llama_index.core.llms import ChatMessage, MessageRole
 from llama_index.core.prompts import ChatPromptTemplate
 from llama_index.core.memory import ChatMemoryBuffer
 
 from pygpt_net.item.ctx import CtxItem
 from .context import Context
 from pygpt_net.item.model import ModelItem
@@ -214,14 +216,53 @@
             self.log("Querying temporary in-memory index: {}...".format(idx))
             response = index.as_query_engine(
                 streaming=False,
             ).query(query)  # query with default prompt
             if response:
                 return response.response
 
+    def query_web(self, type: str, url: str, args: dict, query: str) -> str:
+        """
+        Query web using temp index (created on the fly)
+
+        :param type: type of content
+        :param url: url to index
+        :param args: extra args
+        :param query: query
+        """
+        parts = {
+            "type": type,
+            "url": url,
+            "args": args,
+        }
+        id = json.dumps(parts)
+        model = self.window.core.models.from_defaults()
+        context = self.window.core.idx.llm.get_service_context(model=model)
+        index = self.storage.get_tmp(id, service_context=context)  # get or create tmp index
+
+        idx = "tmp:{}".format(id)  # tmp index id
+        self.log("Indexing to temporary in-memory index: {}...".format(idx))
+
+        # index file to tmp index
+        num, errors = self.window.core.idx.indexing.index_urls(
+            idx=id,
+            index=index,
+            urls=[url],
+            type=type,
+            extra_args=args,
+            is_tmp = True,
+        )
+        if num > 0:
+            self.log("Querying temporary in-memory index: {}...".format(idx))
+            response = index.as_query_engine(
+                streaming=False,
+            ).query(query)  # query with default prompt
+            if response:
+                return response.response
+
     def get_memory_buffer(self, history: list, llm = None) -> ChatMemoryBuffer:
         """
         Get memory buffer
 
         :param history: list with chat history (ChatMessage)
         :param llm: LLM model
         :return: memory buffer with chat history
```

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/idx/context.py` & `pygpt_net-2.1.9/src/pygpt_net/core/idx/context.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/idx/indexing.py` & `pygpt_net-2.1.9/src/pygpt_net/core/idx/indexing.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.03.03 22:00:00                  #
+# Updated Date: 2024.03.04 20:00:00                  #
 # ================================================== #
 
 import os.path
 
 from pathlib import Path
 from sqlalchemy import text
 
@@ -464,24 +464,26 @@
 
     def index_url(
             self,
             idx: str,
             index: BaseIndex,
             url: str,
             type="webpage",
-            extra_args: dict = None
+            extra_args: dict = None,
+            is_tmp: bool = False
     ) -> (int, list):
         """
         Index data from external (remote) resource
 
         :param idx: index name
         :param index: index instance
         :param url: external url to index
         :param type: type of URL (webpage, feed, etc.)
         :param extra_args: extra arguments for loader
+        :param is_tmp: True if temporary index
         :return: number of indexed documents, errors
         """
         errors = []
         n = 0
 
         # check if web loader for defined type exists
         if type not in self.loaders["web"]:
@@ -499,57 +501,61 @@
             if "url" not in extra_args:
                 extra_args["url"] = url
 
             # get unique external content identifier
             unique_id = self.data_providers[type].get_external_id(extra_args)
 
             # remove old document from index
-            self.remove_old_external(idx, unique_id, type)
+            if not is_tmp:
+                self.remove_old_external(idx, unique_id, type)
 
             self.log("Loading web documents from: {}".format(unique_id))
             self.log("Using web loader for type: {}".format(type))
 
             args = self.data_providers[type].prepare_args(**extra_args)
 
             # get documents from external resource
             documents = loader.load_data(
                 **args
             )
             for d in documents:
                 index.insert(document=d)
                 doc_id = d.id_  # URL is used as document ID
-                self.window.core.idx.external.set_indexed(
-                    content=unique_id,
-                    type=type,
-                    idx=idx,
-                    doc_id=doc_id,
-                )  # update external index
+                if not is_tmp:
+                    self.window.core.idx.external.set_indexed(
+                        content=unique_id,
+                        type=type,
+                        idx=idx,
+                        doc_id=doc_id,
+                    )  # update external index
                 self.log("Inserted (web) document: {} / {}".format(n+1, len(documents)))
                 n += 1
         except Exception as e:
             errors.append(str(e))
             self.window.core.debug.log(e)
         return n, errors
 
     def index_urls(
             self,
             idx: str,
             index: BaseIndex,
             urls: list,
             type="webpage",
-            extra_args: dict = None
+            extra_args: dict = None,
+            is_tmp: bool = False
     ) -> (int, list):
         """
         Index data from URLs
 
         :param idx: index name
         :param index: index instance
         :param urls: list of urls
         :param type: type of URL (webpage, feed, etc.)
         :param extra_args: extra arguments for loader
+        :param is_tmp: True if temporary index
         :return: number of indexed documents, errors
         """
         errors = []
         n = 0
 
         # check if web loader for defined type exists
         if type not in self.loaders["web"]:
@@ -561,14 +567,15 @@
         for url in urls:
             indexed, errs = self.index_url(
                 idx=idx,
                 index=index,
                 url=url,
                 type=type,
                 extra_args=extra_args,
+                is_tmp=is_tmp,
             )
             n += indexed
             errors.extend(errs)
         return n, errors
 
     def remove_old_meta_id(self, idx: str, id: int = 0) -> bool:
         """
```

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/idx/llm.py` & `pygpt_net-2.1.9/src/pygpt_net/core/idx/llm.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/idx/types/ctx.py` & `pygpt_net-2.1.9/src/pygpt_net/core/idx/types/ctx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/idx/types/external.py` & `pygpt_net-2.1.9/src/pygpt_net/core/idx/types/external.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/idx/types/files.py` & `pygpt_net-2.1.9/src/pygpt_net/core/idx/types/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/idx/worker.py` & `pygpt_net-2.1.9/src/pygpt_net/core/idx/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/image.py` & `pygpt_net-2.1.9/src/pygpt_net/core/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/info.py` & `pygpt_net-2.1.9/src/pygpt_net/core/info.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/installer.py` & `pygpt_net-2.1.9/src/pygpt_net/core/installer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/llm/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/core/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/locale.py` & `pygpt_net-2.1.9/src/pygpt_net/core/locale.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/models.py` & `pygpt_net-2.1.9/src/pygpt_net/core/models.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/modes.py` & `pygpt_net-2.1.9/src/pygpt_net/core/modes.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/notepad.py` & `pygpt_net-2.1.9/src/pygpt_net/core/notepad.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/platforms.py` & `pygpt_net-2.1.9/src/pygpt_net/core/platforms.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/plugins.py` & `pygpt_net-2.1.9/src/pygpt_net/core/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/presets.py` & `pygpt_net-2.1.9/src/pygpt_net/core/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/prompt.py` & `pygpt_net-2.1.9/src/pygpt_net/core/prompt.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/render/base.py` & `pygpt_net-2.1.9/src/pygpt_net/core/render/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/render/markdown/parser.py` & `pygpt_net-2.1.9/src/pygpt_net/core/render/markdown/parser.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/render/markdown/renderer.py` & `pygpt_net-2.1.9/src/pygpt_net/core/render/markdown/renderer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/render/plain/renderer.py` & `pygpt_net-2.1.9/src/pygpt_net/core/render/plain/renderer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/settings.py` & `pygpt_net-2.1.9/src/pygpt_net/core/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/tokens.py` & `pygpt_net-2.1.9/src/pygpt_net/core/tokens.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/updater/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/core/updater/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/web.py` & `pygpt_net-2.1.9/src/pygpt_net/core/web.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/core/worker.py` & `pygpt_net-2.1.9/src/pygpt_net/core/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/config/config.json` & `pygpt_net-2.1.9/src/pygpt_net/data/config/config.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9894957983193278%*

 * *Differences: {"'__meta__'": "{'version': '2.1.9', 'app.version': '2.1.9', 'updated_at': '2024-03-04T00:00:00'}",*

 * * "'log.events'": 'False'}*

```diff
@@ -1,12 +1,12 @@
 {
     "__meta__": {
-        "app.version": "2.1.8",
-        "updated_at": "2024-03-03T00:00:00",
-        "version": "2.1.8"
+        "app.version": "2.1.9",
+        "updated_at": "2024-03-04T00:00:00",
+        "version": "2.1.9"
     },
     "agent.auto_stop": true,
     "agent.goal.notify": true,
     "agent.idx": "base",
     "agent.iterations": 3,
     "agent.mode": "chat",
     "ai_name": "",
@@ -96,14 +96,15 @@
     "llama.idx.status": {},
     "llama.idx.storage": "SimpleVectorStore",
     "llama.idx.storage.args": [],
     "llama.log": false,
     "lock_modes": true,
     "log.assistants": false,
     "log.dalle": false,
+    "log.events": false,
     "log.level": "error",
     "log.llama": false,
     "log.plugins": false,
     "max_output_tokens": 1024,
     "max_tokens_length": 32000,
     "max_total_tokens": 128000,
     "mode": "chat",
```

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/config/models.json` & `pygpt_net-2.1.9/src/pygpt_net/data/config/models.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'__meta__'": "{'version': '2.1.9', 'app.version': '2.1.9', 'updated_at': '2024-03-04T00:00:00'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "__meta__": {
-        "app.version": "2.1.8",
-        "updated_at": "2024-03-03T00:00:00",
-        "version": "2.1.8"
+        "app.version": "2.1.9",
+        "updated_at": "2024-03-04T00:00:00",
+        "version": "2.1.9"
     },
     "items": {
         "dall-e-2": {
             "ctx": 0,
             "default": false,
             "id": "dall-e-2",
             "langchain": {
```

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/config/modes.json` & `pygpt_net-2.1.9/src/pygpt_net/data/config/modes.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'__meta__'": "{'version': '2.1.9', 'app.version': '2.1.9', 'updated_at': '2024-03-04T00:00:00'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "__meta__": {
-        "app.version": "2.1.8",
-        "updated_at": "2024-03-03T00:00:00",
-        "version": "2.1.8"
+        "app.version": "2.1.9",
+        "updated_at": "2024-03-04T00:00:00",
+        "version": "2.1.9"
     },
     "items": {
         "agent": {
             "default": false,
             "id": "agent",
             "label": "mode.agent",
             "name": "Agent (autonomous)"
```

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/config/presets/current.agent.json` & `pygpt_net-2.1.9/src/pygpt_net/data/config/presets/current.agent.json`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/config/settings.json` & `pygpt_net-2.1.9/src/pygpt_net/data/config/settings.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9852941176470589%*

 * *Differences: {"'log.events'": "OrderedDict([('section', 'developer'), ('type', 'bool'), ('slider', False), "*

 * *                 "('label', 'Log and debug events'), ('value', False), ('min', None), ('max', "*

 * *                 "None), ('multiplier', None), ('step', None), ('advanced', False)])"}*

```diff
@@ -615,14 +615,26 @@
         "multiplier": null,
         "section": "developer",
         "slider": false,
         "step": null,
         "type": "bool",
         "value": false
     },
+    "log.events": {
+        "advanced": false,
+        "label": "Log and debug events",
+        "max": null,
+        "min": null,
+        "multiplier": null,
+        "section": "developer",
+        "slider": false,
+        "step": null,
+        "type": "bool",
+        "value": false
+    },
     "log.level": {
         "advanced": false,
         "description": "Tip: Running application with --debug=1 or --debug=2 command line arguments overwrites this settings and force enables logging to %workdir%/app.log file. Log levels: 1 = INFO, 2 = DEBUG",
         "keys": [
             {
                 "error": "ERROR (default)"
             },
```

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/config/settings_section.json` & `pygpt_net-2.1.9/src/pygpt_net/data/config/settings_section.json`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/css/fix_windows.css` & `pygpt_net-2.1.9/src/pygpt_net/data/css/fix_windows.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/css/markdown.dark.css` & `pygpt_net-2.1.9/src/pygpt_net/data/css/markdown.dark.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/css/style.dark.css` & `pygpt_net-2.1.9/src/pygpt_net/data/css/style.dark.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/css/style.light.css` & `pygpt_net-2.1.9/src/pygpt_net/data/css/style.light.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/fonts/Lato/Lato-Black.ttf` & `pygpt_net-2.1.9/src/pygpt_net/data/fonts/Lato/Lato-Black.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/fonts/Lato/Lato-BlackItalic.ttf` & `pygpt_net-2.1.9/src/pygpt_net/data/fonts/Lato/Lato-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/fonts/Lato/Lato-Bold.ttf` & `pygpt_net-2.1.9/src/pygpt_net/data/fonts/Lato/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/fonts/Lato/Lato-BoldItalic.ttf` & `pygpt_net-2.1.9/src/pygpt_net/data/fonts/Lato/Lato-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/fonts/Lato/Lato-Italic.ttf` & `pygpt_net-2.1.9/src/pygpt_net/data/fonts/Lato/Lato-Italic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/fonts/Lato/Lato-Light.ttf` & `pygpt_net-2.1.9/src/pygpt_net/data/fonts/Lato/Lato-Light.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/fonts/Lato/Lato-LightItalic.ttf` & `pygpt_net-2.1.9/src/pygpt_net/data/fonts/Lato/Lato-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/fonts/Lato/Lato-Regular.ttf` & `pygpt_net-2.1.9/src/pygpt_net/data/fonts/Lato/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/fonts/Lato/Lato-Thin.ttf` & `pygpt_net-2.1.9/src/pygpt_net/data/fonts/Lato/Lato-Thin.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/fonts/Lato/Lato-ThinItalic.ttf` & `pygpt_net-2.1.9/src/pygpt_net/data/fonts/Lato/Lato-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/fonts/Lato/OFL.txt` & `pygpt_net-2.1.9/src/pygpt_net/data/fonts/Lato/OFL.txt`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/icon.ico` & `pygpt_net-2.1.9/src/pygpt_net/data/icon.ico`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/icon.png` & `pygpt_net-2.1.9/src/pygpt_net/data/icon.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/icon_tray_busy.ico` & `pygpt_net-2.1.9/src/pygpt_net/data/icon_tray_busy.ico`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/icon_tray_error.ico` & `pygpt_net-2.1.9/src/pygpt_net/data/icon_tray_error.ico`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/icon_tray_idle.ico` & `pygpt_net-2.1.9/src/pygpt_net/data/icon_tray_idle.ico`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/icons/abc.svg` & `pygpt_net-2.1.9/src/pygpt_net/data/icons/abc.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/icons/alarm.svg` & `pygpt_net-2.1.9/src/pygpt_net/data/icons/alarm.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/icons/apps.svg` & `pygpt_net-2.1.9/src/pygpt_net/data/icons/apps.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/icons/build.svg` & `pygpt_net-2.1.9/src/pygpt_net/data/icons/build.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/icons/calendar.svg` & `pygpt_net-2.1.9/src/pygpt_net/data/icons/calendar.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/icons/cut.svg` & `pygpt_net-2.1.9/src/pygpt_net/data/icons/cut.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/icons/db.svg` & `pygpt_net-2.1.9/src/pygpt_net/data/icons/db.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/icons/error.svg` & `pygpt_net-2.1.9/src/pygpt_net/data/icons/error.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/icons/hearing.svg` & `pygpt_net-2.1.9/src/pygpt_net/data/icons/hearing.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/icons/help.svg` & `pygpt_net-2.1.9/src/pygpt_net/data/icons/help.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/icons/info.svg` & `pygpt_net-2.1.9/src/pygpt_net/data/icons/info.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/icons/key.svg` & `pygpt_net-2.1.9/src/pygpt_net/data/icons/key.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/icons/keyboard.svg` & `pygpt_net-2.1.9/src/pygpt_net/data/icons/keyboard.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/icons/language.svg` & `pygpt_net-2.1.9/src/pygpt_net/data/icons/language.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/icons/palette.svg` & `pygpt_net-2.1.9/src/pygpt_net/data/icons/palette.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/icons/public_filled.svg` & `pygpt_net-2.1.9/src/pygpt_net/data/icons/public_filled.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/icons/robot.svg` & `pygpt_net-2.1.9/src/pygpt_net/data/icons/robot.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/icons/router.svg` & `pygpt_net-2.1.9/src/pygpt_net/data/icons/router.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/icons/sensors.svg` & `pygpt_net-2.1.9/src/pygpt_net/data/icons/sensors.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/icons/settings.svg` & `pygpt_net-2.1.9/src/pygpt_net/data/icons/settings.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/icons/share.svg` & `pygpt_net-2.1.9/src/pygpt_net/data/icons/share.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/icons/view.svg` & `pygpt_net-2.1.9/src/pygpt_net/data/icons/view.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/icons/voice.svg` & `pygpt_net-2.1.9/src/pygpt_net/data/icons/voice.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/locale.de.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/locale.de.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/locale.en.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/locale.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/locale.es.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/locale.es.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/locale.fr.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/locale.fr.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/locale.it.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/locale.it.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/locale.pl.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/locale.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/locale.ua.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/locale.ua.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.agent.en.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.agent.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.agent.pl.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.agent.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.audio_input.en.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.audio_input.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.audio_input.pl.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.audio_input.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.audio_output.en.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.audio_output.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.audio_output.pl.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.audio_output.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.cmd_api.en.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.cmd_api.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.cmd_api.pl.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.cmd_api.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.en.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.pl.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.cmd_custom.pl.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.cmd_custom.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.cmd_files.en.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.cmd_files.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.cmd_files.pl.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.cmd_files.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.cmd_history.en.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.cmd_history.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.cmd_history.pl.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.cmd_history.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.cmd_serial.en.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.cmd_serial.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.cmd_serial.pl.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.cmd_serial.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.cmd_web.en.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.cmd_web.en.ini`

 * *Files 8% similar despite different names*

```diff
@@ -63,23 +63,27 @@
 cmd_web_url_raw.tooltip = If enabled, model will be able to open specified URL and get raw content
 
 cmd_web_urls.label = Enable: "web_urls" command
 cmd_web_urls.description = If enabled, model will be able to search the Web and get founded URLs list
 cmd_web_urls.tooltip = If enabled, model will be able to search the Web and get founded URLs list
 
 cmd_web_index.label = Enable: "web_index" command
-cmd_web_index.description = If enabled, model will be able to index pages and external content using Llama-index
-cmd_web_index.tooltip = If enabled, model will be able to index pages and external content using Llama-index
+cmd_web_index.description = If enabled, model will be able to index pages and external content using Llama-index (persistent index)
+cmd_web_index.tooltip = If enabled, model will be able to index pages and external content using Llama-index (persistent index)
+
+cmd_web_index_query.label = Enable: "web_index_query" command - quick query the web content with Llama-index
+cmd_web_index_query.description = If enabled, model will be able to index and query web content using Llama-index (temporary index, on the fly)
+cmd_web_index_query.tooltip = If enabled, model will be able to index and query web content using Llama-index (temporary index, on the fly)
 
 auto_index.label = Auto-index all used URLs using Llama-index
-auto_index.description = If enabled, every URL used by the model will be automatically indexed using Llama-index
-auto_index.tooltip = If enabled, every URL used by the model will be automatically indexed using Llama-index
+auto_index.description = If enabled, every URL used by the model will be automatically indexed using Llama-index (persistent index)
+auto_index.tooltip = If enabled, every URL used by the model will be automatically indexed using Llama-index (persistent index)
 
 idx.label = Index to use
-idx.description = ID of index to use for web page indexing
+idx.description = ID of index to use for web page indexing (persistent index)
 idx.tooltip = Index name
 
 summary_model.label = Model used for web page summarize
 summary_model.description = Model used for web page summarize, default: gpt-3.5-turbo-1106
 summary_model.tooltip = Model used for web page summarize, default: gpt-3.5-turbo-1106
 
 prompt_summarize.label = Summarize prompt
@@ -108,8 +112,12 @@
 
 syntax_web_urls.label = Syntax: web_urls
 syntax_web_urls.description = Syntax for web_urls command
 syntax_web_urls.tooltip = Syntax for web_urls command
 
 syntax_web_index.label = Syntax: web_index
 syntax_web_index.description = Syntax for web_index command
-syntax_web_index.tooltip = Syntax for web_index command
+syntax_web_index.tooltip = Syntax for web_index command
+
+syntax_web_index_query.label = Syntax: web_index_query
+syntax_web_index_query.description = Syntax for web_index_query command
+syntax_web_index_query.tooltip = Syntax for web_index_query command
```

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.cmd_web.pl.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.cmd_web.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.crontab.en.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.crontab.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.crontab.pl.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.crontab.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.idx_llama_index.en.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.idx_llama_index.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.idx_llama_index.pl.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.idx_llama_index.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.openai_dalle.en.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.openai_dalle.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.openai_dalle.pl.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.openai_dalle.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.openai_vision.en.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.openai_vision.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.openai_vision.pl.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.openai_vision.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.real_time.en.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.real_time.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/locale/plugin.real_time.pl.ini` & `pygpt_net-2.1.9/src/pygpt_net/data/locale/plugin.real_time.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/logo.png` & `pygpt_net-2.1.9/src/pygpt_net/data/logo.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/win32/README.rtf` & `pygpt_net-2.1.9/src/pygpt_net/data/win32/README.rtf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/win32/USER-LICENSE.rtf` & `pygpt_net-2.1.9/src/pygpt_net/data/win32/USER-LICENSE.rtf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/data/win32/pygpt.aip` & `pygpt_net-2.1.9/src/pygpt_net/data/win32/pygpt.aip`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/icons.qrc` & `pygpt_net-2.1.9/src/pygpt_net/icons.qrc`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/icons_rc.py` & `pygpt_net-2.1.9/src/pygpt_net/icons_rc.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/item/assistant.py` & `pygpt_net-2.1.9/src/pygpt_net/item/assistant.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/item/attachment.py` & `pygpt_net-2.1.9/src/pygpt_net/item/attachment.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/item/calendar_note.py` & `pygpt_net-2.1.9/src/pygpt_net/item/calendar_note.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/item/ctx.py` & `pygpt_net-2.1.9/src/pygpt_net/item/ctx.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.03.03 22:00:00                  #
+# Updated Date: 2024.03.04 20:00:00                  #
 # ================================================== #
 
 import datetime
 import json
 import time
 
 
@@ -43,14 +43,15 @@
         self.output_name = None
         self.input_timestamp = None
         self.output_timestamp = None
         self.input_tokens = 0
         self.output_tokens = 0
         self.total_tokens = 0
         self.extra = None
+        self.extra_ctx = None
         self.current = False
         self.internal = False
         self.is_vision = False
         self.idx = 0
         self.first = False
         self.tool_calls = []  # API tool calls
         self.index_meta = {}  # llama-index metadata ctx used
@@ -127,14 +128,15 @@
             "output_name": self.output_name,
             "input_timestamp": self.input_timestamp,
             "output_timestamp": self.output_timestamp,
             "input_tokens": self.input_tokens,
             "output_tokens": self.output_tokens,
             "total_tokens": self.total_tokens,
             "extra": self.extra,
+            "extra_ctx": self.extra_ctx,
             "current": self.current,
             "internal": self.internal,
             "is_vision": self.is_vision,
             "idx": self.idx,
             "first": self.first,
             "tool_calls": self.tool_calls,
             "index_meta": self.index_meta,
@@ -169,14 +171,15 @@
         self.output_name = data.get("output_name", None)
         self.input_timestamp = data.get("input_timestamp", None)
         self.output_timestamp = data.get("output_timestamp", None)
         self.input_tokens = data.get("input_tokens", 0)
         self.output_tokens = data.get("output_tokens", 0)
         self.total_tokens = data.get("total_tokens", 0)
         self.extra = data.get("extra", None)
+        self.extra_ctx = data.get("extra_ctx", False)
         self.current = data.get("current", False)
         self.internal = data.get("internal", False)
         self.is_vision = data.get("is_vision", False)
         self.idx = data.get("idx", 0)
         self.first = data.get("first", False)
         self.tool_calls = data.get("tool_calls", [])
         self.index_meta = data.get("index_meta", {})
```

### Comparing `pygpt_net-2.1.8/src/pygpt_net/item/index.py` & `pygpt_net-2.1.9/src/pygpt_net/item/index.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/item/mode.py` & `pygpt_net-2.1.9/src/pygpt_net/item/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/item/model.py` & `pygpt_net-2.1.9/src/pygpt_net/item/model.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/item/notepad.py` & `pygpt_net-2.1.9/src/pygpt_net/item/notepad.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/item/preset.py` & `pygpt_net-2.1.9/src/pygpt_net/item/preset.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/launcher.py` & `pygpt_net-2.1.9/src/pygpt_net/launcher.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/migrations/Version20231227152900.py` & `pygpt_net-2.1.9/src/pygpt_net/migrations/Version20231227152900.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/migrations/Version20231230095000.py` & `pygpt_net-2.1.9/src/pygpt_net/migrations/Version20231230095000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/migrations/Version20231231230000.py` & `pygpt_net-2.1.9/src/pygpt_net/migrations/Version20231231230000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/migrations/Version20240106060000.py` & `pygpt_net-2.1.9/src/pygpt_net/migrations/Version20240106060000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/migrations/Version20240107060000.py` & `pygpt_net-2.1.9/src/pygpt_net/migrations/Version20240107060000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/migrations/Version20240222160000.py` & `pygpt_net-2.1.9/src/pygpt_net/migrations/Version20240222160000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/migrations/Version20240223050000.py` & `pygpt_net-2.1.9/src/pygpt_net/migrations/Version20240223050000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/migrations/Version20240303190000.py` & `pygpt_net-2.1.9/src/pygpt_net/migrations/Version20240303190000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/migrations/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/migrations/base.py` & `pygpt_net-2.1.9/src/pygpt_net/migrations/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/plugin/agent/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/plugin/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/plugin/audio_input/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/plugin/audio_input/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/plugin/audio_input/simple.py` & `pygpt_net-2.1.9/src/pygpt_net/plugin/audio_input/simple.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/plugin/audio_input/worker.py` & `pygpt_net-2.1.9/src/pygpt_net/plugin/audio_input/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/plugin/audio_output/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/plugin/audio_output/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/plugin/audio_output/worker.py` & `pygpt_net-2.1.9/src/pygpt_net/plugin/audio_output/worker.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,19 +2,17 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.01.30 13:00:00                  #
+# Updated Date: 2024.03.04 22:00:00                  #
 # ================================================== #
 
-import pygame
-
 from PySide6.QtCore import Slot, Signal
 from pygpt_net.plugin.base import BaseWorker, BaseSignals
 
 
 class WorkerSignals(BaseSignals):
     playback = Signal(object)
     stop = Signal()
@@ -27,19 +25,20 @@
         self.args = args
         self.kwargs = kwargs
         self.plugin = None
         self.text = None
 
     @Slot()
     def run(self):
+        from pygame import mixer
         try:
             path = self.plugin.get_provider().speech(self.text)
             if path:
-                pygame.mixer.init()
-                playback = pygame.mixer.Sound(path)
+                mixer.init()
+                playback = mixer.Sound(path)
                 self.stop_playback()  # stop previous playback
                 playback.play()
                 self.send(playback)  # send playback object to main thread
         except Exception as e:
             self.error(e)
 
     def send(self, playback):
```

### Comparing `pygpt_net-2.1.8/src/pygpt_net/plugin/base.py` & `pygpt_net-2.1.9/src/pygpt_net/plugin/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.03.03 22:00:00                  #
+# Updated Date: 2024.03.04 20:00:00                  #
 # ================================================== #
 
 from PySide6.QtCore import QObject, Signal, QRunnable, Slot
 
 from pygpt_net.core.dispatcher import Event
 from pygpt_net.item.ctx import CtxItem
 from pygpt_net.utils import trans
@@ -205,15 +205,16 @@
                     self.window.controller.files.update_explorer()
 
         # dispatch late response (reply)
         if ctx is not None:
             ctx.results.append(response)
             ctx.reply = True
             if "context" in response:
-                ctx.output = response["context"]
+                ctx.extra_ctx = response["context"]
+                response["result"] = "OK"
             self.window.core.dispatcher.reply(ctx)
 
     @Slot(object)
     def handle_status(self, data: str):
         """
         Handle thread status msg signal
```

### Comparing `pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_api/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_api/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_api/worker.py` & `pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_api/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_code_interpreter/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_code_interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_code_interpreter/runner.py` & `pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_code_interpreter/runner.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_code_interpreter/worker.py` & `pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_code_interpreter/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_custom/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_custom/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_custom/worker.py` & `pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_custom/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_files/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_files/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.03.03 22:00:00                  #
+# Updated Date: 2024.03.04 20:00:00                  #
 # ================================================== #
 
 from pygpt_net.plugin.base import BasePlugin
 from pygpt_net.core.dispatcher import Event
 from pygpt_net.item.ctx import CtxItem
 
 from .worker import Worker
@@ -230,15 +230,15 @@
             label="Syntax: send_file",
             description="Syntax for send files as attachment",
             advanced=True,
         )
         self.add_option(
             "syntax_read_file",
             type="textarea",
-            value='"read_file": read data from file, params: "filename"',
+            value='"read_file": read data from file, if multiple files then pass list of files, params: "filename"',
             label="Syntax: read_file",
             description="Syntax for reading files",
             advanced=True,
         )
         self.add_option(
             "syntax_query_file",
             type="textarea",
```

### Comparing `pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_files/worker.py` & `pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_files/worker.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.03.03 22:00:00                  #
+# Updated Date: 2024.03.04 20:00:00                  #
 # ================================================== #
 
 import mimetypes
 import os.path
 import shutil
 import ssl
 from urllib.request import Request, urlopen
@@ -161,15 +161,14 @@
         :param item: item with parameters
         """
         request = self.prepare_request(item)
         try:
             self.msg = "Saving file: {}".format(item["params"]['filename'])
             self.log(self.msg)
             path = self.prepare_path(item["params"]['filename'])
-
             data = item["params"]['data']
             with open(path, 'w', encoding="utf-8") as file:
                 file.write(data)
                 response = {
                     "request": request,
                     "result": "OK",
                 }
@@ -217,58 +216,30 @@
 
         :param item: item with parameters
         """
         request = self.prepare_request(item)
         try:
             self.msg = "Reading file: {}".format(item["params"]['filename'])
             self.log(self.msg)
-            path = self.prepare_path(item["params"]['filename'])
-            # check if file exists
-            if os.path.exists(path):
-                # auto-index file using Llama-index
-                if self.plugin.get_option_value("auto_index") \
-                        or self.plugin.get_option_value("only_index"):
-                    idx_name = self.plugin.get_option_value("idx")
-                    files, errors = self.plugin.window.core.idx.index_files(
-                        idx_name,
-                        path,
-                    )
-                    # if only index, return response and continue
-                    if self.plugin.get_option_value("only_index"):
-                        data = {
-                            'num_indexed': len(files),
-                            'index_name': idx_name,
-                            'errors': errors,
-                            'path': path,
-                        }
-                        response = {
-                            "request": request,
-                            "result": data,
-                        }
-                        self.log("File read (index only): {}".format(path))
-                        self.response(response, self.get_extra_data())
-                        return
-
-                # read file as text
-                data = self.plugin.read_as_text(
-                    path,
-                    use_loaders=self.plugin.get_option_value("use_loaders"),
-                )
-                response = {
-                    "request": request,
-                    "result": data,
-                    "context": os.path.basename(path) + ":\n--------------------------------\n" + data,  # add additional context
-                }
-                self.log("File read: {}".format(path))
-            else:
-                response = {
-                    "request": request,
-                    "result": "File not found",
-                }
-                self.log("File not found: {}".format(path))
+            path = item["params"]['filename']
+            paths = []
+            if isinstance(path, list):
+                paths = path
+            elif isinstance(path, str):
+                paths = [path]
+            data, context = self.read_files(paths)
+            context_str = None
+            if context:
+                context_str = "\n\n".join(context)
+            response = {
+                "request": request,
+                "result": data,
+            }
+            if context_str:
+                response["context"] = context_str
         except Exception as e:
             response = {
                 "request": request,
                 "result": "Error: {}".format(e),
             }
             self.error(e)
             self.log("Error: {}".format(e))
@@ -291,27 +262,26 @@
                 query = item["params"]["query"]
 
             # check if file exists
             if os.path.exists(path):
                 if query is not None:
                     # query file using temp index (created on the fly)
                     self.log("Querying file: {}".format(path))
-                    response = self.plugin.window.core.idx.chat.query_file(path, query)
-                    self.log("Response from temporary in-memory index: {}".format(response))
-                    if response:
+                    answer = self.plugin.window.core.idx.chat.query_file(path, query)
+                    self.log("Response from temporary in-memory index: {}".format(answer))
+                    if answer:
                         response = {
                             "request": request,
-                            "result": response,
-                            "context": "From: " + os.path.basename(path) + ":\n--------------------------------\n" + response,
+                            "result": answer,
+                            "context": "From: " + os.path.basename(path) + ":\n--------------------------------\n" + answer,
                             # add additional context
                         }
 
-                # auto-index file to standard index using Llama-index
-                if self.plugin.get_option_value("auto_index") \
-                        or self.plugin.get_option_value("only_index"):
+                # + auto-index file to main index using Llama-index
+                if self.plugin.get_option_value("auto_index"):
                     idx_name = self.plugin.get_option_value("idx")
                     self.plugin.window.core.idx.index_files(
                         idx_name,
                         path,
                     )
             else:
                 response = {
@@ -913,7 +883,51 @@
         if self.is_absolute_path(path):
             return path
         else:
             return os.path.join(
                 self.plugin.window.core.config.get_user_dir('data'),
                 path,
             )
+
+    def read_files(self, paths: list) -> (dict, str):
+        """
+        Read files from directory
+
+        :param paths: list of paths
+        :return: response data and context
+        """
+        data = []
+        context = []
+        for path in paths:
+            path = self.prepare_path(path)
+            if os.path.exists(path):
+                # + auto-index file using Llama-index
+                if self.plugin.get_option_value("auto_index") \
+                        or self.plugin.get_option_value("only_index"):
+                    idx_name = self.plugin.get_option_value("idx")
+                    files, errors = self.plugin.window.core.idx.index_files(
+                        idx_name,
+                        path,
+                    )
+                    # if only index, return response and continue
+                    if self.plugin.get_option_value("only_index"):
+                        data.append({
+                            'num_indexed': len(files),
+                            'index_name': idx_name,
+                            'errors': errors,
+                            'path': path,
+                        })
+                        self.log("File read (index only): {}".format(path))
+                        return data, context
+
+                # read file as text
+                content = self.plugin.read_as_text(
+                    path,
+                    use_loaders=self.plugin.get_option_value("use_loaders"),
+                )
+                context.append(os.path.basename(path) + ":\n--------------------------------\n" + content)
+                self.log("File read: {}".format(path))
+            else:
+                self.log("File not found: {}".format(path))
+                data.append("File not found: {}".format(path))
+
+        return data, context
```

### Comparing `pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_history/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_history/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_serial/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_serial/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_serial/worker.py` & `pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_serial/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_web/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_web/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.03.01 17:00:00                  #
+# Updated Date: 2024.03.04 20:00:00                  #
 # ================================================== #
 
 import ssl
 from urllib.request import Request, urlopen
 
 from pygpt_net.plugin.base import BasePlugin
 from pygpt_net.provider.web.base import BaseProvider
@@ -31,14 +31,15 @@
         self.input_text = None
         self.allowed_cmds = [
             "web_search",
             "web_urls",
             "web_url_open",
             "web_url_raw",
             "web_index",
+            "web_index_query",
         ]
         self.order = 100
         self.use_locale = True
         self.websearch = WebSearch(self)
 
     def init_options(self):
         """Initialize options"""
@@ -153,33 +154,42 @@
             tooltip="If enabled, model will be able to search the Web and get founded URLs list",
         )
         self.add_option(
             "cmd_web_index",
             type="bool",
             value=True,
             label="Enable: \"web_index\" command",
-            description="If enabled, model will be able to index web pages using Llama-index",
-            tooltip="If enabled, model will be able to index web pages using Llama-index",
+            description="If enabled, model will be able to index web content using Llama-index (persistent index)",
+            tooltip="If enabled, model will be able to index web pages using Llama-index (persistent index)",
+            tab="indexing",
+        )
+        self.add_option(
+            "cmd_web_index_query",
+            type="bool",
+            value=True,
+            label="Enable: \"web_index_query\" command - quick query the web content with Llama-index",
+            description="If enabled, model will be able to index and query web content using Llama-index (temporary index, on the fly)",
+            tooltip="If enabled, model will be able to index and query web content using Llama-index (temporary index, on the fly)",
             tab="indexing",
         )
         self.add_option(
             "auto_index",
             type="bool",
             value=False,
             label="Auto-index all used URLs using Llama-index",
-            description="If enabled, every URL used by the model will be automatically indexed using Llama-index",
-            tooltip="If enabled, every URL used by the model will be automatically indexed using Llama-index",
+            description="If enabled, every URL used by the model will be automatically indexed using Llama-index (persistent index)",
+            tooltip="If enabled, every URL used by the model will be automatically indexed using Llama-index (persistent index)",
             tab="indexing",
         )
         self.add_option(
             "idx",
             type="text",
             value="base",
             label="Index to use",
-            description="ID of index to use for web page indexing",
+            description="ID of index to use for web page indexing (persistent index)",
             tooltip="Index name",
             tab="indexing",
         )
         self.add_option(
             "summary_model",
             type="text",
             value="gpt-3.5-turbo-1106",
@@ -247,14 +257,22 @@
                   'a list of found links to websites will be returned, 10 links per page max. You can change the page '
                   'or the number of links per page using the provided parameters, params: "query", "page", '
                   '"num_links"',
             label="Syntax: web_urls",
             description="Syntax for web_urls command",
             advanced=True,
         )
+        self.add_option(
+            "syntax_web_index_query",
+            type="textarea",
+            value='"web_index_query": read, index and query web content for additional context data, params: (same as for web_index)',
+            label="Syntax: web_index_query",
+            description="Syntax for querying web for additional context data",
+            advanced=True,
+        )
         """
         # handled by code
         self.add_option(
             "syntax_web_index",
             type="textarea",
             value='"web_index": use it to index (embed in Vector Store) provided webpage URL for future use, '
                   'params: "url"',
```

### Comparing `pygpt_net-2.1.8/src/pygpt_net/plugin/cmd_web/websearch.py` & `pygpt_net-2.1.9/src/pygpt_net/plugin/cmd_web/websearch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/plugin/crontab/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/plugin/crontab/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/plugin/extra_prompt/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/plugin/extra_prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/plugin/idx_llama_index/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/plugin/idx_llama_index/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/plugin/openai_dalle/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/plugin/openai_dalle/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/plugin/openai_vision/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/plugin/openai_vision/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/plugin/real_time/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/plugin/real_time/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/audio_input/base.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/audio_input/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/audio_input/bing_speech_recognition.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/audio_input/bing_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/audio_input/google_cloud_speech_recognition.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/audio_input/google_cloud_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/audio_input/google_speech_recognition.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/audio_input/google_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/audio_input/openai_whisper.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/audio_input/openai_whisper.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/audio_input/openai_whisper_local.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/audio_input/openai_whisper_local.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/audio_output/base.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/audio_output/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/audio_output/eleven_labs.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/audio_output/eleven_labs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/audio_output/google_tts.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/audio_output/google_tts.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/audio_output/ms_azure_tts.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/audio_output/ms_azure_tts.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/audio_output/openai_tts.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/audio_output/openai_tts.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/assistant/base.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/assistant/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/assistant/json_file.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/assistant/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/attachment/base.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/attachment/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/attachment/json_file.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/attachment/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/calendar/base.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/calendar/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/calendar/db_sqlite/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/calendar/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/calendar/db_sqlite/patch.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/calendar/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/calendar/db_sqlite/storage.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/calendar/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/config/base.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/config/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/config/json_file.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/config/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/config/patch.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/config/patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.03.03 22:00:00                  #
+# Updated Date: 2024.03.04 20:00:00                  #
 # ================================================== #
 
 import os
 
 from packaging.version import parse as parse_version, Version
 
 
@@ -1014,14 +1014,23 @@
             # < 2.1.8 - syntax
             if old < parse_version("2.1.8"):
                 print("Migrating config from < 2.1.8...")
                 if 'idx_llama_index' in data["plugins"] and 'syntax_prepare_question' in data["plugins"]["idx_llama_index"]:
                     syntax = 'Simplify the question into a short query for retrieving information from a vector store.'
                     data["plugins"]["idx_llama_index"]["syntax_prepare_question"] = syntax
 
+            # < 2.1.9 - syntax
+            if old < parse_version("2.1.9"):
+                print("Migrating config from < 2.1.9...")
+                if 'cmd_files' in data["plugins"] and 'syntax_read_file' in data["plugins"]["cmd_files"]:
+                    syntax = '"read_file": read data from file, if multiple files then pass list of files, params: "filename"'
+                    data["plugins"]["cmd_files"]["syntax_read_file"] = syntax
+                if 'log.events' not in data:
+                    data["log.events"] = False
+
         # update file
         migrated = False
         if updated:
             data = dict(sorted(data.items()))
             self.window.core.config.data = data
             self.window.core.config.save()
             migrated = True
```

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/ctx/base.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/ctx/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/ctx/db_sqlite/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/ctx/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/ctx/db_sqlite/patch.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/ctx/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/ctx/db_sqlite/storage.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/ctx/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/ctx/db_sqlite/utils.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/ctx/db_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/ctx/json_file.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/ctx/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/history/base.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/history/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/history/patch.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/history/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/history/txt_file.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/history/txt_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/index/base.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/index/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/index/db_sqlite/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/index/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/index/db_sqlite/patch.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/index/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/index/db_sqlite/storage.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/index/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/index/db_sqlite/utils.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/index/db_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/index/json_file.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/index/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/index/patch.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/index/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/mode/base.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/mode/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/mode/json_file.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/mode/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/mode/patch.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/mode/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/model/base.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/model/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/model/json_file.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/model/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/model/patch.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/model/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/notepad/base.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/notepad/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/notepad/db_sqlite/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/notepad/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/notepad/db_sqlite/patch.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/notepad/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/notepad/db_sqlite/storage.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/notepad/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/notepad/json_file.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/notepad/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/preset/base.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/preset/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/preset/json_file.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/preset/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/core/preset/patch.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/core/preset/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/gpt/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/gpt/assistants.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/gpt/assistants.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/gpt/chat.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/gpt/chat.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/gpt/completion.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/gpt/completion.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/gpt/image.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/gpt/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/gpt/summarizer.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/gpt/summarizer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/gpt/vision.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/gpt/vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/gpt/worker/assistants.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/gpt/worker/assistants.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/gpt/worker/importer.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/gpt/worker/importer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/llms/anthropic.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/llms/azure_openai.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/llms/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/llms/base.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/llms/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/llms/hugging_face.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/llms/hugging_face.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/llms/llama.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/llms/llama.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/llms/ollama.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/llms/ollama.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/llms/openai.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/llms/openai.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/base.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/file_csv.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/file_csv.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/file_docx.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/file_docx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/file_epub.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/file_epub.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/file_excel.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/file_excel.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/file_html.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/file_html.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/file_image_vision.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/file_image_vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/file_ipynb.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/file_ipynb.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/file_json.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/file_json.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/file_markdown.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/file_markdown.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/file_pdf.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/file_pdf.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/file_video_audio.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/file_video_audio.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/file_xml.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/file_xml.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/bitbucket/repo.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/bitbucket/repo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/base.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/database/base.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/database/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/github/issues.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/github/issues.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/github/repo.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/github/repo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/google/calendar.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/google/calendar.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/google/docs.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/google/docs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/google/gmail.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/google/gmail.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/google/keep.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/google/keep.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/google/sheets.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/google/sheets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/image_vision/base.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/image_vision/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/json/base.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/json/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/pandas_excel/base.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/pandas_excel/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/simple_csv/base.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/simple_csv/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/video_audio/base.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/video_audio/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/web_page/base.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/web_page/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/yt/base.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/yt/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/hub/yt/utils.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/hub/yt/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_bitbucket.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_bitbucket.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_chatgpt_retrieval.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_chatgpt_retrieval.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_database.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_database.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_github_issues.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_github_issues.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_github_repo.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_github_repo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_google_calendar.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_google_calendar.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_google_docs.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_google_docs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_google_drive.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_google_drive.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_google_gmail.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_google_gmail.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_google_keep.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_google_keep.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_google_sheets.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_google_sheets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_microsoft_onedrive.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_microsoft_onedrive.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_page.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_page.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_rss.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_rss.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_sitemap.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_sitemap.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_twitter.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_twitter.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/loaders/web_yt.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/loaders/web_yt.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/vector_stores/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/vector_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/vector_stores/base.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/vector_stores/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/vector_stores/chroma.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/vector_stores/chroma.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/vector_stores/elasticsearch.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/vector_stores/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/vector_stores/pinecode.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/vector_stores/pinecode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/vector_stores/redis.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/vector_stores/redis.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/vector_stores/simple.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/vector_stores/simple.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/vector_stores/temp.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/vector_stores/temp.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/web/base.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/web/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/web/google_custom_search.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/web/google_custom_search.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/provider/web/microsoft_bing.py` & `pygpt_net-2.1.9/src/pygpt_net/provider/web/microsoft_bing.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/base/config_dialog.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/base/config_dialog.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/dialog/about.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/dialog/about.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/dialog/applog.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/dialog/applog.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/dialog/assistant.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/dialog/assistant.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/dialog/changelog.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/dialog/changelog.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/dialog/create.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/dialog/create.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/dialog/debug.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/dialog/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/dialog/dictionary.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/dialog/dictionary.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/dialog/editor.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/dialog/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/dialog/image.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/dialog/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/dialog/license.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/dialog/license.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/dialog/logger.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/dialog/logger.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/dialog/models.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/dialog/models.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/dialog/plugins.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/dialog/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/dialog/preset.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/dialog/preset.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/dialog/rename.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/dialog/rename.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/dialog/settings.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/dialog/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/dialog/snap.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/dialog/snap.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/dialog/start.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/dialog/start.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/dialog/update.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/dialog/update.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/dialogs.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/layout/chat/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/layout/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/layout/chat/attachments.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/layout/chat/attachments.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/layout/chat/attachments_uploaded.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/layout/chat/attachments_uploaded.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/layout/chat/calendar.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/layout/chat/calendar.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/layout/chat/input.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/layout/chat/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/layout/chat/markdown.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/layout/chat/markdown.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/layout/chat/output.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/layout/chat/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/layout/chat/painter.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/layout/chat/painter.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/layout/ctx/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/layout/ctx/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/layout/ctx/ctx_list.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/layout/ctx/ctx_list.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/layout/ctx/search_input.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/layout/ctx/search_input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/layout/ctx/video.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/layout/ctx/video.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/layout/status.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/layout/status.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/layout/toolbox/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/layout/toolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/layout/toolbox/agent.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/layout/toolbox/agent.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/layout/toolbox/assistants.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/layout/toolbox/assistants.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/layout/toolbox/footer.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/layout/toolbox/footer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/layout/toolbox/image.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/layout/toolbox/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/layout/toolbox/indexes.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/layout/toolbox/indexes.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/layout/toolbox/mode.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/layout/toolbox/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/layout/toolbox/model.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/layout/toolbox/model.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/layout/toolbox/presets.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/layout/toolbox/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/layout/toolbox/prompt.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/layout/toolbox/prompt.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/layout/toolbox/vision.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/layout/toolbox/vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/main.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/main.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/menu/__init__.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/menu/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/menu/about.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/menu/about.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/menu/audio.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/menu/audio.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/menu/config.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/menu/config.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/menu/debug.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/menu/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/menu/file.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/menu/file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/menu/lang.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/menu/lang.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/menu/plugins.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/menu/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/menu/theme.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/menu/theme.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/menu/video.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/menu/video.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/tray.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/tray.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/audio/input.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/audio/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/audio/input_button.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/audio/input_button.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/audio/output.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/audio/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/calendar/select.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/calendar/select.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/alert.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/alert.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/applog.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/applog.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/base.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/confirm.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/confirm.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/create.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/create.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/debug.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/editor.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/editor_file.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/editor_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/image.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/info.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/info.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/license.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/license.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/logger.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/logger.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/model.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/model.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/rename.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/rename.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/settings.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/settings_plugin.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/settings_plugin.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/snap.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/snap.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/dialog/update.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/dialog/update.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/draw/painter.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/draw/painter.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/element/button.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/element/button.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/element/group.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/element/group.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/element/labels.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/element/labels.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/filesystem/explorer.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/filesystem/explorer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/image/display.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/image/display.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/lists/assistant.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/lists/assistant.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/lists/attachment.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/lists/attachment.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/lists/base.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/lists/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/lists/context.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/lists/context.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/lists/debug.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/lists/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/lists/index.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/lists/index.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/lists/mode.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/lists/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/lists/model.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/lists/model.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/lists/model_editor.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/lists/model_editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/lists/plugin.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/lists/plugin.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/lists/preset.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/lists/preset.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/lists/settings.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/lists/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/lists/uploaded.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/lists/uploaded.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/option/checkbox.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/option/checkbox.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/option/combo.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/option/combo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/option/dictionary.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/option/dictionary.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/option/input.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/option/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/option/slider.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/option/slider.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/option/textarea.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/option/textarea.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/tabs/Input.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/tabs/Input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/tabs/output.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/tabs/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/textarea/calendar_note.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/textarea/calendar_note.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/textarea/create.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/textarea/create.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/textarea/input.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/textarea/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/textarea/name.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/textarea/name.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/textarea/notepad.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/textarea/notepad.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/textarea/output.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/textarea/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/textarea/rename.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/textarea/rename.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/textarea/search_input.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/textarea/search_input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/ui/widget/vision/camera.py` & `pygpt_net-2.1.9/src/pygpt_net/ui/widget/vision/camera.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/src/pygpt_net/utils.py` & `pygpt_net-2.1.9/src/pygpt_net/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.1.8/PKG-INFO` & `pygpt_net-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygpt-net
-Version: 2.1.8
+Version: 2.1.9
 Summary: Desktop AI Assistant powered by GPT-4, GPT-4V, GPT-3.5, DALL-E 3, Langchain LLMs, Llama-index, Whisper with chatbot, assistant, text completion, vision and image generation, internet access, chat with files, commands and code execution, file upload and download and more
 Home-page: https://github.com/szczyglis-dev/py-gpt
 License: MIT
 Keywords: py_gpt,py-gpt,pygpt,desktop,app,gpt,gpt4,gpt4-v,gpt3.5,gpt-4,gpt-4V,gpt-3.5,tts,whisper,vision,chatgpt,dall-e,chat,chatbot,assistant,text completion,image generation,ai,api,openai,api key,langchain,llama-index,presets,ui,qt,pyside
 Author: Marcin Szczyglinski
 Author-email: info@pygpt.net
 Requires-Python: >=3.10,<3.12
@@ -65,15 +65,15 @@
 Project-URL: Repository, https://github.com/szczyglis-dev/py-gpt
 Description-Content-Type: text/markdown
 
 # PyGPT - Desktop AI Assistant
 
 [![pygpt](https://snapcraft.io/pygpt/badge.svg)](https://snapcraft.io/pygpt)
 
-Release: **2.1.8** | build: **2024.03.03** | Python: **>=3.10, <3.12**
+Release: **2.1.9** | build: **2024.03.04** | Python: **>=3.10, <3.12**
 
 Official website: https://pygpt.net | Documentation: https://pygpt.readthedocs.io
 
 Snap Store: https://snapcraft.io/pygpt | PyPi: https://pypi.org/project/pygpt-net
 
 Compiled version for Linux (`tar.gz`) and Windows 10/11 (`msi`) 64-bit: https://pygpt.net/#download
 
@@ -479,15 +479,15 @@
 ##  Chat with files (Llama-index)
 
 This mode enables chat interaction with your documents and entire context history through conversation. 
 It seamlessly incorporates `Llama-index` into the chat interface, allowing for immediate querying of your indexed documents.
 
 **Querying single files**
 
-From version `2.1.8`, you can also query individual files "on the fly" using the `query_file` command from the `Files I/O` plugin. This allows you to query any file by simply asking a question about that file. A temporary index will be created in memory for the file being queried, and an answer will be returned from it. 
+From version `2.1.8`, you can also query individual files "on the fly" using the `query_file` command from the `Files I/O` plugin. This allows you to query any file by simply asking a question about that file. A temporary index will be created in memory for the file being queried, and an answer will be returned from it. From version `2.1.9` similar command is available for querying web and external content: `Directly query web content with Llama-index`.
 
 For example:
 
 If you have a file: `data/my_cars.txt` with content `My car is red.`
 
 You can ask for: `Query the file my_cars.txt about what color my car is.`
 
@@ -1788,15 +1788,15 @@
 
 - `Enable: Read file` *cmd_read_file*
 
 Allows `read_file` command execution. *Default:* `True`
 
 - `Enable: Query file with Llama-index` *cmd_query_file*
 
-Allows `query_file` command execution *Default:* `True`
+Allows `query_file` command execution  (temporary index, on the fly) *Default:* `True`
 
 - `Enable: Append to file` *cmd_append_file*
 
 Allows `append_file` command execution. *Default:* `True`
 
 - `Enable: Save file` *cmd_save_file*
 
@@ -1981,27 +1981,29 @@
 
 If enabled, model will be able to open specified URL and get raw content
 
 - `Enable: "web_urls" command` *cmd_web_urls*
 
 If enabled, model will be able to search the Web and get founded URLs list
 
-If enabled, model will be able to search the Web and get founded URLs list
-
 - `Enable: "web_index" command` *cmd_web_index*
 
-If enabled, model will be able to index web pages using Llama-index
+If enabled, model will be able to index (on the fly) web pages using Llama-index (persistent index)
+
+- `Enable: "web_index_query" command - quick query the web content with Llama-index` *cmd_web_index_query*
+
+If enabled, model will be able to index and query web content using Llama-index (temporary index, on the fly)
 
 - `Auto-index all used URLs using Llama-index` *auto_index*
 
-If enabled, every URL used by the model will be automatically indexed using Llama-index
+If enabled, every URL used by the model will be automatically indexed using Llama-index (persistent index)
 
 - `Index to use` *idx*
 
-ID of index to use for web page indexing
+ID of index to use for web page indexing (persistent index)
 
 - `Model used for web page summarize` *summary_model*
 
 Model used for web page summarize, default: gpt-3.5-turbo-1106
 
 - `Summarize prompt` *prompt_summarize*
 
@@ -2796,15 +2798,17 @@
 
 - `Check for updates on start`: Enables checking for updates on start. Default: True.
 
 - `Check for updates in background`: Enables checking for updates in background (checking every 5 minutes). Default: True.
 
 **Developer**
 
-- `Show debug menu`: enables debug (developer) menu
+- `Show debug menu`: enables debug (developer) menu.
+
+- `Log and debug events`: Enables logging of events dispatch.
 
 - `Log plugin usage to console`: Enables logging of plugin usage to console.
 
 - `Log DALL-E usage to console`: Enables logging of DALL-E usage to console.
 
 - `Log Llama-index usage to console`: Enables logging of Llama-index usage to console.
 
@@ -2943,14 +2947,20 @@
 
 ---
 
 # CHANGELOG
 
 ## Recent changes:
 
+# 2.1.9 (2024-03-04)
+
+- A new option has been added to the `Web Search` plugin: `web_index_query`, which allows for indexing a web and external content in a temporary index (in memory) and quickly querying its content. Works similar to `query_file` command.
+- The `read_file` command has been expanded to handle multiple files at once.
+- Added `Log and debug events` option to Developer settings.
+
 # 2.1.8 (2024-03-03)
 
 - A new option has been added to the `Files I/O` plugin: `query_file`, which allows for indexing a file in a temporary index (in memory) and quickly querying its content. This enables the use of Llama-index for fast querying or adding context from individual files. From now on, you can ask questions about individual files without indexing them to the main vector store. See the "Querying single files" in "Modes -> Chat with files" section in a README for more info.
 - The `read_file` command has been expanded to return just the exact file content, without wrapping it in JSON.
 - Improved prompt for preparing queries in the Chat with files plugin.
 - Updated docs.
```

