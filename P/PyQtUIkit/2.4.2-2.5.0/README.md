# Comparing `tmp/PyQtUIkit-2.4.2.tar.gz` & `tmp/PyQtUIkit-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQtUIkit-2.4.2.tar", last modified: Sat Apr 13 15:35:33 2024, max compression
+gzip compressed data, was "PyQtUIkit-2.5.0.tar", last modified: Sat Apr 13 22:50:51 2024, max compression
```

## Comparing `PyQtUIkit-2.4.2.tar` & `PyQtUIkit-2.5.0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 15:35:33.290948 PyQtUIkit-2.4.2/
--rw-rw-rw-   0        0        0     1090 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/LICENSE
--rw-rw-rw-   0        0        0     2938 2024-04-13 15:35:33.290948 PyQtUIkit-2.4.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-13 15:35:33.244097 PyQtUIkit-2.4.2/PyQtUIkit/
--rw-rw-rw-   0        0        0       49 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/__init__.py
--rw-rw-rw-   0        0        0     3896 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/_icons.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:35:33.259697 PyQtUIkit-2.4.2/PyQtUIkit/builder/
--rw-rw-rw-   0        0        0     1116 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/builder/__init__.py
--rw-rw-rw-   0        0        0     1825 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/builder/builder_class.py
--rw-rw-rw-   0        0        0     1383 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/builder/builder_module.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:35:33.259697 PyQtUIkit-2.4.2/PyQtUIkit/core/
--rw-rw-rw-   0        0        0       84 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/core/__init__.py
--rw-rw-rw-   0        0        0       19 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/core/_version.py
--rw-rw-rw-   0        0        0     1503 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/core/font.py
--rw-rw-rw-   0        0        0     1019 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/core/icon.py
--rw-rw-rw-   0        0        0     4655 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/core/properties.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:35:33.275321 PyQtUIkit-2.4.2/PyQtUIkit/fonts/
--rw-rw-rw-   0        0        0   168060 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-Black.ttf
--rw-rw-rw-   0        0        0   174108 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
--rw-rw-rw-   0        0        0   167336 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-Bold.ttf
--rw-rw-rw-   0        0        0   171508 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
--rw-rw-rw-   0        0        0   170504 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-Italic.ttf
--rw-rw-rw-   0        0        0   167000 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-Light.ttf
--rw-rw-rw-   0        0        0   173172 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-LightItalic.ttf
--rw-rw-rw-   0        0        0   168644 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-Medium.ttf
--rw-rw-rw-   0        0        0   173416 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
--rw-rw-rw-   0        0        0   168260 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-Regular.ttf
--rw-rw-rw-   0        0        0   168488 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-Thin.ttf
--rw-rw-rw-   0        0        0   172860 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
--rw-rw-rw-   0        0        0    87392 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-Bold.ttf
--rw-rw-rw-   0        0        0    94636 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
--rw-rw-rw-   0        0        0    88248 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
--rw-rw-rw-   0        0        0    94016 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
--rw-rw-rw-   0        0        0    94372 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-Italic.ttf
--rw-rw-rw-   0        0        0    87980 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-Light.ttf
--rw-rw-rw-   0        0        0    94256 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
--rw-rw-rw-   0        0        0    87172 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-Medium.ttf
--rw-rw-rw-   0        0        0    94412 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
--rw-rw-rw-   0        0        0    87236 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-Regular.ttf
--rw-rw-rw-   0        0        0    87496 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
--rw-rw-rw-   0        0        0    94508 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
--rw-rw-rw-   0        0        0    88288 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-Thin.ttf
--rw-rw-rw-   0        0        0    93588 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
-drwxrwxrwx   0        0        0        0 2024-04-13 15:35:33.275321 PyQtUIkit-2.4.2/PyQtUIkit/themes/
--rw-rw-rw-   0        0        0     2180 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/themes/__init__.py
--rw-rw-rw-   0        0        0     5879 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/themes/builtin_themes.py
--rw-rw-rw-   0        0        0  2340473 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/themes/icons.py
--rw-rw-rw-   0        0        0     1470 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/themes/svg.py
--rw-rw-rw-   0        0        0     1402 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/themes/theme.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:35:33.290948 PyQtUIkit-2.4.2/PyQtUIkit/widgets/
--rw-rw-rw-   0        0        0     1626 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/__init__.py
--rw-rw-rw-   0        0        0     3515 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/_widget.py
--rw-rw-rw-   0        0        0     1359 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/application.py
--rw-rw-rw-   0        0        0     7833 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/button.py
--rw-rw-rw-   0        0        0     2788 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/checkbox.py
--rw-rw-rw-   0        0        0    10059 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/combo_box.py
--rw-rw-rw-   0        0        0     7021 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/dialog.py
--rw-rw-rw-   0        0        0     5807 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/flow_layout.py
--rw-rw-rw-   0        0        0     2280 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/group.py
--rw-rw-rw-   0        0        0     4293 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/hbox_layout.py
--rw-rw-rw-   0        0        0     1578 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/icon_widget.py
--rw-rw-rw-   0        0        0     1100 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/label.py
--rw-rw-rw-   0        0        0     1487 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/line_edit.py
--rw-rw-rw-   0        0        0     3448 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/list_widget.py
--rw-rw-rw-   0        0        0     1424 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/main_window.py
--rw-rw-rw-   0        0        0     3302 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/menu.py
--rw-rw-rw-   0        0        0     4336 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/menu_bar.py
--rw-rw-rw-   0        0        0     7084 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/navigation.py
--rw-rw-rw-   0        0        0     2647 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     6683 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/radio.py
--rw-rw-rw-   0        0        0     3881 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/scroll_area.py
--rw-rw-rw-   0        0        0     1486 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/separator.py
--rw-rw-rw-   0        0        0     7515 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/spin_box.py
--rw-rw-rw-   0        0        0     3580 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/spinner.py
--rw-rw-rw-   0        0        0    13353 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/tab_bar.py
--rw-rw-rw-   0        0        0     1218 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/tabs.py
--rw-rw-rw-   0        0        0     2167 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/text_edit.py
--rw-rw-rw-   0        0        0     4465 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/toggle.py
--rw-rw-rw-   0        0        0    16120 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/tree_widget.py
--rw-rw-rw-   0        0        0     4620 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/PyQtUIkit/widgets/vbox_layout.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:35:33.259697 PyQtUIkit-2.4.2/PyQtUIkit.egg-info/
--rw-rw-rw-   0        0        0     2938 2024-04-13 15:35:33.000000 PyQtUIkit-2.4.2/PyQtUIkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2537 2024-04-13 15:35:33.000000 PyQtUIkit-2.4.2/PyQtUIkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 15:35:33.000000 PyQtUIkit-2.4.2/PyQtUIkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-13 15:35:33.000000 PyQtUIkit-2.4.2/PyQtUIkit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2024-04-13 15:35:33.000000 PyQtUIkit-2.4.2/PyQtUIkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-13 15:35:33.000000 PyQtUIkit-2.4.2/PyQtUIkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-13 15:35:33.290948 PyQtUIkit-2.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1411 2024-04-13 15:34:44.000000 PyQtUIkit-2.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 22:50:51.764407 PyQtUIkit-2.5.0/
+-rw-rw-rw-   0        0        0     1090 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/LICENSE
+-rw-rw-rw-   0        0        0     2938 2024-04-13 22:50:51.764407 PyQtUIkit-2.5.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-13 22:50:51.733159 PyQtUIkit-2.5.0/PyQtUIkit/
+-rw-rw-rw-   0        0        0       49 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/__init__.py
+-rw-rw-rw-   0        0        0     3896 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/_icons.py
+drwxrwxrwx   0        0        0        0 2024-04-13 22:50:51.733159 PyQtUIkit-2.5.0/PyQtUIkit/builder/
+-rw-rw-rw-   0        0        0     1116 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/builder/__init__.py
+-rw-rw-rw-   0        0        0     1825 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/builder/builder_class.py
+-rw-rw-rw-   0        0        0     1383 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/builder/builder_module.py
+drwxrwxrwx   0        0        0        0 2024-04-13 22:50:51.733159 PyQtUIkit-2.5.0/PyQtUIkit/core/
+-rw-rw-rw-   0        0        0       84 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/core/__init__.py
+-rw-rw-rw-   0        0        0       19 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/core/_version.py
+-rw-rw-rw-   0        0        0     1503 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/core/font.py
+-rw-rw-rw-   0        0        0     1019 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/core/icon.py
+-rw-rw-rw-   0        0        0     4655 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/core/properties.py
+drwxrwxrwx   0        0        0        0 2024-04-13 22:50:51.748781 PyQtUIkit-2.5.0/PyQtUIkit/fonts/
+-rw-rw-rw-   0        0        0   168060 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/fonts/Roboto-Black.ttf
+-rw-rw-rw-   0        0        0   174108 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
+-rw-rw-rw-   0        0        0   167336 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/fonts/Roboto-Bold.ttf
+-rw-rw-rw-   0        0        0   171508 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
+-rw-rw-rw-   0        0        0   170504 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/fonts/Roboto-Italic.ttf
+-rw-rw-rw-   0        0        0   167000 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/fonts/Roboto-Light.ttf
+-rw-rw-rw-   0        0        0   173172 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/fonts/Roboto-LightItalic.ttf
+-rw-rw-rw-   0        0        0   168644 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/fonts/Roboto-Medium.ttf
+-rw-rw-rw-   0        0        0   173416 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
+-rw-rw-rw-   0        0        0   168260 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/fonts/Roboto-Regular.ttf
+-rw-rw-rw-   0        0        0   168488 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/fonts/Roboto-Thin.ttf
+-rw-rw-rw-   0        0        0   172860 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
+-rw-rw-rw-   0        0        0    87392 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/fonts/RobotoMono-Bold.ttf
+-rw-rw-rw-   0        0        0    94636 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
+-rw-rw-rw-   0        0        0    88248 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
+-rw-rw-rw-   0        0        0    94016 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
+-rw-rw-rw-   0        0        0    94372 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/fonts/RobotoMono-Italic.ttf
+-rw-rw-rw-   0        0        0    87980 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/fonts/RobotoMono-Light.ttf
+-rw-rw-rw-   0        0        0    94256 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
+-rw-rw-rw-   0        0        0    87172 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/fonts/RobotoMono-Medium.ttf
+-rw-rw-rw-   0        0        0    94412 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
+-rw-rw-rw-   0        0        0    87236 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/fonts/RobotoMono-Regular.ttf
+-rw-rw-rw-   0        0        0    87496 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
+-rw-rw-rw-   0        0        0    94508 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
+-rw-rw-rw-   0        0        0    88288 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/fonts/RobotoMono-Thin.ttf
+-rw-rw-rw-   0        0        0    93588 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
+drwxrwxrwx   0        0        0        0 2024-04-13 22:50:51.748781 PyQtUIkit-2.5.0/PyQtUIkit/themes/
+-rw-rw-rw-   0        0        0     2180 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/themes/__init__.py
+-rw-rw-rw-   0        0        0     5879 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/themes/builtin_themes.py
+-rw-rw-rw-   0        0        0  2340473 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/themes/icons.py
+-rw-rw-rw-   0        0        0     1470 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/themes/svg.py
+-rw-rw-rw-   0        0        0     1402 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/themes/theme.py
+drwxrwxrwx   0        0        0        0 2024-04-13 22:50:51.764407 PyQtUIkit-2.5.0/PyQtUIkit/widgets/
+-rw-rw-rw-   0        0        0     1638 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3515 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/_widget.py
+-rw-rw-rw-   0        0        0     1359 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/application.py
+-rw-rw-rw-   0        0        0     7833 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/button.py
+-rw-rw-rw-   0        0        0     2788 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/checkbox.py
+-rw-rw-rw-   0        0        0    10054 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/combo_box.py
+-rw-rw-rw-   0        0        0     8253 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/dialog.py
+-rw-rw-rw-   0        0        0     5807 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/flow_layout.py
+-rw-rw-rw-   0        0        0     2317 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/form.py
+-rw-rw-rw-   0        0        0     2280 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/group.py
+-rw-rw-rw-   0        0        0     1578 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0     1100 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/label.py
+-rw-rw-rw-   0        0        0     4994 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/layout.py
+-rw-rw-rw-   0        0        0     1487 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     3448 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/list_widget.py
+-rw-rw-rw-   0        0        0     1424 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/main_window.py
+-rw-rw-rw-   0        0        0     3302 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/menu.py
+-rw-rw-rw-   0        0        0     4336 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/menu_bar.py
+-rw-rw-rw-   0        0        0     7084 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/navigation.py
+-rw-rw-rw-   0        0        0     2647 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     6683 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/radio.py
+-rw-rw-rw-   0        0        0     3881 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0     1486 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/separator.py
+-rw-rw-rw-   0        0        0     7515 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     3580 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/spinner.py
+-rw-rw-rw-   0        0        0    13348 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/tab_bar.py
+-rw-rw-rw-   0        0        0     1218 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/tabs.py
+-rw-rw-rw-   0        0        0     2167 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/text_edit.py
+-rw-rw-rw-   0        0        0     4465 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/toggle.py
+-rw-rw-rw-   0        0        0    16164 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/PyQtUIkit/widgets/tree_widget.py
+drwxrwxrwx   0        0        0        0 2024-04-13 22:50:51.733159 PyQtUIkit-2.5.0/PyQtUIkit.egg-info/
+-rw-rw-rw-   0        0        0     2938 2024-04-13 22:50:51.000000 PyQtUIkit-2.5.0/PyQtUIkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2525 2024-04-13 22:50:51.000000 PyQtUIkit-2.5.0/PyQtUIkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 22:50:51.000000 PyQtUIkit-2.5.0/PyQtUIkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-13 22:50:51.000000 PyQtUIkit-2.5.0/PyQtUIkit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2024-04-13 22:50:51.000000 PyQtUIkit-2.5.0/PyQtUIkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-13 22:50:51.000000 PyQtUIkit-2.5.0/PyQtUIkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-13 22:50:51.764407 PyQtUIkit-2.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1411 2024-04-13 22:50:23.000000 PyQtUIkit-2.5.0/setup.py
```

### Comparing `PyQtUIkit-2.4.2/LICENSE` & `PyQtUIkit-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PKG-INFO` & `PyQtUIkit-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.4.2
+Version: 2.5.0
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/_icons.py` & `PyQtUIkit-2.5.0/PyQtUIkit/_icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/builder/__init__.py` & `PyQtUIkit-2.5.0/PyQtUIkit/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/builder/builder_class.py` & `PyQtUIkit-2.5.0/PyQtUIkit/builder/builder_class.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/builder/builder_module.py` & `PyQtUIkit-2.5.0/PyQtUIkit/builder/builder_module.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/core/font.py` & `PyQtUIkit-2.5.0/PyQtUIkit/core/font.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/core/icon.py` & `PyQtUIkit-2.5.0/PyQtUIkit/core/icon.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/core/properties.py` & `PyQtUIkit-2.5.0/PyQtUIkit/core/properties.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-Black.ttf` & `PyQtUIkit-2.5.0/PyQtUIkit/fonts/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-BlackItalic.ttf` & `PyQtUIkit-2.5.0/PyQtUIkit/fonts/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-Bold.ttf` & `PyQtUIkit-2.5.0/PyQtUIkit/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-BoldItalic.ttf` & `PyQtUIkit-2.5.0/PyQtUIkit/fonts/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-Italic.ttf` & `PyQtUIkit-2.5.0/PyQtUIkit/fonts/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-Light.ttf` & `PyQtUIkit-2.5.0/PyQtUIkit/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-LightItalic.ttf` & `PyQtUIkit-2.5.0/PyQtUIkit/fonts/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-Medium.ttf` & `PyQtUIkit-2.5.0/PyQtUIkit/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-MediumItalic.ttf` & `PyQtUIkit-2.5.0/PyQtUIkit/fonts/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-Regular.ttf` & `PyQtUIkit-2.5.0/PyQtUIkit/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-Thin.ttf` & `PyQtUIkit-2.5.0/PyQtUIkit/fonts/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/fonts/Roboto-ThinItalic.ttf` & `PyQtUIkit-2.5.0/PyQtUIkit/fonts/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-Bold.ttf` & `PyQtUIkit-2.5.0/PyQtUIkit/fonts/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf` & `PyQtUIkit-2.5.0/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf` & `PyQtUIkit-2.5.0/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf` & `PyQtUIkit-2.5.0/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-Italic.ttf` & `PyQtUIkit-2.5.0/PyQtUIkit/fonts/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-Light.ttf` & `PyQtUIkit-2.5.0/PyQtUIkit/fonts/RobotoMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf` & `PyQtUIkit-2.5.0/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-Medium.ttf` & `PyQtUIkit-2.5.0/PyQtUIkit/fonts/RobotoMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf` & `PyQtUIkit-2.5.0/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-Regular.ttf` & `PyQtUIkit-2.5.0/PyQtUIkit/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf` & `PyQtUIkit-2.5.0/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf` & `PyQtUIkit-2.5.0/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-Thin.ttf` & `PyQtUIkit-2.5.0/PyQtUIkit/fonts/RobotoMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf` & `PyQtUIkit-2.5.0/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/themes/__init__.py` & `PyQtUIkit-2.5.0/PyQtUIkit/themes/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/themes/builtin_themes.py` & `PyQtUIkit-2.5.0/PyQtUIkit/themes/builtin_themes.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/themes/icons.py` & `PyQtUIkit-2.5.0/PyQtUIkit/themes/icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/themes/svg.py` & `PyQtUIkit-2.5.0/PyQtUIkit/themes/svg.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/themes/theme.py` & `PyQtUIkit-2.5.0/PyQtUIkit/themes/theme.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/__init__.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from PyQtUIkit.widgets.hbox_layout import KitHBoxLayout
-from PyQtUIkit.widgets.vbox_layout import KitVBoxLayout
+from PyQtUIkit.widgets.layout import KitHBoxLayout, KitVBoxLayout
 from PyQtUIkit.widgets.flow_layout import KitFlowLayout
 from PyQtUIkit.widgets.label import KitLabel
 from PyQtUIkit.widgets.icon_widget import KitIconWidget
 from PyQtUIkit.widgets.button import KitButton, KitIconButton, KitLayoutButton
 from PyQtUIkit.widgets.line_edit import KitLineEdit
 from PyQtUIkit.widgets.list_widget import KitListWidget, KitListWidgetItem
 from PyQtUIkit.widgets.main_window import KitMainWindow
