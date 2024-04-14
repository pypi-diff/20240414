# Comparing `tmp/hhd-2.6.2.tar.gz` & `tmp/hhd-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hhd-2.6.2.tar", last modified: Tue Apr  9 19:21:08 2024, max compression
+gzip compressed data, was "hhd-2.6.3.tar", last modified: Sun Apr 14 20:23:14 2024, max compression
```

## Comparing `hhd-2.6.2.tar` & `hhd-2.6.3.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.075641 hhd-2.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-09 19:20:58.000000 hhd-2.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-09 19:20:58.000000 hhd-2.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    22812 2024-04-09 19:21:08.075641 hhd-2.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-09 19:20:58.000000 hhd-2.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)    22000 2024-04-09 19:20:58.000000 hhd-2.6.2/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:21:08.075641 hhd-2.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.051642 hhd-2.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.059641 hhd-2.6.2/src/hhd/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26086 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.059641 hhd-2.6.2/src/hhd/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/contrib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/contrib/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/contrib/gs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/contrib/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/contrib/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.063641 hhd-2.6.2/src/hhd/controller/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37040 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/controller/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/controller/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.063641 hhd-2.6.2/src/hhd/controller/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/controller/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/controller/lib/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/controller/lib/hid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/controller/lib/hide.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/controller/lib/ioctl.py
--rw-r--r--   0 runner    (1001) docker     (127)     7958 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/controller/lib/uhid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.063641 hhd-2.6.2/src/hhd/controller/physical/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/controller/physical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21658 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/controller/physical/evdev.py
--rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/controller/physical/hidraw.py
--rw-r--r--   0 runner    (1001) docker     (127)    20696 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/controller/physical/imu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/controller/physical/rgb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.063641 hhd-2.6.2/src/hhd/controller/virtual/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/controller/virtual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.063641 hhd-2.6.2/src/hhd/controller/virtual/dualsense/
--rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/controller/virtual/dualsense/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29110 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/controller/virtual/dualsense/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.063641 hhd-2.6.2/src/hhd/controller/virtual/sd/
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/controller/virtual/sd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/controller/virtual/sd/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.063641 hhd-2.6.2/src/hhd/controller/virtual/uinput/
--rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/controller/virtual/uinput/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/controller/virtual/uinput/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.055642 hhd-2.6.2/src/hhd/device/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.063641 hhd-2.6.2/src/hhd/device/generic/
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/device/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/device/generic/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/device/generic/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/device/generic/controllers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.055642 hhd-2.6.2/src/hhd/device/gpd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.067642 hhd-2.6.2/src/hhd/device/gpd/win/
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/device/gpd/win/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/device/gpd/win/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/device/gpd/win/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/device/gpd/win/controllers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.067642 hhd-2.6.2/src/hhd/device/legion_go/
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/device/legion_go/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17892 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/device/legion_go/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/device/legion_go/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/device/legion_go/controllers.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/device/legion_go/gyro_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/device/legion_go/hid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.067642 hhd-2.6.2/src/hhd/device/orange_pi/
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/device/orange_pi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/device/orange_pi/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/device/orange_pi/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/device/orange_pi/controllers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.067642 hhd-2.6.2/src/hhd/device/rog_ally/
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/device/rog_ally/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10640 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/device/rog_ally/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/device/rog_ally/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/device/rog_ally/controllers.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/device/rog_ally/hid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.067642 hhd-2.6.2/src/hhd/http/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15114 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/http/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/http/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/http/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.067642 hhd-2.6.2/src/hhd/http/static/
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/http/static/index.js
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/http/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.067642 hhd-2.6.2/src/hhd/i18n/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/i18n/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.055642 hhd-2.6.2/src/hhd/i18n/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.071642 hhd-2.6.2/src/hhd/i18n/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12310 2024-04-09 19:21:05.000000 hhd-2.6.2/src/hhd/i18n/pt/LC_MESSAGES/adjustor.mo
--rw-r--r--   0 runner    (1001) docker     (127)    22062 2024-04-09 19:21:05.000000 hhd-2.6.2/src/hhd/i18n/pt/LC_MESSAGES/hhd.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.055642 hhd-2.6.2/src/hhd/i18n/zh/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.071642 hhd-2.6.2/src/hhd/i18n/zh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-04-09 19:21:05.000000 hhd-2.6.2/src/hhd/i18n/zh/LC_MESSAGES/adjustor.mo
--rw-r--r--   0 runner    (1001) docker     (127)    16335 2024-04-09 19:21:05.000000 hhd-2.6.2/src/hhd/i18n/zh/LC_MESSAGES/hhd.mo
--rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.071642 hhd-2.6.2/src/hhd/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/plugins/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.071642 hhd-2.6.2/src/hhd/plugins/display/
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/plugins/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/plugins/display/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/plugins/gyro.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/plugins/inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/plugins/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/plugins/outputs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.071642 hhd-2.6.2/src/hhd/plugins/overlay/
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/plugins/overlay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/plugins/overlay/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/plugins/overlay/controllers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/plugins/overlay/overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/plugins/overlay/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)    12985 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/plugins/overlay/x11.py
--rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/plugins/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.075641 hhd-2.6.2/src/hhd/plugins/powerbutton/
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/plugins/powerbutton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/plugins/powerbutton/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/plugins/powerbutton/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/plugins/powerbutton/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)    22188 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/plugins/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/plugins/touchpad.yml
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/plugins/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/sections.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-09 19:20:58.000000 hhd-2.6.2/src/hhd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.075641 hhd-2.6.2/src/hhd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22812 2024-04-09 19:21:08.000000 hhd-2.6.2/src/hhd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-09 19:21:08.000000 hhd-2.6.2/src/hhd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:21:08.000000 hhd-2.6.2/src/hhd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-09 19:21:08.000000 hhd-2.6.2/src/hhd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 19:21:08.000000 hhd-2.6.2/src/hhd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-09 19:21:08.000000 hhd-2.6.2/src/hhd.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.055642 hhd-2.6.2/usr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.055642 hhd-2.6.2/usr/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.075641 hhd-2.6.2/usr/lib/modules-load.d/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 19:20:58.000000 hhd-2.6.2/usr/lib/modules-load.d/hhd-user.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.055642 hhd-2.6.2/usr/lib/systemd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.075641 hhd-2.6.2/usr/lib/systemd/system/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-09 19:20:58.000000 hhd-2.6.2/usr/lib/systemd/system/hhd@.service
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-09 19:20:58.000000 hhd-2.6.2/usr/lib/systemd/system/hhd_local@.service
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.075641 hhd-2.6.2/usr/lib/systemd/user/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-09 19:20:58.000000 hhd-2.6.2/usr/lib/systemd/user/hhd-user.service
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.055642 hhd-2.6.2/usr/lib/udev/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.075641 hhd-2.6.2/usr/lib/udev/hwdb.d/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-09 19:20:58.000000 hhd-2.6.2/usr/lib/udev/hwdb.d/83-hhd.hwdb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:21:08.075641 hhd-2.6.2/usr/lib/udev/rules.d/
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-09 19:20:58.000000 hhd-2.6.2/usr/lib/udev/rules.d/83-hhd-user.rules
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-09 19:20:58.000000 hhd-2.6.2/usr/lib/udev/rules.d/83-hhd.rules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.671635 hhd-2.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-14 20:23:02.000000 hhd-2.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-14 20:23:02.000000 hhd-2.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    22812 2024-04-14 20:23:14.671635 hhd-2.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-14 20:23:02.000000 hhd-2.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    22000 2024-04-14 20:23:02.000000 hhd-2.6.3/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 20:23:14.671635 hhd-2.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.647635 hhd-2.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.651635 hhd-2.6.3/src/hhd/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26086 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.655635 hhd-2.6.3/src/hhd/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/contrib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/contrib/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/contrib/gs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/contrib/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/contrib/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.655635 hhd-2.6.3/src/hhd/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37040 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/controller/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/controller/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.659635 hhd-2.6.3/src/hhd/controller/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/controller/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/controller/lib/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/controller/lib/hid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/controller/lib/hide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/controller/lib/ioctl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7958 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/controller/lib/uhid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.659635 hhd-2.6.3/src/hhd/controller/physical/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/controller/physical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21658 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/controller/physical/evdev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/controller/physical/hidraw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20696 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/controller/physical/imu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/controller/physical/rgb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.659635 hhd-2.6.3/src/hhd/controller/virtual/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/controller/virtual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.659635 hhd-2.6.3/src/hhd/controller/virtual/dualsense/
+-rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/controller/virtual/dualsense/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29110 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/controller/virtual/dualsense/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.659635 hhd-2.6.3/src/hhd/controller/virtual/sd/
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/controller/virtual/sd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/controller/virtual/sd/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.659635 hhd-2.6.3/src/hhd/controller/virtual/uinput/
+-rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/controller/virtual/uinput/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/controller/virtual/uinput/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.647635 hhd-2.6.3/src/hhd/device/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.659635 hhd-2.6.3/src/hhd/device/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/device/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/device/generic/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/device/generic/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/device/generic/controllers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.647635 hhd-2.6.3/src/hhd/device/gpd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.659635 hhd-2.6.3/src/hhd/device/gpd/win/
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/device/gpd/win/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/device/gpd/win/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/device/gpd/win/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/device/gpd/win/controllers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.663635 hhd-2.6.3/src/hhd/device/legion_go/
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/device/legion_go/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17892 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/device/legion_go/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/device/legion_go/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/device/legion_go/controllers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/device/legion_go/gyro_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/device/legion_go/hid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.663635 hhd-2.6.3/src/hhd/device/orange_pi/
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/device/orange_pi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/device/orange_pi/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/device/orange_pi/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/device/orange_pi/controllers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.663635 hhd-2.6.3/src/hhd/device/rog_ally/
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/device/rog_ally/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10604 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/device/rog_ally/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/device/rog_ally/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/device/rog_ally/controllers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/device/rog_ally/hid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.663635 hhd-2.6.3/src/hhd/http/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15114 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/http/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/http/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/http/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.663635 hhd-2.6.3/src/hhd/http/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/http/static/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/http/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.663635 hhd-2.6.3/src/hhd/i18n/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/i18n/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.647635 hhd-2.6.3/src/hhd/i18n/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.667635 hhd-2.6.3/src/hhd/i18n/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12310 2024-04-14 20:23:11.000000 hhd-2.6.3/src/hhd/i18n/pt/LC_MESSAGES/adjustor.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    22062 2024-04-14 20:23:11.000000 hhd-2.6.3/src/hhd/i18n/pt/LC_MESSAGES/hhd.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.647635 hhd-2.6.3/src/hhd/i18n/zh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.667635 hhd-2.6.3/src/hhd/i18n/zh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-04-14 20:23:11.000000 hhd-2.6.3/src/hhd/i18n/zh/LC_MESSAGES/adjustor.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    16357 2024-04-14 20:23:11.000000 hhd-2.6.3/src/hhd/i18n/zh/LC_MESSAGES/hhd.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.667635 hhd-2.6.3/src/hhd/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/plugins/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.667635 hhd-2.6.3/src/hhd/plugins/display/
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/plugins/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/plugins/display/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/plugins/gyro.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/plugins/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/plugins/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/plugins/outputs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.667635 hhd-2.6.3/src/hhd/plugins/overlay/
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/plugins/overlay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/plugins/overlay/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/plugins/overlay/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/plugins/overlay/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/plugins/overlay/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    12985 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/plugins/overlay/x11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/plugins/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.671635 hhd-2.6.3/src/hhd/plugins/powerbutton/
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/plugins/powerbutton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/plugins/powerbutton/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/plugins/powerbutton/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/plugins/powerbutton/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    22188 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/plugins/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/plugins/touchpad.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/plugins/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/sections.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-14 20:23:02.000000 hhd-2.6.3/src/hhd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.671635 hhd-2.6.3/src/hhd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22812 2024-04-14 20:23:14.000000 hhd-2.6.3/src/hhd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-14 20:23:14.000000 hhd-2.6.3/src/hhd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 20:23:14.000000 hhd-2.6.3/src/hhd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-14 20:23:14.000000 hhd-2.6.3/src/hhd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-14 20:23:14.000000 hhd-2.6.3/src/hhd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-14 20:23:14.000000 hhd-2.6.3/src/hhd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.651635 hhd-2.6.3/usr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.651635 hhd-2.6.3/usr/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.671635 hhd-2.6.3/usr/lib/modules-load.d/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-14 20:23:02.000000 hhd-2.6.3/usr/lib/modules-load.d/hhd-user.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.651635 hhd-2.6.3/usr/lib/systemd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.671635 hhd-2.6.3/usr/lib/systemd/system/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-14 20:23:02.000000 hhd-2.6.3/usr/lib/systemd/system/hhd@.service
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-14 20:23:02.000000 hhd-2.6.3/usr/lib/systemd/system/hhd_local@.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.671635 hhd-2.6.3/usr/lib/systemd/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-14 20:23:02.000000 hhd-2.6.3/usr/lib/systemd/user/hhd-user.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.651635 hhd-2.6.3/usr/lib/udev/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.671635 hhd-2.6.3/usr/lib/udev/hwdb.d/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-14 20:23:02.000000 hhd-2.6.3/usr/lib/udev/hwdb.d/83-hhd.hwdb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:23:14.671635 hhd-2.6.3/usr/lib/udev/rules.d/
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-14 20:23:02.000000 hhd-2.6.3/usr/lib/udev/rules.d/83-hhd-user.rules
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-14 20:23:02.000000 hhd-2.6.3/usr/lib/udev/rules.d/83-hhd.rules
```

### Comparing `hhd-2.6.2/LICENSE` & `hhd-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/PKG-INFO` & `hhd-2.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhd
-Version: 2.6.2
+Version: 2.6.3
 Summary: Handheld Daemon, a tool for configuring handheld devices.
 Author-email: Kapenekakis Antheas <pypi@antheas.dev>
 Project-URL: Homepage, https://github.com/hhd-dev/hhd
 Project-URL: Bug Tracker, https://github.com/hhd-dev/hhd/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `hhd-2.6.2/pyproject.toml` & `hhd-2.6.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hhd"
