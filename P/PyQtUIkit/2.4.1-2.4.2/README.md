# Comparing `tmp/PyQtUIkit-2.4.1.tar.gz` & `tmp/PyQtUIkit-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQtUIkit-2.4.1.tar", last modified: Fri Apr 12 09:56:51 2024, max compression
+gzip compressed data, was "PyQtUIkit-2.4.2.tar", last modified: Sat Apr 13 15:35:33 2024, max compression
```

## Comparing `PyQtUIkit-2.4.1.tar` & `PyQtUIkit-2.4.2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 09:56:51.634648 PyQtUIkit-2.4.1/
--rw-rw-rw-   0        0        0     1090 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/LICENSE
--rw-rw-rw-   0        0        0     2938 2024-04-12 09:56:51.634648 PyQtUIkit-2.4.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-12 09:56:51.587775 PyQtUIkit-2.4.1/PyQtUIkit/
--rw-rw-rw-   0        0        0       49 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/__init__.py
--rw-rw-rw-   0        0        0     3896 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/_icons.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:56:51.603398 PyQtUIkit-2.4.1/PyQtUIkit/builder/
--rw-rw-rw-   0        0        0     1116 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/builder/__init__.py
--rw-rw-rw-   0        0        0     1825 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/builder/builder_class.py
--rw-rw-rw-   0        0        0     1383 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/builder/builder_module.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:56:51.603398 PyQtUIkit-2.4.1/PyQtUIkit/core/
--rw-rw-rw-   0        0        0       84 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/core/__init__.py
--rw-rw-rw-   0        0        0       19 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/core/_version.py
--rw-rw-rw-   0        0        0     1503 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/core/font.py
--rw-rw-rw-   0        0        0     1019 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/core/icon.py
--rw-rw-rw-   0        0        0     4655 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/core/properties.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:56:51.619023 PyQtUIkit-2.4.1/PyQtUIkit/fonts/
--rw-rw-rw-   0        0        0   168060 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/fonts/Roboto-Black.ttf
--rw-rw-rw-   0        0        0   174108 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
--rw-rw-rw-   0        0        0   167336 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/fonts/Roboto-Bold.ttf
--rw-rw-rw-   0        0        0   171508 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
--rw-rw-rw-   0        0        0   170504 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/fonts/Roboto-Italic.ttf
--rw-rw-rw-   0        0        0   167000 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/fonts/Roboto-Light.ttf
--rw-rw-rw-   0        0        0   173172 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/fonts/Roboto-LightItalic.ttf
--rw-rw-rw-   0        0        0   168644 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/fonts/Roboto-Medium.ttf
--rw-rw-rw-   0        0        0   173416 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
--rw-rw-rw-   0        0        0   168260 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/fonts/Roboto-Regular.ttf
--rw-rw-rw-   0        0        0   168488 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/fonts/Roboto-Thin.ttf
--rw-rw-rw-   0        0        0   172860 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
--rw-rw-rw-   0        0        0    87392 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/fonts/RobotoMono-Bold.ttf
--rw-rw-rw-   0        0        0    94636 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
--rw-rw-rw-   0        0        0    88248 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
--rw-rw-rw-   0        0        0    94016 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
--rw-rw-rw-   0        0        0    94372 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/fonts/RobotoMono-Italic.ttf
--rw-rw-rw-   0        0        0    87980 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/fonts/RobotoMono-Light.ttf
--rw-rw-rw-   0        0        0    94256 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
--rw-rw-rw-   0        0        0    87172 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/fonts/RobotoMono-Medium.ttf
--rw-rw-rw-   0        0        0    94412 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
--rw-rw-rw-   0        0        0    87236 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/fonts/RobotoMono-Regular.ttf
--rw-rw-rw-   0        0        0    87496 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
--rw-rw-rw-   0        0        0    94508 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
--rw-rw-rw-   0        0        0    88288 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/fonts/RobotoMono-Thin.ttf
--rw-rw-rw-   0        0        0    93588 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
-drwxrwxrwx   0        0        0        0 2024-04-12 09:56:51.619023 PyQtUIkit-2.4.1/PyQtUIkit/themes/
--rw-rw-rw-   0        0        0     2180 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/themes/__init__.py
--rw-rw-rw-   0        0        0     5879 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/themes/builtin_themes.py
--rw-rw-rw-   0        0        0  2340473 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/themes/icons.py
--rw-rw-rw-   0        0        0     1470 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/themes/svg.py
--rw-rw-rw-   0        0        0     1402 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/themes/theme.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:56:51.634648 PyQtUIkit-2.4.1/PyQtUIkit/widgets/
--rw-rw-rw-   0        0        0     1626 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/__init__.py
--rw-rw-rw-   0        0        0     3515 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/_widget.py
--rw-rw-rw-   0        0        0     1359 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/application.py
--rw-rw-rw-   0        0        0     7833 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/button.py
--rw-rw-rw-   0        0        0     2788 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/checkbox.py
--rw-rw-rw-   0        0        0    10059 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/combo_box.py
--rw-rw-rw-   0        0        0     7021 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/dialog.py
--rw-rw-rw-   0        0        0     5807 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/flow_layout.py
--rw-rw-rw-   0        0        0     2280 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/group.py
--rw-rw-rw-   0        0        0     4293 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/hbox_layout.py
--rw-rw-rw-   0        0        0     1578 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/icon_widget.py
--rw-rw-rw-   0        0        0     1100 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/label.py
--rw-rw-rw-   0        0        0     1487 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/line_edit.py
--rw-rw-rw-   0        0        0     3448 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/list_widget.py
--rw-rw-rw-   0        0        0     1424 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/main_window.py
--rw-rw-rw-   0        0        0     3302 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/menu.py
--rw-rw-rw-   0        0        0     4336 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/menu_bar.py
--rw-rw-rw-   0        0        0     7084 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/navigation.py
--rw-rw-rw-   0        0        0     2647 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     6683 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/radio.py
--rw-rw-rw-   0        0        0     3881 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/scroll_area.py
--rw-rw-rw-   0        0        0     1486 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/separator.py
--rw-rw-rw-   0        0        0     7515 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/spin_box.py
--rw-rw-rw-   0        0        0     3580 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/spinner.py
--rw-rw-rw-   0        0        0    13353 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/tab_bar.py
--rw-rw-rw-   0        0        0     1218 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/tabs.py
--rw-rw-rw-   0        0        0     2167 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/text_edit.py
--rw-rw-rw-   0        0        0     4465 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/toggle.py
--rw-rw-rw-   0        0        0    17251 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/tree_widget.py
--rw-rw-rw-   0        0        0     4620 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/PyQtUIkit/widgets/vbox_layout.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:56:51.587775 PyQtUIkit-2.4.1/PyQtUIkit.egg-info/
--rw-rw-rw-   0        0        0     2938 2024-04-12 09:56:51.000000 PyQtUIkit-2.4.1/PyQtUIkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2537 2024-04-12 09:56:51.000000 PyQtUIkit-2.4.1/PyQtUIkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 09:56:51.000000 PyQtUIkit-2.4.1/PyQtUIkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-12 09:56:51.000000 PyQtUIkit-2.4.1/PyQtUIkit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2024-04-12 09:56:51.000000 PyQtUIkit-2.4.1/PyQtUIkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-12 09:56:51.000000 PyQtUIkit-2.4.1/PyQtUIkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 09:56:51.634648 PyQtUIkit-2.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1411 2024-04-12 09:56:09.000000 PyQtUIkit-2.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:35:33.290948 PyQtUIkit-2.4.2/
+-rw-rw-rw-   0        0        0     1090 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/LICENSE
+-rw-rw-rw-   0        0        0     2938 2024-04-13 15:35:33.290948 PyQtUIkit-2.4.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-13 15:35:33.244097 PyQtUIkit-2.4.2/PyQtUIkit/
+-rw-rw-rw-   0        0        0       49 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/__init__.py
+-rw-rw-rw-   0        0        0     3896 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/_icons.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:35:33.259697 PyQtUIkit-2.4.2/PyQtUIkit/builder/
+-rw-rw-rw-   0        0        0     1116 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/builder/__init__.py
+-rw-rw-rw-   0        0        0     1825 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/builder/builder_class.py
+-rw-rw-rw-   0        0        0     1383 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/builder/builder_module.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:35:33.259697 PyQtUIkit-2.4.2/PyQtUIkit/core/
+-rw-rw-rw-   0        0        0       84 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/core/__init__.py
+-rw-rw-rw-   0        0        0       19 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/core/_version.py
+-rw-rw-rw-   0        0        0     1503 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/core/font.py
+-rw-rw-rw-   0        0        0     1019 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/core/icon.py
+-rw-rw-rw-   0        0        0     4655 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/core/properties.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:35:33.275321 PyQtUIkit-2.4.2/PyQtUIkit/fonts/
+-rw-rw-rw-   0        0        0   168060 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-Black.ttf
+-rw-rw-rw-   0        0        0   174108 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
+-rw-rw-rw-   0        0        0   167336 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-Bold.ttf
+-rw-rw-rw-   0        0        0   171508 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
+-rw-rw-rw-   0        0        0   170504 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-Italic.ttf
+-rw-rw-rw-   0        0        0   167000 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-Light.ttf
+-rw-rw-rw-   0        0        0   173172 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-LightItalic.ttf
+-rw-rw-rw-   0        0        0   168644 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-Medium.ttf
+-rw-rw-rw-   0        0        0   173416 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
+-rw-rw-rw-   0        0        0   168260 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-Regular.ttf
+-rw-rw-rw-   0        0        0   168488 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-Thin.ttf
+-rw-rw-rw-   0        0        0   172860 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
+-rw-rw-rw-   0        0        0    87392 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-Bold.ttf
+-rw-rw-rw-   0        0        0    94636 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
+-rw-rw-rw-   0        0        0    88248 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
+-rw-rw-rw-   0        0        0    94016 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
+-rw-rw-rw-   0        0        0    94372 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-Italic.ttf
+-rw-rw-rw-   0        0        0    87980 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-Light.ttf
+-rw-rw-rw-   0        0        0    94256 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
+-rw-rw-rw-   0        0        0    87172 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-Medium.ttf
+-rw-rw-rw-   0        0        0    94412 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
+-rw-rw-rw-   0        0        0    87236 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-Regular.ttf
+-rw-rw-rw-   0        0        0    87496 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
+-rw-rw-rw-   0        0        0    94508 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
+-rw-rw-rw-   0        0        0    88288 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-Thin.ttf
+-rw-rw-rw-   0        0        0    93588 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
+drwxrwxrwx   0        0        0        0 2024-04-13 15:35:33.275321 PyQtUIkit-2.4.2/PyQtUIkit/themes/
+-rw-rw-rw-   0        0        0     2180 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/themes/__init__.py
+-rw-rw-rw-   0        0        0     5879 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/themes/builtin_themes.py
+-rw-rw-rw-   0        0        0  2340473 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/themes/icons.py
+-rw-rw-rw-   0        0        0     1470 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/themes/svg.py
+-rw-rw-rw-   0        0        0     1402 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/themes/theme.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:35:33.290948 PyQtUIkit-2.4.2/PyQtUIkit/widgets/
+-rw-rw-rw-   0        0        0     1626 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3515 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/_widget.py
+-rw-rw-rw-   0        0        0     1359 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/application.py
+-rw-rw-rw-   0        0        0     7833 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/button.py
+-rw-rw-rw-   0        0        0     2788 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/checkbox.py
+-rw-rw-rw-   0        0        0    10059 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/combo_box.py
+-rw-rw-rw-   0        0        0     7021 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/dialog.py
+-rw-rw-rw-   0        0        0     5807 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/flow_layout.py
+-rw-rw-rw-   0        0        0     2280 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/group.py
+-rw-rw-rw-   0        0        0     4293 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/hbox_layout.py
+-rw-rw-rw-   0        0        0     1578 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0     1100 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/label.py
+-rw-rw-rw-   0        0        0     1487 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     3448 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/list_widget.py
+-rw-rw-rw-   0        0        0     1424 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/main_window.py
+-rw-rw-rw-   0        0        0     3302 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/menu.py
+-rw-rw-rw-   0        0        0     4336 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/menu_bar.py
+-rw-rw-rw-   0        0        0     7084 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/navigation.py
+-rw-rw-rw-   0        0        0     2647 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     6683 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/radio.py
+-rw-rw-rw-   0        0        0     3881 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0     1486 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/separator.py
+-rw-rw-rw-   0        0        0     7515 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     3580 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/spinner.py
+-rw-rw-rw-   0        0        0    13353 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/tab_bar.py
+-rw-rw-rw-   0        0        0     1218 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/tabs.py
+-rw-rw-rw-   0        0        0     2167 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/text_edit.py
+-rw-rw-rw-   0        0        0     4465 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/toggle.py
+-rw-rw-rw-   0        0        0    16120 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/tree_widget.py
+-rw-rw-rw-   0        0        0     4620 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/vbox_layout.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:35:33.259697 PyQtUIkit-2.4.2/PyQtUIkit.egg-info/
+-rw-rw-rw-   0        0        0     2938 2024-04-13 15:35:33.000000 PyQtUIkit-2.4.2/PyQtUIkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2537 2024-04-13 15:35:33.000000 PyQtUIkit-2.4.2/PyQtUIkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 15:35:33.000000 PyQtUIkit-2.4.2/PyQtUIkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-13 15:35:33.000000 PyQtUIkit-2.4.2/PyQtUIkit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2024-04-13 15:35:33.000000 PyQtUIkit-2.4.2/PyQtUIkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-13 15:35:33.000000 PyQtUIkit-2.4.2/PyQtUIkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-13 15:35:33.290948 PyQtUIkit-2.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1411 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/setup.py
```

### Comparing `PyQtUIkit-2.4.1/LICENSE` & `PyQtUIkit-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PKG-INFO` & `PyQtUIkit-2.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.4.1
+Version: 2.4.2
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/_icons.py` & `PyQtUIkit-2.4.2/PyQtUIkit/_icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/builder/__init__.py` & `PyQtUIkit-2.4.2/PyQtUIkit/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/builder/builder_class.py` & `PyQtUIkit-2.4.2/PyQtUIkit/builder/builder_class.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/builder/builder_module.py` & `PyQtUIkit-2.4.2/PyQtUIkit/builder/builder_module.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/core/font.py` & `PyQtUIkit-2.4.2/PyQtUIkit/core/font.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/core/icon.py` & `PyQtUIkit-2.4.2/PyQtUIkit/core/icon.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/core/properties.py` & `PyQtUIkit-2.4.2/PyQtUIkit/core/properties.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/fonts/Roboto-Black.ttf` & `PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/fonts/Roboto-BlackItalic.ttf` & `PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/fonts/Roboto-Bold.ttf` & `PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/fonts/Roboto-BoldItalic.ttf` & `PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/fonts/Roboto-Italic.ttf` & `PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/fonts/Roboto-Light.ttf` & `PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/fonts/Roboto-LightItalic.ttf` & `PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/fonts/Roboto-Medium.ttf` & `PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/fonts/Roboto-MediumItalic.ttf` & `PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/fonts/Roboto-Regular.ttf` & `PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/fonts/Roboto-Thin.ttf` & `PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/fonts/Roboto-ThinItalic.ttf` & `PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/fonts/RobotoMono-Bold.ttf` & `PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf` & `PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf` & `PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf` & `PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/fonts/RobotoMono-Italic.ttf` & `PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/fonts/RobotoMono-Light.ttf` & `PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf` & `PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/fonts/RobotoMono-Medium.ttf` & `PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf` & `PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/fonts/RobotoMono-Regular.ttf` & `PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf` & `PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf` & `PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/fonts/RobotoMono-Thin.ttf` & `PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf` & `PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/themes/__init__.py` & `PyQtUIkit-2.4.2/PyQtUIkit/themes/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/themes/builtin_themes.py` & `PyQtUIkit-2.4.2/PyQtUIkit/themes/builtin_themes.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/themes/icons.py` & `PyQtUIkit-2.4.2/PyQtUIkit/themes/icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/themes/svg.py` & `PyQtUIkit-2.4.2/PyQtUIkit/themes/svg.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/themes/theme.py` & `PyQtUIkit-2.4.2/PyQtUIkit/themes/theme.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/__init__.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/_widget.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/application.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/application.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/button.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/button.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/checkbox.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/combo_box.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/dialog.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/flow_layout.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/group.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/group.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/hbox_layout.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/hbox_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/icon_widget.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/label.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/line_edit.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/line_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/list_widget.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/list_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/main_window.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/main_window.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/menu.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/menu_bar.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/menu_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/navigation.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/navigation.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/progress_bar.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/radio.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/radio.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/scroll_area.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/separator.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/separator.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/spin_box.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/spinner.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/spinner.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/tab_bar.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/tab_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/tabs.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/tabs.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/text_edit.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/text_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/toggle.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/toggle.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/tree_widget.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/tree_widget.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from enum import Enum
 
 from PyQt6.QtCore import Qt, pyqtSignal, QPoint