@@ -18,11 +17,12 @@
 from PyQtUIkit.widgets.tree_widget import KitTreeWidget, KitTreeWidgetItem
 from PyQtUIkit.widgets.menu import KitMenu
 from PyQtUIkit.widgets.group import KitHGroup, KitVGroup
 from PyQtUIkit.widgets.navigation import KitNavigation
 from PyQtUIkit.widgets.radio import KitVRadio, KitHRadio
 from PyQtUIkit.widgets.tabs import KitTabLayout
 from PyQtUIkit.widgets.text_edit import KitTextEdit
-from PyQtUIkit.widgets.dialog import KitDialog
+from PyQtUIkit.widgets.form import KitForm
+from PyQtUIkit.widgets.dialog import KitDialog, KitFormDialog
 from PyQtUIkit.widgets.application import KitApplication, KitAsyncApplication
 from PyQtUIkit.widgets.separator import KitHSeparator, KitVSeparator
 from PyQtUIkit.widgets.menu_bar import KitMenuBar
```

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/_widget.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/application.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/application.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/button.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/button.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/checkbox.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/combo_box.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/combo_box.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from PyQt6.QtWidgets import QPushButton, QVBoxLayout, QMenu, QHBoxLayout, QApplication
 
 from PyQtUIkit.core import IntProperty, PaletteProperty, IconProperty, EnumProperty, KitFont, FontProperty, \
     MethodsProperty
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget, KitGroupItem as _KitGroupItem
 from PyQtUIkit.widgets.icon_widget import KitIconWidget
 from PyQtUIkit.widgets.scroll_area import KitScrollArea
-from PyQtUIkit.widgets.vbox_layout import KitVBoxLayout
+from PyQtUIkit.widgets.layout import KitVBoxLayout
 from PyQtUIkit.widgets.button import KitLayoutButton
 
 
 class KitComboBoxItem(QPushButton, _KitWidget):
     selected = pyqtSignal(object)
     icon = IconProperty('icon')
     font = FontProperty('font')
```

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/dialog.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/dialog.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from PyQt6.QtCore import Qt
 from PyQt6.QtWidgets import QDialog, QVBoxLayout, QLabel
 
 from PyQtUIkit.core.properties import PaletteProperty, BoolProperty, StringProperty, IconProperty
 from PyQtUIkit.widgets import KitIconButton, KitHBoxLayout, KitVBoxLayout, KitButton, KitIconWidget, KitLabel
