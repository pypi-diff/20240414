# Comparing `tmp/nerfw-0.1.3.tar.gz` & `tmp/nerfw-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerfw-0.1.3.tar", last modified: Sun Apr 14 14:58:44 2024, max compression
+gzip compressed data, was "nerfw-0.1.4.tar", last modified: Sun Apr 14 15:24:39 2024, max compression
```

## Comparing `nerfw-0.1.3.tar` & `nerfw-0.1.4.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 14:58:44.094207 nerfw-0.1.3/
--rw-r--r--   0 root         (0) root         (0)     1094 2024-04-14 14:57:06.000000 nerfw-0.1.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4325 2024-04-14 14:58:44.094207 nerfw-0.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1630 2024-04-14 14:57:06.000000 nerfw-0.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 14:58:44.074207 nerfw-0.1.3/nerfw/
--rw-r--r--   0 root         (0) root         (0)      116 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 14:58:44.078207 nerfw-0.1.3/nerfw/game/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/game/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1214 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/game/animation.py
--rw-r--r--   0 root         (0) root         (0)     1422 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/game/audio.py
--rw-r--r--   0 root         (0) root         (0)     2446 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/game/character.py
--rw-r--r--   0 root         (0) root         (0)     1570 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/game/choice.py
--rw-r--r--   0 root         (0) root         (0)     3462 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/game/game.py
--rw-r--r--   0 root         (0) root         (0)     3308 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/game/scene.py
--rw-r--r--   0 root         (0) root         (0)     1210 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/game/string_input.py
--rw-r--r--   0 root         (0) root         (0)     1154 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/game/unlock_scene.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 14:58:44.082207 nerfw-0.1.3/nerfw/helpers/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      258 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/helpers/breaker.py
--rw-r--r--   0 root         (0) root         (0)     1590 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/helpers/db_handler.py
--rw-r--r--   0 root         (0) root         (0)     1209 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/helpers/deconstructor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 14:58:44.082207 nerfw-0.1.3/nerfw/helpers/errors/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/helpers/errors/__init__.py
--rw-r--r--   0 root         (0) root         (0)      212 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/helpers/errors/character_not_found.py
--rw-r--r--   0 root         (0) root         (0)      213 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/helpers/errors/function_not_found.py
--rw-r--r--   0 root         (0) root         (0)      183 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/helpers/errors/password_mismatch.py
--rw-r--r--   0 root         (0) root         (0)      248 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/helpers/errors/unsupported_login_method.py
--rw-r--r--   0 root         (0) root         (0)      207 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/helpers/errors/user_already_registered.py
--rw-r--r--   0 root         (0) root         (0)      199 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/helpers/errors/user_doesnt_exist.py
--rw-r--r--   0 root         (0) root         (0)      221 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/helpers/errors/user_not_allowed.py
--rw-r--r--   0 root         (0) root         (0)      239 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/helpers/errors/wrong_naming.py
--rw-r--r--   0 root         (0) root         (0)      621 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/helpers/img_handler.py
--rw-r--r--   0 root         (0) root         (0)     2419 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/helpers/input_handler.py
--rw-r--r--   0 root         (0) root         (0)      860 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/helpers/logger.py
--rw-r--r--   0 root         (0) root         (0)     1099 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/helpers/login_base.py
--rw-r--r--   0 root         (0) root         (0)     1087 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/helpers/recorder.py
--rw-r--r--   0 root         (0) root         (0)     2548 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/nerfw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 14:58:44.086207 nerfw-0.1.3/nerfw/server/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 14:58:44.090207 nerfw-0.1.3/nerfw/server/build/
--rw-r--r--   0 root         (0) root         (0)      763 2024-04-14 14:58:28.000000 nerfw-0.1.3/nerfw/server/build/asset-manifest.json
--rw-r--r--   0 root         (0) root         (0)      631 2024-04-14 14:58:19.000000 nerfw-0.1.3/nerfw/server/build/favicon.ico
--rw-r--r--   0 root         (0) root         (0)      648 2024-04-14 14:58:28.000000 nerfw-0.1.3/nerfw/server/build/index.html
--rw-r--r--   0 root         (0) root         (0)     6753 2024-04-14 14:58:19.000000 nerfw-0.1.3/nerfw/server/build/logo192.png
--rw-r--r--   0 root         (0) root         (0)    25319 2024-04-14 14:58:19.000000 nerfw-0.1.3/nerfw/server/build/logo512.png
--rw-r--r--   0 root         (0) root         (0)      482 2024-04-14 14:58:19.000000 nerfw-0.1.3/nerfw/server/build/manifest.json
--rw-r--r--   0 root         (0) root         (0)       67 2024-04-14 14:58:19.000000 nerfw-0.1.3/nerfw/server/build/robots.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 14:58:44.074207 nerfw-0.1.3/nerfw/server/build/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 14:58:44.090207 nerfw-0.1.3/nerfw/server/build/static/css/
--rw-r--r--   0 root         (0) root         (0)     7756 2024-04-14 14:58:28.000000 nerfw-0.1.3/nerfw/server/build/static/css/main.6c3c7095.css
--rw-r--r--   0 root         (0) root         (0)    15431 2024-04-14 14:58:28.000000 nerfw-0.1.3/nerfw/server/build/static/css/main.6c3c7095.css.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 14:58:44.090207 nerfw-0.1.3/nerfw/server/build/static/js/
--rw-r--r--   0 root         (0) root         (0)     4603 2024-04-14 14:58:28.000000 nerfw-0.1.3/nerfw/server/build/static/js/787.4afdcc44.chunk.js
--rw-r--r--   0 root         (0) root         (0)    10597 2024-04-14 14:58:28.000000 nerfw-0.1.3/nerfw/server/build/static/js/787.4afdcc44.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)   201232 2024-04-14 14:58:28.000000 nerfw-0.1.3/nerfw/server/build/static/js/main.0361928c.js
--rw-r--r--   0 root         (0) root         (0)     1697 2024-04-14 14:58:28.000000 nerfw-0.1.3/nerfw/server/build/static/js/main.0361928c.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   860030 2024-04-14 14:58:28.000000 nerfw-0.1.3/nerfw/server/build/static/js/main.0361928c.js.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 14:58:44.094207 nerfw-0.1.3/nerfw/server/build/static/media/
--rw-r--r--   0 root         (0) root         (0)      735 2024-04-14 14:58:28.000000 nerfw-0.1.3/nerfw/server/build/static/media/PATREON_SYMBOL_1_WHITE_RGB.17310609229eef2df4c7c31535ee8843.svg
--rw-r--r--   0 root         (0) root         (0)      960 2024-04-14 14:58:28.000000 nerfw-0.1.3/nerfw/server/build/static/media/github-mark-white.97ed8e7eef60d61ca469881dd6f34511.svg
--rw-r--r--   0 root         (0) root         (0)      775 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/server/gallery.py
--rw-r--r--   0 root         (0) root         (0)     1728 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/server/login_default.py
--rw-r--r--   0 root         (0) root         (0)     4527 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/server/login_github.py
--rw-r--r--   0 root         (0) root         (0)     5268 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/server/login_patreon.py
--rw-r--r--   0 root         (0) root         (0)     1447 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/server/password_manager.py
--rw-r--r--   0 root         (0) root         (0)      555 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/server/require_token.py
--rw-r--r--   0 root         (0) root         (0)     1219 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/server/saves_handler.py
--rw-r--r--   0 root         (0) root         (0)    11376 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/server/server.py
--rw-r--r--   0 root         (0) root         (0)     2090 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/server/token_handler.py
--rw-r--r--   0 root         (0) root         (0)     1501 2024-04-14 14:57:06.000000 nerfw-0.1.3/nerfw/server/wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 14:58:44.094207 nerfw-0.1.3/nerfw.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4325 2024-04-14 14:58:44.000000 nerfw-0.1.3/nerfw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2117 2024-04-14 14:58:44.000000 nerfw-0.1.3/nerfw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-14 14:58:44.000000 nerfw-0.1.3/nerfw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      114 2024-04-14 14:58:44.000000 nerfw-0.1.3/nerfw.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-14 14:58:44.000000 nerfw-0.1.3/nerfw.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1823 2024-04-14 14:57:06.000000 nerfw-0.1.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-14 14:58:44.094207 nerfw-0.1.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 15:24:39.697186 nerfw-0.1.4/
+-rw-r--r--   0 root         (0) root         (0)     1094 2024-04-14 15:23:06.000000 nerfw-0.1.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4325 2024-04-14 15:24:39.697186 nerfw-0.1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1630 2024-04-14 15:23:06.000000 nerfw-0.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 15:24:39.681186 nerfw-0.1.4/nerfw/
+-rw-r--r--   0 root         (0) root         (0)      116 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 15:24:39.681186 nerfw-0.1.4/nerfw/game/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/game/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1214 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/game/animation.py
+-rw-r--r--   0 root         (0) root         (0)     1422 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/game/audio.py
+-rw-r--r--   0 root         (0) root         (0)     2446 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/game/character.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/game/choice.py
+-rw-r--r--   0 root         (0) root         (0)     3462 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/game/game.py
+-rw-r--r--   0 root         (0) root         (0)     3308 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/game/scene.py
+-rw-r--r--   0 root         (0) root         (0)     1210 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/game/string_input.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/game/unlock_scene.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 15:24:39.685186 nerfw-0.1.4/nerfw/helpers/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      258 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/helpers/breaker.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/helpers/db_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/helpers/deconstructor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 15:24:39.689186 nerfw-0.1.4/nerfw/helpers/errors/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/helpers/errors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      212 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/helpers/errors/character_not_found.py
+-rw-r--r--   0 root         (0) root         (0)      213 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/helpers/errors/function_not_found.py
+-rw-r--r--   0 root         (0) root         (0)      183 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/helpers/errors/password_mismatch.py
+-rw-r--r--   0 root         (0) root         (0)      248 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/helpers/errors/unsupported_login_method.py
+-rw-r--r--   0 root         (0) root         (0)      207 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/helpers/errors/user_already_registered.py
+-rw-r--r--   0 root         (0) root         (0)      199 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/helpers/errors/user_doesnt_exist.py
+-rw-r--r--   0 root         (0) root         (0)      221 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/helpers/errors/user_not_allowed.py
+-rw-r--r--   0 root         (0) root         (0)      239 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/helpers/errors/wrong_naming.py
+-rw-r--r--   0 root         (0) root         (0)      621 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/helpers/img_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2419 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/helpers/input_handler.py
+-rw-r--r--   0 root         (0) root         (0)      860 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/helpers/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1099 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/helpers/login_base.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/helpers/recorder.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/nerfw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 15:24:39.689186 nerfw-0.1.4/nerfw/server/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 15:24:39.693186 nerfw-0.1.4/nerfw/server/build/
+-rw-r--r--   0 root         (0) root         (0)      763 2024-04-14 15:24:25.000000 nerfw-0.1.4/nerfw/server/build/asset-manifest.json
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-14 15:24:15.000000 nerfw-0.1.4/nerfw/server/build/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)      648 2024-04-14 15:24:25.000000 nerfw-0.1.4/nerfw/server/build/index.html
+-rw-r--r--   0 root         (0) root         (0)     6753 2024-04-14 15:24:15.000000 nerfw-0.1.4/nerfw/server/build/logo192.png
+-rw-r--r--   0 root         (0) root         (0)    25319 2024-04-14 15:24:15.000000 nerfw-0.1.4/nerfw/server/build/logo512.png
+-rw-r--r--   0 root         (0) root         (0)      482 2024-04-14 15:24:15.000000 nerfw-0.1.4/nerfw/server/build/manifest.json
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-14 15:24:15.000000 nerfw-0.1.4/nerfw/server/build/robots.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 15:24:39.677186 nerfw-0.1.4/nerfw/server/build/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 15:24:39.693186 nerfw-0.1.4/nerfw/server/build/static/css/
+-rw-r--r--   0 root         (0) root         (0)     7751 2024-04-14 15:24:25.000000 nerfw-0.1.4/nerfw/server/build/static/css/main.361d15c9.css
+-rw-r--r--   0 root         (0) root         (0)    15433 2024-04-14 15:24:25.000000 nerfw-0.1.4/nerfw/server/build/static/css/main.361d15c9.css.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 15:24:39.693186 nerfw-0.1.4/nerfw/server/build/static/js/
+-rw-r--r--   0 root         (0) root         (0)     4603 2024-04-14 15:24:25.000000 nerfw-0.1.4/nerfw/server/build/static/js/787.4afdcc44.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    10597 2024-04-14 15:24:25.000000 nerfw-0.1.4/nerfw/server/build/static/js/787.4afdcc44.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)   201232 2024-04-14 15:24:25.000000 nerfw-0.1.4/nerfw/server/build/static/js/main.0361928c.js
+-rw-r--r--   0 root         (0) root         (0)     1697 2024-04-14 15:24:25.000000 nerfw-0.1.4/nerfw/server/build/static/js/main.0361928c.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   860030 2024-04-14 15:24:25.000000 nerfw-0.1.4/nerfw/server/build/static/js/main.0361928c.js.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 15:24:39.697186 nerfw-0.1.4/nerfw/server/build/static/media/
+-rw-r--r--   0 root         (0) root         (0)      735 2024-04-14 15:24:25.000000 nerfw-0.1.4/nerfw/server/build/static/media/PATREON_SYMBOL_1_WHITE_RGB.17310609229eef2df4c7c31535ee8843.svg
+-rw-r--r--   0 root         (0) root         (0)      960 2024-04-14 15:24:25.000000 nerfw-0.1.4/nerfw/server/build/static/media/github-mark-white.97ed8e7eef60d61ca469881dd6f34511.svg
+-rw-r--r--   0 root         (0) root         (0)      775 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/server/gallery.py
+-rw-r--r--   0 root         (0) root         (0)     1728 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/server/login_default.py
+-rw-r--r--   0 root         (0) root         (0)     4527 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/server/login_github.py
+-rw-r--r--   0 root         (0) root         (0)     5268 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/server/login_patreon.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/server/password_manager.py
+-rw-r--r--   0 root         (0) root         (0)      555 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/server/require_token.py
+-rw-r--r--   0 root         (0) root         (0)     1219 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/server/saves_handler.py
+-rw-r--r--   0 root         (0) root         (0)    11376 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     2090 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/server/token_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1501 2024-04-14 15:23:06.000000 nerfw-0.1.4/nerfw/server/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 15:24:39.697186 nerfw-0.1.4/nerfw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4325 2024-04-14 15:24:39.000000 nerfw-0.1.4/nerfw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2117 2024-04-14 15:24:39.000000 nerfw-0.1.4/nerfw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-14 15:24:39.000000 nerfw-0.1.4/nerfw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      114 2024-04-14 15:24:39.000000 nerfw-0.1.4/nerfw.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-14 15:24:39.000000 nerfw-0.1.4/nerfw.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1823 2024-04-14 15:23:06.000000 nerfw-0.1.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-14 15:24:39.697186 nerfw-0.1.4/setup.cfg
```

### Comparing `nerfw-0.1.3/LICENSE` & `nerfw-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/PKG-INFO` & `nerfw-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerfw
-Version: 0.1.3
+Version: 0.1.4
 Summary: Framework for creation of web based visual novels
 Author-email: Nergan <noname.nosurname2016@yandex.ru>
 License: MIT License
         
         Copyright (c) 2021-present PyO3 Project and Contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nerfw-0.1.3/README.md` & `nerfw-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/game/animation.py` & `nerfw-0.1.4/nerfw/game/animation.py`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/game/audio.py` & `nerfw-0.1.4/nerfw/game/audio.py`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/game/character.py` & `nerfw-0.1.4/nerfw/game/character.py`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/game/choice.py` & `nerfw-0.1.4/nerfw/game/choice.py`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/game/game.py` & `nerfw-0.1.4/nerfw/game/game.py`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/game/scene.py` & `nerfw-0.1.4/nerfw/game/scene.py`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/game/string_input.py` & `nerfw-0.1.4/nerfw/game/string_input.py`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/game/unlock_scene.py` & `nerfw-0.1.4/nerfw/game/unlock_scene.py`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/helpers/db_handler.py` & `nerfw-0.1.4/nerfw/helpers/db_handler.py`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/helpers/deconstructor.py` & `nerfw-0.1.4/nerfw/helpers/deconstructor.py`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/helpers/img_handler.py` & `nerfw-0.1.4/nerfw/helpers/img_handler.py`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/helpers/input_handler.py` & `nerfw-0.1.4/nerfw/helpers/input_handler.py`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/helpers/logger.py` & `nerfw-0.1.4/nerfw/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/helpers/login_base.py` & `nerfw-0.1.4/nerfw/helpers/login_base.py`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/helpers/recorder.py` & `nerfw-0.1.4/nerfw/helpers/recorder.py`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/nerfw.py` & `nerfw-0.1.4/nerfw/nerfw.py`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/server/build/favicon.ico` & `nerfw-0.1.4/nerfw/server/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/server/build/index.html` & `nerfw-0.1.4/nerfw/server/build/index.html`

 * *Files 19% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/favicon.ico?v=2"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="NerFW" content="Web site created using create-react-app"/><link rel="apple-touch-icon" href="/logo192.png"/><link rel="manifest" href="/manifest.json"/><title>{{ name_game }}</title><script defer="defer" src="/static/js/main.0361928c.js"></script><link href="/static/css/main.6c3c7095.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