-from PyQt6.QtWidgets import QPushButton, QHBoxLayout, QLabel, QVBoxLayout, QWidget
 
 from PyQtUIkit.core import KitFont
 from PyQtUIkit.core.properties import IntProperty, StringProperty, IconProperty, BoolProperty, EnumProperty, \
     PaletteProperty, FontProperty
-from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
 from PyQtUIkit.widgets.dialog import KitDialog
 from PyQtUIkit.widgets.hbox_layout import KitHBoxLayout
+from PyQtUIkit.widgets.vbox_layout import KitVBoxLayout
 from PyQtUIkit.widgets.icon_widget import KitIconWidget
 from PyQtUIkit.widgets.label import KitLabel
 from PyQtUIkit.widgets.scroll_area import KitScrollArea
+from PyQtUIkit.widgets.button import KitLayoutButton, KitIconButton
 
 
-class KitTreeWidgetItem(QVBoxLayout, _KitWidget):
+class KitTreeWidgetItem(KitVBoxLayout):
     name = StringProperty('name', '')
     radius = IntProperty('radius', 4)
     icon = IconProperty('icon')
     text_palette = PaletteProperty('text_palette', 'Main')
     font = FontProperty('font')
     font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
+    always_expandable = BoolProperty('always_expandable', False)
 
     def __init__(self, name='', icon=''):
         super().__init__()
         self._name = name
         self._icon = icon
         self._main_palette = 'Main'
         self._text_palette = 'Main'