+from PyQtUIkit.widgets.form import KitForm
 from PyQtUIkit.widgets._widget import _KitWidget
 
 
 class KitDialog(QDialog, _KitWidget):
     header_palette = PaletteProperty('header_palette', 'Menu')
     button_close = BoolProperty('button_close', True)
     name = StringProperty('name', '')
@@ -98,15 +99,15 @@
     def danger(parent, title: str, text: str):
         dialog = _KitMessageBox(parent, title, text, 'sharp-alert-circle')
         dialog.icon_palette = 'Danger'
         dialog.exec()
 
     @staticmethod
     def warning(parent, title: str, text: str):
-        dialog = _KitMessageBox(parent, title, text, 'solid-alert-triangle')
+        dialog = _KitMessageBox(parent, title, text, 'solid-warning')
         dialog.icon_palette = 'Warning'
         dialog.exec()
 
     @staticmethod
     def success(parent, title: str, text: str):
         dialog = _KitMessageBox(parent, title, text, 'sharp-checkmark-circle')
         dialog.icon_palette = 'Success'
@@ -197,7 +198,44 @@
         layout.addWidget(self._label, 100)
 
     def _apply_theme(self):
         self._label.setText(self.text)
         self._icon_widget.icon = self._icon
         self._icon_widget.main_palette = self.icon_palette
         super()._apply_theme()