+<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/favicon.ico?v=2"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="NerFW" content="Web site created using create-react-app"/><link rel="apple-touch-icon" href="/logo192.png"/><link rel="manifest" href="/manifest.json"/><title>{{ name_game }}</title><script defer="defer" src="/static/js/main.0361928c.js"></script><link href="/static/css/main.361d15c9.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
```

### Comparing `nerfw-0.1.3/nerfw/server/build/logo192.png` & `nerfw-0.1.4/nerfw/server/build/logo192.png`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/server/build/logo512.png` & `nerfw-0.1.4/nerfw/server/build/logo512.png`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/server/build/static/css/main.6c3c7095.css` & `nerfw-0.1.4/nerfw/server/build/static/css/main.361d15c9.css`

 * *Files 2% similar despite different names*

```diff
@@ -1,2 +1,2 @@
-body{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Oxygen,Ubuntu,Cantarell,Fira Sans,Droid Sans,Helvetica Neue,sans-serif}*,body{margin:0}*{box-sizing:border-box;padding:0}code{font-family:source-code-pro,Menlo,Monaco,Consolas,Courier New,monospace}.App{text-align:center}.App-logo{height:40vmin;pointer-events:none}@media (prefers-reduced-motion:no-preference){.App-logo{-webkit-animation:App-logo-spin 20s linear infinite;animation:App-logo-spin 20s linear infinite}}.App-header{align-items:center;background-color:#282c34;color:#fff;display:flex;flex-direction:column;font-size:calc(10px + 2vmin);justify-content:center;min-height:100vh}.App-link{color:#61dafb}@-webkit-keyframes App-logo-spin{0%{-webkit-transform:rotate(0deg);transform:rotate(0deg)}to{-webkit-transform:rotate(1turn);transform:rotate(1turn)}}@keyframes App-logo-spin{0%{-webkit-transform:rotate(0deg);transform:rotate(0deg)}to{-webkit-transform:rotate(1turn);transform:rotate(1turn)}}.choice{align-items:center;align-self:center;border-radius:10px;flex-direction:column;gap:20px;justify-content:center;padding:30px}#dialogue_menu,.choice{background:#44475a90;box-shadow:inset 0 0 20px hsla(0,0%,100%,.5);display:flex;outline-color:hsla(0,0%,100%,0);position:absolute}#dialogue_menu{bottom:1%;flex-direction:column-reverse;height:30%;justify-content:space-between;left:1%;right:1%;text-shadow:1px 1px 2px #427388;width:98%}button_div{margin:10px}.stringInput{align-items:center;align-self:center;background:#44475a90;border-radius:10px;box-shadow:inset 0 0 20px hsla(0,0%,100%,.5);display:flex;flex-direction:column;gap:10px;justify-content:center;outline-color:hsla(0,0%,100%,0);padding:30px;position:fixed}.button_specific{position:relative;width:-webkit-fit-content;width:-moz-fit-content;width:fit-content}.big_wrapper{background:#00000090;display:flex;flex-direction:column;height:100%;justify-content:center;left:0;position:fixed;top:0;width:100%}input{margin:0}label{color:#fff;font-size:20px;font-weight:700}@-webkit-keyframes slideIn{0%{left:var(--moveStartX);top:var(--moveStartY)}to{left:var(--moveEndX);top:var(--moveEndY)}}@keyframes slideIn{0%{left:var(--moveStartX);top:var(--moveStartY)}to{left:var(--moveEndX);top:var(--moveEndY)}}html{-webkit-user-select:none;user-select:none}body,html{height:100%}body{background:#282a36}button{background-color:initial;border:0 solid;box-shadow:inset 0 0 20px hsla(0,0%,100%,0);color:#fff;cursor:pointer;font-size:16px;font-weight:400;margin:0 0 1%;outline:1px solid;outline-color:hsla(0,0%,100%,.5);outline-offset:0;padding:7px 12px;text-decoration:none;text-shadow:none;text-transform:uppercase;transition:all 1.25s cubic-bezier(.19,1,.22,1)}button:hover{border:1px solid;box-shadow:inset 0 0 20px hsla(0,0%,100%,.5),0 0 20px hsla(0,0%,100%,.2);outline-color:hsla(0,0%,100%,0);outline-offset:15px;text-shadow:1px 1px 2px #427388}input[type=submit]{background-color:initial;border:0 solid;box-shadow:inset 0 0 20px hsla(0,0%,100%,0);color:#fff;cursor:pointer;font-size:16px;font-weight:400;margin:0 0 2em;outline:1px solid;outline-color:hsla(0,0%,100%,.5);outline-offset:0;padding:7px 12px;text-decoration:none;text-shadow:none;text-transform:uppercase;transition:all 1.25s cubic-bezier(.19,1,.22,1)}input[type=submit]:hover{border:1px solid;box-shadow:inset 0 0 20px hsla(0,0%,100%,.5),0 0 20px hsla(0,0%,100%,.2);outline-color:hsla(0,0%,100%,0);outline-offset:15px;text-shadow:1px 1px 2px #427388}input[type=password],input[type=text]{background-color:initial;border:0 solid;box-shadow:inset 0 0 20px hsla(0,0%,100%,0);color:#fff;cursor:pointer;font-size:16px;font-weight:400;margin:0 0 2em;outline:1px solid;outline-color:hsla(0,0%,100%,.5);outline-offset:0;padding:7px 12px;text-decoration:none;text-shadow:none;transition:all 1.25s cubic-bezier(.19,1,.22,1)}input[type=password]:hover,input[type=text]:hover{border:1px solid;box-shadow:inset 0 0 20px hsla(0,0%,100%,.5),0 0 20px hsla(0,0%,100%,.2);text-shadow:1px 1px 2px #427388}#popup{align-items:center;background-color:#313442;border-radius:10px;box-shadow:inset 0 0 20px hsla(0,0%,100%,.5);color:#fff;display:none;flex-direction:column;font-size:16px;font-weight:400;height:10%;justify-content:center;outline:1px solid;outline-color:hsla(0,0%,100%,.5);padding:30px;position:fixed;width:9%;z-index:1}.MainMenuButtons{align-items:left;display:flex;flex-direction:column;margin:10px;width:15%}.MainMenuButtons button{background:linear-gradient(90deg,#fff5,#fff0,#0000);background-position:99%;background-size:200% 100%;border-bottom:1px solid #fff;border-image:linear-gradient(90deg,#fff,#fff0,#0000);border-image-slice:1;cursor:pointer;margin:5px;outline:none;padding:5px;text-align:left}.MainMenuButtons button:hover{background-position:0;border:0 solid;border-bottom:1px solid #fff;border-image:linear-gradient(90deg,#fff,#fff0);border-image-slice:1;box-shadow:none;outline:none}.LogOutButton{bottom:0;margin:20px;position:fixed}.login-wrapper{align-items:center;display:flex;flex-direction:column;height:100%;justify-content:space-around}#root{height:100%}form{display:flex;flex-direction:column;height:10%;justify-content:space-around}.outterWrapper{height:100vh}.button-Github{background-color:#ffffff20;margin:10%}img{border-radius:15px;margin:5%}.innerWrapper,.outterWrapper{align-items:center;display:flex;flex-direction:column;justify-content:center}.innerWrapper{background-color:#00000030;border:1px solid #ccc;border-radius:15px;box-shadow:0 0 20px #ccc;margin:25%;padding:20px}.button-Patreon{background-color:#ffffff20;margin:10%}.innerWrapper img{border-radius:15px;margin:10%;width:80%}.LoadSave{background:linear-gradient(90deg,#fff5,#fff0,#0000);background-position:99%;background-size:200% 100%;border-bottom:1px solid #fff;border-image:linear-gradient(90deg,#fff,#fff0,#0000);border-image-slice:1;outline:none;text-align:left}.LoadSave:hover{background-position:0;border:0 solid;border-bottom:1px solid #fff;border-image:linear-gradient(90deg,#fff,#fff0);border-image-slice:1;box-shadow:none;outline:none}.ButtonsDiv{display:flex;flex-direction:column;width:10%}.Save{position:relative;transition:all .5s ease-in-out}.Save:after{background-image:linear-gradient(90deg,#282a36,rgba(1,1,1,0))}.SavesScreenshots{display:grid;grid-template:1fr/1fr;height:100%;place-items:center}.SavesScreenshots>*{grid-column:1/1;grid-row:1/1}.GalleryWrapper{display:flex;flex-direction:row;margin:20px}.CategorieSelector{display:flex;flex-direction:column;justify-content:left;width:15%}.CategorieButton{background:linear-gradient(90deg,#fff5,#fff0,#0000);background-position:99%;background-size:200% 100%;border-bottom:1px solid #fff;border-image:linear-gradient(90deg,#fff,#fff0,#0000);border-image-slice:1;cursor:pointer;margin:5px;outline:none;padding:5px;text-align:left}.CategorieButton:hover{background-position:0;border:0 solid;border-bottom:1px solid #fff;border-image:linear-gradient(90deg,#fff,#fff0);border-image-slice:1;box-shadow:none;outline:none}.MainMenuButtonDiv{bottom:1%;left:1%;position:fixed}.ImageFrame{border:2px solid #fff;border-radius:10px;box-shadow:inset 0 0 20px hsla(0,0%,100%,.5),0 0 20px hsla(0,0%,100%,.2);cursor:pointer;display:flex;flex-direction:column;justify-content:left;margin:10px;transition:all 1.25s cubic-bezier(.19,1,.22,1)}.Title{color:#fff;font-size:20px;font-weight:400;text-align:center}.GalleryImages{display:flex;overflow:auto}.ImagesInner{flex-direction:row;flex-wrap:wrap;margin:10px}.ImagesInner,.unauthenticated{align-items:center;display:flex;justify-content:center}.unauthenticated{flex-direction:column;height:100%;width:100%}.button-unauth{bottom:0;position:fixed}h1,h2{color:#fff}
-/*# sourceMappingURL=main.6c3c7095.css.map*/
+body{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Oxygen,Ubuntu,Cantarell,Fira Sans,Droid Sans,Helvetica Neue,sans-serif}*,body{margin:0}*{box-sizing:border-box;padding:0}code{font-family:source-code-pro,Menlo,Monaco,Consolas,Courier New,monospace}.App{text-align:center}.App-logo{height:40vmin;pointer-events:none}@media (prefers-reduced-motion:no-preference){.App-logo{-webkit-animation:App-logo-spin 20s linear infinite;animation:App-logo-spin 20s linear infinite}}.App-header{align-items:center;background-color:#282c34;color:#fff;display:flex;flex-direction:column;font-size:calc(10px + 2vmin);justify-content:center;min-height:100vh}.App-link{color:#61dafb}@-webkit-keyframes App-logo-spin{0%{-webkit-transform:rotate(0deg);transform:rotate(0deg)}to{-webkit-transform:rotate(1turn);transform:rotate(1turn)}}@keyframes App-logo-spin{0%{-webkit-transform:rotate(0deg);transform:rotate(0deg)}to{-webkit-transform:rotate(1turn);transform:rotate(1turn)}}.choice{align-items:center;align-self:center;border-radius:10px;flex-direction:column;gap:20px;justify-content:center;padding:30px}#dialogue_menu,.choice{background:#44475a90;box-shadow:inset 0 0 20px hsla(0,0%,100%,.5);display:flex;outline-color:hsla(0,0%,100%,0);position:absolute}#dialogue_menu{bottom:1%;flex-direction:column-reverse;height:30%;justify-content:space-between;left:1%;right:1%;text-shadow:1px 1px 2px #427388;width:98%}button_div{margin:10px}.stringInput{align-items:center;align-self:center;background:#44475a90;border-radius:10px;box-shadow:inset 0 0 20px hsla(0,0%,100%,.5);display:flex;flex-direction:column;gap:10px;justify-content:center;outline-color:hsla(0,0%,100%,0);padding:30px;position:fixed}.button_specific{position:relative;width:-webkit-fit-content;width:-moz-fit-content;width:fit-content}.big_wrapper{background:#00000090;display:flex;flex-direction:column;height:100%;justify-content:center;left:0;position:fixed;top:0;width:100%}input{margin:0}label{color:#fff;font-size:20px;font-weight:700}@-webkit-keyframes slideIn{0%{left:var(--moveStartX);top:var(--moveStartY)}to{left:var(--moveEndX);top:var(--moveEndY)}}@keyframes slideIn{0%{left:var(--moveStartX);top:var(--moveStartY)}to{left:var(--moveEndX);top:var(--moveEndY)}}html{-webkit-user-select:none;user-select:none}body,html{height:100%}body{background:#282a36}button{background-color:initial;border:0 solid;box-shadow:inset 0 0 20px hsla(0,0%,100%,0);color:#fff;cursor:pointer;font-size:16px;font-weight:400;margin:0 0 1%;outline:1px solid;outline-color:hsla(0,0%,100%,.5);outline-offset:0;padding:7px 12px;text-decoration:none;text-shadow:none;text-transform:uppercase;transition:all 1.25s cubic-bezier(.19,1,.22,1)}button:hover{border:1px solid;box-shadow:inset 0 0 20px hsla(0,0%,100%,.5),0 0 20px hsla(0,0%,100%,.2);outline-color:hsla(0,0%,100%,0);outline-offset:15px;text-shadow:1px 1px 2px #427388}input[type=submit]{background-color:initial;border:0 solid;box-shadow:inset 0 0 20px hsla(0,0%,100%,0);color:#fff;cursor:pointer;font-size:16px;font-weight:400;margin:0 0 2em;outline:1px solid;outline-color:hsla(0,0%,100%,.5);outline-offset:0;padding:7px 12px;text-decoration:none;text-shadow:none;text-transform:uppercase;transition:all 1.25s cubic-bezier(.19,1,.22,1)}input[type=submit]:hover{border:1px solid;box-shadow:inset 0 0 20px hsla(0,0%,100%,.5),0 0 20px hsla(0,0%,100%,.2);outline-color:hsla(0,0%,100%,0);outline-offset:15px;text-shadow:1px 1px 2px #427388}input[type=password],input[type=text]{background-color:initial;border:0 solid;box-shadow:inset 0 0 20px hsla(0,0%,100%,0);color:#fff;cursor:pointer;font-size:16px;font-weight:400;margin:0 0 2em;outline:1px solid;outline-color:hsla(0,0%,100%,.5);outline-offset:0;padding:7px 12px;text-decoration:none;text-shadow:none;transition:all 1.25s cubic-bezier(.19,1,.22,1)}input[type=password]:hover,input[type=text]:hover{border:1px solid;box-shadow:inset 0 0 20px hsla(0,0%,100%,.5),0 0 20px hsla(0,0%,100%,.2);text-shadow:1px 1px 2px #427388}#popup{align-items:center;background-color:#313442;border-radius:10px;box-shadow:inset 0 0 20px hsla(0,0%,100%,.5);color:#fff;display:none;flex-direction:column;font-size:16px;font-weight:400;height:10%;justify-content:center;outline:1px solid;outline-color:hsla(0,0%,100%,.5);padding:30px;position:fixed;width:9%;z-index:1}.MainMenuButtons{align-items:left;display:flex;flex-direction:column;margin:10px;width:15%}.MainMenuButtons button{background:linear-gradient(90deg,#fff5,#fff0,#0000);background-position:99%;background-size:200% 100%;border-bottom:1px solid #fff;border-image:linear-gradient(90deg,#fff,#fff0,#0000);border-image-slice:1;cursor:pointer;margin:5px;outline:none;padding:5px;text-align:left}.MainMenuButtons button:hover{background-position:0;border:0 solid;border-bottom:1px solid #fff;border-image:linear-gradient(90deg,#fff,#fff0);border-image-slice:1;box-shadow:none;outline:none}.LogOutButton{bottom:0;margin:20px;position:fixed}.login-wrapper{align-items:center;display:flex;flex-direction:column;height:100%;justify-content:space-around}#root{height:100%}form{display:flex;flex-direction:column;height:10%;justify-content:space-around}.outterWrapper{height:100vh}.button-Github{background-color:#ffffff20;margin:10%}.innerWrapper img{margin:5%}.innerWrapper,.outterWrapper{align-items:center;display:flex;flex-direction:column;justify-content:center}.innerWrapper{background-color:#00000030;border:1px solid #ccc;border-radius:15px;box-shadow:0 0 20px #ccc;margin:25%;padding:20px}.button-Patreon{background-color:#ffffff20;margin:10%}.innerWrapper img{border-radius:15px;margin:10%;width:80%}.LoadSave{background:linear-gradient(90deg,#fff5,#fff0,#0000);background-position:99%;background-size:200% 100%;border-bottom:1px solid #fff;border-image:linear-gradient(90deg,#fff,#fff0,#0000);border-image-slice:1;outline:none;text-align:left}.LoadSave:hover{background-position:0;border:0 solid;border-bottom:1px solid #fff;border-image:linear-gradient(90deg,#fff,#fff0);border-image-slice:1;box-shadow:none;outline:none}.ButtonsDiv{display:flex;flex-direction:column;width:10%}.Save{position:relative;transition:all .5s ease-in-out}.Save:after{background-image:linear-gradient(90deg,#282a36,rgba(1,1,1,0))}.SavesScreenshots{display:grid;grid-template:1fr/1fr;height:100%;place-items:center}.SavesScreenshots>*{grid-column:1/1;grid-row:1/1}.GalleryWrapper{display:flex;flex-direction:row;margin:20px}.CategorieSelector{display:flex;flex-direction:column;justify-content:left;width:15%}.CategorieButton{background:linear-gradient(90deg,#fff5,#fff0,#0000);background-position:99%;background-size:200% 100%;border-bottom:1px solid #fff;border-image:linear-gradient(90deg,#fff,#fff0,#0000);border-image-slice:1;cursor:pointer;margin:5px;outline:none;padding:5px;text-align:left}.CategorieButton:hover{background-position:0;border:0 solid;border-bottom:1px solid #fff;border-image:linear-gradient(90deg,#fff,#fff0);border-image-slice:1;box-shadow:none;outline:none}.MainMenuButtonDiv{bottom:1%;left:1%;position:fixed}.ImageFrame{border:2px solid #fff;border-radius:10px;box-shadow:inset 0 0 20px hsla(0,0%,100%,.5),0 0 20px hsla(0,0%,100%,.2);cursor:pointer;display:flex;flex-direction:column;justify-content:left;margin:10px;transition:all 1.25s cubic-bezier(.19,1,.22,1)}.Title{color:#fff;font-size:20px;font-weight:400;text-align:center}.GalleryImages{display:flex;overflow:auto}.ImagesInner{flex-direction:row;flex-wrap:wrap;margin:10px}.ImagesInner,.unauthenticated{align-items:center;display:flex;justify-content:center}.unauthenticated{flex-direction:column;height:100%;width:100%}.button-unauth{bottom:0;position:fixed}h1,h2{color:#fff}
+/*# sourceMappingURL=main.361d15c9.css.map*/
```

### Comparing `nerfw-0.1.3/nerfw/server/build/static/css/main.6c3c7095.css.map` & `nerfw-0.1.4/nerfw/server/build/static/css/main.361d15c9.css.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8469387755102041%*

 * *Differences: {"'file'": "'static/css/main.361d15c9.css'",*

 * * "'mappings'": "'AAAA,KAKE,kCAAmC,CACnC,iCAAkC,CAJlC,mIAMF,CAEA,OATE,QAaD,CAJD,EAGE,qBAAsB,CADtB,SAED,CAGD,KACE,uEAEF,CCpBA,KACE,iBACF,CAEA,UACE,aAAc,CACd,mBACF,CAEA,8CACE,UACE,mDAA4C,CAA5C,2CACF,CACF,CAEA,YAKE,kBAAmB,CAJnB,wBAAyB,CAOzB,UAAY,CALZ,YAAa,CACb,qBAAsB,CAGtB,4BAA6B,CAD7B,sBAAuB,CAJvB,gBAOF,CAEA,UACE,aACF,CAEA,iCACE,GACE,8BAAuB,CAAvB,sBACF,CACA,GACE,+BAAyB,CAAzB,uBACF,CACF,CAPA,yBACE,GACE,8BAAuB,CAAvB,sBACF,CACA,GACE,+BAAyB,CAAzB,uBACF,CACF,CCrCA,QAKI,k […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/css/main.6c3c7095.css",
-    "mappings": "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",
+    "file": "static/css/main.361d15c9.css",
+    "mappings": "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",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "stylesheets/index.css",
         "stylesheets/App.css",
         "game/choices.css",
         "game/dialogue_menu.css",
@@ -22,15 +22,15 @@
         "body {\n  margin: 0;\n  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Roboto', 'Oxygen',\n    'Ubuntu', 'Cantarell', 'Fira Sans', 'Droid Sans', 'Helvetica Neue',\n    sans-serif;\n  -webkit-font-smoothing: antialiased;\n  -moz-osx-font-smoothing: grayscale;\n  height: 100%;\n}\n\n*{\n  margin: 0;\n  padding: 0;\n  box-sizing: border-box;\n }\n \n\ncode {\n  font-family: source-code-pro, Menlo, Monaco, Consolas, 'Courier New',\n    monospace;\n}\n",
         ".App {\n  text-align: center;\n}\n\n.App-logo {\n  height: 40vmin;\n  pointer-events: none;\n}\n\n@media (prefers-reduced-motion: no-preference) {\n  .App-logo {\n    animation: App-logo-spin infinite 20s linear;\n  }\n}\n\n.App-header {\n  background-color: #282c34;\n  min-height: 100vh;\n  display: flex;\n  flex-direction: column;\n  align-items: center;\n  justify-content: center;\n  font-size: calc(10px + 2vmin);\n  color: white;\n}\n\n.App-link {\n  color: #61dafb;\n}\n\n@keyframes App-logo-spin {\n  from {\n    transform: rotate(0deg);\n  }\n  to {\n    transform: rotate(360deg);\n  }\n}\n",
         ".choice {\n    background: #44475a90;\n    display: flex;\n    justify-content: center;\n    flex-direction: column;\n    align-items: center;\n    position: absolute;\n    padding: 30px 30px 30px 30px;\n    gap: 20px;\n    outline-color: rgba(255, 255, 255, 0);\n    box-shadow: inset 0 0 20px rgba(255, 255, 255, .5);\n    border-radius: 10px;\n    align-self: center;\n}\n\n.button_specific {\n    position: relative;\n    width: fit-content;\n}\n\n.big_wrapper {\n    background: #00000090;\n    width: 100%;\n    height: 100%;\n    display: flex;\n    justify-content: center;\n    position: fixed;\n    flex-direction: column;\n    top: 0;\n    left: 0;\n}",
         "#dialogue_menu {\n    display: flex;\n    flex-direction: column-reverse;\n    justify-content: space-between;\n    background: #44475a90;\n    outline-color: rgba(255, 255, 255, 0);\n    box-shadow: inset 0 0 20px rgba(255, 255, 255, .5);\n    text-shadow: 1px 1px 2px #427388;\n    position: absolute;\n    width: 98%;\n    bottom: 1%;\n    height: 30%;\n    right: 1%;\n    left: 1%;\n}\n\nbutton_div {\n    margin: 10px;\n}",
         ".stringInput {\n    background: #44475a90;\n    display: flex;\n    justify-content: center;\n    flex-direction: column;\n    align-items: center;\n    position: fixed;\n    padding: 30px 30px 30px 30px;\n    gap: 10px;\n    outline-color: rgba(255, 255, 255, 0);\n    box-shadow: inset 0 0 20px rgba(255, 255, 255, .5);\n    border-radius: 10px;\n    align-self: center;\n}\n\n.button_specific {\n    position: relative;\n    width: fit-content;\n}\n\n.big_wrapper {\n    background: #00000090;\n    width: 100%;\n    height: 100%;\n    display: flex;\n    justify-content: center;\n    position: fixed;\n    flex-direction: column;\n    top: 0;\n    left: 0;\n}\n\ninput {\n    margin: 0 0 0;\n}\n\nlabel {\n    color: white;\n    font-size: 20px;\n    font-weight: bold;\n}",
         "@keyframes slideIn {\n    from {\n        left: var(--moveStartX);\n        top: var(--moveStartY);\n    }\n    to {\n        left: var(--moveEndX);\n        top: var(--moveEndY);\n    }\n}\n\n\n\nhtml {\n  height: 100%;\n  user-select: none;\n}\n\nbody {\n  background: #282a36;\n  height: 100%;\n}\n\nbutton {\n    background-color: transparent;\n    border: 0 solid;\n    box-shadow: inset 0 0 20px rgba(255, 255, 255, 0);\n    outline: 1px solid;\n    outline-color: rgba(255, 255, 255, .5);\n    outline-offset: 0px;\n    text-shadow: none;\n    transition: all 1250ms cubic-bezier(0.19, 1, 0.22, 1);\n    color: #fff;\n    cursor: pointer;\n    font-size:16px;\n    font-weight: 400;\n    text-decoration: none;\n    text-transform: uppercase;\n    padding: 7px 12px;\n    margin: 0 0 1%;\n    cursor: pointer;\n}\n\nbutton:hover {\n  border: 1px solid;\n  box-shadow: inset 0 0 20px rgba(255, 255, 255, .5), 0 0 20px rgba(255, 255, 255, .2);\n  outline-color: rgba(255, 255, 255, 0);\n  outline-offset: 15px;\n  text-shadow: 1px 1px 2px #427388;\n}\n\ninput[type=submit] {\n  background-color: transparent;\n  border: 0 solid;\n  box-shadow: inset 0 0 20px rgba(255, 255, 255, 0);\n  outline: 1px solid;\n  outline-color: rgba(255, 255, 255, .5);\n  outline-offset: 0px;\n  text-shadow: none;\n  transition: all 1250ms cubic-bezier(0.19, 1, 0.22, 1);\n  color: #fff;\n  cursor: pointer;\n  font-size:16px;\n  font-weight: 400;\n  margin: 0 0 2em;\n  text-decoration: none;\n  text-transform: uppercase;\n  padding: 7px 12px;\n}\n\ninput[type=submit]:hover {\n  border: 1px solid;\n  box-shadow: inset 0 0 20px rgba(255, 255, 255, .5), 0 0 20px rgba(255, 255, 255, .2);\n  outline-color: rgba(255, 255, 255, 0);\n  outline-offset: 15px;\n  text-shadow: 1px 1px 2px #427388;\n}\n\ninput[type=text], input[type=password] {\n  background-color: transparent;\n  border: 0 solid;\n  box-shadow: inset 0 0 20px rgba(255, 255, 255, 0);\n  outline: 1px solid;\n  outline-color: rgba(255, 255, 255, .5);\n  outline-offset: 0px;\n  text-shadow: none;\n  transition: all 1250ms cubic-bezier(0.19, 1, 0.22, 1);\n  color: #fff;\n  cursor: pointer;\n  font-size:16px;\n  font-weight: 400;\n  margin: 0 0 2em;\n  text-decoration: none;\n  padding: 7px 12px;\n}\n\ninput[type=text]:hover, input[type=password]:hover {\n  border: 1px solid;\n  box-shadow: inset 0 0 20px rgba(255, 255, 255, .5), 0 0 20px rgba(255, 255, 255, .2);\n  text-shadow: 1px 1px 2px #427388;\n}\n\n#popup {\n    display: none;\n    position: fixed;\n    z-index: 1;\n    width: 9%;\n    height: 10%;\n    justify-content: center;\n    align-items: center;\n    background-color: #313442;\n    border-radius: 10px;\n    outline: 1px solid;\n    outline-color: rgba(255, 255, 255, .5);\n    box-shadow: inset 0 0 20px rgba(255, 255, 255, .5);\n    color: #fff;\n    font-weight: 400;\n    font-size: 16px;\n    flex-direction: column;\n    padding: 30px 30px 30px 30px;\n}\n\n.MainMenuButtons {\n    display: flex;\n    flex-direction: column;\n    align-items: left;\n    width: 15%;\n    margin: 10px;\n}\n\n.MainMenuButtons button {\n    margin: 10px;\n  margin: 5px;\n  padding: 5px;\n  cursor: pointer;\n  outline: none;\n  background: linear-gradient(to right, #fff5, #fff0, #0000);\n  background-size: 200% 100%;\n  background-position: 99%;\n  border-bottom: 1px solid #fff;\n  border-image: linear-gradient(to right, #fff, #fff0, #0000);\n  border-image-slice: 1;\n  text-align: left;\n}\n\n.MainMenuButtons button:hover {\n  outline: none;\n  border: 0px solid;\n  border-bottom: 1px solid #fff;\n  border-image: linear-gradient(to right, #fff, #fff0);\n  border-image-slice: 1;\n  box-shadow: none;\n  background-position: 0%;\n}\n\n.LogOutButton {\n  position: fixed;\n  bottom: 0;\n  margin: 20px;\n}\n",
         ".login-wrapper {\n    height: 100%;\n    display: flex;\n    align-items: center;\n    flex-direction: column;\n    justify-content: space-around;\n}\n\n#root{\n    height: 100%;\n}\n\nform {\n    display: flex;\n    justify-content: space-around;\n    flex-direction: column;\n    height: 10%;\n}",
-        ".outterWrapper {\n    display: flex;\n    flex-direction: column;\n    justify-content: center;\n    align-items: center;\n    height: 100vh;\n}\n\n.innerWrapper {\n    display: flex;\n    flex-direction: column;\n    justify-content: center;\n    align-items: center;\n\n    border: 1px solid #ccc;\n    border-radius: 15px;\n    box-shadow: 0 0 20px #ccc;\n    background-color: #00000030;\n    padding: 20px 20px 20px 20px;\n}\n\n.button-Github {\n    margin: 10%;\n    background-color: #ffffff20;\n}\n\nimg {\n    margin: 5%;\n    border-radius: 15px;\n}",
+        ".outterWrapper {\n    display: flex;\n    flex-direction: column;\n    justify-content: center;\n    align-items: center;\n    height: 100vh;\n}\n\n.innerWrapper {\n    display: flex;\n    flex-direction: column;\n    justify-content: center;\n    align-items: center;\n\n    border: 1px solid #ccc;\n    border-radius: 15px;\n    box-shadow: 0 0 20px #ccc;\n    background-color: #00000030;\n    padding: 20px 20px 20px 20px;\n}\n\n.button-Github {\n    margin: 10%;\n    background-color: #ffffff20;\n}\n\n.innerWrapper img {\n    margin: 5%;\n    border-radius: 15px;\n}",
         ".outterWrapper {\n    display: flex;\n    flex-direction: column;\n    justify-content: center;\n    align-items: center;\n}\n\n.innerWrapper {\n    display: flex;\n    flex-direction: column;\n    justify-content: center;\n    align-items: center;\n\n    border: 1px solid #ccc;\n    border-radius: 15px;\n    box-shadow: 0 0 20px #ccc;\n    background-color: #00000030;\n    padding: 20px 20px 20px 20px;\n    margin: 25%;\n}\n\n.button-Patreon {\n    margin: 10%;\n    background-color: #ffffff20;\n}\n\n.innerWrapper img {\n    margin: 10%;\n    border-radius: 15px;\n    width: 80%;\n}",
         ".LoadSave {\n    outline: none;\n    background: linear-gradient(to right, #fff5, #fff0, #0000);\n    background-size: 200% 100%;\n    background-position: 99%;\n    border-bottom: 1px solid #fff;\n    border-image: linear-gradient(to right, #fff, #fff0, #0000);\n    border-image-slice: 1;\n    text-align: left;\n}\n\n.LoadSave:hover {\n    outline: none;\n    border: 0px solid;\n    border-bottom: 1px solid #fff;\n    border-image: linear-gradient(to right, #fff, #fff0);\n    border-image-slice: 1;\n    box-shadow: none;\n    background-position: 0%;\n}\n\n.ButtonsDiv {\n    display: flex;\n    flex-direction: column;\n    width: 10%;\n}\n\n.Save {\n    position: relative;\n    transition: all .5s ease-in-out;\n}\n\n.Save::after{\n    background-image: linear-gradient(to right, #282a36, rgba(1, 1, 1, 0));\n}",
         ".SavesScreenshots {\n    height: 100%;\n    display: grid;\n    grid-template: 1fr / 1fr;\n    place-items: center;\n  }\n\n  .SavesScreenshots > * {\n    grid-column: 1 / 1;\n    grid-row: 1 / 1;\n  }",
         ".GalleryWrapper {\n  display: flex;\n  flex-direction: row;\n  margin: 20px;\n}\n\n.CategorieSelector {\n  display: flex;\n  flex-direction: column;\n  justify-content: left;\n  width: 15%;\n}\n\n.CategorieButton {\n    margin: 5px;\n    padding: 5px;\n    cursor: pointer;\n    outline: none;\n    background: linear-gradient(to right, #fff5, #fff0, #0000);\n    background-size: 200% 100%;\n    background-position: 99%;\n    border-bottom: 1px solid #fff;\n    border-image: linear-gradient(to right, #fff, #fff0, #0000);\n    border-image-slice: 1;\n    text-align: left;\n}\n\n.CategorieButton:hover {\n    outline: none;\n    border: 0px solid;\n    border-bottom: 1px solid #fff;\n    border-image: linear-gradient(to right, #fff, #fff0);\n    border-image-slice: 1;\n    box-shadow: none;\n    background-position: 0%;\n}\n\n.MainMenuButtonDiv {\n    position: fixed;\n    left: 1%;\n    bottom: 1%;\n}\n\n.ImageFrame {\n  display: flex;\n  flex-direction: column;\n  margin: 10px;\n  justify-content: left;\n  border: solid 2px #fff;\n  border-radius: 10px;\n  box-shadow: inset 0 0 20px rgba(255, 255, 255, .5), 0 0 20px rgba(255, 255, 255, .2);\n  cursor: pointer;\n  transition: all 1250ms cubic-bezier(0.19, 1, 0.22, 1);\n}\n\n.Title {\n  font-size: 20px;\n  font-weight: 400;\n  color: #fff;\n  text-align: center;\n}\n\n.GalleryImages {\n  display: flex;\n  overflow: auto;\n}\n\n.ImagesInner {\n  display: flex;\n  flex-direction: row;\n  flex-wrap: wrap;\n  justify-content: center;\n  align-items: center;\n  margin: 10px;\n}",
         ".unauthenticated {\n    display: flex;\n    flex-direction: column;\n    align-items: center;\n    justify-content: center;\n    height: 100%;\n    width: 100%;\n}\n\n.button-unauth {\n    position: fixed;\n    bottom: 0;\n}\n\nh1, h2 {\n    color: white;\n}"
     ],
     "version": 3
```

### Comparing `nerfw-0.1.3/nerfw/server/build/static/js/787.4afdcc44.chunk.js` & `nerfw-0.1.4/nerfw/server/build/static/js/787.4afdcc44.chunk.js`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/server/build/static/js/787.4afdcc44.chunk.js.map` & `nerfw-0.1.4/nerfw/server/build/static/js/787.4afdcc44.chunk.js.map`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/server/build/static/js/main.0361928c.js` & `nerfw-0.1.4/nerfw/server/build/static/js/main.0361928c.js`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/server/build/static/js/main.0361928c.js.LICENSE.txt` & `nerfw-0.1.4/nerfw/server/build/static/js/main.0361928c.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/server/build/static/js/main.0361928c.js.map` & `nerfw-0.1.4/nerfw/server/build/static/js/main.0361928c.js.map`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/server/build/static/media/PATREON_SYMBOL_1_WHITE_RGB.17310609229eef2df4c7c31535ee8843.svg` & `nerfw-0.1.4/nerfw/server/build/static/media/PATREON_SYMBOL_1_WHITE_RGB.17310609229eef2df4c7c31535ee8843.svg`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/server/build/static/media/github-mark-white.97ed8e7eef60d61ca469881dd6f34511.svg` & `nerfw-0.1.4/nerfw/server/build/static/media/github-mark-white.97ed8e7eef60d61ca469881dd6f34511.svg`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/server/gallery.py` & `nerfw-0.1.4/nerfw/server/gallery.py`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/server/login_default.py` & `nerfw-0.1.4/nerfw/server/login_default.py`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/server/login_github.py` & `nerfw-0.1.4/nerfw/server/login_github.py`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/server/login_patreon.py` & `nerfw-0.1.4/nerfw/server/login_patreon.py`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/server/password_manager.py` & `nerfw-0.1.4/nerfw/server/password_manager.py`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/server/require_token.py` & `nerfw-0.1.4/nerfw/server/require_token.py`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/server/saves_handler.py` & `nerfw-0.1.4/nerfw/server/saves_handler.py`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/server/server.py` & `nerfw-0.1.4/nerfw/server/server.py`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/server/token_handler.py` & `nerfw-0.1.4/nerfw/server/token_handler.py`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw/server/wrapper.py` & `nerfw-0.1.4/nerfw/server/wrapper.py`

 * *Files identical despite different names*

### Comparing `nerfw-0.1.3/nerfw.egg-info/PKG-INFO` & `nerfw-0.1.4/nerfw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerfw
-Version: 0.1.3
+Version: 0.1.4
 Summary: Framework for creation of web based visual novels
 Author-email: Nergan <noname.nosurname2016@yandex.ru>
 License: MIT License
         
         Copyright (c) 2021-present PyO3 Project and Contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nerfw-0.1.3/nerfw.egg-info/SOURCES.txt` & `nerfw-0.1.4/nerfw.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -49,16 +49,16 @@
 nerfw/server/build/asset-manifest.json
 nerfw/server/build/favicon.ico
 nerfw/server/build/index.html
 nerfw/server/build/logo192.png
 nerfw/server/build/logo512.png
 nerfw/server/build/manifest.json
 nerfw/server/build/robots.txt
-nerfw/server/build/static/css/main.6c3c7095.css
-nerfw/server/build/static/css/main.6c3c7095.css.map
+nerfw/server/build/static/css/main.361d15c9.css
+nerfw/server/build/static/css/main.361d15c9.css.map
 nerfw/server/build/static/js/787.4afdcc44.chunk.js
 nerfw/server/build/static/js/787.4afdcc44.chunk.js.map
 nerfw/server/build/static/js/main.0361928c.js
 nerfw/server/build/static/js/main.0361928c.js.LICENSE.txt
 nerfw/server/build/static/js/main.0361928c.js.map
 nerfw/server/build/static/media/PATREON_SYMBOL_1_WHITE_RGB.17310609229eef2df4c7c31535ee8843.svg
 nerfw/server/build/static/media/github-mark-white.97ed8e7eef60d61ca469881dd6f34511.svg
```

### Comparing `nerfw-0.1.3/pyproject.toml` & `nerfw-0.1.4/pyproject.toml`

 * *Files identical despite different names*