@@ -38,55 +39,46 @@
         self._icon1 = None
         self._icon2 = None
         self.__never_expanded = True
         self.__move_widget = None
         self.__last_pos = None
 
         self.setAlignment(Qt.AlignmentFlag.AlignTop)
-        self.setContentsMargins(0, 0, 0, 0)
-        self.setSpacing(0)
 
-        self.__button = QPushButton()
+        self.__button = KitLayoutButton()
+        self.__button.setSpacing(3)
         self.__button.mousePressEvent = self._on_clicked
         self.__button.mouseMoveEvent = self._on_move
         self.__button.mouseReleaseEvent = self._on_released
         self.__button.mouseDoubleClickEvent = self._on_double_clicked
         self.addWidget(self.__button)
 
-        self.__top_layout = QHBoxLayout()
-        self.__top_layout.setContentsMargins(0, 0, 0, 0)
-        self.__top_layout.setSpacing(3)
-        self.__button.setLayout(self.__top_layout)
-
-        self.__arrow_right = QPushButton()
+        self.__arrow_right = KitIconButton('line-chevron-forward')
         self.__arrow_right.setFixedSize(20, 20)
+        self.__arrow_right.border = 0
         self.__arrow_right.hide()
         self.__arrow_right.clicked.connect(self.expand)