+
+
+class KitFormDialog(KitDialog):
+    def __init__(self, parent, *args):
+        super().__init__(parent)
+        self.button_close = False
+        self.setMinimumWidth(320)
+        self.setMaximumHeight(60)
+
+        main_layout = KitVBoxLayout()
+        main_layout.alignment = Qt.AlignmentFlag.AlignTop
+        main_layout.padding = 20, 20, 20, 10
+        main_layout.spacing = 16
+        self.setWidget(main_layout)
+
+        self._form = KitForm(*args)
+        main_layout.addWidget(self._form)
+
+        buttons_layout = KitHBoxLayout()
+        buttons_layout.spacing = 6
+        buttons_layout.alignment = Qt.AlignmentFlag.AlignRight
+        main_layout.addWidget(buttons_layout)
+
+        self._button_cancel = KitButton("Cancel")
+        self._button_cancel.setFixedSize(100, 26)
+        self._button_cancel.on_click = self.reject
+        buttons_layout.addWidget(self._button_cancel)
+
+        self._button_ok = KitButton("Ok")
+        self._button_ok.setFixedSize(100, 26)
+        self._button_ok.on_click = self.accept
+        buttons_layout.addWidget(self._button_ok)
+
+        self.resize(300, 60)
+
+    def res(self):
+        return self._form.res()
```

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/flow_layout.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/group.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/group.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/hbox_layout.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/layout.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from PyQt6.QtCore import QMargins
-from PyQt6.QtWidgets import QWidget, QHBoxLayout
+from PyQt6.QtCore import QMargins, Qt
+from PyQt6.QtWidgets import QWidget, QVBoxLayout, QHBoxLayout
 
 from PyQtUIkit.core.properties import IntProperty, MethodsProperty
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
 
 
-class KitHBoxLayout(QWidget, _KitWidget):
+class KitBoxLayout(QWidget, _KitWidget):
     border = IntProperty('border', 0)
     radius = IntProperty('radius', 4)
 
-    def __init__(self):
+    def __init__(self, orientation=Qt.Orientation.Horizontal):
         super().__init__()
         self._widgets = []
-        self.main_palette = 'Transparent'
+        self._main_palette = 'Transparent'
 
-        strange_layout = QHBoxLayout()
+        strange_layout = QVBoxLayout()
         strange_layout.setContentsMargins(0, 0, 0, 0)
         self.setLayout(strange_layout)
 
         strange_widget = QWidget()
         strange_layout.addWidget(strange_widget)
 
-        self.__layout = QHBoxLayout()
+        self.__layout = QVBoxLayout() if orientation == Qt.Orientation.Vertical else QHBoxLayout()
         self.__layout.setContentsMargins(0, 0, 0, 0)
         self.__layout.setSpacing(0)
         strange_widget.setLayout(self.__layout)
 
         self._add_child_func = self.addWidget
         self._build_from_kui()
 
@@ -117,7 +117,21 @@
             border-radius: {self.radius}px;
         }}
         """)
 
     padding = MethodsProperty(getContentsMargins, _set_margins)
     spacing = MethodsProperty(getSpacing, setSpacing)
     alignment = MethodsProperty(getAlignment, setAlignment)
+    max_width = MethodsProperty(QWidget.maximumWidth, QWidget.setMaximumWidth)
+    min_width = MethodsProperty(QWidget.minimumWidth, QWidget.setMinimumWidth)
+    max_height = MethodsProperty(QWidget.maximumHeight, QWidget.setMaximumHeight)
+    min_height = MethodsProperty(QWidget.minimumHeight, QWidget.setMinimumHeight)
+
+
+class KitVBoxLayout(KitBoxLayout):
+    def __init__(self):
+        super().__init__(orientation=Qt.Orientation.Vertical)
+
+
+class KitHBoxLayout(KitBoxLayout):
+    def __init__(self):
+        super().__init__(orientation=Qt.Orientation.Horizontal)
```

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/icon_widget.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/label.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/line_edit.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/line_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/list_widget.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/list_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/main_window.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/main_window.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/menu.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/menu_bar.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/menu_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/navigation.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/navigation.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/progress_bar.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/radio.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/radio.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/scroll_area.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/separator.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/separator.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/spin_box.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/spinner.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/spinner.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/tab_bar.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/tab_bar.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from PyQtUIkit.core import KitFont
 from PyQtUIkit.core.properties import IntProperty, PaletteProperty, IconProperty, EnumProperty, FontProperty
 from PyQtUIkit.themes import KitPalette
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
 from PyQtUIkit.widgets.icon_widget import KitIconWidget
 from PyQtUIkit.widgets.button import KitIconButton, KitButton
 from PyQtUIkit.widgets.scroll_area import KitScrollArea