-version = "2.6.2"
+version = "2.6.3"
 authors = [
   { name="Kapenekakis Antheas", email="pypi@antheas.dev" },
 ]
 description = "Handheld Daemon, a tool for configuring handheld devices."
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `hhd-2.6.2/readme.md` & `hhd-2.6.3/readme.md`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/__main__.py` & `hhd-2.6.3/src/hhd/__main__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/contrib/dev.py` & `hhd-2.6.3/src/hhd/contrib/dev.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/contrib/gs.py` & `hhd-2.6.3/src/hhd/contrib/gs.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/contrib/i18n.py` & `hhd-2.6.3/src/hhd/contrib/i18n.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/contrib/main.py` & `hhd-2.6.3/src/hhd/contrib/main.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/controller/__init__.py` & `hhd-2.6.3/src/hhd/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/controller/base.py` & `hhd-2.6.3/src/hhd/controller/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/controller/const.py` & `hhd-2.6.3/src/hhd/controller/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/controller/lib/common.py` & `hhd-2.6.3/src/hhd/controller/lib/common.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/controller/lib/hid.py` & `hhd-2.6.3/src/hhd/controller/lib/hid.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/controller/lib/hide.py` & `hhd-2.6.3/src/hhd/controller/lib/hide.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/controller/lib/ioctl.py` & `hhd-2.6.3/src/hhd/controller/lib/ioctl.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/controller/lib/uhid.py` & `hhd-2.6.3/src/hhd/controller/lib/uhid.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/controller/physical/evdev.py` & `hhd-2.6.3/src/hhd/controller/physical/evdev.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/controller/physical/hidraw.py` & `hhd-2.6.3/src/hhd/controller/physical/hidraw.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/controller/physical/imu.py` & `hhd-2.6.3/src/hhd/controller/physical/imu.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/controller/physical/rgb.py` & `hhd-2.6.3/src/hhd/controller/physical/rgb.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/controller/virtual/dualsense/__init__.py` & `hhd-2.6.3/src/hhd/controller/virtual/dualsense/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/controller/virtual/dualsense/const.py` & `hhd-2.6.3/src/hhd/controller/virtual/dualsense/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/controller/virtual/sd/__init__.py` & `hhd-2.6.3/src/hhd/controller/virtual/sd/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/controller/virtual/sd/const.py` & `hhd-2.6.3/src/hhd/controller/virtual/sd/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/controller/virtual/uinput/__init__.py` & `hhd-2.6.3/src/hhd/controller/virtual/uinput/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/controller/virtual/uinput/const.py` & `hhd-2.6.3/src/hhd/controller/virtual/uinput/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/device/generic/__init__.py` & `hhd-2.6.3/src/hhd/device/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/device/generic/base.py` & `hhd-2.6.3/src/hhd/device/generic/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/device/generic/const.py` & `hhd-2.6.3/src/hhd/device/generic/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/device/generic/controllers.yml` & `hhd-2.6.3/src/hhd/device/generic/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/device/gpd/win/__init__.py` & `hhd-2.6.3/src/hhd/device/gpd/win/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/device/gpd/win/base.py` & `hhd-2.6.3/src/hhd/device/gpd/win/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/device/gpd/win/const.py` & `hhd-2.6.3/src/hhd/device/gpd/win/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/device/gpd/win/controllers.yml` & `hhd-2.6.3/src/hhd/device/gpd/win/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/device/legion_go/__init__.py` & `hhd-2.6.3/src/hhd/device/legion_go/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/device/legion_go/base.py` & `hhd-2.6.3/src/hhd/device/legion_go/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/device/legion_go/const.py` & `hhd-2.6.3/src/hhd/device/legion_go/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/device/legion_go/controllers.yml` & `hhd-2.6.3/src/hhd/device/legion_go/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/device/legion_go/gyro_fix.py` & `hhd-2.6.3/src/hhd/device/legion_go/gyro_fix.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/device/legion_go/hid.py` & `hhd-2.6.3/src/hhd/device/legion_go/hid.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/device/orange_pi/__init__.py` & `hhd-2.6.3/src/hhd/device/orange_pi/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/device/orange_pi/base.py` & `hhd-2.6.3/src/hhd/device/orange_pi/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/device/orange_pi/const.py` & `hhd-2.6.3/src/hhd/device/orange_pi/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/device/orange_pi/controllers.yml` & `hhd-2.6.3/src/hhd/device/orange_pi/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/device/rog_ally/__init__.py` & `hhd-2.6.3/src/hhd/device/rog_ally/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/device/rog_ally/base.py` & `hhd-2.6.3/src/hhd/device/rog_ally/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import time
 from threading import Event as TEvent
 from typing import Literal, Sequence
 
 from hhd.controller import Axis, Event, Multiplexer, can_read
 from hhd.controller.physical.evdev import B as EC
 from hhd.controller.physical.evdev import GenericGamepadEvdev, enumerate_evs