-        self.__top_layout.addWidget(self.__arrow_right)
+        self.__button.addWidget(self.__arrow_right)
 
-        self.__arrow_down = QPushButton()
+        self.__arrow_down = KitIconButton('line-chevron-down')
         self.__arrow_down.setFixedSize(20, 20)
+        self.__arrow_down.border = 0
         self.__arrow_down.hide()
         self.__arrow_down.clicked.connect(self.collapse)
-        self.__top_layout.addWidget(self.__arrow_down)
+        self.__button.addWidget(self.__arrow_down)
 
         self.__icon_widget = KitIconWidget()
-        self.__top_layout.addWidget(self.__icon_widget)
+        self.__button.addWidget(self.__icon_widget)
 
-        self.__label = QLabel(self._name)
-        self.__top_layout.addWidget(self.__label)
+        self.__label = KitLabel(self._name)
+        self.__button.addWidget(self.__label)
 
-        self.__widget = QWidget()
-        self.addWidget(self.__widget)
-        self.__widget.hide()
-
-        self.__layout = QVBoxLayout()
-        self.__layout.setSpacing(0)
-        self.__layout.setContentsMargins(0, 0, 0, 0)
-        self.__widget.setLayout(self.__layout)
+        self.__layout = KitVBoxLayout()
+        self.__layout.hide()
+        self.addWidget(self.__layout)
 
     def parent(self):
         return self.__parent
 
     def level(self):
         return self.__level
 