-from PyQtUIkit.widgets.hbox_layout import KitHBoxLayout
+from PyQtUIkit.widgets.layout import KitHBoxLayout
 from PyQtUIkit.widgets.label import KitLabel
 
 
 class KitTab(QPushButton, _KitWidget):
     radius_top = IntProperty('radius_top', 5)
     radius_bottom = IntProperty('radius_bottom', 0)
     font = FontProperty('font')
```

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/tabs.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/tabs.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/text_edit.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/text_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/toggle.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/toggle.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit/widgets/tree_widget.py` & `PyQtUIkit-2.5.0/PyQtUIkit/widgets/tree_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 
 from PyQt6.QtCore import Qt, pyqtSignal, QPoint
 
 from PyQtUIkit.core import KitFont
 from PyQtUIkit.core.properties import IntProperty, StringProperty, IconProperty, BoolProperty, EnumProperty, \
     PaletteProperty, FontProperty
 from PyQtUIkit.widgets.dialog import KitDialog
-from PyQtUIkit.widgets.hbox_layout import KitHBoxLayout
-from PyQtUIkit.widgets.vbox_layout import KitVBoxLayout
+from PyQtUIkit.widgets.layout import KitVBoxLayout, KitHBoxLayout
 from PyQtUIkit.widgets.icon_widget import KitIconWidget
 from PyQtUIkit.widgets.label import KitLabel
 from PyQtUIkit.widgets.scroll_area import KitScrollArea
 from PyQtUIkit.widgets.button import KitLayoutButton, KitIconButton
 
 
 class KitTreeWidgetItem(KitVBoxLayout):
@@ -42,14 +41,15 @@
         self.__move_widget = None
         self.__last_pos = None
 
         self.setAlignment(Qt.AlignmentFlag.AlignTop)
 
         self.__button = KitLayoutButton()
         self.__button.setSpacing(3)
+        self.__button.border = 0
         self.__button.mousePressEvent = self._on_clicked
         self.__button.mouseMoveEvent = self._on_move
         self.__button.mouseReleaseEvent = self._on_released
         self.__button.mouseDoubleClickEvent = self._on_double_clicked
         self.addWidget(self.__button)
 
         self.__arrow_right = KitIconButton('line-chevron-forward')
@@ -135,14 +135,17 @@
 
     def collapse(self):
         self.__expanded = False
         self.__layout.hide()
         self.__arrow_down.hide()
         self.__arrow_right.show()
 
+    def expanded(self):
+        return self.__expanded
+
     def selected(self):
         return self.__selected
 
     def firstExpand(self):
         pass
 
     def neverExpanded(self):
@@ -243,16 +246,16 @@
         self.__icon_widget.setFixedSize(self._height - 4, self._height - 4)
         self.__icon_widget._icon = self._icon
 
         if self.__children or self.always_expandable:
             self.__arrow_down.setHidden(not self.__expanded)
             self.__arrow_right.setHidden(self.__expanded)
         else:
-            self.__arrow_down.setHidden(False)
-            self.__arrow_right.setHidden(False)
+            self.__arrow_down.setHidden(True)
+            self.__arrow_right.setHidden(True)
 
         super()._apply_theme()
         self._apply_selected_theme()
 
     def _apply_selected_theme(self):
         self.__button.setStyleSheet(f"""
             QPushButton {{
```

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit.egg-info/PKG-INFO` & `PyQtUIkit-2.5.0/PyQtUIkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.4.2
+Version: 2.5.0
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.4.2/PyQtUIkit.egg-info/SOURCES.txt` & `PyQtUIkit-2.5.0/PyQtUIkit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -51,18 +51,19 @@
 PyQtUIkit/widgets/_widget.py
 PyQtUIkit/widgets/application.py
 PyQtUIkit/widgets/button.py
 PyQtUIkit/widgets/checkbox.py
 PyQtUIkit/widgets/combo_box.py
 PyQtUIkit/widgets/dialog.py
 PyQtUIkit/widgets/flow_layout.py