-from hhd.controller.physical.hidraw import GenericGamepadHidraw
+from hhd.controller.physical.hidraw import GenericGamepadHidraw, enumerate_unique
 from hhd.controller.physical.imu import CombinedImu, HrtimerTrigger
 from hhd.plugins import Config, Context, Emitter, get_outputs
 
 from .hid import Brightness, RgbCallback, switch_mode
 
 SELECT_TIMEOUT = 1
 
@@ -132,33 +132,33 @@
 
 
 def plugin_run(
     conf: Config, emit: Emitter, context: Context, should_exit: TEvent, updated: TEvent
 ):
     init = time.perf_counter()
     repeated_fail = False
+    first = True
     while not should_exit.is_set():
         try:
-            first = True
-            while True:
-                gamepad_devs = enumerate_evs(vid=GAMEPAD_VID)
-                asus_devs = enumerate_evs(vid=ASUS_VID)
-                if not gamepad_devs or not asus_devs:
-                    if first:
-                        first = False
-                        logger.warning(f"Ally controller not found, waiting...")
-                    time.sleep(FIND_DELAY)
-                else:
-                    break
+            gamepad_devs = enumerate_evs(vid=GAMEPAD_VID)
+            nkey_devs = enumerate_unique(vid=ASUS_VID)
+            if not gamepad_devs or not nkey_devs:
+                if first:
+                    first = False
+                    logger.warning(f"Ally controller not found, waiting...")
+                time.sleep(FIND_DELAY)
+                continue
+
             logger.info("Launching emulated controller.")
             updated.clear()
             init = time.perf_counter()
             controller_loop(conf.copy(), should_exit, updated, emit)
             repeated_fail = False
         except Exception as e:
+            first = True
             failed_fast = init + LONGER_ERROR_MARGIN > time.perf_counter()
             sleep_time = (
                 LONGER_ERROR_DELAY if repeated_fail and failed_fast else ERROR_DELAY
             )
             repeated_fail = failed_fast
             logger.error(f"Received the following error:\n{type(e)}: {e}")
             logger.error(
```

### Comparing `hhd-2.6.2/src/hhd/device/rog_ally/const.py` & `hhd-2.6.3/src/hhd/device/rog_ally/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/device/rog_ally/controllers.yml` & `hhd-2.6.3/src/hhd/device/rog_ally/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/device/rog_ally/hid.py` & `hhd-2.6.3/src/hhd/device/rog_ally/hid.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/http/api.py` & `hhd-2.6.3/src/hhd/http/api.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/http/i18n.py` & `hhd-2.6.3/src/hhd/http/i18n.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/http/index.html` & `hhd-2.6.3/src/hhd/http/index.html`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/http/static/index.js` & `hhd-2.6.3/src/hhd/http/static/index.js`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/i18n/pt/LC_MESSAGES/adjustor.mo` & `hhd-2.6.3/src/hhd/i18n/pt/LC_MESSAGES/adjustor.mo`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/i18n/pt/LC_MESSAGES/hhd.mo` & `hhd-2.6.3/src/hhd/i18n/pt/LC_MESSAGES/hhd.mo`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/i18n/zh/LC_MESSAGES/adjustor.mo` & `hhd-2.6.3/src/hhd/i18n/zh/LC_MESSAGES/adjustor.mo`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/i18n/zh/LC_MESSAGES/hhd.mo` & `hhd-2.6.3/src/hhd/i18n/zh/LC_MESSAGES/hhd.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -462,22 +462,22 @@
 msgid "Stretch"
 msgstr "拉伸"
 
 msgid "Swap Legion with Start/Select"
 msgstr "交换 Start/Select 按钮"
 
 msgid "Swap ROG and Start/Select"
-msgstr "交换 Start/Select 按钮"
+msgstr "交换 ROG Start/Select 按钮"
 
 msgid "Swaps A with B and X with Y."
 msgstr "A 与 B 交换, X 与 Y 交换"
 
 msgid ""
 "Swaps the Armory Crate and Command center buttons with start and select."
-msgstr "交换 Legion Go 的 Start/Select 按钮"
+msgstr "交换 Armory Crate/Command center 与 Start/Select 按钮"
 
 msgid "Swaps the legion buttons with start select."
 msgstr "交换 Legion Go 的 Start/Select 按钮"
 
 msgid "System"
 msgstr "系统"
```

### Comparing `hhd-2.6.2/src/hhd/logging.py` & `hhd-2.6.3/src/hhd/logging.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/plugins/__init__.py` & `hhd-2.6.3/src/hhd/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/plugins/conf.py` & `hhd-2.6.3/src/hhd/plugins/conf.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/plugins/display/__init__.py` & `hhd-2.6.3/src/hhd/plugins/display/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/plugins/gyro.yml` & `hhd-2.6.3/src/hhd/plugins/gyro.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/plugins/inputs.py` & `hhd-2.6.3/src/hhd/plugins/inputs.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/plugins/outputs.py` & `hhd-2.6.3/src/hhd/plugins/outputs.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/plugins/outputs.yml` & `hhd-2.6.3/src/hhd/plugins/outputs.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/plugins/overlay/__init__.py` & `hhd-2.6.3/src/hhd/plugins/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/plugins/overlay/base.py` & `hhd-2.6.3/src/hhd/plugins/overlay/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/plugins/overlay/controllers.py` & `hhd-2.6.3/src/hhd/plugins/overlay/controllers.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/plugins/overlay/overlay.py` & `hhd-2.6.3/src/hhd/plugins/overlay/overlay.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/plugins/overlay/x11.py` & `hhd-2.6.3/src/hhd/plugins/overlay/x11.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/plugins/plugin.py` & `hhd-2.6.3/src/hhd/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/plugins/powerbutton/__init__.py` & `hhd-2.6.3/src/hhd/plugins/powerbutton/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/plugins/powerbutton/base.py` & `hhd-2.6.3/src/hhd/plugins/powerbutton/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/plugins/powerbutton/const.py` & `hhd-2.6.3/src/hhd/plugins/powerbutton/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/plugins/settings.py` & `hhd-2.6.3/src/hhd/plugins/settings.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/plugins/touchpad.yml` & `hhd-2.6.3/src/hhd/plugins/touchpad.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/plugins/utils.py` & `hhd-2.6.3/src/hhd/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/settings.yml` & `hhd-2.6.3/src/hhd/settings.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd/utils.py` & `hhd-2.6.3/src/hhd/utils.py`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/src/hhd.egg-info/PKG-INFO` & `hhd-2.6.3/src/hhd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhd
-Version: 2.6.2
+Version: 2.6.3
 Summary: Handheld Daemon, a tool for configuring handheld devices.
 Author-email: Kapenekakis Antheas <pypi@antheas.dev>
 Project-URL: Homepage, https://github.com/hhd-dev/hhd
 Project-URL: Bug Tracker, https://github.com/hhd-dev/hhd/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `hhd-2.6.2/src/hhd.egg-info/SOURCES.txt` & `hhd-2.6.3/src/hhd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/usr/lib/udev/hwdb.d/83-hhd.hwdb` & `hhd-2.6.3/usr/lib/udev/hwdb.d/83-hhd.hwdb`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/usr/lib/udev/rules.d/83-hhd-user.rules` & `hhd-2.6.3/usr/lib/udev/rules.d/83-hhd-user.rules`

 * *Files identical despite different names*

### Comparing `hhd-2.6.2/usr/lib/udev/rules.d/83-hhd.rules` & `hhd-2.6.3/usr/lib/udev/rules.d/83-hhd.rules`

 * *Files identical despite different names*