@@ -98,83 +90,86 @@
 
     def insertItem(self, index, item: 'KitTreeWidgetItem'):
         item._set_level(self.__level + 1)
         item._set_root(self.__root, self)
         item._set_tm(self._tm)
 
         self.__children.insert(index, item)
-        self.__layout.insertLayout(index, item)
+        self.__layout.insertWidget(index, item)
 
         self.__arrow_down.setHidden(not self.__expanded)
         self.__arrow_right.setHidden(self.__expanded)
         self._update_padding()
 
     def childrenCount(self):
         return len(self.__children)
 
     def child(self, index):
         return self.__children[index]
 
     def clear(self):
         for _ in range(self.count()):
-            self.takeAt(0).widget().setParent(None)
+            self.__layout.clear()
         for el in self.__children:
             if el.selected():
                 self.__root._set_current(None)
         self.__children.clear()
 
     def deleteItem(self, item):
         if isinstance(item, KitTreeWidgetItem):
             item = self.__children.index(item)
-        self.takeAt(item).widget().setParent(None)
+        self.__layout.deleteWidget(item)
         if self.__children.pop(item).selected():
             self.__root._set_current(None)
 
     def deleteSelf(self):
         self.__parent.deleteItem(self)
 
     def expand(self):
         self.__expanded = True