+PyQtUIkit/widgets/form.py
 PyQtUIkit/widgets/group.py
-PyQtUIkit/widgets/hbox_layout.py
 PyQtUIkit/widgets/icon_widget.py
 PyQtUIkit/widgets/label.py
+PyQtUIkit/widgets/layout.py
 PyQtUIkit/widgets/line_edit.py
 PyQtUIkit/widgets/list_widget.py
 PyQtUIkit/widgets/main_window.py
 PyQtUIkit/widgets/menu.py
 PyQtUIkit/widgets/menu_bar.py
 PyQtUIkit/widgets/navigation.py
 PyQtUIkit/widgets/progress_bar.py
@@ -71,9 +72,8 @@
 PyQtUIkit/widgets/separator.py
 PyQtUIkit/widgets/spin_box.py
 PyQtUIkit/widgets/spinner.py
 PyQtUIkit/widgets/tab_bar.py
 PyQtUIkit/widgets/tabs.py
 PyQtUIkit/widgets/text_edit.py
 PyQtUIkit/widgets/toggle.py
-PyQtUIkit/widgets/tree_widget.py
-PyQtUIkit/widgets/vbox_layout.py
+PyQtUIkit/widgets/tree_widget.py
```

### Comparing `PyQtUIkit-2.4.2/setup.py` & `PyQtUIkit-2.5.0/setup.py`

 * *Files identical despite different names*