-        self.__widget.show()
+        self.__layout.show()
         self.__arrow_down.show()
         self.__arrow_right.hide()
         if self.__never_expanded:
             self.firstExpand()
             self.__never_expanded = False
 
     def collapse(self):
         self.__expanded = False
-        self.__widget.hide()
+        self.__layout.hide()
         self.__arrow_down.hide()
         self.__arrow_right.show()
 
     def selected(self):
         return self.__selected
 
     def firstExpand(self):
         pass
 
+    def neverExpanded(self):
+        return self.__never_expanded
+
     def _on_clicked(self, a0):
-        QPushButton.mousePressEvent(self.__button, a0)
+        KitLayoutButton.mousePressEvent(self.__button, a0)
         self.__last_pos = a0.pos()
         self.__root._item_click(self, right=a0.button() == Qt.MouseButton.RightButton)
 
     def _on_double_clicked(self, a0):
-        QPushButton.mouseDoubleClickEvent(self.__button, a0)
+        KitLayoutButton.mouseDoubleClickEvent(self.__button, a0)
         self.__root._item_double_click(self)
 
     def _select(self, multi=False):
         self.__selected = True
         self._apply_selected_theme()
         if multi:
             for el in self.__children:
                 el._select(True)
 
     def _on_move(self, a0):
-        QPushButton.mouseMoveEvent(self.__button, a0)
+        KitLayoutButton.mouseMoveEvent(self.__button, a0)
         if self.__last_pos is None:
             return
         if not self.__root.movable:
             return 
         if self.__move_widget is None:
             self.__move_widget = _MoveItem(self, (self.__button.width(), self._height), self.name, self._icon,
                                            self._text_palette)
@@ -182,15 +177,15 @@
             self.__move_widget.move(self.__button.mapToGlobal(a0.pos()))
             self.__move_widget.show()
         else:
             self.__move_widget.move(self.__move_widget.pos() + a0.pos() - self.__last_pos)
         self.__last_pos = a0.pos()
 
     def _on_released(self, a0):
-        QPushButton.mouseReleaseEvent(self.__button, a0)
+        KitLayoutButton.mouseReleaseEvent(self.__button, a0)
         if isinstance(self.__move_widget, _MoveItem):
             self.__move_widget.close()
             self.__root._request_move(self, self.__move_widget.pos())
             self.__move_widget = None
         self.__last_pos = None
 
     def _deselect(self, multi=False):
@@ -203,15 +198,16 @@
     def _set_level(self, level):
         self.__level = level
         self._update_padding()
         for item in self.__children:
             item._set_level(self.__level + 1)
 
     def _update_padding(self):
-        self.__top_layout.setContentsMargins((self.__level - 1) * 15 + 3 + (0 if self.__children else 25), 0, 0, 0)
+        self.__button.setContentsMargins((self.__level - 1) * 15 + 3 +
+                                         (0 if self.__children or self.always_expandable else 25), 0, 0, 0)
 
     def _hide_button(self):
         self.__button.hide()
 
     def _set_tm(self, tm):
         super()._set_tm(tm)
         self.__icon_widget._set_tm(tm)
@@ -239,41 +235,27 @@
     def _apply_theme(self):
         if not self._tm or not self._tm.active:
             return
         for el in self.__children:
             el._height = self._height
             el.main_palette = self._main_palette
             el.text_palette = self._text_palette
-        if self._icon:
-            self.__icon_widget._icon = self._icon
-            self.__icon_widget.show()
-            self.__icon_widget._main_palette = self._text_palette
-            self.__icon_widget.setFixedSize(self._height - 6, self._height - 6)
-            self.__icon_widget._apply_theme()
-        else:
-            self.__icon_widget.hide()
         self.__button.setFixedHeight(self._height)
-        self.__arrow_right.setIcon(self.__root._icon1)
-        self.__arrow_down.setIcon(self.__root._icon2)
+        self.__icon_widget.setFixedSize(self._height - 4, self._height - 4)
+        self.__icon_widget._icon = self._icon
+
+        if self.__children or self.always_expandable:
+            self.__arrow_down.setHidden(not self.__expanded)
+            self.__arrow_right.setHidden(self.__expanded)
+        else:
+            self.__arrow_down.setHidden(False)
+            self.__arrow_right.setHidden(False)
+
+        super()._apply_theme()
         self._apply_selected_theme()
-        self.__label.setFont(self.font.get(self.font_size))
-        for el in [self.__arrow_right, self.__arrow_down]:
-            el.setStyleSheet(f"""
-            QPushButton {{
-                background-color: transparent;
-                border: 0px solid black;
-                border-radius: {self.radius}px;
-            }}
-            QPushButton:hover {{
-                background-color: {self.main_palette.main};
-            }}
-            """)
-        self.__label.setStyleSheet(f"color: {self.text_palette.text_only}; background-color: transparent;")
-        for el in self.__children:
-            el._apply_theme()
 
     def _apply_selected_theme(self):
         self.__button.setStyleSheet(f"""
             QPushButton {{
                 color: {self.main_palette.text};
                 background-color: {self.main_palette.selected if self.__selected else self.main_palette.main};
                 border: 0px solid black;
@@ -336,18 +318,15 @@
         self.__selected = []
         self.__selected_level = 0
 
         self.__tree = KitTreeWidgetItem()
         self.__tree._hide_button()
         self.__tree._set_root(self, None)
         self.__tree.expand()
-
-        self.__widget = QWidget()
-        self.__widget.setLayout(self.__tree)
-        self.setWidget(self.__widget)
+        self.setWidget(self.__tree)
 
     def addItem(self, item: KitTreeWidgetItem):
         item._main_palette = self._main_palette
         self.__tree.addItem(item)
 
     def currentItem(self) -> KitTreeWidgetItem | None:
         return self.__current
@@ -356,15 +335,15 @@
         return self.__selected
 
     def _set_current(self, item):
         self.currentItemChanged.emit(item)
         self.__current = item
 
     def _request_move(self, item, pos):
-        dest, _ = self.__tree._find_by_pos(pos - self.__widget.mapToGlobal(QPoint(0, 0)))
+        dest, _ = self.__tree._find_by_pos(pos - self.__tree.mapToGlobal(QPoint(0, 0)))
         if dest:
             self.moveRequested.emit(item, dest)
 
     def _item_click(self, item: KitTreeWidgetItem, right=False):
         if self.selection_type == KitTreeWidget.SelectionType.MULTI:
             if self.__control:
                 if not item.selected():
@@ -455,14 +434,11 @@
 
     def _set_tm(self, tm):
         super()._set_tm(tm)
         self.__tree._set_tm(tm)
 
     def _apply_theme(self):
         self.__tree.main_palette = self._main_palette
-        self.__widget.setStyleSheet("background-color: transparent;")
-        self._icon1 = self._tm.icon('line-chevron-right', self.main_palette.text)
-        self._icon2 = self._tm.icon('line-chevron-down', self.main_palette.text)
         self.__tree._main_palette = self._main_palette
         self.__tree._text_palette = self._items_palette
         self.__tree._apply_theme()
         super()._apply_theme()
```

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit/widgets/vbox_layout.py` & `PyQtUIkit-2.4.2/PyQtUIkit/widgets/vbox_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit.egg-info/PKG-INFO` & `PyQtUIkit-2.4.2/PyQtUIkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.4.1
+Version: 2.4.2
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.4.1/PyQtUIkit.egg-info/SOURCES.txt` & `PyQtUIkit-2.4.2/PyQtUIkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.1/setup.py` & `PyQtUIkit-2.4.2/setup.py`

 * *Files identical despite different names*

