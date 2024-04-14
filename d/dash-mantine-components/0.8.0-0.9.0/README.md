# Comparing `tmp/dash_mantine_components-0.8.0.tar.gz` & `tmp/dash_mantine_components-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_mantine_components-0.8.0.tar", last modified: Sun May  1 08:02:49 2022, max compression
+gzip compressed data, was "dash_mantine_components-0.9.0.tar", last modified: Wed Jun  1 05:33:19 2022, max compression
```

## Comparing `dash_mantine_components-0.8.0.tar` & `dash_mantine_components-0.9.0.tar`

### file list

```diff
@@ -1,98 +1,101 @@
-drwxr-xr-x   0 snehilvijay   (501) staff       (20)        0 2022-05-01 08:02:49.911078 dash_mantine_components-0.8.0/
--rw-r--r--   0 snehilvijay   (501) staff       (20)     1068 2022-03-22 15:21:12.000000 dash_mantine_components-0.8.0/LICENSE
--rw-r--r--   0 snehilvijay   (501) staff       (20)      503 2022-03-22 15:21:12.000000 dash_mantine_components-0.8.0/MANIFEST.in
--rw-r--r--   0 snehilvijay   (501) staff       (20)     3708 2022-05-01 08:02:49.910786 dash_mantine_components-0.8.0/PKG-INFO
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2568 2022-05-01 07:46:57.000000 dash_mantine_components-0.8.0/README.md
-drwxr-xr-x   0 snehilvijay   (501) staff       (20)        0 2022-05-01 08:02:49.908280 dash_mantine_components-0.8.0/dash_mantine_components/
--rw-r--r--   0 snehilvijay   (501) staff       (20)     3005 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/Accordion.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     1462 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/AccordionItem.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     3782 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/ActionIcon.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2034 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/Affix.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2888 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/Alert.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     3534 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/Anchor.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2410 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/Avatar.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2427 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/AvatarsGroup.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     1661 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/BackgroundImage.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     3121 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/Badge.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2022 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/Blockquote.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     1760 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/Breadcrumbs.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     5075 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/Button.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2872 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/Center.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     3772 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/Checkbox.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     4986 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/Chips.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     1862 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/Code.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     3278 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/Col.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     3704 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/ColorPicker.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     3252 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/Container.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     9560 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/DatePicker.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     9638 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/DateRangePicker.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     1477 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/DemoSlider.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2556 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/Divider.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     5024 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/Drawer.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2424 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/Grid.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2531 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/Group.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     3513 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/Header.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     3898 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/Highlight.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2800 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/Image.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2375 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/InputWrapper.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     4495 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/JsonInput.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     1422 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/Kbd.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2653 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/List.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     1610 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/ListItem.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     1922 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/Loader.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     3705 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/LoadingOverlay.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2022 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/MantineProvider.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     1781 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/Mark.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2253 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/MediaQuery.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     4811 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/Menu.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2759 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/MenuItem.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     1162 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/MenuLabel.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     4893 2022-05-01 08:00:46.000000 dash_mantine_components-0.8.0/dash_mantine_components/Modal.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     8406 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/MultiSelect.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     3992 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/Navbar.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2664 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/Notification.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2703 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/NotificationsProvider.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     4834 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/NumberInput.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     3501 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/Paper.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     3326 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/Prism.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2860 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/Progress.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     4304 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/RadioGroup.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2396 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/RingProgress.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2336 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/ScrollArea.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     4632 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/SegmentedControl.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     8015 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/Select.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2420 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/SimpleGrid.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2740 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/Skeleton.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     6008 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/Slider.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     1716 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/Space.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2492 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/Spoiler.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     3938 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/Switch.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     1851 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/Tab.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2754 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/Table.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     3887 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/Tabs.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     3392 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/Text.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     3721 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/TextInput.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2664 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/ThemeIcon.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     1405 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/ThemeSwitcher.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     5411 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/TimeInput.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2422 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/Timeline.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2573 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/TimelineItem.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     1782 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/Title.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     4967 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/Tooltip.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2581 2022-04-24 09:14:21.000000 dash_mantine_components-0.8.0/dash_mantine_components/__init__.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     3568 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/_imports_.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)   615635 2022-05-01 08:00:43.000000 dash_mantine_components-0.8.0/dash_mantine_components/dash_mantine_components.min.js
--rw-r--r--   0 snehilvijay   (501) staff       (20)      107 2022-05-01 08:00:43.000000 dash_mantine_components-0.8.0/dash_mantine_components/dash_mantine_components.min.js.map
--rw-r--r--   0 snehilvijay   (501) staff       (20)   422064 2022-05-01 08:00:47.000000 dash_mantine_components-0.8.0/dash_mantine_components/metadata.json
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2576 2022-05-01 08:00:44.000000 dash_mantine_components-0.8.0/dash_mantine_components/package-info.json
-drwxr-xr-x   0 snehilvijay   (501) staff       (20)        0 2022-05-01 08:02:49.910333 dash_mantine_components-0.8.0/dash_mantine_components/theme/
--rw-r--r--   0 snehilvijay   (501) staff       (20)      102 2022-04-24 09:14:21.000000 dash_mantine_components-0.8.0/dash_mantine_components/theme/__init__.py
--rw-r--r--   0 snehilvijay   (501) staff       (20)     3043 2022-04-24 09:14:21.000000 dash_mantine_components-0.8.0/dash_mantine_components/theme/default_colors.py
-drwxr-xr-x   0 snehilvijay   (501) staff       (20)        0 2022-05-01 08:02:49.909641 dash_mantine_components-0.8.0/dash_mantine_components.egg-info/
--rw-r--r--   0 snehilvijay   (501) staff       (20)     3708 2022-05-01 08:02:49.000000 dash_mantine_components-0.8.0/dash_mantine_components.egg-info/PKG-INFO
--rw-r--r--   0 snehilvijay   (501) staff       (20)     3306 2022-05-01 08:02:49.000000 dash_mantine_components-0.8.0/dash_mantine_components.egg-info/SOURCES.txt
--rw-r--r--   0 snehilvijay   (501) staff       (20)        1 2022-05-01 08:02:49.000000 dash_mantine_components-0.8.0/dash_mantine_components.egg-info/dependency_links.txt
--rw-r--r--   0 snehilvijay   (501) staff       (20)       24 2022-05-01 08:02:49.000000 dash_mantine_components-0.8.0/dash_mantine_components.egg-info/top_level.txt
--rw-r--r--   0 snehilvijay   (501) staff       (20)     2576 2022-04-26 14:34:53.000000 dash_mantine_components-0.8.0/package.json
--rw-r--r--   0 snehilvijay   (501) staff       (20)       38 2022-05-01 08:02:49.911185 dash_mantine_components-0.8.0/setup.cfg
--rw-r--r--   0 snehilvijay   (501) staff       (20)      723 2022-03-22 15:21:12.000000 dash_mantine_components-0.8.0/setup.py
+drwxr-xr-x   0 snehilvijay   (501) staff       (20)        0 2022-06-01 05:33:19.395117 dash_mantine_components-0.9.0/
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     1068 2022-03-22 15:21:12.000000 dash_mantine_components-0.9.0/LICENSE
+-rw-r--r--   0 snehilvijay   (501) staff       (20)      503 2022-03-22 15:21:12.000000 dash_mantine_components-0.9.0/MANIFEST.in
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     3708 2022-06-01 05:33:19.394825 dash_mantine_components-0.9.0/PKG-INFO
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2568 2022-05-01 07:46:57.000000 dash_mantine_components-0.9.0/README.md
+drwxr-xr-x   0 snehilvijay   (501) staff       (20)        0 2022-06-01 05:33:19.392659 dash_mantine_components-0.9.0/dash_mantine_components/
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     3005 2022-06-01 05:33:16.000000 dash_mantine_components-0.9.0/dash_mantine_components/Accordion.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     1462 2022-06-01 05:33:16.000000 dash_mantine_components-0.9.0/dash_mantine_components/AccordionItem.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     3782 2022-06-01 05:33:16.000000 dash_mantine_components-0.9.0/dash_mantine_components/ActionIcon.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2034 2022-06-01 05:33:16.000000 dash_mantine_components-0.9.0/dash_mantine_components/Affix.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2888 2022-06-01 05:33:16.000000 dash_mantine_components-0.9.0/dash_mantine_components/Alert.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     3534 2022-06-01 05:33:16.000000 dash_mantine_components-0.9.0/dash_mantine_components/Anchor.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2410 2022-06-01 05:33:16.000000 dash_mantine_components-0.9.0/dash_mantine_components/Avatar.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2427 2022-06-01 05:33:16.000000 dash_mantine_components-0.9.0/dash_mantine_components/AvatarsGroup.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     1661 2022-06-01 05:33:16.000000 dash_mantine_components-0.9.0/dash_mantine_components/BackgroundImage.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     3121 2022-06-01 05:33:16.000000 dash_mantine_components-0.9.0/dash_mantine_components/Badge.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2022 2022-06-01 05:33:16.000000 dash_mantine_components-0.9.0/dash_mantine_components/Blockquote.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     1760 2022-06-01 05:33:16.000000 dash_mantine_components-0.9.0/dash_mantine_components/Breadcrumbs.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     5075 2022-06-01 05:33:16.000000 dash_mantine_components-0.9.0/dash_mantine_components/Button.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2872 2022-06-01 05:33:16.000000 dash_mantine_components-0.9.0/dash_mantine_components/Center.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     3772 2022-06-01 05:33:16.000000 dash_mantine_components-0.9.0/dash_mantine_components/Checkbox.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     4986 2022-06-01 05:33:16.000000 dash_mantine_components-0.9.0/dash_mantine_components/Chips.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     1862 2022-06-01 05:33:16.000000 dash_mantine_components-0.9.0/dash_mantine_components/Code.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     3278 2022-06-01 05:33:16.000000 dash_mantine_components-0.9.0/dash_mantine_components/Col.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     3704 2022-06-01 05:33:16.000000 dash_mantine_components-0.9.0/dash_mantine_components/ColorPicker.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     3252 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Container.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     9560 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/DatePicker.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     9638 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/DateRangePicker.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     1477 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/DemoSlider.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2556 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Divider.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     5024 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Drawer.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2424 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Grid.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2556 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Group.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     3513 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Header.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     3898 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Highlight.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2800 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Image.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2375 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/InputWrapper.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     4495 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/JsonInput.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     1422 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Kbd.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2653 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/List.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     1610 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/ListItem.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     1922 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Loader.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     3705 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/LoadingOverlay.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2022 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/MantineProvider.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     1781 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Mark.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2253 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/MediaQuery.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     4811 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Menu.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2759 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/MenuItem.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     1162 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/MenuLabel.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     4893 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Modal.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     8406 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/MultiSelect.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     3992 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Navbar.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2664 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Notification.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2703 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/NotificationsProvider.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     4834 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/NumberInput.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     3896 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Pagination.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     3501 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Paper.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     3928 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/PasswordInput.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     3326 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Prism.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2860 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Progress.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     4304 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/RadioGroup.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2396 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/RingProgress.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2336 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/ScrollArea.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     4632 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/SegmentedControl.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     8015 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Select.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2420 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/SimpleGrid.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2740 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Skeleton.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     6008 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Slider.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     1716 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Space.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2492 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Spoiler.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     1984 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Stack.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     3938 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Switch.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     1851 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Tab.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2754 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Table.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     3887 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Tabs.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     3392 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Text.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     3888 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/TextInput.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2664 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/ThemeIcon.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     1405 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/ThemeSwitcher.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     5411 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/TimeInput.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2422 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Timeline.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2573 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/TimelineItem.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     1782 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Title.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     4967 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/Tooltip.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2581 2022-05-09 19:57:21.000000 dash_mantine_components-0.9.0/dash_mantine_components/__init__.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     3721 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/_imports_.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)   635370 2022-06-01 05:33:14.000000 dash_mantine_components-0.9.0/dash_mantine_components/dash_mantine_components.min.js
+-rw-r--r--   0 snehilvijay   (501) staff       (20)      107 2022-06-01 05:33:14.000000 dash_mantine_components-0.9.0/dash_mantine_components/dash_mantine_components.min.js.map
+-rw-r--r--   0 snehilvijay   (501) staff       (20)   440535 2022-06-01 05:33:17.000000 dash_mantine_components-0.9.0/dash_mantine_components/metadata.json
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2576 2022-06-01 05:33:15.000000 dash_mantine_components-0.9.0/dash_mantine_components/package-info.json
+drwxr-xr-x   0 snehilvijay   (501) staff       (20)        0 2022-06-01 05:33:19.394404 dash_mantine_components-0.9.0/dash_mantine_components/theme/
+-rw-r--r--   0 snehilvijay   (501) staff       (20)      102 2022-04-24 09:14:21.000000 dash_mantine_components-0.9.0/dash_mantine_components/theme/__init__.py
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     3043 2022-04-24 09:14:21.000000 dash_mantine_components-0.9.0/dash_mantine_components/theme/default_colors.py
+drwxr-xr-x   0 snehilvijay   (501) staff       (20)        0 2022-06-01 05:33:19.393851 dash_mantine_components-0.9.0/dash_mantine_components.egg-info/
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     3708 2022-06-01 05:33:19.000000 dash_mantine_components-0.9.0/dash_mantine_components.egg-info/PKG-INFO
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     3418 2022-06-01 05:33:19.000000 dash_mantine_components-0.9.0/dash_mantine_components.egg-info/SOURCES.txt
+-rw-r--r--   0 snehilvijay   (501) staff       (20)        1 2022-06-01 05:33:19.000000 dash_mantine_components-0.9.0/dash_mantine_components.egg-info/dependency_links.txt
+-rw-r--r--   0 snehilvijay   (501) staff       (20)       24 2022-06-01 05:33:19.000000 dash_mantine_components-0.9.0/dash_mantine_components.egg-info/top_level.txt
+-rw-r--r--   0 snehilvijay   (501) staff       (20)     2576 2022-06-01 05:31:13.000000 dash_mantine_components-0.9.0/package.json
+-rw-r--r--   0 snehilvijay   (501) staff       (20)       38 2022-06-01 05:33:19.395217 dash_mantine_components-0.9.0/setup.cfg
+-rw-r--r--   0 snehilvijay   (501) staff       (20)      723 2022-03-22 15:21:12.000000 dash_mantine_components-0.9.0/setup.py
```

### Comparing `dash_mantine_components-0.8.0/LICENSE` & `dash_mantine_components-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/PKG-INFO` & `dash_mantine_components-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash_mantine_components
-Version: 0.8.0
+Version: 0.9.0
 Summary: Plotly Dash components based on Mantine
 Home-page: https://github.com/snehilvj/dash-mantine-components
 Author: Snehil Vijay <snehilvj@outlook.com>
 Author-email: snehilvj@outlook.com
 License: MIT
 Description: <p align="center">
             <img src="https://raw.githubusercontent.com/snehilvj/dash-mantine-components/master/assets/logo.png" alt="logo" width=300 >
```

### Comparing `dash_mantine_components-0.8.0/README.md` & `dash_mantine_components-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Accordion.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Accordion.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/AccordionItem.py` & `dash_mantine_components-0.9.0/dash_mantine_components/AccordionItem.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/ActionIcon.py` & `dash_mantine_components-0.9.0/dash_mantine_components/ActionIcon.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Affix.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Affix.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Alert.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Alert.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Anchor.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Anchor.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Avatar.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Avatar.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/AvatarsGroup.py` & `dash_mantine_components-0.9.0/dash_mantine_components/AvatarsGroup.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/BackgroundImage.py` & `dash_mantine_components-0.9.0/dash_mantine_components/BackgroundImage.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Badge.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Badge.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Blockquote.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Blockquote.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Breadcrumbs.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Button.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Button.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Center.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Center.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Checkbox.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Checkbox.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Chips.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Chips.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Code.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Code.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Col.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Col.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/ColorPicker.py` & `dash_mantine_components-0.9.0/dash_mantine_components/ColorPicker.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Container.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Container.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/DatePicker.py` & `dash_mantine_components-0.9.0/dash_mantine_components/DatePicker.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/DateRangePicker.py` & `dash_mantine_components-0.9.0/dash_mantine_components/DateRangePicker.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/DemoSlider.py` & `dash_mantine_components-0.9.0/dash_mantine_components/DemoSlider.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Divider.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Divider.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Drawer.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Drawer.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Grid.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Grid.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Group.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Group.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 class Group(Component):
     """A Group component.
 Compose elements and components in flex container. For more information, see: https://mantine.dev/core/group/
 
 Keyword arguments:
 
 - children (a list of or a singular dash component, string or number; optional):
-    Content.
+    Primary content inside the stack.
 
 - id (string; optional):
     The ID of this component, used to identify dash components in
     callbacks.
 
 - align (a value equal to: "stretch", "center", "flex-end", "flex-start"; optional):
     Defines align-items css property.
```

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Header.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Header.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Highlight.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Highlight.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Image.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Image.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/InputWrapper.py` & `dash_mantine_components-0.9.0/dash_mantine_components/InputWrapper.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/JsonInput.py` & `dash_mantine_components-0.9.0/dash_mantine_components/JsonInput.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Kbd.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Kbd.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/List.py` & `dash_mantine_components-0.9.0/dash_mantine_components/List.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/ListItem.py` & `dash_mantine_components-0.9.0/dash_mantine_components/ListItem.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Loader.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Loader.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/LoadingOverlay.py` & `dash_mantine_components-0.9.0/dash_mantine_components/LoadingOverlay.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/MantineProvider.py` & `dash_mantine_components-0.9.0/dash_mantine_components/MantineProvider.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Mark.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Mark.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/MediaQuery.py` & `dash_mantine_components-0.9.0/dash_mantine_components/MediaQuery.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Menu.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Menu.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/MenuItem.py` & `dash_mantine_components-0.9.0/dash_mantine_components/MenuItem.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/MenuLabel.py` & `dash_mantine_components-0.9.0/dash_mantine_components/MenuLabel.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Modal.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Modal.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/MultiSelect.py` & `dash_mantine_components-0.9.0/dash_mantine_components/MultiSelect.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Navbar.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Navbar.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Notification.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Notification.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/NotificationsProvider.py` & `dash_mantine_components-0.9.0/dash_mantine_components/NotificationsProvider.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/NumberInput.py` & `dash_mantine_components-0.9.0/dash_mantine_components/NumberInput.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Paper.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Paper.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Prism.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Prism.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Progress.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Progress.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/RadioGroup.py` & `dash_mantine_components-0.9.0/dash_mantine_components/RadioGroup.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/RingProgress.py` & `dash_mantine_components-0.9.0/dash_mantine_components/RingProgress.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/ScrollArea.py` & `dash_mantine_components-0.9.0/dash_mantine_components/ScrollArea.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/SegmentedControl.py` & `dash_mantine_components-0.9.0/dash_mantine_components/SegmentedControl.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Select.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Select.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/SimpleGrid.py` & `dash_mantine_components-0.9.0/dash_mantine_components/SimpleGrid.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Skeleton.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Skeleton.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Slider.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Slider.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Space.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Space.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Spoiler.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Spoiler.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Switch.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Switch.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Tab.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Tab.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Table.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Table.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Tabs.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Tabs.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Text.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Text.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/TextInput.py` & `dash_mantine_components-0.9.0/dash_mantine_components/TextInput.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,27 +53,30 @@
 
 - size (a value equal to: "xs", "sm", "md", "lg", "xl"; optional):
     Input size.
 
 - style (dict; optional):
     Inline style override.
 
+- type (a value equal to: "number", "search", "text", "tel", "url", "email", "password"; optional):
+    Input element type.
+
 - value (a list of or a singular dash component, string or number; default ""):
     Input value.
 
 - variant (a value equal to: "default", "filled", "unstyled", "headless"; optional):
     Defines input appearance, defaults to default in light color
     scheme and filled in dark."""
     @_explicitize_args
-    def __init__(self, class_name=Component.UNDEFINED, description=Component.UNDEFINED, disabled=Component.UNDEFINED, error=Component.UNDEFINED, icon=Component.UNDEFINED, iconWidth=Component.UNDEFINED, id=Component.UNDEFINED, label=Component.UNDEFINED, placeholder=Component.UNDEFINED, radius=Component.UNDEFINED, required=Component.UNDEFINED, rightSection=Component.UNDEFINED, rightSectionWidth=Component.UNDEFINED, size=Component.UNDEFINED, style=Component.UNDEFINED, value=Component.UNDEFINED, variant=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', 'class_name', 'description', 'disabled', 'error', 'icon', 'iconWidth', 'label', 'placeholder', 'radius', 'required', 'rightSection', 'rightSectionWidth', 'size', 'style', 'value', 'variant']
+    def __init__(self, class_name=Component.UNDEFINED, description=Component.UNDEFINED, disabled=Component.UNDEFINED, error=Component.UNDEFINED, icon=Component.UNDEFINED, iconWidth=Component.UNDEFINED, id=Component.UNDEFINED, label=Component.UNDEFINED, placeholder=Component.UNDEFINED, radius=Component.UNDEFINED, required=Component.UNDEFINED, rightSection=Component.UNDEFINED, rightSectionWidth=Component.UNDEFINED, size=Component.UNDEFINED, style=Component.UNDEFINED, type=Component.UNDEFINED, value=Component.UNDEFINED, variant=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['id', 'class_name', 'description', 'disabled', 'error', 'icon', 'iconWidth', 'label', 'placeholder', 'radius', 'required', 'rightSection', 'rightSectionWidth', 'size', 'style', 'type', 'value', 'variant']
         self._type = 'TextInput'
         self._namespace = 'dash_mantine_components'
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', 'class_name', 'description', 'disabled', 'error', 'icon', 'iconWidth', 'label', 'placeholder', 'radius', 'required', 'rightSection', 'rightSectionWidth', 'size', 'style', 'value', 'variant']
+        self.available_properties = ['id', 'class_name', 'description', 'disabled', 'error', 'icon', 'iconWidth', 'label', 'placeholder', 'radius', 'required', 'rightSection', 'rightSectionWidth', 'size', 'style', 'type', 'value', 'variant']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs
         args = {k: _locals[k] for k in _explicit_args if k != 'children'}
         for k in []:
             if k not in args:
```

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/ThemeIcon.py` & `dash_mantine_components-0.9.0/dash_mantine_components/ThemeIcon.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/ThemeSwitcher.py` & `dash_mantine_components-0.9.0/dash_mantine_components/ThemeSwitcher.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/TimeInput.py` & `dash_mantine_components-0.9.0/dash_mantine_components/TimeInput.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Timeline.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Timeline.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/TimelineItem.py` & `dash_mantine_components-0.9.0/dash_mantine_components/TimelineItem.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Title.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Title.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/Tooltip.py` & `dash_mantine_components-0.9.0/dash_mantine_components/Tooltip.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/__init__.py` & `dash_mantine_components-0.9.0/dash_mantine_components/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/_imports_.py` & `dash_mantine_components-0.9.0/dash_mantine_components/_imports_.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,27 +43,30 @@
 from .MenuLabel import MenuLabel
 from .Modal import Modal
 from .MultiSelect import MultiSelect
 from .Navbar import Navbar
 from .Notification import Notification
 from .NotificationsProvider import NotificationsProvider
 from .NumberInput import NumberInput
+from .Pagination import Pagination
 from .Paper import Paper
+from .PasswordInput import PasswordInput
 from .Prism import Prism
 from .Progress import Progress
 from .RadioGroup import RadioGroup
 from .RingProgress import RingProgress
 from .ScrollArea import ScrollArea
 from .SegmentedControl import SegmentedControl
 from .Select import Select
 from .SimpleGrid import SimpleGrid
 from .Skeleton import Skeleton
 from .Slider import Slider
 from .Space import Space
 from .Spoiler import Spoiler
+from .Stack import Stack
 from .Switch import Switch
 from .Tab import Tab
 from .Table import Table
 from .Tabs import Tabs
 from .Text import Text
 from .TextInput import TextInput
 from .ThemeIcon import ThemeIcon
@@ -120,27 +123,30 @@
     "MenuLabel",
     "Modal",
     "MultiSelect",
     "Navbar",
     "Notification",
     "NotificationsProvider",
     "NumberInput",
+    "Pagination",
     "Paper",
+    "PasswordInput",
     "Prism",
     "Progress",
     "RadioGroup",
     "RingProgress",
     "ScrollArea",
     "SegmentedControl",
     "Select",
     "SimpleGrid",
     "Skeleton",
     "Slider",
     "Space",
     "Spoiler",
+    "Stack",
     "Switch",
     "Tab",
     "Table",
     "Tabs",
     "Text",
     "TextInput",
     "ThemeIcon",
```

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/dash_mantine_components.min.js` & `dash_mantine_components-0.9.0/dash_mantine_components/dash_mantine_components.min.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -64,15 +64,15 @@
             var t = function(e) {
                     return /\/_dash-component-suites\//.test(e.src)
                 }(a()),
                 r = o(e);
             if (!t) return r;
             var n = r.split("/"),
                 i = n.slice(-1)[0].split(".");
-            return i.splice(1, 0, "v0_8_0m1651392035"), n.splice(-1, 1, i.join(".")), n.join("/")
+            return i.splice(1, 0, "v0_9_0m1654061588"), n.splice(-1, 1, i.join(".")), n.join("/")
         }
     }
     return r(r.s = 16)
 }([function(e, t) {
     e.exports = window.React
 }, function(e, t) {
     e.exports = window.PropTypes
@@ -16143,73 +16143,400 @@
         radius: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         required: i.a.bool,
         rightSection: i.a.any,
         rightSectionWidth: i.a.number,
         setProps: i.a.func,
         size: i.a.oneOf(["xs", "sm", "md", "lg", "xl"]),
         style: i.a.object,
+        type: i.a.oneOf(["number", "search", "text", "tel", "url", "email", "password"]),
         value: i.a.node,
         variant: i.a.oneOf(["default", "filled", "unstyled", "headless"])
     };
-    var hO = yO,
-        vO = Object.defineProperty,
-        OO = Object.getOwnPropertySymbols,
-        wO = Object.prototype.hasOwnProperty,
-        xO = Object.prototype.propertyIsEnumerable,
-        SO = (e, t, r) => t in e ? vO(e, t, {
+    var hO = yO;
+
+    function vO(e = !1) {
+        return function(e, t) {
+            const [r, a] = Object(n.useState)(e);
+            return [r, e => {
+                a(void 0 !== e ? e : e => e === t[0] ? t[1] : t[0])
+            }]
+        }(e, [!0, !1])
+    }
+    var OO = Object.defineProperty,
+        wO = Object.defineProperties,
+        xO = Object.getOwnPropertyDescriptors,
+        SO = Object.getOwnPropertySymbols,
+        kO = Object.prototype.hasOwnProperty,
+        EO = Object.prototype.propertyIsEnumerable,
+        jO = (e, t, r) => t in e ? OO(e, t, {
+            enumerable: !0,
+            configurable: !0,
+            writable: !0,
+            value: r
+        }) : e[t] = r,
+        PO = (e, t) => {
+            for (var r in t || (t = {})) kO.call(t, r) && jO(e, r, t[r]);
+            if (SO)
+                for (var r of SO(t)) EO.call(t, r) && jO(e, r, t[r]);
+            return e
+        },
+        zO = Er((e, {
+            size: t,
+            rightSectionWidth: r
+        }) => {
+            return {
+                visibilityToggle: {},
+                input: {
+                    position: "relative",
+                    overflow: "hidden"
+                },
+                innerInput: (n = PO({}, e.fn.fontStyles()), a = {
+                    backgroundColor: "transparent",
+                    border: 0,
+                    boxSizing: "border-box",
+                    position: "absolute",
+                    display: "block",
+                    width: `calc(100% - ${r}px)`,
+                    paddingLeft: e.fn.size({
+                        size: t,
+                        sizes: _r
+                    }) / 3,
+                    fontSize: e.fn.size({
+                        size: t,
+                        sizes: e.fontSizes
+                    }),
+                    height: e.fn.size({
+                        size: t,
+                        sizes: _r
+                    }) - 2,
+                    lineHeight: e.fn.size({
+                        size: t,
+                        sizes: _r
+                    }) - 2 + "px",
+                    color: "dark" === e.colorScheme ? e.colors.dark[0] : e.black,
+                    top: 0,
+                    bottom: 0,
+                    left: 0,
+                    right: 0,
+                    "&:focus": {
+                        outline: 0
+                    },
+                    "&:disabled": {
+                        cursor: "not-allowed"
+                    },
+                    "&::placeholder": {
+                        opacity: 1,
+                        userSelect: "none",
+                        color: "dark" === e.colorScheme ? e.colors.dark[3] : e.colors.gray[5]
+                    }
+                }, wO(n, xO(a))),
+                invalid: {
+                    color: e.colors.red["dark" === e.colorScheme ? 6 : 7],
+                    "&::placeholder": {
+                        opacity: 1,
+                        color: e.colors.red["dark" === e.colorScheme ? 6 : 7]
+                    }
+                },
+                withIcon: {
+                    paddingLeft: e.fn.size({
+                        size: t,
+                        sizes: _r
+                    }) + "px !important"
+                }
+            };
+            var n, a
+        }),
+        CO = Object.defineProperty,
+        NO = Object.defineProperties,
+        TO = Object.getOwnPropertyDescriptors,
+        DO = Object.getOwnPropertySymbols,
+        IO = Object.prototype.hasOwnProperty,
+        RO = Object.prototype.propertyIsEnumerable,
+        _O = (e, t, r) => t in e ? CO(e, t, {
+            enumerable: !0,
+            configurable: !0,
+            writable: !0,
+            value: r
+        }) : e[t] = r,
+        LO = (e, t) => {
+            for (var r in t || (t = {})) IO.call(t, r) && _O(e, r, t[r]);
+            if (DO)
+                for (var r of DO(t)) RO.call(t, r) && _O(e, r, t[r]);
+            return e
+        };
+    const AO = {
+            xs: 22,
+            sm: 28,
+            md: 26,
+            lg: 32,
+            xl: 40
+        },
+        MO = {
+            xs: 12,
+            sm: 15,
+            md: 17,
+            lg: 19,
+            xl: 21
+        },
+        FO = {
+            xs: 28,
+            sm: 34,
+            md: 34,
+            lg: 44,
+            xl: 54
+        },
+        $O = {
+            size: "sm",
+            toggleTabIndex: -1,
+            visibilityToggleIcon: ({
+                reveal: e,
+                size: t = 15
+            }) => a.a.createElement("svg", {
+                width: t,
+                height: t,
+                viewBox: "0 0 15 15",
+                fill: "none",
+                xmlns: "http://www.w3.org/2000/svg"
+            }, a.a.createElement("path", {
+                d: e ? "M13.3536 2.35355C13.5488 2.15829 13.5488 1.84171 13.3536 1.64645C13.1583 1.45118 12.8417 1.45118 12.6464 1.64645L10.6828 3.61012C9.70652 3.21671 8.63759 3 7.5 3C4.30786 3 1.65639 4.70638 0.0760002 7.23501C-0.0253338 7.39715 -0.0253334 7.60288 0.0760014 7.76501C0.902945 9.08812 2.02314 10.1861 3.36061 10.9323L1.64645 12.6464C1.45118 12.8417 1.45118 13.1583 1.64645 13.3536C1.84171 13.5488 2.15829 13.5488 2.35355 13.3536L4.31723 11.3899C5.29348 11.7833 6.36241 12 7.5 12C10.6921 12 13.3436 10.2936 14.924 7.76501C15.0253 7.60288 15.0253 7.39715 14.924 7.23501C14.0971 5.9119 12.9769 4.81391 11.6394 4.06771L13.3536 2.35355ZM9.90428 4.38861C9.15332 4.1361 8.34759 4 7.5 4C4.80285 4 2.52952 5.37816 1.09622 7.50001C1.87284 8.6497 2.89609 9.58106 4.09974 10.1931L9.90428 4.38861ZM5.09572 10.6114L10.9003 4.80685C12.1039 5.41894 13.1272 6.35031 13.9038 7.50001C12.4705 9.62183 10.1971 11 7.5 11C6.65241 11 5.84668 10.8639 5.09572 10.6114Z" : "M7.5 11C4.80285 11 2.52952 9.62184 1.09622 7.50001C2.52952 5.37816 4.80285 4 7.5 4C10.1971 4 12.4705 5.37816 13.9038 7.50001C12.4705 9.62183 10.1971 11 7.5 11ZM7.5 3C4.30786 3 1.65639 4.70638 0.0760002 7.23501C-0.0253338 7.39715 -0.0253334 7.60288 0.0760014 7.76501C1.65639 10.2936 4.30786 12 7.5 12C10.6921 12 13.3436 10.2936 14.924 7.76501C15.0253 7.60288 15.0253 7.39715 14.924 7.23501C13.3436 4.70638 10.6921 3 7.5 3ZM7.5 9.5C8.60457 9.5 9.5 8.60457 9.5 7.5C9.5 6.39543 8.60457 5.5 7.5 5.5C6.39543 5.5 5.5 6.39543 5.5 7.5C5.5 8.60457 6.39543 9.5 7.5 9.5Z",
+                fill: "currentColor",
+                fillRule: "evenodd",
+                clipRule: "evenodd"
+            })),
+            __staticSelector: "PasswordInput"
+        },
+        BO = Object(n.forwardRef)((e, t) => {
+            const r = ir("PasswordInput", $O, e),
+                {
+                    radius: n,
+                    disabled: o,
+                    size: i,
+                    toggleTabIndex: l,
+                    className: s,
+                    id: c,
+                    label: u,
+                    error: d,
+                    required: p,
+                    style: f,
+                    icon: m,
+                    description: b,
+                    wrapperProps: g,
+                    classNames: y,
+                    styles: h,
+                    variant: v,
+                    visibilityToggleIcon: O,
+                    __staticSelector: w,
+                    rightSection: x,
+                    rightSectionWidth: S,
+                    rightSectionProps: k,
+                    sx: E,
+                    labelProps: j,
+                    descriptionProps: P,
+                    errorProps: z
+                } = r,
+                C = ((e, t) => {
+                    var r = {};
+                    for (var n in e) IO.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && DO)
+                        for (var n of DO(e)) t.indexOf(n) < 0 && RO.call(e, n) && (r[n] = e[n]);
+                    return r
+                })(r, ["radius", "disabled", "size", "toggleTabIndex", "className", "id", "label", "error", "required", "style", "icon", "description", "wrapperProps", "classNames", "styles", "variant", "visibilityToggleIcon", "__staticSelector", "rightSection", "rightSectionWidth", "rightSectionProps", "sx", "labelProps", "descriptionProps", "errorProps"]),
+                N = or(),
+                T = N.fn.size({
+                    size: i,
+                    sizes: FO
+                }),
+                {
+                    classes: D,
+                    cx: I
+                } = zO({
+                    size: i,
+                    rightSectionWidth: T
+                }, {
+                    name: "PasswordInput",
+                    classNames: y,
+                    styles: h
+                }),
+                R = Ja(c),
+                {
+                    systemStyles: _,
+                    rest: L
+                } = gn(C),
+                [A, M] = vO(!1),
+                F = a.a.createElement(ol, {
+                    className: D.visibilityToggle,
+                    tabIndex: l,
+                    radius: n,
+                    size: N.fn.size({
+                        size: i,
+                        sizes: AO
+                    }),
+                    "aria-hidden": !0,
+                    onMouseDown: e => {
+                        e.preventDefault(), M()
+                    },
+                    onKeyDown: e => {
+                        "Space" === e.nativeEvent.code && (e.preventDefault(), M())
+                    }
+                }, a.a.createElement(O, {
+                    reveal: A,
+                    size: N.fn.size({
+                        size: i,
+                        sizes: MO
+                    })
+                }));
+            return a.a.createElement(Ao, LO(LO({
+                required: p,
+                id: R,
+                label: u,
+                error: d,
+                description: b,
+                size: i,
+                className: s,
+                style: f,
+                classNames: y,
+                styles: h,
+                __staticSelector: w,
+                sx: E,
+                errorProps: z,
+                descriptionProps: P,
+                labelProps: j
+            }, _), g), a.a.createElement(zc, {
+                component: "div",
+                invalid: !!d,
+                icon: m,
+                size: i,
+                classNames: ($ = LO({}, y), B = {
+                    input: D.input
+                }, NO($, TO(B))),
+                styles: h,
+                radius: n,
+                disabled: o,
+                __staticSelector: w,
+                rightSectionWidth: T,
+                rightSection: !o && F,
+                variant: v
+            }, a.a.createElement("input", LO({
+                type: A ? "text" : "password",
+                required: p,
+                className: I(D.innerInput, {
+                    [D.withIcon]: m,
+                    [D.invalid]: !!d
+                }),
+                disabled: o,
+                id: R,
+                ref: t
+            }, L))));
+            var $, B
+        });
+
+    function WO() {
+        return (WO = Object.assign || function(e) {
+            for (var t = 1; t < arguments.length; t++) {
+                var r = arguments[t];
+                for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
+            }
+            return e
+        }).apply(this, arguments)
+    }
+    BO.displayName = "@mantine/core/PasswordInput";
+    var HO = function(e) {
+        var t = e.setProps,
+            r = e.class_name,
+            n = G(["setProps", "class_name"], e);
+        n = ta(n, ["label", "description", "rightSection", "icon", "error"]);
+        return a.a.createElement(BO, WO({}, n, {
+            className: r,
+            onChange: function(e) {
+                return r = e.currentTarget.value, void t({
+                    value: r
+                });
+                var r
+            }
+        }))
+    };
+    HO.displayName = "PasswordInput", HO.defaultProps = {
+        value: ""
+    }, HO.propTypes = {
+        class_name: i.a.string,
+        description: i.a.any,
+        disabled: i.a.bool,
+        error: i.a.any,
+        icon: i.a.any,
+        iconWidth: i.a.number,
+        id: i.a.string,
+        label: i.a.any,
+        placeholder: i.a.string,
+        radius: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
+        required: i.a.bool,
+        rightSection: i.a.any,
+        rightSectionWidth: i.a.number,
+        setProps: i.a.func,
+        size: i.a.oneOf(["xs", "sm", "md", "lg", "xl"]),
+        style: i.a.object,
+        type: i.a.oneOf(["number", "search", "text", "tel", "url", "email", "password"]),
+        value: i.a.node,
+        variant: i.a.oneOf(["default", "filled", "unstyled", "headless"])
+    };
+    var VO = HO,
+        qO = Object.defineProperty,
+        UO = Object.getOwnPropertySymbols,
+        GO = Object.prototype.hasOwnProperty,
+        YO = Object.prototype.propertyIsEnumerable,
+        ZO = (e, t, r) => t in e ? qO(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const kO = Object(n.forwardRef)((e, t) => {
+    const KO = Object(n.forwardRef)((e, t) => {
         const r = ir("Center", {}, e),
             {
                 inline: n,
                 sx: o
             } = r,
             i = ((e, t) => {
                 var r = {};
-                for (var n in e) wO.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                if (null != e && OO)
-                    for (var n of OO(e)) t.indexOf(n) < 0 && xO.call(e, n) && (r[n] = e[n]);
+                for (var n in e) GO.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                if (null != e && UO)
+                    for (var n of UO(e)) t.indexOf(n) < 0 && YO.call(e, n) && (r[n] = e[n]);
                 return r
             })(r, ["inline", "sx"]);
         return a.a.createElement(Cn, ((e, t) => {
-            for (var r in t || (t = {})) wO.call(t, r) && SO(e, r, t[r]);
-            if (OO)
-                for (var r of OO(t)) xO.call(t, r) && SO(e, r, t[r]);
+            for (var r in t || (t = {})) GO.call(t, r) && ZO(e, r, t[r]);
+            if (UO)
+                for (var r of UO(t)) YO.call(t, r) && ZO(e, r, t[r]);
             return e
         })({
             ref: t,
             sx: [{
                 display: n ? "inline-flex" : "flex",
                 alignItems: "center",
                 justifyContent: "center"
             }, ...Array.isArray(o) ? o : [o]]
         }, i))
     });
 
-    function EO() {
-        return (EO = Object.assign || function(e) {
+    function XO() {
+        return (XO = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    kO.displayName = "@mantine/core/Center";
-    var jO = function(e) {
+    KO.displayName = "@mantine/core/Center";
+    var JO = function(e) {
         var t = e.class_name;
-        return a.a.createElement(kO, EO({}, G(["children", "setProps", "class_name"], e), {
+        return a.a.createElement(KO, XO({}, G(["children", "setProps", "class_name"], e), {
             className: t
         }), e.children)
     };
-    jO.displayName = "Center", jO.defaultProps = {}, jO.propTypes = {
+    JO.displayName = "Center", JO.defaultProps = {}, JO.propTypes = {
         children: i.a.node,
         class_name: i.a.string,
         id: i.a.string,
         m: i.a.oneOfType([i.a.string, i.a.number]),
         my: i.a.oneOfType([i.a.string, i.a.number]),
         mx: i.a.oneOfType([i.a.string, i.a.number]),
         mt: i.a.oneOfType([i.a.string, i.a.number]),
@@ -16221,106 +16548,106 @@
         px: i.a.oneOfType([i.a.string, i.a.number]),
         pt: i.a.oneOfType([i.a.string, i.a.number]),
         pb: i.a.oneOfType([i.a.string, i.a.number]),
         pl: i.a.oneOfType([i.a.string, i.a.number]),
         pr: i.a.oneOfType([i.a.string, i.a.number]),
         style: i.a.object
     };
-    var PO = jO,
-        zO = Er((e, {
+    var QO = JO,
+        ew = Er((e, {
             fluid: t,
             size: r,
             sizes: n
         }) => ({
             root: {
                 maxWidth: t ? "100%" : e.fn.size({
                     size: r,
                     sizes: n
                 }),
                 marginLeft: "auto",
                 marginRight: "auto"
             }
         })),
-        CO = Object.defineProperty,
-        NO = Object.getOwnPropertySymbols,
-        TO = Object.prototype.hasOwnProperty,
-        DO = Object.prototype.propertyIsEnumerable,
-        IO = (e, t, r) => t in e ? CO(e, t, {
+        tw = Object.defineProperty,
+        rw = Object.getOwnPropertySymbols,
+        nw = Object.prototype.hasOwnProperty,
+        aw = Object.prototype.propertyIsEnumerable,
+        ow = (e, t, r) => t in e ? tw(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const RO = {
+    const iw = {
             px: "md",
             sizes: {
                 xs: 540,
                 sm: 720,
                 md: 960,
                 lg: 1140,
                 xl: 1320
             }
         },
-        _O = Object(n.forwardRef)((e, t) => {
-            const r = ir("Container", RO, e),
+        lw = Object(n.forwardRef)((e, t) => {
+            const r = ir("Container", iw, e),
                 {
                     className: n,
                     fluid: o,
                     size: i,
                     styles: l,
                     classNames: s,
                     sizes: c
                 } = r,
                 u = ((e, t) => {
                     var r = {};
-                    for (var n in e) TO.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && NO)
-                        for (var n of NO(e)) t.indexOf(n) < 0 && DO.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) nw.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && rw)
+                        for (var n of rw(e)) t.indexOf(n) < 0 && aw.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["className", "fluid", "size", "styles", "classNames", "sizes"]),
                 {
                     classes: d,
                     cx: p
-                } = zO({
+                } = ew({
                     fluid: o,
                     size: i,
                     sizes: c
                 }, {
                     styles: l,
                     classNames: s,
                     name: "Container"
                 });
             return a.a.createElement(Cn, ((e, t) => {
-                for (var r in t || (t = {})) TO.call(t, r) && IO(e, r, t[r]);
-                if (NO)
-                    for (var r of NO(t)) DO.call(t, r) && IO(e, r, t[r]);
+                for (var r in t || (t = {})) nw.call(t, r) && ow(e, r, t[r]);
+                if (rw)
+                    for (var r of rw(t)) aw.call(t, r) && ow(e, r, t[r]);
                 return e
             })({
                 className: p(d.root, n),
                 ref: t
             }, u))
         });
 
-    function LO() {
-        return (LO = Object.assign || function(e) {
+    function sw() {
+        return (sw = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    _O.displayName = "@mantine/core/Container";
-    var AO = function(e) {
+    lw.displayName = "@mantine/core/Container";
+    var cw = function(e) {
         var t = e.class_name;
-        return a.a.createElement(_O, LO({}, G(["children", "setProps", "class_name"], e), {
+        return a.a.createElement(lw, sw({}, G(["children", "setProps", "class_name"], e), {
             className: t
         }), e.children)
     };
-    AO.displayName = "Container", AO.defaultProps = {}, AO.propTypes = {
+    cw.displayName = "Container", cw.defaultProps = {}, cw.propTypes = {
         children: i.a.node,
         class_name: i.a.string,
         fluid: i.a.bool,
         id: i.a.string,
         size: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         style: i.a.object,
         m: i.a.oneOfType([i.a.string, i.a.number]),
@@ -16334,99 +16661,99 @@
         py: i.a.oneOfType([i.a.string, i.a.number]),
         px: i.a.oneOfType([i.a.string, i.a.number]),
         pt: i.a.oneOfType([i.a.string, i.a.number]),
         pb: i.a.oneOfType([i.a.string, i.a.number]),
         pl: i.a.oneOfType([i.a.string, i.a.number]),
         pr: i.a.oneOfType([i.a.string, i.a.number])
     };
-    var MO = AO;
-    const FO = {
+    var uw = cw;
+    const dw = {
             x: 0,
             y: 0,
             width: 0,
             height: 0,
             top: 0,
             left: 0,
             bottom: 0,
             right: 0
         },
-        $O = "undefined" != typeof window;
+        pw = "undefined" != typeof window;
 
-    function BO() {
+    function fw() {
         const e = Object(n.useRef)(0),
             t = Object(n.useRef)(null),
-            [r, a] = Object(n.useState)(FO),
-            o = Object(n.useMemo)(() => $O ? new ResizeObserver(r => {
+            [r, a] = Object(n.useState)(dw),
+            o = Object(n.useMemo)(() => pw ? new ResizeObserver(r => {
                 const n = r[0];
                 n && (cancelAnimationFrame(e.current), e.current = requestAnimationFrame(() => {
                     t.current && a(n.contentRect)
                 }))
             }) : null, []);
         return Object(n.useEffect)(() => (t.current && o.observe(t.current), () => {
             o.disconnect(), e.current && cancelAnimationFrame(e.current)
         }), [t.current]), [t, r]
     }
-    var WO = Object.defineProperty,
-        HO = Object.defineProperties,
-        VO = Object.getOwnPropertyDescriptors,
-        qO = Object.getOwnPropertySymbols,
-        UO = Object.prototype.hasOwnProperty,
-        GO = Object.prototype.propertyIsEnumerable,
-        YO = (e, t, r) => t in e ? WO(e, t, {
+    var mw = Object.defineProperty,
+        bw = Object.defineProperties,
+        gw = Object.getOwnPropertyDescriptors,
+        yw = Object.getOwnPropertySymbols,
+        hw = Object.prototype.hasOwnProperty,
+        vw = Object.prototype.propertyIsEnumerable,
+        Ow = (e, t, r) => t in e ? mw(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        ZO = (e, t) => {
-            for (var r in t || (t = {})) UO.call(t, r) && YO(e, r, t[r]);
-            if (qO)
-                for (var r of qO(t)) GO.call(t, r) && YO(e, r, t[r]);
+        ww = (e, t) => {
+            for (var r in t || (t = {})) hw.call(t, r) && Ow(e, r, t[r]);
+            if (yw)
+                for (var r of yw(t)) vw.call(t, r) && Ow(e, r, t[r]);
             return e
         };
-    const KO = {
+    const xw = {
         xs: "3px 6px",
         sm: "5px 10px",
         md: "7px 14px",
         lg: "9px 16px",
         xl: "12px 20px"
     };
-    var XO = Er((e, {
+    var Sw = Er((e, {
             fullWidth: t,
             color: r,
             radius: n,
             shouldAnimate: a,
             transitionDuration: o,
             transitionTimingFunction: i,
             size: l,
             orientation: s
         }, c) => {
             const u = "vertical" === s;
             return {
-                label: (d = ZO(ZO({
+                label: (d = ww(ww({
                     ref: c("label")
                 }, e.fn.focusStyles()), e.fn.fontStyles()), p = {
                     WebkitTapHighlightColor: "transparent",
                     borderRadius: e.fn.radius(n),
                     fontWeight: 500,
                     fontSize: l in e.fontSizes ? e.fontSizes[l] : e.fontSizes.sm,
                     cursor: "pointer",
                     display: "block",
                     textAlign: "center",
-                    padding: KO[l in KO ? l : "sm"],
+                    padding: xw[l in xw ? l : "sm"],
                     whiteSpace: "nowrap",
                     overflow: "hidden",
                     textOverflow: "ellipsis",
                     userSelect: "none",
                     color: "dark" === e.colorScheme ? e.colors.dark[1] : e.colors.gray[7],
                     transition: `color ${a?0:o}ms ${i||e.transitionTimingFunction}`,
                     "&:hover": {
                         color: "dark" === e.colorScheme ? e.colors.dark[0] : e.black
                     }
-                }, HO(d, VO(p))),
+                }, bw(d, gw(p))),
                 control: {
                     ref: c("control"),
                     position: "relative",
                     boxSizing: "border-box",
                     flex: 1,
                     zIndex: 2,
                     transition: `border-left-color ${a?0:o}ms ${i||e.transitionTimingFunction}`,
@@ -16492,31 +16819,31 @@
                     boxShadow: r || "dark" === e.colorScheme ? "none" : e.shadows.xs,
                     transition: `transform ${a?0:o}ms ${e.transitionTimingFunction}, width ${a?0:o/2}ms ${i||e.transitionTimingFunction}`,
                     backgroundColor: r in e.colors ? e.fn.themeColor(r, 6) : "dark" === e.colorScheme ? e.colors.dark[5] : e.white
                 }
             };
             var d, p
         }),
-        JO = Object.defineProperty,
-        QO = Object.getOwnPropertySymbols,
-        ew = Object.prototype.hasOwnProperty,
-        tw = Object.prototype.propertyIsEnumerable,
-        rw = (e, t, r) => t in e ? JO(e, t, {
+        kw = Object.defineProperty,
+        Ew = Object.getOwnPropertySymbols,
+        jw = Object.prototype.hasOwnProperty,
+        Pw = Object.prototype.propertyIsEnumerable,
+        zw = (e, t, r) => t in e ? kw(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const nw = {
+    const Cw = {
             disabled: !1,
             size: "sm",
             transitionDuration: 200
         },
-        aw = Object(n.forwardRef)((e, t) => {
-            const r = ir("SegmentedControl", nw, e),
+        Nw = Object(n.forwardRef)((e, t) => {
+            const r = ir("SegmentedControl", Cw, e),
                 {
                     className: o,
                     disabled: i,
                     data: l,
                     name: s,
                     value: c,
                     onChange: u,
@@ -16529,17 +16856,17 @@
                     classNames: y,
                     styles: h,
                     defaultValue: v,
                     orientation: O
                 } = r,
                 w = ((e, t) => {
                     var r = {};
-                    for (var n in e) ew.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && QO)
-                        for (var n of QO(e)) t.indexOf(n) < 0 && tw.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) jw.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && Ew)
+                        for (var n of Ew(e)) t.indexOf(n) < 0 && Pw.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["className", "disabled", "data", "name", "value", "onChange", "color", "fullWidth", "radius", "size", "transitionDuration", "transitionTimingFunction", "classNames", "styles", "defaultValue", "orientation"]),
                 x = vd(),
                 S = l.map(e => "string" == typeof e ? {
                     label: e,
                     value: e
                 } : e),
@@ -16551,15 +16878,15 @@
                     onChange: u,
                     rule: e => !!e
                 }),
                 {
                     classes: z,
                     cx: C,
                     theme: N
-                } = XO({
+                } = Sw({
                     size: m,
                     fullWidth: p,
                     color: d,
                     radius: f,
                     shouldAnimate: x || !k,
                     transitionDuration: b,
                     transitionTimingFunction: g,
@@ -16572,15 +16899,15 @@
                 [T, D] = Object(n.useState)({
                     width: 0,
                     height: 0,
                     translate: [0, 0]
                 }),
                 I = Ja(s),
                 R = Object(n.useRef)({}),
-                [_, L] = BO();
+                [_, L] = fw();
             Object(n.useEffect)(() => {
                 if (j in R.current && _.current) {
                     const e = R.current[j],
                         t = e.getBoundingClientRect(),
                         r = e.offsetWidth / t.width,
                         n = t.width * r || 0,
                         a = t.height * r || 0,
@@ -16616,17 +16943,17 @@
                 }),
                 htmlFor: `${I}-${e.value}`,
                 ref: t => {
                     R.current[e.value] = t
                 }
             }, e.label)));
             return a.a.createElement(Cn, ((e, t) => {
-                for (var r in t || (t = {})) ew.call(t, r) && rw(e, r, t[r]);
-                if (QO)
-                    for (var r of QO(t)) tw.call(t, r) && rw(e, r, t[r]);
+                for (var r in t || (t = {})) jw.call(t, r) && zw(e, r, t[r]);
+                if (Ew)
+                    for (var r of Ew(t)) Pw.call(t, r) && zw(e, r, t[r]);
                 return e
             })({
                 className: C(z.root, o),
                 ref: ua(_, t)
             }, w), !!j && a.a.createElement(Cn, {
                 component: "span",
                 className: z.active,
@@ -16634,41 +16961,41 @@
                     width: T.width,
                     height: T.height,
                     transform: `translate(${T.translate[0]}px, ${T.translate[1]}px )`
                 }
             }), A)
         });
 
-    function ow() {
-        return (ow = Object.assign || function(e) {
+    function Tw() {
+        return (Tw = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    aw.displayName = "@mantine/core/SegmentedControl";
-    var iw = function(e) {
+    Nw.displayName = "@mantine/core/SegmentedControl";
+    var Dw = function(e) {
         var t = e.setProps,
             r = e.class_name;
-        return a.a.createElement(aw, ow({
+        return a.a.createElement(Nw, Tw({
             onChange: function(e) {
                 t({
                     value: e
                 })
             }
         }, G(["setProps", "class_name"], e), {
             className: r
         }))
     };
-    iw.displayName = "SegmentedControl", iw.defaultProps = {
+    Dw.displayName = "SegmentedControl", Dw.defaultProps = {
         persisted_props: ["value"],
         persistence_type: "local"
-    }, iw.propTypes = {
+    }, Dw.propTypes = {
         class_name: i.a.string,
         color: i.a.oneOf(["dark", "gray", "red", "pink", "grape", "violet", "indigo", "blue", "cyan", "teal", "green", "lime", "yellow", "orange"]),
         data: i.a.oneOfType([i.a.arrayOf(i.a.exact({
             label: i.a.string.isRequired,
             value: i.a.string.isRequired
         })), i.a.arrayOf(i.a.string)]).isRequired,
         disabled: i.a.bool,
@@ -16682,116 +17009,116 @@
         setProps: i.a.func,
         size: i.a.oneOf(["xs", "sm", "md", "lg", "xl"]),
         style: i.a.object,
         transitionDuration: i.a.number,
         transitionTimingFunction: i.a.string,
         value: i.a.string
     };
-    var lw = iw,
-        sw = Object.defineProperty,
-        cw = Object.defineProperties,
-        uw = Object.getOwnPropertyDescriptors,
-        dw = Object.getOwnPropertySymbols,
-        pw = Object.prototype.hasOwnProperty,
-        fw = Object.prototype.propertyIsEnumerable,
-        mw = (e, t, r) => t in e ? sw(e, t, {
+    var Iw = Dw,
+        Rw = Object.defineProperty,
+        _w = Object.defineProperties,
+        Lw = Object.getOwnPropertyDescriptors,
+        Aw = Object.getOwnPropertySymbols,
+        Mw = Object.prototype.hasOwnProperty,
+        Fw = Object.prototype.propertyIsEnumerable,
+        $w = (e, t, r) => t in e ? Rw(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        bw = (e, t) => {
-            for (var r in t || (t = {})) pw.call(t, r) && mw(e, r, t[r]);
-            if (dw)
-                for (var r of dw(t)) fw.call(t, r) && mw(e, r, t[r]);
+        Bw = (e, t) => {
+            for (var r in t || (t = {})) Mw.call(t, r) && $w(e, r, t[r]);
+            if (Aw)
+                for (var r of Aw(t)) Fw.call(t, r) && $w(e, r, t[r]);
             return e
         },
-        gw = (e, t) => cw(e, uw(t));
-    const yw = {
+        Ww = (e, t) => _w(e, Lw(t));
+    const Hw = {
             xs: 16,
             sm: 20,
             md: 24,
             lg: 30,
             xl: 36
         },
-        hw = {
+        Vw = {
             xs: 30,
             sm: 38,
             md: 46,
             lg: 56,
             xl: 68
         },
-        vw = {
+        qw = {
             xs: 12,
             sm: 14,
             md: 18,
             lg: 22,
             xl: 28
         },
-        Ow = {
+        Uw = {
             xs: 5,
             sm: 6,
             md: 7,
             lg: 9,
             xl: 11
         };
-    Object.keys(yw).reduce((e, t) => (e[t] = {
-        width: hw[t],
-        height: yw[t]
+    Object.keys(Hw).reduce((e, t) => (e[t] = {
+        width: Vw[t],
+        height: Hw[t]
     }, e), {});
-    var ww = Er((e, {
+    var Gw = Er((e, {
             size: t,
             radius: r,
             color: n,
             offLabel: a,
             onLabel: o
         }) => {
             const i = e.fn.size({
                     size: t,
-                    sizes: vw
+                    sizes: qw
                 }),
                 l = e.fn.size({
                     size: r,
                     sizes: e.radius
                 });
             return {
                 root: {
                     display: "flex",
                     alignItems: "center"
                 },
-                input: gw(bw({}, e.fn.focusStyles()), {
+                input: Ww(Bw({}, e.fn.focusStyles()), {
                     overflow: "hidden",
                     WebkitTapHighlightColor: "transparent",
                     position: "relative",
                     borderRadius: l,
                     backgroundColor: "dark" === e.colorScheme ? e.colors.dark[4] : e.colors.gray[2],
                     border: "1px solid " + ("dark" === e.colorScheme ? e.colors.dark[4] : e.colors.gray[3]),
                     height: e.fn.size({
                         size: t,
-                        sizes: yw
+                        sizes: Hw
                     }),
                     width: e.fn.size({
                         size: t,
-                        sizes: hw
+                        sizes: Vw
                     }),
                     minWidth: e.fn.size({
                         size: t,
-                        sizes: hw
+                        sizes: Vw
                     }),
                     margin: 0,
                     transitionProperty: "background-color, border-color",
                     transitionTimingFunction: e.transitionTimingFunction,
                     transitionDuration: "150ms",
                     boxSizing: "border-box",
                     appearance: "none",
                     display: "flex",
                     alignItems: "center",
                     fontSize: e.fn.size({
                         size: t,
-                        sizes: Ow
+                        sizes: Uw
                     }),
                     fontWeight: 600,
                     "&::before": {
                         zIndex: 1,
                         borderRadius: l,
                         boxSizing: "border-box",
                         content: "''",
@@ -16819,15 +17146,15 @@
                         color: "dark" === e.colorScheme ? e.colors.dark[1] : e.colors.gray[6],
                         transition: "color 150ms " + e.transitionTimingFunction
                     },
                     "&:checked": {
                         backgroundColor: e.fn.themeColor(n, 6),
                         borderColor: e.fn.themeColor(n, 6),
                         "&::before": {
-                            transform: `translateX(${e.fn.size({size:t,sizes:hw})-e.fn.size({size:t,sizes:vw})-("xs"===t?3:4)}px)`,
+                            transform: `translateX(${e.fn.size({size:t,sizes:Vw})-e.fn.size({size:t,sizes:qw})-("xs"===t?3:4)}px)`,
                             borderColor: e.white
                         },
                         "&::after": {
                             transform: "translateX(-200%)",
                             content: o ? `'${o}'` : "''",
                             color: e.white
                         }
@@ -16838,52 +17165,52 @@
                         cursor: "not-allowed",
                         "&::before": {
                             borderColor: "dark" === e.colorScheme ? e.colors.dark[4] : e.colors.gray[2],
                             backgroundColor: "dark" === e.colorScheme ? e.colors.dark[3] : e.colors.gray[0]
                         }
                     }
                 }),
-                label: gw(bw({}, e.fn.fontStyles()), {
+                label: Ww(Bw({}, e.fn.fontStyles()), {
                     WebkitTapHighlightColor: "transparent",
                     fontSize: e.fn.size({
                         size: t,
                         sizes: e.fontSizes
                     }),
                     fontFamily: e.fontFamily,
                     paddingLeft: e.spacing.sm,
                     color: "dark" === e.colorScheme ? e.colors.dark[0] : e.black
                 })
             }
         }),
-        xw = Object.defineProperty,
-        Sw = Object.defineProperties,
-        kw = Object.getOwnPropertyDescriptors,
-        Ew = Object.getOwnPropertySymbols,
-        jw = Object.prototype.hasOwnProperty,
-        Pw = Object.prototype.propertyIsEnumerable,
-        zw = (e, t, r) => t in e ? xw(e, t, {
+        Yw = Object.defineProperty,
+        Zw = Object.defineProperties,
+        Kw = Object.getOwnPropertyDescriptors,
+        Xw = Object.getOwnPropertySymbols,
+        Jw = Object.prototype.hasOwnProperty,
+        Qw = Object.prototype.propertyIsEnumerable,
+        ex = (e, t, r) => t in e ? Yw(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        Cw = (e, t) => {
-            for (var r in t || (t = {})) jw.call(t, r) && zw(e, r, t[r]);
-            if (Ew)
-                for (var r of Ew(t)) Pw.call(t, r) && zw(e, r, t[r]);
+        tx = (e, t) => {
+            for (var r in t || (t = {})) Jw.call(t, r) && ex(e, r, t[r]);
+            if (Xw)
+                for (var r of Xw(t)) Qw.call(t, r) && ex(e, r, t[r]);
             return e
         };
-    const Nw = {
+    const rx = {
             offLabel: "",
             onLabel: "",
             size: "sm",
             radius: "xl"
         },
-        Tw = Object(n.forwardRef)((e, t) => {
-            const r = ir("Switch", Nw, e),
+        nx = Object(n.forwardRef)((e, t) => {
+            const r = ir("Switch", rx, e),
                 {
                     className: n,
                     color: o,
                     label: i,
                     offLabel: l,
                     onLabel: s,
                     id: c,
@@ -16894,23 +17221,23 @@
                     children: m,
                     classNames: b,
                     styles: g,
                     sx: y
                 } = r,
                 h = ((e, t) => {
                     var r = {};
-                    for (var n in e) jw.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && Ew)
-                        for (var n of Ew(e)) t.indexOf(n) < 0 && Pw.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) Jw.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && Xw)
+                        for (var n of Xw(e)) t.indexOf(n) < 0 && Qw.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["className", "color", "label", "offLabel", "onLabel", "id", "style", "size", "radius", "wrapperProps", "children", "classNames", "styles", "sx"]),
                 {
                     classes: v,
                     cx: O
-                } = ww({
+                } = Gw({
                     size: d,
                     color: o,
                     radius: p,
                     offLabel: l,
                     onLabel: s
                 }, {
                     classNames: b,
@@ -16918,61 +17245,61 @@
                     name: "Switch"
                 }),
                 {
                     systemStyles: w,
                     rest: x
                 } = gn(h),
                 S = Ja(c);
-            return a.a.createElement(Cn, Cw(Cw({
+            return a.a.createElement(Cn, tx(tx({
                 className: O(v.root, n),
                 style: u,
                 sx: y
-            }, w), f), a.a.createElement("input", (k = Cw({}, x), E = {
+            }, w), f), a.a.createElement("input", (k = tx({}, x), E = {
                 id: S,
                 ref: t,
                 type: "checkbox",
                 className: v.input
-            }, Sw(k, kw(E)))), i && a.a.createElement("label", {
+            }, Zw(k, Kw(E)))), i && a.a.createElement("label", {
                 className: v.label,
                 htmlFor: S
             }, i));
             var k, E
         });
 
-    function Dw() {
-        return (Dw = Object.assign || function(e) {
+    function ax() {
+        return (ax = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    Tw.displayName = "@mantine/core/Switch";
-    var Iw = function(e) {
+    nx.displayName = "@mantine/core/Switch";
+    var ox = function(e) {
         var t = e.setProps,
             r = e.class_name,
             n = e.label;
-        return a.a.createElement(Tw, Dw({
+        return a.a.createElement(nx, ax({
             onChange: function(e) {
                 return r = e.currentTarget.checked, void t({
                     checked: r
                 });
                 var r
             }
         }, G(["setProps", "class_name", "label"], e), {
             className: r,
             label: ea(n)
         }))
     };
-    Iw.displayName = "Switch", Iw.defaultProps = {
+    ox.displayName = "Switch", ox.defaultProps = {
         checked: !1,
         persisted_props: ["checked"],
         persistence_type: "local"
-    }, Iw.propTypes = {
+    }, ox.propTypes = {
         class_name: i.a.string,
         color: i.a.oneOf(["dark", "gray", "red", "pink", "grape", "violet", "indigo", "blue", "cyan", "teal", "green", "lime", "yellow", "orange"]),
         disabled: i.a.bool,
         id: i.a.string,
         label: i.a.any,
         offLabel: i.a.string,
         onLabel: i.a.string,
@@ -16981,72 +17308,72 @@
         persistence_type: i.a.oneOf(["local", "session", "memory"]),
         radius: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         setProps: i.a.func,
         size: i.a.oneOf(["xs", "sm", "md", "lg", "xl"]),
         style: i.a.object,
         checked: i.a.bool
     };
-    var Rw = Iw,
-        _w = Object.defineProperty,
-        Lw = Object.defineProperties,
-        Aw = Object.getOwnPropertyDescriptors,
-        Mw = Object.getOwnPropertySymbols,
-        Fw = Object.prototype.hasOwnProperty,
-        $w = Object.prototype.propertyIsEnumerable,
-        Bw = (e, t, r) => t in e ? _w(e, t, {
+    var ix = ox,
+        lx = Object.defineProperty,
+        sx = Object.defineProperties,
+        cx = Object.getOwnPropertyDescriptors,
+        ux = Object.getOwnPropertySymbols,
+        dx = Object.prototype.hasOwnProperty,
+        px = Object.prototype.propertyIsEnumerable,
+        fx = (e, t, r) => t in e ? lx(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        Ww = (e, t) => {
-            for (var r in t || (t = {})) Fw.call(t, r) && Bw(e, r, t[r]);
-            if (Mw)
-                for (var r of Mw(t)) $w.call(t, r) && Bw(e, r, t[r]);
+        mx = (e, t) => {
+            for (var r in t || (t = {})) dx.call(t, r) && fx(e, r, t[r]);
+            if (ux)
+                for (var r of ux(t)) px.call(t, r) && fx(e, r, t[r]);
             return e
         },
-        Hw = Er((e, {
+        bx = Er((e, {
             color: t,
             radius: r
         }) => {
             return {
                 root: {
                     position: "relative",
                     display: "inline-block"
                 },
-                body: (n = Ww({}, e.fn.fontStyles()), a = {
+                body: (n = mx({}, e.fn.fontStyles()), a = {
                     backgroundColor: e.fn.themeColor(t, "dark" === e.colorScheme ? 3 : 9),
                     lineHeight: e.lineHeight,
                     fontSize: e.fontSizes.sm,
                     borderRadius: e.fn.radius(r),
                     padding: `${e.spacing.xs/2}px ${e.spacing.xs}px`,
                     color: "dark" === e.colorScheme ? e.colors.dark[9] : e.white,
                     position: "relative",
                     overflow: "hidden",
                     textOverflow: "ellipsis"
-                }, Lw(n, Aw(a))),
+                }, sx(n, cx(a))),
                 arrow: {
                     border: 0,
                     background: e.fn.themeColor(t, "dark" === e.colorScheme ? 3 : 9),
                     zIndex: 1
                 }
             };
             var n, a
         }),
-        Vw = Object.defineProperty,
-        qw = Object.getOwnPropertySymbols,
-        Uw = Object.prototype.hasOwnProperty,
-        Gw = Object.prototype.propertyIsEnumerable,
-        Yw = (e, t, r) => t in e ? Vw(e, t, {
+        gx = Object.defineProperty,
+        yx = Object.getOwnPropertySymbols,
+        hx = Object.prototype.hasOwnProperty,
+        vx = Object.prototype.propertyIsEnumerable,
+        Ox = (e, t, r) => t in e ? gx(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const Zw = {
+    const wx = {
             openDelay: 0,
             closeDelay: 0,
             gutter: 5,
             color: "gray",
             disabled: !1,
             withArrow: !1,
             arrowSize: 2,
@@ -17057,16 +17384,16 @@
             zIndex: ac("popover"),
             width: "auto",
             wrapLines: !1,
             allowPointerEvents: !1,
             positionDependencies: [],
             withinPortal: !0
         },
-        Kw = Object(n.forwardRef)((e, t) => {
-            const r = ir("Tooltip", Zw, e),
+        xx = Object(n.forwardRef)((e, t) => {
+            const r = ir("Tooltip", wx, e),
                 {
                     className: o,
                     label: i,
                     children: l,
                     opened: s,
                     openDelay: c,
                     closeDelay: u,
@@ -17092,24 +17419,24 @@
                     classNames: N,
                     styles: T,
                     onMouseLeave: D,
                     onMouseEnter: I
                 } = r,
                 R = ((e, t) => {
                     var r = {};
-                    for (var n in e) Uw.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && qw)
-                        for (var n of qw(e)) t.indexOf(n) < 0 && Gw.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) hx.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && yx)
+                        for (var n of yx(e)) t.indexOf(n) < 0 && vx.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["className", "label", "children", "opened", "openDelay", "closeDelay", "gutter", "color", "radius", "disabled", "withArrow", "arrowSize", "position", "placement", "transition", "transitionDuration", "zIndex", "transitionTimingFunction", "width", "wrapLines", "allowPointerEvents", "positionDependencies", "withinPortal", "tooltipRef", "tooltipId", "classNames", "styles", "onMouseLeave", "onMouseEnter"]),
                 {
                     classes: _,
                     cx: L,
                     theme: A
-                } = Hw({
+                } = bx({
                     color: p,
                     radius: f
                 }, {
                     classNames: N,
                     styles: T,
                     name: "Tooltip"
                 }),
@@ -17128,17 +17455,17 @@
                     window.clearTimeout(M.current), 0 !== u ? F.current = window.setTimeout(() => {
                         B(!1)
                     }, u) : B(!1)
                 };
             return Object(n.useEffect)(() => () => {
                 window.clearTimeout(M.current), window.clearTimeout(F.current)
             }, []), a.a.createElement(Cn, ((e, t) => {
-                for (var r in t || (t = {})) Uw.call(t, r) && Yw(e, r, t[r]);
-                if (qw)
-                    for (var r of qw(t)) Gw.call(t, r) && Yw(e, r, t[r]);
+                for (var r in t || (t = {})) hx.call(t, r) && Ox(e, r, t[r]);
+                if (yx)
+                    for (var r of yx(t)) vx.call(t, r) && Ox(e, r, t[r]);
                 return e
             })({
                 className: L(_.root, o),
                 onMouseEnter: e => {
                     U(), "function" == typeof I && I(e)
                 },
                 onMouseLeave: e => {
@@ -17169,33 +17496,33 @@
                     pointerEvents: E ? "all" : "none",
                     whiteSpace: k ? "normal" : "nowrap",
                     width: S
                 }
             }, i)), l)
         });
 
-    function Xw() {
-        return (Xw = Object.assign || function(e) {
+    function Sx() {
+        return (Sx = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    Kw.displayName = "@mantine/core/Tooltip";
-    var Jw = function(e) {
+    xx.displayName = "@mantine/core/Tooltip";
+    var kx = function(e) {
         var t = e.class_name,
             r = e.label;
-        return a.a.createElement(Kw, Xw({}, G(["setProps", "class_name", "label"], e), {
+        return a.a.createElement(xx, Sx({}, G(["setProps", "class_name", "label"], e), {
             className: t,
             label: ea(r)
         }), e.children)
     };
-    Jw.displayName = "Tooltip", Jw.defaultProps = {}, Jw.propTypes = {
+    kx.displayName = "Tooltip", kx.defaultProps = {}, kx.propTypes = {
         arrowDistance: i.a.number,
         arrowSize: i.a.number,
         children: i.a.node,
         class_name: i.a.string,
         closeDelay: i.a.number,
         color: i.a.oneOf(["dark", "gray", "red", "pink", "grape", "violet", "indigo", "blue", "cyan", "teal", "green", "lime", "yellow", "orange"]),
         disabled: i.a.bool,
@@ -17213,27 +17540,27 @@
         transitionDuration: i.a.number,
         transitionTimingFunction: i.a.string,
         width: i.a.oneOfType([i.a.number, i.a.oneOf(["auto"])]),
         withArrow: i.a.bool,
         wrapLines: i.a.bool,
         zIndex: i.a.number
     };
-    var Qw = Jw;
+    var Ex = kx;
 
-    function ex() {
-        return (ex = Object.assign || function(e) {
+    function jx() {
+        return (jx = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
 
-    function tx(e, t) {
+    function Px(e, t) {
         return function(e) {
             if (Array.isArray(e)) return e
         }(e) || function(e, t) {
             var r = null == e ? null : "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
             if (null == r) return;
             var n, a, o = [],
                 i = !0,
@@ -17248,55 +17575,55 @@
                 } finally {
                     if (l) throw a
                 }
             }
             return o
         }(e, t) || function(e, t) {
             if (!e) return;
-            if ("string" == typeof e) return rx(e, t);
+            if ("string" == typeof e) return zx(e, t);
             var r = Object.prototype.toString.call(e).slice(8, -1);
             "Object" === r && e.constructor && (r = e.constructor.name);
             if ("Map" === r || "Set" === r) return Array.from(e);
-            if ("Arguments" === r || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(r)) return rx(e, t)
+            if ("Arguments" === r || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(r)) return zx(e, t)
         }(e, t) || function() {
             throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()
     }
 
-    function rx(e, t) {
+    function zx(e, t) {
         (null == t || t > e.length) && (t = e.length);
         for (var r = 0, n = new Array(t); r < t; r++) n[r] = e[r];
         return n
     }
-    var nx = function(e) {
+    var Cx = function(e) {
         var t = e.opened,
             r = e.children,
             o = e.setProps,
             i = e.class_name,
             l = e.title,
-            s = tx(Object(n.useState)(t), 2),
+            s = Px(Object(n.useState)(t), 2),
             c = s[0],
             u = s[1];
         Object(n.useEffect)((function() {
             u(t)
         }), [t]);
-        return a.a.createElement(xp, ex({}, G(["opened", "setProps", "children", "title"], e), {
+        return a.a.createElement(xp, jx({}, G(["opened", "setProps", "children", "title"], e), {
             className: i,
             opened: c,
             onClose: function() {
                 u(!1), o({
                     opened: !1
                 })
             },
             title: ea(l)
         }), r)
     };
-    nx.displayName = "Modal", nx.defaultProps = {
+    Cx.displayName = "Modal", Cx.defaultProps = {
         opened: !1
-    }, nx.propTypes = {
+    }, Cx.propTypes = {
         centered: i.a.bool,
         children: i.a.node,
         class_name: i.a.string,
         closeOnClickOutside: i.a.bool,
         closeOnEscape: i.a.bool,
         id: i.a.string,
         opened: i.a.bool,
@@ -17313,16 +17640,16 @@
         transition: i.a.oneOf(["fade", "skew-up", "skew-down", "rotate-right", "rotate-left", "slide-down", "slide-up", "slide-right", "slide-left", "scale-y", "scale-x", "scale", "pop", "pop-top-left", "pop-top-right", "pop-bottom-left", "pop-bottom-right"]),
         transitionDuration: i.a.number,
         transitionTimingFunction: i.a.string,
         trapFocus: i.a.bool,
         withCloseButton: i.a.bool,
         zIndex: i.a.number
     };
-    var ax, ox, ix, lx = nx,
-        sx = function() {
+    var Nx, Tx, Dx, Ix = Cx,
+        Rx = function() {
             var e = /(?:^|\s)lang(?:uage)?-([\w-]+)(?=\s|$)/i,
                 t = 0,
                 r = {},
                 n = {
                     util: {
                         encode: function e(t) {
                             return t instanceof a ? new a(t.type, e(t.content), t.alias) : Array.isArray(t) ? t.map(e) : t.replace(/&/g, "&amp;").replace(/</g, "&lt;").replace(/\u00a0/g, " ")
@@ -17558,16 +17885,16 @@
                     i = t.alias;
                 i && (Array.isArray(i) ? Array.prototype.push.apply(o.classes, i) : o.classes.push(i)), n.hooks.run("wrap", o);
                 var l = "";
                 for (var s in o.attributes) l += " " + s + '="' + (o.attributes[s] || "").replace(/"/g, "&quot;") + '"';
                 return "<" + o.tag + ' class="' + o.classes.join(" ") + '"' + l + ">" + o.content + "</" + o.tag + ">"
             }, n
         }(),
-        cx = sx;
-    sx.default = sx, cx.languages.markup = {
+        _x = Rx;
+    Rx.default = Rx, _x.languages.markup = {
             comment: {
                 pattern: /<!--(?:(?!<!--)[\s\S])*?-->/,
                 greedy: !0
             },
             prolog: {
                 pattern: /<\?[\s\S]+?\?>/,
                 greedy: !0
@@ -17625,70 +17952,70 @@
                     }
                 }
             },
             entity: [{
                 pattern: /&[\da-z]{1,8};/i,
                 alias: "named-entity"
             }, /&#x?[\da-f]{1,8};/i]
-        }, cx.languages.markup.tag.inside["attr-value"].inside.entity = cx.languages.markup.entity, cx.languages.markup.doctype.inside["internal-subset"].inside = cx.languages.markup, cx.hooks.add("wrap", (function(e) {
+        }, _x.languages.markup.tag.inside["attr-value"].inside.entity = _x.languages.markup.entity, _x.languages.markup.doctype.inside["internal-subset"].inside = _x.languages.markup, _x.hooks.add("wrap", (function(e) {
             "entity" === e.type && (e.attributes.title = e.content.replace(/&amp;/, "&"))
-        })), Object.defineProperty(cx.languages.markup.tag, "addInlined", {
+        })), Object.defineProperty(_x.languages.markup.tag, "addInlined", {
             value: function(e, t) {
                 var r = {};
                 r["language-" + t] = {
                     pattern: /(^<!\[CDATA\[)[\s\S]+?(?=\]\]>$)/i,
                     lookbehind: !0,
-                    inside: cx.languages[t]
+                    inside: _x.languages[t]
                 }, r.cdata = /^<!\[CDATA\[|\]\]>$/i;
                 var n = {
                     "included-cdata": {
                         pattern: /<!\[CDATA\[[\s\S]*?\]\]>/i,
                         inside: r
                     }
                 };
                 n["language-" + t] = {
                     pattern: /[\s\S]+/,
-                    inside: cx.languages[t]
+                    inside: _x.languages[t]
                 };
                 var a = {};
                 a[e] = {
                     pattern: RegExp(/(<__[^>]*>)(?:<!\[CDATA\[(?:[^\]]|\](?!\]>))*\]\]>|(?!<!\[CDATA\[)[\s\S])*?(?=<\/__>)/.source.replace(/__/g, (function() {
                         return e
                     })), "i"),
                     lookbehind: !0,
                     greedy: !0,
                     inside: n
-                }, cx.languages.insertBefore("markup", "cdata", a)
+                }, _x.languages.insertBefore("markup", "cdata", a)
             }
-        }), Object.defineProperty(cx.languages.markup.tag, "addAttribute", {
+        }), Object.defineProperty(_x.languages.markup.tag, "addAttribute", {
             value: function(e, t) {
-                cx.languages.markup.tag.inside["special-attr"].push({
+                _x.languages.markup.tag.inside["special-attr"].push({
                     pattern: RegExp(/(^|["'\s])/.source + "(?:" + e + ")" + /\s*=\s*(?:"[^"]*"|'[^']*'|[^\s'">=]+(?=[\s>]))/.source, "i"),
                     lookbehind: !0,
                     inside: {
                         "attr-name": /^[^\s=]+/,
                         "attr-value": {
                             pattern: /=[\s\S]+/,
                             inside: {
                                 value: {
                                     pattern: /(^=\s*(["']|(?!["'])))\S[\s\S]*(?=\2$)/,
                                     lookbehind: !0,
                                     alias: [t, "language-" + t],
-                                    inside: cx.languages[t]
+                                    inside: _x.languages[t]
                                 },
                                 punctuation: [{
                                     pattern: /^=/,
                                     alias: "attr-equals"
                                 }, /"|'/]
                             }
                         }
                     }
                 })
             }
-        }), cx.languages.html = cx.languages.markup, cx.languages.mathml = cx.languages.markup, cx.languages.svg = cx.languages.markup, cx.languages.xml = cx.languages.extend("markup", {}), cx.languages.ssml = cx.languages.xml, cx.languages.atom = cx.languages.xml, cx.languages.rss = cx.languages.xml,
+        }), _x.languages.html = _x.languages.markup, _x.languages.mathml = _x.languages.markup, _x.languages.svg = _x.languages.markup, _x.languages.xml = _x.languages.extend("markup", {}), _x.languages.ssml = _x.languages.xml, _x.languages.atom = _x.languages.xml, _x.languages.rss = _x.languages.xml,
         function(e) {
             var t = "\\b(?:BASH|BASHOPTS|BASH_ALIASES|BASH_ARGC|BASH_ARGV|BASH_CMDS|BASH_COMPLETION_COMPAT_DIR|BASH_LINENO|BASH_REMATCH|BASH_SOURCE|BASH_VERSINFO|BASH_VERSION|COLORTERM|COLUMNS|COMP_WORDBREAKS|DBUS_SESSION_BUS_ADDRESS|DEFAULTS_PATH|DESKTOP_SESSION|DIRSTACK|DISPLAY|EUID|GDMSESSION|GDM_LANG|GNOME_KEYRING_CONTROL|GNOME_KEYRING_PID|GPG_AGENT_INFO|GROUPS|HISTCONTROL|HISTFILE|HISTFILESIZE|HISTSIZE|HOME|HOSTNAME|HOSTTYPE|IFS|INSTANCE|JOB|LANG|LANGUAGE|LC_ADDRESS|LC_ALL|LC_IDENTIFICATION|LC_MEASUREMENT|LC_MONETARY|LC_NAME|LC_NUMERIC|LC_PAPER|LC_TELEPHONE|LC_TIME|LESSCLOSE|LESSOPEN|LINES|LOGNAME|LS_COLORS|MACHTYPE|MAILCHECK|MANDATORY_PATH|NO_AT_BRIDGE|OLDPWD|OPTERR|OPTIND|ORBIT_SOCKETDIR|OSTYPE|PAPERSIZE|PATH|PIPESTATUS|PPID|PS1|PS2|PS3|PS4|PWD|RANDOM|REPLY|SECONDS|SELINUX_INIT|SESSION|SESSIONTYPE|SESSION_MANAGER|SHELL|SHELLOPTS|SHLVL|SSH_AUTH_SOCK|TERM|UID|UPSTART_EVENTS|UPSTART_INSTANCE|UPSTART_JOB|UPSTART_SESSION|USER|WINDOWID|XAUTHORITY|XDG_CONFIG_DIRS|XDG_CURRENT_DESKTOP|XDG_DATA_DIRS|XDG_GREETER_DATA_DIR|XDG_MENU_PREFIX|XDG_RUNTIME_DIR|XDG_SEAT|XDG_SEAT_PATH|XDG_SESSION_DESKTOP|XDG_SESSION_ID|XDG_SESSION_PATH|XDG_SESSION_TYPE|XDG_VTNR|XMODIFIERS)\\b",
                 r = {
                     pattern: /(^(["']?)\w+\2)[ \t]+\S.*/,
                     lookbehind: !0,
                     alias: "punctuation",
                     inside: null
@@ -17833,15 +18160,15 @@
                 number: {
                     pattern: /(^|\s)(?:[1-9]\d*|0)(?:[.,]\d+)?\b/,
                     lookbehind: !0
                 }
             }, r.inside = e.languages.bash;
             for (var a = ["comment", "function-name", "for-or-select", "assign-left", "string", "environment", "function", "keyword", "builtin", "boolean", "file-descriptor", "operator", "punctuation", "number"], o = n.variable[1].inside, i = 0; i < a.length; i++) o[a[i]] = e.languages.bash[a[i]];
             e.languages.shell = e.languages.bash
-        }(cx), cx.languages.clike = {
+        }(_x), _x.languages.clike = {
             comment: [{
                 pattern: /(^|[^\\])\/\*[\s\S]*?(?:\*\/|$)/,
                 lookbehind: !0,
                 greedy: !0
             }, {
                 pattern: /(^|[^\\:])\/\/.*/,
                 lookbehind: !0,
@@ -17860,15 +18187,15 @@
             },
             keyword: /\b(?:break|catch|continue|do|else|finally|for|function|if|in|instanceof|new|null|return|throw|try|while)\b/,
             boolean: /\b(?:false|true)\b/,
             function: /\b\w+(?=\()/,
             number: /\b0x[\da-f]+\b|(?:\b\d+(?:\.\d*)?|\B\.\d+)(?:e[+-]?\d+)?/i,
             operator: /[<>]=?|[!=]=?=?|--?|\+\+?|&&?|\|\|?|[?*/~^%]/,
             punctuation: /[{}[\];(),.:]/
-        }, cx.languages.c = cx.languages.extend("clike", {
+        }, _x.languages.c = _x.languages.extend("clike", {
             comment: {
                 pattern: /\/\/(?:[^\r\n\\]|\\(?:\r\n?|\n|(?![\r\n])))*|\/\*[\s\S]*?(?:\*\/|$)/,
                 greedy: !0
             },
             string: {
                 pattern: /"(?:\\(?:\r\n|[\s\S])|[^"\\\r\n])*"/,
                 greedy: !0
@@ -17877,32 +18204,32 @@
                 pattern: /(\b(?:enum|struct)\s+(?:__attribute__\s*\(\([\s\S]*?\)\)\s*)?)\w+|\b[a-z]\w*_t\b/,
                 lookbehind: !0
             },
             keyword: /\b(?:_Alignas|_Alignof|_Atomic|_Bool|_Complex|_Generic|_Imaginary|_Noreturn|_Static_assert|_Thread_local|__attribute__|asm|auto|break|case|char|const|continue|default|do|double|else|enum|extern|float|for|goto|if|inline|int|long|register|return|short|signed|sizeof|static|struct|switch|typedef|typeof|union|unsigned|void|volatile|while)\b/,
             function: /\b[a-z_]\w*(?=\s*\()/i,
             number: /(?:\b0x(?:[\da-f]+(?:\.[\da-f]*)?|\.[\da-f]+)(?:p[+-]?\d+)?|(?:\b\d+(?:\.\d*)?|\B\.\d+)(?:e[+-]?\d+)?)[ful]{0,4}/i,
             operator: />>=?|<<=?|->|([-+&|:])\1|[?:~]|[-+*/%&|^!=<>]=?/
-        }), cx.languages.insertBefore("c", "string", {
+        }), _x.languages.insertBefore("c", "string", {
             char: {
                 pattern: /'(?:\\(?:\r\n|[\s\S])|[^'\\\r\n]){0,32}'/,
                 greedy: !0
             }
-        }), cx.languages.insertBefore("c", "string", {
+        }), _x.languages.insertBefore("c", "string", {
             macro: {
                 pattern: /(^[\t ]*)#\s*[a-z](?:[^\r\n\\/]|\/(?!\*)|\/\*(?:[^*]|\*(?!\/))*\*\/|\\(?:\r\n|[\s\S]))*/im,
                 lookbehind: !0,
                 greedy: !0,
                 alias: "property",
                 inside: {
                     string: [{
                         pattern: /^(#\s*include\s*)<[^>]+>/,
                         lookbehind: !0
-                    }, cx.languages.c.string],
-                    char: cx.languages.c.char,
-                    comment: cx.languages.c.comment,
+                    }, _x.languages.c.string],
+                    char: _x.languages.c.char,
+                    comment: _x.languages.c.comment,
                     "macro-name": [{
                         pattern: /(^#\s*define\s+)\w+\b(?!\()/i,
                         lookbehind: !0
                     }, {
                         pattern: /(^#\s*define\s+)\w+\b(?=\()/i,
                         lookbehind: !0,
                         alias: "function"
@@ -17912,81 +18239,81 @@
                         lookbehind: !0,
                         alias: "keyword"
                     },
                     "directive-hash": /^#/,
                     punctuation: /##|\\(?=[\r\n])/,
                     expression: {
                         pattern: /\S[\s\S]*/,
-                        inside: cx.languages.c
+                        inside: _x.languages.c
                     }
                 }
             }
-        }), cx.languages.insertBefore("c", "function", {
+        }), _x.languages.insertBefore("c", "function", {
             constant: /\b(?:EOF|NULL|SEEK_CUR|SEEK_END|SEEK_SET|__DATE__|__FILE__|__LINE__|__TIMESTAMP__|__TIME__|__func__|stderr|stdin|stdout)\b/
-        }), delete cx.languages.c.boolean, ax = cx, ox = /\b(?:alignas|alignof|asm|auto|bool|break|case|catch|char|char16_t|char32_t|char8_t|class|co_await|co_return|co_yield|compl|concept|const|const_cast|consteval|constexpr|constinit|continue|decltype|default|delete|do|double|dynamic_cast|else|enum|explicit|export|extern|final|float|for|friend|goto|if|import|inline|int|int16_t|int32_t|int64_t|int8_t|long|module|mutable|namespace|new|noexcept|nullptr|operator|override|private|protected|public|register|reinterpret_cast|requires|return|short|signed|sizeof|static|static_assert|static_cast|struct|switch|template|this|thread_local|throw|try|typedef|typeid|typename|uint16_t|uint32_t|uint64_t|uint8_t|union|unsigned|using|virtual|void|volatile|wchar_t|while)\b/, ix = /\b(?!<keyword>)\w+(?:\s*\.\s*\w+)*\b/.source.replace(/<keyword>/g, (function() {
-            return ox.source
-        })), ax.languages.cpp = ax.languages.extend("c", {
+        }), delete _x.languages.c.boolean, Nx = _x, Tx = /\b(?:alignas|alignof|asm|auto|bool|break|case|catch|char|char16_t|char32_t|char8_t|class|co_await|co_return|co_yield|compl|concept|const|const_cast|consteval|constexpr|constinit|continue|decltype|default|delete|do|double|dynamic_cast|else|enum|explicit|export|extern|final|float|for|friend|goto|if|import|inline|int|int16_t|int32_t|int64_t|int8_t|long|module|mutable|namespace|new|noexcept|nullptr|operator|override|private|protected|public|register|reinterpret_cast|requires|return|short|signed|sizeof|static|static_assert|static_cast|struct|switch|template|this|thread_local|throw|try|typedef|typeid|typename|uint16_t|uint32_t|uint64_t|uint8_t|union|unsigned|using|virtual|void|volatile|wchar_t|while)\b/, Dx = /\b(?!<keyword>)\w+(?:\s*\.\s*\w+)*\b/.source.replace(/<keyword>/g, (function() {
+            return Tx.source
+        })), Nx.languages.cpp = Nx.languages.extend("c", {
             "class-name": [{
                 pattern: RegExp(/(\b(?:class|concept|enum|struct|typename)\s+)(?!<keyword>)\w+/.source.replace(/<keyword>/g, (function() {
-                    return ox.source
+                    return Tx.source
                 }))),
                 lookbehind: !0
             }, /\b[A-Z]\w*(?=\s*::\s*\w+\s*\()/, /\b[A-Z_]\w*(?=\s*::\s*~\w+\s*\()/i, /\b\w+(?=\s*<(?:[^<>]|<(?:[^<>]|<[^<>]*>)*>)*>\s*::\s*\w+\s*\()/],
-            keyword: ox,
+            keyword: Tx,
             number: {
                 pattern: /(?:\b0b[01']+|\b0x(?:[\da-f']+(?:\.[\da-f']*)?|\.[\da-f']+)(?:p[+-]?[\d']+)?|(?:\b[\d']+(?:\.[\d']*)?|\B\.[\d']+)(?:e[+-]?[\d']+)?)[ful]{0,4}/i,
                 greedy: !0
             },
             operator: />>=?|<<=?|->|--|\+\+|&&|\|\||[?:~]|<=>|[-+*/%&|^!=<>]=?|\b(?:and|and_eq|bitand|bitor|not|not_eq|or|or_eq|xor|xor_eq)\b/,
             boolean: /\b(?:false|true)\b/
-        }), ax.languages.insertBefore("cpp", "string", {
+        }), Nx.languages.insertBefore("cpp", "string", {
             module: {
                 pattern: RegExp(/(\b(?:import|module)\s+)/.source + "(?:" + /"(?:\\(?:\r\n|[\s\S])|[^"\\\r\n])*"|<[^<>\r\n]*>/.source + "|" + /<mod-name>(?:\s*:\s*<mod-name>)?|:\s*<mod-name>/.source.replace(/<mod-name>/g, (function() {
-                    return ix
+                    return Dx
                 })) + ")"),
                 lookbehind: !0,
                 greedy: !0,
                 inside: {
                     string: /^[<"][\s\S]+/,
                     operator: /:/,
                     punctuation: /\./
                 }
             },
             "raw-string": {
                 pattern: /R"([^()\\ ]{0,16})\([\s\S]*?\)\1"/,
                 alias: "string",
                 greedy: !0
             }
-        }), ax.languages.insertBefore("cpp", "keyword", {
+        }), Nx.languages.insertBefore("cpp", "keyword", {
             "generic-function": {
                 pattern: /\b(?!operator\b)[a-z_]\w*\s*<(?:[^<>]|<[^<>]*>)*>(?=\s*\()/i,
                 inside: {
                     function: /^\w+/,
                     generic: {
                         pattern: /<[\s\S]+/,
                         alias: "class-name",
-                        inside: ax.languages.cpp
+                        inside: Nx.languages.cpp
                     }
                 }
             }
-        }), ax.languages.insertBefore("cpp", "operator", {
+        }), Nx.languages.insertBefore("cpp", "operator", {
             "double-colon": {
                 pattern: /::/,
                 alias: "punctuation"
             }
-        }), ax.languages.insertBefore("cpp", "class-name", {
+        }), Nx.languages.insertBefore("cpp", "class-name", {
             "base-clause": {
                 pattern: /(\b(?:class|struct)\s+\w+\s*:\s*)[^;{}"'\s]+(?:\s+[^;{}"'\s]+)*(?=\s*[;{])/,
                 lookbehind: !0,
                 greedy: !0,
-                inside: ax.languages.extend("cpp", {})
+                inside: Nx.languages.extend("cpp", {})
             }
-        }), ax.languages.insertBefore("inside", "double-colon", {
+        }), Nx.languages.insertBefore("inside", "double-colon", {
             "class-name": /\b[a-z_]\w*\b(?!\s*::)/i
-        }, ax.languages.cpp["base-clause"]),
+        }, Nx.languages.cpp["base-clause"]),
         function(e) {
             var t = /(?:"(?:\\(?:\r\n|[\s\S])|[^"\\\r\n])*"|'(?:\\(?:\r\n|[\s\S])|[^'\\\r\n])*')/;
             e.languages.css = {
                 comment: /\/\*[\s\S]*?\*\//,
                 atrule: {
                     pattern: /@[\w-](?:[^;{\s]|\s+(?![\s{]))*(?:;|(?=\s*\{))/,
                     inside: {
@@ -18031,15 +18358,15 @@
                     pattern: /(^|[^-a-z0-9])[-a-z0-9]+(?=\()/i,
                     lookbehind: !0
                 },
                 punctuation: /[(){};:,]/
             }, e.languages.css.atrule.inside.rest = e.languages.css;
             var r = e.languages.markup;
             r && (r.tag.addInlined("style", "css"), r.tag.addAttribute("style", "css"))
-        }(cx),
+        }(_x),
         function(e) {
             var t, r = /("|')(?:\\(?:\r\n|[\s\S])|(?!\1)[^\\\r\n])*\1/;
             e.languages.css.selector = {
                 pattern: e.languages.css.selector.pattern,
                 lookbehind: !0,
                 inside: t = {
                     "pseudo-element": /:(?:after|before|first-letter|first-line|selection)|::[-\w]+/,
@@ -18123,16 +18450,16 @@
                         punctuation: /[(),]/
                     }
                 }],
                 entity: /\\[\da-f]{1,8}/i,
                 unit: n,
                 number: a
             })
-        }(cx), cx.languages.javascript = cx.languages.extend("clike", {
-            "class-name": [cx.languages.clike["class-name"], {
+        }(_x), _x.languages.javascript = _x.languages.extend("clike", {
+            "class-name": [_x.languages.clike["class-name"], {
                 pattern: /(^|[^$\w\xA0-\uFFFF])(?!\s)[_$A-Z\xA0-\uFFFF](?:(?!\s)[$\w\xA0-\uFFFF])*(?=\.(?:constructor|prototype))/,
                 lookbehind: !0
             }],
             keyword: [{
                 pattern: /((?:^|\})\s*)catch\b/,
                 lookbehind: !0
             }, {
@@ -18141,53 +18468,53 @@
             }],
             function: /#?(?!\s)[_$a-zA-Z\xA0-\uFFFF](?:(?!\s)[$\w\xA0-\uFFFF])*(?=\s*(?:\.\s*(?:apply|bind|call)\s*)?\()/,
             number: {
                 pattern: RegExp(/(^|[^\w$])/.source + "(?:" + /NaN|Infinity/.source + "|" + /0[bB][01]+(?:_[01]+)*n?/.source + "|" + /0[oO][0-7]+(?:_[0-7]+)*n?/.source + "|" + /0[xX][\dA-Fa-f]+(?:_[\dA-Fa-f]+)*n?/.source + "|" + /\d+(?:_\d+)*n/.source + "|" + /(?:\d+(?:_\d+)*(?:\.(?:\d+(?:_\d+)*)?)?|\.\d+(?:_\d+)*)(?:[Ee][+-]?\d+(?:_\d+)*)?/.source + ")" + /(?![\w$])/.source),
                 lookbehind: !0
             },
             operator: /--|\+\+|\*\*=?|=>|&&=?|\|\|=?|[!=]==|<<=?|>>>?=?|[-+*/%&|^!=<>]=?|\.{3}|\?\?=?|\?\.?|[~:]/
-        }), cx.languages.javascript["class-name"][0].pattern = /(\b(?:class|extends|implements|instanceof|interface|new)\s+)[\w.\\]+/, cx.languages.insertBefore("javascript", "keyword", {
+        }), _x.languages.javascript["class-name"][0].pattern = /(\b(?:class|extends|implements|instanceof|interface|new)\s+)[\w.\\]+/, _x.languages.insertBefore("javascript", "keyword", {
             regex: {
                 pattern: /((?:^|[^$\w\xA0-\uFFFF."'\])\s]|\b(?:return|yield))\s*)\/(?:\[(?:[^\]\\\r\n]|\\.)*\]|\\.|[^/\\\[\r\n])+\/[dgimyus]{0,7}(?=(?:\s|\/\*(?:[^*]|\*(?!\/))*\*\/)*(?:$|[\r\n,.;:})\]]|\/\/))/,
                 lookbehind: !0,
                 greedy: !0,
                 inside: {
                     "regex-source": {
                         pattern: /^(\/)[\s\S]+(?=\/[a-z]*$)/,
                         lookbehind: !0,
                         alias: "language-regex",
-                        inside: cx.languages.regex
+                        inside: _x.languages.regex
                     },
                     "regex-delimiter": /^\/|\/$/,
                     "regex-flags": /^[a-z]+$/
                 }
             },
             "function-variable": {
                 pattern: /#?(?!\s)[_$a-zA-Z\xA0-\uFFFF](?:(?!\s)[$\w\xA0-\uFFFF])*(?=\s*[=:]\s*(?:async\s*)?(?:\bfunction\b|(?:\((?:[^()]|\([^()]*\))*\)|(?!\s)[_$a-zA-Z\xA0-\uFFFF](?:(?!\s)[$\w\xA0-\uFFFF])*)\s*=>))/,
                 alias: "function"
             },
             parameter: [{
                 pattern: /(function(?:\s+(?!\s)[_$a-zA-Z\xA0-\uFFFF](?:(?!\s)[$\w\xA0-\uFFFF])*)?\s*\(\s*)(?!\s)(?:[^()\s]|\s+(?![\s)])|\([^()]*\))+(?=\s*\))/,
                 lookbehind: !0,
-                inside: cx.languages.javascript
+                inside: _x.languages.javascript
             }, {
                 pattern: /(^|[^$\w\xA0-\uFFFF])(?!\s)[_$a-z\xA0-\uFFFF](?:(?!\s)[$\w\xA0-\uFFFF])*(?=\s*=>)/i,
                 lookbehind: !0,
-                inside: cx.languages.javascript
+                inside: _x.languages.javascript
             }, {
                 pattern: /(\(\s*)(?!\s)(?:[^()\s]|\s+(?![\s)])|\([^()]*\))+(?=\s*\)\s*=>)/,
                 lookbehind: !0,
-                inside: cx.languages.javascript
+                inside: _x.languages.javascript
             }, {
                 pattern: /((?:\b|\s|^)(?!(?:as|async|await|break|case|catch|class|const|continue|debugger|default|delete|do|else|enum|export|extends|finally|for|from|function|get|if|implements|import|in|instanceof|interface|let|new|null|of|package|private|protected|public|return|set|static|super|switch|this|throw|try|typeof|undefined|var|void|while|with|yield)(?![$\w\xA0-\uFFFF]))(?:(?!\s)[_$a-zA-Z\xA0-\uFFFF](?:(?!\s)[$\w\xA0-\uFFFF])*\s*)\(\s*|\]\s*\(\s*)(?!\s)(?:[^()\s]|\s+(?![\s)])|\([^()]*\))+(?=\s*\)\s*\{)/,
                 lookbehind: !0,
-                inside: cx.languages.javascript
+                inside: _x.languages.javascript
             }],
             constant: /\b[A-Z](?:[A-Z_]|\dx?)*\b/
-        }), cx.languages.insertBefore("javascript", "string", {
+        }), _x.languages.insertBefore("javascript", "string", {
             hashbang: {
                 pattern: /^#!.*/,
                 greedy: !0,
                 alias: "comment"
             },
             "template-string": {
                 pattern: /`(?:\\[\s\S]|\$\{(?:[^{}]|\{(?:[^{}]|\{[^}]*\})*\})+\}|(?!\$\{)[^\\`])*`/,
@@ -18201,33 +18528,33 @@
                         pattern: /((?:^|[^\\])(?:\\{2})*)\$\{(?:[^{}]|\{(?:[^{}]|\{[^}]*\})*\})+\}/,
                         lookbehind: !0,
                         inside: {
                             "interpolation-punctuation": {
                                 pattern: /^\$\{|\}$/,
                                 alias: "punctuation"
                             },
-                            rest: cx.languages.javascript
+                            rest: _x.languages.javascript
                         }
                     },
                     string: /[\s\S]+/
                 }
             },
             "string-property": {
                 pattern: /((?:^|[,{])[ \t]*)(["'])(?:\\(?:\r\n|[\s\S])|(?!\2)[^\\\r\n])*\2(?=\s*:)/m,
                 lookbehind: !0,
                 greedy: !0,
                 alias: "property"
             }
-        }), cx.languages.insertBefore("javascript", "operator", {
+        }), _x.languages.insertBefore("javascript", "operator", {
             "literal-property": {
                 pattern: /((?:^|[,{])[ \t]*)(?!\s)[_$a-zA-Z\xA0-\uFFFF](?:(?!\s)[$\w\xA0-\uFFFF])*(?=\s*:)/m,
                 lookbehind: !0,
                 alias: "property"
             }
-        }), cx.languages.markup && (cx.languages.markup.tag.addInlined("script", "javascript"), cx.languages.markup.tag.addAttribute(/on(?:abort|blur|change|click|composition(?:end|start|update)|dblclick|error|focus(?:in|out)?|key(?:down|up)|load|mouse(?:down|enter|leave|move|out|over|up)|reset|resize|scroll|select|slotchange|submit|unload|wheel)/.source, "javascript")), cx.languages.js = cx.languages.javascript,
+        }), _x.languages.markup && (_x.languages.markup.tag.addInlined("script", "javascript"), _x.languages.markup.tag.addAttribute(/on(?:abort|blur|change|click|composition(?:end|start|update)|dblclick|error|focus(?:in|out)?|key(?:down|up)|load|mouse(?:down|enter|leave|move|out|over|up)|reset|resize|scroll|select|slotchange|submit|unload|wheel)/.source, "javascript")), _x.languages.js = _x.languages.javascript,
         function(e) {
             var t = e.util.clone(e.languages.javascript),
                 r = /(?:\s|\/\/.*(?!.)|\/\*(?:[^*]|\*(?!\/))\*\/)/.source,
                 n = /(?:\{(?:\{(?:\{[^{}]*\}|[^{}])*\}|[^{}])*\})/.source,
                 a = /(?:\{<S>*\.{3}(?:[^{}]|<BRACES>)*\})/.source;
 
             function o(e, t) {
@@ -18273,15 +18600,15 @@
                         }
                         a.content && "string" != typeof a.content && l(a.content)
                     }
                 };
             e.hooks.add("after-tokenize", (function(e) {
                 "jsx" !== e.language && "tsx" !== e.language || l(e.tokens)
             }))
-        }(cx),
+        }(_x),
         function(e) {
             function t(e, t) {
                 return RegExp(e.replace(/<ID>/g, (function() {
                     return /(?!\s)[_$a-zA-Z\xA0-\uFFFF](?:(?!\s)[$\w\xA0-\uFFFF])*/.source
                 })), t)
             }
             e.languages.insertBefore("javascript", "function-variable", {
@@ -18359,15 +18686,15 @@
                     o = e.languages.javascript[a];
                 "RegExp" === e.util.type(o) && (o = e.languages.javascript[a] = {
                     pattern: o
                 });
                 var i = o.inside || {};
                 o.inside = i, i["maybe-class-name"] = /^[A-Z][\s\S]*/
             }
-        }(cx),
+        }(_x),
         function(e) {
             var t = e.languages.javascript["template-string"],
                 r = t.pattern.source,
                 n = t.inside.interpolation,
                 a = n.inside["interpolation-punctuation"],
                 o = n.pattern.source;
 
@@ -18488,15 +18815,15 @@
                                     }
                                 } else t(i);
                             else "string" != typeof i && t([i])
                         }
                     }
                 }(t.tokens)
             }))
-        }(cx),
+        }(_x),
         function(e) {
             var t = /#(?!\{).+/,
                 r = {
                     pattern: /#\{[^}]+\}/,
                     alias: "variable"
                 };
             e.languages.coffeescript = e.languages.extend("javascript", {
@@ -18555,15 +18882,15 @@
                     inside: {
                         interpolation: r
                     }
                 }]
             }), e.languages.insertBefore("coffeescript", "keyword", {
                 property: /(?!\d)\w+(?=\s*:(?!:))/
             }), delete e.languages.coffeescript["template-string"], e.languages.coffee = e.languages.coffeescript
-        }(cx),
+        }(_x),
         function(e) {
             e.languages.diff = {
                 coord: [/^(?:\*{3}|-{3}|\+{3}).*$/m, /^@@.*@@$/m, /^\d.*$/m]
             };
             var t = {
                 "deleted-sign": "-",
                 "deleted-arrow": "<",
@@ -18588,54 +18915,54 @@
                             alias: /\w+/.exec(r)[0]
                         }
                     }
                 }
             })), Object.defineProperty(e.languages.diff, "PREFIXES", {
                 value: t
             })
-        }(cx), cx.languages.git = {
+        }(_x), _x.languages.git = {
             comment: /^#.*/m,
             deleted: /^[-–].*/m,
             inserted: /^\+.*/m,
             string: /("|')(?:\\.|(?!\1)[^\\\r\n])*\1/,
             command: {
                 pattern: /^.*\$ git .*$/m,
                 inside: {
                     parameter: /\s--?\w+/
                 }
             },
             coord: /^@@.*@@$/m,
             "commit-sha1": /^commit \w{40}$/m
-        }, cx.languages.go = cx.languages.extend("clike", {
+        }, _x.languages.go = _x.languages.extend("clike", {
             string: {
                 pattern: /(^|[^\\])"(?:\\.|[^"\\\r\n])*"|`[^`]*`/,
                 lookbehind: !0,
                 greedy: !0
             },
             keyword: /\b(?:break|case|chan|const|continue|default|defer|else|fallthrough|for|func|go(?:to)?|if|import|interface|map|package|range|return|select|struct|switch|type|var)\b/,
             boolean: /\b(?:_|false|iota|nil|true)\b/,
             number: [/\b0(?:b[01_]+|o[0-7_]+)i?\b/i, /\b0x(?:[a-f\d_]+(?:\.[a-f\d_]*)?|\.[a-f\d_]+)(?:p[+-]?\d+(?:_\d+)*)?i?(?!\w)/i, /(?:\b\d[\d_]*(?:\.[\d_]*)?|\B\.\d[\d_]*)(?:e[+-]?[\d_]+)?i?(?!\w)/i],
             operator: /[*\/%^!=]=?|\+[=+]?|-[=-]?|\|[=|]?|&(?:=|&|\^=?)?|>(?:>=?|=)?|<(?:<=?|=|-)?|:=|\.\.\./,
             builtin: /\b(?:append|bool|byte|cap|close|complex|complex(?:64|128)|copy|delete|error|float(?:32|64)|u?int(?:8|16|32|64)?|imag|len|make|new|panic|print(?:ln)?|real|recover|rune|string|uintptr)\b/
-        }), cx.languages.insertBefore("go", "string", {
+        }), _x.languages.insertBefore("go", "string", {
             char: {
                 pattern: /'(?:\\.|[^'\\\r\n]){0,10}'/,
                 greedy: !0
             }
-        }), delete cx.languages.go["class-name"], cx.languages.graphql = {
+        }), delete _x.languages.go["class-name"], _x.languages.graphql = {
             comment: /#.*/,
             description: {
                 pattern: /(?:"""(?:[^"]|(?!""")")*"""|"(?:\\.|[^\\"\r\n])*")(?=\s*[a-z_])/i,
                 greedy: !0,
                 alias: "string",
                 inside: {
                     "language-markdown": {
                         pattern: /(^"(?:"")?)(?!\1)[\s\S]+(?=\1$)/,
                         lookbehind: !0,
-                        inside: cx.languages.markdown
+                        inside: _x.languages.markdown
                     }
                 }
             },
             string: {
                 pattern: /"""(?:[^"]|(?!""")")*"""|"(?:\\.|[^\\"\r\n])*"/,
                 greedy: !0
             },
@@ -18677,15 +19004,15 @@
             },
             keyword: /\b(?:directive|enum|extend|fragment|implements|input|interface|mutation|on|query|repeatable|scalar|schema|subscription|type|union)\b/,
             operator: /[!=|&]|\.{3}/,
             "property-query": /\w+(?=\s*\()/,
             object: /\w+(?=\s*\{)/,
             punctuation: /[!(){}\[\]:=,]/,
             property: /\w+/
-        }, cx.hooks.add("after-tokenize", (function(e) {
+        }, _x.hooks.add("after-tokenize", (function(e) {
             if ("graphql" === e.language)
                 for (var t = e.tokens.filter((function(e) {
                         return "string" != typeof e && "comment" !== e.type && "scalar" !== e.type
                     })), r = 0; r < t.length;) {
                     var n = t[r++];
                     if ("keyword" === n.type && "mutation" === n.content) {
                         var a = [];
@@ -18783,15 +19110,15 @@
                                 }
                                 return l
                             }(r.tokens)
                         }
                     }
                 }
             })
-        }(cx),
+        }(_x),
         function(e) {
             e.languages.handlebars = {
                 comment: /\{\{![\s\S]*?\}\}/,
                 delimiter: {
                     pattern: /^\{\{\{?|\}\}\}?$/,
                     alias: "punctuation"
                 },
@@ -18813,15 +19140,15 @@
                 punctuation: /[!"#%&':()*+,.\/;<=>@\[\\\]^`{|}~]/,
                 variable: /[^!"#%&'()*+,\/;<=>@\[\\\]^`{|}~\s]+/
             }, e.hooks.add("before-tokenize", (function(t) {
                 e.languages["markup-templating"].buildPlaceholders(t, "handlebars", /\{\{\{[\s\S]+?\}\}\}|\{\{[\s\S]+?\}\}/g)
             })), e.hooks.add("after-tokenize", (function(t) {
                 e.languages["markup-templating"].tokenizePlaceholders(t, "handlebars")
             })), e.languages.hbs = e.languages.handlebars
-        }(cx), cx.languages.json = {
+        }(_x), _x.languages.json = {
             property: {
                 pattern: /(^|[^\\])"(?:\\.|[^\\"\r\n])*"(?=\s*:)/,
                 lookbehind: !0,
                 greedy: !0
             },
             string: {
                 pattern: /(^|[^\\])"(?:\\.|[^\\"\r\n])*"(?!\s*:)/,
@@ -18836,15 +19163,15 @@
             punctuation: /[{}[\],]/,
             operator: /:/,
             boolean: /\b(?:false|true)\b/,
             null: {
                 pattern: /\bnull\b/,
                 alias: "keyword"
             }
-        }, cx.languages.webmanifest = cx.languages.json, cx.languages.less = cx.languages.extend("css", {
+        }, _x.languages.webmanifest = _x.languages.json, _x.languages.less = _x.languages.extend("css", {
             comment: [/\/\*[\s\S]*?\*\//, {
                 pattern: /(^|[^\\])\/\/.*/,
                 lookbehind: !0
             }],
             atrule: {
                 pattern: /@[\w-](?:\((?:[^(){}]|\([^(){}]*\))*\)|[^(){};\s]|\s+(?!\s))*?(?=\s*\{)/,
                 inside: {
@@ -18855,27 +19182,27 @@
                 pattern: /(?:@\{[\w-]+\}|[^{};\s@])(?:@\{[\w-]+\}|\((?:[^(){}]|\([^(){}]*\))*\)|[^(){};@\s]|\s+(?!\s))*?(?=\s*\{)/,
                 inside: {
                     variable: /@+[\w-]+/
                 }
             },
             property: /(?:@\{[\w-]+\}|[\w-])+(?:\+_?)?(?=\s*:)/,
             operator: /[+\-*\/]/
-        }), cx.languages.insertBefore("less", "property", {
+        }), _x.languages.insertBefore("less", "property", {
             variable: [{
                 pattern: /@[\w-]+\s*:/,
                 inside: {
                     punctuation: /:/
                 }
             }, /@@?[\w-]+/],
             "mixin-usage": {
                 pattern: /([{;]\s*)[.#](?!\d)[\w-].*?(?=[(;])/,
                 lookbehind: !0,
                 alias: "function"
             }
-        }), cx.languages.makefile = {
+        }), _x.languages.makefile = {
             comment: {
                 pattern: /(^|[^\\])#(?:\\(?:\r\n|[\s\S])|[^\\\r\n])*/,
                 lookbehind: !0
             },
             string: {
                 pattern: /(["'])(?:\\(?:\r\n|[\s\S])|(?!\1)[^\\\r\n])*\1/,
                 greedy: !0
@@ -19141,22 +19468,22 @@
                     amp: "&",
                     lt: "<",
                     gt: ">",
                     quot: '"'
                 },
                 s = String.fromCodePoint || String.fromCharCode;
             e.languages.md = e.languages.markdown
-        }(cx), cx.languages.objectivec = cx.languages.extend("c", {
+        }(_x), _x.languages.objectivec = _x.languages.extend("c", {
             string: {
                 pattern: /@?"(?:\\(?:\r\n|[\s\S])|[^"\\\r\n])*"/,
                 greedy: !0
             },
             keyword: /\b(?:asm|auto|break|case|char|const|continue|default|do|double|else|enum|extern|float|for|goto|if|in|inline|int|long|register|return|self|short|signed|sizeof|static|struct|super|switch|typedef|typeof|union|unsigned|void|volatile|while)\b|(?:@interface|@end|@implementation|@protocol|@class|@public|@protected|@private|@property|@try|@catch|@finally|@throw|@synthesize|@dynamic|@selector)\b/,
             operator: /-[->]?|\+\+?|!=?|<<?=?|>>?=?|==?|&&?|\|\|?|[~^%?*\/@]/
-        }), delete cx.languages.objectivec["class-name"], cx.languages.objc = cx.languages.objectivec, cx.languages.ocaml = {
+        }), delete _x.languages.objectivec["class-name"], _x.languages.objc = _x.languages.objectivec, _x.languages.ocaml = {
             comment: {
                 pattern: /\(\*[\s\S]*?\*\)/,
                 greedy: !0
             },
             char: {
                 pattern: /'(?:[^\\\r\n']|\\(?:.|[ox]?[0-9a-f]{1,3}))'/i,
                 greedy: !0
@@ -19189,15 +19516,15 @@
             boolean: /\b(?:false|true)\b/,
             "operator-like-punctuation": {
                 pattern: /\[[<>|]|[>|]\]|\{<|>\}/,
                 alias: "punctuation"
             },
             operator: /\.[.~]|:[=>]|[=<>@^|&+\-*\/$%!?~][!$%&*+\-.\/:<=>?@^|~]*|\b(?:and|asr|land|lor|lsl|lsr|lxor|mod|or)\b/,
             punctuation: /;;|::|[(){}\[\].,:;#]|\b_\b/
-        }, cx.languages.python = {
+        }, _x.languages.python = {
             comment: {
                 pattern: /(^|[^\\])#.*/,
                 lookbehind: !0,
                 greedy: !0
             },
             "string-interpolation": {
                 pattern: /(?:f|fr|rf)(?:("""|''')[\s\S]*?\1|("|')(?:\\.|(?!\2)[^\\\r\n])*\2)/i,
@@ -19248,33 +19575,33 @@
             },
             keyword: /\b(?:_(?=\s*:)|and|as|assert|async|await|break|case|class|continue|def|del|elif|else|except|exec|finally|for|from|global|if|import|in|is|lambda|match|nonlocal|not|or|pass|print|raise|return|try|while|with|yield)\b/,
             builtin: /\b(?:__import__|abs|all|any|apply|ascii|basestring|bin|bool|buffer|bytearray|bytes|callable|chr|classmethod|cmp|coerce|compile|complex|delattr|dict|dir|divmod|enumerate|eval|execfile|file|filter|float|format|frozenset|getattr|globals|hasattr|hash|help|hex|id|input|int|intern|isinstance|issubclass|iter|len|list|locals|long|map|max|memoryview|min|next|object|oct|open|ord|pow|property|range|raw_input|reduce|reload|repr|reversed|round|set|setattr|slice|sorted|staticmethod|str|sum|super|tuple|type|unichr|unicode|vars|xrange|zip)\b/,
             boolean: /\b(?:False|None|True)\b/,
             number: /\b0(?:b(?:_?[01])+|o(?:_?[0-7])+|x(?:_?[a-f0-9])+)\b|(?:\b\d+(?:_\d+)*(?:\.(?:\d+(?:_\d+)*)?)?|\B\.\d+(?:_\d+)*)(?:e[+-]?\d+(?:_\d+)*)?j?(?!\w)/i,
             operator: /[-+%=]=?|!=|:=|\*\*?=?|\/\/?=?|<[<=>]?|>[=>]?|[&|^~]/,
             punctuation: /[{}[\];(),.:]/
-        }, cx.languages.python["string-interpolation"].inside.interpolation.inside.rest = cx.languages.python, cx.languages.py = cx.languages.python, cx.languages.reason = cx.languages.extend("clike", {
+        }, _x.languages.python["string-interpolation"].inside.interpolation.inside.rest = _x.languages.python, _x.languages.py = _x.languages.python, _x.languages.reason = _x.languages.extend("clike", {
             string: {
                 pattern: /"(?:\\(?:\r\n|[\s\S])|[^\\\r\n"])*"/,
                 greedy: !0
             },
             "class-name": /\b[A-Z]\w*/,
             keyword: /\b(?:and|as|assert|begin|class|constraint|do|done|downto|else|end|exception|external|for|fun|function|functor|if|in|include|inherit|initializer|lazy|let|method|module|mutable|new|nonrec|object|of|open|or|private|rec|sig|struct|switch|then|to|try|type|val|virtual|when|while|with)\b/,
             operator: /\.{3}|:[:=]|\|>|->|=(?:==?|>)?|<=?|>=?|[|^?'#!~`]|[+\-*\/]\.?|\b(?:asr|land|lor|lsl|lsr|lxor|mod)\b/
-        }), cx.languages.insertBefore("reason", "class-name", {
+        }), _x.languages.insertBefore("reason", "class-name", {
             char: {
                 pattern: /'(?:\\x[\da-f]{2}|\\o[0-3][0-7][0-7]|\\\d{3}|\\.|[^'\\\r\n])'/,
                 greedy: !0
             },
             constructor: /\b[A-Z]\w*\b(?!\s*\.)/,
             label: {
                 pattern: /\b[a-z]\w*(?=::)/,
                 alias: "symbol"
             }
-        }), delete cx.languages.reason.function,
+        }), delete _x.languages.reason.function,
         function(e) {
             e.languages.sass = e.languages.extend("css", {
                 comment: {
                     pattern: /^([ \t]*)\/[\/*].*(?:(?:\r?\n|\r)\1[ \t].+)*/m,
                     lookbehind: !0,
                     greedy: !0
                 }
@@ -19319,15 +19646,15 @@
             }), delete e.languages.sass.property, delete e.languages.sass.important, e.languages.insertBefore("sass", "punctuation", {
                 selector: {
                     pattern: /^([ \t]*)\S(?:,[^,\r\n]+|[^,\r\n]*)(?:,[^,\r\n]+)*(?:,(?:\r?\n|\r)\1[ \t]+\S(?:,[^,\r\n]+|[^,\r\n]*)(?:,[^,\r\n]+)*)*/m,
                     lookbehind: !0,
                     greedy: !0
                 }
             })
-        }(cx), cx.languages.scss = cx.languages.extend("css", {
+        }(_x), _x.languages.scss = _x.languages.extend("css", {
             comment: {
                 pattern: /(^|[^\\])(?:\/\*[\s\S]*?\*\/|\/\/.*)/,
                 lookbehind: !0
             },
             atrule: {
                 pattern: /@[\w-](?:\([^()]+\)|[^()\s]|\s+(?!\s))*?(?=\s+[{;])/,
                 inside: {
@@ -19348,22 +19675,22 @@
             },
             property: {
                 pattern: /(?:[-\w]|\$[-\w]|#\{\$[-\w]+\})+(?=\s*:)/,
                 inside: {
                     variable: /\$[-\w]+|#\{\$[-\w]+\}/
                 }
             }
-        }), cx.languages.insertBefore("scss", "atrule", {
+        }), _x.languages.insertBefore("scss", "atrule", {
             keyword: [/@(?:content|debug|each|else(?: if)?|extend|for|forward|function|if|import|include|mixin|return|use|warn|while)\b/i, {
                 pattern: /( )(?:from|through)(?= )/,
                 lookbehind: !0
             }]
-        }), cx.languages.insertBefore("scss", "important", {
+        }), _x.languages.insertBefore("scss", "important", {
             variable: /\$[-\w]+|#\{\$[-\w]+\}/
-        }), cx.languages.insertBefore("scss", "function", {
+        }), _x.languages.insertBefore("scss", "function", {
             "module-modifier": {
                 pattern: /\b(?:as|hide|show|with)\b/i,
                 alias: "keyword"
             },
             placeholder: {
                 pattern: /%[-\w]+/,
                 alias: "selector"
@@ -19377,15 +19704,15 @@
                 pattern: /\bnull\b/,
                 alias: "keyword"
             },
             operator: {
                 pattern: /(\s)(?:[-+*\/%]|[=!]=|<=?|>=?|and|not|or)(?=\s)/,
                 lookbehind: !0
             }
-        }), cx.languages.scss.atrule.inside.rest = cx.languages.scss, cx.languages.sql = {
+        }), _x.languages.scss.atrule.inside.rest = _x.languages.scss, _x.languages.sql = {
             comment: {
                 pattern: /(^|[^\\])(?:\/\*[\s\S]*?\*\/|(?:--|\/\/|#).*)/,
                 lookbehind: !0
             },
             variable: [{
                 pattern: /@(["'`])(?:\\[\s\S]|(?!\1)[^\\])+\1/,
                 greedy: !0
@@ -19525,15 +19852,15 @@
                     pattern: /(^|[^\\])(?:\/\*[\s\S]*?\*\/|\/\/.*)/,
                     lookbehind: !0,
                     greedy: !0
                 },
                 interpolation: n.interpolation,
                 punctuation: /[{}()\[\];:.]/
             }
-        }(cx),
+        }(_x),
         function(e) {
             e.languages.typescript = e.languages.extend("javascript", {
                 "class-name": {
                     pattern: /(\b(?:class|extends|implements|instanceof|interface|new|type)\s+)(?!keyof\b)(?!\s)[_$a-zA-Z\xA0-\uFFFF](?:(?!\s)[$\w\xA0-\uFFFF])*(?:\s*<(?:[^<>]|<(?:[^<>]|<[^<>]*>)*>)*>)?/,
                     lookbehind: !0,
                     greedy: !0,
                     inside: null
@@ -19561,21 +19888,21 @@
                             pattern: /<[\s\S]+/,
                             alias: "class-name",
                             inside: t
                         }
                     }
                 }
             }), e.languages.ts = e.languages.typescript
-        }(cx),
+        }(_x),
         function(e) {
             var t = e.util.clone(e.languages.typescript);
             e.languages.tsx = e.languages.extend("jsx", t), delete e.languages.tsx.parameter, delete e.languages.tsx["literal-property"];
             var r = e.languages.tsx.tag;
             r.pattern = RegExp(/(^|[^\w$]|(?=<\/))/.source + "(?:" + r.pattern.source + ")", r.pattern.flags), r.lookbehind = !0
-        }(cx), cx.languages.wasm = {
+        }(_x), _x.languages.wasm = {
             comment: [/\(;[\s\S]*?;\)/, {
                 pattern: /;;.*/,
                 greedy: !0
             }],
             string: {
                 pattern: /"(?:\\[\s\S]|[^"\\])*"/,
                 greedy: !0
@@ -19661,17 +19988,17 @@
                     pattern: i(/[+-]?(?:0x[\da-f]+|0o[0-7]+|(?:\d+(?:\.\d*)?|\.\d+)(?:e[+-]?\d+)?|\.inf|\.nan)/.source, "i"),
                     lookbehind: !0
                 },
                 tag: r,
                 important: t,
                 punctuation: /---|[:[\]{}\-,|>?]|\.\.\./
             }, e.languages.yml = e.languages.yaml
-        }(cx);
-    var ux = {
-        Prism: cx,
+        }(_x);
+    var Lx = {
+        Prism: _x,
         theme: {
             plain: {
                 backgroundColor: "#2a2734",
                 color: "#9a86fd"
             },
             styles: [{
                 types: ["comment", "prolog", "doctype", "cdata", "punctuation"],
@@ -19733,85 +20060,85 @@
                 style: {
                     color: "#c4b9fe"
                 }
             }]
         }
     };
 
-    function dx(e, t, r) {
+    function Ax(e, t, r) {
         return t in e ? Object.defineProperty(e, t, {
             value: r,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = r, e
     }
 
-    function px() {
-        return (px = Object.assign || function(e) {
+    function Mx() {
+        return (Mx = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    var fx = /\r\n|\r|\n/,
-        mx = function(e) {
+    var Fx = /\r\n|\r|\n/,
+        $x = function(e) {
             0 === e.length ? e.push({
                 types: ["plain"],
                 content: "\n",
                 empty: !0
             }) : 1 === e.length && "" === e[0].content && (e[0].content = "\n", e[0].empty = !0)
         },
-        bx = function(e, t) {
+        Bx = function(e, t) {
             var r = e.length;
             return r > 0 && e[r - 1] === t ? e : e.concat(t)
         },
-        gx = function(e, t) {
+        Wx = function(e, t) {
             var r = e.plain,
                 n = Object.create(null),
                 a = e.styles.reduce((function(e, r) {
                     var n = r.languages,
                         a = r.style;
                     return n && !n.includes(t) || r.types.forEach((function(t) {
-                        var r = px({}, e[t], a);
+                        var r = Mx({}, e[t], a);
                         e[t] = r
                     })), e
                 }), n);
-            return a.root = r, a.plain = px({}, r, {
+            return a.root = r, a.plain = Mx({}, r, {
                 backgroundColor: null
             }), a
         };
 
-    function yx(e, t) {
+    function Hx(e, t) {
         var r = {};
         for (var n in e) Object.prototype.hasOwnProperty.call(e, n) && -1 === t.indexOf(n) && (r[n] = e[n]);
         return r
     }
-    var hx = function(e) {
+    var Vx = function(e) {
         function t() {
             for (var t = this, r = [], n = arguments.length; n--;) r[n] = arguments[n];
-            e.apply(this, r), dx(this, "getThemeDict", (function(e) {
+            e.apply(this, r), Ax(this, "getThemeDict", (function(e) {
                 if (void 0 !== t.themeDict && e.theme === t.prevTheme && e.language === t.prevLanguage) return t.themeDict;
                 t.prevTheme = e.theme, t.prevLanguage = e.language;
-                var r = e.theme ? gx(e.theme, e.language) : void 0;
+                var r = e.theme ? Wx(e.theme, e.language) : void 0;
                 return t.themeDict = r
-            })), dx(this, "getLineProps", (function(e) {
+            })), Ax(this, "getLineProps", (function(e) {
                 var r = e.key,
                     n = e.className,
                     a = e.style,
-                    o = px({}, yx(e, ["key", "className", "style", "line"]), {
+                    o = Mx({}, Hx(e, ["key", "className", "style", "line"]), {
                         className: "token-line",
                         style: void 0,
                         key: void 0
                     }),
                     i = t.getThemeDict(t.props);
-                return void 0 !== i && (o.style = i.plain), void 0 !== a && (o.style = void 0 !== o.style ? px({}, o.style, a) : a), void 0 !== r && (o.key = r), n && (o.className += " " + n), o
-            })), dx(this, "getStyleForToken", (function(e) {
+                return void 0 !== i && (o.style = i.plain), void 0 !== a && (o.style = void 0 !== o.style ? Mx({}, o.style, a) : a), void 0 !== r && (o.key = r), n && (o.className += " " + n), o
+            })), Ax(this, "getStyleForToken", (function(e) {
                 var r = e.types,
                     n = e.empty,
                     a = r.length,
                     o = t.getThemeDict(t.props);
                 if (void 0 !== o) {
                     if (1 === a && "plain" === r[0]) return n ? {
                         display: "inline-block"
@@ -19821,27 +20148,27 @@
                             display: "inline-block"
                         } : {},
                         l = r.map((function(e) {
                             return o[e]
                         }));
                     return Object.assign.apply(Object, [i].concat(l))
                 }
-            })), dx(this, "getTokenProps", (function(e) {
+            })), Ax(this, "getTokenProps", (function(e) {
                 var r = e.key,
                     n = e.className,
                     a = e.style,
                     o = e.token,
-                    i = px({}, yx(e, ["key", "className", "style", "token"]), {
+                    i = Mx({}, Hx(e, ["key", "className", "style", "token"]), {
                         className: "token " + o.types.join(" "),
                         children: o.content,
                         style: t.getStyleForToken(o),
                         key: void 0
                     });
-                return void 0 !== a && (i.style = void 0 !== i.style ? px({}, i.style, a) : a), void 0 !== r && (i.key = r), n && (i.className += " " + n), i
-            })), dx(this, "tokenize", (function(e, t, r, n) {
+                return void 0 !== a && (i.style = void 0 !== i.style ? Mx({}, i.style, a) : a), void 0 !== r && (i.key = r), n && (i.className += " " + n), i
+            })), Ax(this, "tokenize", (function(e, t, r, n) {
                 var a = {
                     code: t,
                     grammar: r,
                     language: n,
                     tokens: []
                 };
                 e.hooks.run("before-tokenize", a);
@@ -19863,40 +20190,40 @@
                             []
                         ], r = [e], n = [0], a = [e.length], o = 0, i = 0, l = [], s = [l]; i > -1;) {
                         for (;
                             (o = n[i]++) < a[i];) {
                             var c = void 0,
                                 u = t[i],
                                 d = r[i][o];
-                            if ("string" == typeof d ? (u = i > 0 ? u : ["plain"], c = d) : (u = bx(u, d.type), d.alias && (u = bx(u, d.alias)), c = d.content), "string" == typeof c) {
-                                var p = c.split(fx),
+                            if ("string" == typeof d ? (u = i > 0 ? u : ["plain"], c = d) : (u = Bx(u, d.type), d.alias && (u = Bx(u, d.alias)), c = d.content), "string" == typeof c) {
+                                var p = c.split(Fx),
                                     f = p.length;
                                 l.push({
                                     types: u,
                                     content: p[0]
                                 });
-                                for (var m = 1; m < f; m++) mx(l), s.push(l = []), l.push({
+                                for (var m = 1; m < f; m++) $x(l), s.push(l = []), l.push({
                                     types: u,
                                     content: p[m]
                                 })
                             } else i++, t.push(u), r.push(c), n.push(0), a.push(c.length)
                         }
                         i--, t.pop(), r.pop(), n.pop(), a.pop()
                     }
-                    return mx(l), s
+                    return $x(l), s
                 }(void 0 !== i ? this.tokenize(t, n, i, r) : [n]),
                 className: "prism-code language-" + r,
                 style: void 0 !== o ? o.root : {},
                 getLineProps: this.getLineProps,
                 getTokenProps: this.getTokenProps
             })
         }, t
     }(n.Component);
 
-    function vx({
+    function qx({
         timeout: e = 2e3
     } = {}) {
         const [t, r] = Object(n.useState)(null), [a, o] = Object(n.useState)(!1), [i, l] = Object(n.useState)(null);
         return {
             copy: t => {
                 "clipboard" in navigator ? navigator.clipboard.writeText(t).then(() => {
                     return t = !0, clearTimeout(i), l(setTimeout(() => o(!1), e)), void o(t);
@@ -19907,15 +20234,15 @@
                 o(!1), r(null), clearTimeout(i)
             },
             error: t,
             copied: a
         }
     }
 
-    function Ox({
+    function Ux({
         copied: e
     }) {
         return a.a.createElement("svg", {
             width: "15",
             height: "15",
             viewBox: "0 0 15 15",
             fill: "none",
@@ -19928,16 +20255,16 @@
         }) : a.a.createElement("path", {
             d: "M5 2V1H10V2H5ZM4.75 0C4.33579 0 4 0.335786 4 0.75V1H3.5C2.67157 1 2 1.67157 2 2.5V12.5C2 13.3284 2.67157 14 3.5 14H11.5C12.3284 14 13 13.3284 13 12.5V2.5C13 1.67157 12.3284 1 11.5 1H11V0.75C11 0.335786 10.6642 0 10.25 0H4.75ZM11 2V2.25C11 2.66421 10.6642 3 10.25 3H4.75C4.33579 3 4 2.66421 4 2.25V2H3.5C3.22386 2 3 2.22386 3 2.5V12.5C3 12.7761 3.22386 13 3.5 13H11.5C11.7761 13 12 12.7761 12 12.5V2.5C12 2.22386 11.7761 2 11.5 2H11Z",
             fill: "currentColor",
             fillRule: "evenodd",
             clipRule: "evenodd"
         }))
     }
-    Ox.displayName = "@mantine/prism/CopyIcon";
-    const wx = (e, t) => "dark" === t ? (e => ({
+    Ux.displayName = "@mantine/prism/CopyIcon";
+    const Gx = (e, t) => "dark" === t ? (e => ({
         plain: {
             color: e.colors.gray[4],
             backgroundColor: e.colors.dark[8]
         },
         styles: [{
             types: ["comment"],
             style: {
@@ -20077,15 +20404,15 @@
         }, {
             types: ["url"],
             style: {
                 color: e.colors.gray[7]
             }
         }]
     }))(e);
-    var xx = Er((e, {
+    var Yx = Er((e, {
             colorScheme: t,
             native: r,
             maxLineSize: n
         }) => ({
             scrollArea: {},
             root: {
                 position: "relative"
@@ -20122,15 +20449,15 @@
                 marginLeft: "rtl" === e.dir ? e.spacing.xs : void 0,
                 userSelect: "none"
             },
             lineContent: {
                 width: "100%"
             }
         })),
-        Sx = Er(e => ({
+        Zx = Er(e => ({
             tabs: {
                 borderBottom: "1px solid " + ("dark" === e.colorScheme ? e.colors.dark[5] : e.colors.gray[2])
             },
             tab: {
                 paddingLeft: e.spacing.sm,
                 paddingRight: e.spacing.sm,
                 height: 34,
@@ -20159,51 +20486,51 @@
             code: {
                 borderTopRightRadius: 0,
                 borderTopLeftRadius: 0,
                 border: "1px solid " + ("dark" === e.colorScheme ? e.colors.dark[5] : e.colors.gray[2]),
                 borderTop: 0
             }
         })),
-        kx = Object.defineProperty,
-        Ex = Object.defineProperties,
-        jx = Object.getOwnPropertyDescriptors,
-        Px = Object.getOwnPropertySymbols,
-        zx = Object.prototype.hasOwnProperty,
-        Cx = Object.prototype.propertyIsEnumerable,
-        Nx = (e, t, r) => t in e ? kx(e, t, {
+        Kx = Object.defineProperty,
+        Xx = Object.defineProperties,
+        Jx = Object.getOwnPropertyDescriptors,
+        Qx = Object.getOwnPropertySymbols,
+        eS = Object.prototype.hasOwnProperty,
+        tS = Object.prototype.propertyIsEnumerable,
+        rS = (e, t, r) => t in e ? Kx(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        Tx = (e, t) => {
-            for (var r in t || (t = {})) zx.call(t, r) && Nx(e, r, t[r]);
-            if (Px)
-                for (var r of Px(t)) Cx.call(t, r) && Nx(e, r, t[r]);
+        nS = (e, t) => {
+            for (var r in t || (t = {})) eS.call(t, r) && rS(e, r, t[r]);
+            if (Qx)
+                for (var r of Qx(t)) tS.call(t, r) && rS(e, r, t[r]);
             return e
         },
-        Dx = (e, t) => Ex(e, jx(t)),
-        Ix = (e, t) => {
+        aS = (e, t) => Xx(e, Jx(t)),
+        oS = (e, t) => {
             var r = {};
-            for (var n in e) zx.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-            if (null != e && Px)
-                for (var n of Px(e)) t.indexOf(n) < 0 && Cx.call(e, n) && (r[n] = e[n]);
+            for (var n in e) eS.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+            if (null != e && Qx)
+                for (var n of Qx(e)) t.indexOf(n) < 0 && tS.call(e, n) && (r[n] = e[n]);
             return r
         };
-    const Rx = {
+    const iS = {
             noCopy: !1,
             copyLabel: "Copy code",
             copiedLabel: "Copied",
             withLineNumbers: !1,
             trim: !0,
             highlightLines: {},
             scrollAreaComponent: ag
         },
-        _x = Object(n.forwardRef)((e, t) => {
-            const r = ir("Prism", Rx, e),
+        lS = Object(n.forwardRef)((e, t) => {
+            const r = ir("Prism", iS, e),
                 {
                     className: n,
                     children: o,
                     language: i,
                     noCopy: l,
                     classNames: s,
                     styles: c,
@@ -20211,51 +20538,51 @@
                     copiedLabel: d,
                     withLineNumbers: p,
                     highlightLines: f,
                     scrollAreaComponent: m,
                     colorScheme: b,
                     trim: g
                 } = r,
-                y = Ix(r, ["className", "children", "language", "noCopy", "classNames", "styles", "copyLabel", "copiedLabel", "withLineNumbers", "highlightLines", "scrollAreaComponent", "colorScheme", "trim"]),
+                y = oS(r, ["className", "children", "language", "noCopy", "classNames", "styles", "copyLabel", "copiedLabel", "withLineNumbers", "highlightLines", "scrollAreaComponent", "colorScheme", "trim"]),
                 h = g && "string" == typeof o ? o.trim() : o,
                 v = h.split("\n").length.toString().length,
                 O = or(),
-                w = vx(),
+                w = qx(),
                 {
                     classes: x,
                     cx: S
-                } = xx({
+                } = Yx({
                     colorScheme: b || O.colorScheme,
                     native: m !== ag,
                     maxLineSize: v
                 }, {
                     classNames: s,
                     styles: c,
                     name: "Prism"
                 });
-            return a.a.createElement(Cn, Tx({
+            return a.a.createElement(Cn, nS({
                 className: S(x.root, n),
                 ref: t
-            }, y), !l && a.a.createElement(Kw, {
+            }, y), !l && a.a.createElement(xx, {
                 className: x.copy,
                 label: w.copied ? d : u,
                 position: "left",
                 placement: "center",
                 transition: "fade",
                 withArrow: !0,
                 arrowSize: 4,
                 gutter: 8,
                 color: w.copied ? "teal" : "gray"
             }, a.a.createElement(ol, {
                 "aria-label": w.copied ? d : u,
                 onClick: () => w.copy(h)
-            }, a.a.createElement(Ox, {
+            }, a.a.createElement(Ux, {
                 copied: w.copied
-            }))), a.a.createElement(hx, Dx(Tx({}, ux), {
-                theme: wx(O, b || O.colorScheme),
+            }))), a.a.createElement(Vx, aS(nS({}, Lx), {
+                theme: Gx(O, b || O.colorScheme),
                 code: h,
                 language: i
             }), ({
                 className: e,
                 style: t,
                 tokens: r,
                 getLineProps: n,
@@ -20273,17 +20600,17 @@
                 const u = t + 1,
                     d = n({
                         line: e,
                         key: t
                     }),
                     m = u in f,
                     b = "dark" === O.colorScheme ? O.fn.rgba(O.fn.themeColor(null == (i = f[u]) ? void 0 : i.color, 9), .25) : O.fn.themeColor(null == (l = f[u]) ? void 0 : l.color, 0);
-                return a.a.createElement("div", Dx(Tx({}, d), {
+                return a.a.createElement("div", aS(nS({}, d), {
                     className: S(x.line, d.className),
-                    style: Tx({}, m ? {
+                    style: nS({}, m ? {
                         backgroundColor: b
                     } : null)
                 }), p && a.a.createElement("div", {
                     className: x.lineNumber,
                     style: {
                         color: m ? O.fn.themeColor(null == (s = f[u]) ? void 0 : s.color, "dark" === O.colorScheme ? 5 : 8) : void 0
                     }
@@ -20291,91 +20618,91 @@
                     className: x.lineContent
                 }, e.map((e, t) => {
                     var r, n;
                     const i = o({
                         token: e,
                         key: t
                     });
-                    return a.a.createElement("span", Dx(Tx({}, i), {
-                        style: Dx(Tx({}, i.style), {
+                    return a.a.createElement("span", aS(nS({}, i), {
+                        style: aS(nS({}, i.style), {
                             color: m ? O.fn.themeColor(null == (r = f[u]) ? void 0 : r.color, "dark" === O.colorScheme ? 5 : 8) : null == (n = null == i ? void 0 : i.style) ? void 0 : n.color
                         })
                     }))
                 })))
             }).filter(Boolean)))))
         });
 
-    function Lx(e) {
+    function sS(e) {
         return null
     }
-    const Ax = Object(n.forwardRef)((e, t) => {
+    const cS = Object(n.forwardRef)((e, t) => {
         const r = ir("PrismTabs", {}, e),
             {
                 children: o,
                 classNames: i,
                 styles: l
             } = r,
-            s = Ix(r, ["children", "classNames", "styles"]),
+            s = oS(r, ["children", "classNames", "styles"]),
             {
                 classes: c,
                 cx: u
-            } = Sx(null, {
+            } = Zx(null, {
                 name: "PrismTabs",
                 classNames: i,
                 styles: l
             }),
-            d = n.Children.toArray(o).filter(e => e.type === Lx).map((e, t) => {
+            d = n.Children.toArray(o).filter(e => e.type === sS).map((e, t) => {
                 const r = e.props,
                     {
                         label: n,
                         icon: o
                     } = r,
-                    s = Ix(r, ["label", "icon"]);
+                    s = oS(r, ["label", "icon"]);
                 return a.a.createElement(Ua.Tab, {
                     label: n,
                     icon: o,
                     key: t
-                }, a.a.createElement(_x, Dx(Tx({}, s), {
+                }, a.a.createElement(lS, aS(nS({}, s), {
                     styles: l,
-                    classNames: Dx(Tx({}, i), {
+                    classNames: aS(nS({}, i), {
                         code: u(c.code, null == i ? void 0 : i.code)
                     })
                 })))
             });
-        return a.a.createElement(Ua, Tx({
+        return a.a.createElement(Ua, nS({
             ref: t,
             variant: "unstyled",
             tabPadding: 0,
             classNames: {
                 tabsList: u(c.tabs, null == i ? void 0 : i.tabs),
                 tabActive: u(c.tabActive, null == i ? void 0 : i.tabActive),
                 tabControl: u(c.tab, null == i ? void 0 : i.tab)
             }
         }, s), d)
     });
 
-    function Mx() {
-        return (Mx = Object.assign || function(e) {
+    function uS() {
+        return (uS = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    _x.Tabs = Ax, _x.Tab = Lx, _x.displayName = "@mantine/prism/Prism", Ax.displayName = "@mantine/prism/Tabs", Lx.displayName = "@mantine/prism/Tab";
-    var Fx = function(e) {
+    lS.Tabs = cS, lS.Tab = sS, lS.displayName = "@mantine/prism/Prism", cS.displayName = "@mantine/prism/Tabs", sS.displayName = "@mantine/prism/Tab";
+    var dS = function(e) {
         var t = e.class_name;
-        return a.a.createElement(_x, Mx({}, G(["children", "setProps", "class_name"], e), {
+        return a.a.createElement(lS, uS({}, G(["children", "setProps", "class_name"], e), {
             className: t
         }), e.children)
     };
-    Fx.displayName = "Prism", Fx.defaultProps = {
+    dS.displayName = "Prism", dS.defaultProps = {
         trim: !0
-    }, Fx.propTypes = {
+    }, dS.propTypes = {
         class_name: i.a.string,
         children: i.a.string,
         colorScheme: i.a.oneOf(["light", "dark"]),
         copiedLabel: i.a.string,
         copyLabel: i.a.string,
         highlightLines: i.a.objectOf(i.a.exact({
             color: i.a.oneOf(["dark", "gray", "red", "pink", "grape", "violet", "indigo", "blue", "cyan", "teal", "green", "lime", "yellow", "orange"]),
@@ -20384,60 +20711,60 @@
         id: i.a.string,
         language: i.a.oneOf(["markup", "bash", "clike", "c", "cpp", "css", "javascript", "jsx", "coffeescript", "actionscript", "css-extr", "diff", "git", "go", "graphql", "handlebars", "json", "less", "makefile", "markdown", "objectivec", "ocaml", "python", "reason", "sass", "scss", "sql", "stylus", "tsx", "typescript", "wasm", "yaml"]).isRequired,
         noCopy: i.a.bool,
         style: i.a.object,
         trim: i.a.bool,
         withLineNumbers: i.a.bool
     };
-    var $x = Fx;
+    var pS = dS;
 
-    function Bx(e) {
+    function fS(e) {
         const t = Object(n.createContext)(e);
         return [t.Provider, function(e) {
             const r = Object(n.useContext)(t),
                 [a] = e.split(".");
             if (!r) throw new Error(`${e} component was rendered outside of ${a} component context`);
             return r
         }]
     }
-    const [Wx, Hx] = Bx(null);
-    var Vx = Object.defineProperty,
-        qx = Object.getOwnPropertySymbols,
-        Ux = Object.prototype.hasOwnProperty,
-        Gx = Object.prototype.propertyIsEnumerable,
-        Yx = (e, t, r) => t in e ? Vx(e, t, {
+    const [mS, bS] = fS(null);
+    var gS = Object.defineProperty,
+        yS = Object.getOwnPropertySymbols,
+        hS = Object.prototype.hasOwnProperty,
+        vS = Object.prototype.propertyIsEnumerable,
+        OS = (e, t, r) => t in e ? gS(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        Zx = (e, t) => {
-            for (var r in t || (t = {})) Ux.call(t, r) && Yx(e, r, t[r]);
-            if (qx)
-                for (var r of qx(t)) Gx.call(t, r) && Yx(e, r, t[r]);
+        wS = (e, t) => {
+            for (var r in t || (t = {})) hS.call(t, r) && OS(e, r, t[r]);
+            if (yS)
+                for (var r of yS(t)) vS.call(t, r) && OS(e, r, t[r]);
             return e
         };
-    const Kx = (e, t) => 100 / (t / e) + "%",
-        Xx = (e, t) => e ? 100 / (t / e) + "%" : void 0;
+    const xS = (e, t) => 100 / (t / e) + "%",
+        SS = (e, t) => e ? 100 / (t / e) + "%" : void 0;
 
-    function Jx({
+    function kS({
         sizes: e,
         offsets: t,
         theme: r,
         columns: n,
         grow: a
     }) {
         return se.reduce((o, i) => ("number" == typeof e[i] && (o[`@media (min-width: ${r.breakpoints[i]+1}px)`] = {
-            flexBasis: Kx(e[i], n),
+            flexBasis: xS(e[i], n),
             flexShrink: 0,
-            maxWidth: a ? "unset" : Kx(e[i], n),
-            marginLeft: Xx(t[i], n)
+            maxWidth: a ? "unset" : xS(e[i], n),
+            marginLeft: SS(t[i], n)
         }), o), {})
     }
-    var Qx = Er((e, {
+    var ES = Er((e, {
             gutter: t,
             grow: r,
             offset: n,
             offsetXs: a,
             offsetSm: o,
             offsetMd: i,
             offsetLg: l,
@@ -20446,26 +20773,26 @@
             span: u,
             xs: d,
             sm: p,
             md: f,
             lg: m,
             xl: b
         }) => ({
-            root: Zx({
+            root: wS({
                 boxSizing: "border-box",
                 flexGrow: r ? 1 : 0,
                 padding: e.fn.size({
                     size: t,
                     sizes: e.spacing
                 }) / 2,
-                marginLeft: Xx(n, c),
-                flexBasis: Kx(u, c),
+                marginLeft: SS(n, c),
+                flexBasis: xS(u, c),
                 flexShrink: 0,
-                maxWidth: r ? "unset" : Kx(u, c)
-            }, Jx({
+                maxWidth: r ? "unset" : xS(u, c)
+            }, kS({
                 sizes: {
                     xs: d,
                     sm: p,
                     md: f,
                     lg: m,
                     xl: b
                 },
@@ -20477,26 +20804,26 @@
                     xl: s
                 },
                 theme: e,
                 columns: c,
                 grow: r
             }))
         })),
-        eS = Object.defineProperty,
-        tS = Object.getOwnPropertySymbols,
-        rS = Object.prototype.hasOwnProperty,
-        nS = Object.prototype.propertyIsEnumerable,
-        aS = (e, t, r) => t in e ? eS(e, t, {
+        jS = Object.defineProperty,
+        PS = Object.getOwnPropertySymbols,
+        zS = Object.prototype.hasOwnProperty,
+        CS = Object.prototype.propertyIsEnumerable,
+        NS = (e, t, r) => t in e ? jS(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
 
-    function oS(e) {
+    function TS(e) {
         var t = e,
             {
                 children: r,
                 span: n,
                 offset: o = 0,
                 offsetXs: i = 0,
                 offsetSm: l = 0,
@@ -20511,27 +20838,27 @@
                 className: g,
                 classNames: y,
                 styles: h,
                 id: v
             } = t,
             O = ((e, t) => {
                 var r = {};
-                for (var n in e) rS.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                if (null != e && tS)
-                    for (var n of tS(e)) t.indexOf(n) < 0 && nS.call(e, n) && (r[n] = e[n]);
+                for (var n in e) zS.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                if (null != e && PS)
+                    for (var n of PS(e)) t.indexOf(n) < 0 && CS.call(e, n) && (r[n] = e[n]);
                 return r
             })(t, ["children", "span", "offset", "offsetXs", "offsetSm", "offsetMd", "offsetLg", "offsetXl", "xs", "sm", "md", "lg", "xl", "className", "classNames", "styles", "id"]);
         const {
             columns: w,
             gutter: x,
             grow: S
-        } = Hx("Grid.Col"), k = n || w, {
+        } = bS("Grid.Col"), k = n || w, {
             classes: E,
             cx: j
-        } = Qx({
+        } = ES({
             gutter: x,
             offset: o,
             offsetXs: i,
             offsetSm: l,
             offsetMd: s,
             offsetLg: c,
             offsetXl: u,
@@ -20547,24 +20874,24 @@
             classNames: y,
             styles: h,
             name: "Col"
         });
         return ! function(e) {
             return "number" == typeof e && e > 0 && e % 1 == 0
         }(k) || k > w ? null : a.a.createElement(Cn, ((e, t) => {
-            for (var r in t || (t = {})) rS.call(t, r) && aS(e, r, t[r]);
-            if (tS)
-                for (var r of tS(t)) nS.call(t, r) && aS(e, r, t[r]);
+            for (var r in t || (t = {})) zS.call(t, r) && NS(e, r, t[r]);
+            if (PS)
+                for (var r of PS(t)) CS.call(t, r) && NS(e, r, t[r]);
             return e
         })({
             className: j(E.root, g)
         }, O), r)
     }
-    oS.displayName = "@mantine/core/Col";
-    var iS = Er((e, {
+    TS.displayName = "@mantine/core/Col";
+    var DS = Er((e, {
             justify: t,
             align: r,
             gutter: n
         }) => ({
             root: {
                 margin: -e.fn.size({
                     size: n,
@@ -20572,98 +20899,98 @@
                 }) / 2,
                 display: "flex",
                 flexWrap: "wrap",
                 justifyContent: t,
                 alignItems: r
             }
         })),
-        lS = Object.defineProperty,
-        sS = Object.getOwnPropertySymbols,
-        cS = Object.prototype.hasOwnProperty,
-        uS = Object.prototype.propertyIsEnumerable,
-        dS = (e, t, r) => t in e ? lS(e, t, {
+        IS = Object.defineProperty,
+        RS = Object.getOwnPropertySymbols,
+        _S = Object.prototype.hasOwnProperty,
+        LS = Object.prototype.propertyIsEnumerable,
+        AS = (e, t, r) => t in e ? IS(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const pS = {
+    const MS = {
             gutter: "md",
             justify: "flex-start",
             align: "stretch",
             columns: 12
         },
-        fS = Object(n.forwardRef)((e, t) => {
-            const r = ir("Grid", pS, e),
+        FS = Object(n.forwardRef)((e, t) => {
+            const r = ir("Grid", MS, e),
                 {
                     gutter: n,
                     children: o,
                     grow: i,
                     justify: l,
                     align: s,
                     columns: c,
                     className: u,
                     classNames: d,
                     styles: p,
                     id: f
                 } = r,
                 m = ((e, t) => {
                     var r = {};
-                    for (var n in e) cS.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && sS)
-                        for (var n of sS(e)) t.indexOf(n) < 0 && uS.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) _S.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && RS)
+                        for (var n of RS(e)) t.indexOf(n) < 0 && LS.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["gutter", "children", "grow", "justify", "align", "columns", "className", "classNames", "styles", "id"]),
                 {
                     classes: b,
                     cx: g
-                } = iS({
+                } = DS({
                     gutter: n,
                     justify: l,
                     align: s
                 }, {
                     classNames: d,
                     styles: p,
                     name: "Grid"
                 });
-            return a.a.createElement(Wx, {
+            return a.a.createElement(mS, {
                 value: {
                     gutter: n,
                     grow: i,
                     columns: c
                 }
             }, a.a.createElement(Cn, ((e, t) => {
-                for (var r in t || (t = {})) cS.call(t, r) && dS(e, r, t[r]);
-                if (sS)
-                    for (var r of sS(t)) uS.call(t, r) && dS(e, r, t[r]);
+                for (var r in t || (t = {})) _S.call(t, r) && AS(e, r, t[r]);
+                if (RS)
+                    for (var r of RS(t)) LS.call(t, r) && AS(e, r, t[r]);
                 return e
             })({
                 className: g(b.root, u),
                 ref: t
             }, m), o))
         });
 
-    function mS() {
-        return (mS = Object.assign || function(e) {
+    function $S() {
+        return ($S = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    fS.Col = oS, fS.displayName = "@mantine/core/Grid";
-    var bS = function(e) {
+    FS.Col = TS, FS.displayName = "@mantine/core/Grid";
+    var BS = function(e) {
         var t = e.class_name,
             r = e.children;
-        return a.a.createElement(fS.Col, mS({}, G(["children", "class_name"], e), {
+        return a.a.createElement(FS.Col, $S({}, G(["children", "class_name"], e), {
             className: t
         }), r)
     };
-    bS.displayName = "Col", bS.defaultProps = {}, bS.propTypes = {
+    BS.displayName = "Col", BS.defaultProps = {}, BS.propTypes = {
         children: i.a.node,
         class_name: i.a.string,
         gutter: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         id: i.a.string,
         offset: i.a.number,
         offsetXs: i.a.number,
         offsetSm: i.a.number,
@@ -20674,95 +21001,95 @@
         style: i.a.object,
         xs: i.a.number,
         sm: i.a.number,
         md: i.a.number,
         lg: i.a.number,
         xl: i.a.number
     };
-    var gS = bS;
+    var WS = BS;
 
-    function yS() {
-        return (yS = Object.assign || function(e) {
+    function HS() {
+        return (HS = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    var hS = function(e) {
+    var VS = function(e) {
         var t = e.children,
             r = e.class_name;
-        return a.a.createElement(fS, yS({}, G(["setProps", "children", "class_name"], e), {
+        return a.a.createElement(FS, HS({}, G(["setProps", "children", "class_name"], e), {
             className: r
         }), t)
     };
-    hS.displayName = "Grid", hS.defaultProps = {}, hS.propTypes = {
+    VS.displayName = "Grid", VS.defaultProps = {}, VS.propTypes = {
         align: i.a.oneOf(["stretch", "center", "flex-end", "flex-start"]),
         children: i.a.node,
         class_name: i.a.string,
         columns: i.a.number,
         grow: i.a.bool,
         gutter: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         id: i.a.string,
         justify: i.a.oneOf(["space-between", "space-around", "center", "flex-end", "flex-start"]),
         style: i.a.object
     };
-    var vS = hS;
+    var qS = VS;
 
-    function OS() {
-        return (OS = Object.assign || function(e) {
+    function US() {
+        return (US = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    var wS = function(e) {
+    var GS = function(e) {
         var t = e.children,
             r = e.class_name;
-        return a.a.createElement(Ma, OS({}, G(["children", "setProps", "class_name"], e), {
+        return a.a.createElement(Ma, US({
             className: r
-        }), a.a.Children.map(t, (function(e, t) {
+        }, G(["setProps", "children", "class_name"], e)), a.a.Children.map(t, (function(e, t) {
             return a.a.createElement("div", {
                 key: t
             }, e)
         })))
     };
-    wS.displayName = "Group", wS.defaultProps = {}, wS.propTypes = {
+    GS.displayName = "Group", GS.defaultProps = {}, GS.propTypes = {
         align: i.a.oneOf(["stretch", "center", "flex-end", "flex-start"]),
         children: i.a.node,
         class_name: i.a.string,
         direction: i.a.oneOf(["row", "column"]),
         grow: i.a.bool,
         id: i.a.string,
         noWrap: i.a.bool,
         position: i.a.oneOf(["right", "center", "left", "apart"]),
         spacing: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         style: i.a.object
     };
-    var xS = wS;
+    var YS = GS;
 
-    function SS() {
-        return (SS = Object.assign || function(e) {
+    function ZS() {
+        return (ZS = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    var kS = function(e) {
+    var KS = function(e) {
         var t = e.class_name;
-        return a.a.createElement(jo, SS({}, G(["setProps", "children", "class_name"], e), {
+        return a.a.createElement(jo, ZS({}, G(["setProps", "children", "class_name"], e), {
             className: t
         }), e.children)
     };
-    kS.displayName = "Text", kS.defaultProps = {}, kS.propTypes = {
+    KS.displayName = "Text", KS.defaultProps = {}, KS.propTypes = {
         align: i.a.oneOf(["left", "right", "center"]),
         children: i.a.node,
         class_name: i.a.string,
         color: i.a.oneOf(["dark", "gray", "red", "pink", "grape", "violet", "indigo", "blue", "cyan", "teal", "green", "lime", "yellow", "orange", "dimmed"]),
         gradient: i.a.exact({
             from: i.a.string.isRequired,
             to: i.a.string.isRequired,
@@ -20775,141 +21102,141 @@
         size: i.a.oneOf(["xs", "sm", "md", "lg", "xl"]),
         style: i.a.object,
         transform: i.a.oneOf(["capitalize", "uppercase", "lowercase"]),
         underline: i.a.bool,
         variant: i.a.oneOf(["link", "gradient", "text"]),
         weight: i.a.oneOfType([i.a.oneOf(["normal", "bold", "bolder", "lighter", "initial", "inherit"]), i.a.number])
     };
-    var ES = kS,
-        jS = Object.defineProperty,
-        PS = Object.defineProperties,
-        zS = Object.getOwnPropertyDescriptors,
-        CS = Object.getOwnPropertySymbols,
-        NS = Object.prototype.hasOwnProperty,
-        TS = Object.prototype.propertyIsEnumerable,
-        DS = (e, t, r) => t in e ? jS(e, t, {
+    var XS = KS,
+        JS = Object.defineProperty,
+        QS = Object.defineProperties,
+        ek = Object.getOwnPropertyDescriptors,
+        tk = Object.getOwnPropertySymbols,
+        rk = Object.prototype.hasOwnProperty,
+        nk = Object.prototype.propertyIsEnumerable,
+        ak = (e, t, r) => t in e ? JS(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        IS = (e, t) => {
-            for (var r in t || (t = {})) NS.call(t, r) && DS(e, r, t[r]);
-            if (CS)
-                for (var r of CS(t)) TS.call(t, r) && DS(e, r, t[r]);
+        ok = (e, t) => {
+            for (var r in t || (t = {})) rk.call(t, r) && ak(e, r, t[r]);
+            if (tk)
+                for (var r of tk(t)) nk.call(t, r) && ak(e, r, t[r]);
             return e
         },
-        RS = Er((e, {
+        ik = Er((e, {
             element: t,
             align: r
         }) => {
             return {
-                root: (n = IS({}, e.fn.fontStyles()), a = {
+                root: (n = ok({}, e.fn.fontStyles()), a = {
                     fontFamily: e.headings.fontFamily,
                     fontWeight: e.headings.fontWeight,
                     fontSize: e.headings.sizes[t].fontSize,
                     lineHeight: e.headings.sizes[t].lineHeight,
                     margin: 0,
                     color: "inherit",
                     textAlign: r
-                }, PS(n, zS(a)))
+                }, QS(n, ek(a)))
             };
             var n, a
         }),
-        _S = Object.defineProperty,
-        LS = Object.getOwnPropertySymbols,
-        AS = Object.prototype.hasOwnProperty,
-        MS = Object.prototype.propertyIsEnumerable,
-        FS = (e, t, r) => t in e ? _S(e, t, {
+        lk = Object.defineProperty,
+        sk = Object.getOwnPropertySymbols,
+        ck = Object.prototype.hasOwnProperty,
+        uk = Object.prototype.propertyIsEnumerable,
+        dk = (e, t, r) => t in e ? lk(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const $S = {
+    const pk = {
             order: 1
         },
-        BS = Object(n.forwardRef)((e, t) => {
-            const r = ir("Title", $S, e),
+        fk = Object(n.forwardRef)((e, t) => {
+            const r = ir("Title", pk, e),
                 {
                     className: n,
                     order: o,
                     children: i,
                     align: l
                 } = r,
                 s = ((e, t) => {
                     var r = {};
-                    for (var n in e) AS.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && LS)
-                        for (var n of LS(e)) t.indexOf(n) < 0 && MS.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) ck.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && sk)
+                        for (var n of sk(e)) t.indexOf(n) < 0 && uk.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["className", "order", "children", "align"]),
                 {
                     classes: c,
                     cx: u
-                } = RS({
+                } = ik({
                     element: "h" + o,
                     align: l
                 }, {
                     name: "Title"
                 });
             return [1, 2, 3, 4, 5, 6].includes(o) ? a.a.createElement(Cn, ((e, t) => {
-                for (var r in t || (t = {})) AS.call(t, r) && FS(e, r, t[r]);
-                if (LS)
-                    for (var r of LS(t)) MS.call(t, r) && FS(e, r, t[r]);
+                for (var r in t || (t = {})) ck.call(t, r) && dk(e, r, t[r]);
+                if (sk)
+                    for (var r of sk(t)) uk.call(t, r) && dk(e, r, t[r]);
                 return e
             })({
                 component: "h" + o,
                 ref: t,
                 className: u(c.root, n)
             }, s), i) : null
         });
 
-    function WS() {
-        return (WS = Object.assign || function(e) {
+    function mk() {
+        return (mk = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    BS.displayName = "@mantine/core/Title";
-    var HS = function(e) {
+    fk.displayName = "@mantine/core/Title";
+    var bk = function(e) {
         var t = e.class_name;
-        return a.a.createElement(BS, WS({}, G(["setProps", "children", "class_name"], e), {
+        return a.a.createElement(fk, mk({}, G(["setProps", "children", "class_name"], e), {
             className: t
         }), e.children)
     };
-    HS.displayName = "Title", HS.defaultProps = {}, HS.propTypes = {
+    bk.displayName = "Title", bk.defaultProps = {}, bk.propTypes = {
         align: i.a.oneOf(["left", "right", "center", "justify"]),
         children: i.a.string,
         class_name: i.a.string,
         id: i.a.string,
         order: i.a.number,
         style: i.a.object
     };
-    var VS = HS;
-    var qS = Object.defineProperty,
-        US = Object.getOwnPropertySymbols,
-        GS = Object.prototype.hasOwnProperty,
-        YS = Object.prototype.propertyIsEnumerable,
-        ZS = (e, t, r) => t in e ? qS(e, t, {
+    var gk = bk;
+    var yk = Object.defineProperty,
+        hk = Object.getOwnPropertySymbols,
+        vk = Object.prototype.hasOwnProperty,
+        Ok = Object.prototype.propertyIsEnumerable,
+        wk = (e, t, r) => t in e ? yk(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        KS = (e, t) => {
-            for (var r in t || (t = {})) GS.call(t, r) && ZS(e, r, t[r]);
-            if (US)
-                for (var r of US(t)) YS.call(t, r) && ZS(e, r, t[r]);
+        xk = (e, t) => {
+            for (var r in t || (t = {})) vk.call(t, r) && wk(e, r, t[r]);
+            if (hk)
+                for (var r of hk(t)) Ok.call(t, r) && wk(e, r, t[r]);
             return e
         },
-        XS = Er((e, {
+        Sk = Er((e, {
             spacing: t,
             breakpoints: r,
             cols: n
         }) => {
             const a = function(e, t) {
                 if (0 === t.length) return t;
                 const r = "maxWidth" in t[0] ? "maxWidth" : "minWidth",
@@ -20928,224 +21255,224 @@
                     gap: e.fn.size({
                         size: n.spacing || t,
                         sizes: e.spacing
                     })
                 }, r
             }, {});
             return {
-                root: KS({
+                root: xk({
                     boxSizing: "border-box",
                     display: "grid",
                     gridTemplateColumns: `repeat(${n}, minmax(0, 1fr))`,
                     gap: e.fn.size({
                         size: t,
                         sizes: e.spacing
                     })
                 }, a)
             }
         }),
-        JS = Object.defineProperty,
-        QS = Object.getOwnPropertySymbols,
-        ek = Object.prototype.hasOwnProperty,
-        tk = Object.prototype.propertyIsEnumerable,
-        rk = (e, t, r) => t in e ? JS(e, t, {
+        kk = Object.defineProperty,
+        Ek = Object.getOwnPropertySymbols,
+        jk = Object.prototype.hasOwnProperty,
+        Pk = Object.prototype.propertyIsEnumerable,
+        zk = (e, t, r) => t in e ? kk(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const nk = {
+    const Ck = {
             breakpoints: [],
             cols: 1,
             spacing: "md"
         },
-        ak = Object(n.forwardRef)((e, t) => {
-            const r = ir("SimpleGrid", nk, e),
+        Nk = Object(n.forwardRef)((e, t) => {
+            const r = ir("SimpleGrid", Ck, e),
                 {
                     className: n,
                     breakpoints: o,
                     cols: i,
                     spacing: l,
                     children: s,
                     classNames: c,
                     styles: u
                 } = r,
                 d = ((e, t) => {
                     var r = {};
-                    for (var n in e) ek.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && QS)
-                        for (var n of QS(e)) t.indexOf(n) < 0 && tk.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) jk.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && Ek)
+                        for (var n of Ek(e)) t.indexOf(n) < 0 && Pk.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["className", "breakpoints", "cols", "spacing", "children", "classNames", "styles"]),
                 {
                     classes: p,
                     cx: f
-                } = XS({
+                } = Sk({
                     breakpoints: o,
                     cols: i,
                     spacing: l
                 }, {
                     classNames: c,
                     styles: u,
                     name: "SimpleGrid"
                 });
             return a.a.createElement(Cn, ((e, t) => {
-                for (var r in t || (t = {})) ek.call(t, r) && rk(e, r, t[r]);
-                if (QS)
-                    for (var r of QS(t)) tk.call(t, r) && rk(e, r, t[r]);
+                for (var r in t || (t = {})) jk.call(t, r) && zk(e, r, t[r]);
+                if (Ek)
+                    for (var r of Ek(t)) Pk.call(t, r) && zk(e, r, t[r]);
                 return e
             })({
                 className: f(p.root, n),
                 ref: t
             }, d), s)
         });
 
-    function ok() {
-        return (ok = Object.assign || function(e) {
+    function Tk() {
+        return (Tk = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    ak.displayName = "@mantine/core/SimpleGrid";
-    var ik = function(e) {
+    Nk.displayName = "@mantine/core/SimpleGrid";
+    var Dk = function(e) {
         var t = e.class_name;
-        return a.a.createElement(ak, ok({}, G(["setProps", "children", "class_name"], e), {
+        return a.a.createElement(Nk, Tk({}, G(["setProps", "children", "class_name"], e), {
             className: t
         }), e.children)
     };
-    ik.displayName = "SimpleGrid", ik.defaultProps = {}, ik.propTypes = {
+    Dk.displayName = "SimpleGrid", Dk.defaultProps = {}, Dk.propTypes = {
         breakpoints: i.a.arrayOf(i.a.exact({
             maxWidth: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
             cols: i.a.number.isRequired,
             spacing: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number])
         })),
         children: i.a.node,
         class_name: i.a.string,
         cols: i.a.number.isRequired,
         id: i.a.string,
         spacing: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         style: i.a.object
     };
-    var lk = ik,
-        sk = Object.defineProperty,
-        ck = Object.getOwnPropertySymbols,
-        uk = Object.prototype.hasOwnProperty,
-        dk = Object.prototype.propertyIsEnumerable,
-        pk = (e, t, r) => t in e ? sk(e, t, {
+    var Ik = Dk,
+        Rk = Object.defineProperty,
+        _k = Object.getOwnPropertySymbols,
+        Lk = Object.prototype.hasOwnProperty,
+        Ak = Object.prototype.propertyIsEnumerable,
+        Mk = (e, t, r) => t in e ? Rk(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        fk = (e, t) => {
-            for (var r in t || (t = {})) uk.call(t, r) && pk(e, r, t[r]);
-            if (ck)
-                for (var r of ck(t)) dk.call(t, r) && pk(e, r, t[r]);
+        Fk = (e, t) => {
+            for (var r in t || (t = {})) Lk.call(t, r) && Mk(e, r, t[r]);
+            if (_k)
+                for (var r of _k(t)) Ak.call(t, r) && Mk(e, r, t[r]);
             return e
         };
-    const mk = {
+    const $k = {
             position: {
                 bottom: 0,
                 right: 0
             },
             zIndex: ac("modal")
         },
-        bk = Object(n.forwardRef)((e, t) => {
-            const r = ir("Affix", mk, e),
+        Bk = Object(n.forwardRef)((e, t) => {
+            const r = ir("Affix", $k, e),
                 {
                     target: n,
                     position: o,
                     zIndex: i,
                     sx: l
                 } = r,
                 s = ((e, t) => {
                     var r = {};
-                    for (var n in e) uk.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && ck)
-                        for (var n of ck(e)) t.indexOf(n) < 0 && dk.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) Lk.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && _k)
+                        for (var n of _k(e)) t.indexOf(n) < 0 && Ak.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["target", "position", "zIndex", "sx"]);
             return a.a.createElement(Fu, {
                 zIndex: i,
                 target: n
-            }, a.a.createElement(Cn, fk({
-                sx: [fk({
+            }, a.a.createElement(Cn, Fk({
+                sx: [Fk({
                     position: "fixed"
                 }, o), ...Array.isArray(l) ? l : [l]],
                 ref: t
             }, s)))
         });
 
-    function gk() {
-        return (gk = Object.assign || function(e) {
+    function Wk() {
+        return (Wk = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    bk.displayName = "@mantine/core/Affix";
-    var yk = function(e) {
+    Bk.displayName = "@mantine/core/Affix";
+    var Hk = function(e) {
         var t = {
             props: e
         };
-        return a.a.createElement(bk, gk({}, G(["setProps", "children", "class_name"], e), {
+        return a.a.createElement(Bk, Wk({}, G(["setProps", "children", "class_name"], e), {
             className: t
         }), e.children)
     };
-    yk.displayName = "Affix", yk.defaultProps = {}, yk.propTypes = {
+    Hk.displayName = "Affix", Hk.defaultProps = {}, Hk.propTypes = {
         children: i.a.node,
         class_name: i.a.string,
         id: i.a.string,
         position: i.a.exact({
             top: i.a.oneOfType([i.a.number, i.a.string]),
             left: i.a.oneOfType([i.a.number, i.a.string]),
             bottom: i.a.oneOfType([i.a.number, i.a.string]),
             right: i.a.oneOfType([i.a.number, i.a.string])
         }),
         style: i.a.object,
         zIndex: i.a.string
     };
-    var hk = yk,
-        vk = Object.defineProperty,
-        Ok = Object.getOwnPropertySymbols,
-        wk = Object.prototype.hasOwnProperty,
-        xk = Object.prototype.propertyIsEnumerable,
-        Sk = (e, t, r) => t in e ? vk(e, t, {
+    var Vk = Hk,
+        qk = Object.defineProperty,
+        Uk = Object.getOwnPropertySymbols,
+        Gk = Object.prototype.hasOwnProperty,
+        Yk = Object.prototype.propertyIsEnumerable,
+        Zk = (e, t, r) => t in e ? qk(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const kk = {
+    const Kk = {
             w: 0,
             h: 0
         },
-        Ek = Object(n.forwardRef)((e, t) => {
-            const r = ir("Space", kk, e),
+        Xk = Object(n.forwardRef)((e, t) => {
+            const r = ir("Space", Kk, e),
                 {
                     w: n,
                     h: o,
                     sx: i
                 } = r,
                 l = ((e, t) => {
                     var r = {};
-                    for (var n in e) wk.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && Ok)
-                        for (var n of Ok(e)) t.indexOf(n) < 0 && xk.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) Gk.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && Uk)
+                        for (var n of Uk(e)) t.indexOf(n) < 0 && Yk.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["w", "h", "sx"]);
             return a.a.createElement(Cn, ((e, t) => {
-                for (var r in t || (t = {})) wk.call(t, r) && Sk(e, r, t[r]);
-                if (Ok)
-                    for (var r of Ok(t)) xk.call(t, r) && Sk(e, r, t[r]);
+                for (var r in t || (t = {})) Gk.call(t, r) && Zk(e, r, t[r]);
+                if (Uk)
+                    for (var r of Uk(t)) Yk.call(t, r) && Zk(e, r, t[r]);
                 return e
             })({
                 ref: t,
                 sx: [e => {
                     const t = e.fn.size({
                             size: n,
                             sizes: e.spacing
@@ -21160,126 +21487,126 @@
                         minWidth: t,
                         minHeight: r
                     }
                 }, ...Array.isArray(i) ? i : [i]]
             }, l))
         });
 
-    function jk() {
-        return (jk = Object.assign || function(e) {
+    function Jk() {
+        return (Jk = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    Ek.displayName = "@mantine/core/Space";
-    var Pk = function(e) {
+    Xk.displayName = "@mantine/core/Space";
+    var Qk = function(e) {
         var t = e.class_name;
-        return a.a.createElement(Ek, jk({}, G(["setProps", "class_name"], e), {
+        return a.a.createElement(Xk, Jk({}, G(["setProps", "class_name"], e), {
             className: t
         }))
     };
-    Pk.displayName = "Space", Pk.defaultProps = {}, Pk.propTypes = {
+    Qk.displayName = "Space", Qk.defaultProps = {}, Qk.propTypes = {
         class_name: i.a.string,
         h: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         id: i.a.string,
         style: i.a.object,
         w: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number])
     };
-    var zk = Pk,
-        Ck = Object.defineProperty,
-        Nk = Object.defineProperties,
-        Tk = Object.getOwnPropertyDescriptors,
-        Dk = Object.getOwnPropertySymbols,
-        Ik = Object.prototype.hasOwnProperty,
-        Rk = Object.prototype.propertyIsEnumerable,
-        _k = (e, t, r) => t in e ? Ck(e, t, {
+    var eE = Qk,
+        tE = Object.defineProperty,
+        rE = Object.defineProperties,
+        nE = Object.getOwnPropertyDescriptors,
+        aE = Object.getOwnPropertySymbols,
+        oE = Object.prototype.hasOwnProperty,
+        iE = Object.prototype.propertyIsEnumerable,
+        lE = (e, t, r) => t in e ? tE(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        Lk = (e, t) => {
-            for (var r in t || (t = {})) Ik.call(t, r) && _k(e, r, t[r]);
-            if (Dk)
-                for (var r of Dk(t)) Rk.call(t, r) && _k(e, r, t[r]);
+        sE = (e, t) => {
+            for (var r in t || (t = {})) oE.call(t, r) && lE(e, r, t[r]);
+            if (aE)
+                for (var r of aE(t)) iE.call(t, r) && lE(e, r, t[r]);
             return e
         };
-    const Ak = {
+    const cE = {
             xs: 24,
             sm: 28,
             md: 32,
             lg: 36,
             xl: 40
         },
-        Mk = {
+        uE = {
             xs: 10,
             sm: 12,
             md: 14,
             lg: 16,
             xl: 18
         },
-        Fk = {
+        dE = {
             xs: 16,
             sm: 20,
             md: 24,
             lg: 28,
             xl: 32
         },
-        $k = {
+        pE = {
             xs: 7.5,
             sm: 10,
             md: 11.5,
             lg: 13,
             xl: 15
         };
-    var Bk = Er((e, {
+    var fE = Er((e, {
             radius: t,
             size: r,
             color: n
         }, a) => {
             return {
                 root: {},
-                label: (o = Lk({
+                label: (o = sE({
                     ref: a("label")
                 }, e.fn.fontStyles()), i = {
                     boxSizing: "border-box",
                     color: "dark" === e.colorScheme ? e.colors.dark[0] : e.black,
                     display: "inline-block",
                     alignItems: "center",
                     userSelect: "none",
                     border: "1px solid " + ("dark" === e.colorScheme ? e.colors.dark[3] : e.colors.gray[4]),
                     borderRadius: e.fn.radius(t),
                     height: e.fn.size({
                         size: r,
-                        sizes: Ak
+                        sizes: cE
                     }),
                     fontSize: e.fn.size({
                         size: r,
                         sizes: e.fontSizes
                     }),
                     lineHeight: e.fn.size({
                         size: r,
-                        sizes: Ak
+                        sizes: cE
                     }) - 2 + "px",
                     paddingLeft: e.fn.size({
                         size: r,
-                        sizes: Fk
+                        sizes: dE
                     }),
                     paddingRight: e.fn.size({
                         size: r,
-                        sizes: Fk
+                        sizes: dE
                     }),
                     cursor: "pointer",
                     whiteSpace: "nowrap",
                     transition: "background-color 100ms ease",
                     WebkitTapHighlightColor: "transparent"
-                }, Nk(o, Tk(i))),
+                }, rE(o, nE(i))),
                 outline: {
                     ref: a("outline"),
                     backgroundColor: "dark" === e.colorScheme ? e.colors.dark[7] : e.white,
                     "&:hover": {
                         backgroundColor: "dark" === e.colorScheme ? e.colors.dark[8] : e.colors.gray[0]
                     }
                 },
@@ -21292,29 +21619,29 @@
                     }
                 },
                 iconWrapper: {
                     ref: a("iconWrapper"),
                     color: e.fn.themeColor(n, 6),
                     width: e.fn.size({
                         size: r,
-                        sizes: Mk
+                        sizes: uE
                     }) + e.fn.size({
                         size: r,
                         sizes: e.spacing
                     }) / 1.5,
                     maxWidth: e.fn.size({
                         size: r,
-                        sizes: Mk
+                        sizes: uE
                     }) + e.fn.size({
                         size: r,
                         sizes: e.spacing
                     }) / 1.5,
                     height: e.fn.size({
                         size: r,
-                        sizes: Mk
+                        sizes: uE
                     }),
                     display: "inline-block",
                     verticalAlign: "middle",
                     overflow: "hidden"
                 },
                 disabled: {
                     backgroundColor: ("dark" === e.colorScheme ? e.colors.dark[5] : e.colors.gray[1]) + " !important",
@@ -21327,19 +21654,19 @@
                     ["& ." + a("iconWrapper")]: {
                         color: "dark" === e.colorScheme ? e.colors.dark[3] : e.colors.gray[5]
                     }
                 },
                 checked: {
                     paddingLeft: e.fn.size({
                         size: r,
-                        sizes: $k
+                        sizes: pE
                     }),
                     paddingRight: e.fn.size({
                         size: r,
-                        sizes: $k
+                        sizes: pE
                     }),
                     ["&." + a("outline")]: {
                         border: "1px solid " + e.fn.themeColor(n, 6)
                     },
                     ["&." + a("filled")]: {
                         "&, &:hover": {
                             backgroundColor: "dark" === e.colorScheme ? dr({
@@ -21349,19 +21676,19 @@
                             }).background : e.fn.themeColor(n, 1)
                         }
                     }
                 },
                 checkIcon: {
                     width: e.fn.size({
                         size: r,
-                        sizes: Mk
+                        sizes: uE
                     }),
                     height: e.fn.size({
                         size: r,
-                        sizes: Mk
+                        sizes: uE
                     }) / 1.1,
                     display: "block"
                 },
                 input: {
                     width: 0,
                     height: 0,
                     padding: 0,
@@ -21379,38 +21706,38 @@
                             }
                         }
                     }
                 }
             };
             var o, i
         }),
-        Wk = Object.defineProperty,
-        Hk = Object.getOwnPropertySymbols,
-        Vk = Object.prototype.hasOwnProperty,
-        qk = Object.prototype.propertyIsEnumerable,
-        Uk = (e, t, r) => t in e ? Wk(e, t, {
+        mE = Object.defineProperty,
+        bE = Object.getOwnPropertySymbols,
+        gE = Object.prototype.hasOwnProperty,
+        yE = Object.prototype.propertyIsEnumerable,
+        hE = (e, t, r) => t in e ? mE(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        Gk = (e, t) => {
-            for (var r in t || (t = {})) Vk.call(t, r) && Uk(e, r, t[r]);
-            if (Hk)
-                for (var r of Hk(t)) qk.call(t, r) && Uk(e, r, t[r]);
+        vE = (e, t) => {
+            for (var r in t || (t = {})) gE.call(t, r) && hE(e, r, t[r]);
+            if (bE)
+                for (var r of bE(t)) yE.call(t, r) && hE(e, r, t[r]);
             return e
         };
-    const Yk = {
+    const OE = {
             type: "checkbox",
             size: "sm",
             radius: "xl",
             __staticSelector: "Chip"
         },
-        Zk = Object(n.forwardRef)((e, t) => {
-            const r = ir("Chip", Yk, e),
+        wE = Object(n.forwardRef)((e, t) => {
+            const r = ir("Chip", OE, e),
                 {
                     radius: n,
                     type: o,
                     size: i,
                     variant: l,
                     disabled: s,
                     __staticSelector: c,
@@ -21425,29 +21752,29 @@
                     defaultChecked: h,
                     onChange: v,
                     sx: O,
                     wrapperProps: w
                 } = r,
                 x = ((e, t) => {
                     var r = {};
-                    for (var n in e) Vk.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && Hk)
-                        for (var n of Hk(e)) t.indexOf(n) < 0 && qk.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) gE.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && bE)
+                        for (var n of bE(e)) t.indexOf(n) < 0 && yE.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["radius", "type", "size", "variant", "disabled", "__staticSelector", "id", "color", "children", "className", "classNames", "style", "styles", "checked", "defaultChecked", "onChange", "sx", "wrapperProps"]),
                 S = Ja(u),
                 {
                     systemStyles: k,
                     rest: E
                 } = gn(x),
                 {
                     classes: j,
                     cx: P,
                     theme: z
-                } = Bk({
+                } = fE({
                     radius: n,
                     size: i,
                     color: d
                 }, {
                     classNames: m,
                     styles: g,
                     name: c
@@ -21456,19 +21783,19 @@
                     value: y,
                     defaultValue: h,
                     finalValue: !1,
                     onChange: v,
                     rule: e => "boolean" == typeof e
                 }),
                 T = "dark" === z.colorScheme ? "filled" : "outline";
-            return a.a.createElement(Cn, Gk(Gk({
+            return a.a.createElement(Cn, vE(vE({
                 className: P(j.root, f),
                 style: b,
                 sx: O
-            }, k), w), a.a.createElement("input", Gk({
+            }, k), w), a.a.createElement("input", vE({
                 type: o,
                 className: j.input,
                 checked: C,
                 onChange: e => N(e.currentTarget.checked),
                 id: S,
                 disabled: s,
                 ref: t
@@ -21481,33 +21808,33 @@
             }, C && a.a.createElement("span", {
                 className: j.iconWrapper
             }, a.a.createElement(fh, {
                 indeterminate: !1,
                 className: j.checkIcon
             })), p))
         });
-    Zk.displayName = "@mantine/core/Chip";
-    var Kk = Object.defineProperty,
-        Xk = Object.getOwnPropertySymbols,
-        Jk = Object.prototype.hasOwnProperty,
-        Qk = Object.prototype.propertyIsEnumerable,
-        eE = (e, t, r) => t in e ? Kk(e, t, {
+    wE.displayName = "@mantine/core/Chip";
+    var xE = Object.defineProperty,
+        SE = Object.getOwnPropertySymbols,
+        kE = Object.prototype.hasOwnProperty,
+        EE = Object.prototype.propertyIsEnumerable,
+        jE = (e, t, r) => t in e ? xE(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const tE = {
+    const PE = {
         size: "sm",
         spacing: "xs",
         radius: "xl"
     };
 
-    function rE(e) {
-        const t = ir("Chips", tE, e),
+    function zE(e) {
+        const t = ir("Chips", PE, e),
             {
                 value: r,
                 defaultValue: n,
                 onChange: o,
                 color: i,
                 spacing: l,
                 radius: s,
@@ -21518,28 +21845,28 @@
                 children: f,
                 id: m,
                 classNames: b,
                 styles: g
             } = t,
             y = ((e, t) => {
                 var r = {};
-                for (var n in e) Jk.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                if (null != e && Xk)
-                    for (var n of Xk(e)) t.indexOf(n) < 0 && Qk.call(e, n) && (r[n] = e[n]);
+                for (var n in e) kE.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                if (null != e && SE)
+                    for (var n of SE(e)) t.indexOf(n) < 0 && EE.call(e, n) && (r[n] = e[n]);
                 return r
             })(t, ["value", "defaultValue", "onChange", "color", "spacing", "radius", "size", "name", "variant", "multiple", "children", "id", "classNames", "styles"]),
             h = Ja(m),
             [v, O] = la({
                 value: r,
                 defaultValue: n,
                 finalValue: p ? [] : null,
                 onChange: o,
                 rule: e => p ? Array.isArray(e) : "string" == typeof e
             }),
-            w = si(f, Zk).map((e, t) => a.a.cloneElement(e, {
+            w = si(f, wE).map((e, t) => a.a.cloneElement(e, {
                 variant: d,
                 radius: s,
                 color: i,
                 __staticSelector: "Chips",
                 classNames: b,
                 styles: g,
                 name: u,
@@ -21549,58 +21876,58 @@
                 checked: Array.isArray(v) ? v.includes(e.props.value) : e.props.value === v,
                 onChange: () => {
                     const t = e.props.value;
                     Array.isArray(v) ? O(v.includes(t) ? v.filter(e => e !== t) : [...v, t]) : O(t)
                 }
             }));
         return a.a.createElement(Ma, ((e, t) => {
-            for (var r in t || (t = {})) Jk.call(t, r) && eE(e, r, t[r]);
-            if (Xk)
-                for (var r of Xk(t)) Qk.call(t, r) && eE(e, r, t[r]);
+            for (var r in t || (t = {})) kE.call(t, r) && jE(e, r, t[r]);
+            if (SE)
+                for (var r of SE(t)) EE.call(t, r) && jE(e, r, t[r]);
             return e
         })({
             spacing: l,
             id: h
         }, y), w)
     }
 
-    function nE() {
-        return (nE = Object.assign || function(e) {
+    function CE() {
+        return (CE = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    rE.displayName = "@mantine/core/Chips";
-    var aE = function(e) {
+    zE.displayName = "@mantine/core/Chips";
+    var NE = function(e) {
         var t = e.setProps,
             r = e.data,
             n = e.class_name;
-        return a.a.createElement(rE, nE({
+        return a.a.createElement(zE, CE({
             onChange: function(e) {
                 t({
                     value: e
                 })
             }
         }, G(["setProps", "data", "class_name"], e), {
             className: n
         }), r.map((function(e, t) {
-            return a.a.createElement(Zk, {
+            return a.a.createElement(wE, {
                 disabled: e.disabled,
                 value: e.value,
                 key: t
             }, e.label)
         })))
     };
-    aE.displayName = "Chips", aE.defaultProps = {
+    NE.displayName = "Chips", NE.defaultProps = {
         persisted_props: ["value"],
         persistence_type: "local"
-    }, aE.propTypes = {
+    }, NE.propTypes = {
         align: i.a.oneOf(["stretch", "center", "flex-end", "flex-start"]),
         class_name: i.a.string,
         color: i.a.oneOf(["dark", "gray", "red", "pink", "grape", "violet", "indigo", "blue", "cyan", "teal", "green", "lime", "yellow", "orange"]),
         data: i.a.arrayOf(i.a.exact({
             label: i.a.string.isRequired,
             value: i.a.string.isRequired,
             disabled: i.a.bool
@@ -21618,34 +21945,34 @@
         setProps: i.a.func,
         size: i.a.oneOf(["xs", "sm", "md", "lg", "xl"]),
         spacing: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         style: i.a.object,
         value: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string)]),
         variant: i.a.oneOf(["outline", "filled"])
     };
-    var oE = aE,
-        iE = Object.defineProperty,
-        lE = Object.defineProperties,
-        sE = Object.getOwnPropertyDescriptors,
-        cE = Object.getOwnPropertySymbols,
-        uE = Object.prototype.hasOwnProperty,
-        dE = Object.prototype.propertyIsEnumerable,
-        pE = (e, t, r) => t in e ? iE(e, t, {
+    var TE = NE,
+        DE = Object.defineProperty,
+        IE = Object.defineProperties,
+        RE = Object.getOwnPropertyDescriptors,
+        _E = Object.getOwnPropertySymbols,
+        LE = Object.prototype.hasOwnProperty,
+        AE = Object.prototype.propertyIsEnumerable,
+        ME = (e, t, r) => t in e ? DE(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        fE = (e, t) => {
-            for (var r in t || (t = {})) uE.call(t, r) && pE(e, r, t[r]);
-            if (cE)
-                for (var r of cE(t)) dE.call(t, r) && pE(e, r, t[r]);
+        FE = (e, t) => {
+            for (var r in t || (t = {})) LE.call(t, r) && ME(e, r, t[r]);
+            if (_E)
+                for (var r of _E(t)) AE.call(t, r) && ME(e, r, t[r]);
             return e
         };
-    const mE = {
+    const $E = {
             xs: {
                 fontSize: 9,
                 height: 16
             },
             sm: {
                 fontSize: 10,
                 height: 18
@@ -21659,39 +21986,39 @@
                 height: 26
             },
             xl: {
                 fontSize: 16,
                 height: 32
             }
         },
-        bE = {
+        BE = {
             xs: 4,
             sm: 4,
             md: 6,
             lg: 8,
             xl: 10
         };
-    Object.keys(mE).reduce((e, t) => (e[t] = mE[t].height, e), {});
-    var gE = Er((e, {
+    Object.keys($E).reduce((e, t) => (e[t] = $E[t].height, e), {});
+    var WE = Er((e, {
             color: t,
             size: r,
             radius: n,
             gradientFrom: a,
             gradientTo: o,
             gradientDeg: i,
             fullWidth: l
         }) => {
             const s = e.fn.size({
                     size: r,
-                    sizes: bE
+                    sizes: BE
                 }),
                 {
                     fontSize: c,
                     height: u
-                } = r in mE ? mE[r] : mE.md,
+                } = r in $E ? $E[r] : $E.md,
                 d = dr({
                     color: t,
                     theme: e,
                     variant: "light"
                 }),
                 p = dr({
                     theme: e,
@@ -21720,15 +22047,15 @@
                     marginLeft: e.spacing.xs / 2
                 },
                 inner: {
                     whiteSpace: "nowrap",
                     overflow: "hidden",
                     textOverflow: "ellipsis"
                 },
-                root: (b = fE(fE({}, e.fn.focusStyles()), e.fn.fontStyles()), g = {
+                root: (b = FE(FE({}, e.fn.focusStyles()), e.fn.fontStyles()), g = {
                     fontSize: c,
                     height: u,
                     WebkitTapHighlightColor: "transparent",
                     lineHeight: u - 2 + "px",
                     textDecoration: "none",
                     padding: `0 ${e.fn.size({size:r,sizes:e.spacing})/1.5}px`,
                     boxSizing: "border-box",
@@ -21739,15 +22066,15 @@
                     textTransform: "uppercase",
                     borderRadius: e.fn.radius(n),
                     fontWeight: 700,
                     letterSpacing: .25,
                     cursor: "default",
                     textOverflow: "ellipsis",
                     overflow: "hidden"
-                }, lE(b, sE(g))),
+                }, IE(b, RE(g))),
                 light: {
                     backgroundColor: d.background,
                     color: d.color,
                     border: "1px solid transparent"
                 },
                 filled: {
                     backgroundColor: p.background,
@@ -21781,36 +22108,36 @@
                         backgroundColor: e.fn.themeColor(t, "dark" === e.colorScheme ? 4 : 6),
                         marginRight: s
                     }
                 }
             };
             var b, g
         }),
-        yE = Object.defineProperty,
-        hE = Object.getOwnPropertySymbols,
-        vE = Object.prototype.hasOwnProperty,
-        OE = Object.prototype.propertyIsEnumerable,
-        wE = (e, t, r) => t in e ? yE(e, t, {
+        HE = Object.defineProperty,
+        VE = Object.getOwnPropertySymbols,
+        qE = Object.prototype.hasOwnProperty,
+        UE = Object.prototype.propertyIsEnumerable,
+        GE = (e, t, r) => t in e ? HE(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const xE = {
+    const YE = {
             variant: "light",
             size: "md",
             radius: "xl",
             gradient: {
                 from: "blue",
                 to: "cyan",
                 deg: 45
             }
         },
-        SE = Object(n.forwardRef)((e, t) => {
-            const r = ir("Badge", xE, e),
+        ZE = Object(n.forwardRef)((e, t) => {
+            const r = ir("Badge", YE, e),
                 {
                     component: n,
                     className: o,
                     color: i,
                     variant: l,
                     fullWidth: s,
                     children: c,
@@ -21820,72 +22147,72 @@
                     radius: f,
                     gradient: m,
                     classNames: b,
                     styles: g
                 } = r,
                 y = ((e, t) => {
                     var r = {};
-                    for (var n in e) vE.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && hE)
-                        for (var n of hE(e)) t.indexOf(n) < 0 && OE.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) qE.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && VE)
+                        for (var n of VE(e)) t.indexOf(n) < 0 && UE.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["component", "className", "color", "variant", "fullWidth", "children", "size", "leftSection", "rightSection", "radius", "gradient", "classNames", "styles"]),
                 {
                     classes: h,
                     cx: v
-                } = gE({
+                } = WE({
                     size: u,
                     fullWidth: s,
                     color: i,
                     radius: f,
                     gradientFrom: m.from,
                     gradientTo: m.to,
                     gradientDeg: m.deg
                 }, {
                     classNames: b,
                     styles: g,
                     name: "Badge"
                 });
             return a.a.createElement(Cn, ((e, t) => {
-                for (var r in t || (t = {})) vE.call(t, r) && wE(e, r, t[r]);
-                if (hE)
-                    for (var r of hE(t)) OE.call(t, r) && wE(e, r, t[r]);
+                for (var r in t || (t = {})) qE.call(t, r) && GE(e, r, t[r]);
+                if (VE)
+                    for (var r of VE(t)) UE.call(t, r) && GE(e, r, t[r]);
                 return e
             })({
                 component: n || "div",
                 className: v(h[l], h.root, o),
                 ref: t
             }, y), d && a.a.createElement("span", {
                 className: h.leftSection
             }, d), a.a.createElement("span", {
                 className: h.inner
             }, c), p && a.a.createElement("span", {
                 className: h.rightSection
             }, p))
         });
 
-    function kE() {
-        return (kE = Object.assign || function(e) {
+    function KE() {
+        return (KE = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    SE.displayName = "@mantine/core/Badge";
-    var EE = function(e) {
+    ZE.displayName = "@mantine/core/Badge";
+    var XE = function(e) {
         var t = e.children,
             r = e.class_name,
             n = G(["setProps", "children", "class_name"], e);
-        return n = ta(n, ["leftSection", "rightSection"]), a.a.createElement(SE, kE({}, n, {
+        return n = ta(n, ["leftSection", "rightSection"]), a.a.createElement(ZE, KE({}, n, {
             className: r
         }), t)
     };
-    EE.displayName = "Badge", EE.defaultProps = {}, EE.propTypes = {
+    XE.displayName = "Badge", XE.defaultProps = {}, XE.propTypes = {
         children: i.a.string,
         class_name: i.a.string,
         color: i.a.oneOf(["dark", "gray", "red", "pink", "grape", "violet", "indigo", "blue", "cyan", "teal", "green", "lime", "yellow", "orange"]),
         fullWidth: i.a.bool,
         gradient: i.a.exact({
             from: i.a.string.isRequired,
             to: i.a.string.isRequired,
@@ -21895,91 +22222,91 @@
         id: i.a.string,
         radius: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         rightSection: i.a.any,
         size: i.a.oneOf(["xs", "sm", "md", "lg", "xl"]),
         style: i.a.object,
         variant: i.a.oneOf(["light", "filled", "outline", "dot", "gradient"])
     };
-    var jE = EE,
-        PE = Er(() => ({
+    var JE = XE,
+        QE = Er(() => ({
             root: {
                 backgroundColor: "transparent",
                 cursor: "pointer",
                 padding: 0,
                 border: 0
             }
         })),
-        zE = Object.defineProperty,
-        CE = Object.getOwnPropertySymbols,
-        NE = Object.prototype.hasOwnProperty,
-        TE = Object.prototype.propertyIsEnumerable,
-        DE = (e, t, r) => t in e ? zE(e, t, {
+        ej = Object.defineProperty,
+        tj = Object.getOwnPropertySymbols,
+        rj = Object.prototype.hasOwnProperty,
+        nj = Object.prototype.propertyIsEnumerable,
+        aj = (e, t, r) => t in e ? ej(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        IE = (e, t) => {
-            for (var r in t || (t = {})) NE.call(t, r) && DE(e, r, t[r]);
-            if (CE)
-                for (var r of CE(t)) TE.call(t, r) && DE(e, r, t[r]);
+        oj = (e, t) => {
+            for (var r in t || (t = {})) rj.call(t, r) && aj(e, r, t[r]);
+            if (tj)
+                for (var r of tj(t)) nj.call(t, r) && aj(e, r, t[r]);
             return e
         };
-    const RE = {},
-        _E = Object(n.forwardRef)((e, t) => {
-            const r = ir("Anchor", RE, e),
+    const ij = {},
+        lj = Object(n.forwardRef)((e, t) => {
+            const r = ir("Anchor", ij, e),
                 {
                     component: n,
                     className: o,
                     classNames: i,
                     styles: l
                 } = r,
                 s = ((e, t) => {
                     var r = {};
-                    for (var n in e) NE.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && CE)
-                        for (var n of CE(e)) t.indexOf(n) < 0 && TE.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) rj.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && tj)
+                        for (var n of tj(e)) t.indexOf(n) < 0 && nj.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["component", "className", "classNames", "styles"]),
                 {
                     classes: c,
                     cx: u
-                } = PE(null, {
+                } = QE(null, {
                     name: "Anchor",
                     classNames: i,
                     styles: l
                 }),
                 d = "button" === n ? {
                     type: "button"
                 } : null;
-            return a.a.createElement(jo, IE(IE({
+            return a.a.createElement(jo, oj(oj({
                 component: n || "a",
                 variant: "link",
                 ref: t,
                 className: u(c.root, o)
             }, d), s))
         });
 
-    function LE() {
-        return (LE = Object.assign || function(e) {
+    function sj() {
+        return (sj = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    _E.displayName = "@mantine/core/Anchor";
-    var AE = function(e) {
+    lj.displayName = "@mantine/core/Anchor";
+    var cj = function(e) {
         var t = e.class_name;
-        return a.a.createElement(_E, LE({}, G(["setProps", "children", "class_name"], e), {
+        return a.a.createElement(lj, sj({}, G(["setProps", "children", "class_name"], e), {
             className: t
         }), e.children)
     };
-    AE.displayName = "Anchor", AE.defaultProps = {}, AE.propTypes = {
+    cj.displayName = "Anchor", cj.defaultProps = {}, cj.propTypes = {
         align: i.a.oneOf(["left", "right", "center"]),
         children: i.a.string,
         class_name: i.a.string,
         color: i.a.oneOf(["dark", "gray", "red", "pink", "grape", "violet", "indigo", "blue", "cyan", "teal", "green", "lime", "yellow", "orange"]),
         gradient: i.a.exact({
             from: i.a.string.isRequired,
             to: i.a.string.isRequired,
@@ -21994,124 +22321,124 @@
         style: i.a.object,
         target: i.a.oneOf(["_blank", "_self"]),
         transform: i.a.oneOf(["capitalize", "uppercase", "lowercase"]),
         underline: i.a.bool,
         variant: i.a.oneOf(["link", "gradient", "text"]),
         weight: i.a.oneOfType([i.a.oneOf(["normal", "bold", "bolder", "lighter", "initial", "inherit"]), i.a.number])
     };
-    var ME = AE,
-        FE = Object.defineProperty,
-        $E = Object.getOwnPropertySymbols,
-        BE = Object.prototype.hasOwnProperty,
-        WE = Object.prototype.propertyIsEnumerable,
-        HE = (e, t, r) => t in e ? FE(e, t, {
+    var uj = cj,
+        dj = Object.defineProperty,
+        pj = Object.getOwnPropertySymbols,
+        fj = Object.prototype.hasOwnProperty,
+        mj = Object.prototype.propertyIsEnumerable,
+        bj = (e, t, r) => t in e ? dj(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
 
-    function VE(e) {
+    function gj(e) {
         return a.a.createElement("svg", ((e, t) => {
-            for (var r in t || (t = {})) BE.call(t, r) && HE(e, r, t[r]);
-            if ($E)
-                for (var r of $E(t)) WE.call(t, r) && HE(e, r, t[r]);
+            for (var r in t || (t = {})) fj.call(t, r) && bj(e, r, t[r]);
+            if (pj)
+                for (var r of pj(t)) mj.call(t, r) && bj(e, r, t[r]);
             return e
         })({
             width: "15",
             height: "15",
             viewBox: "0 0 15 15",
             fill: "none",
             xmlns: "http://www.w3.org/2000/svg"
         }, e), a.a.createElement("path", {
             d: "M2.5 1H12.5C13.3284 1 14 1.67157 14 2.5V12.5C14 13.3284 13.3284 14 12.5 14H2.5C1.67157 14 1 13.3284 1 12.5V2.5C1 1.67157 1.67157 1 2.5 1ZM2.5 2C2.22386 2 2 2.22386 2 2.5V8.3636L3.6818 6.6818C3.76809 6.59551 3.88572 6.54797 4.00774 6.55007C4.12975 6.55216 4.24568 6.60372 4.32895 6.69293L7.87355 10.4901L10.6818 7.6818C10.8575 7.50607 11.1425 7.50607 11.3182 7.6818L13 9.3636V2.5C13 2.22386 12.7761 2 12.5 2H2.5ZM2 12.5V9.6364L3.98887 7.64753L7.5311 11.4421L8.94113 13H2.5C2.22386 13 2 12.7761 2 12.5ZM12.5 13H10.155L8.48336 11.153L11 8.6364L13 10.6364V12.5C13 12.7761 12.7761 13 12.5 13ZM6.64922 5.5C6.64922 5.03013 7.03013 4.64922 7.5 4.64922C7.96987 4.64922 8.35078 5.03013 8.35078 5.5C8.35078 5.96987 7.96987 6.35078 7.5 6.35078C7.03013 6.35078 6.64922 5.96987 6.64922 5.5ZM7.5 3.74922C6.53307 3.74922 5.74922 4.53307 5.74922 5.5C5.74922 6.46693 6.53307 7.25078 7.5 7.25078C8.46693 7.25078 9.25078 6.46693 9.25078 5.5C9.25078 4.53307 8.46693 3.74922 7.5 3.74922Z",
             fill: "currentColor",
             fillRule: "evenodd",
             clipRule: "evenodd"
         }))
     }
-    var qE = Object.defineProperty,
-        UE = Object.defineProperties,
-        GE = Object.getOwnPropertyDescriptors,
-        YE = Object.getOwnPropertySymbols,
-        ZE = Object.prototype.hasOwnProperty,
-        KE = Object.prototype.propertyIsEnumerable,
-        XE = (e, t, r) => t in e ? qE(e, t, {
+    var yj = Object.defineProperty,
+        hj = Object.defineProperties,
+        vj = Object.getOwnPropertyDescriptors,
+        Oj = Object.getOwnPropertySymbols,
+        wj = Object.prototype.hasOwnProperty,
+        xj = Object.prototype.propertyIsEnumerable,
+        Sj = (e, t, r) => t in e ? yj(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        JE = (e, t) => {
-            for (var r in t || (t = {})) ZE.call(t, r) && XE(e, r, t[r]);
-            if (YE)
-                for (var r of YE(t)) KE.call(t, r) && XE(e, r, t[r]);
+        kj = (e, t) => {
+            for (var r in t || (t = {})) wj.call(t, r) && Sj(e, r, t[r]);
+            if (Oj)
+                for (var r of Oj(t)) xj.call(t, r) && Sj(e, r, t[r]);
             return e
         },
-        QE = (e, t) => UE(e, GE(t)),
-        ej = Er((e, {
+        Ej = (e, t) => hj(e, vj(t)),
+        jj = Er((e, {
             radius: t
         }) => ({
             root: {},
             imageWrapper: {
                 position: "relative"
             },
             figure: {
                 margin: 0
             },
-            image: QE(JE({}, e.fn.fontStyles()), {
+            image: Ej(kj({}, e.fn.fontStyles()), {
                 display: "block",
                 width: "100%",
                 height: "100%",
                 border: 0,
                 borderRadius: e.fn.size({
                     size: t,
                     sizes: e.radius
                 })
             }),
             caption: {
                 color: "dark" === e.colorScheme ? e.colors.dark[2] : e.colors.gray[7],
                 marginTop: e.spacing.xs
             },
-            placeholder: QE(JE({}, e.fn.cover()), {
+            placeholder: Ej(kj({}, e.fn.cover()), {
                 display: "flex",
                 alignItems: "center",
                 justifyContent: "center",
                 color: "dark" === e.colorScheme ? e.colors.dark[2] : e.colors.gray[6],
                 backgroundColor: "dark" === e.colorScheme ? e.colors.dark[8] : e.colors.gray[0],
                 borderRadius: e.fn.size({
                     size: t,
                     sizes: e.radius
                 })
             })
         })),
-        tj = Object.defineProperty,
-        rj = Object.getOwnPropertySymbols,
-        nj = Object.prototype.hasOwnProperty,
-        aj = Object.prototype.propertyIsEnumerable,
-        oj = (e, t, r) => t in e ? tj(e, t, {
+        Pj = Object.defineProperty,
+        zj = Object.getOwnPropertySymbols,
+        Cj = Object.prototype.hasOwnProperty,
+        Nj = Object.prototype.propertyIsEnumerable,
+        Tj = (e, t, r) => t in e ? Pj(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        ij = (e, t) => {
-            for (var r in t || (t = {})) nj.call(t, r) && oj(e, r, t[r]);
-            if (rj)
-                for (var r of rj(t)) aj.call(t, r) && oj(e, r, t[r]);
+        Dj = (e, t) => {
+            for (var r in t || (t = {})) Cj.call(t, r) && Tj(e, r, t[r]);
+            if (zj)
+                for (var r of zj(t)) Nj.call(t, r) && Tj(e, r, t[r]);
             return e
         };
-    const lj = {
+    const Ij = {
             fit: "cover",
             width: "100%",
             height: "auto",
             radius: 0
         },
-        sj = Object(n.forwardRef)((e, t) => {
-            const r = ir("Image", lj, e),
+        Rj = Object(n.forwardRef)((e, t) => {
+            const r = ir("Image", Ij, e),
                 {
                     className: o,
                     alt: i,
                     src: l,
                     fit: s,
                     width: c,
                     height: u,
@@ -22122,42 +22449,42 @@
                     imageRef: b,
                     classNames: g,
                     styles: y,
                     caption: h
                 } = r,
                 v = ((e, t) => {
                     var r = {};
-                    for (var n in e) nj.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && rj)
-                        for (var n of rj(e)) t.indexOf(n) < 0 && aj.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) Cj.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && zj)
+                        for (var n of zj(e)) t.indexOf(n) < 0 && Nj.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["className", "alt", "src", "fit", "width", "height", "radius", "imageProps", "withPlaceholder", "placeholder", "imageRef", "classNames", "styles", "caption"]),
                 {
                     classes: O,
                     cx: w
-                } = ej({
+                } = jj({
                     radius: d
                 }, {
                     classNames: g,
                     styles: y,
                     name: "Image"
                 }),
                 [x, S] = Object(n.useState)(!1),
                 [k, E] = Object(n.useState)(!l),
                 j = f && (!x || k);
             return _u(() => {
                 S(!1), E(!1)
-            }, [l]), a.a.createElement(Cn, ij({
+            }, [l]), a.a.createElement(Cn, Dj({
                 className: w(O.root, o),
                 ref: t
             }, v), a.a.createElement("figure", {
                 className: O.figure
             }, a.a.createElement("div", {
                 className: O.imageWrapper
-            }, a.a.createElement("img", ij({
+            }, a.a.createElement("img", Dj({
                 className: O.image,
                 src: l,
                 alt: i,
                 style: {
                     objectFit: s,
                     width: c,
                     height: u
@@ -22168,118 +22495,118 @@
                 },
                 onError: e => {
                     E(!0), "function" == typeof(null == p ? void 0 : p.onError) && p.onError(e)
                 }
             }, p)), j && a.a.createElement("div", {
                 className: O.placeholder,
                 title: i
-            }, m || a.a.createElement(VE, {
+            }, m || a.a.createElement(gj, {
                 style: {
                     width: 40,
                     height: 40
                 }
             }))), !!h && a.a.createElement(jo, {
                 component: "figcaption",
                 size: "sm",
                 align: "center",
                 className: O.caption
             }, h)))
         });
 
-    function cj() {
-        return (cj = Object.assign || function(e) {
+    function _j() {
+        return (_j = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    sj.displayName = "@mantine/core/Image";
-    var uj = function(e) {
+    Rj.displayName = "@mantine/core/Image";
+    var Lj = function(e) {
         var t = e.class_name,
             r = e.placeholder;
-        return a.a.createElement(sj, cj({}, G(["setProps", "class_name", "placeholder"], e), {
+        return a.a.createElement(Rj, _j({}, G(["setProps", "class_name", "placeholder"], e), {
             className: t,
             placeholder: ea(r)
         }))
     };
-    uj.displayName = "Image", uj.defaultProps = {}, uj.propTypes = {
+    Lj.displayName = "Image", Lj.defaultProps = {}, Lj.propTypes = {
         alt: i.a.string,
         caption: i.a.string,
         class_name: i.a.string,
         fit: i.a.oneOf(["cover", "contain"]),
         height: i.a.oneOfType([i.a.string, i.a.number]),
         id: i.a.string,
         placeholder: i.a.any,
         radius: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         src: i.a.string,
         style: i.a.object,
         width: i.a.oneOfType([i.a.string, i.a.number]),
         withPlaceholder: i.a.bool
     };
-    var dj = uj,
-        pj = Object.defineProperty,
-        fj = Object.getOwnPropertySymbols,
-        mj = Object.prototype.hasOwnProperty,
-        bj = Object.prototype.propertyIsEnumerable,
-        gj = (e, t, r) => t in e ? pj(e, t, {
+    var Aj = Lj,
+        Mj = Object.defineProperty,
+        Fj = Object.getOwnPropertySymbols,
+        $j = Object.prototype.hasOwnProperty,
+        Bj = Object.prototype.propertyIsEnumerable,
+        Wj = (e, t, r) => t in e ? Mj(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
 
-    function yj(e) {
+    function Hj(e) {
         return a.a.createElement("svg", ((e, t) => {
-            for (var r in t || (t = {})) mj.call(t, r) && gj(e, r, t[r]);
-            if (fj)
-                for (var r of fj(t)) bj.call(t, r) && gj(e, r, t[r]);
+            for (var r in t || (t = {})) $j.call(t, r) && Wj(e, r, t[r]);
+            if (Fj)
+                for (var r of Fj(t)) Bj.call(t, r) && Wj(e, r, t[r]);
             return e
         })({
             width: "20",
             height: "20",
             viewBox: "0 0 409.294 409.294",
             fill: "currentColor",
             xmlns: "http://www.w3.org/2000/svg"
         }, e), a.a.createElement("path", {
             d: "M0 204.647v175.412h175.412V204.647H58.471c0-64.48 52.461-116.941 116.941-116.941V29.235C78.684 29.235 0 107.919 0 204.647zM409.294 87.706V29.235c-96.728 0-175.412 78.684-175.412 175.412v175.412h175.412V204.647H292.353c0-64.48 52.461-116.941 116.941-116.941z"
         }))
     }
-    var hj = Object.defineProperty,
-        vj = Object.defineProperties,
-        Oj = Object.getOwnPropertyDescriptors,
-        wj = Object.getOwnPropertySymbols,
-        xj = Object.prototype.hasOwnProperty,
-        Sj = Object.prototype.propertyIsEnumerable,
-        kj = (e, t, r) => t in e ? hj(e, t, {
+    var Vj = Object.defineProperty,
+        qj = Object.defineProperties,
+        Uj = Object.getOwnPropertyDescriptors,
+        Gj = Object.getOwnPropertySymbols,
+        Yj = Object.prototype.hasOwnProperty,
+        Zj = Object.prototype.propertyIsEnumerable,
+        Kj = (e, t, r) => t in e ? Vj(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        Ej = (e, t) => {
-            for (var r in t || (t = {})) xj.call(t, r) && kj(e, r, t[r]);
-            if (wj)
-                for (var r of wj(t)) Sj.call(t, r) && kj(e, r, t[r]);
+        Xj = (e, t) => {
+            for (var r in t || (t = {})) Yj.call(t, r) && Kj(e, r, t[r]);
+            if (Gj)
+                for (var r of Gj(t)) Zj.call(t, r) && Kj(e, r, t[r]);
             return e
         },
-        jj = Er((e, {
+        Jj = Er((e, {
             color: t
         }) => {
             return {
-                root: (r = Ej({}, e.fn.fontStyles()), n = {
+                root: (r = Xj({}, e.fn.fontStyles()), n = {
                     fontSize: e.fontSizes.lg,
                     lineHeight: e.lineHeight,
                     color: "dark" === e.colorScheme ? e.colors.dark[0] : e.black,
                     margin: 0,
                     borderTopRightRadius: e.radius.sm,
                     borderBottomRightRadius: e.radius.sm,
                     padding: `${e.spacing.md}px ${e.spacing.lg}px`
-                }, vj(r, Oj(n))),
+                }, qj(r, Uj(n))),
                 inner: {
                     display: "flex"
                 },
                 body: {
                     flex: 1,
                     overflow: "hidden",
                     textOverflow: "ellipsis"
@@ -22297,60 +22624,60 @@
                     color: "dark" === e.colorScheme ? e.colors.dark[2] : e.colors.gray[6],
                     overflow: "hidden",
                     textOverflow: "ellipsis"
                 }
             };
             var r, n
         }),
-        Pj = Object.defineProperty,
-        zj = Object.getOwnPropertySymbols,
-        Cj = Object.prototype.hasOwnProperty,
-        Nj = Object.prototype.propertyIsEnumerable,
-        Tj = (e, t, r) => t in e ? Pj(e, t, {
+        Qj = Object.defineProperty,
+        eP = Object.getOwnPropertySymbols,
+        tP = Object.prototype.hasOwnProperty,
+        rP = Object.prototype.propertyIsEnumerable,
+        nP = (e, t, r) => t in e ? Qj(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const Dj = {
+    const aP = {
             color: "gray",
-            icon: a.a.createElement(yj, null)
+            icon: a.a.createElement(Hj, null)
         },
-        Ij = Object(n.forwardRef)((e, t) => {
-            const r = ir("Blockquote", Dj, e),
+        oP = Object(n.forwardRef)((e, t) => {
+            const r = ir("Blockquote", aP, e),
                 {
                     className: n,
                     color: o,
                     icon: i,
                     cite: l,
                     children: s,
                     classNames: c,
                     styles: u
                 } = r,
                 d = ((e, t) => {
                     var r = {};
-                    for (var n in e) Cj.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && zj)
-                        for (var n of zj(e)) t.indexOf(n) < 0 && Nj.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) tP.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && eP)
+                        for (var n of eP(e)) t.indexOf(n) < 0 && rP.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["className", "color", "icon", "cite", "children", "classNames", "styles"]),
                 {
                     classes: p,
                     cx: f
-                } = jj({
+                } = Jj({
                     color: o
                 }, {
                     classNames: c,
                     styles: u,
                     name: "Blockquote"
                 });
             return a.a.createElement(Cn, ((e, t) => {
-                for (var r in t || (t = {})) Cj.call(t, r) && Tj(e, r, t[r]);
-                if (zj)
-                    for (var r of zj(t)) Nj.call(t, r) && Tj(e, r, t[r]);
+                for (var r in t || (t = {})) tP.call(t, r) && nP(e, r, t[r]);
+                if (eP)
+                    for (var r of eP(t)) rP.call(t, r) && nP(e, r, t[r]);
                 return e
             })({
                 component: "blockquote",
                 className: f(p.root, n),
                 ref: t
             }, d), a.a.createElement("div", {
                 className: p.inner
@@ -22359,93 +22686,93 @@
             }, i), a.a.createElement("div", {
                 className: p.body
             }, s, l && a.a.createElement("cite", {
                 className: p.cite
             }, l))))
         });
 
-    function Rj() {
-        return (Rj = Object.assign || function(e) {
+    function iP() {
+        return (iP = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    Ij.displayName = "@mantine/core/Blockquote";
-    var _j = function(e) {
+    oP.displayName = "@mantine/core/Blockquote";
+    var lP = function(e) {
         var t = e.children,
             r = e.class_name,
             n = e.icon;
-        return a.a.createElement(Ij, Rj({}, G(["setProps", "children", "class_name", "icon"], e), {
+        return a.a.createElement(oP, iP({}, G(["setProps", "children", "class_name", "icon"], e), {
             className: r,
             icon: n ? ea(n) : void 0
         }), t)
     };
-    _j.displayName = "Blockquote", _j.defaultProps = {}, _j.propTypes = {
+    lP.displayName = "Blockquote", lP.defaultProps = {}, lP.propTypes = {
         children: i.a.string,
         class_name: i.a.string,
         cite: i.a.string,
         color: i.a.oneOf(["dark", "gray", "red", "pink", "grape", "violet", "indigo", "blue", "cyan", "teal", "green", "lime", "yellow", "orange"]),
         icon: i.a.any,
         id: i.a.string,
         style: i.a.object
     };
-    var Lj = _j,
-        Aj = Object.defineProperty,
-        Mj = Object.getOwnPropertySymbols,
-        Fj = Object.prototype.hasOwnProperty,
-        $j = Object.prototype.propertyIsEnumerable,
-        Bj = (e, t, r) => t in e ? Aj(e, t, {
+    var sP = lP,
+        cP = Object.defineProperty,
+        uP = Object.getOwnPropertySymbols,
+        dP = Object.prototype.hasOwnProperty,
+        pP = Object.prototype.propertyIsEnumerable,
+        fP = (e, t, r) => t in e ? cP(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
 
-    function Wj(e) {
+    function mP(e) {
         return a.a.createElement("svg", ((e, t) => {
-            for (var r in t || (t = {})) Fj.call(t, r) && Bj(e, r, t[r]);
-            if (Mj)
-                for (var r of Mj(t)) $j.call(t, r) && Bj(e, r, t[r]);
+            for (var r in t || (t = {})) dP.call(t, r) && fP(e, r, t[r]);
+            if (uP)
+                for (var r of uP(t)) pP.call(t, r) && fP(e, r, t[r]);
             return e
         })({
             viewBox: "0 0 15 15",
             fill: "none",
             xmlns: "http://www.w3.org/2000/svg",
             width: 16,
             height: 16
         }, e), a.a.createElement("path", {
             d: "M3.13523 6.15803C3.3241 5.95657 3.64052 5.94637 3.84197 6.13523L7.5 9.56464L11.158 6.13523C11.3595 5.94637 11.6759 5.95657 11.8648 6.15803C12.0536 6.35949 12.0434 6.67591 11.842 6.86477L7.84197 10.6148C7.64964 10.7951 7.35036 10.7951 7.15803 10.6148L3.15803 6.86477C2.95657 6.67591 2.94637 6.35949 3.13523 6.15803Z",
             fill: "currentColor",
             fillRule: "evenodd",
             clipRule: "evenodd"
         }))
     }
-    var Hj = Object.defineProperty,
-        Vj = Object.defineProperties,
-        qj = Object.getOwnPropertyDescriptors,
-        Uj = Object.getOwnPropertySymbols,
-        Gj = Object.prototype.hasOwnProperty,
-        Yj = Object.prototype.propertyIsEnumerable,
-        Zj = (e, t, r) => t in e ? Hj(e, t, {
+    var bP = Object.defineProperty,
+        gP = Object.defineProperties,
+        yP = Object.getOwnPropertyDescriptors,
+        hP = Object.getOwnPropertySymbols,
+        vP = Object.prototype.hasOwnProperty,
+        OP = Object.prototype.propertyIsEnumerable,
+        wP = (e, t, r) => t in e ? bP(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        Kj = (e, t) => {
-            for (var r in t || (t = {})) Gj.call(t, r) && Zj(e, r, t[r]);
-            if (Uj)
-                for (var r of Uj(t)) Yj.call(t, r) && Zj(e, r, t[r]);
+        xP = (e, t) => {
+            for (var r in t || (t = {})) vP.call(t, r) && wP(e, r, t[r]);
+            if (hP)
+                for (var r of hP(t)) OP.call(t, r) && wP(e, r, t[r]);
             return e
         },
-        Xj = (e, t) => Vj(e, qj(t)),
-        Jj = Er((e, {
+        SP = (e, t) => gP(e, yP(t)),
+        kP = Er((e, {
             transitionDuration: t,
             disableIconRotation: r,
             iconPosition: n,
             offsetIcon: a,
             iconSize: o
         }, i) => ({
             icon: {
@@ -22474,65 +22801,65 @@
             },
             itemTitle: {
                 ref: i("itemTitle"),
                 margin: 0,
                 padding: 0,
                 fontWeight: "normal"
             },
-            control: Xj(Kj(Kj({}, e.fn.focusStyles()), e.fn.fontStyles()), {
+            control: SP(xP(xP({}, e.fn.focusStyles()), e.fn.fontStyles()), {
                 ref: i("control"),
                 width: "100%",
                 display: "flex",
                 alignItems: "center",
                 flexDirection: "right" === n ? "row-reverse" : "row",
                 padding: `${e.spacing.md}px ${e.spacing.md/2}px`,
                 paddingLeft: "right" === n ? e.spacing.sm + 4 : null,
                 fontWeight: 500,
                 textAlign: "left",
                 color: "dark" === e.colorScheme ? e.colors.dark[0] : e.black,
                 "&:hover": {
                     backgroundColor: "dark" === e.colorScheme ? e.colors.dark[5] : e.colors.gray[0]
                 }
             }),
-            content: Xj(Kj({}, e.fn.fontStyles()), {
+            content: SP(xP({}, e.fn.fontStyles()), {
                 wordBreak: "break-word",
                 lineHeight: e.lineHeight,
                 paddingLeft: "right" === n ? 0 : a ? o + e.spacing.xs / 2 : 0
             }),
             contentInner: {
                 padding: e.spacing.md,
                 paddingTop: e.spacing.xs / 2
             }
         })),
-        Qj = Object.defineProperty,
-        eP = Object.defineProperties,
-        tP = Object.getOwnPropertyDescriptors,
-        rP = Object.getOwnPropertySymbols,
-        nP = Object.prototype.hasOwnProperty,
-        aP = Object.prototype.propertyIsEnumerable,
-        oP = (e, t, r) => t in e ? Qj(e, t, {
+        EP = Object.defineProperty,
+        jP = Object.defineProperties,
+        PP = Object.getOwnPropertyDescriptors,
+        zP = Object.getOwnPropertySymbols,
+        CP = Object.prototype.hasOwnProperty,
+        NP = Object.prototype.propertyIsEnumerable,
+        TP = (e, t, r) => t in e ? EP(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        iP = (e, t) => {
-            for (var r in t || (t = {})) nP.call(t, r) && oP(e, r, t[r]);
-            if (rP)
-                for (var r of rP(t)) aP.call(t, r) && oP(e, r, t[r]);
+        DP = (e, t) => {
+            for (var r in t || (t = {})) CP.call(t, r) && TP(e, r, t[r]);
+            if (zP)
+                for (var r of zP(t)) NP.call(t, r) && TP(e, r, t[r]);
             return e
         },
-        lP = (e, t) => eP(e, tP(t));
+        IP = (e, t) => jP(e, PP(t));
 
-    function sP(e) {
+    function RP(e) {
         return (null == e ? void 0 : e.current) ? e.current.scrollHeight : "auto"
     }
-    const cP = "undefined" != typeof window && window.requestAnimationFrame;
+    const _P = "undefined" != typeof window && window.requestAnimationFrame;
 
-    function uP({
+    function LP({
         transitionDuration: e,
         transitionTimingFunction: t = "ease",
         onTransitionEnd: r = (() => {}),
         opened: a
     }) {
         const o = Object(n.useRef)(null),
             i = {
@@ -22541,199 +22868,199 @@
                 overflow: "hidden"
             },
             [l, s] = Object(n.useState)(a ? {} : i),
             c = e => {
                 Object(Lu.flushSync)(() => s(e))
             },
             u = e => {
-                c(t => iP(iP({}, t), e))
+                c(t => DP(DP({}, t), e))
             };
 
         function d(r) {
             return {
                 transition: `height ${e||function(e){if(!e||"string"==typeof e)return 0;const t=e/36;return Math.round(10*(4+15*t**.25+t/5))}(r)}ms ${t}`
             }
         }
         _u(() => {
-            cP(a ? () => {
+            _P(a ? () => {
                 u({
                     willChange: "height",
                     display: "block",
                     overflow: "hidden"
-                }), cP(() => {
-                    const e = sP(o);
-                    u(lP(iP({}, d(e)), {
+                }), _P(() => {
+                    const e = RP(o);
+                    u(IP(DP({}, d(e)), {
                         height: e
                     }))
                 })
             } : () => {
-                const e = sP(o);
-                u(lP(iP({}, d(e)), {
+                const e = RP(o);
+                u(IP(DP({}, d(e)), {
                     willChange: "height",
                     height: e
-                })), cP(() => u({
+                })), _P(() => u({
                     height: "0px",
                     overflow: "hidden"
                 }))
             })
         }, [a]);
         const p = e => {
             if (e.target === o.current && "height" === e.propertyName)
                 if (a) {
-                    const e = sP(o);
+                    const e = RP(o);
                     e === l.height ? c({}) : u({
                         height: e
                     }), r()
                 } else "0px" === l.height && (c(i), r())
         };
         return function(e = {}) {
             var t = e,
                 {
                     style: r = {},
                     refKey: n = "ref"
                 } = t,
                 i = ((e, t) => {
                     var r = {};
-                    for (var n in e) nP.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && rP)
-                        for (var n of rP(e)) t.indexOf(n) < 0 && aP.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) CP.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && zP)
+                        for (var n of zP(e)) t.indexOf(n) < 0 && NP.call(e, n) && (r[n] = e[n]);
                     return r
                 })(t, ["style", "refKey"]);
             const s = i[n];
-            return lP(iP({
+            return IP(DP({
                 "aria-hidden": !a
             }, i), {
                 [n]: ua(o, s),
                 onTransitionEnd: p,
-                style: iP(iP({
+                style: DP(DP({
                     boxSizing: "border-box"
                 }, r), l)
             })
         }
     }
-    var dP = Object.defineProperty,
-        pP = Object.getOwnPropertySymbols,
-        fP = Object.prototype.hasOwnProperty,
-        mP = Object.prototype.propertyIsEnumerable,
-        bP = (e, t, r) => t in e ? dP(e, t, {
+    var AP = Object.defineProperty,
+        MP = Object.getOwnPropertySymbols,
+        FP = Object.prototype.hasOwnProperty,
+        $P = Object.prototype.propertyIsEnumerable,
+        BP = (e, t, r) => t in e ? AP(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        gP = (e, t) => {
-            for (var r in t || (t = {})) fP.call(t, r) && bP(e, r, t[r]);
-            if (pP)
-                for (var r of pP(t)) mP.call(t, r) && bP(e, r, t[r]);
+        WP = (e, t) => {
+            for (var r in t || (t = {})) FP.call(t, r) && BP(e, r, t[r]);
+            if (MP)
+                for (var r of MP(t)) $P.call(t, r) && BP(e, r, t[r]);
             return e
         };
-    const yP = {
+    const HP = {
         transitionDuration: 200,
         transitionTimingFunction: "ease",
         animateOpacity: !0
     };
 
-    function hP(e) {
-        const t = ir("Collapse", yP, e),
+    function VP(e) {
+        const t = ir("Collapse", HP, e),
             {
                 children: r,
                 in: n,
                 transitionDuration: o,
                 transitionTimingFunction: i,
                 style: l,
                 onTransitionEnd: s,
                 animateOpacity: c
             } = t,
             u = ((e, t) => {
                 var r = {};
-                for (var n in e) fP.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                if (null != e && pP)
-                    for (var n of pP(e)) t.indexOf(n) < 0 && mP.call(e, n) && (r[n] = e[n]);
+                for (var n in e) FP.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                if (null != e && MP)
+                    for (var n of MP(e)) t.indexOf(n) < 0 && $P.call(e, n) && (r[n] = e[n]);
                 return r
             })(t, ["children", "in", "transitionDuration", "transitionTimingFunction", "style", "onTransitionEnd", "animateOpacity"]),
             d = vd() ? 0 : o,
             {
                 systemStyles: p,
                 rest: f
             } = gn(u),
-            m = uP({
+            m = LP({
                 opened: n,
                 transitionDuration: d,
                 transitionTimingFunction: i,
                 onTransitionEnd: s
             });
-        return 0 === d ? n ? a.a.createElement(Cn, gP({}, f), r) : null : a.a.createElement(Cn, gP({}, m(gP(gP({
+        return 0 === d ? n ? a.a.createElement(Cn, WP({}, f), r) : null : a.a.createElement(Cn, WP({}, m(WP(WP({
             style: l
         }, f), p))), a.a.createElement("div", {
             style: {
                 opacity: n || !c ? 1 : 0,
                 transition: c ? `opacity ${d}ms ${i}` : "none"
             }
         }, r))
     }
-    hP.displayName = "@mantine/core/Collapse";
-    var vP = Object.defineProperty,
-        OP = Object.getOwnPropertySymbols,
-        wP = Object.prototype.hasOwnProperty,
-        xP = Object.prototype.propertyIsEnumerable,
-        SP = (e, t, r) => t in e ? vP(e, t, {
+    VP.displayName = "@mantine/core/Collapse";
+    var qP = Object.defineProperty,
+        UP = Object.getOwnPropertySymbols,
+        GP = Object.prototype.hasOwnProperty,
+        YP = Object.prototype.propertyIsEnumerable,
+        ZP = (e, t, r) => t in e ? qP(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
 
-    function kP(e) {
+    function KP(e) {
         var t = e,
             {
                 opened: r,
                 onToggle: n,
                 label: o,
                 children: i,
                 className: l,
                 classNames: s,
                 styles: c,
                 transitionDuration: u,
-                icon: d = a.a.createElement(Wj, null),
+                icon: d = a.a.createElement(mP, null),
                 disableIconRotation: p = !1,
                 offsetIcon: f = !0,
                 iconSize: m = 24,
                 iconPosition: b = "left",
                 order: g = 3,
                 id: y,
                 controlRef: h,
                 onControlKeyDown: v
             } = t,
             O = ((e, t) => {
                 var r = {};
-                for (var n in e) wP.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                if (null != e && OP)
-                    for (var n of OP(e)) t.indexOf(n) < 0 && xP.call(e, n) && (r[n] = e[n]);
+                for (var n in e) GP.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                if (null != e && UP)
+                    for (var n of UP(e)) t.indexOf(n) < 0 && YP.call(e, n) && (r[n] = e[n]);
                 return r
             })(t, ["opened", "onToggle", "label", "children", "className", "classNames", "styles", "transitionDuration", "icon", "disableIconRotation", "offsetIcon", "iconSize", "iconPosition", "order", "id", "controlRef", "onControlKeyDown"]);
         const w = vd() ? 0 : u,
             {
                 classes: x,
                 cx: S
-            } = Jj({
+            } = kP({
                 transitionDuration: w,
                 disableIconRotation: p,
                 iconPosition: b,
                 offsetIcon: f,
                 iconSize: m
             }, {
                 classNames: s,
                 styles: c,
                 name: "Accordion"
             }),
             k = "h" + Math.min(6, Math.max(2, g));
         return a.a.createElement(Cn, ((e, t) => {
-            for (var r in t || (t = {})) wP.call(t, r) && SP(e, r, t[r]);
-            if (OP)
-                for (var r of OP(t)) xP.call(t, r) && SP(e, r, t[r]);
+            for (var r in t || (t = {})) GP.call(t, r) && ZP(e, r, t[r]);
+            if (UP)
+                for (var r of UP(t)) YP.call(t, r) && ZP(e, r, t[r]);
             return e
         })({
             className: S(x.item, {
                 [x.itemOpened]: r
             }, l)
         }, O), a.a.createElement(k, {
             className: x.itemTitle
@@ -22742,115 +23069,115 @@
             onClick: n,
             type: "button",
             "aria-expanded": r,
             "aria-controls": y + "-body",
             id: y,
             ref: h,
             onKeyDown: v
-        }, a.a.createElement(kO, {
+        }, a.a.createElement(KO, {
             className: x.icon
         }, d), a.a.createElement("div", {
             className: x.label
-        }, o))), a.a.createElement(hP, {
+        }, o))), a.a.createElement(VP, {
             in: r,
             transitionDuration: w
         }, a.a.createElement("div", {
             className: x.content,
             role: "region",
             id: y + "-body",
             "aria-labelledby": y
         }, a.a.createElement("div", {
             className: x.contentInner
         }, i))))
     }
-    kP.displayName = "@mantine/core/AccordionItem";
-    var EP = Object.defineProperty,
-        jP = Object.defineProperties,
-        PP = Object.getOwnPropertyDescriptors,
-        zP = Object.getOwnPropertySymbols,
-        CP = Object.prototype.hasOwnProperty,
-        NP = Object.prototype.propertyIsEnumerable,
-        TP = (e, t, r) => t in e ? EP(e, t, {
+    KP.displayName = "@mantine/core/AccordionItem";
+    var XP = Object.defineProperty,
+        JP = Object.defineProperties,
+        QP = Object.getOwnPropertyDescriptors,
+        ez = Object.getOwnPropertySymbols,
+        tz = Object.prototype.hasOwnProperty,
+        rz = Object.prototype.propertyIsEnumerable,
+        nz = (e, t, r) => t in e ? XP(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
 
-    function DP(e, t = -1) {
+    function az(e, t = -1) {
         return Array.from({
             length: e
         }).reduce((e, r, n) => (e[n] = n === t, e), {})
     }
 
-    function IP({
+    function oz({
         initialState: e,
         total: t,
         initialItem: r = -1,
         state: n,
         onChange: a,
         multiple: o = !1
     }) {
         const [i, l] = la({
             value: n,
-            defaultValue: e || DP(t, r),
+            defaultValue: e || az(t, r),
             finalValue: {},
             onChange: a,
             rule: e => null !== e && "object" == typeof e
         });
         return _u(() => {
-            o || l(DP(t))
+            o || l(az(t))
         }, [o]), [i, {
             toggle: e => {
-                if (o) l(((e, t) => jP(e, PP(t)))(((e, t) => {
-                    for (var r in t || (t = {})) CP.call(t, r) && TP(e, r, t[r]);
-                    if (zP)
-                        for (var r of zP(t)) NP.call(t, r) && TP(e, r, t[r]);
+                if (o) l(((e, t) => JP(e, QP(t)))(((e, t) => {
+                    for (var r in t || (t = {})) tz.call(t, r) && nz(e, r, t[r]);
+                    if (ez)
+                        for (var r of ez(t)) rz.call(t, r) && nz(e, r, t[r]);
                     return e
                 })({}, i), {
                     [e]: !i[e]
                 }));
                 else {
                     const r = Array(t).fill(0).reduce((e, t, r) => (e[r] = !1, e), {});
                     r[e] = !i[e], l(r)
                 }
             },
             setState: l
         }]
     }
-    var RP = Object.defineProperty,
-        _P = Object.defineProperties,
-        LP = Object.getOwnPropertyDescriptors,
-        AP = Object.getOwnPropertySymbols,
-        MP = Object.prototype.hasOwnProperty,
-        FP = Object.prototype.propertyIsEnumerable,
-        $P = (e, t, r) => t in e ? RP(e, t, {
+    var iz = Object.defineProperty,
+        lz = Object.defineProperties,
+        sz = Object.getOwnPropertyDescriptors,
+        cz = Object.getOwnPropertySymbols,
+        uz = Object.prototype.hasOwnProperty,
+        dz = Object.prototype.propertyIsEnumerable,
+        pz = (e, t, r) => t in e ? iz(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        BP = (e, t) => {
-            for (var r in t || (t = {})) MP.call(t, r) && $P(e, r, t[r]);
-            if (AP)
-                for (var r of AP(t)) FP.call(t, r) && $P(e, r, t[r]);
+        fz = (e, t) => {
+            for (var r in t || (t = {})) uz.call(t, r) && pz(e, r, t[r]);
+            if (cz)
+                for (var r of cz(t)) dz.call(t, r) && pz(e, r, t[r]);
             return e
         };
-    const WP = {
+    const mz = {
             initialItem: -1,
             multiple: !1,
             disableIconRotation: !1,
             transitionDuration: 200,
             iconPosition: "left",
             offsetIcon: !0,
             iconSize: 24,
             order: 3
         },
-        HP = Object(n.forwardRef)((e, t) => {
-            const r = ir("Accordion", WP, e),
+        bz = Object(n.forwardRef)((e, t) => {
+            const r = ir("Accordion", mz, e),
                 {
                     children: o,
                     initialItem: i,
                     initialState: l,
                     state: s,
                     onChange: c,
                     multiple: u,
@@ -22863,21 +23190,21 @@
                     icon: y,
                     classNames: h,
                     styles: v,
                     id: O
                 } = r,
                 w = ((e, t) => {
                     var r = {};
-                    for (var n in e) MP.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && AP)
-                        for (var n of AP(e)) t.indexOf(n) < 0 && FP.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) uz.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && cz)
+                        for (var n of cz(e)) t.indexOf(n) < 0 && dz.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["children", "initialItem", "initialState", "state", "onChange", "multiple", "disableIconRotation", "transitionDuration", "iconPosition", "offsetIcon", "iconSize", "order", "icon", "classNames", "styles", "id"]),
                 x = Ja(O),
-                S = si(o, kP),
+                S = si(o, KP),
                 {
                     handleItemKeydown: k,
                     assignControlRef: E
                 } = function(e) {
                     const t = Object(n.useRef)([]);
                     return _u(() => {
                         t.current = t.current.slice(0, e)
@@ -22896,25 +23223,25 @@
                             }
                         },
                         assignControlRef: e => r => {
                             t.current[e] = r
                         }
                     }
                 }(S.length),
-                [j, P] = IP({
+                [j, P] = oz({
                     multiple: u,
                     total: S.length,
                     initialItem: i,
                     state: s,
                     initialState: l,
                     onChange: c
                 }),
                 z = S.map((e, t) => {
                     var r, n, o, i, l;
-                    return a.a.createElement(kP, (i = BP({}, e.props), l = {
+                    return a.a.createElement(KP, (i = fz({}, e.props), l = {
                         icon: e.props.icon || y,
                         iconPosition: e.props.iconPosition || f,
                         disableIconRotation: d,
                         key: t,
                         transitionDuration: p,
                         opened: j[t],
                         onToggle: () => P.toggle(t),
@@ -22922,53 +23249,53 @@
                         styles: (null == (n = e.props) ? void 0 : n.styles) || v,
                         id: `${x}-${t}`,
                         onControlKeyDown: k(t),
                         controlRef: da(E(t), null == (o = e.props) ? void 0 : o.controlRef),
                         offsetIcon: m,
                         iconSize: b,
                         order: g
-                    }, _P(i, LP(l))))
+                    }, lz(i, sz(l))))
                 });
-            return a.a.createElement(Cn, BP({
+            return a.a.createElement(Cn, fz({
                 ref: t
             }, w), z)
         });
 
-    function VP() {
-        return (VP = Object.assign || function(e) {
+    function gz() {
+        return (gz = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    HP.Item = kP, HP.displayName = "@mantine/core/Accordion";
-    var qP = function(e) {
+    bz.Item = KP, bz.displayName = "@mantine/core/Accordion";
+    var yz = function(e) {
         var t = e.children,
             r = e.setProps,
             n = e.class_name,
             o = e.icon;
-        return a.a.createElement(HP, VP({}, G(["setProps", "class_name", "icon"], e), {
+        return a.a.createElement(bz, gz({}, G(["setProps", "class_name", "icon"], e), {
             onChange: function(e) {
                 r({
                     state: e
                 })
             },
             icon: o ? ea(o) : void 0,
             className: n
         }), a.a.Children.map(t, (function(e, t) {
             var r = e.props._dashprivate_layout.props,
                 n = ta(G(["children"], r), ["label", "icon"]);
-            return a.a.createElement(HP.Item, VP({}, n, {
+            return a.a.createElement(bz.Item, gz({}, n, {
                 key: t
             }), e)
         })))
     };
-    qP.displayName = "Accordion", qP.defaultProps = {}, qP.propTypes = {
+    yz.displayName = "Accordion", yz.defaultProps = {}, yz.propTypes = {
         children: i.a.node,
         class_name: i.a.string,
         disableIconRotation: i.a.bool,
         icon: i.a.any,
         iconPosition: i.a.oneOf(["right", "left"]),
         iconSize: i.a.number,
         id: i.a.string,
@@ -22976,33 +23303,33 @@
         offsetIcon: i.a.bool,
         order: i.a.oneOf([1, 2, 3, 4, 5, 6]),
         setProps: i.a.func,
         state: i.a.objectOf(i.a.bool),
         style: i.a.object,
         transitionDuration: i.a.number
     };
-    var UP = qP,
-        GP = function(e) {
+    var hz = yz,
+        vz = function(e) {
             return a.a.createElement(a.a.Fragment, null, e.children)
         };
-    GP.displayName = "AccordionItem", GP.defaultProps = {}, GP.propTypes = {
+    vz.displayName = "AccordionItem", vz.defaultProps = {}, vz.propTypes = {
         children: i.a.node,
         icon: i.a.any,
         label: i.a.any.isRequired
     };
-    var YP = GP;
-    const ZP = zt({
+    var Oz = vz;
+    const wz = zt({
         "from, to": {
             opacity: .4
         },
         "50%": {
             opacity: 1
         }
     });
-    var KP = Er((e, {
+    var xz = Er((e, {
             height: t,
             width: r,
             radius: n,
             circle: a,
             animate: o
         }) => ({
             root: {
@@ -23027,103 +23354,103 @@
                     content: '""',
                     position: "absolute",
                     background: "dark" === e.colorScheme ? e.colors.dark[4] : e.colors.gray[3],
                     top: 0,
                     bottom: 0,
                     left: 0,
                     right: 0,
-                    animation: o ? ZP + " 1500ms linear infinite" : "none",
+                    animation: o ? wz + " 1500ms linear infinite" : "none",
                     zIndex: 11
                 }
             }
         })),
-        XP = Object.defineProperty,
-        JP = Object.getOwnPropertySymbols,
-        QP = Object.prototype.hasOwnProperty,
-        ez = Object.prototype.propertyIsEnumerable,
-        tz = (e, t, r) => t in e ? XP(e, t, {
+        Sz = Object.defineProperty,
+        kz = Object.getOwnPropertySymbols,
+        Ez = Object.prototype.hasOwnProperty,
+        jz = Object.prototype.propertyIsEnumerable,
+        Pz = (e, t, r) => t in e ? Sz(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const rz = {
+    const zz = {
             height: "auto",
             width: "100%",
             visible: !0,
             animate: !0
         },
-        nz = Object(n.forwardRef)((e, t) => {
-            const r = ir("Skeleton", rz, e),
+        Cz = Object(n.forwardRef)((e, t) => {
+            const r = ir("Skeleton", zz, e),
                 {
                     height: n,
                     width: o,
                     visible: i,
                     animate: l,
                     className: s,
                     circle: c,
                     radius: u,
                     classNames: d,
                     styles: p
                 } = r,
                 f = ((e, t) => {
                     var r = {};
-                    for (var n in e) QP.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && JP)
-                        for (var n of JP(e)) t.indexOf(n) < 0 && ez.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) Ez.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && kz)
+                        for (var n of kz(e)) t.indexOf(n) < 0 && jz.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["height", "width", "visible", "animate", "className", "circle", "radius", "classNames", "styles"]),
                 {
                     classes: m,
                     cx: b
-                } = KP({
+                } = xz({
                     height: n,
                     width: o,
                     circle: c,
                     radius: u,
                     animate: l
                 }, {
                     classNames: d,
                     styles: p,
                     name: "Skeleton"
                 });
             return a.a.createElement(Cn, ((e, t) => {
-                for (var r in t || (t = {})) QP.call(t, r) && tz(e, r, t[r]);
-                if (JP)
-                    for (var r of JP(t)) ez.call(t, r) && tz(e, r, t[r]);
+                for (var r in t || (t = {})) Ez.call(t, r) && Pz(e, r, t[r]);
+                if (kz)
+                    for (var r of kz(t)) jz.call(t, r) && Pz(e, r, t[r]);
                 return e
             })({
                 className: b(m.root, {
                     [m.visible]: i
                 }, s),
                 ref: t
             }, f))
         });
 
-    function az() {
-        return (az = Object.assign || function(e) {
+    function Nz() {
+        return (Nz = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    nz.displayName = "@mantine/core/Skeleton";
-    var oz = function(e) {
+    Cz.displayName = "@mantine/core/Skeleton";
+    var Tz = function(e) {
         var t = e.children,
             r = e.visible,
             n = e.loading_state;
-        return a.a.createElement(nz, az({}, G(["setProps", "children", "visible", "loading_state"], e), {
+        return a.a.createElement(Cz, Nz({}, G(["setProps", "children", "visible", "loading_state"], e), {
             visible: r || n && n.is_loading
         }), t)
     };
-    oz.displayName = "Skeleton", oz._dashprivate_isLoadingComponent = !0, oz.defaultProps = {
+    Tz.displayName = "Skeleton", Tz._dashprivate_isLoadingComponent = !0, Tz.defaultProps = {
         visible: !0
-    }, oz.propTypes = {
+    }, Tz.propTypes = {
         animate: i.a.bool,
         children: i.a.node,
         circle: i.a.bool,
         height: i.a.oneOfType([i.a.string, i.a.number]),
         id: i.a.string,
         loading_state: i.a.shape({
             is_loading: i.a.bool,
@@ -23131,16 +23458,16 @@
             component_name: i.a.string
         }),
         radius: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         style: i.a.object,
         visible: i.a.bool,
         width: i.a.oneOfType([i.a.string, i.a.number])
     };
-    var iz = oz,
-        lz = Er((e, {
+    var Dz = Tz,
+        Iz = Er((e, {
             transitionDuration: t
         }) => ({
             control: {},
             root: {
                 position: "relative"
             },
             content: {
@@ -23149,135 +23476,135 @@
                 transitionTimingFunction: "ease",
                 transitionDuration: t + "ms",
                 "@media (prefers-reduced-motion)": {
                     transitionDuration: "0ms"
                 }
             }
         })),
-        sz = Object.defineProperty,
-        cz = Object.getOwnPropertySymbols,
-        uz = Object.prototype.hasOwnProperty,
-        dz = Object.prototype.propertyIsEnumerable,
-        pz = (e, t, r) => t in e ? sz(e, t, {
+        Rz = Object.defineProperty,
+        _z = Object.getOwnPropertySymbols,
+        Lz = Object.prototype.hasOwnProperty,
+        Az = Object.prototype.propertyIsEnumerable,
+        Mz = (e, t, r) => t in e ? Rz(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const fz = {
+    const Fz = {
             maxHeight: 100,
             transitionDuration: 200,
             initialState: !1
         },
-        mz = Object(n.forwardRef)((e, t) => {
-            const r = ir("Spoiler", fz, e),
+        $z = Object(n.forwardRef)((e, t) => {
+            const r = ir("Spoiler", Fz, e),
                 {
                     className: o,
                     children: i,
                     maxHeight: l,
                     hideLabel: s,
                     showLabel: c,
                     transitionDuration: u,
                     controlRef: d,
                     initialState: p,
                     classNames: f,
                     styles: m
                 } = r,
                 b = ((e, t) => {
                     var r = {};
-                    for (var n in e) uz.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && cz)
-                        for (var n of cz(e)) t.indexOf(n) < 0 && dz.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) Lz.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && _z)
+                        for (var n of _z(e)) t.indexOf(n) < 0 && Az.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["className", "children", "maxHeight", "hideLabel", "showLabel", "transitionDuration", "controlRef", "initialState", "classNames", "styles"]),
                 {
                     classes: g,
                     cx: y
-                } = lz({
+                } = Iz({
                     transitionDuration: u
                 }, {
                     classNames: f,
                     styles: m,
                     name: "Spoiler"
                 }),
                 [h, v] = Object(n.useState)(p),
                 [O, w] = Object(n.useState)(p),
                 x = Object(n.useRef)(null),
                 S = h ? s : c;
             return Object(n.useEffect)(() => {
                 w(l < x.current.clientHeight)
             }, [l, i]), a.a.createElement(Cn, ((e, t) => {
-                for (var r in t || (t = {})) uz.call(t, r) && pz(e, r, t[r]);
-                if (cz)
-                    for (var r of cz(t)) dz.call(t, r) && pz(e, r, t[r]);
+                for (var r in t || (t = {})) Lz.call(t, r) && Mz(e, r, t[r]);
+                if (_z)
+                    for (var r of _z(t)) Az.call(t, r) && Mz(e, r, t[r]);
                 return e
             })({
                 className: y(g.root, o),
                 ref: t
             }, b), a.a.createElement("div", {
                 className: g.content,
                 style: {
                     maxHeight: h ? x.current && x.current.clientHeight : l
                 }
             }, a.a.createElement("div", {
                 ref: x
-            }, i)), O && a.a.createElement(_E, {
+            }, i)), O && a.a.createElement(lj, {
                 component: "button",
                 ref: d,
                 onClick: () => v(e => !e),
                 className: g.control
             }, S))
         });
 
-    function bz() {
-        return (bz = Object.assign || function(e) {
+    function Bz() {
+        return (Bz = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    mz.displayName = "@mantine/core/Spoiler";
-    var gz = function(e) {
+    $z.displayName = "@mantine/core/Spoiler";
+    var Wz = function(e) {
         var t = e.children,
             r = e.class_name;
-        return a.a.createElement(mz, bz({}, G(["setProps", "children", "class_name"], e), {
+        return a.a.createElement($z, Bz({}, G(["setProps", "children", "class_name"], e), {
             className: r
         }), t)
     };
-    gz.displayName = "Spoiler", gz.defaultProps = {}, gz.propTypes = {
+    Wz.displayName = "Spoiler", Wz.defaultProps = {}, Wz.propTypes = {
         class_name: i.a.string,
         children: i.a.node,
         hideLabel: i.a.string.isRequired,
         id: i.a.string,
         initialState: i.a.bool,
         maxHeight: i.a.number,
         showLabel: i.a.string.isRequired,
         style: i.a.object,
         transitionDuration: i.a.number
     };
-    var yz = gz;
+    var Hz = Wz;
 
-    function hz() {
-        return (hz = Object.assign || function(e) {
+    function Vz() {
+        return (Vz = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    var vz = function(e) {
+    var qz = function(e) {
         var t = e.class_name;
-        return a.a.createElement(Md, hz({}, G(["setProps", "children", "class_name"], e), {
+        return a.a.createElement(Md, Vz({}, G(["setProps", "children", "class_name"], e), {
             className: t
         }), e.children)
     };
-    vz.displayName = "Paper", vz.defaultProps = {}, vz.propTypes = {
+    qz.displayName = "Paper", qz.defaultProps = {}, qz.propTypes = {
         children: i.a.node,
         class_name: i.a.string,
         id: i.a.string,
         radius: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         shadow: i.a.oneOf(["xs", "sm", "md", "lg", "xl"]),
         style: i.a.object,
         withBorder: i.a.bool,
@@ -23292,16 +23619,16 @@
         py: i.a.oneOfType([i.a.string, i.a.number]),
         px: i.a.oneOfType([i.a.string, i.a.number]),
         pt: i.a.oneOfType([i.a.string, i.a.number]),
         pb: i.a.oneOfType([i.a.string, i.a.number]),
         pl: i.a.oneOfType([i.a.string, i.a.number]),
         pr: i.a.oneOfType([i.a.string, i.a.number])
     };
-    var Oz = vz,
-        wz = Er(e => ({
+    var Uz = qz,
+        Gz = Er(e => ({
             root: {
                 display: "flex"
             },
             breadcrumb: {
                 lineHeight: 1,
                 whiteSpace: "nowrap",
                 WebkitTapHighlightColor: "transparent"
@@ -23312,114 +23639,114 @@
                 color: "dark" === e.colorScheme ? e.colors.dark[2] : e.colors.gray[7],
                 lineHeight: 1,
                 display: "flex",
                 alignItems: "center",
                 justifyContent: "center"
             }
         })),
-        xz = Object.defineProperty,
-        Sz = Object.getOwnPropertySymbols,
-        kz = Object.prototype.hasOwnProperty,
-        Ez = Object.prototype.propertyIsEnumerable,
-        jz = (e, t, r) => t in e ? xz(e, t, {
+        Yz = Object.defineProperty,
+        Zz = Object.getOwnPropertySymbols,
+        Kz = Object.prototype.hasOwnProperty,
+        Xz = Object.prototype.propertyIsEnumerable,
+        Jz = (e, t, r) => t in e ? Yz(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const Pz = {
+    const Qz = {
             separator: "/"
         },
-        zz = Object(n.forwardRef)((e, t) => {
-            const r = ir("Breadcrumbs", Pz, e),
+        eC = Object(n.forwardRef)((e, t) => {
+            const r = ir("Breadcrumbs", Qz, e),
                 {
                     className: n,
                     children: o,
                     separator: i,
                     classNames: l,
                     styles: s
                 } = r,
                 c = ((e, t) => {
                     var r = {};
-                    for (var n in e) kz.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && Sz)
-                        for (var n of Sz(e)) t.indexOf(n) < 0 && Ez.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) Kz.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && Zz)
+                        for (var n of Zz(e)) t.indexOf(n) < 0 && Xz.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["className", "children", "separator", "classNames", "styles"]),
                 {
                     classes: u,
                     cx: d
-                } = wz(null, {
+                } = Gz(null, {
                     classNames: l,
                     styles: s,
                     name: "Breadcrumbs"
                 }),
                 p = a.a.Children.toArray(o).reduce((e, t, r, n) => (e.push(a.a.cloneElement(t, {
                     className: u.breadcrumb,
                     key: r
                 })), r !== n.length - 1 && e.push(a.a.createElement(jo, {
                     size: "sm",
                     className: u.separator,
                     key: "separator-" + r
                 }, i)), e), []);
             return a.a.createElement(Cn, ((e, t) => {
-                for (var r in t || (t = {})) kz.call(t, r) && jz(e, r, t[r]);
-                if (Sz)
-                    for (var r of Sz(t)) Ez.call(t, r) && jz(e, r, t[r]);
+                for (var r in t || (t = {})) Kz.call(t, r) && Jz(e, r, t[r]);
+                if (Zz)
+                    for (var r of Zz(t)) Xz.call(t, r) && Jz(e, r, t[r]);
                 return e
             })({
                 className: d(u.root, n),
                 ref: t
             }, c), p)
         });
-    zz.displayName = "@mantine/core/Breadcrumbs";
-    var Cz = function(e) {
+    eC.displayName = "@mantine/core/Breadcrumbs";
+    var tC = function(e) {
         var t = e.children,
             r = e.separator,
             n = e.class_name;
-        return a.a.createElement(zz, {
+        return a.a.createElement(eC, {
             separator: r,
             className: n
         }, t)
     };
-    Cz.displayName = "Breadcrumbs", Cz.defaultProps = {}, Cz.propTypes = {
+    tC.displayName = "Breadcrumbs", tC.defaultProps = {}, tC.propTypes = {
         children: i.a.node,
         class_name: i.a.string,
         id: i.a.string,
         separator: i.a.string,
         style: i.a.object
     };
-    var Nz = Cz;
-    const Tz = {
+    var rC = tC;
+    const nC = {
             xs: 3,
             sm: 5,
             md: 8,
             lg: 12,
             xl: 16
         },
-        Dz = zt({
+        aC = zt({
             from: {
                 backgroundPosition: "0 0"
             },
             to: {
                 backgroundPosition: "40px 0"
             }
         });
-    var Iz = Er((e, {
+    var oC = Er((e, {
             color: t,
             radius: r,
             size: n,
             striped: a,
             animate: o
         }) => ({
             root: {
                 position: "relative",
                 height: e.fn.size({
                     size: n,
-                    sizes: Tz
+                    sizes: nC
                 }),
                 backgroundColor: "dark" === e.colorScheme ? e.colors.dark[4] : e.colors.gray[2],
                 borderRadius: e.fn.size({
                     size: r,
                     sizes: e.radius
                 }),
                 overflow: "hidden"
@@ -23431,15 +23758,15 @@
                 left: 0,
                 height: "100%",
                 display: "flex",
                 justifyContent: "center",
                 alignItems: "center",
                 backgroundColor: e.fn.themeColor(t || e.primaryColor, 6, !1),
                 transition: "width 100ms linear",
-                animation: o ? Dz + " 1000ms linear infinite" : "none",
+                animation: o ? aC + " 1000ms linear infinite" : "none",
                 backgroundSize: "20px 20px",
                 backgroundImage: a ? "linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent)" : "none",
                 "&:last-of-type": {
                     borderTopRightRadius: e.fn.size({
                         size: r,
                         sizes: e.radius
                     }),
@@ -23462,61 +23789,61 @@
                     transitionDuration: "0ms"
                 }
             },
             label: {
                 color: e.white,
                 fontSize: .65 * e.fn.size({
                     size: n,
-                    sizes: Tz
+                    sizes: nC
                 }),
                 fontWeight: 700,
                 userSelect: "none",
                 overflow: "hidden",
                 whiteSpace: "nowrap"
             }
         })),
-        Rz = Object.defineProperty,
-        _z = Object.defineProperties,
-        Lz = Object.getOwnPropertyDescriptors,
-        Az = Object.getOwnPropertySymbols,
-        Mz = Object.prototype.hasOwnProperty,
-        Fz = Object.prototype.propertyIsEnumerable,
-        $z = (e, t, r) => t in e ? Rz(e, t, {
+        iC = Object.defineProperty,
+        lC = Object.defineProperties,
+        sC = Object.getOwnPropertyDescriptors,
+        cC = Object.getOwnPropertySymbols,
+        uC = Object.prototype.hasOwnProperty,
+        dC = Object.prototype.propertyIsEnumerable,
+        pC = (e, t, r) => t in e ? iC(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        Bz = (e, t) => {
-            for (var r in t || (t = {})) Mz.call(t, r) && $z(e, r, t[r]);
-            if (Az)
-                for (var r of Az(t)) Fz.call(t, r) && $z(e, r, t[r]);
+        fC = (e, t) => {
+            for (var r in t || (t = {})) uC.call(t, r) && pC(e, r, t[r]);
+            if (cC)
+                for (var r of cC(t)) dC.call(t, r) && pC(e, r, t[r]);
             return e
         };
 
-    function Wz(e) {
+    function mC(e) {
         return e.reduce((e, t) => {
             var r, n;
-            return e.sections.push((r = Bz({}, t), n = {
+            return e.sections.push((r = fC({}, t), n = {
                 accumulated: e.accumulated
-            }, _z(r, Lz(n)))), e.accumulated += t.value, e
+            }, lC(r, sC(n)))), e.accumulated += t.value, e
         }, {
             accumulated: 0,
             sections: []
         }).sections
     }
-    const Hz = {
+    const bC = {
             size: "md",
             radius: "sm",
             striped: !1,
             animate: !1,
             label: ""
         },
-        Vz = Object(n.forwardRef)((e, t) => {
-            const r = ir("Progress", Hz, e),
+        gC = Object(n.forwardRef)((e, t) => {
+            const r = ir("Progress", bC, e),
                 {
                     className: n,
                     value: o,
                     color: i,
                     size: l,
                     radius: s,
                     striped: c,
@@ -23525,46 +23852,46 @@
                     "aria-label": p,
                     classNames: f,
                     styles: m,
                     sections: b
                 } = r,
                 g = ((e, t) => {
                     var r = {};
-                    for (var n in e) Mz.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && Az)
-                        for (var n of Az(e)) t.indexOf(n) < 0 && Fz.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) uC.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && cC)
+                        for (var n of cC(e)) t.indexOf(n) < 0 && dC.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["className", "value", "color", "size", "radius", "striped", "animate", "label", "aria-label", "classNames", "styles", "sections"]),
                 {
                     classes: y,
                     cx: h,
                     theme: v
-                } = Iz({
+                } = oC({
                     color: i,
                     size: l,
                     radius: s,
                     striped: c || u,
                     animate: u
                 }, {
                     classNames: f,
                     styles: m,
                     name: "Progress"
                 }),
-                O = Array.isArray(b) ? Wz(b).map((e, t) => a.a.createElement(Cn, {
+                O = Array.isArray(b) ? mC(b).map((e, t) => a.a.createElement(Cn, {
                     key: t,
                     className: y.bar,
                     sx: {
                         width: e.value + "%",
                         left: e.accumulated + "%",
                         backgroundColor: v.fn.themeColor(e.color, 6, !1)
                     }
                 }, e.label && a.a.createElement(jo, {
                     className: y.label
                 }, e.label))) : null;
-            return a.a.createElement(Cn, Bz({
+            return a.a.createElement(Cn, fC({
                 className: h(y.root, n),
                 ref: t
             }, g), O || a.a.createElement("div", {
                 role: "progressbar",
                 "aria-valuemax": 100,
                 "aria-valuemin": 0,
                 "aria-valuenow": o,
@@ -23574,31 +23901,31 @@
                     width: o + "%"
                 }
             }, d ? a.a.createElement(jo, {
                 className: y.label
             }, d) : ""))
         });
 
-    function qz() {
-        return (qz = Object.assign || function(e) {
+    function yC() {
+        return (yC = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    Vz.displayName = "@mantine/core/Progress";
-    var Uz = function(e) {
+    gC.displayName = "@mantine/core/Progress";
+    var hC = function(e) {
         var t = e.class_name;
-        return a.a.createElement(Vz, qz({}, G(["setProps", "class_name"], e), {
+        return a.a.createElement(gC, yC({}, G(["setProps", "class_name"], e), {
             className: t
         }))
     };
-    Uz.displayName = "Progress", Uz.defaultProps = {}, Uz.propTypes = {
+    hC.displayName = "Progress", hC.defaultProps = {}, hC.propTypes = {
         animate: i.a.bool,
         class_name: i.a.string,
         color: i.a.oneOf(["dark", "gray", "red", "pink", "grape", "violet", "indigo", "blue", "cyan", "teal", "green", "lime", "yellow", "orange"]),
         label: i.a.string,
         id: i.a.string,
         radius: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         sections: i.a.arrayOf(i.a.exact({
@@ -23606,45 +23933,45 @@
             color: i.a.oneOf(["dark", "gray", "red", "pink", "grape", "violet", "indigo", "blue", "cyan", "teal", "green", "lime", "yellow", "orange"]),
             label: i.a.string
         })),
         size: i.a.oneOf(["xs", "sm", "md", "lg", "xl"]),
         striped: i.a.bool,
         value: i.a.number
     };
-    var Gz = Uz;
+    var vC = hC;
 
-    function Yz(e, t) {
+    function OC(e, t) {
         if (null == e) return {};
         var r, n, a = {},
             o = Object.keys(e);
         for (n = 0; n < o.length; n++) r = o[n], t.indexOf(r) >= 0 || (a[r] = e[r]);
         return a
     }
 
-    function Zz(e, t) {
-        return (Zz = Object.setPrototypeOf || function(e, t) {
+    function wC(e, t) {
+        return (wC = Object.setPrototypeOf || function(e, t) {
             return e.__proto__ = t, e
         })(e, t)
     }
 
-    function Kz(e, t) {
-        e.prototype = Object.create(t.prototype), e.prototype.constructor = e, Zz(e, t)
+    function xC(e, t) {
+        e.prototype = Object.create(t.prototype), e.prototype.constructor = e, wC(e, t)
     }
-    var Xz = !1,
-        Jz = a.a.createContext(null),
-        Qz = function(e) {
+    var SC = !1,
+        kC = a.a.createContext(null),
+        EC = function(e) {
             function t(t, r) {
                 var n;
                 n = e.call(this, t, r) || this;
                 var a, o = r && !r.isMounting ? t.enter : t.appear;
                 return n.appearStatus = null, t.in ? o ? (a = "exited", n.appearStatus = "entering") : a = "entered" : a = t.unmountOnExit || t.mountOnEnter ? "unmounted" : "exited", n.state = {
                     status: a
                 }, n.nextCallback = null, n
             }
-            Kz(t, e), t.getDerivedStateFromProps = function(e, t) {
+            xC(t, e), t.getDerivedStateFromProps = function(e, t) {
                 return e.in && "unmounted" === t.status ? {
                     status: "exited"
                 } : null
             };
             var r = t.prototype;
             return r.componentDidMount = function() {
                 this.updateStatus(!0, this.appearStatus)
@@ -23673,15 +24000,15 @@
                     r = this.props.enter,
                     n = this.context ? this.context.isMounting : e,
                     a = this.props.nodeRef ? [n] : [Au.a.findDOMNode(this), n],
                     o = a[0],
                     i = a[1],
                     l = this.getTimeouts(),
                     s = n ? l.appear : l.enter;
-                !e && !r || Xz ? this.safeSetState({
+                !e && !r || SC ? this.safeSetState({
                     status: "entered"
                 }, (function() {
                     t.props.onEntered(o)
                 })) : (this.props.onEnter(o, i), this.safeSetState({
                     status: "entering"
                 }, (function() {
                     t.props.onEntering(o, i), t.onTransitionEnd(s, (function() {
@@ -23693,15 +24020,15 @@
                     }))
                 })))
             }, r.performExit = function() {
                 var e = this,
                     t = this.props.exit,
                     r = this.getTimeouts(),
                     n = this.props.nodeRef ? void 0 : Au.a.findDOMNode(this);
-                t && !Xz ? (this.props.onExit(n), this.safeSetState({
+                t && !SC ? (this.props.onExit(n), this.safeSetState({
                     status: "exiting"
                 }, (function() {
                     e.props.onExiting(n), e.onTransitionEnd(r.exit, (function() {
                         e.safeSetState({
                             status: "exited"
                         }, (function() {
                             e.props.onExited(n)
@@ -23738,55 +24065,55 @@
                     null != e && setTimeout(this.nextCallback, e)
                 } else setTimeout(this.nextCallback, 0)
             }, r.render = function() {
                 var e = this.state.status;
                 if ("unmounted" === e) return null;
                 var t = this.props,
                     r = t.children,
-                    n = (t.in, t.mountOnEnter, t.unmountOnExit, t.appear, t.enter, t.exit, t.timeout, t.addEndListener, t.onEnter, t.onEntering, t.onEntered, t.onExit, t.onExiting, t.onExited, t.nodeRef, Yz(t, ["children", "in", "mountOnEnter", "unmountOnExit", "appear", "enter", "exit", "timeout", "addEndListener", "onEnter", "onEntering", "onEntered", "onExit", "onExiting", "onExited", "nodeRef"]));
-                return a.a.createElement(Jz.Provider, {
+                    n = (t.in, t.mountOnEnter, t.unmountOnExit, t.appear, t.enter, t.exit, t.timeout, t.addEndListener, t.onEnter, t.onEntering, t.onEntered, t.onExit, t.onExiting, t.onExited, t.nodeRef, OC(t, ["children", "in", "mountOnEnter", "unmountOnExit", "appear", "enter", "exit", "timeout", "addEndListener", "onEnter", "onEntering", "onEntered", "onExit", "onExiting", "onExited", "nodeRef"]));
+                return a.a.createElement(kC.Provider, {
                     value: null
                 }, "function" == typeof r ? r(e, n) : a.a.cloneElement(a.a.Children.only(r), n))
             }, t
         }(a.a.Component);
 
-    function eC() {}
-    Qz.contextType = Jz, Qz.propTypes = {}, Qz.defaultProps = {
+    function jC() {}
+    EC.contextType = kC, EC.propTypes = {}, EC.defaultProps = {
         in: !1,
         mountOnEnter: !1,
         unmountOnExit: !1,
         appear: !1,
         enter: !0,
         exit: !0,
-        onEnter: eC,
-        onEntering: eC,
-        onEntered: eC,
-        onExit: eC,
-        onExiting: eC,
-        onExited: eC
-    }, Qz.UNMOUNTED = "unmounted", Qz.EXITED = "exited", Qz.ENTERING = "entering", Qz.ENTERED = "entered", Qz.EXITING = "exiting";
-    var tC = Qz;
+        onEnter: jC,
+        onEntering: jC,
+        onEntered: jC,
+        onExit: jC,
+        onExiting: jC,
+        onExited: jC
+    }, EC.UNMOUNTED = "unmounted", EC.EXITED = "exited", EC.ENTERING = "entering", EC.ENTERED = "entered", EC.EXITING = "exiting";
+    var PC = EC;
 
-    function rC(e, t) {
+    function zC(e, t) {
         var r = Object.create(null);
         return e && n.Children.map(e, (function(e) {
             return e
         })).forEach((function(e) {
             r[e.key] = function(e) {
                 return t && Object(n.isValidElement)(e) ? t(e) : e
             }(e)
         })), r
     }
 
-    function nC(e, t, r) {
+    function CC(e, t, r) {
         return null != r[t] ? r[t] : e.props[t]
     }
 
-    function aC(e, t, r) {
-        var a = rC(e.children),
+    function NC(e, t, r) {
+        var a = zC(e.children),
             o = function(e, t) {
                 function r(r) {
                     return r in t ? t[r] : e[r]
                 }
                 e = e || {}, t = t || {};
                 var n, a = Object.create(null),
                     o = [];
@@ -23809,177 +24136,177 @@
                 var s = i in t,
                     c = i in a,
                     u = t[i],
                     d = Object(n.isValidElement)(u) && !u.props.in;
                 !c || s && !d ? c || !s || d ? c && s && Object(n.isValidElement)(u) && (o[i] = Object(n.cloneElement)(l, {
                     onExited: r.bind(null, l),
                     in: u.props.in,
-                    exit: nC(l, "exit", e),
-                    enter: nC(l, "enter", e)
+                    exit: CC(l, "exit", e),
+                    enter: CC(l, "enter", e)
                 })) : o[i] = Object(n.cloneElement)(l, {
                     in: !1
                 }) : o[i] = Object(n.cloneElement)(l, {
                     onExited: r.bind(null, l),
                     in: !0,
-                    exit: nC(l, "exit", e),
-                    enter: nC(l, "enter", e)
+                    exit: CC(l, "exit", e),
+                    enter: CC(l, "enter", e)
                 })
             }
         })), o
     }
-    var oC = Object.values || function(e) {
+    var TC = Object.values || function(e) {
             return Object.keys(e).map((function(t) {
                 return e[t]
             }))
         },
-        iC = function(e) {
+        DC = function(e) {
             function t(t, r) {
                 var n, a = (n = e.call(this, t, r) || this).handleExited.bind(function(e) {
                     if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                     return e
                 }(n));
                 return n.state = {
                     contextValue: {
                         isMounting: !0
                     },
                     handleExited: a,
                     firstRender: !0
                 }, n
             }
-            Kz(t, e);
+            xC(t, e);
             var r = t.prototype;
             return r.componentDidMount = function() {
                 this.mounted = !0, this.setState({
                     contextValue: {
                         isMounting: !1
                     }
                 })
             }, r.componentWillUnmount = function() {
                 this.mounted = !1
             }, t.getDerivedStateFromProps = function(e, t) {
                 var r, a, o = t.children,
                     i = t.handleExited;
                 return {
-                    children: t.firstRender ? (r = e, a = i, rC(r.children, (function(e) {
+                    children: t.firstRender ? (r = e, a = i, zC(r.children, (function(e) {
                         return Object(n.cloneElement)(e, {
                             onExited: a.bind(null, e),
                             in: !0,
-                            appear: nC(e, "appear", r),
-                            enter: nC(e, "enter", r),
-                            exit: nC(e, "exit", r)
+                            appear: CC(e, "appear", r),
+                            enter: CC(e, "enter", r),
+                            exit: CC(e, "exit", r)
                         })
-                    }))) : aC(e, o, i),
+                    }))) : NC(e, o, i),
                     firstRender: !1
                 }
             }, r.handleExited = function(e, t) {
-                var r = rC(this.props.children);
+                var r = zC(this.props.children);
                 e.key in r || (e.props.onExited && e.props.onExited(t), this.mounted && this.setState((function(t) {
                     var r = it({}, t.children);
                     return delete r[e.key], {
                         children: r
                     }
                 })))
             }, r.render = function() {
                 var e = this.props,
                     t = e.component,
                     r = e.childFactory,
-                    n = Yz(e, ["component", "childFactory"]),
+                    n = OC(e, ["component", "childFactory"]),
                     o = this.state.contextValue,
-                    i = oC(this.state.children).map(r);
-                return delete n.appear, delete n.enter, delete n.exit, null === t ? a.a.createElement(Jz.Provider, {
+                    i = TC(this.state.children).map(r);
+                return delete n.appear, delete n.enter, delete n.exit, null === t ? a.a.createElement(kC.Provider, {
                     value: o
-                }, i) : a.a.createElement(Jz.Provider, {
+                }, i) : a.a.createElement(kC.Provider, {
                     value: o
                 }, a.a.createElement(t, n, i))
             }, t
         }(a.a.Component);
-    iC.propTypes = {}, iC.defaultProps = {
+    DC.propTypes = {}, DC.defaultProps = {
         component: "div",
         childFactory: function(e) {
             return e
         }
     };
-    var lC = iC;
-    const sC = e => (e + 1) % 1e6;
-    const cC = Object(n.createContext)(null);
-    cC.displayName = "@mantine/notifications/NotificationsContext";
-    const uC = {
+    var IC = DC;
+    const RC = e => (e + 1) % 1e6;
+    const _C = Object(n.createContext)(null);
+    _C.displayName = "@mantine/notifications/NotificationsContext";
+    const LC = {
         show: "mantine:show-notification",
         hide: "mantine:hide-notification",
         update: "mantine:update-notification",
         clean: "mantine:clean-notifications",
         cleanQueue: "mantine:clean-notifications-queue"
     };
 
-    function dC(e, t) {
+    function AC(e, t) {
         return new CustomEvent(e, {
             detail: t
         })
     }
-    var pC = function([e, t], r, n) {
+    var MC = function([e, t], r, n) {
             const a = {};
             return "top" === e && (a.top = n), "bottom" === e && (a.bottom = n), "left" === t && (a.left = n), "right" === t && (a.right = n), "center" === t && (a.left = "50%", a.transform = "translateX(-50%)"), a
         },
-        fC = Object.defineProperty,
-        mC = Object.getOwnPropertySymbols,
-        bC = Object.prototype.hasOwnProperty,
-        gC = Object.prototype.propertyIsEnumerable,
-        yC = (e, t, r) => t in e ? fC(e, t, {
+        FC = Object.defineProperty,
+        $C = Object.getOwnPropertySymbols,
+        BC = Object.prototype.hasOwnProperty,
+        WC = Object.prototype.propertyIsEnumerable,
+        HC = (e, t, r) => t in e ? FC(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        hC = (e, t) => {
-            for (var r in t || (t = {})) bC.call(t, r) && yC(e, r, t[r]);
-            if (mC)
-                for (var r of mC(t)) gC.call(t, r) && yC(e, r, t[r]);
+        VC = (e, t) => {
+            for (var r in t || (t = {})) BC.call(t, r) && HC(e, r, t[r]);
+            if ($C)
+                for (var r of $C(t)) WC.call(t, r) && HC(e, r, t[r]);
             return e
         };
-    const vC = {
+    const qC = {
             left: "translateX(-100%)",
             right: "translateX(100%)",
             "top-center": "translateY(-100%)",
             "bottom-center": "translateY(100%)"
         },
-        OC = {
+        UC = {
             left: "translateX(0)",
             right: "translateX(0)",
             "top-center": "translateY(0)",
             "bottom-center": "translateY(0)"
         };
-    var wC = function({
+    var GC = function({
             state: e,
             maxHeight: t,
             positioning: r,
             transitionDuration: n
         }) {
             const [a, o] = r, i = "center" === o ? a + "-center" : o, l = {
                 opacity: 1,
-                transform: OC[i]
+                transform: UC[i]
             }, s = {
                 opacity: 0,
                 maxHeight: 0,
-                transform: vC[i]
+                transform: qC[i]
             }, c = {
                 entering: l,
                 entered: l,
                 exiting: s,
                 exited: s
             };
-            return hC(hC({}, {
+            return VC(VC({}, {
                 opacity: 0,
                 maxHeight: t,
-                transform: vC[i],
+                transform: qC[i],
                 transitionDuration: `${n}ms, ${n}ms, ${n}ms`,
                 transitionTimingFunction: "cubic-bezier(.51,.3,0,1.21), cubic-bezier(.51,.3,0,1.21), linear",
                 transitionProperty: "opacity, transform, max-height"
             }), c[e])
         },
-        xC = Er((e, {
+        YC = Er((e, {
             color: t,
             radius: r,
             disallowClose: n
         }, a) => {
             const o = e.fn.radius(r),
                 i = Math.min(Math.max(o / 1.2, 4), 30);
             return {
@@ -24053,33 +24380,33 @@
                     textOverflow: "ellipsis",
                     "&:only-child": {
                         color: "dark" === e.colorScheme ? e.colors.dark[0] : e.black
                     }
                 }
             }
         }),
-        SC = Object.defineProperty,
-        kC = Object.defineProperties,
-        EC = Object.getOwnPropertyDescriptors,
-        jC = Object.getOwnPropertySymbols,
-        PC = Object.prototype.hasOwnProperty,
-        zC = Object.prototype.propertyIsEnumerable,
-        CC = (e, t, r) => t in e ? SC(e, t, {
+        ZC = Object.defineProperty,
+        KC = Object.defineProperties,
+        XC = Object.getOwnPropertyDescriptors,
+        JC = Object.getOwnPropertySymbols,
+        QC = Object.prototype.hasOwnProperty,
+        eN = Object.prototype.propertyIsEnumerable,
+        tN = (e, t, r) => t in e ? ZC(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        NC = (e, t) => {
-            for (var r in t || (t = {})) PC.call(t, r) && CC(e, r, t[r]);
-            if (jC)
-                for (var r of jC(t)) zC.call(t, r) && CC(e, r, t[r]);
+        rN = (e, t) => {
+            for (var r in t || (t = {})) QC.call(t, r) && tN(e, r, t[r]);
+            if (JC)
+                for (var r of JC(t)) eN.call(t, r) && tN(e, r, t[r]);
             return e
         };
-    const TC = Object(n.forwardRef)((e, t) => {
+    const nN = Object(n.forwardRef)((e, t) => {
         const r = ir("Notification", {}, e),
             {
                 className: n,
                 color: o,
                 radius: i,
                 loading: l,
                 disallowClose: s,
@@ -24089,33 +24416,33 @@
                 onClose: p,
                 closeButtonProps: f,
                 classNames: m,
                 styles: b
             } = r,
             g = ((e, t) => {
                 var r = {};
-                for (var n in e) PC.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                if (null != e && jC)
-                    for (var n of jC(e)) t.indexOf(n) < 0 && zC.call(e, n) && (r[n] = e[n]);
+                for (var n in e) QC.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                if (null != e && JC)
+                    for (var n of JC(e)) t.indexOf(n) < 0 && eN.call(e, n) && (r[n] = e[n]);
                 return r
             })(r, ["className", "color", "radius", "loading", "disallowClose", "title", "icon", "children", "onClose", "closeButtonProps", "classNames", "styles"]),
             {
                 classes: y,
                 cx: h
-            } = xC({
+            } = YC({
                 color: o,
                 radius: i,
                 disallowClose: s
             }, {
                 classNames: m,
                 styles: b,
                 name: "Notification"
             }),
             v = u || l;
-        return a.a.createElement(Cn, NC({
+        return a.a.createElement(Cn, rN({
             className: h(y.root, {
                 [y.withIcon]: v
             }, n),
             role: "alert",
             ref: t
         }, g), u && !l && a.a.createElement("div", {
             className: y.icon
@@ -24129,122 +24456,122 @@
             className: y.title,
             size: "sm",
             weight: 500
         }, c), a.a.createElement(jo, {
             color: "dimmed",
             className: y.description,
             size: "sm"
-        }, d)), !s && a.a.createElement(yc, (O = NC({}, f), w = {
+        }, d)), !s && a.a.createElement(yc, (O = rN({}, f), w = {
             iconSize: 16,
             color: "gray",
             onClick: p,
             variant: "hover",
             className: y.closeButton
-        }, kC(O, EC(w)))));
+        }, KC(O, XC(w)))));
         var O, w
     });
-    TC.displayName = "@mantine/core/Notification";
-    var DC = function(e, t) {
+    nN.displayName = "@mantine/core/Notification";
+    var aN = function(e, t) {
             return "number" == typeof t ? t : !1 !== t && !1 !== e && e
         },
-        IC = Object.defineProperty,
-        RC = Object.defineProperties,
-        _C = Object.getOwnPropertyDescriptors,
-        LC = Object.getOwnPropertySymbols,
-        AC = Object.prototype.hasOwnProperty,
-        MC = Object.prototype.propertyIsEnumerable,
-        FC = (e, t, r) => t in e ? IC(e, t, {
+        oN = Object.defineProperty,
+        iN = Object.defineProperties,
+        lN = Object.getOwnPropertyDescriptors,
+        sN = Object.getOwnPropertySymbols,
+        cN = Object.prototype.hasOwnProperty,
+        uN = Object.prototype.propertyIsEnumerable,
+        dN = (e, t, r) => t in e ? oN(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        $C = (e, t) => {
-            for (var r in t || (t = {})) AC.call(t, r) && FC(e, r, t[r]);
-            if (LC)
-                for (var r of LC(t)) MC.call(t, r) && FC(e, r, t[r]);
+        pN = (e, t) => {
+            for (var r in t || (t = {})) cN.call(t, r) && dN(e, r, t[r]);
+            if (sN)
+                for (var r of sN(t)) uN.call(t, r) && dN(e, r, t[r]);
             return e
         },
-        BC = (e, t) => {
+        fN = (e, t) => {
             var r = {};
-            for (var n in e) AC.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-            if (null != e && LC)
-                for (var n of LC(e)) t.indexOf(n) < 0 && MC.call(e, n) && (r[n] = e[n]);
+            for (var n in e) cN.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+            if (null != e && sN)
+                for (var n of sN(e)) t.indexOf(n) < 0 && uN.call(e, n) && (r[n] = e[n]);
             return r
         };
 
-    function WC(e) {
+    function mN(e) {
         var t = e,
             {
                 notification: r,
                 autoClose: o,
                 onHide: i,
                 innerRef: l
             } = t,
-            s = BC(t, ["notification", "autoClose", "onHide", "innerRef"]);
+            s = fN(t, ["notification", "autoClose", "onHide", "innerRef"]);
         const c = r,
             {
                 autoClose: u
             } = c,
-            d = BC(c, ["autoClose"]),
-            p = DC(o, u),
+            d = fN(c, ["autoClose"]),
+            p = aN(o, u),
             f = Object(n.useRef)(),
             m = () => {
                 i(r.id), window.clearTimeout(f.current)
             },
             b = () => {
                 clearTimeout(f.current)
             },
             g = () => {
                 "number" == typeof p && (f.current = window.setTimeout(m, p))
             };
         return Object(n.useEffect)(() => {
             "function" == typeof r.onOpen && r.onOpen(r)
-        }, []), Object(n.useEffect)(() => (g(), b), [o, r.autoClose]), a.a.createElement(TC, (y = $C($C({}, d), s), RC(y, _C({
+        }, []), Object(n.useEffect)(() => (g(), b), [o, r.autoClose]), a.a.createElement(nN, (y = pN(pN({}, d), s), iN(y, lN({
             onClose: m,
             onMouseEnter: b,
             onMouseLeave: g,
             ref: l
         }))), r.message);
         var y
     }
-    WC.displayName = "@mantine/notifications/NotificationContainer";
-    var HC = WC,
-        VC = Er(e => ({
+    mN.displayName = "@mantine/notifications/NotificationContainer";
+    var bN = mN,
+        gN = Er(e => ({
             notifications: {
                 width: `calc(100% - ${2*e.spacing.md}px)`,
                 boxSizing: "border-box",
                 position: "fixed",
                 zIndex: 1e3
             },
             notification: {
                 "&:not(:first-of-type)": {
                     marginTop: e.spacing.sm
                 }
             }
         }));
-    var qC = Object.defineProperty,
-        UC = Object.defineProperties,
-        GC = Object.getOwnPropertyDescriptors,
-        YC = Object.getOwnPropertySymbols,
-        ZC = Object.prototype.hasOwnProperty,
-        KC = Object.prototype.propertyIsEnumerable,
-        XC = (e, t, r) => t in e ? qC(e, t, {
+    var yN = Object.defineProperty,
+        hN = Object.defineProperties,
+        vN = Object.getOwnPropertyDescriptors,
+        ON = Object.getOwnPropertySymbols,
+        wN = Object.prototype.hasOwnProperty,
+        xN = Object.prototype.propertyIsEnumerable,
+        SN = (e, t, r) => t in e ? yN(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        JC = (e, t) => {
-            for (var r in t || (t = {})) ZC.call(t, r) && XC(e, r, t[r]);
-            if (YC)
-                for (var r of YC(t)) KC.call(t, r) && XC(e, r, t[r]);
+        kN = (e, t) => {
+            for (var r in t || (t = {})) wN.call(t, r) && SN(e, r, t[r]);
+            if (ON)
+                for (var r of ON(t)) xN.call(t, r) && SN(e, r, t[r]);
             return e
         };
-    var QC = function({
+    var EN = function({
             limit: e
         }) {
             const {
                 state: t,
                 queue: r,
                 update: a,
                 cleanQueue: o
@@ -24287,50 +24614,50 @@
             });
             return {
                 notifications: t,
                 queue: r,
                 showNotification: e => {
                     const t = e.id || Xa();
                     return a(r => {
-                        return e.id && r.some(t => t.id === e.id) ? r : [...r, (n = JC({}, e), a = {
+                        return e.id && r.some(t => t.id === e.id) ? r : [...r, (n = kN({}, e), a = {
                             id: t
-                        }, UC(n, GC(a)))];
+                        }, hN(n, vN(a)))];
                         var n, a
                     }), t
                 },
                 updateNotification: (e, t) => a(r => {
                     const n = r.findIndex(t => t.id === e);
                     if (-1 === n) return r;
                     const a = [...r];
                     return a[n] = t, a
                 }),
                 hideNotification: e => a(t => t.filter(t => t.id !== e || ("function" == typeof t.onClose && t.onClose(t), !1))),
                 cleanQueue: o,
                 clean: () => a(() => [])
             }
         },
-        eN = Object.defineProperty,
-        tN = Object.getOwnPropertySymbols,
-        rN = Object.prototype.hasOwnProperty,
-        nN = Object.prototype.propertyIsEnumerable,
-        aN = (e, t, r) => t in e ? eN(e, t, {
+        jN = Object.defineProperty,
+        PN = Object.getOwnPropertySymbols,
+        zN = Object.prototype.hasOwnProperty,
+        CN = Object.prototype.propertyIsEnumerable,
+        NN = (e, t, r) => t in e ? jN(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        oN = (e, t) => {
-            for (var r in t || (t = {})) rN.call(t, r) && aN(e, r, t[r]);
-            if (tN)
-                for (var r of tN(t)) nN.call(t, r) && aN(e, r, t[r]);
+        TN = (e, t) => {
+            for (var r in t || (t = {})) zN.call(t, r) && NN(e, r, t[r]);
+            if (PN)
+                for (var r of PN(t)) CN.call(t, r) && NN(e, r, t[r]);
             return e
         };
-    const iN = ["top-left", "top-right", "top-center", "bottom-left", "bottom-right", "bottom-center"];
+    const DN = ["top-left", "top-right", "top-center", "bottom-left", "bottom-right", "bottom-center"];
 
-    function lN(e) {
+    function IN(e) {
         var t = e,
             {
                 className: r,
                 position: o = "bottom-right",
                 autoClose: i = 4e3,
                 transitionDuration: l = 250,
                 containerWidth: s = 440,
@@ -24338,43 +24665,43 @@
                 limit: u = 5,
                 zIndex: d = ac("overlay"),
                 style: p,
                 children: f
             } = t,
             m = ((e, t) => {
                 var r = {};
-                for (var n in e) rN.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                if (null != e && tN)
-                    for (var n of tN(e)) t.indexOf(n) < 0 && nN.call(e, n) && (r[n] = e[n]);
+                for (var n in e) zN.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                if (null != e && PN)
+                    for (var n of PN(e)) t.indexOf(n) < 0 && CN.call(e, n) && (r[n] = e[n]);
                 return r
             })(t, ["className", "position", "autoClose", "transitionDuration", "containerWidth", "notificationMaxHeight", "limit", "zIndex", "style", "children"]);
         const b = function() {
-                const [, e] = Object(n.useReducer)(sC, 0);
+                const [, e] = Object(n.useReducer)(RC, 0);
                 return e
             }(),
             g = Object(n.useRef)({}),
             y = Object(n.useRef)(0),
             {
                 notifications: h,
                 queue: v,
                 showNotification: O,
                 updateNotification: w,
                 hideNotification: x,
                 clean: S,
                 cleanQueue: k
-            } = QC({
+            } = EN({
                 limit: u
             }),
             E = vd() ? 1 : l,
             {
                 classes: j,
                 cx: P,
                 theme: z
-            } = VC(),
-            C = (iN.includes(o) ? o : "bottom-right").split("-"),
+            } = gN(),
+            C = (DN.includes(o) ? o : "bottom-right").split("-"),
             N = {
                 notifications: h,
                 queue: v,
                 showNotification: O,
                 hideNotification: x,
                 updateNotification: w,
                 clean: S,
@@ -24388,207 +24715,207 @@
                     show: t => e.showNotification(t.detail),
                     hide: t => e.hideNotification(t.detail),
                     update: t => e.updateNotification(t.detail.id, t.detail),
                     clean: e.clean,
                     cleanQueue: e.cleanQueue
                 };
                 Object(n.useEffect)(() => (Object.keys(t).forEach(e => {
-                    window.addEventListener(uC[e], t[e])
+                    window.addEventListener(LC[e], t[e])
                 }), () => {
                     Object.keys(t).forEach(e => {
-                        window.removeEventListener(uC[e], t[e])
+                        window.removeEventListener(LC[e], t[e])
                     })
                 }), [])
             }(N);
-        const T = h.map(e => a.a.createElement(tC, {
+        const T = h.map(e => a.a.createElement(PC, {
             key: e.id,
             timeout: E,
             onEnter: () => g.current[e.id].offsetHeight,
             nodeRef: {
                 current: g.current[e.id]
             }
-        }, t => a.a.createElement(HC, {
+        }, t => a.a.createElement(bN, {
             innerRef: t => {
                 g.current[e.id] = t
             },
             notification: e,
             onHide: x,
             className: j.notification,
             autoClose: i,
-            sx: [oN({}, wC({
+            sx: [TN({}, GC({
                 state: t,
                 positioning: C,
                 transitionDuration: E,
                 maxHeight: c
             })), ...Array.isArray(e.sx) ? e.sx : [e.sx]]
         })));
-        return a.a.createElement(cC.Provider, {
+        return a.a.createElement(_C.Provider, {
             value: N
         }, a.a.createElement(Fu, {
             zIndex: d
-        }, a.a.createElement(Cn, oN({
+        }, a.a.createElement(Cn, TN({
             className: P(j.notifications, r),
             style: p,
-            sx: oN({
+            sx: TN({
                 maxWidth: s
-            }, pC(C, s, z.spacing.md))
-        }, m), a.a.createElement(lC, null, T))), f)
+            }, MC(C, s, z.spacing.md))
+        }, m), a.a.createElement(IC, null, T))), f)
     }
-    lN.displayName = "@mantine/notifications/NotificationsProvider";
-    var sN = function(e) {
-        return a.a.createElement(lN, G(["setProps", "children"], e), e.children)
+    IN.displayName = "@mantine/notifications/NotificationsProvider";
+    var RN = function(e) {
+        return a.a.createElement(IN, G(["setProps", "children"], e), e.children)
     };
-    sN.displayName = "NotificationsProvider", sN.defaultProps = {}, sN.propTypes = {
+    RN.displayName = "NotificationsProvider", RN.defaultProps = {}, RN.propTypes = {
         autoClose: i.a.oneOfType([i.a.number, i.a.oneOf([!1])]),
         children: i.a.node,
         containerWidth: i.a.number,
         id: i.a.string,
         limit: i.a.number,
         notificationMaxHeight: i.a.number,
         position: i.a.oneOf(["top-left", "top-right", "top-center", "bottom-left", "bottom-right", "bottom-center"]),
         transitionDuration: i.a.number,
         zIndex: i.a.number
     };
-    var cN = sN,
-        uN = function(e) {
+    var _N = RN,
+        LN = function(e) {
             var t = e.action,
                 r = e.autoClose,
                 o = e.color,
                 i = e.disallowClose,
                 l = e.icon,
                 s = e.id,
                 c = e.loading,
                 u = e.message,
                 d = e.radius,
                 p = e.title;
             return Object(n.useEffect)((function() {
                 var t, r = ta(G(["setProps", "children"], e), ["icon", "title", "message"]);
                 switch (r.action) {
                     case "show":
-                        t = r, window.dispatchEvent(dC(uC.show, t));
+                        t = r, window.dispatchEvent(AC(LC.show, t));
                         break;
                     case "update":
                         ! function(e) {
-                            window.dispatchEvent(dC(uC.update, e))
+                            window.dispatchEvent(AC(LC.update, e))
                         }(r);
                         break;
                     case "hide":
                         ! function(e) {
-                            window.dispatchEvent(dC(uC.hide, e))
+                            window.dispatchEvent(AC(LC.hide, e))
                         }(r.id)
                 }
             }), [t, r, o, i, l, s, c, u, d, p]), a.a.createElement("div", null)
         };
-    uN.displayName = "Notification", uN.defaultProps = {}, uN.propTypes = {
+    LN.displayName = "Notification", LN.defaultProps = {}, LN.propTypes = {
         action: i.a.oneOf(["show", "update", "hide"]).isRequired,
         autoClose: i.a.oneOfType([i.a.bool, i.a.number]),
         color: i.a.oneOf(["dark", "gray", "red", "pink", "grape", "violet", "indigo", "blue", "cyan", "teal", "green", "lime", "yellow", "orange"]),
         disallowClose: i.a.bool,
         icon: i.a.any,
         id: i.a.string.isRequired,
         loading: i.a.bool,
         message: i.a.any,
         radius: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         title: i.a.any
     };
-    var dN = uN;
+    var AN = LN;
 
-    function pN() {
-        return (pN = Object.assign || function(e) {
+    function MN() {
+        return (MN = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    var fN = function(e) {
+    var FN = function(e) {
         var t = e.class_name;
-        return a.a.createElement(ag, pN({}, G(["setProps", "children", "class_name"], e), {
+        return a.a.createElement(ag, MN({}, G(["setProps", "children", "class_name"], e), {
             className: t
         }), e.children)
     };
-    fN.displayName = "ScrollArea", fN.defaultProps = {}, fN.propTypes = {
+    FN.displayName = "ScrollArea", FN.defaultProps = {}, FN.propTypes = {
         children: i.a.node,
         class_name: i.a.string,
         dir: i.a.oneOf(["ltr", "rtl"]),
         id: i.a.string,
         offsetScrollbars: i.a.bool,
         scrollHideDelay: i.a.number,
         scrollbarSize: i.a.number,
         setProps: i.a.func,
         style: i.a.object,
         type: i.a.oneOf(["auto", "scroll", "always", "hover"])
     };
-    var mN = fN;
+    var $N = FN;
 
-    function bN({
+    function BN({
         styles: e
     }) {
         const t = or();
         return a.a.createElement(jt, {
             styles: Pt("function" == typeof e ? e(t) : e)
         })
     }
-    const gN = Object(n.createContext)({});
-    gN.Provider;
+    const WN = Object(n.createContext)({});
+    WN.Provider;
 
-    function yN() {
-        return Object(n.useContext)(gN)
+    function HN() {
+        return Object(n.useContext)(WN)
     }
-    var hN = Object.defineProperty,
-        vN = Object.defineProperties,
-        ON = Object.getOwnPropertyDescriptors,
-        wN = Object.getOwnPropertySymbols,
-        xN = Object.prototype.hasOwnProperty,
-        SN = Object.prototype.propertyIsEnumerable,
-        kN = (e, t, r) => t in e ? hN(e, t, {
+    var VN = Object.defineProperty,
+        qN = Object.defineProperties,
+        UN = Object.getOwnPropertyDescriptors,
+        GN = Object.getOwnPropertySymbols,
+        YN = Object.prototype.hasOwnProperty,
+        ZN = Object.prototype.propertyIsEnumerable,
+        KN = (e, t, r) => t in e ? VN(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        EN = (e, t) => {
-            for (var r in t || (t = {})) xN.call(t, r) && kN(e, r, t[r]);
-            if (wN)
-                for (var r of wN(t)) SN.call(t, r) && kN(e, r, t[r]);
+        XN = (e, t) => {
+            for (var r in t || (t = {})) YN.call(t, r) && KN(e, r, t[r]);
+            if (GN)
+                for (var r of GN(t)) ZN.call(t, r) && KN(e, r, t[r]);
             return e
         },
-        jN = Er((e, {
+        JN = Er((e, {
             height: t,
             fixed: r,
             position: n,
             zIndex: a,
             borderPosition: o
         }) => {
             return {
-                root: (i = EN(EN({}, e.fn.fontStyles()), n), l = {
+                root: (i = XN(XN({}, e.fn.fontStyles()), n), l = {
                     zIndex: a,
                     height: t,
                     maxHeight: t,
                     position: r ? "fixed" : "static",
                     boxSizing: "border-box",
                     backgroundColor: "dark" === e.colorScheme ? e.colors.dark[7] : e.white,
                     borderBottom: "bottom" === o ? "1px solid " + ("dark" === e.colorScheme ? e.colors.dark[5] : e.colors.gray[2]) : void 0,
                     borderTop: "top" === o ? "1px solid " + ("dark" === e.colorScheme ? e.colors.dark[5] : e.colors.gray[2]) : void 0
-                }, vN(i, ON(l)))
+                }, qN(i, UN(l)))
             };
             var i, l
         }),
-        PN = Object.defineProperty,
-        zN = Object.getOwnPropertySymbols,
-        CN = Object.prototype.hasOwnProperty,
-        NN = Object.prototype.propertyIsEnumerable,
-        TN = (e, t, r) => t in e ? PN(e, t, {
+        QN = Object.defineProperty,
+        eT = Object.getOwnPropertySymbols,
+        tT = Object.prototype.hasOwnProperty,
+        rT = Object.prototype.propertyIsEnumerable,
+        nT = (e, t, r) => t in e ? QN(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const DN = Object(n.forwardRef)((e, t) => {
+    const aT = Object(n.forwardRef)((e, t) => {
         var r = e,
             {
                 children: n,
                 className: o,
                 classNames: i,
                 styles: l,
                 height: s,
@@ -24596,105 +24923,105 @@
                 position: u,
                 zIndex: d = ac("app"),
                 section: p,
                 __staticSelector: f
             } = r,
             m = ((e, t) => {
                 var r = {};
-                for (var n in e) CN.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                if (null != e && zN)
-                    for (var n of zN(e)) t.indexOf(n) < 0 && NN.call(e, n) && (r[n] = e[n]);
+                for (var n in e) tT.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                if (null != e && eT)
+                    for (var n of eT(e)) t.indexOf(n) < 0 && rT.call(e, n) && (r[n] = e[n]);
                 return r
             })(r, ["children", "className", "classNames", "styles", "height", "fixed", "position", "zIndex", "section", "__staticSelector"]);
-        const b = yN(),
+        const b = HN(),
             {
                 classes: g,
                 cx: y
-            } = jN({
+            } = JN({
                 height: s,
                 fixed: b.fixed || c,
                 position: u,
                 zIndex: b.zIndex || d,
                 borderPosition: "header" === p ? "bottom" : "top"
             }, {
                 name: f,
                 classNames: i,
                 styles: l
             });
         return a.a.createElement(Cn, ((e, t) => {
-            for (var r in t || (t = {})) CN.call(t, r) && TN(e, r, t[r]);
-            if (zN)
-                for (var r of zN(t)) NN.call(t, r) && TN(e, r, t[r]);
+            for (var r in t || (t = {})) tT.call(t, r) && nT(e, r, t[r]);
+            if (eT)
+                for (var r of eT(t)) rT.call(t, r) && nT(e, r, t[r]);
             return e
         })({
             component: "header" === p ? "nav" : "footer",
             className: y(g.root, o),
             ref: t
-        }, m), n, a.a.createElement(bN, {
+        }, m), n, a.a.createElement(BN, {
             styles: () => ({
                 ":root": {
                     [`--mantine-${p}-height`]: s + "px"
                 }
             })
         }))
     });
-    DN.displayName = "@mantine/core/VerticalSection";
-    var IN = Object.defineProperty,
-        RN = Object.defineProperties,
-        _N = Object.getOwnPropertyDescriptors,
-        LN = Object.getOwnPropertySymbols,
-        AN = Object.prototype.hasOwnProperty,
-        MN = Object.prototype.propertyIsEnumerable,
-        FN = (e, t, r) => t in e ? IN(e, t, {
+    aT.displayName = "@mantine/core/VerticalSection";
+    var oT = Object.defineProperty,
+        iT = Object.defineProperties,
+        lT = Object.getOwnPropertyDescriptors,
+        sT = Object.getOwnPropertySymbols,
+        cT = Object.prototype.hasOwnProperty,
+        uT = Object.prototype.propertyIsEnumerable,
+        dT = (e, t, r) => t in e ? oT(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const $N = {
+    const pT = {
             fixed: !1,
             position: {
                 top: 0,
                 left: 0,
                 right: 0
             },
             zIndex: ac("app")
         },
-        BN = Object(n.forwardRef)((e, t) => {
-            const r = ir("Header", $N, e);
-            return a.a.createElement(DN, ((e, t) => RN(e, _N(t)))(((e, t) => {
-                for (var r in t || (t = {})) AN.call(t, r) && FN(e, r, t[r]);
-                if (LN)
-                    for (var r of LN(t)) MN.call(t, r) && FN(e, r, t[r]);
+        fT = Object(n.forwardRef)((e, t) => {
+            const r = ir("Header", pT, e);
+            return a.a.createElement(aT, ((e, t) => iT(e, lT(t)))(((e, t) => {
+                for (var r in t || (t = {})) cT.call(t, r) && dT(e, r, t[r]);
+                if (sT)
+                    for (var r of sT(t)) uT.call(t, r) && dT(e, r, t[r]);
                 return e
             })({
                 section: "header",
                 __staticSelector: "Header"
             }, r), {
                 ref: t
             }))
         });
 
-    function WN() {
-        return (WN = Object.assign || function(e) {
+    function mT() {
+        return (mT = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    BN.displayName = "@mantine/core/Header";
-    var HN = function(e) {
+    fT.displayName = "@mantine/core/Header";
+    var bT = function(e) {
         var t = e.class_name;
-        return a.a.createElement(BN, WN({}, G(["setProps", "children", "class_name"], e), {
+        return a.a.createElement(fT, mT({}, G(["setProps", "children", "class_name"], e), {
             className: t
         }), e.children)
     };
-    HN.displayName = "Header", HN.defaultProps = {}, HN.propTypes = {
+    bT.displayName = "Header", bT.defaultProps = {}, bT.propTypes = {
         children: i.a.node,
         class_name: i.a.string,
         fixed: i.a.bool,
         height: i.a.oneOfType([i.a.string, i.a.number]),
         id: i.a.string,
         position: i.a.exact({
             top: i.a.number,
@@ -24715,132 +25042,132 @@
         py: i.a.oneOfType([i.a.string, i.a.number]),
         px: i.a.oneOfType([i.a.string, i.a.number]),
         pt: i.a.oneOfType([i.a.string, i.a.number]),
         pb: i.a.oneOfType([i.a.string, i.a.number]),
         pl: i.a.oneOfType([i.a.string, i.a.number]),
         pr: i.a.oneOfType([i.a.string, i.a.number])
     };
-    var VN = HN;
+    var gT = bT;
 
-    function qN(e, t) {
+    function yT(e, t) {
         if (!e) return [];
         const r = Object.keys(e).filter(e => "base" !== e).map(r => [t.fn.size({
             size: r,
             sizes: t.breakpoints
         }), e[r]]);
         return r.sort((e, t) => e[0] - t[0]), r
     }
-    var UN = Object.defineProperty,
-        GN = Object.getOwnPropertySymbols,
-        YN = Object.prototype.hasOwnProperty,
-        ZN = Object.prototype.propertyIsEnumerable,
-        KN = (e, t, r) => t in e ? UN(e, t, {
+    var hT = Object.defineProperty,
+        vT = Object.getOwnPropertySymbols,
+        OT = Object.prototype.hasOwnProperty,
+        wT = Object.prototype.propertyIsEnumerable,
+        xT = (e, t, r) => t in e ? hT(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const XN = Object(n.forwardRef)((e, t) => {
+    const ST = Object(n.forwardRef)((e, t) => {
         var r = e,
             {
                 component: n,
                 children: o,
                 grow: i = !1,
                 sx: l
             } = r,
             s = ((e, t) => {
                 var r = {};
-                for (var n in e) YN.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                if (null != e && GN)
-                    for (var n of GN(e)) t.indexOf(n) < 0 && ZN.call(e, n) && (r[n] = e[n]);
+                for (var n in e) OT.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                if (null != e && vT)
+                    for (var n of vT(e)) t.indexOf(n) < 0 && wT.call(e, n) && (r[n] = e[n]);
                 return r
             })(r, ["component", "children", "grow", "sx"]);
         return a.a.createElement(Cn, ((e, t) => {
-            for (var r in t || (t = {})) YN.call(t, r) && KN(e, r, t[r]);
-            if (GN)
-                for (var r of GN(t)) ZN.call(t, r) && KN(e, r, t[r]);
+            for (var r in t || (t = {})) OT.call(t, r) && xT(e, r, t[r]);
+            if (vT)
+                for (var r of vT(t)) wT.call(t, r) && xT(e, r, t[r]);
             return e
         })({
             component: n || "div",
             ref: t,
             sx: [{
                 flex: i ? 1 : 0,
                 boxSizing: "border-box"
             }, ...Array.isArray(l) ? l : [l]]
         }, s), o)
     });
-    XN.displayName = "@mantine/core/Section";
-    var JN = Object.defineProperty,
-        QN = Object.defineProperties,
-        eT = Object.getOwnPropertyDescriptors,
-        tT = Object.getOwnPropertySymbols,
-        rT = Object.prototype.hasOwnProperty,
-        nT = Object.prototype.propertyIsEnumerable,
-        aT = (e, t, r) => t in e ? JN(e, t, {
+    ST.displayName = "@mantine/core/Section";
+    var kT = Object.defineProperty,
+        ET = Object.defineProperties,
+        jT = Object.getOwnPropertyDescriptors,
+        PT = Object.getOwnPropertySymbols,
+        zT = Object.prototype.hasOwnProperty,
+        CT = Object.prototype.propertyIsEnumerable,
+        NT = (e, t, r) => t in e ? kT(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        oT = (e, t) => {
-            for (var r in t || (t = {})) rT.call(t, r) && aT(e, r, t[r]);
-            if (tT)
-                for (var r of tT(t)) nT.call(t, r) && aT(e, r, t[r]);
+        TT = (e, t) => {
+            for (var r in t || (t = {})) zT.call(t, r) && NT(e, r, t[r]);
+            if (PT)
+                for (var r of PT(t)) CT.call(t, r) && NT(e, r, t[r]);
             return e
         },
-        iT = Er((e, {
+        DT = Er((e, {
             height: t,
             width: r,
             fixed: n,
             position: a,
             hiddenBreakpoint: o,
             zIndex: i
         }) => {
-            const l = "object" == typeof r && null !== r ? qN(r, e).reduce((e, [t, r]) => (e[`@media (min-width: ${t+1}px)`] = {
+            const l = "object" == typeof r && null !== r ? yT(r, e).reduce((e, [t, r]) => (e[`@media (min-width: ${t+1}px)`] = {
                 width: r,
                 minWidth: r
             }, e), {}) : null;
             return {
-                root: oT((s = oT(oT({}, e.fn.fontStyles()), a), c = {
+                root: TT((s = TT(TT({}, e.fn.fontStyles()), a), c = {
                     top: (null == a ? void 0 : a.top) || "var(--mantine-header-height)",
                     zIndex: i,
                     height: t || "calc(100vh - var(--mantine-header-height, 0px) - var(--mantine-footer-height, 0px))",
                     width: (null == r ? void 0 : r.base) || "100%",
                     position: n ? "fixed" : "static",
                     boxSizing: "border-box",
                     display: "flex",
                     flexDirection: "column",
                     backgroundColor: "dark" === e.colorScheme ? e.colors.dark[7] : e.white,
                     borderRight: "1px solid " + ("dark" === e.colorScheme ? e.colors.dark[5] : e.colors.gray[2])
-                }, QN(s, eT(c))), l),
+                }, ET(s, jT(c))), l),
                 hidden: {
                     [`@media (max-width: ${e.fn.size({size:o,sizes:e.breakpoints})}px)`]: {
                         display: "none"
                     }
                 }
             };
             var s, c
         }),
-        lT = Object.defineProperty,
-        sT = Object.getOwnPropertySymbols,
-        cT = Object.prototype.hasOwnProperty,
-        uT = Object.prototype.propertyIsEnumerable,
-        dT = (e, t, r) => t in e ? lT(e, t, {
+        IT = Object.defineProperty,
+        RT = Object.getOwnPropertySymbols,
+        _T = Object.prototype.hasOwnProperty,
+        LT = Object.prototype.propertyIsEnumerable,
+        AT = (e, t, r) => t in e ? IT(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        pT = (e, t) => {
-            for (var r in t || (t = {})) cT.call(t, r) && dT(e, r, t[r]);
-            if (sT)
-                for (var r of sT(t)) uT.call(t, r) && dT(e, r, t[r]);
+        MT = (e, t) => {
+            for (var r in t || (t = {})) _T.call(t, r) && AT(e, r, t[r]);
+            if (RT)
+                for (var r of RT(t)) LT.call(t, r) && AT(e, r, t[r]);
             return e
         };
-    const fT = Object(n.forwardRef)((e, t) => {
+    const FT = Object(n.forwardRef)((e, t) => {
         var r = e,
             {
                 width: n,
                 height: o,
                 fixed: i = !1,
                 position: l,
                 zIndex: s = ac("app"),
@@ -24851,105 +25178,105 @@
                 styles: f,
                 children: m,
                 section: b,
                 __staticSelector: g
             } = r,
             y = ((e, t) => {
                 var r = {};
-                for (var n in e) cT.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                if (null != e && sT)
-                    for (var n of sT(e)) t.indexOf(n) < 0 && uT.call(e, n) && (r[n] = e[n]);
+                for (var n in e) _T.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                if (null != e && RT)
+                    for (var n of RT(e)) t.indexOf(n) < 0 && LT.call(e, n) && (r[n] = e[n]);
                 return r
             })(r, ["width", "height", "fixed", "position", "zIndex", "hiddenBreakpoint", "hidden", "className", "classNames", "styles", "children", "section", "__staticSelector"]);
-        const h = yN(),
+        const h = HN(),
             {
                 classes: v,
                 cx: O,
                 theme: w
-            } = iT({
+            } = DT({
                 width: n,
                 height: o,
                 fixed: h.fixed || i,
                 position: l,
                 hiddenBreakpoint: c,
                 zIndex: h.zIndex || s
             }, {
                 classNames: p,
                 styles: f,
                 name: g
             }),
-            x = qN(n, w).reduce((e, [t, r]) => (e[`@media (min-width: ${t+1}px)`] = {
+            x = yT(n, w).reduce((e, [t, r]) => (e[`@media (min-width: ${t+1}px)`] = {
                 [`--mantine-${b}-width`]: r + "px"
             }, e), {});
-        return a.a.createElement(Cn, pT({
+        return a.a.createElement(Cn, MT({
             component: "navbar" === b ? "nav" : "aside",
             ref: t,
             className: O(v.root, {
                 [v.hidden]: u
             }, d)
-        }, y), m, a.a.createElement(bN, {
+        }, y), m, a.a.createElement(BN, {
             styles: () => ({
-                ":root": pT({
+                ":root": MT({
                     [`--mantine-${b}-width`]: (null == n ? void 0 : n.base) ? n.base + "px" : "0px"
                 }, x)
             })
         }))
     });
-    fT.Section = XN, fT.displayName = "@mantine/core/HorizontalSection";
-    var mT = Object.defineProperty,
-        bT = Object.getOwnPropertySymbols,
-        gT = Object.prototype.hasOwnProperty,
-        yT = Object.prototype.propertyIsEnumerable,
-        hT = (e, t, r) => t in e ? mT(e, t, {
+    FT.Section = ST, FT.displayName = "@mantine/core/HorizontalSection";
+    var $T = Object.defineProperty,
+        BT = Object.getOwnPropertySymbols,
+        WT = Object.prototype.hasOwnProperty,
+        HT = Object.prototype.propertyIsEnumerable,
+        VT = (e, t, r) => t in e ? $T(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const vT = {
+    const qT = {
             fixed: !1,
             position: {
                 top: 0,
                 left: 0
             },
             zIndex: ac("app"),
             hiddenBreakpoint: "md",
             hidden: !1
         },
-        OT = Object(n.forwardRef)((e, t) => {
-            const r = ir("Navbar", vT, e);
-            return a.a.createElement(fT, ((e, t) => {
-                for (var r in t || (t = {})) gT.call(t, r) && hT(e, r, t[r]);
-                if (bT)
-                    for (var r of bT(t)) yT.call(t, r) && hT(e, r, t[r]);
+        UT = Object(n.forwardRef)((e, t) => {
+            const r = ir("Navbar", qT, e);
+            return a.a.createElement(FT, ((e, t) => {
+                for (var r in t || (t = {})) WT.call(t, r) && VT(e, r, t[r]);
+                if (BT)
+                    for (var r of BT(t)) HT.call(t, r) && VT(e, r, t[r]);
                 return e
             })({
                 section: "navbar",
                 __staticSelector: "Navbar",
                 ref: t
             }, r))
         });
 
-    function wT() {
-        return (wT = Object.assign || function(e) {
+    function GT() {
+        return (GT = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    OT.Section = fT.Section, OT.displayName = "@mantine/core/Navbar";
-    var xT = function(e) {
+    UT.Section = FT.Section, UT.displayName = "@mantine/core/Navbar";
+    var YT = function(e) {
         var t = e.class_name;
-        return a.a.createElement(OT, wT({}, G(["setProps", "children", "class_name"], e), {
+        return a.a.createElement(UT, GT({}, G(["setProps", "children", "class_name"], e), {
             className: t
         }), e.children)
     };
-    xT.displayName = "Navbar", xT.defaultProps = {}, xT.propTypes = {
+    YT.displayName = "Navbar", YT.defaultProps = {}, YT.propTypes = {
         children: i.a.node,
         class_name: i.a.string,
         fixed: i.a.bool,
         height: i.a.oneOfType([i.a.string, i.a.number]),
         hidden: i.a.bool,
         hiddenBreakpoint: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         id: i.a.string,
@@ -24973,84 +25300,84 @@
         py: i.a.oneOfType([i.a.string, i.a.number]),
         px: i.a.oneOfType([i.a.string, i.a.number]),
         pt: i.a.oneOfType([i.a.string, i.a.number]),
         pb: i.a.oneOfType([i.a.string, i.a.number]),
         pl: i.a.oneOfType([i.a.string, i.a.number]),
         pr: i.a.oneOfType([i.a.string, i.a.number])
     };
-    var ST = xT;
+    var ZT = YT;
 
-    function kT() {
-        return (kT = Object.assign || function(e) {
+    function KT() {
+        return (KT = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    var ET = function(e) {
+    var XT = function(e) {
         var t = e.class_name,
             r = G(["setProps", "class_name"], e);
-        return r = ta(r, ["label", "description", "error"]), a.a.createElement(Ao, kT({}, r, {
+        return r = ta(r, ["label", "description", "error"]), a.a.createElement(Ao, KT({}, r, {
             className: t
         }), e.children)
     };
-    ET.displayName = "InputWrapper", ET.defaultProps = {}, ET.propTypes = {
+    XT.displayName = "InputWrapper", XT.defaultProps = {}, XT.propTypes = {
         children: i.a.node,
         class_name: i.a.string,
         description: i.a.any,
         error: i.a.any,
         id: i.a.string,
         label: i.a.any,
         required: i.a.bool,
         setProps: i.a.func,
         size: i.a.oneOf(["xs", "sm", "md", "lg", "xl"]),
         style: i.a.object
     };
-    var jT = ET,
-        PT = Object.defineProperty,
-        zT = Object.defineProperties,
-        CT = Object.getOwnPropertyDescriptors,
-        NT = Object.getOwnPropertySymbols,
-        TT = Object.prototype.hasOwnProperty,
-        DT = Object.prototype.propertyIsEnumerable,
-        IT = (e, t, r) => t in e ? PT(e, t, {
+    var JT = XT,
+        QT = Object.defineProperty,
+        eD = Object.defineProperties,
+        tD = Object.getOwnPropertyDescriptors,
+        rD = Object.getOwnPropertySymbols,
+        nD = Object.prototype.hasOwnProperty,
+        aD = Object.prototype.propertyIsEnumerable,
+        oD = (e, t, r) => t in e ? QT(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        RT = (e, t) => {
-            for (var r in t || (t = {})) TT.call(t, r) && IT(e, r, t[r]);
-            if (NT)
-                for (var r of NT(t)) DT.call(t, r) && IT(e, r, t[r]);
+        iD = (e, t) => {
+            for (var r in t || (t = {})) nD.call(t, r) && oD(e, r, t[r]);
+            if (rD)
+                for (var r of rD(t)) aD.call(t, r) && oD(e, r, t[r]);
             return e
         },
-        _T = Er((e, {
+        lD = Er((e, {
             size: t,
             radius: r
         }) => {
             const n = "dark" === e.colorScheme ? e.colors.dark[4] : e.colors.gray[3];
             return {
-                root: (a = RT({}, e.fn.focusStyles()), o = {
+                root: (a = iD({}, e.fn.focusStyles()), o = {
                     width: t,
                     height: t,
                     WebkitTapHighlightColor: "transparent",
                     border: 0,
                     borderRadius: e.fn.size({
                         size: r,
                         sizes: e.radius
                     }),
                     appearance: "none",
                     WebkitAppearance: "none",
                     padding: 0,
                     position: "relative",
                     overflow: "hidden"
-                }, zT(a, CT(o))),
+                }, eD(a, tD(o))),
                 overlay: {
                     position: "absolute",
                     borderRadius: e.fn.size({
                         size: r,
                         sizes: e.radius
                     }),
                     top: 0,
@@ -25071,62 +25398,62 @@
                     backgroundImage: `linear-gradient(45deg, ${n} 25%, transparent 25%), linear-gradient(-45deg, ${n} 25%, transparent 25%), linear-gradient(45deg, transparent 75%, ${n} 75%), linear-gradient(-45deg, ${"dark"===e.colorScheme?e.colors.dark[7]:e.white} 75%, ${n} 75%)`,
                     backgroundSize: "8px 8px",
                     backgroundPosition: "0 0, 0 4px, 4px -4px, -4px 0px"
                 }
             };
             var a, o
         }),
-        LT = Object.defineProperty,
-        AT = Object.getOwnPropertySymbols,
-        MT = Object.prototype.hasOwnProperty,
-        FT = Object.prototype.propertyIsEnumerable,
-        $T = (e, t, r) => t in e ? LT(e, t, {
+        sD = Object.defineProperty,
+        cD = Object.getOwnPropertySymbols,
+        uD = Object.prototype.hasOwnProperty,
+        dD = Object.prototype.propertyIsEnumerable,
+        pD = (e, t, r) => t in e ? sD(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const BT = {
+    const fD = {
             size: 25,
             radius: 25
         },
-        WT = Object(n.forwardRef)((e, t) => {
-            const r = ir("ColorSwatch", BT, e),
+        mD = Object(n.forwardRef)((e, t) => {
+            const r = ir("ColorSwatch", fD, e),
                 {
                     component: n,
                     color: o,
                     size: i,
                     radius: l,
                     className: s,
                     children: c,
                     classNames: u,
                     styles: d
                 } = r,
                 p = ((e, t) => {
                     var r = {};
-                    for (var n in e) MT.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && AT)
-                        for (var n of AT(e)) t.indexOf(n) < 0 && FT.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) uD.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && cD)
+                        for (var n of cD(e)) t.indexOf(n) < 0 && dD.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["component", "color", "size", "radius", "className", "children", "classNames", "styles"]),
                 {
                     classes: f,
                     cx: m
-                } = _T({
+                } = lD({
                     radius: l,
                     size: i
                 }, {
                     classNames: u,
                     styles: d,
                     name: "ColorSwatch"
                 });
             return a.a.createElement(Cn, ((e, t) => {
-                for (var r in t || (t = {})) MT.call(t, r) && $T(e, r, t[r]);
-                if (AT)
-                    for (var r of AT(t)) FT.call(t, r) && $T(e, r, t[r]);
+                for (var r in t || (t = {})) uD.call(t, r) && pD(e, r, t[r]);
+                if (cD)
+                    for (var r of cD(t)) dD.call(t, r) && pD(e, r, t[r]);
                 return e
             })({
                 component: n || "div",
                 className: m(f.root, s),
                 ref: t
             }, p), a.a.createElement("div", {
                 className: m(f.alphaOverlay, f.overlay)
@@ -25137,28 +25464,28 @@
                 style: {
                     backgroundColor: o
                 }
             }), a.a.createElement("div", {
                 className: m(f.children, f.overlay)
             }, c))
         });
-    WT.displayName = "@mantine/core/ColorSwatch";
-    const HT = {
+    mD.displayName = "@mantine/core/ColorSwatch";
+    const bD = {
         xs: 8,
         sm: 12,
         md: 16,
         lg: 20,
         xl: 22
     };
-    var VT = Er((e, {
+    var gD = Er((e, {
             size: t
         }) => {
             const r = e.fn.size({
                 size: t,
-                sizes: HT
+                sizes: bD
             });
             return {
                 thumb: {
                     overflow: "hidden",
                     boxSizing: "border-box",
                     position: "absolute",
                     boxShadow: "0 0 1px rgba(0, 0, 0, .6)",
@@ -25166,81 +25493,81 @@
                     backgroundColor: "transparent",
                     width: r,
                     height: r,
                     borderRadius: r
                 }
             }
         }),
-        qT = Object.defineProperty,
-        UT = Object.getOwnPropertySymbols,
-        GT = Object.prototype.hasOwnProperty,
-        YT = Object.prototype.propertyIsEnumerable,
-        ZT = (e, t, r) => t in e ? qT(e, t, {
+        yD = Object.defineProperty,
+        hD = Object.getOwnPropertySymbols,
+        vD = Object.prototype.hasOwnProperty,
+        OD = Object.prototype.propertyIsEnumerable,
+        wD = (e, t, r) => t in e ? yD(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        KT = (e, t) => {
-            for (var r in t || (t = {})) GT.call(t, r) && ZT(e, r, t[r]);
-            if (UT)
-                for (var r of UT(t)) YT.call(t, r) && ZT(e, r, t[r]);
+        xD = (e, t) => {
+            for (var r in t || (t = {})) vD.call(t, r) && wD(e, r, t[r]);
+            if (hD)
+                for (var r of hD(t)) OD.call(t, r) && wD(e, r, t[r]);
             return e
         };
 
-    function XT({
+    function SD({
         position: e,
         className: t,
         styles: r,
         classNames: n,
         style: o,
         size: i,
         __staticSelector: l
     }) {
         const {
             classes: s,
             cx: c
-        } = VT({
+        } = gD({
             size: i
         }, {
             classNames: n,
             styles: r,
             name: l
         });
         return a.a.createElement("div", {
             className: c(s.thumb, t),
-            style: KT({
-                left: `calc(${100*e.x}% - ${HT[i]/2}px)`,
-                top: `calc(${100*e.y}% - ${HT[i]/2}px)`
+            style: xD({
+                left: `calc(${100*e.x}% - ${bD[i]/2}px)`,
+                top: `calc(${100*e.y}% - ${bD[i]/2}px)`
             }, o)
         })
     }
-    XT.displayName = "@mantine/core/Thumb";
-    var JT = Er((e, {
+    SD.displayName = "@mantine/core/Thumb";
+    var kD = Er((e, {
             size: t
         }, r) => {
             const n = {
                 ref: r("sliderThumb")
             };
             return {
                 sliderThumb: n,
                 slider: {
                     position: "relative",
                     height: e.fn.size({
                         size: t,
-                        sizes: HT
+                        sizes: bD
                     }) + 2,
                     boxSizing: "border-box",
                     marginLeft: e.fn.size({
                         size: t,
-                        sizes: HT
+                        sizes: bD
                     }) / 2,
                     marginRight: e.fn.size({
                         size: t,
-                        sizes: HT
+                        sizes: bD
                     }) / 2,
                     outline: 0,
                     ["&:focus ." + n.ref]: {
                         outline: "none",
                         boxShadow: "always" === e.focusRing || "auto" === e.focusRing ? `0 0 0 2px ${"dark"===e.colorScheme?e.colors.dark[9]:e.white}, 0 0 0 4px ${e.colors[e.primaryColor]["dark"===e.colorScheme?7:5]}` : void 0
                     },
                     ["&:focus:not(:focus-visible) ." + n.ref]: {
@@ -25250,37 +25577,37 @@
                 sliderOverlay: {
                     position: "absolute",
                     boxSizing: "border-box",
                     top: 0,
                     bottom: 0,
                     left: -e.fn.size({
                         size: t,
-                        sizes: HT
+                        sizes: bD
                     }) / 2 - 1,
                     right: -e.fn.size({
                         size: t,
-                        sizes: HT
+                        sizes: bD
                     }) / 2 - 1,
                     borderRadius: 1e3
                 }
             }
         }),
-        QT = Object.defineProperty,
-        eD = Object.defineProperties,
-        tD = Object.getOwnPropertyDescriptors,
-        rD = Object.getOwnPropertySymbols,
-        nD = Object.prototype.hasOwnProperty,
-        aD = Object.prototype.propertyIsEnumerable,
-        oD = (e, t, r) => t in e ? QT(e, t, {
+        ED = Object.defineProperty,
+        jD = Object.defineProperties,
+        PD = Object.getOwnPropertyDescriptors,
+        zD = Object.getOwnPropertySymbols,
+        CD = Object.prototype.hasOwnProperty,
+        ND = Object.prototype.propertyIsEnumerable,
+        TD = (e, t, r) => t in e ? ED(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const iD = Object(n.forwardRef)((e, t) => {
+    const DD = Object(n.forwardRef)((e, t) => {
         var r = e,
             {
                 value: o,
                 onChange: i,
                 maxValue: l,
                 round: s,
                 size: c = "md",
@@ -25290,23 +25617,23 @@
                 overlays: f,
                 classNames: m,
                 styles: b,
                 className: g
             } = r,
             y = ((e, t) => {
                 var r = {};
-                for (var n in e) nD.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                if (null != e && rD)
-                    for (var n of rD(e)) t.indexOf(n) < 0 && aD.call(e, n) && (r[n] = e[n]);
+                for (var n in e) CD.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                if (null != e && zD)
+                    for (var n of zD(e)) t.indexOf(n) < 0 && ND.call(e, n) && (r[n] = e[n]);
                 return r
             })(r, ["value", "onChange", "maxValue", "round", "size", "thumbColor", "__staticSelector", "focusable", "overlays", "classNames", "styles", "className"]);
         const {
             classes: h,
             cx: v
-        } = JT({
+        } = kD({
             size: c
         }, {
             classNames: m,
             styles: b,
             name: d
         }), [O, w] = Object(n.useState)({
             y: 0,
@@ -25328,18 +25655,18 @@
                 i(x(r.x))
             },
             E = f.map((e, t) => a.a.createElement("div", {
                 className: h.sliderOverlay,
                 style: e,
                 key: t
             }));
-        return a.a.createElement(Cn, ((e, t) => eD(e, tD(t)))(((e, t) => {
-            for (var r in t || (t = {})) nD.call(t, r) && oD(e, r, t[r]);
-            if (rD)
-                for (var r of rD(t)) aD.call(t, r) && oD(e, r, t[r]);
+        return a.a.createElement(Cn, ((e, t) => jD(e, PD(t)))(((e, t) => {
+            for (var r in t || (t = {})) CD.call(t, r) && TD(e, r, t[r]);
+            if (zD)
+                for (var r of zD(t)) ND.call(t, r) && TD(e, r, t[r]);
             return e
         })({}, y), {
             ref: ua(S, t),
             className: v(h.slider, g),
             role: "slider",
             "aria-valuenow": o,
             "aria-valuemax": l,
@@ -25356,57 +25683,57 @@
                     case "ArrowLeft":
                         k(e, {
                             x: O.x - .05,
                             y: O.y
                         })
                 }
             }
-        }), E, a.a.createElement(XT, {
+        }), E, a.a.createElement(SD, {
             __staticSelector: d,
             classNames: m,
             styles: b,
             position: O,
             style: {
                 top: 1,
                 backgroundColor: u
             },
             className: h.sliderThumb,
             size: c
         }))
     });
-    iD.displayName = "@mantine/core/ColorSlider";
-    var lD = Object.defineProperty,
-        sD = Object.defineProperties,
-        cD = Object.getOwnPropertyDescriptors,
-        uD = Object.getOwnPropertySymbols,
-        dD = Object.prototype.hasOwnProperty,
-        pD = Object.prototype.propertyIsEnumerable,
-        fD = (e, t, r) => t in e ? lD(e, t, {
+    DD.displayName = "@mantine/core/ColorSlider";
+    var ID = Object.defineProperty,
+        RD = Object.defineProperties,
+        _D = Object.getOwnPropertyDescriptors,
+        LD = Object.getOwnPropertySymbols,
+        AD = Object.prototype.hasOwnProperty,
+        MD = Object.prototype.propertyIsEnumerable,
+        FD = (e, t, r) => t in e ? ID(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const mD = Object(n.forwardRef)((e, t) => {
+    const $D = Object(n.forwardRef)((e, t) => {
         var r = e,
             {
                 value: n,
                 onChange: o
             } = r,
             i = ((e, t) => {
                 var r = {};
-                for (var n in e) dD.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                if (null != e && uD)
-                    for (var n of uD(e)) t.indexOf(n) < 0 && pD.call(e, n) && (r[n] = e[n]);
+                for (var n in e) AD.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                if (null != e && LD)
+                    for (var n of LD(e)) t.indexOf(n) < 0 && MD.call(e, n) && (r[n] = e[n]);
                 return r
             })(r, ["value", "onChange"]);
-        return a.a.createElement(iD, ((e, t) => sD(e, cD(t)))(((e, t) => {
-            for (var r in t || (t = {})) dD.call(t, r) && fD(e, r, t[r]);
-            if (uD)
-                for (var r of uD(t)) pD.call(t, r) && fD(e, r, t[r]);
+        return a.a.createElement(DD, ((e, t) => RD(e, _D(t)))(((e, t) => {
+            for (var r in t || (t = {})) AD.call(t, r) && FD(e, r, t[r]);
+            if (LD)
+                for (var r of LD(t)) MD.call(t, r) && FD(e, r, t[r]);
             return e
         })({}, i), {
             ref: t,
             value: n,
             onChange: o,
             maxValue: 360,
             thumbColor: `hsl(${n}, 100%, 50%)`,
@@ -25415,227 +25742,227 @@
                 backgroundImage: "linear-gradient(to right,hsl(0,100%,50%),hsl(60,100%,50%),hsl(120,100%,50%),hsl(170,100%,50%),hsl(240,100%,50%),hsl(300,100%,50%),hsl(360,100%,50%))"
             }, {
                 boxShadow: "rgba(0, 0, 0, .1) 0px 0px 0px 1px inset, rgb(0, 0, 0, .15) 0px 0px 4px inset"
             }]
         }))
     });
 
-    function bD(e, t = 0, r = 10 ** t) {
+    function BD(e, t = 0, r = 10 ** t) {
         return Math.round(r * e) / r
     }
-    mD.displayName = "@mantine/core/HueSlider";
-    const gD = {
+    $D.displayName = "@mantine/core/HueSlider";
+    const WD = {
         grad: .9,
         turn: 360,
         rad: 360 / (2 * Math.PI)
     };
 
-    function yD(e, t = "deg") {
-        return Number(e) * (gD[t] || 1)
+    function HD(e, t = "deg") {
+        return Number(e) * (WD[t] || 1)
     }
-    const hD = /hsla?\(?\s*(-?\d*\.?\d+)(deg|rad|grad|turn)?[,\s]+(-?\d*\.?\d+)%?[,\s]+(-?\d*\.?\d+)%?,?\s*[/\s]*(-?\d*\.?\d+)?(%)?\s*\)?/i;
+    const VD = /hsla?\(?\s*(-?\d*\.?\d+)(deg|rad|grad|turn)?[,\s]+(-?\d*\.?\d+)%?[,\s]+(-?\d*\.?\d+)%?,?\s*[/\s]*(-?\d*\.?\d+)?(%)?\s*\)?/i;
 
-    function vD(e) {
-        const t = hD.exec(e);
+    function qD(e) {
+        const t = VD.exec(e);
         return t ? function({
             h: e,
             s: t,
             l: r,
             a: n
         }) {
             const a = t * ((r < 50 ? r : 100 - r) / 100);
             return {
                 h: e,
                 s: a > 0 ? 2 * a / (r + a) * 100 : 0,
                 v: r + a,
                 a: n
             }
         }({
-            h: yD(t[1], t[2]),
+            h: HD(t[1], t[2]),
             s: Number(t[3]),
             l: Number(t[4]),
             a: void 0 === t[5] ? 1 : Number(t[5]) / (t[6] ? 100 : 1)
         }) : {
             h: 0,
             s: 0,
             v: 0,
             a: 1
         }
     }
 
-    function OD({
+    function UD({
         r: e,
         g: t,
         b: r,
         a: n
     }) {
         const a = Math.max(e, t, r),
             o = a - Math.min(e, t, r),
             i = o ? a === e ? (t - r) / o : a === t ? 2 + (r - e) / o : 4 + (e - t) / o : 0;
         return {
-            h: bD(60 * (i < 0 ? i + 6 : i)),
-            s: bD(a ? o / a * 100 : 0),
-            v: bD(a / 255 * 100),
+            h: BD(60 * (i < 0 ? i + 6 : i)),
+            s: BD(a ? o / a * 100 : 0),
+            v: BD(a / 255 * 100),
             a: n
         }
     }
-    const wD = /rgba?\(?\s*(-?\d*\.?\d+)(%)?[,\s]+(-?\d*\.?\d+)(%)?[,\s]+(-?\d*\.?\d+)(%)?,?\s*[/\s]*(-?\d*\.?\d+)?(%)?\s*\)?/i;
+    const GD = /rgba?\(?\s*(-?\d*\.?\d+)(%)?[,\s]+(-?\d*\.?\d+)(%)?[,\s]+(-?\d*\.?\d+)(%)?,?\s*[/\s]*(-?\d*\.?\d+)?(%)?\s*\)?/i;
 
-    function xD(e) {
-        const t = wD.exec(e);
-        return t ? OD({
+    function YD(e) {
+        const t = GD.exec(e);
+        return t ? UD({
             r: Number(t[1]) / (t[2] ? 100 / 255 : 1),
             g: Number(t[3]) / (t[4] ? 100 / 255 : 1),
             b: Number(t[5]) / (t[6] ? 100 / 255 : 1),
             a: void 0 === t[7] ? 1 : Number(t[7]) / (t[8] ? 100 : 1)
         }) : {
             h: 0,
             s: 0,
             v: 0,
             a: 1
         }
     }
-    const SD = {
+    const ZD = {
             hex: /^#?([0-9A-F]{3}){1,2}$/i,
             rgb: /^rgb\((\d+),\s*(\d+),\s*(\d+)(?:,\s*(\d+(?:\.\d+)?))?\)$/i,
             rgba: /^rgba\((\d+),\s*(\d+),\s*(\d+)(?:,\s*(\d+(?:\.\d+)?))?\)$/i,
             hsl: /hsl\(\s*(\d+)\s*,\s*(\d+(?:\.\d+)?%)\s*,\s*(\d+(?:\.\d+)?%)\)/i,
             hsla: /^hsla\((\d+),\s*([\d.]+)%,\s*([\d.]+)%,\s*(\d*(?:\.\d+)?)\)$/i
         },
-        kD = {
+        KD = {
             hex: function(e) {
                 const t = "#" === e[0] ? e.slice(1) : e;
-                return 3 === t.length ? OD({
+                return 3 === t.length ? UD({
                     r: parseInt(t[0] + t[0], 16),
                     g: parseInt(t[1] + t[1], 16),
                     b: parseInt(t[2] + t[2], 16),
                     a: 1
-                }) : OD({
+                }) : UD({
                     r: parseInt(t.slice(0, 2), 16),
                     g: parseInt(t.slice(2, 4), 16),
                     b: parseInt(t.slice(4, 6), 16),
                     a: 1
                 })
             },
-            rgb: xD,
-            rgba: xD,
-            hsl: vD,
-            hsla: vD
+            rgb: YD,
+            rgba: YD,
+            hsl: qD,
+            hsla: qD
         };
 
-    function ED(e) {
-        for (const [, t] of Object.entries(SD))
+    function XD(e) {
+        for (const [, t] of Object.entries(ZD))
             if (t.test(e)) return !0;
         return !1
     }
 
-    function jD(e) {
+    function JD(e) {
         if ("string" != typeof e) return {
             h: 0,
             s: 0,
             v: 0,
             a: 1
         };
         if ("transparent" === e) return {
             h: 0,
             s: 0,
             v: 0,
             a: 0
         };
         const t = e.trim();
-        for (const [e, r] of Object.entries(SD))
-            if (r.test(t)) return kD[e](t);
+        for (const [e, r] of Object.entries(ZD))
+            if (r.test(t)) return KD[e](t);
         return {
             h: 0,
             s: 0,
             v: 0,
             a: 1
         }
     }
-    var PD = Object.defineProperty,
-        zD = Object.defineProperties,
-        CD = Object.getOwnPropertyDescriptors,
-        ND = Object.getOwnPropertySymbols,
-        TD = Object.prototype.hasOwnProperty,
-        DD = Object.prototype.propertyIsEnumerable,
-        ID = (e, t, r) => t in e ? PD(e, t, {
+    var QD = Object.defineProperty,
+        eI = Object.defineProperties,
+        tI = Object.getOwnPropertyDescriptors,
+        rI = Object.getOwnPropertySymbols,
+        nI = Object.prototype.hasOwnProperty,
+        aI = Object.prototype.propertyIsEnumerable,
+        oI = (e, t, r) => t in e ? QD(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const RD = Object(n.forwardRef)((e, t) => {
+    const iI = Object(n.forwardRef)((e, t) => {
         var r = e,
             {
                 value: n,
                 onChange: o,
                 color: i
             } = r,
             l = ((e, t) => {
                 var r = {};
-                for (var n in e) TD.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                if (null != e && ND)
-                    for (var n of ND(e)) t.indexOf(n) < 0 && DD.call(e, n) && (r[n] = e[n]);
+                for (var n in e) nI.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                if (null != e && rI)
+                    for (var n of rI(e)) t.indexOf(n) < 0 && aI.call(e, n) && (r[n] = e[n]);
                 return r
             })(r, ["value", "onChange", "color"]);
         const s = or(),
             c = "dark" === s.colorScheme ? s.colors.dark[4] : s.colors.gray[3];
-        return a.a.createElement(iD, ((e, t) => zD(e, CD(t)))(((e, t) => {
-            for (var r in t || (t = {})) TD.call(t, r) && ID(e, r, t[r]);
-            if (ND)
-                for (var r of ND(t)) DD.call(t, r) && ID(e, r, t[r]);
+        return a.a.createElement(DD, ((e, t) => eI(e, tI(t)))(((e, t) => {
+            for (var r in t || (t = {})) nI.call(t, r) && oI(e, r, t[r]);
+            if (rI)
+                for (var r of rI(t)) aI.call(t, r) && oI(e, r, t[r]);
             return e
         })({}, l), {
             ref: t,
             value: n,
-            onChange: e => o(bD(e, 2)),
+            onChange: e => o(BD(e, 2)),
             maxValue: 1,
             round: !1,
             overlays: [{
                 backgroundImage: `linear-gradient(45deg, ${c} 25%, transparent 25%), linear-gradient(-45deg, ${c} 25%, transparent 25%), linear-gradient(45deg, transparent 75%, ${c} 75%), linear-gradient(-45deg, ${"dark"===s.colorScheme?s.colors.dark[7]:s.white} 75%, ${c} 75%)`,
                 backgroundSize: "8px 8px",
                 backgroundPosition: "0 0, 0 4px, 4px -4px, -4px 0px"
             }, {
                 backgroundImage: `linear-gradient(90deg, transparent, ${i})`
             }, {
                 boxShadow: "rgba(0, 0, 0, .1) 0px 0px 0px 1px inset, rgb(0, 0, 0, .15) 0px 0px 4px inset"
             }]
         }))
     });
-    RD.displayName = "@mantine/core/AlphaSlider";
-    const _D = {
+    iI.displayName = "@mantine/core/AlphaSlider";
+    const lI = {
         xs: 100,
         sm: 110,
         md: 120,
         lg: 140,
         xl: 160
     };
-    var LD = Er((e, {
+    var sI = Er((e, {
         size: t
     }, r) => {
         const n = -e.fn.size({
                 size: t,
-                sizes: HT
+                sizes: bD
             }) / 2 - 1,
             a = {
                 ref: r("saturationThumb")
             };
         return {
             saturationThumb: a,
             saturation: {
                 boxSizing: "border-box",
                 position: "relative",
                 height: e.fn.size({
                     size: t,
-                    sizes: _D
+                    sizes: lI
                 }),
                 borderRadius: e.radius.sm,
                 margin: e.fn.size({
                     size: t,
-                    sizes: HT
+                    sizes: bD
                 }) / 2,
                 WebkitTapHighlightColor: "transparent",
                 ["&:focus ." + a.ref]: {
                     outline: "none",
                     boxShadow: `0 0 0 1px ${"dark"===e.colorScheme?e.colors.dark[9]:e.white}, 0 0 0 3px ${e.colors[e.primaryColor]["dark"===e.colorScheme?7:5]}`
                 },
                 ["&:focus:not(:focus-visible) ." + a.ref]: {
@@ -25650,96 +25977,96 @@
                 left: n,
                 right: n,
                 bottom: n
             }
         }
     });
 
-    function AD({
+    function cI({
         h: e,
         s: t,
         v: r,
         a: n
     }) {
         const a = e / 360 * 6,
             o = t / 100,
             i = r / 100,
             l = Math.floor(a),
             s = i * (1 - o),
             c = i * (1 - (a - l) * o),
             u = i * (1 - (1 - a + l) * o),
             d = l % 6;
         return {
-            r: bD(255 * [i, c, s, s, u, i][d]),
-            g: bD(255 * [u, i, i, c, s, s][d]),
-            b: bD(255 * [s, s, u, i, i, c][d]),
-            a: bD(n, 2)
+            r: BD(255 * [i, c, s, s, u, i][d]),
+            g: BD(255 * [u, i, i, c, s, s][d]),
+            b: BD(255 * [s, s, u, i, i, c][d]),
+            a: BD(n, 2)
         }
     }
 
-    function MD(e, t) {
+    function uI(e, t) {
         const {
             r: r,
             g: n,
             b: a,
             a: o
-        } = AD(e);
-        return t ? `rgba(${r}, ${n}, ${a}, ${bD(o,2)})` : `rgb(${r}, ${n}, ${a})`
+        } = cI(e);
+        return t ? `rgba(${r}, ${n}, ${a}, ${BD(o,2)})` : `rgb(${r}, ${n}, ${a})`
     }
 
-    function FD({
+    function dI({
         h: e,
         s: t,
         v: r,
         a: n
     }, a) {
         const o = (200 - t) * r / 100,
             i = Math.round(e),
             l = Math.round(o > 0 && o < 200 ? t * r / 100 / (o <= 100 ? o : 200 - o) * 100 : 0),
             s = Math.round(o / 2);
-        return a ? `hsla(${i}, ${l}%, ${s}%, ${bD(n,2)})` : `hsl(${i}, ${l}%, ${s}%)`
+        return a ? `hsla(${i}, ${l}%, ${s}%, ${BD(n,2)})` : `hsl(${i}, ${l}%, ${s}%)`
     }
 
-    function $D(e) {
+    function pI(e) {
         const t = e.toString(16);
         return t.length < 2 ? "0" + t : t
     }
-    const BD = {
+    const fI = {
         hex: function(e) {
             const {
                 r: t,
                 g: r,
                 b: n
-            } = AD(e);
-            return `#${$D(t)}${$D(r)}${$D(n)}`
+            } = cI(e);
+            return `#${pI(t)}${pI(r)}${pI(n)}`
         },
-        rgb: e => MD(e, !1),
-        rgba: e => MD(e, !0),
-        hsl: e => FD(e, !1),
-        hsla: e => FD(e, !0)
+        rgb: e => uI(e, !1),
+        rgba: e => uI(e, !0),
+        hsl: e => dI(e, !1),
+        hsla: e => dI(e, !0)
     };
 
-    function WD(e, t) {
-        return t ? e in BD ? BD[e](t) : BD.hex(t) : "#000000"
+    function mI(e, t) {
+        return t ? e in fI ? fI[e](t) : fI.hex(t) : "#000000"
     }
 
-    function HD({
+    function bI({
         value: e,
         onChange: t,
         focusable: r = !0,
         __staticSelector: o = "saturation",
         size: i,
         color: l,
         saturationLabel: s,
         classNames: c,
         styles: u
     }) {
         const {
             classes: d
-        } = LD({
+        } = sI({
             size: i
         }, {
             classNames: c,
             styles: u,
             name: o
         }), [p, f] = Object(n.useState)({
             x: e.s / 100,
@@ -25771,15 +26098,15 @@
         };
         return a.a.createElement("div", {
             className: d.saturation,
             ref: m,
             role: "slider",
             "aria-label": s,
             "aria-valuenow": p.x,
-            "aria-valuetext": WD("rgba", e),
+            "aria-valuetext": mI("rgba", e),
             tabIndex: r ? 0 : -1,
             onKeyDown: e => {
                 switch (e.nativeEvent.code) {
                     case "ArrowUp":
                         b(e, {
                             y: p.y - .05,
                             x: p.x
@@ -25815,28 +26142,28 @@
                 backgroundImage: "linear-gradient(90deg, #fff, transparent)"
             }
         }), a.a.createElement("div", {
             className: d.saturationOverlay,
             style: {
                 backgroundImage: "linear-gradient(0deg, #000, transparent)"
             }
-        }), a.a.createElement(XT, {
+        }), a.a.createElement(SD, {
             __staticSelector: o,
             classNames: c,
             styles: u,
             position: p,
             className: d.saturationThumb,
             style: {
                 backgroundColor: l
             },
             size: i
         }))
     }
-    HD.displayName = "@mantine/core/Saturation";
-    var VD = Er((e, {
+    bI.displayName = "@mantine/core/Saturation";
+    var gI = Er((e, {
             swatchesPerRow: t
         }) => ({
             swatch: {
                 width: `calc(${100/t}% - 4px)`,
                 height: 0,
                 paddingBottom: `calc(${100/t}% - 4px)`,
                 margin: 2,
@@ -25846,92 +26173,92 @@
                 boxSizing: "border-box",
                 marginLeft: -2,
                 marginRight: -2,
                 display: "flex",
                 flexWrap: "wrap"
             }
         })),
-        qD = Object.defineProperty,
-        UD = Object.getOwnPropertySymbols,
-        GD = Object.prototype.hasOwnProperty,
-        YD = Object.prototype.propertyIsEnumerable,
-        ZD = (e, t, r) => t in e ? qD(e, t, {
+        yI = Object.defineProperty,
+        hI = Object.getOwnPropertySymbols,
+        vI = Object.prototype.hasOwnProperty,
+        OI = Object.prototype.propertyIsEnumerable,
+        wI = (e, t, r) => t in e ? yI(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
 
-    function KD(e) {
+    function xI(e) {
         var t = e,
             {
                 data: r,
                 onSelect: n,
                 swatchesPerRow: o = 10,
                 focusable: i = !0,
                 classNames: l,
                 styles: s,
                 __staticSelector: c = "color-picker"
             } = t,
             u = ((e, t) => {
                 var r = {};
-                for (var n in e) GD.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                if (null != e && UD)
-                    for (var n of UD(e)) t.indexOf(n) < 0 && YD.call(e, n) && (r[n] = e[n]);
+                for (var n in e) vI.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                if (null != e && hI)
+                    for (var n of hI(e)) t.indexOf(n) < 0 && OI.call(e, n) && (r[n] = e[n]);
                 return r
             })(t, ["data", "onSelect", "swatchesPerRow", "focusable", "classNames", "styles", "__staticSelector"]);
         const {
             classes: d
-        } = VD({
+        } = gI({
             swatchesPerRow: o
         }, {
             classNames: l,
             styles: s,
             name: c
-        }), p = r.map((e, t) => a.a.createElement(WT, {
+        }), p = r.map((e, t) => a.a.createElement(mD, {
             className: d.swatch,
             component: "button",
             type: "button",
             color: e,
             key: t,
             radius: "sm",
-            onClick: () => n(jD(e)),
+            onClick: () => n(JD(e)),
             style: {
                 cursor: "pointer"
             },
             "aria-label": e,
             tabIndex: i ? 0 : -1
         }));
         return a.a.createElement("div", ((e, t) => {
-            for (var r in t || (t = {})) GD.call(t, r) && ZD(e, r, t[r]);
-            if (UD)
-                for (var r of UD(t)) YD.call(t, r) && ZD(e, r, t[r]);
+            for (var r in t || (t = {})) vI.call(t, r) && wI(e, r, t[r]);
+            if (hI)
+                for (var r of hI(t)) OI.call(t, r) && wI(e, r, t[r]);
             return e
         })({
             className: d.swatches
         }, u), p)
     }
-    KD.displayName = "@mantine/core/Swatches";
-    const XD = {
+    xI.displayName = "@mantine/core/Swatches";
+    const SI = {
         xs: 180,
         sm: 200,
         md: 240,
         lg: 280,
         xl: 320
     };
-    var JD = Er((e, {
+    var kI = Er((e, {
             size: t,
             fullWidth: r
         }) => ({
             preview: {},
             wrapper: {
                 boxSizing: "border-box",
                 width: r ? "100%" : e.fn.size({
                     size: t,
-                    sizes: XD
+                    sizes: SI
                 }),
                 padding: 1
             },
             body: {
                 display: "flex",
                 boxSizing: "border-box",
                 paddingTop: e.fn.size({
@@ -25952,46 +26279,46 @@
                     marginTop: 5
                 }
             },
             swatch: {
                 cursor: "pointer"
             }
         })),
-        QD = Object.defineProperty,
-        eI = Object.getOwnPropertySymbols,
-        tI = Object.prototype.hasOwnProperty,
-        rI = Object.prototype.propertyIsEnumerable,
-        nI = (e, t, r) => t in e ? QD(e, t, {
+        EI = Object.defineProperty,
+        jI = Object.getOwnPropertySymbols,
+        PI = Object.prototype.hasOwnProperty,
+        zI = Object.prototype.propertyIsEnumerable,
+        CI = (e, t, r) => t in e ? EI(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        aI = (e, t) => {
-            for (var r in t || (t = {})) tI.call(t, r) && nI(e, r, t[r]);
-            if (eI)
-                for (var r of eI(t)) rI.call(t, r) && nI(e, r, t[r]);
+        NI = (e, t) => {
+            for (var r in t || (t = {})) PI.call(t, r) && CI(e, r, t[r]);
+            if (jI)
+                for (var r of jI(t)) zI.call(t, r) && CI(e, r, t[r]);
             return e
         };
-    const oI = {
+    const TI = {
             xs: 26,
             sm: 34,
             md: 42,
             lg: 50,
             xl: 54
         },
-        iI = {
+        DI = {
             swatchesPerRow: 10,
             size: "sm",
             withPicker: !0,
             focusable: !0,
             __staticSelector: "ColorPicker"
         },
-        lI = Object(n.forwardRef)((e, t) => {
-            const r = ir("ColorPicker", iI, e),
+        II = Object(n.forwardRef)((e, t) => {
+            const r = ir("ColorPicker", DI, e),
                 {
                     value: o,
                     defaultValue: i,
                     onChange: l,
                     format: s,
                     swatches: c,
                     swatchesPerRow: u,
@@ -26005,24 +26332,24 @@
                     alphaLabel: h,
                     className: v,
                     styles: O,
                     classNames: w
                 } = r,
                 x = ((e, t) => {
                     var r = {};
-                    for (var n in e) tI.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && eI)
-                        for (var n of eI(e)) t.indexOf(n) < 0 && rI.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) PI.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && jI)
+                        for (var n of jI(e)) t.indexOf(n) < 0 && zI.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["value", "defaultValue", "onChange", "format", "swatches", "swatchesPerRow", "size", "withPicker", "fullWidth", "focusable", "__staticSelector", "saturationLabel", "hueLabel", "alphaLabel", "className", "styles", "classNames"]),
                 {
                     classes: S,
                     cx: k,
                     theme: E
-                } = JD({
+                } = kI({
                     size: d,
                     fullWidth: f
                 }, {
                     classNames: w,
                     styles: O,
                     name: b
                 }),
@@ -26030,120 +26357,120 @@
                 P = Object(n.useRef)(null),
                 z = "rgba" === s || "hsla" === s,
                 [C, N] = Object(n.useState)(!1),
                 [T, D] = la({
                     value: o,
                     defaultValue: i,
                     finalValue: "#FFFFFF",
-                    rule: e => ED(e),
+                    rule: e => XD(e),
                     onChange: l
                 }),
-                [I, R] = Object(n.useState)(jD(T)),
+                [I, R] = Object(n.useState)(JD(T)),
                 _ = e => {
                     N(!0), R(t => {
-                        const r = aI(aI({}, t), e);
-                        return P.current = WD(j.current, r), r
+                        const r = NI(NI({}, t), e);
+                        return P.current = mI(j.current, r), r
                     }), Promise.resolve().then(() => D(P.current)).then(() => N(!1))
                 };
             return Object(n.useEffect)(() => {
-                ED(o) && !C && R(jD(o))
+                XD(o) && !C && R(JD(o))
             }, [o]), _u(() => {
-                j.current = s, D(WD(s, I))
-            }, [s]), a.a.createElement(Cn, aI({
+                j.current = s, D(mI(s, I))
+            }, [s]), a.a.createElement(Cn, NI({
                 className: k(S.wrapper, v),
                 ref: t
-            }, x), p && a.a.createElement(a.a.Fragment, null, a.a.createElement(HD, {
+            }, x), p && a.a.createElement(a.a.Fragment, null, a.a.createElement(bI, {
                 value: I,
                 onChange: _,
                 color: T,
                 styles: O,
                 classNames: w,
                 size: d,
                 focusable: m,
                 saturationLabel: g,
                 __staticSelector: b
             }), a.a.createElement("div", {
                 className: S.body
             }, a.a.createElement("div", {
                 className: S.sliders
-            }, a.a.createElement(mD, {
+            }, a.a.createElement($D, {
                 value: I.h,
                 onChange: e => _({
                     h: e
                 }),
                 size: d,
                 styles: O,
                 classNames: w,
                 focusable: m,
                 "aria-label": y,
                 __staticSelector: b
-            }), z && a.a.createElement(RD, {
+            }), z && a.a.createElement(iI, {
                 value: I.a,
                 onChange: e => _({
                     a: e
                 }),
                 size: d,
-                color: WD("hex", I),
+                color: mI("hex", I),
                 style: {
                     marginTop: 6
                 },
                 styles: O,
                 classNames: w,
                 focusable: m,
                 "aria-label": h,
                 __staticSelector: b
-            })), z && a.a.createElement(WT, {
+            })), z && a.a.createElement(mD, {
                 color: T,
                 radius: "sm",
                 size: E.fn.size({
                     size: d,
-                    sizes: oI
+                    sizes: TI
                 }),
                 className: S.preview
-            }))), Array.isArray(c) && a.a.createElement(KD, {
+            }))), Array.isArray(c) && a.a.createElement(xI, {
                 data: c,
                 onSelect: _,
                 style: {
                     marginTop: 5
                 },
                 swatchesPerRow: u,
                 focusable: m,
                 classNames: w,
                 styles: O,
                 __staticSelector: b
             }))
         });
 
-    function sI() {
-        return (sI = Object.assign || function(e) {
+    function RI() {
+        return (RI = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    lI.displayName = "@mantine/core/ColorPicker";
-    var cI = function(e) {
+    II.displayName = "@mantine/core/ColorPicker";
+    var _I = function(e) {
         var t = e.setProps,
             r = e.class_name;
-        return a.a.createElement(lI, sI({
+        return a.a.createElement(II, RI({
             onChange: function(e) {
                 t({
                     value: e
                 })
             }
         }, G(["setProps", "class_name"], e), {
             className: r
         }))
     };
-    cI.displayName = "ColorPicker", cI.defaultProps = {
+    _I.displayName = "ColorPicker", _I.defaultProps = {
         persisted_props: ["value"],
         persistence_type: "local"
-    }, cI.propTypes = {
+    }, _I.propTypes = {
         class_name: i.a.string,
         focusable: i.a.bool,
         format: i.a.oneOf(["hex", "rgba", "rgb", "hsl", "hsla"]),
         fullWidth: i.a.bool,
         id: i.a.string,
         persistence: i.a.oneOfType([i.a.bool, i.a.string, i.a.number]),
         persisted_props: i.a.arrayOf(i.a.oneOf(["value"])),
@@ -26152,45 +26479,45 @@
         setProps: i.a.func,
         style: i.a.object,
         swatches: i.a.arrayOf(i.a.string),
         swatchesPerRow: i.a.number,
         value: i.a.string,
         withPicker: i.a.bool
     };
-    var uI = cI,
-        dI = function(e) {
+    var LI = _I,
+        AI = function(e) {
             return a.a.createElement(lr, G(["setProps", "children"], e), e.children)
         };
-    dI.displayName = "MantineProvider", dI.defaultProps = {}, dI.propTypes = {
+    AI.displayName = "MantineProvider", AI.defaultProps = {}, AI.propTypes = {
         children: i.a.node,
         id: i.a.string,
         inherit: i.a.bool,
         styles: i.a.object,
         theme: i.a.object,
         withNormalizeCSS: i.a.bool,
         withGlobalStyles: i.a.bool
     };
-    var pI = dI;
+    var MI = AI;
 
-    function fI() {
+    function FI() {
         return "undefined" != typeof window ? function() {
             const {
                 userAgent: e
             } = window.navigator;
             return /(Macintosh)|(MacIntel)|(MacPPC)|(Mac68K)/i.test(e) ? "macos" : /(iPhone)|(iPad)|(iPod)/i.test(e) ? "ios" : /(Win32)|(Win64)|(Windows)|(WinCE)/i.test(e) ? "windows" : /Android/i.test(e) ? "android" : /Linux/i.test(e) ? "linux" : "undetermined"
         }() : "undetermined"
     }
-    const mI = {
+    const $I = {
         xs: 20,
         sm: 24,
         md: 30,
         lg: 34,
         xl: 36
     };
-    var bI = Er((e, {
+    var BI = Er((e, {
         radius: t,
         size: r
     }) => ({
         rightSection: {
             display: "flex",
             flexDirection: "column",
             height: "calc(100% - 2px)",
@@ -26200,15 +26527,15 @@
         control: {
             margin: 0,
             position: "relative",
             flex: "0 0 50%",
             boxSizing: "border-box",
             width: e.fn.size({
                 size: r,
-                sizes: mI
+                sizes: $I
             }),
             padding: 0,
             WebkitTapHighlightColor: "transparent",
             borderBottom: "1px solid " + ("dark" === e.colorScheme ? e.colors.dark[4] : e.colors.gray[4]),
             borderLeft: "1px solid " + ("dark" === e.colorScheme ? e.colors.dark[4] : e.colors.gray[4]),
             borderTop: 0,
             borderRight: 0,
@@ -26252,41 +26579,41 @@
                 borderColor: ("dark" === e.colorScheme ? e.colors.dark[0] : e.black) + " transparent transparent transparent"
             },
             "&:disabled::after": {
                 borderTopColor: "dark" === e.colorScheme ? e.colors.dark[2] : e.colors.gray[5]
             }
         }
     }));
-    const gI = (e, t, r) => Number.isInteger(e) && e >= 0 && 0 === t ? "numeric" : !Number.isInteger(e) && e >= 0 && 0 !== t ? "decimal" : Number.isInteger(e) && e < 0 && 0 === t || !Number.isInteger(e) && e < 0 && 0 !== t ? "ios" === r ? "text" : "decimal" : "numeric";
-    var yI = Object.defineProperty,
-        hI = Object.defineProperties,
-        vI = Object.getOwnPropertyDescriptors,
-        OI = Object.getOwnPropertySymbols,
-        wI = Object.prototype.hasOwnProperty,
-        xI = Object.prototype.propertyIsEnumerable,
-        SI = (e, t, r) => t in e ? yI(e, t, {
+    const WI = (e, t, r) => Number.isInteger(e) && e >= 0 && 0 === t ? "numeric" : !Number.isInteger(e) && e >= 0 && 0 !== t ? "decimal" : Number.isInteger(e) && e < 0 && 0 === t || !Number.isInteger(e) && e < 0 && 0 !== t ? "ios" === r ? "text" : "decimal" : "numeric";
+    var HI = Object.defineProperty,
+        VI = Object.defineProperties,
+        qI = Object.getOwnPropertyDescriptors,
+        UI = Object.getOwnPropertySymbols,
+        GI = Object.prototype.hasOwnProperty,
+        YI = Object.prototype.propertyIsEnumerable,
+        ZI = (e, t, r) => t in e ? HI(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const kI = {
+    const KI = {
             step: 1,
             hideControls: !1,
             size: "sm",
             precision: 0,
             noClampOnBlur: !1,
             formatter: e => e || "",
             parser: e => {
                 const t = parseFloat(e);
                 if (!Number.isNaN(t)) return e
             }
         },
-        EI = Object(n.forwardRef)((e, t) => {
-            const r = ir("NumberInput", kI, e),
+        XI = Object(n.forwardRef)((e, t) => {
+            const r = ir("NumberInput", KI, e),
                 {
                     disabled: o,
                     value: i,
                     onChange: l,
                     decimalSeparator: s,
                     min: c,
                     max: u,
@@ -26307,24 +26634,24 @@
                     size: E,
                     rightSection: j,
                     formatter: P,
                     parser: z
                 } = r,
                 C = ((e, t) => {
                     var r = {};
-                    for (var n in e) wI.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && OI)
-                        for (var n of OI(e)) t.indexOf(n) < 0 && xI.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) GI.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && UI)
+                        for (var n of UI(e)) t.indexOf(n) < 0 && YI.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["disabled", "value", "onChange", "decimalSeparator", "min", "max", "step", "stepHoldInterval", "stepHoldDelay", "onBlur", "onFocus", "hideControls", "radius", "variant", "precision", "defaultValue", "noClampOnBlur", "handlersRef", "classNames", "styles", "size", "rightSection", "formatter", "parser"]),
                 {
                     classes: N,
                     cx: T,
                     theme: D
-                } = bI({
+                } = BI({
                     radius: y,
                     size: E
                 }, {
                     classNames: S,
                     styles: k,
                     name: "NumberInput"
                 }),
@@ -26413,18 +26740,18 @@
                 className: T(N.control, N.controlDown),
                 onMouseDown: e => {
                     Q(e, !1)
                 },
                 onMouseUp: K,
                 onMouseLeave: K
             }));
-            return a.a.createElement(bO, ((e, t) => hI(e, vI(t)))(((e, t) => {
-                for (var r in t || (t = {})) wI.call(t, r) && SI(e, r, t[r]);
-                if (OI)
-                    for (var r of OI(t)) xI.call(t, r) && SI(e, r, t[r]);
+            return a.a.createElement(bO, ((e, t) => VI(e, qI(t)))(((e, t) => {
+                for (var r in t || (t = {})) GI.call(t, r) && ZI(e, r, t[r]);
+                if (UI)
+                    for (var r of UI(t)) YI.call(t, r) && ZI(e, r, t[r]);
                 return e
             })({}, C), {
                 variant: h,
                 value: ((e = "") => {
                     let t = "number" == typeof e ? String(e) : e;
                     return s && (t = t.replace(/\./g, s)), P(t)
                 })(M),
@@ -26458,55 +26785,55 @@
                 },
                 onKeyUp: e => {
                     "ArrowUp" !== e.key && "ArrowDown" !== e.key || K()
                 },
                 rightSection: j || (o || g || "unstyled" === h ? null : ee),
                 rightSectionWidth: D.fn.size({
                     size: E,
-                    sizes: mI
+                    sizes: $I
                 }) + 1,
                 radius: y,
                 max: u,
                 min: c,
                 step: d,
                 size: E,
                 styles: k,
                 classNames: S,
-                inputMode: gI(d, v, fI()),
+                inputMode: WI(d, v, FI()),
                 __staticSelector: "NumberInput"
             }))
         });
 
-    function jI() {
-        return (jI = Object.assign || function(e) {
+    function JI() {
+        return (JI = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    EI.displayName = "@mantine/core/NumberInput";
-    var PI = function(e) {
+    XI.displayName = "@mantine/core/NumberInput";
+    var QI = function(e) {
         var t = e.setProps,
             r = e.class_name,
             n = G(["setProps", "class_name"], e);
         n = ta(n, ["label", "description", "rightSection", "icon", "error"]);
-        return a.a.createElement(EI, jI({}, n, {
+        return a.a.createElement(XI, JI({}, n, {
             className: r,
             onChange: function(e) {
                 return function(e) {
                     t({
                         value: e
                     })
                 }(e)
             }
         }))
     };
-    PI.displayName = "NumberInput", PI.defaultProps = {}, PI.propTypes = {
+    QI.displayName = "NumberInput", QI.defaultProps = {}, QI.propTypes = {
         class_name: i.a.string,
         decimalSeparator: i.a.string,
         description: i.a.any,
         disabled: i.a.bool,
         error: i.a.any,
         hideControls: i.a.bool,
         icon: i.a.any,
@@ -26526,178 +26853,178 @@
         step: i.a.number,
         style: i.a.object,
         stepHoldDelay: i.a.number,
         stepHoldInterval: i.a.number,
         value: i.a.node,
         variant: i.a.oneOf(["default", "filled", "unstyled", "headless"])
     };
-    var zI = PI;
+    var eR = QI;
 
-    function CI(e) {
+    function tR(e) {
         if ("string" == typeof e && 0 === e.trim().length) return !0;
         try {
             return JSON.parse(e), !0
         } catch (e) {
             return !1
         }
     }
-    var NI = Er((e, {
+    var rR = Er((e, {
             size: t
         }) => ({
             input: {
                 fontFamily: e.fontFamilyMonospace,
                 fontSize: e.fn.size({
                     size: t,
                     sizes: e.fontSizes
                 }) - 2
             }
         })),
-        TI = n.useLayoutEffect,
-        DI = function(e) {
+        nR = n.useLayoutEffect,
+        aR = function(e) {
             var t = Object(n.useRef)(e);
-            return TI((function() {
+            return nR((function() {
                 t.current = e
             })), t
         },
-        II = function(e, t) {
+        oR = function(e, t) {
             "function" != typeof e ? e.current = t : e(t)
         },
-        RI = function(e, t) {
+        iR = function(e, t) {
             var r = Object(n.useRef)();
             return Object(n.useCallback)((function(n) {
-                e.current = n, r.current && II(r.current, null), r.current = t, t && II(t, n)
+                e.current = n, r.current && oR(r.current, null), r.current = t, t && oR(t, n)
             }), [t])
         },
-        _I = {
+        lR = {
             "min-height": "0",
             "max-height": "none",
             height: "0",
             visibility: "hidden",
             overflow: "hidden",
             position: "absolute",
             "z-index": "-1000",
             top: "0",
             right: "0"
         },
-        LI = function(e) {
-            Object.keys(_I).forEach((function(t) {
-                e.style.setProperty(t, _I[t], "important")
+        sR = function(e) {
+            Object.keys(lR).forEach((function(t) {
+                e.style.setProperty(t, lR[t], "important")
             }))
         },
-        AI = null;
-    var MI = function() {},
-        FI = ["borderBottomWidth", "borderLeftWidth", "borderRightWidth", "borderTopWidth", "boxSizing", "fontFamily", "fontSize", "fontStyle", "fontWeight", "letterSpacing", "lineHeight", "paddingBottom", "paddingLeft", "paddingRight", "paddingTop", "tabSize", "textIndent", "textRendering", "textTransform", "width", "wordBreak"],
-        $I = !!document.documentElement.currentStyle,
-        BI = function(e, t) {
+        cR = null;
+    var uR = function() {},
+        dR = ["borderBottomWidth", "borderLeftWidth", "borderRightWidth", "borderTopWidth", "boxSizing", "fontFamily", "fontSize", "fontStyle", "fontWeight", "letterSpacing", "lineHeight", "paddingBottom", "paddingLeft", "paddingRight", "paddingTop", "tabSize", "textIndent", "textRendering", "textTransform", "width", "wordBreak"],
+        pR = !!document.documentElement.currentStyle,
+        fR = function(e, t) {
             var r = e.cacheMeasurements,
                 a = e.maxRows,
                 o = e.minRows,
                 i = e.onChange,
-                l = void 0 === i ? MI : i,
+                l = void 0 === i ? uR : i,
                 s = e.onHeightChange,
-                c = void 0 === s ? MI : s,
-                u = Yz(e, ["cacheMeasurements", "maxRows", "minRows", "onChange", "onHeightChange"]);
+                c = void 0 === s ? uR : s,
+                u = OC(e, ["cacheMeasurements", "maxRows", "minRows", "onChange", "onHeightChange"]);
             var d, p = void 0 !== u.value,
                 f = Object(n.useRef)(null),
-                m = RI(f, t),
+                m = iR(f, t),
                 b = Object(n.useRef)(0),
                 g = Object(n.useRef)(),
                 y = function() {
                     var e = f.current,
                         t = r && g.current ? g.current : function(e) {
                             var t = window.getComputedStyle(e);
                             if (null === t) return null;
-                            var r, n = (r = t, FI.reduce((function(e, t) {
+                            var r, n = (r = t, dR.reduce((function(e, t) {
                                     return e[t] = r[t], e
                                 }), {})),
                                 a = n.boxSizing;
-                            return "" === a ? null : ($I && "border-box" === a && (n.width = parseFloat(n.width) + parseFloat(n.borderRightWidth) + parseFloat(n.borderLeftWidth) + parseFloat(n.paddingRight) + parseFloat(n.paddingLeft) + "px"), {
+                            return "" === a ? null : (pR && "border-box" === a && (n.width = parseFloat(n.width) + parseFloat(n.borderRightWidth) + parseFloat(n.borderLeftWidth) + parseFloat(n.paddingRight) + parseFloat(n.paddingLeft) + "px"), {
                                 sizingStyle: n,
                                 paddingSize: parseFloat(n.paddingBottom) + parseFloat(n.paddingTop),
                                 borderSize: parseFloat(n.borderBottomWidth) + parseFloat(n.borderTopWidth)
                             })
                         }(e);
                     if (t) {
                         g.current = t;
                         var n = function(e, t, r, n) {
-                                void 0 === r && (r = 1), void 0 === n && (n = 1 / 0), AI || ((AI = document.createElement("textarea")).setAttribute("tabindex", "-1"), AI.setAttribute("aria-hidden", "true"), LI(AI)), null === AI.parentNode && document.body.appendChild(AI);
+                                void 0 === r && (r = 1), void 0 === n && (n = 1 / 0), cR || ((cR = document.createElement("textarea")).setAttribute("tabindex", "-1"), cR.setAttribute("aria-hidden", "true"), sR(cR)), null === cR.parentNode && document.body.appendChild(cR);
                                 var a = e.paddingSize,
                                     o = e.borderSize,
                                     i = e.sizingStyle,
                                     l = i.boxSizing;
                                 Object.keys(i).forEach((function(e) {
                                     var t = e;
-                                    AI.style[t] = i[t]
-                                })), LI(AI), AI.value = t;
+                                    cR.style[t] = i[t]
+                                })), sR(cR), cR.value = t;
                                 var s = function(e, t) {
                                     var r = e.scrollHeight;
                                     return "border-box" === t.sizingStyle.boxSizing ? r + t.borderSize : r - t.paddingSize
-                                }(AI, e);
-                                AI.value = "x";
-                                var c = AI.scrollHeight - a,
+                                }(cR, e);
+                                cR.value = "x";
+                                var c = cR.scrollHeight - a,
                                     u = c * r;
                                 "border-box" === l && (u = u + a + o), s = Math.max(u, s);
                                 var d = c * n;
                                 return "border-box" === l && (d = d + a + o), [s = Math.min(d, s), c]
                             }(t, e.value || e.placeholder || "x", o, a),
                             i = n[0],
                             l = n[1];
                         b.current !== i && (b.current = i, e.style.setProperty("height", i + "px", "important"), c(i, {
                             rowHeight: l
                         }))
                     }
                 };
-            return Object(n.useLayoutEffect)(y), d = DI(y), Object(n.useLayoutEffect)((function() {
+            return Object(n.useLayoutEffect)(y), d = aR(y), Object(n.useLayoutEffect)((function() {
                 var e = function(e) {
                     d.current(e)
                 };
                 return window.addEventListener("resize", e),
                     function() {
                         window.removeEventListener("resize", e)
                     }
             }), []), Object(n.createElement)("textarea", it({}, u, {
                 onChange: function(e) {
                     p || y(), l(e)
                 },
                 ref: m
             }))
         },
-        WI = Object(n.forwardRef)(BI),
-        HI = Er(e => ({
+        mR = Object(n.forwardRef)(fR),
+        bR = Er(e => ({
             input: {
                 paddingTop: e.spacing.xs,
                 paddingBottom: e.spacing.xs
             }
         })),
-        VI = Object.defineProperty,
-        qI = Object.defineProperties,
-        UI = Object.getOwnPropertyDescriptors,
-        GI = Object.getOwnPropertySymbols,
-        YI = Object.prototype.hasOwnProperty,
-        ZI = Object.prototype.propertyIsEnumerable,
-        KI = (e, t, r) => t in e ? VI(e, t, {
+        gR = Object.defineProperty,
+        yR = Object.defineProperties,
+        hR = Object.getOwnPropertyDescriptors,
+        vR = Object.getOwnPropertySymbols,
+        OR = Object.prototype.hasOwnProperty,
+        wR = Object.prototype.propertyIsEnumerable,
+        xR = (e, t, r) => t in e ? gR(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        XI = (e, t) => {
-            for (var r in t || (t = {})) YI.call(t, r) && KI(e, r, t[r]);
-            if (GI)
-                for (var r of GI(t)) ZI.call(t, r) && KI(e, r, t[r]);
+        SR = (e, t) => {
+            for (var r in t || (t = {})) OR.call(t, r) && xR(e, r, t[r]);
+            if (vR)
+                for (var r of vR(t)) wR.call(t, r) && xR(e, r, t[r]);
             return e
         },
-        JI = (e, t) => qI(e, UI(t));
-    const QI = {
+        kR = (e, t) => yR(e, hR(t));
+    const ER = {
             autosize: !1,
             size: "sm",
             __staticSelector: "Textarea"
         },
-        eR = Object(n.forwardRef)((e, t) => {
-            const r = ir("Textarea", QI, e),
+        jR = Object(n.forwardRef)((e, t) => {
+            const r = ir("Textarea", ER, e),
                 {
                     autosize: n,
                     maxRows: o,
                     minRows: i,
                     label: l,
                     error: s,
                     description: c,
@@ -26713,42 +27040,42 @@
                     sx: v,
                     errorProps: O,
                     descriptionProps: w,
                     labelProps: x
                 } = r,
                 S = ((e, t) => {
                     var r = {};
-                    for (var n in e) YI.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && GI)
-                        for (var n of GI(e)) t.indexOf(n) < 0 && ZI.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) OR.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && vR)
+                        for (var n of vR(e)) t.indexOf(n) < 0 && wR.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["autosize", "maxRows", "minRows", "label", "error", "description", "id", "className", "required", "style", "wrapperProps", "classNames", "styles", "size", "__staticSelector", "sx", "errorProps", "descriptionProps", "labelProps"]),
                 k = Ja(u),
                 {
                     classes: E,
                     cx: j
-                } = HI(),
+                } = bR(),
                 {
                     systemStyles: P,
                     rest: z
                 } = gn(S),
-                C = XI({
+                C = SR({
                     required: p,
                     ref: t,
                     invalid: !!s,
                     id: k,
-                    classNames: JI(XI({}, b), {
+                    classNames: kR(SR({}, b), {
                         input: j(E.input, null == b ? void 0 : b.input)
                     }),
                     styles: g,
                     __staticSelector: h,
                     size: y,
                     multiline: !0
                 }, z);
-            return a.a.createElement(Ao, XI(XI({
+            return a.a.createElement(Ao, SR(SR({
                 label: l,
                 error: s,
                 id: k,
                 description: c,
                 required: p,
                 style: f,
                 className: d,
@@ -26756,130 +27083,130 @@
                 styles: g,
                 size: y,
                 __staticSelector: h,
                 sx: v,
                 errorProps: O,
                 labelProps: x,
                 descriptionProps: w
-            }, P), m), n ? a.a.createElement(zc, JI(XI({}, C), {
-                component: WI,
+            }, P), m), n ? a.a.createElement(zc, kR(SR({}, C), {
+                component: mR,
                 maxRows: o,
                 minRows: i
-            })) : a.a.createElement(zc, JI(XI({}, C), {
+            })) : a.a.createElement(zc, kR(SR({}, C), {
                 component: "textarea",
                 rows: i
             })))
         });
-    eR.displayName = "@mantine/core/Textarea";
-    var tR = Object.defineProperty,
-        rR = Object.defineProperties,
-        nR = Object.getOwnPropertyDescriptors,
-        aR = Object.getOwnPropertySymbols,
-        oR = Object.prototype.hasOwnProperty,
-        iR = Object.prototype.propertyIsEnumerable,
-        lR = (e, t, r) => t in e ? tR(e, t, {
+    jR.displayName = "@mantine/core/Textarea";
+    var PR = Object.defineProperty,
+        zR = Object.defineProperties,
+        CR = Object.getOwnPropertyDescriptors,
+        NR = Object.getOwnPropertySymbols,
+        TR = Object.prototype.hasOwnProperty,
+        DR = Object.prototype.propertyIsEnumerable,
+        IR = (e, t, r) => t in e ? PR(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        sR = (e, t) => {
-            for (var r in t || (t = {})) oR.call(t, r) && lR(e, r, t[r]);
-            if (aR)
-                for (var r of aR(t)) iR.call(t, r) && lR(e, r, t[r]);
+        RR = (e, t) => {
+            for (var r in t || (t = {})) TR.call(t, r) && IR(e, r, t[r]);
+            if (NR)
+                for (var r of NR(t)) DR.call(t, r) && IR(e, r, t[r]);
             return e
         };
-    const cR = {
+    const _R = {
             formatOnBlur: !1,
             size: "sm"
         },
-        uR = Object(n.forwardRef)((e, t) => {
-            const r = ir("JsonInput", cR, e),
+        LR = Object(n.forwardRef)((e, t) => {
+            const r = ir("JsonInput", _R, e),
                 {
                     value: o,
                     defaultValue: i,
                     onChange: l,
                     onFocus: s,
                     onBlur: c,
                     error: u,
                     formatOnBlur: d,
                     size: p,
                     validationError: f,
                     classNames: m
                 } = r,
                 b = ((e, t) => {
                     var r = {};
-                    for (var n in e) oR.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && aR)
-                        for (var n of aR(e)) t.indexOf(n) < 0 && iR.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) TR.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && NR)
+                        for (var n of NR(e)) t.indexOf(n) < 0 && DR.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["value", "defaultValue", "onChange", "onFocus", "onBlur", "error", "formatOnBlur", "size", "validationError", "classNames"]),
                 {
                     classes: g,
                     cx: y
-                } = NI({
+                } = rR({
                     size: p
                 }, {
                     name: "JsonInput"
                 }),
                 [h, v] = la({
                     value: o,
                     defaultValue: i,
                     finalValue: "",
                     rule: e => "string" == typeof e,
                     onChange: l
                 }),
-                [O, w] = Object(n.useState)(CI(h));
-            return a.a.createElement(eR, sR({
+                [O, w] = Object(n.useState)(tR(h));
+            return a.a.createElement(jR, RR({
                 value: h,
                 onChange: e => v(e.currentTarget.value),
                 onFocus: e => {
                     "function" == typeof s && s(e), w(!0)
                 },
                 onBlur: e => {
                     "function" == typeof c && c(e);
-                    const t = CI(e.currentTarget.value);
+                    const t = tR(e.currentTarget.value);
                     d && t && "" !== e.currentTarget.value.trim() && v(JSON.stringify(JSON.parse(e.currentTarget.value), null, 2)), w(t)
                 },
                 error: O ? u : f || !0,
                 __staticSelector: "JsonInput",
-                classNames: (x = sR({}, m), S = {
+                classNames: (x = RR({}, m), S = {
                     input: y(g.input, null == m ? void 0 : m.input)
-                }, rR(x, nR(S))),
+                }, zR(x, CR(S))),
                 autoComplete: "nope",
                 ref: t
             }, b));
             var x, S
         });
 
-    function dR() {
-        return (dR = Object.assign || function(e) {
+    function AR() {
+        return (AR = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    uR.displayName = "@mantine/core/JsonInput";
-    var pR = function(e) {
+    LR.displayName = "@mantine/core/JsonInput";
+    var MR = function(e) {
         var t = e.class_name,
             r = e.setProps,
             n = G(["setProps", "class_name"], e);
         n = ta(n, ["icon", "rightSection", "validationError", "description", "error", "label"]);
-        return a.a.createElement(uR, dR({}, n, {
+        return a.a.createElement(LR, AR({}, n, {
             className: t,
             onChange: function(e) {
                 return r({
                     value: e
                 })
             }
         }))
     };
-    pR.displayName = "JsonInput", pR.defaultProps = {}, pR.propTypes = {
+    MR.displayName = "JsonInput", MR.defaultProps = {}, MR.propTypes = {
         autosize: i.a.bool,
         class_name: i.a.string,
         description: i.a.any,
         disabled: i.a.bool,
         error: i.a.any,
         formatOnBlur: i.a.bool,
         icon: i.a.any,
@@ -26896,41 +27223,41 @@
         setProps: i.a.func,
         size: i.a.oneOf(["xs", "sm", "md", "lg", "xl"]),
         style: i.a.object,
         validationError: i.a.any,
         value: i.a.string,
         variant: i.a.oneOf(["default", "filled", "unstyled", "headless"])
     };
-    var fR = pR,
-        mR = Object.defineProperty,
-        bR = Object.defineProperties,
-        gR = Object.getOwnPropertyDescriptors,
-        yR = Object.getOwnPropertySymbols,
-        hR = Object.prototype.hasOwnProperty,
-        vR = Object.prototype.propertyIsEnumerable,
-        OR = (e, t, r) => t in e ? mR(e, t, {
+    var FR = MR,
+        $R = Object.defineProperty,
+        BR = Object.defineProperties,
+        WR = Object.getOwnPropertyDescriptors,
+        HR = Object.getOwnPropertySymbols,
+        VR = Object.prototype.hasOwnProperty,
+        qR = Object.prototype.propertyIsEnumerable,
+        UR = (e, t, r) => t in e ? $R(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        wR = (e, t) => {
-            for (var r in t || (t = {})) hR.call(t, r) && OR(e, r, t[r]);
-            if (yR)
-                for (var r of yR(t)) vR.call(t, r) && OR(e, r, t[r]);
+        GR = (e, t) => {
+            for (var r in t || (t = {})) VR.call(t, r) && UR(e, r, t[r]);
+            if (HR)
+                for (var r of HR(t)) qR.call(t, r) && UR(e, r, t[r]);
             return e
         };
-    const xR = {
+    const YR = {
         xs: 16,
         sm: 20,
         md: 26,
         lg: 32,
         xl: 40
     };
-    var SR = Er((e, {
+    var ZR = Er((e, {
             color: t,
             size: r,
             radius: n,
             gradientFrom: a,
             gradientTo: o,
             gradientDeg: i,
             variant: l
@@ -26943,115 +27270,115 @@
                         from: a,
                         to: o,
                         deg: i
                     }
                 }),
                 c = e.fn.size({
                     size: r,
-                    sizes: xR
+                    sizes: YR
                 });
             return {
-                root: (u = wR({}, e.fn.fontStyles()), d = {
+                root: (u = GR({}, e.fn.fontStyles()), d = {
                     display: "inline-flex",
                     alignItems: "center",
                     justifyContent: "center",
                     boxSizing: "border-box",
                     width: c,
                     height: c,
                     minWidth: c,
                     minHeight: c,
                     borderRadius: e.fn.radius(n),
                     backgroundColor: s.background,
                     color: s.color,
                     backgroundImage: "gradient" === l ? s.background : null,
                     border: "1px solid " + s.border
-                }, bR(u, gR(d)))
+                }, BR(u, WR(d)))
             };
             var u, d
         }),
-        kR = Object.defineProperty,
-        ER = Object.getOwnPropertySymbols,
-        jR = Object.prototype.hasOwnProperty,
-        PR = Object.prototype.propertyIsEnumerable,
-        zR = (e, t, r) => t in e ? kR(e, t, {
+        KR = Object.defineProperty,
+        XR = Object.getOwnPropertySymbols,
+        JR = Object.prototype.hasOwnProperty,
+        QR = Object.prototype.propertyIsEnumerable,
+        e_ = (e, t, r) => t in e ? KR(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const CR = {
+    const t_ = {
             size: "md",
             variant: "filled",
             gradient: {
                 from: "blue",
                 to: "cyan",
                 deg: 45
             }
         },
-        NR = Object(n.forwardRef)((e, t) => {
-            const r = ir("ThemeIcon", CR, e),
+        r_ = Object(n.forwardRef)((e, t) => {
+            const r = ir("ThemeIcon", t_, e),
                 {
                     className: n,
                     size: o,
                     radius: i,
                     variant: l,
                     color: s,
                     children: c,
                     gradient: u
                 } = r,
                 d = ((e, t) => {
                     var r = {};
-                    for (var n in e) jR.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && ER)
-                        for (var n of ER(e)) t.indexOf(n) < 0 && PR.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) JR.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && XR)
+                        for (var n of XR(e)) t.indexOf(n) < 0 && QR.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["className", "size", "radius", "variant", "color", "children", "gradient"]),
                 {
                     classes: p,
                     cx: f
-                } = SR({
+                } = ZR({
                     variant: l,
                     radius: i,
                     color: s,
                     size: o,
                     gradientFrom: u.from,
                     gradientTo: u.to,
                     gradientDeg: u.deg
                 }, {
                     name: "ThemeIcon"
                 });
             return a.a.createElement(Cn, ((e, t) => {
-                for (var r in t || (t = {})) jR.call(t, r) && zR(e, r, t[r]);
-                if (ER)
-                    for (var r of ER(t)) PR.call(t, r) && zR(e, r, t[r]);
+                for (var r in t || (t = {})) JR.call(t, r) && e_(e, r, t[r]);
+                if (XR)
+                    for (var r of XR(t)) QR.call(t, r) && e_(e, r, t[r]);
                 return e
             })({
                 className: f(p.root, n),
                 ref: t
             }, d), c)
         });
 
-    function TR() {
-        return (TR = Object.assign || function(e) {
+    function n_() {
+        return (n_ = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    NR.displayName = "@mantine/core/ThemeIcon";
-    var DR = function(e) {
+    r_.displayName = "@mantine/core/ThemeIcon";
+    var a_ = function(e) {
         var t = e.class_name,
             r = e.children;
-        return a.a.createElement(NR, TR({}, G(["setProps", "children", "class_name"], e), {
+        return a.a.createElement(r_, n_({}, G(["setProps", "children", "class_name"], e), {
             className: t
         }), r)
     };
-    DR.displayName = "ThemeIcon", DR.defaultProps = {}, DR.propTypes = {
+    a_.displayName = "ThemeIcon", a_.defaultProps = {}, a_.propTypes = {
         children: i.a.node,
         class_name: i.a.string,
         color: i.a.oneOf(["dark", "gray", "red", "pink", "grape", "violet", "indigo", "blue", "cyan", "teal", "green", "lime", "yellow", "orange"]),
         gradient: i.a.exact({
             from: i.a.string,
             to: i.a.string,
             deg: i.a.number
@@ -27059,42 +27386,42 @@
         id: i.a.string,
         radius: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         setProps: i.a.func,
         size: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         style: i.a.object,
         variant: i.a.oneOf(["filled", "light", "gradient", "outline"])
     };
-    var IR = DR;
-    var RR = Object.defineProperty,
-        _R = Object.getOwnPropertySymbols,
-        LR = Object.prototype.hasOwnProperty,
-        AR = Object.prototype.propertyIsEnumerable,
-        MR = (e, t, r) => t in e ? RR(e, t, {
+    var o_ = a_;
+    var i_ = Object.defineProperty,
+        l_ = Object.getOwnPropertySymbols,
+        s_ = Object.prototype.hasOwnProperty,
+        c_ = Object.prototype.propertyIsEnumerable,
+        u_ = (e, t, r) => t in e ? i_(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
 
-    function FR({
+    function d_({
         size: e,
         value: t,
         offset: r,
         sum: n,
         thickness: o,
         root: i,
         color: l,
         lineRoundCaps: s
     }) {
         const c = or(),
             u = c.fn.themeColor(l || ("dark" === c.colorScheme ? "dark" : "gray"), l ? 6 : "dark" === c.colorScheme ? 4 : 1, !1);
         return a.a.createElement("circle", ((e, t) => {
-            for (var r in t || (t = {})) LR.call(t, r) && MR(e, r, t[r]);
-            if (_R)
-                for (var r of _R(t)) AR.call(t, r) && MR(e, r, t[r]);
+            for (var r in t || (t = {})) s_.call(t, r) && u_(e, r, t[r]);
+            if (l_)
+                for (var r of l_(t)) c_.call(t, r) && u_(e, r, t[r]);
             return e
         })({
             fill: "none",
             strokeLinecap: s ? "round" : "butt",
             stroke: u
         }, function({
             size: e,
@@ -27120,88 +27447,88 @@
             size: e,
             thickness: o,
             value: t,
             offset: r,
             root: i
         })))
     }
-    FR.displayName = "@mantine/core/Curve";
-    var $R = Object.defineProperty,
-        BR = Object.defineProperties,
-        WR = Object.getOwnPropertyDescriptors,
-        HR = Object.getOwnPropertySymbols,
-        VR = Object.prototype.hasOwnProperty,
-        qR = Object.prototype.propertyIsEnumerable,
-        UR = (e, t, r) => t in e ? $R(e, t, {
+    d_.displayName = "@mantine/core/Curve";
+    var p_ = Object.defineProperty,
+        f_ = Object.defineProperties,
+        m_ = Object.getOwnPropertyDescriptors,
+        b_ = Object.getOwnPropertySymbols,
+        g_ = Object.prototype.hasOwnProperty,
+        y_ = Object.prototype.propertyIsEnumerable,
+        h_ = (e, t, r) => t in e ? p_(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        GR = (e, t) => {
-            for (var r in t || (t = {})) VR.call(t, r) && UR(e, r, t[r]);
-            if (HR)
-                for (var r of HR(t)) qR.call(t, r) && UR(e, r, t[r]);
+        v_ = (e, t) => {
+            for (var r in t || (t = {})) g_.call(t, r) && h_(e, r, t[r]);
+            if (b_)
+                for (var r of b_(t)) y_.call(t, r) && h_(e, r, t[r]);
             return e
         },
-        YR = (e, t) => BR(e, WR(t));
-    var ZR = Er({
+        O_ = (e, t) => f_(e, m_(t));
+    var w_ = Er({
             root: {
                 position: "relative"
             },
             label: {
                 position: "absolute",
                 top: "50%",
                 transform: "translateY(-50%)"
             }
         }),
-        KR = Object.defineProperty,
-        XR = Object.getOwnPropertySymbols,
-        JR = Object.prototype.hasOwnProperty,
-        QR = Object.prototype.propertyIsEnumerable,
-        e_ = (e, t, r) => t in e ? KR(e, t, {
+        x_ = Object.defineProperty,
+        S_ = Object.getOwnPropertySymbols,
+        k_ = Object.prototype.hasOwnProperty,
+        E_ = Object.prototype.propertyIsEnumerable,
+        j_ = (e, t, r) => t in e ? x_(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        t_ = (e, t) => {
-            for (var r in t || (t = {})) JR.call(t, r) && e_(e, r, t[r]);
-            if (XR)
-                for (var r of XR(t)) QR.call(t, r) && e_(e, r, t[r]);
+        P_ = (e, t) => {
+            for (var r in t || (t = {})) k_.call(t, r) && j_(e, r, t[r]);
+            if (S_)
+                for (var r of S_(t)) E_.call(t, r) && j_(e, r, t[r]);
             return e
         };
-    const r_ = {
+    const z_ = {
             size: 120,
             thickness: 12
         },
-        n_ = Object(n.forwardRef)((e, t) => {
-            const r = ir("RingProgress", r_, e),
+        C_ = Object(n.forwardRef)((e, t) => {
+            const r = ir("RingProgress", z_, e),
                 {
                     className: n,
                     style: o,
                     label: i,
                     sections: l,
                     size: s,
                     thickness: c,
                     classNames: u,
                     styles: d,
                     roundCaps: p
                 } = r,
                 f = ((e, t) => {
                     var r = {};
-                    for (var n in e) JR.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && XR)
-                        for (var n of XR(e)) t.indexOf(n) < 0 && QR.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) k_.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && S_)
+                        for (var n of S_(e)) t.indexOf(n) < 0 && E_.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["className", "style", "label", "sections", "size", "thickness", "classNames", "styles", "roundCaps"]),
                 {
                     classes: m,
                     cx: b
-                } = ZR(null, {
+                } = w_(null, {
                     classNames: u,
                     styles: d,
                     name: "RingProgress"
                 }),
                 g = function({
                     size: e,
                     thickness: t,
@@ -27220,50 +27547,50 @@
                         root: !1
                     }), i -= r[e].value / 100 * o;
                     if (l.push({
                             sum: a,
                             offset: i,
                             data: null,
                             root: !0
-                        }), s.push(YR(GR({}, l[l.length - 1]), {
+                        }), s.push(O_(v_({}, l[l.length - 1]), {
                             lineRoundCaps: !1
                         })), l.length > 2) {
-                        s.push(YR(GR({}, l[0]), {
+                        s.push(O_(v_({}, l[0]), {
                             lineRoundCaps: n
-                        })), s.push(YR(GR({}, l[l.length - 2]), {
+                        })), s.push(O_(v_({}, l[l.length - 2]), {
                             lineRoundCaps: n
                         }));
-                        for (let e = 1; e <= l.length - 3; e += 1) s.push(YR(GR({}, l[e]), {
+                        for (let e = 1; e <= l.length - 3; e += 1) s.push(O_(v_({}, l[e]), {
                             lineRoundCaps: !1
                         }))
-                    } else s.push(YR(GR({}, l[0]), {
+                    } else s.push(O_(v_({}, l[0]), {
                         lineRoundCaps: n
                     }));
                     return s
                 }({
                     size: s,
                     thickness: c,
                     sections: l,
                     renderRoundedLineCaps: p
                 }).map((e, t) => {
                     var r, n;
-                    return a.a.createElement(FR, {
+                    return a.a.createElement(d_, {
                         key: t,
                         value: null == (r = e.data) ? void 0 : r.value,
                         size: s,
                         thickness: c,
                         sum: e.sum,
                         offset: e.offset,
                         color: null == (n = e.data) ? void 0 : n.color,
                         root: e.root,
                         lineRoundCaps: e.lineRoundCaps
                     })
                 });
-            return a.a.createElement(Cn, t_({
-                style: t_({
+            return a.a.createElement(Cn, P_({
+                style: P_({
                     width: s,
                     height: s
                 }, o),
                 className: b(m.root, n),
                 ref: t
             }, f), a.a.createElement("svg", {
                 width: s,
@@ -27276,58 +27603,58 @@
                 style: {
                     right: 2 * c,
                     left: 2 * c
                 }
             }, i))
         });
 
-    function a_() {
-        return (a_ = Object.assign || function(e) {
+    function N_() {
+        return (N_ = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    n_.displayName = "@mantine/core/RingProgress";
-    var o_ = function(e) {
+    C_.displayName = "@mantine/core/RingProgress";
+    var T_ = function(e) {
         var t = e.class_name,
             r = G(["setProps", "class_name"], e);
-        return r.label = ea(r.label), a.a.createElement(n_, a_({}, r, {
+        return r.label = ea(r.label), a.a.createElement(C_, N_({}, r, {
             className: t
         }))
     };
-    o_.displayName = "RingProgress", o_.defaultProps = {}, o_.propTypes = {
+    T_.displayName = "RingProgress", T_.defaultProps = {}, T_.propTypes = {
         class_name: i.a.string,
         id: i.a.string,
         label: i.a.any,
         roundCaps: i.a.bool,
         sections: i.a.arrayOf(i.a.exact({
             value: i.a.number.isRequired,
             color: i.a.oneOfType([i.a.oneOf(["dark", "gray", "red", "pink", "grape", "violet", "indigo", "blue", "cyan", "teal", "green", "lime", "yellow", "orange"]), i.a.string]).isRequired
         })).isRequired,
         setProps: i.a.func,
         size: i.a.number,
         style: i.a.object,
         thickness: i.a.number
     };
-    var i_ = o_;
+    var D_ = T_;
 
-    function l_() {
-        return (l_ = Object.assign || function(e) {
+    function I_() {
+        return (I_ = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
 
-    function s_(e, t) {
+    function R_(e, t) {
         return function(e) {
             if (Array.isArray(e)) return e
         }(e) || function(e, t) {
             var r = null == e ? null : "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
             if (null == r) return;
             var n, a, o = [],
                 i = !0,
@@ -27342,54 +27669,54 @@
                 } finally {
                     if (l) throw a
                 }
             }
             return o
         }(e, t) || function(e, t) {
             if (!e) return;
-            if ("string" == typeof e) return c_(e, t);
+            if ("string" == typeof e) return __(e, t);
             var r = Object.prototype.toString.call(e).slice(8, -1);
             "Object" === r && e.constructor && (r = e.constructor.name);
             if ("Map" === r || "Set" === r) return Array.from(e);
-            if ("Arguments" === r || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(r)) return c_(e, t)
+            if ("Arguments" === r || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(r)) return __(e, t)
         }(e, t) || function() {
             throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()
     }
 
-    function c_(e, t) {
+    function __(e, t) {
         (null == t || t > e.length) && (t = e.length);
         for (var r = 0, n = new Array(t); r < t; r++) n[r] = e[r];
         return n
     }
-    var u_ = function(e) {
+    var L_ = function(e) {
         var t = e.class_name,
             r = e.value,
             o = e.setProps,
-            i = s_(Object(n.useState)(r && new Date(r)), 2),
+            i = R_(Object(n.useState)(r && new Date(r)), 2),
             l = i[0],
             s = i[1];
         _u((function() {
             s(r && new Date(r))
         }), [r]);
         var c = G(["setProps", "class_name", "persistence", "persisted_props", "persistence_type"], e);
-        return c = ta(c, ["icon", "rightSection", "description", "error", "label"]), a.a.createElement(em, l_({}, c, {
+        return c = ta(c, ["icon", "rightSection", "description", "error", "label"]), a.a.createElement(em, I_({}, c, {
             className: t,
             onChange: function(e) {
                 o({
                     value: e && Si()(e).format("YYYY-MM-DDTHH:mm:ss")
                 })
             },
             value: l
         }))
     };
-    u_.displayName = "TimeInput", u_.defaultProps = {
+    L_.displayName = "TimeInput", L_.defaultProps = {
         persisted_props: ["value"],
         persistence_type: "local"
-    }, u_.propTypes = {
+    }, L_.propTypes = {
         amPmPlaceholder: i.a.string,
         class_name: i.a.string,
         clearable: i.a.bool,
         description: i.a.any,
         disabled: i.a.bool,
         error: i.a.any,
         format: i.a.oneOf(["12", "24"]),
@@ -27408,78 +27735,78 @@
         size: i.a.oneOf(["xs", "sm", "md", "lg", "xl"]),
         style: i.a.object,
         timePlaceholder: i.a.string,
         value: i.a.string,
         variant: i.a.oneOf(["default", "filled", "unstyled", "headless"]),
         withSeconds: i.a.bool
     };
-    var d_ = u_;
+    var A_ = L_;
 
-    function p_() {
-        return (p_ = Object.assign || function(e) {
+    function M_() {
+        return (M_ = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    var f_ = function(e) {
+    var F_ = function(e) {
         var t = e.class_name;
-        return a.a.createElement(Mn, p_({}, G(["setProps", "class_name"], e), {
+        return a.a.createElement(Mn, M_({}, G(["setProps", "class_name"], e), {
             className: t
         }))
     };
-    f_.displayName = "Loader", f_.defaultProps = {}, f_.propTypes = {
+    F_.displayName = "Loader", F_.defaultProps = {}, F_.propTypes = {
         class_name: i.a.string,
         id: i.a.string,
         color: i.a.oneOf(["dark", "gray", "red", "pink", "grape", "violet", "indigo", "blue", "cyan", "teal", "green", "lime", "yellow", "orange"]),
         size: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         style: i.a.object,
         variant: i.a.oneOf(["bars", "oval", "dots"])
     };
-    var m_ = f_,
-        b_ = Er({
+    var $_ = F_,
+        B_ = Er({
             root: {
                 position: "absolute",
                 top: 0,
                 left: 0,
                 right: 0,
                 bottom: 0,
                 display: "flex",
                 alignItems: "center",
                 justifyContent: "center",
                 overflow: "hidden"
             }
         }),
-        g_ = Object.defineProperty,
-        y_ = Object.defineProperties,
-        h_ = Object.getOwnPropertyDescriptors,
-        v_ = Object.getOwnPropertySymbols,
-        O_ = Object.prototype.hasOwnProperty,
-        w_ = Object.prototype.propertyIsEnumerable,
-        x_ = (e, t, r) => t in e ? g_(e, t, {
+        W_ = Object.defineProperty,
+        H_ = Object.defineProperties,
+        V_ = Object.getOwnPropertyDescriptors,
+        q_ = Object.getOwnPropertySymbols,
+        U_ = Object.prototype.hasOwnProperty,
+        G_ = Object.prototype.propertyIsEnumerable,
+        Y_ = (e, t, r) => t in e ? W_(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        S_ = (e, t) => {
-            for (var r in t || (t = {})) O_.call(t, r) && x_(e, r, t[r]);
-            if (v_)
-                for (var r of v_(t)) w_.call(t, r) && x_(e, r, t[r]);
+        Z_ = (e, t) => {
+            for (var r in t || (t = {})) U_.call(t, r) && Y_(e, r, t[r]);
+            if (q_)
+                for (var r of q_(t)) G_.call(t, r) && Y_(e, r, t[r]);
             return e
         };
-    const k_ = {
+    const K_ = {
             overlayOpacity: .75,
             transitionDuration: 200,
             zIndex: ac("overlay")
         },
-        E_ = Object(n.forwardRef)((e, t) => {
-            const r = ir("LoadingOverlay", k_, e),
+        X_ = Object(n.forwardRef)((e, t) => {
+            const r = ir("LoadingOverlay", K_, e),
                 {
                     className: n,
                     visible: o,
                     loaderProps: i,
                     overlayOpacity: l,
                     overlayColor: s,
                     transitionDuration: c,
@@ -27488,85 +27815,85 @@
                     loader: p,
                     radius: f,
                     classNames: m,
                     styles: b
                 } = r,
                 g = ((e, t) => {
                     var r = {};
-                    for (var n in e) O_.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && v_)
-                        for (var n of v_(e)) t.indexOf(n) < 0 && w_.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) U_.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && q_)
+                        for (var n of q_(e)) t.indexOf(n) < 0 && G_.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["className", "visible", "loaderProps", "overlayOpacity", "overlayColor", "transitionDuration", "zIndex", "style", "loader", "radius", "classNames", "styles"]),
                 {
                     classes: y,
                     cx: h,
                     theme: v
-                } = b_(null, {
+                } = B_(null, {
                     name: "LoadingOverlay",
                     classNames: m,
                     styles: b
                 });
             return a.a.createElement(wd, {
                 duration: c,
                 mounted: o,
                 transition: "fade"
             }, e => {
-                return a.a.createElement(Cn, S_({
+                return a.a.createElement(Cn, Z_({
                     className: h(y.root, n),
-                    style: (r = S_(S_({}, e), d), o = {
+                    style: (r = Z_(Z_({}, e), d), o = {
                         zIndex: u
-                    }, y_(r, h_(o))),
+                    }, H_(r, V_(o))),
                     ref: t
                 }, g), p ? a.a.createElement("div", {
                     style: {
                         zIndex: u + 1
                     }
-                }, p) : a.a.createElement(Mn, S_({
+                }, p) : a.a.createElement(Mn, Z_({
                     style: {
                         zIndex: u + 1
                     }
                 }, i)), a.a.createElement(bp, {
                     opacity: l,
                     zIndex: u,
                     radius: f,
                     color: s || ("dark" === v.colorScheme ? v.colors.dark[5] : v.white)
                 }));
                 var r, o
             })
         });
 
-    function j_() {
-        return (j_ = Object.assign || function(e) {
+    function J_() {
+        return (J_ = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    E_.displayName = "@mantine/core/LoadingOverlay";
-    var P_ = function(e) {
+    X_.displayName = "@mantine/core/LoadingOverlay";
+    var Q_ = function(e) {
         var t = e.loading_state,
             r = e.class_name,
             n = e.id,
             o = e.children,
             i = e.style,
             l = U({
                 position: "relative"
             }, i);
         return a.a.createElement("div", {
             className: r,
             id: n,
             style: l
-        }, a.a.createElement(E_, j_({}, G(["setProps", "id", "class_name", "children"], e), {
+        }, a.a.createElement(X_, J_({}, G(["setProps", "id", "class_name", "children"], e), {
             visible: t && t.is_loading
         })), o)
     };
-    P_.displayName = "LoadingOverlay", P_._dashprivate_isLoadingComponent = !0, P_.defaultProps = {}, P_.propTypes = {
+    Q_.displayName = "LoadingOverlay", Q_._dashprivate_isLoadingComponent = !0, Q_.defaultProps = {}, Q_.propTypes = {
         children: i.a.node,
         class_name: i.a.string,
         id: i.a.string,
         loader: i.a.node,
         loaderProps: i.a.exact({
             color: i.a.oneOf(["dark", "gray", "red", "pink", "grape", "violet", "indigo", "blue", "cyan", "teal", "green", "lime", "yellow", "orange"]),
             size: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
@@ -27580,108 +27907,108 @@
         overlayColor: i.a.string,
         overlayOpacity: i.a.number,
         radius: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         style: i.a.object,
         transitionDuration: i.a.number,
         zIndex: i.a.number
     };
-    var z_ = P_,
-        C_ = Object.defineProperty,
-        N_ = Object.defineProperties,
-        T_ = Object.getOwnPropertyDescriptors,
-        D_ = Object.getOwnPropertySymbols,
-        I_ = Object.prototype.hasOwnProperty,
-        R_ = Object.prototype.propertyIsEnumerable,
-        __ = (e, t, r) => t in e ? C_(e, t, {
+    var eL = Q_,
+        tL = Object.defineProperty,
+        rL = Object.defineProperties,
+        nL = Object.getOwnPropertyDescriptors,
+        aL = Object.getOwnPropertySymbols,
+        oL = Object.prototype.hasOwnProperty,
+        iL = Object.prototype.propertyIsEnumerable,
+        lL = (e, t, r) => t in e ? tL(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
 
-    function L_(e) {
-        return a.a.createElement("svg", ((e, t) => N_(e, T_(t)))(((e, t) => {
-            for (var r in t || (t = {})) I_.call(t, r) && __(e, r, t[r]);
-            if (D_)
-                for (var r of D_(t)) R_.call(t, r) && __(e, r, t[r]);
+    function sL(e) {
+        return a.a.createElement("svg", ((e, t) => rL(e, nL(t)))(((e, t) => {
+            for (var r in t || (t = {})) oL.call(t, r) && lL(e, r, t[r]);
+            if (aL)
+                for (var r of aL(t)) iL.call(t, r) && lL(e, r, t[r]);
             return e
         })({}, e), {
             width: "15",
             height: "15",
             viewBox: "0 0 15 15",
             fill: "none",
             xmlns: "http://www.w3.org/2000/svg"
         }), a.a.createElement("path", {
             d: "M0.877014 7.49988C0.877014 3.84219 3.84216 0.877045 7.49985 0.877045C11.1575 0.877045 14.1227 3.84219 14.1227 7.49988C14.1227 11.1575 11.1575 14.1227 7.49985 14.1227C3.84216 14.1227 0.877014 11.1575 0.877014 7.49988ZM7.49985 1.82704C4.36683 1.82704 1.82701 4.36686 1.82701 7.49988C1.82701 8.97196 2.38774 10.3131 3.30727 11.3213C4.19074 9.94119 5.73818 9.02499 7.50023 9.02499C9.26206 9.02499 10.8093 9.94097 11.6929 11.3208C12.6121 10.3127 13.1727 8.97172 13.1727 7.49988C13.1727 4.36686 10.6328 1.82704 7.49985 1.82704ZM10.9818 11.9787C10.2839 10.7795 8.9857 9.97499 7.50023 9.97499C6.01458 9.97499 4.71624 10.7797 4.01845 11.9791C4.97952 12.7272 6.18765 13.1727 7.49985 13.1727C8.81227 13.1727 10.0206 12.727 10.9818 11.9787ZM5.14999 6.50487C5.14999 5.207 6.20212 4.15487 7.49999 4.15487C8.79786 4.15487 9.84999 5.207 9.84999 6.50487C9.84999 7.80274 8.79786 8.85487 7.49999 8.85487C6.20212 8.85487 5.14999 7.80274 5.14999 6.50487ZM7.49999 5.10487C6.72679 5.10487 6.09999 5.73167 6.09999 6.50487C6.09999 7.27807 6.72679 7.90487 7.49999 7.90487C8.27319 7.90487 8.89999 7.27807 8.89999 6.50487C8.89999 5.73167 8.27319 5.10487 7.49999 5.10487Z",
             fill: "currentColor",
             fillRule: "evenodd",
             clipRule: "evenodd"
         }))
     }
-    var A_ = Object.defineProperty,
-        M_ = Object.defineProperties,
-        F_ = Object.getOwnPropertyDescriptors,
-        $_ = Object.getOwnPropertySymbols,
-        B_ = Object.prototype.hasOwnProperty,
-        W_ = Object.prototype.propertyIsEnumerable,
-        H_ = (e, t, r) => t in e ? A_(e, t, {
+    var cL = Object.defineProperty,
+        uL = Object.defineProperties,
+        dL = Object.getOwnPropertyDescriptors,
+        pL = Object.getOwnPropertySymbols,
+        fL = Object.prototype.hasOwnProperty,
+        mL = Object.prototype.propertyIsEnumerable,
+        bL = (e, t, r) => t in e ? cL(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        V_ = (e, t) => {
-            for (var r in t || (t = {})) B_.call(t, r) && H_(e, r, t[r]);
-            if ($_)
-                for (var r of $_(t)) W_.call(t, r) && H_(e, r, t[r]);
+        gL = (e, t) => {
+            for (var r in t || (t = {})) fL.call(t, r) && bL(e, r, t[r]);
+            if (pL)
+                for (var r of pL(t)) mL.call(t, r) && bL(e, r, t[r]);
             return e
         },
-        q_ = (e, t) => M_(e, F_(t));
-    const U_ = {
+        yL = (e, t) => uL(e, dL(t));
+    const hL = {
         xs: 16,
         sm: 26,
         md: 38,
         lg: 56,
         xl: 84
     };
-    var G_ = Er((e, {
+    var vL = Er((e, {
             size: t,
             radius: r,
             color: n
         }) => ({
-            root: q_(V_({}, e.fn.focusStyles()), {
+            root: yL(gL({}, e.fn.focusStyles()), {
                 WebkitTapHighlightColor: "transparent",
                 boxSizing: "border-box",
                 position: "relative",
                 userSelect: "none",
                 overflow: "hidden",
                 width: e.fn.size({
                     size: t,
-                    sizes: U_
+                    sizes: hL
                 }),
                 minWidth: e.fn.size({
                     size: t,
-                    sizes: U_
+                    sizes: hL
                 }),
                 height: e.fn.size({
                     size: t,
-                    sizes: U_
+                    sizes: hL
                 }),
                 borderRadius: e.fn.radius(r)
             }),
             image: {
                 objectFit: "cover",
                 width: "100%",
                 height: "100%",
                 display: "block"
             },
-            placeholder: q_(V_({}, e.fn.fontStyles()), {
+            placeholder: yL(gL({}, e.fn.fontStyles()), {
                 fontSize: e.fn.size({
                     size: t,
-                    sizes: U_
+                    sizes: hL
                 }) / 2.5,
                 color: dr({
                     theme: e,
                     color: n,
                     variant: "light"
                 }).color,
                 fontWeight: 700,
@@ -27703,38 +28030,38 @@
                 color: dr({
                     theme: e,
                     color: n,
                     variant: "light"
                 }).color
             }
         })),
-        Y_ = Object.defineProperty,
-        Z_ = Object.defineProperties,
-        K_ = Object.getOwnPropertyDescriptors,
-        X_ = Object.getOwnPropertySymbols,
-        J_ = Object.prototype.hasOwnProperty,
-        Q_ = Object.prototype.propertyIsEnumerable,
-        eL = (e, t, r) => t in e ? Y_(e, t, {
+        OL = Object.defineProperty,
+        wL = Object.defineProperties,
+        xL = Object.getOwnPropertyDescriptors,
+        SL = Object.getOwnPropertySymbols,
+        kL = Object.prototype.hasOwnProperty,
+        EL = Object.prototype.propertyIsEnumerable,
+        jL = (e, t, r) => t in e ? OL(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        tL = (e, t) => {
-            for (var r in t || (t = {})) J_.call(t, r) && eL(e, r, t[r]);
-            if (X_)
-                for (var r of X_(t)) Q_.call(t, r) && eL(e, r, t[r]);
+        PL = (e, t) => {
+            for (var r in t || (t = {})) kL.call(t, r) && jL(e, r, t[r]);
+            if (SL)
+                for (var r of SL(t)) EL.call(t, r) && jL(e, r, t[r]);
             return e
         };
-    const rL = {
+    const zL = {
             size: "md",
             color: "gray"
         },
-        nL = Object(n.forwardRef)((e, t) => {
-            const r = ir("Avatar", rL, e),
+        CL = Object(n.forwardRef)((e, t) => {
+            const r = ir("Avatar", zL, e),
                 {
                     component: o,
                     className: i,
                     size: l,
                     src: s,
                     alt: c,
                     radius: u,
@@ -27742,100 +28069,100 @@
                     color: p,
                     classNames: f,
                     styles: m,
                     imageProps: b
                 } = r,
                 g = ((e, t) => {
                     var r = {};
-                    for (var n in e) J_.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && X_)
-                        for (var n of X_(e)) t.indexOf(n) < 0 && Q_.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) kL.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && SL)
+                        for (var n of SL(e)) t.indexOf(n) < 0 && EL.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["component", "className", "size", "src", "alt", "radius", "children", "color", "classNames", "styles", "imageProps"]),
                 {
                     classes: y,
                     cx: h
-                } = G_({
+                } = vL({
                     color: p,
                     radius: u,
                     size: l
                 }, {
                     classNames: f,
                     styles: m,
                     name: "Avatar"
                 }),
                 [v, O] = Object(n.useState)(!s);
             return Object(n.useEffect)(() => {
                 O(!s)
-            }, [s]), a.a.createElement(Cn, tL({
+            }, [s]), a.a.createElement(Cn, PL({
                 component: o || "div",
                 className: h(y.root, i),
                 ref: t
             }, g), v ? a.a.createElement("div", {
                 className: y.placeholder,
                 title: c
-            }, d || a.a.createElement(L_, {
+            }, d || a.a.createElement(sL, {
                 className: y.placeholderIcon
-            })) : a.a.createElement("img", (w = tL({}, b), x = {
+            })) : a.a.createElement("img", (w = PL({}, b), x = {
                 className: y.image,
                 src: s,
                 alt: c,
                 onError: () => O(!0)
-            }, Z_(w, K_(x)))));
+            }, wL(w, xL(x)))));
             var w, x
         });
 
-    function aL() {
-        return (aL = Object.assign || function(e) {
+    function NL() {
+        return (NL = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    nL.displayName = "@mantine/core/Avatar";
-    var oL = function(e) {
+    CL.displayName = "@mantine/core/Avatar";
+    var TL = function(e) {
         var t = e.class_name,
             r = e.children;
-        return React.createElement(nL, aL({}, G(["setProps", "class_name"], e), {
+        return React.createElement(CL, NL({}, G(["setProps", "class_name"], e), {
             className: t
         }), r)
     };
-    oL.displayName = "Avatar", oL.defaultProps = {}, oL.propTypes = {
+    TL.displayName = "Avatar", TL.defaultProps = {}, TL.propTypes = {
         alt: i.a.string,
         children: i.a.node,
         class_name: i.a.string,
         color: i.a.oneOf(["dark", "gray", "red", "pink", "grape", "violet", "indigo", "blue", "cyan", "teal", "green", "lime", "yellow", "orange"]),
         id: i.a.string,
         radius: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         size: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         src: i.a.string,
         style: i.a.object
     };
-    var iL = oL,
-        lL = Object.defineProperty,
-        sL = Object.defineProperties,
-        cL = Object.getOwnPropertyDescriptors,
-        uL = Object.getOwnPropertySymbols,
-        dL = Object.prototype.hasOwnProperty,
-        pL = Object.prototype.propertyIsEnumerable,
-        fL = (e, t, r) => t in e ? lL(e, t, {
+    var DL = TL,
+        IL = Object.defineProperty,
+        RL = Object.defineProperties,
+        _L = Object.getOwnPropertyDescriptors,
+        LL = Object.getOwnPropertySymbols,
+        AL = Object.prototype.hasOwnProperty,
+        ML = Object.prototype.propertyIsEnumerable,
+        FL = (e, t, r) => t in e ? IL(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        mL = (e, t) => {
-            for (var r in t || (t = {})) dL.call(t, r) && fL(e, r, t[r]);
-            if (uL)
-                for (var r of uL(t)) pL.call(t, r) && fL(e, r, t[r]);
+        $L = (e, t) => {
+            for (var r in t || (t = {})) AL.call(t, r) && FL(e, r, t[r]);
+            if (LL)
+                for (var r of LL(t)) ML.call(t, r) && FL(e, r, t[r]);
             return e
         },
-        bL = Er((e, {
+        BL = Er((e, {
             spacing: t
         }) => {
             return {
                 root: {
                     display: "flex",
                     paddingLeft: e.fn.size({
                         size: t,
@@ -27846,371 +28173,371 @@
                     marginLeft: -e.fn.size({
                         size: t,
                         sizes: e.spacing
                     }) / 2,
                     background: "" + ("dark" === e.colorScheme ? e.colors.dark[7] : e.white),
                     border: "2px solid " + ("dark" === e.colorScheme ? e.colors.dark[7] : e.white)
                 },
-                truncated: (r = mL({}, e.fn.fontStyles()), n = {
+                truncated: (r = $L({}, e.fn.fontStyles()), n = {
                     lineHeight: 1,
                     fontSize: e.fontSizes.sm + "px !important",
                     color: "dark" === e.colorScheme ? e.colors.dark[0] : e.black,
                     width: "100%",
                     height: "100%",
                     backgroundColor: "dark" === e.colorScheme ? e.colors.dark[5] : e.colors.gray[0]
-                }, sL(r, cL(n)))
+                }, RL(r, _L(n)))
             };
             var r, n
         }),
-        gL = Object.defineProperty,
-        yL = Object.defineProperties,
-        hL = Object.getOwnPropertyDescriptors,
-        vL = Object.getOwnPropertySymbols,
-        OL = Object.prototype.hasOwnProperty,
-        wL = Object.prototype.propertyIsEnumerable,
-        xL = (e, t, r) => t in e ? gL(e, t, {
+        WL = Object.defineProperty,
+        HL = Object.defineProperties,
+        VL = Object.getOwnPropertyDescriptors,
+        qL = Object.getOwnPropertySymbols,
+        UL = Object.prototype.hasOwnProperty,
+        GL = Object.prototype.propertyIsEnumerable,
+        YL = (e, t, r) => t in e ? WL(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        SL = (e, t) => {
-            for (var r in t || (t = {})) OL.call(t, r) && xL(e, r, t[r]);
-            if (vL)
-                for (var r of vL(t)) wL.call(t, r) && xL(e, r, t[r]);
+        ZL = (e, t) => {
+            for (var r in t || (t = {})) UL.call(t, r) && YL(e, r, t[r]);
+            if (qL)
+                for (var r of qL(t)) GL.call(t, r) && YL(e, r, t[r]);
             return e
         };
-    const kL = {
+    const KL = {
             size: "md",
             radius: "xl",
             limit: 2,
             spacing: "lg"
         },
-        EL = Object(n.forwardRef)((e, t) => {
-            const r = ir("AvatarsGroup", kL, e),
+        XL = Object(n.forwardRef)((e, t) => {
+            const r = ir("AvatarsGroup", KL, e),
                 {
                     className: n,
                     children: o,
                     size: i = "md",
                     radius: l = "xl",
                     limit: s = 2,
                     classNames: c,
                     styles: u,
                     spacing: d = "lg",
                     total: p
                 } = r,
                 f = ((e, t) => {
                     var r = {};
-                    for (var n in e) OL.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && vL)
-                        for (var n of vL(e)) t.indexOf(n) < 0 && wL.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) UL.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && qL)
+                        for (var n of qL(e)) t.indexOf(n) < 0 && GL.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["className", "children", "size", "radius", "limit", "classNames", "styles", "spacing", "total"]),
                 {
                     classes: m,
                     cx: b
-                } = bL({
+                } = BL({
                     spacing: d
                 }, {
                     classNames: c,
                     styles: u,
                     name: "AvatarsGroup"
                 }),
-                g = si(o, nL).map((e, t) => {
+                g = si(o, CL).map((e, t) => {
                     return a.a.cloneElement(e, {
                         size: i,
                         radius: l,
                         key: t,
                         className: b(m.child, e.props.className),
-                        style: (r = SL({}, e.props.style), n = {
+                        style: (r = ZL({}, e.props.style), n = {
                             zIndex: t + 1
-                        }, yL(r, hL(n)))
+                        }, HL(r, VL(n)))
                     });
                     var r, n
                 }),
                 y = s < 2 ? 2 : s,
                 h = g.length > y ? g.length - y : 0,
                 v = p ? p - Math.min(g.length, y) : h;
-            return a.a.createElement(Cn, SL({
+            return a.a.createElement(Cn, ZL({
                 className: b(n, m.root),
                 ref: t
-            }, f), g.slice(0, g.length - h), v ? a.a.createElement(nL, {
+            }, f), g.slice(0, g.length - h), v ? a.a.createElement(CL, {
                 size: i,
                 radius: l,
                 className: m.child,
                 style: {
                     zIndex: s + 1
                 }
-            }, a.a.createElement(kO, {
+            }, a.a.createElement(KO, {
                 className: m.truncated
             }, "+", v)) : null)
         });
 
-    function jL() {
-        return (jL = Object.assign || function(e) {
+    function JL() {
+        return (JL = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    EL.displayName = "@mantine/core/AvatarsGroup";
-    var PL = function(e) {
+    XL.displayName = "@mantine/core/AvatarsGroup";
+    var QL = function(e) {
         var t = e.children,
             r = e.class_name;
-        return a.a.createElement(EL, jL({}, G(["setProps", "children", "class_name"], e), {
+        return a.a.createElement(XL, JL({}, G(["setProps", "children", "class_name"], e), {
             className: r
         }), a.a.Children.map(t, (function(e, t) {
             var r = e.props._dashprivate_layout.props;
-            return a.a.createElement(nL, jL({}, r, {
+            return a.a.createElement(CL, JL({}, r, {
                 key: t
             }))
         })))
     };
-    PL.displayName = "AvatarsGroup", PL.defaultProps = {}, PL.propTypes = {
+    QL.displayName = "AvatarsGroup", QL.defaultProps = {}, QL.propTypes = {
         children: i.a.node,
         class_name: i.a.string,
         id: i.a.string,
         limit: i.a.number,
         radius: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         size: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         spacing: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         style: i.a.object,
         total: i.a.number
     };
-    var zL = PL,
-        CL = Er(e => ({
+    var eA = QL,
+        tA = Er(e => ({
             root: {
                 lineHeight: e.lineHeight,
                 fontFamily: e.fontFamilyMonospace,
                 fontSize: e.fontSizes.xs,
                 fontWeight: 700,
                 backgroundColor: "dark" === e.colorScheme ? e.colors.dark[4] : e.colors.gray[0],
                 color: "dark" === e.colorScheme ? e.colors.dark[0] : e.colors.gray[7],
                 padding: `3px ${e.spacing.xs/2}px`,
                 borderRadius: e.radius.sm,
                 border: "1px solid " + ("dark" === e.colorScheme ? e.colors.dark[9] : e.colors.gray[3]),
                 borderBottom: "3px solid " + ("dark" === e.colorScheme ? e.colors.dark[9] : e.colors.gray[3])
             }
         })),
-        NL = Object.defineProperty,
-        TL = Object.getOwnPropertySymbols,
-        DL = Object.prototype.hasOwnProperty,
-        IL = Object.prototype.propertyIsEnumerable,
-        RL = (e, t, r) => t in e ? NL(e, t, {
+        rA = Object.defineProperty,
+        nA = Object.getOwnPropertySymbols,
+        aA = Object.prototype.hasOwnProperty,
+        oA = Object.prototype.propertyIsEnumerable,
+        iA = (e, t, r) => t in e ? rA(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const _L = Object(n.forwardRef)((e, t) => {
+    const lA = Object(n.forwardRef)((e, t) => {
         const r = ir("Kbd", {}, e),
             {
                 className: n,
                 children: o
             } = r,
             i = ((e, t) => {
                 var r = {};
-                for (var n in e) DL.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                if (null != e && TL)
-                    for (var n of TL(e)) t.indexOf(n) < 0 && IL.call(e, n) && (r[n] = e[n]);
+                for (var n in e) aA.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                if (null != e && nA)
+                    for (var n of nA(e)) t.indexOf(n) < 0 && oA.call(e, n) && (r[n] = e[n]);
                 return r
             })(r, ["className", "children"]),
             {
                 classes: l,
                 cx: s
-            } = CL(null, {
+            } = tA(null, {
                 name: "Kbd"
             });
         return a.a.createElement(Cn, ((e, t) => {
-            for (var r in t || (t = {})) DL.call(t, r) && RL(e, r, t[r]);
-            if (TL)
-                for (var r of TL(t)) IL.call(t, r) && RL(e, r, t[r]);
+            for (var r in t || (t = {})) aA.call(t, r) && iA(e, r, t[r]);
+            if (nA)
+                for (var r of nA(t)) oA.call(t, r) && iA(e, r, t[r]);
             return e
         })({
             component: "kbd",
             className: s(l.root, n),
             ref: t
         }, i), o)
     });
 
-    function LL() {
-        return (LL = Object.assign || function(e) {
+    function sA() {
+        return (sA = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    _L.displayName = "@mantine/core/Kbd";
-    var AL = function(e) {
+    lA.displayName = "@mantine/core/Kbd";
+    var cA = function(e) {
         var t = e.children,
             r = e.class_name;
-        return React.createElement(_L, LL({}, G(["setProps", "children", "class_name"], e), {
+        return React.createElement(lA, sA({}, G(["setProps", "children", "class_name"], e), {
             className: r
         }), t)
     };
-    AL.displayName = "Kbd", AL.defaultProps = {}, AL.propTypes = {
+    cA.displayName = "Kbd", cA.defaultProps = {}, cA.propTypes = {
         children: i.a.node,
         class_name: i.a.string,
         style: i.a.object
     };
-    var ML = AL,
-        FL = Er((e, {
+    var uA = cA,
+        dA = Er((e, {
             color: t
         }) => ({
             root: {
                 backgroundColor: e.fn.themeColor(t, "dark" === e.colorScheme ? 5 : 2),
                 color: "dark" === e.colorScheme ? e.colors.dark[9] : "inherit"
             }
         })),
-        $L = Object.defineProperty,
-        BL = Object.getOwnPropertySymbols,
-        WL = Object.prototype.hasOwnProperty,
-        HL = Object.prototype.propertyIsEnumerable,
-        VL = (e, t, r) => t in e ? $L(e, t, {
+        pA = Object.defineProperty,
+        fA = Object.getOwnPropertySymbols,
+        mA = Object.prototype.hasOwnProperty,
+        bA = Object.prototype.propertyIsEnumerable,
+        gA = (e, t, r) => t in e ? pA(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const qL = {
+    const yA = {
             color: "yellow"
         },
-        UL = Object(n.forwardRef)((e, t) => {
-            const r = ir("Mark", qL, e),
+        hA = Object(n.forwardRef)((e, t) => {
+            const r = ir("Mark", yA, e),
                 {
                     color: n,
                     className: o,
                     classNames: i,
                     styles: l
                 } = r,
                 s = ((e, t) => {
                     var r = {};
-                    for (var n in e) WL.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && BL)
-                        for (var n of BL(e)) t.indexOf(n) < 0 && HL.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) mA.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && fA)
+                        for (var n of fA(e)) t.indexOf(n) < 0 && bA.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["color", "className", "classNames", "styles"]),
                 {
                     classes: c,
                     cx: u
-                } = FL({
+                } = dA({
                     color: n
                 }, {
                     classNames: i,
                     styles: l,
                     name: "Mark"
                 });
             return a.a.createElement(Cn, ((e, t) => {
-                for (var r in t || (t = {})) WL.call(t, r) && VL(e, r, t[r]);
-                if (BL)
-                    for (var r of BL(t)) HL.call(t, r) && VL(e, r, t[r]);
+                for (var r in t || (t = {})) mA.call(t, r) && gA(e, r, t[r]);
+                if (fA)
+                    for (var r of fA(t)) bA.call(t, r) && gA(e, r, t[r]);
                 return e
             })({
                 component: "mark",
                 ref: t,
                 className: u(c.root, o)
             }, s))
         });
 
-    function GL(e) {
+    function vA(e) {
         return e.replace(/[-[\]{}()*+?.,\\^$|#]/g, "\\$&")
     }
-    UL.displayName = "@mantine/core/Mark";
-    var YL = Object.defineProperty,
-        ZL = Object.getOwnPropertySymbols,
-        KL = Object.prototype.hasOwnProperty,
-        XL = Object.prototype.propertyIsEnumerable,
-        JL = (e, t, r) => t in e ? YL(e, t, {
+    hA.displayName = "@mantine/core/Mark";
+    var OA = Object.defineProperty,
+        wA = Object.getOwnPropertySymbols,
+        xA = Object.prototype.hasOwnProperty,
+        SA = Object.prototype.propertyIsEnumerable,
+        kA = (e, t, r) => t in e ? OA(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const QL = {
+    const EA = {
             highlightColor: "yellow"
         },
-        eA = Object(n.forwardRef)((e, t) => {
-            const r = ir("Highlight", QL, e),
+        jA = Object(n.forwardRef)((e, t) => {
+            const r = ir("Highlight", EA, e),
                 {
                     children: n,
                     highlight: o,
                     highlightColor: i,
                     component: l,
                     highlightStyles: s
                 } = r,
                 c = ((e, t) => {
                     var r = {};
-                    for (var n in e) KL.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && ZL)
-                        for (var n of ZL(e)) t.indexOf(n) < 0 && XL.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) xA.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && wA)
+                        for (var n of wA(e)) t.indexOf(n) < 0 && SA.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["children", "highlight", "highlightColor", "component", "highlightStyles"]),
                 u = function(e, t) {
                     if (null == t) return [{
                         chunk: e,
                         highlighted: !1
                     }];
-                    const r = Array.isArray(t) ? t.map(GL) : GL(t);
+                    const r = Array.isArray(t) ? t.map(vA) : vA(t);
                     if (!(Array.isArray(r) ? r.filter(e => e.trim().length > 0).length > 0 : "" !== r.trim())) return [{
                         chunk: e,
                         highlighted: !1
                     }];
                     const n = "string" == typeof r ? r.trim() : r.filter(e => 0 !== e.trim().length).map(e => e.trim()).join("|"),
                         a = new RegExp(`(${n})`, "gi");
                     return e.split(a).map(e => ({
                         chunk: e,
                         highlighted: a.test(e)
                     })).filter(({
                         chunk: e
                     }) => e)
                 }(n, o);
             return a.a.createElement(jo, ((e, t) => {
-                for (var r in t || (t = {})) KL.call(t, r) && JL(e, r, t[r]);
-                if (ZL)
-                    for (var r of ZL(t)) XL.call(t, r) && JL(e, r, t[r]);
+                for (var r in t || (t = {})) xA.call(t, r) && kA(e, r, t[r]);
+                if (wA)
+                    for (var r of wA(t)) SA.call(t, r) && kA(e, r, t[r]);
                 return e
             })({
                 component: l,
                 ref: t
             }, c), u.map(({
                 chunk: e,
                 highlighted: t
-            }, r) => t ? a.a.createElement(UL, {
+            }, r) => t ? a.a.createElement(hA, {
                 key: r,
                 color: i,
                 sx: s
             }, e) : a.a.createElement("span", {
                 key: r
             }, e)))
         });
 
-    function tA() {
-        return (tA = Object.assign || function(e) {
+    function PA() {
+        return (PA = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    eA.displayName = "@mantine/core/Highlight";
-    var rA = function(e) {
+    jA.displayName = "@mantine/core/Highlight";
+    var zA = function(e) {
         var t = e.children,
             r = e.class_name;
-        return a.a.createElement(eA, tA({
+        return a.a.createElement(jA, PA({
             className: r
         }, G(["children", "class_name", "setProps"], e)), t)
     };
-    rA.displayName = "Highlight", rA.defaultProps = {
+    zA.displayName = "Highlight", zA.defaultProps = {
         highlightColor: "yellow"
-    }, rA.propTypes = {
+    }, zA.propTypes = {
         align: i.a.oneOf(["left", "right", "center", "justify"]),
         children: i.a.string,
         class_name: i.a.string,
         color: i.a.oneOf(["dark", "gray", "red", "pink", "grape", "violet", "indigo", "blue", "cyan", "teal", "green", "lime", "yellow", "orange"]),
         gradient: i.a.exact({
             from: i.a.string.isRequired,
             to: i.a.string.isRequired,
@@ -28225,16 +28552,16 @@
         size: i.a.oneOf(["xs", "sm", "md", "lg", "xl"]),
         style: i.a.object,
         transform: i.a.oneOf(["none", "capitalize", "lowercase", "uppercase"]),
         underline: i.a.bool,
         variant: i.a.oneOf(["link", "text", "gradient"]),
         weight: i.a.oneOfType([i.a.oneOf(["normal", "bold", "bolder", "lighter", "initial", "inherit"]), i.a.number])
     };
-    var nA = rA,
-        aA = Er((e, {
+    var CA = zA,
+        NA = Er((e, {
             bulletSize: t,
             color: r,
             radius: n,
             align: a,
             lineVariant: o,
             lineWidth: i
         }, l) => ({
@@ -28309,26 +28636,26 @@
             itemTitle: {
                 fontWeight: 500,
                 lineHeight: 1,
                 marginBottom: e.spacing.xs / 2,
                 textAlign: a
             }
         })),
-        oA = Object.defineProperty,
-        iA = Object.getOwnPropertySymbols,
-        lA = Object.prototype.hasOwnProperty,
-        sA = Object.prototype.propertyIsEnumerable,
-        cA = (e, t, r) => t in e ? oA(e, t, {
+        TA = Object.defineProperty,
+        DA = Object.getOwnPropertySymbols,
+        IA = Object.prototype.hasOwnProperty,
+        RA = Object.prototype.propertyIsEnumerable,
+        _A = (e, t, r) => t in e ? TA(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
 
-    function uA(e) {
+    function LA(e) {
         var t = e,
             {
                 className: r,
                 bullet: n,
                 title: o,
                 bulletSize: i = 20,
                 radius: l = "xl",
@@ -28340,38 +28667,38 @@
                 children: f,
                 color: m,
                 align: b,
                 lineVariant: g = "solid"
             } = t,
             y = ((e, t) => {
                 var r = {};
-                for (var n in e) lA.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                if (null != e && iA)
-                    for (var n of iA(e)) t.indexOf(n) < 0 && sA.call(e, n) && (r[n] = e[n]);
+                for (var n in e) IA.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                if (null != e && DA)
+                    for (var n of DA(e)) t.indexOf(n) < 0 && RA.call(e, n) && (r[n] = e[n]);
                 return r
             })(t, ["className", "bullet", "title", "bulletSize", "radius", "lineWidth", "active", "lineActive", "classNames", "styles", "children", "color", "align", "lineVariant"]);
         const {
             classes: h,
             cx: v
-        } = aA({
+        } = NA({
             bulletSize: i,
             color: m,
             radius: l,
             align: b,
             lineVariant: g,
             lineWidth: s
         }, {
             classNames: d,
             styles: p,
             name: "Timeline"
         });
         return a.a.createElement(Cn, ((e, t) => {
-            for (var r in t || (t = {})) lA.call(t, r) && cA(e, r, t[r]);
-            if (iA)
-                for (var r of iA(t)) sA.call(t, r) && cA(e, r, t[r]);
+            for (var r in t || (t = {})) IA.call(t, r) && _A(e, r, t[r]);
+            if (DA)
+                for (var r of DA(t)) RA.call(t, r) && _A(e, r, t[r]);
             return e
         })({
             className: v(h.item, {
                 [h.itemLineActive]: u,
                 [h.itemActive]: c
             }, r)
         }, y), a.a.createElement("div", {
@@ -28382,35 +28709,35 @@
             className: h.itemBody
         }, o && a.a.createElement(jo, {
             className: h.itemTitle
         }, o), a.a.createElement("div", {
             className: h.itemContent
         }, f)))
     }
-    uA.displayName = "@mantine/core/TimelineItem";
-    var dA = Object.defineProperty,
-        pA = Object.getOwnPropertySymbols,
-        fA = Object.prototype.hasOwnProperty,
-        mA = Object.prototype.propertyIsEnumerable,
-        bA = (e, t, r) => t in e ? dA(e, t, {
+    LA.displayName = "@mantine/core/TimelineItem";
+    var AA = Object.defineProperty,
+        MA = Object.getOwnPropertySymbols,
+        FA = Object.prototype.hasOwnProperty,
+        $A = Object.prototype.propertyIsEnumerable,
+        BA = (e, t, r) => t in e ? AA(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const gA = {
+    const WA = {
             active: -1,
             radius: "xl",
             bulletSize: 20,
             align: "left",
             lineWidth: 4,
             reverseActive: !1
         },
-        yA = Object(n.forwardRef)((e, t) => {
-            const r = ir("Timeline", gA, e),
+        HA = Object(n.forwardRef)((e, t) => {
+            const r = ir("Timeline", WA, e),
                 {
                     children: n,
                     active: o,
                     color: i,
                     radius: l,
                     bulletSize: s,
                     align: c,
@@ -28418,20 +28745,20 @@
                     classNames: d,
                     styles: p,
                     sx: f,
                     reverseActive: m
                 } = r,
                 b = ((e, t) => {
                     var r = {};
-                    for (var n in e) fA.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && pA)
-                        for (var n of pA(e)) t.indexOf(n) < 0 && mA.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) FA.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && MA)
+                        for (var n of MA(e)) t.indexOf(n) < 0 && $A.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["children", "active", "color", "radius", "bulletSize", "align", "lineWidth", "classNames", "styles", "sx", "reverseActive"]),
-                g = si(n, uA),
+                g = si(n, LA),
                 y = g.map((e, t) => a.a.cloneElement(e, {
                     classNames: d,
                     styles: p,
                     align: c,
                     lineWidth: u,
                     radius: e.props.radius || l,
                     color: e.props.color || i,
@@ -28441,100 +28768,100 @@
                 })),
                 h = "left" === c ? {
                     paddingLeft: s / 2 + u / 2
                 } : {
                     paddingRight: s / 2 + u / 2
                 };
             return a.a.createElement(Cn, ((e, t) => {
-                for (var r in t || (t = {})) fA.call(t, r) && bA(e, r, t[r]);
-                if (pA)
-                    for (var r of pA(t)) mA.call(t, r) && bA(e, r, t[r]);
+                for (var r in t || (t = {})) FA.call(t, r) && BA(e, r, t[r]);
+                if (MA)
+                    for (var r of MA(t)) $A.call(t, r) && BA(e, r, t[r]);
                 return e
             })({
                 ref: t,
                 sx: [h, ...Array.isArray(f) ? f : [f]]
             }, b), y)
         });
 
-    function hA() {
-        return (hA = Object.assign || function(e) {
+    function VA() {
+        return (VA = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    yA.Item = uA, yA.displayName = "@mantine/core/Timeline";
-    var vA = function(e) {
+    HA.Item = LA, HA.displayName = "@mantine/core/Timeline";
+    var qA = function(e) {
         var t = e.children,
             r = e.class_name;
-        return a.a.createElement(yA, hA({}, G(["children", "setProps"], e), {
+        return a.a.createElement(HA, VA({}, G(["children", "setProps"], e), {
             className: r
         }), a.a.Children.map(t, (function(e, t) {
             var r = e.props._dashprivate_layout.props,
                 n = ta(G(["children"], r), ["title", "bullet"]);
-            return a.a.createElement(yA.Item, hA({}, n, {
+            return a.a.createElement(HA.Item, VA({}, n, {
                 key: t
             }), e)
         })))
     };
-    vA.displayName = "Timeline", vA.defaultProps = {}, vA.propTypes = {
+    qA.displayName = "Timeline", qA.defaultProps = {}, qA.propTypes = {
         active: i.a.number,
         align: i.a.oneOf(["left", "right"]),
         bulletSize: i.a.number,
         children: i.a.node,
         class_name: i.a.string,
         color: i.a.oneOf(["dark", "gray", "red", "pink", "grape", "violet", "indigo", "blue", "cyan", "teal", "green", "lime", "yellow", "orange"]),
         lineWidth: i.a.number,
         radius: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         reverseActive: i.a.bool
     };
-    var OA = vA,
-        wA = function(e) {
+    var UA = qA,
+        GA = function(e) {
             return a.a.createElement("div", null, e.children)
         };
-    wA.displayName = "TimelineItem", wA.defaultProps = {}, wA.propTypes = {
+    GA.displayName = "TimelineItem", GA.defaultProps = {}, GA.propTypes = {
         align: i.a.oneOf(["left", "right"]),
         bullet: i.a.any,
         bulletSize: i.a.number,
         children: i.a.node,
         color: i.a.oneOf(["dark", "gray", "red", "pink", "grape", "violet", "indigo", "blue", "cyan", "teal", "green", "lime", "yellow", "orange"]),
         lineVariant: i.a.oneOf(["dashed", "dotted", "solid"]),
         lineWidth: i.a.number,
         radius: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         title: i.a.any
     };
-    var xA = wA;
+    var YA = GA;
 
-    function SA() {
-        return (SA = Object.assign || function(e) {
+    function ZA() {
+        return (ZA = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    var kA = function(e) {
+    var KA = function(e) {
         var t = e.children,
             r = e.class_name;
-        return a.a.createElement(UL, SA({}, G(["children", "class_name", "setProps"], e), {
+        return a.a.createElement(hA, ZA({}, G(["children", "class_name", "setProps"], e), {
             className: r
         }), t)
     };
-    kA.displayName = "Mark", kA.defaultProps = {}, kA.propTypes = {
+    KA.displayName = "Mark", KA.defaultProps = {}, KA.propTypes = {
         children: i.a.string,
         class_name: i.a.string,
         color: i.a.oneOf(["dark", "gray", "red", "pink", "grape", "violet", "indigo", "blue", "cyan", "teal", "green", "lime", "yellow", "orange"]),
         id: i.a.string,
         style: i.a.object
     };
-    var EA = kA,
-        jA = Er((e, {
+    var XA = KA,
+        JA = Er((e, {
             smallerThan: t,
             largerThan: r,
             query: n,
             styles: a
         }) => {
             const o = {},
                 i = e.fn.size({
@@ -28546,121 +28873,121 @@
                     sizes: e.breakpoints
                 });
             return void 0 !== r && void 0 !== t ? o[`@media (min-width: ${i}px) and (max-width: ${l}px)`] = a : (void 0 !== r && (o[`@media (min-width: ${e.fn.size({size:r,sizes:e.breakpoints})+1}px)`] = a), void 0 !== t && (o[`@media (max-width: ${e.fn.size({size:t,sizes:e.breakpoints})}px)`] = a)), n && (o["@media " + n] = a), {
                 media: o
             }
         });
 
-    function PA(e) {
+    function QA(e) {
         var t;
         const {
             children: r,
             smallerThan: o,
             largerThan: i,
             query: l,
             styles: s,
             className: c
         } = ir("MediaQuery", {}, e), {
             classes: u,
             cx: d
-        } = jA({
+        } = JA({
             smallerThan: o,
             largerThan: i,
             query: l,
             styles: s
         }, {
             name: "MediaQuery"
         }), p = n.Children.only(r);
         return "object" == typeof p && null !== p && "props" in p ? a.a.cloneElement(p, {
             className: d(u.media, null == (t = p.props) ? void 0 : t.className, c)
         }) : p
     }
 
-    function zA() {
-        return (zA = Object.assign || function(e) {
+    function eM() {
+        return (eM = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    PA.displayName = "@mantine/core/MediaQuery";
-    var CA = function(e) {
+    QA.displayName = "@mantine/core/MediaQuery";
+    var tM = function(e) {
         var t = e.children,
             r = e.class_name;
-        return a.a.createElement(PA, zA({}, G(["children", "class_name", "setProps"], e), {
+        return a.a.createElement(QA, eM({}, G(["children", "class_name", "setProps"], e), {
             className: r
         }), a.a.createElement(Cn, null, t))
     };
-    CA.displayName = "MediaQuery", CA.defaultProps = {}, CA.propTypes = {
+    tM.displayName = "MediaQuery", tM.defaultProps = {}, tM.propTypes = {
         children: i.a.node,
         class_name: i.a.string,
         id: i.a.string,
         largerThan: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         query: i.a.string,
         smallerThan: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         styles: i.a.object
     };
-    var NA = CA,
-        TA = Object.defineProperty,
-        DA = Object.getOwnPropertySymbols,
-        IA = Object.prototype.hasOwnProperty,
-        RA = Object.prototype.propertyIsEnumerable,
-        _A = (e, t, r) => t in e ? TA(e, t, {
+    var rM = tM,
+        nM = Object.defineProperty,
+        aM = Object.getOwnPropertySymbols,
+        oM = Object.prototype.hasOwnProperty,
+        iM = Object.prototype.propertyIsEnumerable,
+        lM = (e, t, r) => t in e ? nM(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
 
-    function LA(e) {
+    function sM(e) {
         return a.a.createElement("svg", ((e, t) => {
-            for (var r in t || (t = {})) IA.call(t, r) && _A(e, r, t[r]);
-            if (DA)
-                for (var r of DA(t)) RA.call(t, r) && _A(e, r, t[r]);
+            for (var r in t || (t = {})) oM.call(t, r) && lM(e, r, t[r]);
+            if (aM)
+                for (var r of aM(t)) iM.call(t, r) && lM(e, r, t[r]);
             return e
         })({
             width: "15",
             height: "15",
             viewBox: "0 0 15 15",
             fill: "none",
             xmlns: "http://www.w3.org/2000/svg"
         }, e), a.a.createElement("path", {
             d: "M3.625 7.5C3.625 8.12132 3.12132 8.625 2.5 8.625C1.87868 8.625 1.375 8.12132 1.375 7.5C1.375 6.87868 1.87868 6.375 2.5 6.375C3.12132 6.375 3.625 6.87868 3.625 7.5ZM8.625 7.5C8.625 8.12132 8.12132 8.625 7.5 8.625C6.87868 8.625 6.375 8.12132 6.375 7.5C6.375 6.87868 6.87868 6.375 7.5 6.375C8.12132 6.375 8.625 6.87868 8.625 7.5ZM12.5 8.625C13.1213 8.625 13.625 8.12132 13.625 7.5C13.625 6.87868 13.1213 6.375 12.5 6.375C11.8787 6.375 11.375 6.87868 11.375 7.5C11.375 8.12132 11.8787 8.625 12.5 8.625Z",
             fill: "currentColor",
             fillRule: "evenodd",
             clipRule: "evenodd"
         }))
     }
-    const [AA, MA] = Bx(null);
-    var FA = Object.defineProperty,
-        $A = Object.defineProperties,
-        BA = Object.getOwnPropertyDescriptors,
-        WA = Object.getOwnPropertySymbols,
-        HA = Object.prototype.hasOwnProperty,
-        VA = Object.prototype.propertyIsEnumerable,
-        qA = (e, t, r) => t in e ? FA(e, t, {
+    const [cM, uM] = fS(null);
+    var dM = Object.defineProperty,
+        pM = Object.defineProperties,
+        fM = Object.getOwnPropertyDescriptors,
+        mM = Object.getOwnPropertySymbols,
+        bM = Object.prototype.hasOwnProperty,
+        gM = Object.prototype.propertyIsEnumerable,
+        yM = (e, t, r) => t in e ? dM(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        UA = (e, t) => {
-            for (var r in t || (t = {})) HA.call(t, r) && qA(e, r, t[r]);
-            if (WA)
-                for (var r of WA(t)) VA.call(t, r) && qA(e, r, t[r]);
+        hM = (e, t) => {
+            for (var r in t || (t = {})) bM.call(t, r) && yM(e, r, t[r]);
+            if (mM)
+                for (var r of mM(t)) gM.call(t, r) && yM(e, r, t[r]);
             return e
         },
-        GA = Er((e, {
+        vM = Er((e, {
             radius: t,
             color: r
         }) => {
             return {
-                item: (n = UA({}, e.fn.fontStyles()), a = {
+                item: (n = hM({}, e.fn.fontStyles()), a = {
                     WebkitTapHighlightColor: "transparent",
                     fontSize: e.fontSizes.sm,
                     border: 0,
                     backgroundColor: "transparent",
                     outline: 0,
                     width: "100%",
                     textAlign: "left",
@@ -28674,15 +29001,15 @@
                         sizes: e.radius
                     }),
                     color: r ? e.fn.themeColor(r, "dark" === e.colorScheme ? 5 : 7) : "dark" === e.colorScheme ? e.colors.dark[0] : e.black,
                     "&:disabled": {
                         color: "dark" === e.colorScheme ? e.colors.dark[3] : e.colors.gray[5],
                         pointerEvents: "none"
                     }
-                }, $A(n, BA(a))),
+                }, pM(n, fM(a))),
                 itemHovered: {
                     backgroundColor: r ? e.fn.rgba(e.fn.themeColor(r, "dark" === e.colorScheme ? 9 : 0), "dark" === e.colorScheme ? .2 : 1) : "dark" === e.colorScheme ? e.fn.rgba(e.colors.dark[3], .35) : e.colors.gray[0]
                 },
                 itemInner: {
                     display: "flex",
                     alignItems: "center",
                     height: "100%"
@@ -28701,57 +29028,57 @@
                 },
                 itemLabel: {
                     lineHeight: 1
                 }
             };
             var n, a
         });
-    var YA = Object.defineProperty,
-        ZA = Object.getOwnPropertySymbols,
-        KA = Object.prototype.hasOwnProperty,
-        XA = Object.prototype.propertyIsEnumerable,
-        JA = (e, t, r) => t in e ? YA(e, t, {
+    var OM = Object.defineProperty,
+        wM = Object.getOwnPropertySymbols,
+        xM = Object.prototype.hasOwnProperty,
+        SM = Object.prototype.propertyIsEnumerable,
+        kM = (e, t, r) => t in e ? OM(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const QA = Object(n.forwardRef)((e, t) => {
+    const EM = Object(n.forwardRef)((e, t) => {
         var r = e,
             {
                 className: o,
                 children: i,
                 icon: l,
                 color: s,
                 disabled: c,
                 rightSection: u,
                 component: d,
                 onClick: p
             } = r,
             f = ((e, t) => {
                 var r = {};
-                for (var n in e) KA.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                if (null != e && ZA)
-                    for (var n of ZA(e)) t.indexOf(n) < 0 && XA.call(e, n) && (r[n] = e[n]);
+                for (var n in e) xM.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                if (null != e && wM)
+                    for (var n of wM(e)) t.indexOf(n) < 0 && SM.call(e, n) && (r[n] = e[n]);
                 return r
             })(r, ["className", "children", "icon", "color", "disabled", "rightSection", "component", "onClick"]);
         const m = Object(n.useRef)(),
             {
                 hovered: b,
                 onItemHover: g,
                 radius: y,
                 onItemKeyDown: h,
                 classNames: v,
                 styles: O,
                 onItemClick: w
-            } = MA("Menu.Item"),
+            } = uM("Menu.Item"),
             {
                 classes: x,
                 cx: S
-            } = GA({
+            } = vM({
                 color: s,
                 radius: y
             }, {
                 classNames: v,
                 styles: O,
                 name: "Menu"
             }),
@@ -28762,17 +29089,17 @@
                 let r = e;
                 for (;
                     (r = r.parentElement) && !r.classList.contains(t););
                 return r
             }(j, E.parentClassName).querySelectorAll(E.elementSelector)).findIndex(e => e === j) : -1);
         var E, j;
         return a.a.createElement(Cn, ((e, t) => {
-            for (var r in t || (t = {})) KA.call(t, r) && JA(e, r, t[r]);
-            if (ZA)
-                for (var r of ZA(t)) XA.call(t, r) && JA(e, r, t[r]);
+            for (var r in t || (t = {})) xM.call(t, r) && kM(e, r, t[r]);
+            if (wM)
+                for (var r of wM(t)) SM.call(t, r) && kM(e, r, t[r]);
             return e
         })({
             component: d || "button",
             type: "button",
             role: "menuitem",
             className: S(x.item, {
                 [x.itemHovered]: b === k
@@ -28791,78 +29118,78 @@
             className: x.itemIcon
         }, l), a.a.createElement("div", {
             className: x.itemBody
         }, a.a.createElement("div", {
             className: x.itemLabel
         }, i), u)))
     });
-    QA.displayName = "@mantine/core/MenuItem";
-    var eM = Er(e => ({
+    EM.displayName = "@mantine/core/MenuItem";
+    var jM = Er(e => ({
             label: {
                 color: "dark" === e.colorScheme ? e.colors.dark[2] : e.colors.gray[6],
                 fontWeight: 500,
                 fontSize: e.fontSizes.xs,
                 padding: `${e.spacing.xs/2}px ${e.spacing.sm}px`,
                 cursor: "default"
             }
         })),
-        tM = Object.defineProperty,
-        rM = Object.getOwnPropertySymbols,
-        nM = Object.prototype.hasOwnProperty,
-        aM = Object.prototype.propertyIsEnumerable,
-        oM = (e, t, r) => t in e ? tM(e, t, {
+        PM = Object.defineProperty,
+        zM = Object.getOwnPropertySymbols,
+        CM = Object.prototype.hasOwnProperty,
+        NM = Object.prototype.propertyIsEnumerable,
+        TM = (e, t, r) => t in e ? PM(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
 
-    function iM(e) {
+    function DM(e) {
         const {
             classNames: t,
             styles: r
-        } = MA("Menu.Label"), {
+        } = uM("Menu.Label"), {
             classes: n
-        } = eM(null, {
+        } = jM(null, {
             name: "Menu",
             classNames: t,
             styles: r
         });
         return a.a.createElement(jo, ((e, t) => {
-            for (var r in t || (t = {})) nM.call(t, r) && oM(e, r, t[r]);
-            if (rM)
-                for (var r of rM(t)) aM.call(t, r) && oM(e, r, t[r]);
+            for (var r in t || (t = {})) CM.call(t, r) && TM(e, r, t[r]);
+            if (zM)
+                for (var r of zM(t)) NM.call(t, r) && TM(e, r, t[r]);
             return e
         })({
             className: n.label
         }, e))
     }
-    iM.displayName = "@mantine/core/MenuLabel";
-    const lM = {
+    DM.displayName = "@mantine/core/MenuLabel";
+    const IM = {
         xs: 120,
         sm: 160,
         md: 200,
         lg: 240,
         xl: 300
     };
-    var sM = Er((e, {
+    var RM = Er((e, {
             size: t
         }) => ({
             root: {
                 display: "inline-block",
                 position: "relative"
             },
             arrow: {
                 borderColor: "dark" === e.colorScheme ? e.colors.dark[6] : e.colors.gray[2],
                 background: "dark" === e.colorScheme ? e.colors.dark[6] : e.white
             },
             body: {
                 width: e.fn.size({
                     size: t,
-                    sizes: lM
+                    sizes: IM
                 }),
                 overflow: "hidden",
                 pointerEvents: "all",
                 border: "1px solid " + ("dark" === e.colorScheme ? e.colors.dark[6] : e.colors.gray[2]),
                 backgroundColor: "dark" === e.colorScheme ? e.colors.dark[6] : e.white,
                 padding: 4,
                 "& .mantine-Divider-horizontal": {
@@ -28874,34 +29201,34 @@
                 color: "dark" === e.colorScheme ? e.colors.dark[2] : e.colors.gray[6],
                 fontWeight: 500,
                 fontSize: e.fontSizes.xs,
                 padding: `${e.spacing.xs/2}px ${e.spacing.sm}px`,
                 cursor: "default"
             }
         })),
-        cM = Object.defineProperty,
-        uM = Object.defineProperties,
-        dM = Object.getOwnPropertyDescriptors,
-        pM = Object.getOwnPropertySymbols,
-        fM = Object.prototype.hasOwnProperty,
-        mM = Object.prototype.propertyIsEnumerable,
-        bM = (e, t, r) => t in e ? cM(e, t, {
+        _M = Object.defineProperty,
+        LM = Object.defineProperties,
+        AM = Object.getOwnPropertyDescriptors,
+        MM = Object.getOwnPropertySymbols,
+        FM = Object.prototype.hasOwnProperty,
+        $M = Object.prototype.propertyIsEnumerable,
+        BM = (e, t, r) => t in e ? _M(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        gM = (e, t) => {
-            for (var r in t || (t = {})) fM.call(t, r) && bM(e, r, t[r]);
-            if (pM)
-                for (var r of pM(t)) mM.call(t, r) && bM(e, r, t[r]);
+        WM = (e, t) => {
+            for (var r in t || (t = {})) FM.call(t, r) && BM(e, r, t[r]);
+            if (MM)
+                for (var r of MM(t)) $M.call(t, r) && BM(e, r, t[r]);
             return e
         };
-    const yM = {
-            control: a.a.createElement(ol, null, a.a.createElement(LA, null)),
+    const HM = {
+            control: a.a.createElement(ol, null, a.a.createElement(sM, null)),
             closeOnItemClick: !0,
             transitionDuration: 150,
             size: "md",
             shadow: "md",
             position: "bottom",
             placement: "start",
             gutter: 5,
@@ -28913,16 +29240,16 @@
             delay: 100,
             zIndex: ac("popover"),
             withinPortal: !0,
             trapFocus: !0,
             closeOnScroll: !1,
             clickOutsideEvents: ["mousedown", "touchstart"]
         },
-        hM = Object(n.forwardRef)((e, t) => {
-            const r = ir("Menu", yM, e),
+        VM = Object(n.forwardRef)((e, t) => {
+            const r = ir("Menu", HM, e),
                 {
                     control: o,
                     children: i,
                     onClose: l,
                     onOpen: s,
                     opened: c,
                     menuId: u,
@@ -28952,24 +29279,24 @@
                     onChange: R,
                     className: _,
                     sx: L,
                     clickOutsideEvents: A
                 } = r,
                 M = ((e, t) => {
                     var r = {};
-                    for (var n in e) fM.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && pM)
-                        for (var n of pM(e)) t.indexOf(n) < 0 && mM.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) FM.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && MM)
+                        for (var n of MM(e)) t.indexOf(n) < 0 && $M.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["control", "children", "onClose", "onOpen", "opened", "menuId", "closeOnItemClick", "transitionDuration", "size", "shadow", "position", "placement", "gutter", "withArrow", "transition", "transitionTimingFunction", "menuButtonLabel", "controlRefProp", "trigger", "radius", "delay", "zIndex", "withinPortal", "trapFocus", "classNames", "styles", "closeOnScroll", "onMouseLeave", "onMouseEnter", "onChange", "className", "sx", "clickOutsideEvents"]),
                 [F, $] = Object(n.useState)(-1),
                 {
                     classes: B,
                     cx: W
-                } = sM({
+                } = RM({
                     size: f
                 }, {
                     classNames: C,
                     styles: N,
                     name: "Menu"
                 }),
                 H = Object(n.useRef)(),
@@ -29026,41 +29353,41 @@
                                 }(t)
                             }(F, t);
                             $(r), t[r].focus()
                         }
                         "Escape" === e.nativeEvent.code && (te(), X())
                     }
                 },
-                ie = Object(n.cloneElement)(o, (le = gM({}, ae), se = {
+                ie = Object(n.cloneElement)(o, (le = WM({}, ae), se = {
                     onClick: e => {
                         ae.onClick(), "function" == typeof o.props.onClick && o.props.onClick(e)
                     },
                     role: "button",
                     "aria-haspopup": "menu",
                     "aria-expanded": J,
                     "aria-controls": K,
                     "aria-label": w,
                     title: w,
                     [x]: ua(q, t),
                     onKeyDown: oe
-                }, uM(le, dM(se))));
+                }, LM(le, AM(se))));
             var le, se;
-            return a.a.createElement(AA, {
+            return a.a.createElement(cM, {
                 value: {
                     hovered: F,
                     radius: k,
                     styles: N,
                     classNames: C,
                     onItemHover: $,
                     onItemKeyDown: oe,
                     onItemClick: () => {
                         d && (te(), "click" === S && X())
                     }
                 }
-            }, a.a.createElement(Cn, gM({
+            }, a.a.createElement(Cn, WM({
                 ref: G,
                 onMouseLeave: e => {
                     "function" == typeof D && D(e), "hover" === S && (E > 0 ? H.current = window.setTimeout(() => te(), E) : te())
                 },
                 onMouseEnter: e => {
                     "function" == typeof I && I(e), window.clearTimeout(H.current)
                 },
@@ -29076,44 +29403,44 @@
                 placement: g,
                 gutter: y,
                 withArrow: h,
                 arrowSize: 3,
                 zIndex: j,
                 arrowClassName: B.arrow,
                 withinPortal: P
-            }, a.a.createElement(Md, gM({
+            }, a.a.createElement(Md, WM({
                 shadow: m,
                 className: B.body,
                 role: "menu",
                 "aria-orientation": "vertical",
                 radius: k,
                 onMouseLeave: () => $(-1),
                 ref: Z,
                 id: K
             }, M), i))))
         });
 
-    function vM() {
-        return (vM = Object.assign || function(e) {
+    function qM() {
+        return (qM = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    hM.Item = QA, hM.Label = iM, hM.displayName = "@mantine/core/Menu";
-    var OM = function(e) {
+    VM.Item = EM, VM.Label = DM, VM.displayName = "@mantine/core/Menu";
+    var UM = function(e) {
         var t = e.children,
             r = e.class_name;
-        return a.a.createElement(hM, vM({}, G(["children", "setProps", "class_name"], e), {
+        return a.a.createElement(VM, qM({}, G(["children", "setProps", "class_name"], e), {
             className: r
         }), t)
     };
-    OM.displayName = "Menu", OM.defaultProps = {}, OM.propTypes = {
+    UM.displayName = "Menu", UM.defaultProps = {}, UM.propTypes = {
         arrowDistance: i.a.number,
         arrowSize: i.a.number,
         children: i.a.node,
         class_name: i.a.string,
         closeOnItemClick: i.a.bool,
         closeOnScroll: i.a.bool,
         delay: i.a.number,
@@ -29131,196 +29458,196 @@
         transitionDuration: i.a.number,
         transitionTimingFunction: i.a.string,
         trapFocus: i.a.bool,
         trigger: i.a.oneOf(["hover", "click"]),
         withArrow: i.a.bool,
         zIndex: i.a.number
     };
-    var wM = OM;
+    var GM = UM;
 
-    function xM() {
-        return (xM = Object.assign || function(e) {
+    function YM() {
+        return (YM = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    var SM = function(e) {
+    var ZM = function(e) {
         var t = e.children,
             r = e.class_name,
             n = e.n_clicks,
             o = e.setProps,
             i = e.disabled,
             l = e.href,
             s = ta(G(["children", "class_name", "setProps"], e), ["icon", "rightSection"]);
-        return a.a.createElement(hM.Item, xM({}, s, {
+        return a.a.createElement(VM.Item, YM({}, s, {
             onClick: function() {
                 i || o({
                     n_clicks: n + 1
                 })
             },
             className: r,
             component: l && "a"
         }), t)
     };
-    SM.displayName = "MenuItem", SM.defaultProps = {
+    ZM.displayName = "MenuItem", ZM.defaultProps = {
         n_clicks: 0
-    }, SM.propTypes = {
+    }, ZM.propTypes = {
         children: i.a.string,
         class_name: i.a.string,
         color: i.a.oneOf(["dark", "gray", "red", "pink", "grape", "violet", "indigo", "blue", "cyan", "teal", "green", "lime", "yellow", "orange"]),
         disabled: i.a.bool,
         href: i.a.string,
         icon: i.a.any,
         id: i.a.string,
         n_clicks: i.a.number,
         rightSection: i.a.any,
         setProps: i.a.func,
         style: i.a.object,
         target: i.a.oneOf(["_blank", "_self"])
     };
-    var kM = SM,
-        EM = function(e) {
-            return a.a.createElement(hM.Label, null, e.children)
+    var KM = ZM,
+        XM = function(e) {
+            return a.a.createElement(VM.Label, null, e.children)
         };
-    EM.displayName = "MenuLabel", EM.defaultProps = {}, EM.propTypes = {
+    XM.displayName = "MenuLabel", XM.defaultProps = {}, XM.propTypes = {
         children: i.a.string
     };
-    var jM = EM,
-        PM = Object.defineProperty,
-        zM = Object.defineProperties,
-        CM = Object.getOwnPropertyDescriptors,
-        NM = Object.getOwnPropertySymbols,
-        TM = Object.prototype.hasOwnProperty,
-        DM = Object.prototype.propertyIsEnumerable,
-        IM = (e, t, r) => t in e ? PM(e, t, {
+    var JM = XM,
+        QM = Object.defineProperty,
+        eF = Object.defineProperties,
+        tF = Object.getOwnPropertyDescriptors,
+        rF = Object.getOwnPropertySymbols,
+        nF = Object.prototype.hasOwnProperty,
+        aF = Object.prototype.propertyIsEnumerable,
+        oF = (e, t, r) => t in e ? QM(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        RM = (e, t) => {
-            for (var r in t || (t = {})) TM.call(t, r) && IM(e, r, t[r]);
-            if (NM)
-                for (var r of NM(t)) DM.call(t, r) && IM(e, r, t[r]);
+        iF = (e, t) => {
+            for (var r in t || (t = {})) nF.call(t, r) && oF(e, r, t[r]);
+            if (rF)
+                for (var r of rF(t)) aF.call(t, r) && oF(e, r, t[r]);
             return e
         },
-        _M = Er((e, {
+        lF = Er((e, {
             color: t
         }) => {
             const r = dr({
                 theme: e,
                 color: t,
                 variant: "light"
             });
             return {
-                root: (n = RM({}, e.fn.fontStyles()), a = {
+                root: (n = iF({}, e.fn.fontStyles()), a = {
                     lineHeight: e.lineHeight,
                     padding: `2px ${e.spacing.xs/2}px`,
                     borderRadius: e.radius.sm,
                     color: "dark" === e.colorScheme ? "dark" === t ? e.colors.dark[0] : e.white : e.colors.dark[7],
                     backgroundColor: "dark" === e.colorScheme && "dark" === t ? e.colors.dark[4] : r.background,
                     fontFamily: e.fontFamilyMonospace,
                     fontSize: e.fontSizes.xs
-                }, zM(n, CM(a))),
+                }, eF(n, tF(a))),
                 block: {
                     padding: e.spacing.xs,
                     margin: 0,
                     overflowX: "auto"
                 }
             };
             var n, a
         }),
-        LM = Object.defineProperty,
-        AM = Object.getOwnPropertySymbols,
-        MM = Object.prototype.hasOwnProperty,
-        FM = Object.prototype.propertyIsEnumerable,
-        $M = (e, t, r) => t in e ? LM(e, t, {
+        sF = Object.defineProperty,
+        cF = Object.getOwnPropertySymbols,
+        uF = Object.prototype.hasOwnProperty,
+        dF = Object.prototype.propertyIsEnumerable,
+        pF = (e, t, r) => t in e ? sF(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        BM = (e, t) => {
-            for (var r in t || (t = {})) MM.call(t, r) && $M(e, r, t[r]);
-            if (AM)
-                for (var r of AM(t)) FM.call(t, r) && $M(e, r, t[r]);
+        fF = (e, t) => {
+            for (var r in t || (t = {})) uF.call(t, r) && pF(e, r, t[r]);
+            if (cF)
+                for (var r of cF(t)) dF.call(t, r) && pF(e, r, t[r]);
             return e
         };
-    const WM = Object(n.forwardRef)((e, t) => {
+    const mF = Object(n.forwardRef)((e, t) => {
         const r = ir("Code", {}, e),
             {
                 className: n,
                 children: o,
                 block: i,
                 color: l,
                 styles: s,
                 classNames: c
             } = r,
             u = ((e, t) => {
                 var r = {};
-                for (var n in e) MM.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                if (null != e && AM)
-                    for (var n of AM(e)) t.indexOf(n) < 0 && FM.call(e, n) && (r[n] = e[n]);
+                for (var n in e) uF.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                if (null != e && cF)
+                    for (var n of cF(e)) t.indexOf(n) < 0 && dF.call(e, n) && (r[n] = e[n]);
                 return r
             })(r, ["className", "children", "block", "color", "styles", "classNames"]),
             d = or(),
             p = l || ("dark" === d.colorScheme ? "dark" : "gray"),
             {
                 classes: f,
                 cx: m
-            } = _M({
+            } = lF({
                 color: p
             }, {
                 name: "Code",
                 styles: s,
                 classNames: c
             });
-        return i ? a.a.createElement(Cn, BM({
+        return i ? a.a.createElement(Cn, fF({
             component: "pre",
             dir: "ltr",
             className: m(f.root, f.block, n),
             ref: t
-        }, u), o) : a.a.createElement(Cn, BM({
+        }, u), o) : a.a.createElement(Cn, fF({
             component: "code",
             className: m(f.root, n),
             ref: t,
             dir: "ltr"
         }, u), o)
     });
 
-    function HM() {
-        return (HM = Object.assign || function(e) {
+    function bF() {
+        return (bF = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    WM.displayName = "@mantine/core/Code";
-    var VM = function(e) {
+    mF.displayName = "@mantine/core/Code";
+    var gF = function(e) {
         var t = e.children,
             r = e.class_name;
-        return React.createElement(WM, HM({}, G(["setProps", "children", "class_name"], e), {
+        return React.createElement(mF, bF({}, G(["setProps", "children", "class_name"], e), {
             className: r
         }), t)
     };
-    VM.displayName = "Code", VM.defaultProps = {}, VM.propTypes = {
+    gF.displayName = "Code", gF.defaultProps = {}, gF.propTypes = {
         block: i.a.bool,
         children: i.a.node,
         class_name: i.a.string,
         color: i.a.oneOf(["dark", "gray", "red", "pink", "grape", "violet", "indigo", "blue", "cyan", "teal", "green", "lime", "yellow", "orange"]),
         style: i.a.object
     };
-    var qM = VM;
-    const UM = Object(n.createContext)(null);
-    var GM = Er((e, {
+    var yF = gF;
+    const hF = Object(n.createContext)(null);
+    var vF = Er((e, {
             spacing: t,
             center: r
         }, n) => {
             const a = {
                 ref: n("itemWrapper"),
                 display: "inline"
             };
@@ -29345,129 +29672,129 @@
                 itemIcon: {
                     display: "inline-block",
                     verticalAlign: "middle",
                     marginRight: e.spacing.sm
                 }
             }
         }),
-        YM = Object.defineProperty,
-        ZM = Object.getOwnPropertySymbols,
-        KM = Object.prototype.hasOwnProperty,
-        XM = Object.prototype.propertyIsEnumerable,
-        JM = (e, t, r) => t in e ? YM(e, t, {
+        OF = Object.defineProperty,
+        wF = Object.getOwnPropertySymbols,
+        xF = Object.prototype.hasOwnProperty,
+        SF = Object.prototype.propertyIsEnumerable,
+        kF = (e, t, r) => t in e ? OF(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
 
-    function QM(e) {
+    function EF(e) {
         var t = e,
             {
                 className: r,
                 children: o,
                 icon: i
             } = t,
             l = ((e, t) => {
                 var r = {};
-                for (var n in e) KM.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                if (null != e && ZM)
-                    for (var n of ZM(e)) t.indexOf(n) < 0 && XM.call(e, n) && (r[n] = e[n]);
+                for (var n in e) xF.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                if (null != e && wF)
+                    for (var n of wF(e)) t.indexOf(n) < 0 && SF.call(e, n) && (r[n] = e[n]);
                 return r
             })(t, ["className", "children", "icon"]);
         const {
             classNames: s,
             styles: c,
             icon: u,
             spacing: d,
             center: p
-        } = Object(n.useContext)(UM) || {}, f = i || u, {
+        } = Object(n.useContext)(hF) || {}, f = i || u, {
             classes: m,
             cx: b
-        } = GM({
+        } = vF({
             spacing: d,
             center: p
         }, {
             classNames: s,
             styles: c,
             name: "List"
         });
         return a.a.createElement(Cn, ((e, t) => {
-            for (var r in t || (t = {})) KM.call(t, r) && JM(e, r, t[r]);
-            if (ZM)
-                for (var r of ZM(t)) XM.call(t, r) && JM(e, r, t[r]);
+            for (var r in t || (t = {})) xF.call(t, r) && kF(e, r, t[r]);
+            if (wF)
+                for (var r of wF(t)) SF.call(t, r) && kF(e, r, t[r]);
             return e
         })({
             component: "li",
             className: b(m.item, {
                 [m.withIcon]: f
             }, r)
         }, l), a.a.createElement("div", {
             className: m.itemWrapper
         }, f && a.a.createElement("span", {
             className: m.itemIcon
         }, f), a.a.createElement("span", null, o)))
     }
-    QM.displayName = "@mantine/core/ListItem";
-    var eF = Object.defineProperty,
-        tF = Object.defineProperties,
-        rF = Object.getOwnPropertyDescriptors,
-        nF = Object.getOwnPropertySymbols,
-        aF = Object.prototype.hasOwnProperty,
-        oF = Object.prototype.propertyIsEnumerable,
-        iF = (e, t, r) => t in e ? eF(e, t, {
+    EF.displayName = "@mantine/core/ListItem";
+    var jF = Object.defineProperty,
+        PF = Object.defineProperties,
+        zF = Object.getOwnPropertyDescriptors,
+        CF = Object.getOwnPropertySymbols,
+        NF = Object.prototype.hasOwnProperty,
+        TF = Object.prototype.propertyIsEnumerable,
+        DF = (e, t, r) => t in e ? jF(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        lF = (e, t) => {
-            for (var r in t || (t = {})) aF.call(t, r) && iF(e, r, t[r]);
-            if (nF)
-                for (var r of nF(t)) oF.call(t, r) && iF(e, r, t[r]);
+        IF = (e, t) => {
+            for (var r in t || (t = {})) NF.call(t, r) && DF(e, r, t[r]);
+            if (CF)
+                for (var r of CF(t)) TF.call(t, r) && DF(e, r, t[r]);
             return e
         },
-        sF = Er((e, {
+        RF = Er((e, {
             withPadding: t,
             size: r,
             listStyleType: n
         }) => {
             return {
-                root: (a = lF({}, e.fn.fontStyles()), o = {
+                root: (a = IF({}, e.fn.fontStyles()), o = {
                     listStyleType: n,
                     color: "dark" === e.colorScheme ? e.colors.dark[0] : e.black,
                     fontSize: e.fn.size({
                         size: r,
                         sizes: e.fontSizes
                     }),
                     lineHeight: e.lineHeight,
                     margin: 0,
                     paddingLeft: t ? e.spacing.xl : 0,
                     listStylePosition: "inside"
-                }, tF(a, rF(o)))
+                }, PF(a, zF(o)))
             };
             var a, o
         }),
-        cF = Object.defineProperty,
-        uF = Object.getOwnPropertySymbols,
-        dF = Object.prototype.hasOwnProperty,
-        pF = Object.prototype.propertyIsEnumerable,
-        fF = (e, t, r) => t in e ? cF(e, t, {
+        _F = Object.defineProperty,
+        LF = Object.getOwnPropertySymbols,
+        AF = Object.prototype.hasOwnProperty,
+        MF = Object.prototype.propertyIsEnumerable,
+        FF = (e, t, r) => t in e ? _F(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r;
-    const mF = {
+    const $F = {
             type: "unordered",
             size: "md",
             spacing: 0
         },
-        bF = Object(n.forwardRef)((e, t) => {
-            const r = ir("List", mF, e),
+        BF = Object(n.forwardRef)((e, t) => {
+            const r = ir("List", $F, e),
                 {
                     children: n,
                     type: o,
                     size: i,
                     listStyleType: l,
                     withPadding: s,
                     center: c,
@@ -29475,171 +29802,171 @@
                     icon: d,
                     className: p,
                     styles: f,
                     classNames: m
                 } = r,
                 b = ((e, t) => {
                     var r = {};
-                    for (var n in e) dF.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && uF)
-                        for (var n of uF(e)) t.indexOf(n) < 0 && pF.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) AF.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && LF)
+                        for (var n of LF(e)) t.indexOf(n) < 0 && MF.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["children", "type", "size", "listStyleType", "withPadding", "center", "spacing", "icon", "className", "styles", "classNames"]),
                 {
                     classes: g,
                     cx: y
-                } = sF({
+                } = RF({
                     withPadding: s,
                     size: i,
                     listStyleType: l
                 }, {
                     classNames: m,
                     styles: f,
                     name: "List"
                 });
-            return a.a.createElement(UM.Provider, {
+            return a.a.createElement(hF.Provider, {
                 value: {
                     classNames: m,
                     styles: f,
                     spacing: u,
                     center: c,
                     icon: d
                 }
             }, a.a.createElement(Cn, ((e, t) => {
-                for (var r in t || (t = {})) dF.call(t, r) && fF(e, r, t[r]);
-                if (uF)
-                    for (var r of uF(t)) pF.call(t, r) && fF(e, r, t[r]);
+                for (var r in t || (t = {})) AF.call(t, r) && FF(e, r, t[r]);
+                if (LF)
+                    for (var r of LF(t)) MF.call(t, r) && FF(e, r, t[r]);
                 return e
             })({
                 component: "unordered" === o ? "ul" : "ol",
                 className: y(g.root, p),
                 ref: t
             }, b), n))
         });
 
-    function gF() {
-        return (gF = Object.assign || function(e) {
+    function WF() {
+        return (WF = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    bF.Item = QM, bF.displayName = "@mantine/core/List";
-    var yF = function(e) {
+    BF.Item = EF, BF.displayName = "@mantine/core/List";
+    var HF = function(e) {
         var t = e.class_name,
             r = e.children,
             n = e.icon;
-        return a.a.createElement(bF, gF({}, G(["setProps", "children", "class_name", "icon"], e), {
+        return a.a.createElement(BF, WF({}, G(["setProps", "children", "class_name", "icon"], e), {
             className: t,
             icon: ea(n)
         }), a.a.Children.map(r, (function(e, t) {
             var r = e.props._dashprivate_layout.props;
-            return a.a.createElement(bF.Item, {
+            return a.a.createElement(BF.Item, {
                 key: t,
                 className: r.class_name,
                 icon: ea(r.icon),
                 id: r.id
             }, e)
         })))
     };
-    yF.displayName = "List", yF.defaultProps = {}, yF.propTypes = {
+    HF.displayName = "List", HF.defaultProps = {}, HF.propTypes = {
         center: i.a.bool,
         children: i.a.node,
         class_name: i.a.string,
         icon: i.a.any,
         id: i.a.string,
         listStyleType: i.a.string,
         size: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         spacing: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         style: i.a.object,
         type: i.a.oneOf(["ordered", "unordered"]),
         withPadding: i.a.bool
     };
-    var hF = yF,
-        vF = function(e) {
+    var VF = HF,
+        qF = function(e) {
             return a.a.createElement(a.a.Fragment, null, e.children)
         };
-    vF.displayName = "ListItem", vF.defaultProps = {}, vF.propTypes = {
+    qF.displayName = "ListItem", qF.defaultProps = {}, qF.propTypes = {
         children: i.a.node,
         class_name: i.a.string,
         icon: i.a.any,
         id: i.a.string
     };
-    var OF = vF,
-        wF = Object.defineProperty,
-        xF = Object.defineProperties,
-        SF = Object.getOwnPropertyDescriptors,
-        kF = Object.getOwnPropertySymbols,
-        EF = Object.prototype.hasOwnProperty,
-        jF = Object.prototype.propertyIsEnumerable,
-        PF = (e, t, r) => t in e ? wF(e, t, {
+    var UF = qF,
+        GF = Object.defineProperty,
+        YF = Object.defineProperties,
+        ZF = Object.getOwnPropertyDescriptors,
+        KF = Object.getOwnPropertySymbols,
+        XF = Object.prototype.hasOwnProperty,
+        JF = Object.prototype.propertyIsEnumerable,
+        QF = (e, t, r) => t in e ? GF(e, t, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: r
         }) : e[t] = r,
-        zF = (e, t) => {
-            for (var r in t || (t = {})) EF.call(t, r) && PF(e, r, t[r]);
-            if (kF)
-                for (var r of kF(t)) jF.call(t, r) && PF(e, r, t[r]);
+        e$ = (e, t) => {
+            for (var r in t || (t = {})) XF.call(t, r) && QF(e, r, t[r]);
+            if (KF)
+                for (var r of KF(t)) JF.call(t, r) && QF(e, r, t[r]);
             return e
         },
-        CF = (e, t) => xF(e, SF(t));
-    const NF = {
+        t$ = (e, t) => YF(e, ZF(t));
+    const r$ = {
             radius: 0
         },
-        TF = Object(n.forwardRef)((e, t) => {
-            const r = ir("BackgroundImage", NF, e),
+        n$ = Object(n.forwardRef)((e, t) => {
+            const r = ir("BackgroundImage", r$, e),
                 {
                     src: n,
                     radius: o,
                     sx: i
                 } = r,
                 l = ((e, t) => {
                     var r = {};
-                    for (var n in e) EF.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
-                    if (null != e && kF)
-                        for (var n of kF(e)) t.indexOf(n) < 0 && jF.call(e, n) && (r[n] = e[n]);
+                    for (var n in e) XF.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && KF)
+                        for (var n of KF(e)) t.indexOf(n) < 0 && JF.call(e, n) && (r[n] = e[n]);
                     return r
                 })(r, ["src", "radius", "sx"]);
-            return a.a.createElement(Cn, CF(zF({}, l), {
+            return a.a.createElement(Cn, t$(e$({}, l), {
                 ref: t,
-                sx: [e => CF(zF({}, e.fn.focusStyles()), {
+                sx: [e => t$(e$({}, e.fn.focusStyles()), {
                     backgroundSize: "cover",
                     backgroundPosition: "center",
                     display: "block",
                     width: "100%",
                     border: 0,
                     textDecoration: "none",
                     color: "dark" === e.colorScheme ? e.colors.dark[0] : e.black,
                     backgroundImage: `url(${n})`,
                     borderRadius: e.fn.radius(o)
                 }), ...Array.isArray(i) ? i : [i]]
             }))
         });
-    TF.displayName = "@mantine/core/BackgroundImage";
-    var DF = function(e) {
+    n$.displayName = "@mantine/core/BackgroundImage";
+    var a$ = function(e) {
         var t = e.children,
             r = e.radius,
             n = e.src;
-        return a.a.createElement(TF, {
+        return a.a.createElement(n$, {
             radius: r,
             src: n
         }, t)
     };
-    DF.displayName = "BackgroundImage", DF.defaultProps = {}, DF.propTypes = {
+    a$.displayName = "BackgroundImage", a$.defaultProps = {}, a$.propTypes = {
         children: i.a.node,
         id: i.a.string,
         radius: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         src: i.a.string
     };
-    var IF = DF,
-        RF = function(e) {
+    var o$ = a$,
+        i$ = function(e) {
             var t = e.setProps,
                 r = e.label,
                 n = e.value,
                 o = e.style,
                 i = {
                     1: "xs",
                     2: "sm",
@@ -29679,54 +30006,54 @@
                     sm: 2,
                     md: 3,
                     lg: 4,
                     xl: 5
                 } [n]
             }))
         };
-    RF.displayName = "DemoSlider", RF.defaultProps = {}, RF.propTypes = {
+    i$.displayName = "DemoSlider", i$.defaultProps = {}, i$.propTypes = {
         id: i.a.string,
         label: i.a.string,
         setProps: i.a.func,
         style: i.a.object,
         value: i.a.string
     };
-    var _F = RF;
+    var l$ = i$;
 
-    function LF() {
-        return (LF = Object.assign || function(e) {
+    function s$() {
+        return (s$ = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var r = arguments[t];
                 for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
             }
             return e
         }).apply(this, arguments)
     }
-    var AF = function(e) {
+    var c$ = function(e) {
         var t = e.children,
             r = e.n_clicks,
             n = e.setProps,
             o = e.loading,
             i = e.loading_state,
             l = e.class_name,
             s = G(["setProps", "n_clicks", "children", "loading_state", "class_name"], e);
-        return a.a.createElement(ol, LF({}, s, {
+        return a.a.createElement(ol, s$({}, s, {
             onClick: function() {
                 n({
                     n_clicks: r + 1
                 })
             },
             loading: o || i && i.is_loading,
             className: l
         }), t)
     };
-    AF.displayName = "ActionIcon", AF.defaultProps = {
+    c$.displayName = "ActionIcon", c$.defaultProps = {
         n_clicks: 0,
         loading: !1
-    }, AF.propTypes = {
+    }, c$.propTypes = {
         children: i.a.node,
         class_name: i.a.string,
         color: i.a.oneOf(["dark", "gray", "red", "pink", "grape", "violet", "indigo", "blue", "cyan", "teal", "green", "lime", "yellow", "orange"]),
         id: i.a.string,
         loaderProps: i.a.exact({
             color: i.a.oneOf(["dark", "gray", "red", "pink", "grape", "violet", "indigo", "blue", "cyan", "teal", "green", "lime", "yellow", "orange"]),
             size: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
@@ -29741,38 +30068,38 @@
         n_clicks: i.a.number,
         radius: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         size: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
         setProps: i.a.func,
         style: i.a.object,
         variant: i.a.oneOf(["transparent", "default", "hover", "filled", "light", "gradient", "outline"])
     };
-    var MF = AF;
+    var u$ = c$;
 
-    function FF(e) {
+    function d$(e) {
         try {
             return JSON.stringify(e)
         } catch (e) {
             throw new Error("@mantine/hooks use-local-storage: Failed to serialize the value")
         }
     }
 
-    function $F(e) {
+    function p$(e) {
         try {
             return JSON.parse(e)
         } catch (t) {
             return e
         }
     }
 
-    function BF({
+    function f$({
         key: e,
         defaultValue: t,
         getInitialValueInEffect: r = !1,
-        deserialize: a = $F,
-        serialize: o = FF
+        deserialize: a = p$,
+        serialize: o = d$
     }) {
         var i;
         const [l, s] = Object(n.useState)("undefined" != typeof window && "localStorage" in window && !r ? a(null != (i = window.localStorage.getItem(e)) ? i : void 0) : null != t ? t : ""), c = Object(n.useCallback)(t => {
             t instanceof Function ? s(r => {
                 const n = t(r);
                 return window.localStorage.setItem(e, o(n)), n
             }) : (window.localStorage.setItem(e, o(t)), s(t))
@@ -29784,26 +30111,26 @@
             void 0 !== t && void 0 === l && c(t)
         }, [t, l, c]), Object(n.useEffect)(() => {
             var n;
             r && s(a(null != (n = window.localStorage.getItem(e)) ? n : void 0) || (null != t ? t : ""))
         }, []), [void 0 === l ? t : l, c]
     }
 
-    function WF(e, t) {
+    function m$(e, t) {
         if (null == e) return {};
         var r, n, a = {},
             o = Object.keys(e);
         for (n = 0; n < o.length; n++) r = o[n], t.indexOf(r) >= 0 || (a[r] = e[r]);
         return a
     }
-    var HF = ["color"],
-        VF = Object(n.forwardRef)((function(e, t) {
+    var b$ = ["color"],
+        g$ = Object(n.forwardRef)((function(e, t) {
             var r = e.color,
                 a = void 0 === r ? "currentColor" : r,
-                o = WF(e, HF);
+                o = m$(e, b$);
             return Object(n.createElement)("svg", Object.assign({
                 width: "15",
                 height: "15",
                 viewBox: "0 0 15 15",
                 fill: "none",
                 xmlns: "http://www.w3.org/2000/svg"
             }, o, {
@@ -29811,19 +30138,19 @@
             }), Object(n.createElement)("path", {
                 d: "M2.89998 0.499976C2.89998 0.279062 2.72089 0.0999756 2.49998 0.0999756C2.27906 0.0999756 2.09998 0.279062 2.09998 0.499976V1.09998H1.49998C1.27906 1.09998 1.09998 1.27906 1.09998 1.49998C1.09998 1.72089 1.27906 1.89998 1.49998 1.89998H2.09998V2.49998C2.09998 2.72089 2.27906 2.89998 2.49998 2.89998C2.72089 2.89998 2.89998 2.72089 2.89998 2.49998V1.89998H3.49998C3.72089 1.89998 3.89998 1.72089 3.89998 1.49998C3.89998 1.27906 3.72089 1.09998 3.49998 1.09998H2.89998V0.499976ZM5.89998 3.49998C5.89998 3.27906 5.72089 3.09998 5.49998 3.09998C5.27906 3.09998 5.09998 3.27906 5.09998 3.49998V4.09998H4.49998C4.27906 4.09998 4.09998 4.27906 4.09998 4.49998C4.09998 4.72089 4.27906 4.89998 4.49998 4.89998H5.09998V5.49998C5.09998 5.72089 5.27906 5.89998 5.49998 5.89998C5.72089 5.89998 5.89998 5.72089 5.89998 5.49998V4.89998H6.49998C6.72089 4.89998 6.89998 4.72089 6.89998 4.49998C6.89998 4.27906 6.72089 4.09998 6.49998 4.09998H5.89998V3.49998ZM1.89998 6.49998C1.89998 6.27906 1.72089 6.09998 1.49998 6.09998C1.27906 6.09998 1.09998 6.27906 1.09998 6.49998V7.09998H0.499976C0.279062 7.09998 0.0999756 7.27906 0.0999756 7.49998C0.0999756 7.72089 0.279062 7.89998 0.499976 7.89998H1.09998V8.49998C1.09998 8.72089 1.27906 8.89997 1.49998 8.89997C1.72089 8.89997 1.89998 8.72089 1.89998 8.49998V7.89998H2.49998C2.72089 7.89998 2.89998 7.72089 2.89998 7.49998C2.89998 7.27906 2.72089 7.09998 2.49998 7.09998H1.89998V6.49998ZM8.54406 0.98184L8.24618 0.941586C8.03275 0.917676 7.90692 1.1655 8.02936 1.34194C8.17013 1.54479 8.29981 1.75592 8.41754 1.97445C8.91878 2.90485 9.20322 3.96932 9.20322 5.10022C9.20322 8.37201 6.82247 11.0878 3.69887 11.6097C3.45736 11.65 3.20988 11.6772 2.96008 11.6906C2.74563 11.702 2.62729 11.9535 2.77721 12.1072C2.84551 12.1773 2.91535 12.2458 2.98667 12.3128L3.05883 12.3795L3.31883 12.6045L3.50684 12.7532L3.62796 12.8433L3.81491 12.9742L3.99079 13.089C4.11175 13.1651 4.23536 13.2375 4.36157 13.3059L4.62496 13.4412L4.88553 13.5607L5.18837 13.6828L5.43169 13.7686C5.56564 13.8128 5.70149 13.8529 5.83857 13.8885C5.94262 13.9155 6.04767 13.9401 6.15405 13.9622C6.27993 13.9883 6.40713 14.0109 6.53544 14.0298L6.85241 14.0685L7.11934 14.0892C7.24637 14.0965 7.37436 14.1002 7.50322 14.1002C11.1483 14.1002 14.1032 11.1453 14.1032 7.50023C14.1032 7.25044 14.0893 7.00389 14.0623 6.76131L14.0255 6.48407C13.991 6.26083 13.9453 6.04129 13.8891 5.82642C13.8213 5.56709 13.7382 5.31398 13.6409 5.06881L13.5279 4.80132L13.4507 4.63542L13.3766 4.48666C13.2178 4.17773 13.0353 3.88295 12.8312 3.60423L12.6782 3.40352L12.4793 3.16432L12.3157 2.98361L12.1961 2.85951L12.0355 2.70246L11.8134 2.50184L11.4925 2.24191L11.2483 2.06498L10.9562 1.87446L10.6346 1.68894L10.3073 1.52378L10.1938 1.47176L9.95488 1.3706L9.67791 1.2669L9.42566 1.1846L9.10075 1.09489L8.83599 1.03486L8.54406 0.98184ZM10.4032 5.30023C10.4032 4.27588 10.2002 3.29829 9.83244 2.40604C11.7623 3.28995 13.1032 5.23862 13.1032 7.50023C13.1032 10.593 10.596 13.1002 7.50322 13.1002C6.63646 13.1002 5.81597 12.9036 5.08355 12.5522C6.5419 12.0941 7.81081 11.2082 8.74322 10.0416C8.87963 10.2284 9.10028 10.3497 9.34928 10.3497C9.76349 10.3497 10.0993 10.0139 10.0993 9.59971C10.0993 9.24256 9.84965 8.94373 9.51535 8.86816C9.57741 8.75165 9.63653 8.63334 9.6926 8.51332C9.88358 8.63163 10.1088 8.69993 10.35 8.69993C11.0403 8.69993 11.6 8.14028 11.6 7.44993C11.6 6.75976 11.0406 6.20024 10.3505 6.19993C10.3853 5.90487 10.4032 5.60464 10.4032 5.30023Z",
                 fill: a,
                 fillRule: "evenodd",
                 clipRule: "evenodd"
             }))
         })),
-        qF = ["color"],
-        UF = Object(n.forwardRef)((function(e, t) {
+        y$ = ["color"],
+        h$ = Object(n.forwardRef)((function(e, t) {
             var r = e.color,
                 a = void 0 === r ? "currentColor" : r,
-                o = WF(e, qF);
+                o = m$(e, y$);
             return Object(n.createElement)("svg", Object.assign({
                 width: "15",
                 height: "15",
                 viewBox: "0 0 15 15",
                 fill: "none",
                 xmlns: "http://www.w3.org/2000/svg"
             }, o, {
@@ -29832,15 +30159,15 @@
                 d: "M7.5 0C7.77614 0 8 0.223858 8 0.5V2.5C8 2.77614 7.77614 3 7.5 3C7.22386 3 7 2.77614 7 2.5V0.5C7 0.223858 7.22386 0 7.5 0ZM2.1967 2.1967C2.39196 2.00144 2.70854 2.00144 2.90381 2.1967L4.31802 3.61091C4.51328 3.80617 4.51328 4.12276 4.31802 4.31802C4.12276 4.51328 3.80617 4.51328 3.61091 4.31802L2.1967 2.90381C2.00144 2.70854 2.00144 2.39196 2.1967 2.1967ZM0.5 7C0.223858 7 0 7.22386 0 7.5C0 7.77614 0.223858 8 0.5 8H2.5C2.77614 8 3 7.77614 3 7.5C3 7.22386 2.77614 7 2.5 7H0.5ZM2.1967 12.8033C2.00144 12.608 2.00144 12.2915 2.1967 12.0962L3.61091 10.682C3.80617 10.4867 4.12276 10.4867 4.31802 10.682C4.51328 10.8772 4.51328 11.1938 4.31802 11.3891L2.90381 12.8033C2.70854 12.9986 2.39196 12.9986 2.1967 12.8033ZM12.5 7C12.2239 7 12 7.22386 12 7.5C12 7.77614 12.2239 8 12.5 8H14.5C14.7761 8 15 7.77614 15 7.5C15 7.22386 14.7761 7 14.5 7H12.5ZM10.682 4.31802C10.4867 4.12276 10.4867 3.80617 10.682 3.61091L12.0962 2.1967C12.2915 2.00144 12.608 2.00144 12.8033 2.1967C12.9986 2.39196 12.9986 2.70854 12.8033 2.90381L11.3891 4.31802C11.1938 4.51328 10.8772 4.51328 10.682 4.31802ZM8 12.5C8 12.2239 7.77614 12 7.5 12C7.22386 12 7 12.2239 7 12.5V14.5C7 14.7761 7.22386 15 7.5 15C7.77614 15 8 14.7761 8 14.5V12.5ZM10.682 10.682C10.8772 10.4867 11.1938 10.4867 11.3891 10.682L12.8033 12.0962C12.9986 12.2915 12.9986 12.608 12.8033 12.8033C12.608 12.9986 12.2915 12.9986 12.0962 12.8033L10.682 11.3891C10.4867 11.1938 10.4867 10.8772 10.682 10.682ZM5.5 7.5C5.5 6.39543 6.39543 5.5 7.5 5.5C8.60457 5.5 9.5 6.39543 9.5 7.5C9.5 8.60457 8.60457 9.5 7.5 9.5C6.39543 9.5 5.5 8.60457 5.5 7.5ZM7.5 4.5C5.84315 4.5 4.5 5.84315 4.5 7.5C4.5 9.15685 5.84315 10.5 7.5 10.5C9.15685 10.5 10.5 9.15685 10.5 7.5C10.5 5.84315 9.15685 4.5 7.5 4.5Z",
                 fill: a,
                 fillRule: "evenodd",
                 clipRule: "evenodd"
             }))
         }));
 
-    function GF(e, t) {
+    function v$(e, t) {
         return function(e) {
             if (Array.isArray(e)) return e
         }(e) || function(e, t) {
             var r = null == e ? null : "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
             if (null == r) return;
             var n, a, o = [],
                 i = !0,
@@ -29855,70 +30182,668 @@
                 } finally {
                     if (l) throw a
                 }
             }
             return o
         }(e, t) || function(e, t) {
             if (!e) return;
-            if ("string" == typeof e) return YF(e, t);
+            if ("string" == typeof e) return O$(e, t);
             var r = Object.prototype.toString.call(e).slice(8, -1);
             "Object" === r && e.constructor && (r = e.constructor.name);
             if ("Map" === r || "Set" === r) return Array.from(e);
-            if ("Arguments" === r || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(r)) return YF(e, t)
+            if ("Arguments" === r || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(r)) return O$(e, t)
         }(e, t) || function() {
             throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()
     }
 
-    function YF(e, t) {
+    function O$(e, t) {
         (null == t || t > e.length) && (t = e.length);
         for (var r = 0, n = new Array(t); r < t; r++) n[r] = e[r];
         return n
     }
-    var ZF = function(e) {
+    var w$ = function(e) {
         var t = e.style,
             r = e.setProps,
-            o = GF(BF({
+            o = v$(f$({
                 key: "color-scheme",
                 defaultValue: "light"
             }), 2),
             i = o[0],
             l = o[1];
         return Object(n.useEffect)((function() {
             r({
                 value: i
             })
-        }), [i]), a.a.createElement(Kw, {
-            label: "Change Theme"
-        }, a.a.createElement(NR, {
+        }), [i]), a.a.createElement(r_, {
             size: 36,
             radius: 30,
             style: t,
             variant: "outline",
             onClick: function() {
                 return l((function(e) {
                     return "dark" === e ? "light" : "dark"
                 }))
             },
             color: "dark" === i ? "yellow" : "dark"
-        }, "dark" === i ? a.a.createElement(UF, {
+        }, "dark" === i ? a.a.createElement(h$, {
             size: 22
-        }) : a.a.createElement(VF, {
+        }) : a.a.createElement(g$, {
             size: 22
-        })))
+        }))
     };
-    ZF.displayName = "ThemeSwitcher", ZF.defaultProps = {
+    w$.displayName = "ThemeSwitcher", w$.defaultProps = {
         value: "light"
-    }, ZF.propTypes = {
+    }, w$.propTypes = {
         id: i.a.string,
         setProps: i.a.func,
         style: i.a.object,
         value: i.a.oneOf(["dark", "light"])
     };
-    var KF = ZF;
+    var x$ = w$,
+        S$ = Er((e, {
+            spacing: t,
+            align: r,
+            justify: n
+        }) => ({
+            root: {
+                display: "flex",
+                flexDirection: "column",
+                alignItems: r,
+                justifyContent: n,
+                gap: e.fn.size({
+                    size: t,
+                    sizes: e.spacing
+                })
+            }
+        })),
+        k$ = Object.defineProperty,
+        E$ = Object.getOwnPropertySymbols,
+        j$ = Object.prototype.hasOwnProperty,
+        P$ = Object.prototype.propertyIsEnumerable,
+        z$ = (e, t, r) => t in e ? k$(e, t, {
+            enumerable: !0,
+            configurable: !0,
+            writable: !0,
+            value: r
+        }) : e[t] = r;
+    const C$ = {
+            spacing: "md",
+            align: "stretch",
+            justify: "top"
+        },
+        N$ = Object(n.forwardRef)((e, t) => {
+            const r = ir("Stack", C$, e),
+                {
+                    spacing: n,
+                    className: o,
+                    classNames: i,
+                    styles: l,
+                    align: s,
+                    justify: c
+                } = r,
+                u = ((e, t) => {
+                    var r = {};
+                    for (var n in e) j$.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && E$)
+                        for (var n of E$(e)) t.indexOf(n) < 0 && P$.call(e, n) && (r[n] = e[n]);
+                    return r
+                })(r, ["spacing", "className", "classNames", "styles", "align", "justify"]),
+                {
+                    classes: d,
+                    cx: p
+                } = S$({
+                    spacing: n,
+                    align: s,
+                    justify: c
+                }, {
+                    name: "Stack",
+                    classNames: i,
+                    styles: l
+                });
+            return a.a.createElement(Cn, ((e, t) => {
+                for (var r in t || (t = {})) j$.call(t, r) && z$(e, r, t[r]);
+                if (E$)
+                    for (var r of E$(t)) P$.call(t, r) && z$(e, r, t[r]);
+                return e
+            })({
+                className: p(d.root, o),
+                ref: t
+            }, u))
+        });
+
+    function T$() {
+        return (T$ = Object.assign || function(e) {
+            for (var t = 1; t < arguments.length; t++) {
+                var r = arguments[t];
+                for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
+            }
+            return e
+        }).apply(this, arguments)
+    }
+    N$.displayName = "@mantine/core/Stack";
+    var D$ = function(e) {
+        var t = e.children,
+            r = e.class_name;
+        return a.a.createElement(N$, T$({
+            className: r
+        }, G(["setProps", "children", "class_name"], e)), a.a.Children.map(t, (function(e, t) {
+            return a.a.createElement("div", {
+                key: t
+            }, e)
+        })))
+    };
+    D$.displayName = "Stack", D$.defaultProps = {}, D$.propTypes = {
+        align: i.a.oneOf(["stretch", "center", "flex-end", "flex-start"]),
+        children: i.a.node,
+        class_name: i.a.string,
+        justify: i.a.oneOf(["space-between", "space-around", "center", "flex-end", "flex-start"]),
+        spacing: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
+        style: i.a.object
+    };
+    var I$ = D$;
+
+    function R$(e, t) {
+        const r = t - e + 1;
+        return Array.from({
+            length: r
+        }, (t, r) => r + e)
+    }
+    var _$ = Object.defineProperty,
+        L$ = Object.getOwnPropertySymbols,
+        A$ = Object.prototype.hasOwnProperty,
+        M$ = Object.prototype.propertyIsEnumerable,
+        F$ = (e, t, r) => t in e ? _$(e, t, {
+            enumerable: !0,
+            configurable: !0,
+            writable: !0,
+            value: r
+        }) : e[t] = r;
+
+    function $$(e) {
+        return a.a.createElement("svg", ((e, t) => {
+            for (var r in t || (t = {})) A$.call(t, r) && F$(e, r, t[r]);
+            if (L$)
+                for (var r of L$(t)) M$.call(t, r) && F$(e, r, t[r]);
+            return e
+        })({
+            width: 16,
+            height: 16,
+            viewBox: "0 0 16 16",
+            fill: "none",
+            xmlns: "http://www.w3.org/2000/svg"
+        }, e), a.a.createElement("path", {
+            d: "M2 8c0-.733.6-1.333 1.333-1.333.734 0 1.334.6 1.334 1.333s-.6 1.333-1.334 1.333C2.6 9.333 2 8.733 2 8zm9.333 0c0-.733.6-1.333 1.334-1.333C13.4 6.667 14 7.267 14 8s-.6 1.333-1.333 1.333c-.734 0-1.334-.6-1.334-1.333zM6.667 8c0-.733.6-1.333 1.333-1.333s1.333.6 1.333 1.333S8.733 9.333 8 9.333 6.667 8.733 6.667 8z",
+            fill: "currentColor"
+        }))
+    }
+    var B$ = Object.defineProperty,
+        W$ = Object.getOwnPropertySymbols,
+        H$ = Object.prototype.hasOwnProperty,
+        V$ = Object.prototype.propertyIsEnumerable,
+        q$ = (e, t, r) => t in e ? B$(e, t, {
+            enumerable: !0,
+            configurable: !0,
+            writable: !0,
+            value: r
+        }) : e[t] = r;
+
+    function U$(e) {
+        return a.a.createElement("svg", ((e, t) => {
+            for (var r in t || (t = {})) H$.call(t, r) && q$(e, r, t[r]);
+            if (W$)
+                for (var r of W$(t)) V$.call(t, r) && q$(e, r, t[r]);
+            return e
+        })({
+            width: 16,
+            height: 16,
+            viewBox: "0 0 16 16",
+            fill: "none",
+            xmlns: "http://www.w3.org/2000/svg"
+        }, e), a.a.createElement("path", {
+            d: "M8.781 8l-3.3-3.3.943-.943L10.667 8l-4.243 4.243-.943-.943 3.3-3.3z",
+            fill: "currentColor"
+        }))
+    }
+    var G$ = Object.defineProperty,
+        Y$ = Object.getOwnPropertySymbols,
+        Z$ = Object.prototype.hasOwnProperty,
+        K$ = Object.prototype.propertyIsEnumerable,
+        X$ = (e, t, r) => t in e ? G$(e, t, {
+            enumerable: !0,
+            configurable: !0,
+            writable: !0,
+            value: r
+        }) : e[t] = r;
+
+    function J$(e) {
+        return a.a.createElement("svg", ((e, t) => {
+            for (var r in t || (t = {})) Z$.call(t, r) && X$(e, r, t[r]);
+            if (Y$)
+                for (var r of Y$(t)) K$.call(t, r) && X$(e, r, t[r]);
+            return e
+        })({
+            width: 16,
+            height: 16,
+            viewBox: "0 0 16 16",
+            fill: "none",
+            xmlns: "http://www.w3.org/2000/svg"
+        }, e), a.a.createElement("path", {
+            d: "M7.219 8l3.3 3.3-.943.943L5.333 8l4.243-4.243.943.943-3.3 3.3z",
+            fill: "currentColor"
+        }))
+    }
+    var Q$ = Object.defineProperty,
+        eB = Object.getOwnPropertySymbols,
+        tB = Object.prototype.hasOwnProperty,
+        rB = Object.prototype.propertyIsEnumerable,
+        nB = (e, t, r) => t in e ? Q$(e, t, {
+            enumerable: !0,
+            configurable: !0,
+            writable: !0,
+            value: r
+        }) : e[t] = r;
+
+    function aB(e) {
+        return a.a.createElement("svg", ((e, t) => {
+            for (var r in t || (t = {})) tB.call(t, r) && nB(e, r, t[r]);
+            if (eB)
+                for (var r of eB(t)) rB.call(t, r) && nB(e, r, t[r]);
+            return e
+        })({
+            width: 16,
+            height: 16,
+            viewBox: "0 0 16 16",
+            fill: "none",
+            xmlns: "http://www.w3.org/2000/svg"
+        }, e), a.a.createElement("path", {
+            d: "M6.85355 3.85355C7.04882 3.65829 7.04882 3.34171 6.85355 3.14645C6.65829 2.95118 6.34171 2.95118 6.14645 3.14645L2.14645 7.14645C1.95118 7.34171 1.95118 7.65829 2.14645 7.85355L6.14645 11.8536C6.34171 12.0488 6.65829 12.0488 6.85355 11.8536C7.04882 11.6583 7.04882 11.3417 6.85355 11.1464L3.20711 7.5L6.85355 3.85355ZM12.8536 3.85355C13.0488 3.65829 13.0488 3.34171 12.8536 3.14645C12.6583 2.95118 12.3417 2.95118 12.1464 3.14645L8.14645 7.14645C7.95118 7.34171 7.95118 7.65829 8.14645 7.85355L12.1464 11.8536C12.3417 12.0488 12.6583 12.0488 12.8536 11.8536C13.0488 11.6583 13.0488 11.3417 12.8536 11.1464L9.20711 7.5L12.8536 3.85355Z",
+            fill: "currentColor"
+        }))
+    }
+    var oB = Object.defineProperty,
+        iB = Object.getOwnPropertySymbols,
+        lB = Object.prototype.hasOwnProperty,
+        sB = Object.prototype.propertyIsEnumerable,
+        cB = (e, t, r) => t in e ? oB(e, t, {
+            enumerable: !0,
+            configurable: !0,
+            writable: !0,
+            value: r
+        }) : e[t] = r;
+
+    function uB(e) {
+        return a.a.createElement("svg", ((e, t) => {
+            for (var r in t || (t = {})) lB.call(t, r) && cB(e, r, t[r]);
+            if (iB)
+                for (var r of iB(t)) sB.call(t, r) && cB(e, r, t[r]);
+            return e
+        })({
+            width: 16,
+            height: 16,
+            viewBox: "0 0 16 16",
+            fill: "none",
+            xmlns: "http://www.w3.org/2000/svg"
+        }, e), a.a.createElement("path", {
+            d: "M2.14645 11.1464C1.95118 11.3417 1.95118 11.6583 2.14645 11.8536C2.34171 12.0488 2.65829 12.0488 2.85355 11.8536L6.85355 7.85355C7.04882 7.65829 7.04882 7.34171 6.85355 7.14645L2.85355 3.14645C2.65829 2.95118 2.34171 2.95118 2.14645 3.14645C1.95118 3.34171 1.95118 3.65829 2.14645 3.85355L5.79289 7.5L2.14645 11.1464ZM8.14645 11.1464C7.95118 11.3417 7.95118 11.6583 8.14645 11.8536C8.34171 12.0488 8.65829 12.0488 8.85355 11.8536L12.8536 7.85355C13.0488 7.65829 13.0488 7.34171 12.8536 7.14645L8.85355 3.14645C8.65829 2.95118 8.34171 2.95118 8.14645 3.14645C7.95118 3.34171 7.95118 3.65829 8.14645 3.85355L11.7929 7.5L8.14645 11.1464Z",
+            fill: "currentColor"
+        }))
+    }
+    var dB = Object.defineProperty,
+        pB = Object.getOwnPropertySymbols,
+        fB = Object.prototype.hasOwnProperty,
+        mB = Object.prototype.propertyIsEnumerable,
+        bB = (e, t, r) => t in e ? dB(e, t, {
+            enumerable: !0,
+            configurable: !0,
+            writable: !0,
+            value: r
+        }) : e[t] = r;
+    const gB = {
+            dots: $$,
+            next: U$,
+            prev: J$,
+            first: aB,
+            last: uB
+        },
+        yB = {
+            dots: $$,
+            prev: U$,
+            next: J$,
+            last: aB,
+            first: uB
+        };
+
+    function hB(e) {
+        var t = e,
+            {
+                page: r,
+                active: n,
+                onClick: o
+            } = t,
+            i = ((e, t) => {
+                var r = {};
+                for (var n in e) fB.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                if (null != e && pB)
+                    for (var n of pB(e)) t.indexOf(n) < 0 && mB.call(e, n) && (r[n] = e[n]);
+                return r
+            })(t, ["page", "active", "onClick"]);
+        const l = ("rtl" === or().dir ? yB : gB)[r],
+            s = l ? a.a.createElement(l, null) : r;
+        return a.a.createElement("button", ((e, t) => {
+            for (var r in t || (t = {})) fB.call(t, r) && bB(e, r, t[r]);
+            if (pB)
+                for (var r of pB(t)) mB.call(t, r) && bB(e, r, t[r]);
+            return e
+        })({
+            type: "button",
+            onClick: o
+        }, i), s)
+    }
+    hB.displayName = "@mantine/core/Pagination/DefaultItem";
+    var vB = Object.defineProperty,
+        OB = Object.defineProperties,
+        wB = Object.getOwnPropertyDescriptors,
+        xB = Object.getOwnPropertySymbols,
+        SB = Object.prototype.hasOwnProperty,
+        kB = Object.prototype.propertyIsEnumerable,
+        EB = (e, t, r) => t in e ? vB(e, t, {
+            enumerable: !0,
+            configurable: !0,
+            writable: !0,
+            value: r
+        }) : e[t] = r,
+        jB = (e, t) => {
+            for (var r in t || (t = {})) SB.call(t, r) && EB(e, r, t[r]);
+            if (xB)
+                for (var r of xB(t)) kB.call(t, r) && EB(e, r, t[r]);
+            return e
+        };
+    const PB = {
+        xs: 22,
+        sm: 26,
+        md: 32,
+        lg: 38,
+        xl: 44
+    };
+    var zB = Er((e, {
+            size: t,
+            radius: r,
+            color: n
+        }, a) => {
+            const o = dr({
+                color: n,
+                theme: e,
+                variant: "filled"
+            });
+            return {
+                item: (i = jB({}, e.fn.focusStyles()), l = {
+                    cursor: "pointer",
+                    userSelect: "none",
+                    display: "flex",
+                    alignItems: "center",
+                    justifyContent: "center",
+                    fontWeight: 500,
+                    border: "1px solid " + ("dark" === e.colorScheme ? e.colors.dark[5] : e.colors.gray[3]),
+                    color: "dark" === e.colorScheme ? e.colors.dark[0] : e.black,
+                    height: e.fn.size({
+                        size: t,
+                        sizes: PB
+                    }),
+                    minWidth: e.fn.size({
+                        size: t,
+                        sizes: PB
+                    }),
+                    padding: `0 ${e.fn.size({size:t,sizes:e.spacing})/2}px`,
+                    fontSize: e.fn.size({
+                        size: t,
+                        sizes: e.fontSizes
+                    }),
+                    borderRadius: e.fn.radius(r),
+                    lineHeight: 1,
+                    backgroundColor: "dark" === e.colorScheme ? e.colors.dark[5] : e.white,
+                    [`&:active:not(:disabled):not(.${a("dots")})`]: {
+                        transform: "translateY(1px)"
+                    },
+                    "&:disabled": {
+                        opacity: .6,
+                        cursor: "not-allowed",
+                        color: "dark" === e.colorScheme ? e.colors.dark[3] : e.colors.gray[5]
+                    }
+                }, OB(i, wB(l))),
+                active: {
+                    borderColor: "transparent",
+                    color: o.color,
+                    backgroundColor: o.background
+                },
+                dots: {
+                    ref: a("dots"),
+                    cursor: "default",
+                    borderColor: "transparent",
+                    backgroundColor: "transparent"
+                }
+            };
+            var i, l
+        }),
+        CB = Object.defineProperty,
+        NB = Object.getOwnPropertySymbols,
+        TB = Object.prototype.hasOwnProperty,
+        DB = Object.prototype.propertyIsEnumerable,
+        IB = (e, t, r) => t in e ? CB(e, t, {
+            enumerable: !0,
+            configurable: !0,
+            writable: !0,
+            value: r
+        }) : e[t] = r;
+    const RB = {
+            itemComponent: hB,
+            initialPage: 1,
+            siblings: 1,
+            boundaries: 1,
+            size: "md",
+            radius: "sm",
+            withEdges: !1,
+            withControls: !0
+        },
+        _B = Object(n.forwardRef)((e, t) => {
+            const r = ir("Pagination", RB, e),
+                {
+                    itemComponent: o,
+                    classNames: i,
+                    styles: l,
+                    page: s,
+                    initialPage: c,
+                    color: u,
+                    total: d,
+                    siblings: p,
+                    boundaries: f,
+                    size: m,
+                    radius: b,
+                    onChange: g,
+                    getItemAriaLabel: y,
+                    spacing: h,
+                    withEdges: v,
+                    withControls: O,
+                    sx: w
+                } = r,
+                x = ((e, t) => {
+                    var r = {};
+                    for (var n in e) TB.call(e, n) && t.indexOf(n) < 0 && (r[n] = e[n]);
+                    if (null != e && NB)
+                        for (var n of NB(e)) t.indexOf(n) < 0 && DB.call(e, n) && (r[n] = e[n]);
+                    return r
+                })(r, ["itemComponent", "classNames", "styles", "page", "initialPage", "color", "total", "siblings", "boundaries", "size", "radius", "onChange", "getItemAriaLabel", "spacing", "withEdges", "withControls", "sx"]),
+                {
+                    classes: S,
+                    cx: k,
+                    theme: E
+                } = zB({
+                    color: u,
+                    size: m,
+                    radius: b
+                }, {
+                    classNames: i,
+                    styles: l,
+                    name: "Pagination"
+                }),
+                {
+                    range: j,
+                    setPage: P,
+                    next: z,
+                    previous: C,
+                    active: N,
+                    first: T,
+                    last: D
+                } = function({
+                    total: e,
+                    siblings: t = 1,
+                    boundaries: r = 1,
+                    page: a,
+                    initialPage: o = 1,
+                    onChange: i
+                }) {
+                    const [l, s] = la({
+                        value: a,
+                        onChange: i,
+                        defaultValue: o,
+                        finalValue: o,
+                        rule: t => "number" == typeof t && t <= e
+                    }), c = t => {
+                        s(t <= 0 ? 1 : t > e ? e : t)
+                    };
+                    return {
+                        range: Object(n.useMemo)(() => {
+                            if (2 * t + 3 + 2 * r >= e) return R$(1, e);
+                            const n = Math.max(l - t, r),
+                                a = Math.min(l + t, e - r),
+                                o = n > r + 2,
+                                i = a < e - (r + 1);
+                            if (!o && i) {
+                                return [...R$(1, 2 * t + r + 2), "dots", ...R$(e - (r - 1), e)]
+                            }
+                            if (o && !i) {
+                                const n = r + 1 + 2 * t;
+                                return [...R$(1, r), "dots", ...R$(e - n, e)]
+                            }
+                            return [...R$(1, r), "dots", ...R$(n, a), "dots", ...R$(e - r + 1, e)]
+                        }, [e, t, l]),
+                        active: l,
+                        setPage: c,
+                        next: () => c(l + 1),
+                        previous: () => c(l - 1),
+                        first: () => c(1),
+                        last: () => c(e)
+                    }
+                }({
+                    page: s,
+                    siblings: p,
+                    total: d,
+                    onChange: g,
+                    initialPage: c,
+                    boundaries: f
+                }),
+                I = j.map((e, t) => a.a.createElement(o, {
+                    key: t,
+                    page: e,
+                    active: e === N,
+                    "aria-label": "function" == typeof y ? y(e) : null,
+                    tabIndex: "dots" === e ? -1 : 0,
+                    className: k(S.item, {
+                        [S.active]: e === N,
+                        [S.dots]: "dots" === e
+                    }),
+                    onClick: "dots" !== e ? () => P(e) : void 0
+                }));
+            return a.a.createElement(Ma, ((e, t) => {
+                for (var r in t || (t = {})) TB.call(t, r) && IB(e, r, t[r]);
+                if (NB)
+                    for (var r of NB(t)) DB.call(t, r) && IB(e, r, t[r]);
+                return e
+            })({
+                spacing: h || E.fn.size({
+                    size: m,
+                    sizes: E.spacing
+                }) / 2,
+                ref: t,
+                sx: w
+            }, x), v && a.a.createElement(o, {
+                page: "first",
+                onClick: T,
+                "aria-label": y ? y("first") : void 0,
+                "aria-disabled": 1 === N,
+                className: S.item,
+                disabled: 1 === N
+            }), O && a.a.createElement(o, {
+                page: "prev",
+                onClick: C,
+                "aria-label": y ? y("prev") : void 0,
+                "aria-disabled": 1 === N,
+                className: S.item,
+                disabled: 1 === N
+            }), I, O && a.a.createElement(o, {
+                page: "next",
+                onClick: z,
+                "aria-label": y ? y("next") : void 0,
+                "aria-disabled": N === d,
+                className: S.item,
+                disabled: N === d
+            }), v && a.a.createElement(o, {
+                page: "last",
+                onClick: D,
+                "aria-label": y ? y("last") : void 0,
+                "aria-disabled": N === d,
+                className: S.item,
+                disabled: N === d
+            }))
+        });
+
+    function LB() {
+        return (LB = Object.assign || function(e) {
+            for (var t = 1; t < arguments.length; t++) {
+                var r = arguments[t];
+                for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
+            }
+            return e
+        }).apply(this, arguments)
+    }
+    _B.displayName = "@mantine/core/Pagination";
+    var AB = function(e) {
+        var t = e.setProps,
+            r = e.class_name;
+        return a.a.createElement(_B, LB({}, G(["setProps", "class_name"], e), {
+            onChange: function(e) {
+                return t({
+                    page: e
+                })
+            },
+            className: r
+        }))
+    };
+    AB.displayName = "Pagination", AB.defaultProps = {}, AB.propTypes = {
+        align: i.a.oneOf(["stretch", "center", "flex-end", "flex-start"]),
+        boundaries: i.a.number,
+        class_name: i.a.string,
+        color: i.a.oneOf(["dark", "gray", "red", "pink", "grape", "violet", "indigo", "blue", "cyan", "teal", "green", "lime", "yellow", "orange"]),
+        direction: i.a.oneOf(["row", "column"]),
+        grow: i.a.bool,
+        id: i.a.string,
+        noWrap: i.a.bool,
+        page: i.a.number,
+        position: i.a.oneOf(["right", "center", "left", "apart"]),
+        radius: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
+        setProps: i.a.func,
+        siblings: i.a.number,
+        size: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
+        spacing: i.a.oneOfType([i.a.oneOf(["xs", "sm", "md", "lg", "xl"]), i.a.number]),
+        style: i.a.object,
+        total: i.a.number.isRequired,
+        withControls: i.a.bool,
+        withEdges: i.a.bool
+    };
+    var MB = AB;
     r.d(t, "Button", (function() {
         return aa
     })), r.d(t, "Tab", (function() {
         return ia
     })), r.d(t, "Tabs", (function() {
         return Za
     })), r.d(t, "RadioGroup", (function() {
@@ -29941,131 +30866,137 @@
         return Lh
     })), r.d(t, "Slider", (function() {
         return Fv
     })), r.d(t, "Alert", (function() {
         return oO
     })), r.d(t, "TextInput", (function() {
         return hO
+    })), r.d(t, "PasswordInput", (function() {
+        return VO
     })), r.d(t, "Center", (function() {
-        return PO
+        return QO
     })), r.d(t, "Container", (function() {
-        return MO
+        return uw
     })), r.d(t, "SegmentedControl", (function() {
-        return lw
+        return Iw
     })), r.d(t, "Switch", (function() {
-        return Rw
+        return ix
     })), r.d(t, "Tooltip", (function() {
-        return Qw
+        return Ex
     })), r.d(t, "Modal", (function() {
-        return lx
+        return Ix
     })), r.d(t, "Prism", (function() {
-        return $x
+        return pS
     })), r.d(t, "Col", (function() {
-        return gS
+        return WS
     })), r.d(t, "Grid", (function() {
-        return vS
+        return qS
     })), r.d(t, "Group", (function() {
-        return xS
+        return YS
     })), r.d(t, "Text", (function() {
-        return ES
+        return XS
     })), r.d(t, "Title", (function() {
-        return VS
+        return gk
     })), r.d(t, "SimpleGrid", (function() {
-        return lk
+        return Ik
     })), r.d(t, "Affix", (function() {
-        return hk
+        return Vk
     })), r.d(t, "Space", (function() {
-        return zk
+        return eE
     })), r.d(t, "Chips", (function() {
-        return oE
+        return TE
     })), r.d(t, "Badge", (function() {
-        return jE
+        return JE
     })), r.d(t, "Anchor", (function() {
-        return ME
+        return uj
     })), r.d(t, "Image", (function() {
-        return dj
+        return Aj
     })), r.d(t, "Blockquote", (function() {
-        return Lj
+        return sP
     })), r.d(t, "Accordion", (function() {
-        return UP
+        return hz
     })), r.d(t, "AccordionItem", (function() {
-        return YP
+        return Oz
     })), r.d(t, "Skeleton", (function() {
-        return iz
+        return Dz
     })), r.d(t, "Spoiler", (function() {
-        return yz
+        return Hz
     })), r.d(t, "Paper", (function() {
-        return Oz
+        return Uz
     })), r.d(t, "Breadcrumbs", (function() {
-        return Nz
+        return rC
     })), r.d(t, "Progress", (function() {
-        return Gz
+        return vC
     })), r.d(t, "NotificationsProvider", (function() {
-        return cN
+        return _N
     })), r.d(t, "Notification", (function() {
-        return dN
+        return AN
     })), r.d(t, "ScrollArea", (function() {
-        return mN
+        return $N
     })), r.d(t, "Header", (function() {
-        return VN
+        return gT
     })), r.d(t, "Navbar", (function() {
-        return ST
+        return ZT
     })), r.d(t, "InputWrapper", (function() {
-        return jT
+        return JT
     })), r.d(t, "ColorPicker", (function() {
-        return uI
+        return LI
     })), r.d(t, "MantineProvider", (function() {
-        return pI
+        return MI
     })), r.d(t, "NumberInput", (function() {
-        return zI
+        return eR
     })), r.d(t, "JsonInput", (function() {
-        return fR
+        return FR
     })), r.d(t, "ThemeIcon", (function() {
-        return IR
+        return o_
     })), r.d(t, "RingProgress", (function() {
-        return i_
+        return D_
     })), r.d(t, "TimeInput", (function() {
-        return d_
+        return A_
     })), r.d(t, "Loader", (function() {
-        return m_
+        return $_
     })), r.d(t, "LoadingOverlay", (function() {
-        return z_
+        return eL
     })), r.d(t, "Avatar", (function() {
-        return iL
+        return DL
     })), r.d(t, "AvatarsGroup", (function() {
-        return zL
+        return eA
     })), r.d(t, "Kbd", (function() {
-        return ML
+        return uA
     })), r.d(t, "Highlight", (function() {
-        return nA
+        return CA
     })), r.d(t, "Timeline", (function() {
-        return OA
+        return UA
     })), r.d(t, "TimelineItem", (function() {
-        return xA
+        return YA
     })), r.d(t, "Mark", (function() {
-        return EA
+        return XA
     })), r.d(t, "MediaQuery", (function() {
-        return NA
+        return rM
     })), r.d(t, "Menu", (function() {
-        return wM
+        return GM
     })), r.d(t, "MenuItem", (function() {
-        return kM
+        return KM
     })), r.d(t, "MenuLabel", (function() {
-        return jM
+        return JM
     })), r.d(t, "Code", (function() {
-        return qM
+        return yF
     })), r.d(t, "List", (function() {
-        return hF
+        return VF
     })), r.d(t, "ListItem", (function() {
-        return OF
+        return UF
     })), r.d(t, "BackgroundImage", (function() {
-        return IF
+        return o$
     })), r.d(t, "DemoSlider", (function() {
-        return _F
+        return l$
     })), r.d(t, "ActionIcon", (function() {
-        return MF
+        return u$
     })), r.d(t, "ThemeSwitcher", (function() {
-        return KF
+        return x$
+    })), r.d(t, "Stack", (function() {
+        return I$
+    })), r.d(t, "Pagination", (function() {
+        return MB
     }))
 }]);
 //# sourceMappingURL=dash_mantine_components.min.js.map
 //# sourceMappingURL=dash_mantine_components.min.js.map
```

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/metadata.json` & `dash_mantine_components-0.9.0/dash_mantine_components/metadata.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9614896114484932%*

 * *Differences: {"'src/lib/components/Group.react.js'": "{'props': {'children': {'description': 'Primary content "*

 * *                                        "inside the stack'}}}",*

 * * "'src/lib/components/Pagination.react.js'": "OrderedDict([('description', 'Display active page "*

 * *                                             'and navigate between multiple pages. For more '*

 * *                                             'information, see: '*

 * *                                             "https://mantine.dev/core/pagination/'), "*

 * *    […]*

```diff
@@ -6095,15 +6095,15 @@
                             "computed": false,
                             "value": "\"flex-start\""
                         }
                     ]
                 }
             },
             "children": {
-                "description": "Content",
+                "description": "Primary content inside the stack",
                 "required": false,
                 "type": {
                     "name": "node"
                 }
             },
             "class_name": {
                 "description": "Often used with CSS to style elements with common properties",
@@ -10669,14 +10669,348 @@
                             "value": "\"headless\""
                         }
                     ]
                 }
             }
         }
     },
+    "src/lib/components/Pagination.react.js": {
+        "description": "Display active page and navigate between multiple pages. For more information, see: https://mantine.dev/core/pagination/",
+        "displayName": "Pagination",
+        "methods": [],
+        "props": {
+            "align": {
+                "description": "Defines align-items css property",
+                "required": false,
+                "type": {
+                    "name": "enum",
+                    "value": [
+                        {
+                            "computed": false,
+                            "value": "\"stretch\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"center\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"flex-end\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"flex-start\""
+                        }
+                    ]
+                }
+            },
+            "boundaries": {
+                "description": "Amount of elements visible on left/right edges",
+                "required": false,
+                "type": {
+                    "name": "number"
+                }
+            },
+            "class_name": {
+                "description": "Often used with CSS to style elements with common properties",
+                "required": false,
+                "type": {
+                    "name": "string"
+                }
+            },
+            "color": {
+                "description": "Active item color from theme, defaults to theme.primaryColor",
+                "required": false,
+                "type": {
+                    "name": "enum",
+                    "value": [
+                        {
+                            "computed": false,
+                            "value": "\"dark\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"gray\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"red\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"pink\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"grape\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"violet\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"indigo\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"blue\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"cyan\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"teal\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"green\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"lime\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"yellow\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"orange\""
+                        }
+                    ]
+                }
+            },
+            "direction": {
+                "description": "Defines flex-direction property, row for horizontal, column for vertical",
+                "required": false,
+                "type": {
+                    "name": "enum",
+                    "value": [
+                        {
+                            "computed": false,
+                            "value": "\"row\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"column\""
+                        }
+                    ]
+                }
+            },
+            "grow": {
+                "description": "Defines flex-grow property for each element, true -> 1, false -> 0",
+                "required": false,
+                "type": {
+                    "name": "bool"
+                }
+            },
+            "id": {
+                "description": "The ID of this component, used to identify dash components in callbacks",
+                "required": false,
+                "type": {
+                    "name": "string"
+                }
+            },
+            "noWrap": {
+                "description": "Defined flex-wrap property",
+                "required": false,
+                "type": {
+                    "name": "bool"
+                }
+            },
+            "page": {
+                "description": "Controlled active page number",
+                "required": false,
+                "type": {
+                    "name": "number"
+                }
+            },
+            "position": {
+                "description": "Defines justify-content property",
+                "required": false,
+                "type": {
+                    "name": "enum",
+                    "value": [
+                        {
+                            "computed": false,
+                            "value": "\"right\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"center\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"left\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"apart\""
+                        }
+                    ]
+                }
+            },
+            "radius": {
+                "description": "Predefined item radius or number to set border-radius in px",
+                "required": false,
+                "type": {
+                    "name": "union",
+                    "value": [
+                        {
+                            "name": "enum",
+                            "value": [
+                                {
+                                    "computed": false,
+                                    "value": "\"xs\""
+                                },
+                                {
+                                    "computed": false,
+                                    "value": "\"sm\""
+                                },
+                                {
+                                    "computed": false,
+                                    "value": "\"md\""
+                                },
+                                {
+                                    "computed": false,
+                                    "value": "\"lg\""
+                                },
+                                {
+                                    "computed": false,
+                                    "value": "\"xl\""
+                                }
+                            ]
+                        },
+                        {
+                            "name": "number"
+                        }
+                    ]
+                }
+            },
+            "setProps": {
+                "description": "Tells dash if any prop has changed its value",
+                "required": false,
+                "type": {
+                    "name": "func"
+                }
+            },
+            "siblings": {
+                "description": "Siblings amount on left/right side of selected page",
+                "required": false,
+                "type": {
+                    "name": "number"
+                }
+            },
+            "size": {
+                "description": "Predefined item size or number to set width and height in px",
+                "required": false,
+                "type": {
+                    "name": "union",
+                    "value": [
+                        {
+                            "name": "enum",
+                            "value": [
+                                {
+                                    "computed": false,
+                                    "value": "\"xs\""
+                                },
+                                {
+                                    "computed": false,
+                                    "value": "\"sm\""
+                                },
+                                {
+                                    "computed": false,
+                                    "value": "\"md\""
+                                },
+                                {
+                                    "computed": false,
+                                    "value": "\"lg\""
+                                },
+                                {
+                                    "computed": false,
+                                    "value": "\"xl\""
+                                }
+                            ]
+                        },
+                        {
+                            "name": "number"
+                        }
+                    ]
+                }
+            },
+            "spacing": {
+                "description": "Spacing between items from theme or number to set value in px, defaults to theme.spacing.xs / 2",
+                "required": false,
+                "type": {
+                    "name": "union",
+                    "value": [
+                        {
+                            "name": "enum",
+                            "value": [
+                                {
+                                    "computed": false,
+                                    "value": "\"xs\""
+                                },
+                                {
+                                    "computed": false,
+                                    "value": "\"sm\""
+                                },
+                                {
+                                    "computed": false,
+                                    "value": "\"md\""
+                                },
+                                {
+                                    "computed": false,
+                                    "value": "\"lg\""
+                                },
+                                {
+                                    "computed": false,
+                                    "value": "\"xl\""
+                                }
+                            ]
+                        },
+                        {
+                            "name": "number"
+                        }
+                    ]
+                }
+            },
+            "style": {
+                "description": "Inline style",
+                "required": false,
+                "type": {
+                    "name": "object"
+                }
+            },
+            "total": {
+                "description": "Total amount of pages",
+                "required": true,
+                "type": {
+                    "name": "number"
+                }
+            },
+            "withControls": {
+                "description": "Show/hide prev/next controls",
+                "required": false,
+                "type": {
+                    "name": "bool"
+                }
+            },
+            "withEdges": {
+                "description": "Show/hide jump to start/end controls",
+                "required": false,
+                "type": {
+                    "name": "bool"
+                }
+            }
+        }
+    },
     "src/lib/components/Paper.react.js": {
         "description": "Renders white or dark background depending on color scheme. For more information, see: https://mantine.dev/core/paper/",
         "displayName": "Paper",
         "methods": [],
         "props": {
             "children": {
                 "description": "Paper content",
@@ -10987,14 +11321,258 @@
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             }
         }
     },
+    "src/lib/components/PasswordInput.react.js": {
+        "description": "Capture password from user with option to toggle visibility. For more information, see: https://mantine.dev/core/password-input/",
+        "displayName": "PasswordInput",
+        "methods": [],
+        "props": {
+            "class_name": {
+                "description": "Often used with CSS to style elements with common properties",
+                "required": false,
+                "type": {
+                    "name": "string"
+                }
+            },
+            "description": {
+                "description": "Input description, displayed after label",
+                "required": false,
+                "type": {
+                    "name": "any"
+                }
+            },
+            "disabled": {
+                "description": "The component can show it is currently unable to be interacted with",
+                "required": false,
+                "type": {
+                    "name": "bool"
+                }
+            },
+            "error": {
+                "description": "Displays error message after input",
+                "required": false,
+                "type": {
+                    "name": "any"
+                }
+            },
+            "icon": {
+                "description": "Adds icon on the left side of input",
+                "required": false,
+                "type": {
+                    "name": "any"
+                }
+            },
+            "iconWidth": {
+                "description": "Width of icon section in px",
+                "required": false,
+                "type": {
+                    "name": "number"
+                }
+            },
+            "id": {
+                "description": "The ID of this component, used to identify dash components in callbacks",
+                "required": false,
+                "type": {
+                    "name": "string"
+                }
+            },
+            "label": {
+                "description": "Input label, displayed before input",
+                "required": false,
+                "type": {
+                    "name": "any"
+                }
+            },
+            "placeholder": {
+                "description": "Placeholder, displayed when date is not selected",
+                "required": false,
+                "type": {
+                    "name": "string"
+                }
+            },
+            "radius": {
+                "description": "Input border-radius from theme or number to set border-radius in px",
+                "required": false,
+                "type": {
+                    "name": "union",
+                    "value": [
+                        {
+                            "name": "enum",
+                            "value": [
+                                {
+                                    "computed": false,
+                                    "value": "\"xs\""
+                                },
+                                {
+                                    "computed": false,
+                                    "value": "\"sm\""
+                                },
+                                {
+                                    "computed": false,
+                                    "value": "\"md\""
+                                },
+                                {
+                                    "computed": false,
+                                    "value": "\"lg\""
+                                },
+                                {
+                                    "computed": false,
+                                    "value": "\"xl\""
+                                }
+                            ]
+                        },
+                        {
+                            "name": "number"
+                        }
+                    ]
+                }
+            },
+            "required": {
+                "description": "Adds red asterisk on the right side of label",
+                "required": false,
+                "type": {
+                    "name": "bool"
+                }
+            },
+            "rightSection": {
+                "description": "Right section of input, similar to icon but on the right",
+                "required": false,
+                "type": {
+                    "name": "any"
+                }
+            },
+            "rightSectionWidth": {
+                "description": "Width of right section, is used to calculate input padding-right",
+                "required": false,
+                "type": {
+                    "name": "number"
+                }
+            },
+            "setProps": {
+                "description": "Tells dash if any prop has changed its value",
+                "required": false,
+                "type": {
+                    "name": "func"
+                }
+            },
+            "size": {
+                "description": "Input size",
+                "required": false,
+                "type": {
+                    "name": "enum",
+                    "value": [
+                        {
+                            "computed": false,
+                            "value": "\"xs\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"sm\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"md\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"lg\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"xl\""
+                        }
+                    ]
+                }
+            },
+            "style": {
+                "description": "Inline style override",
+                "required": false,
+                "type": {
+                    "name": "object"
+                }
+            },
+            "type": {
+                "description": "Input element type",
+                "required": false,
+                "type": {
+                    "name": "enum",
+                    "value": [
+                        {
+                            "computed": false,
+                            "value": "\"number\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"search\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"text\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"tel\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"url\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"email\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"password\""
+                        }
+                    ]
+                }
+            },
+            "value": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "\"\""
+                },
+                "description": "Input value",
+                "required": false,
+                "type": {
+                    "name": "node"
+                }
+            },
+            "variant": {
+                "description": "Defines input appearance, defaults to default in light color scheme and filled in dark",
+                "required": false,
+                "type": {
+                    "name": "enum",
+                    "value": [
+                        {
+                            "computed": false,
+                            "value": "\"default\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"filled\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"unstyled\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"headless\""
+                        }
+                    ]
+                }
+            }
+        }
+    },
     "src/lib/components/Prism.react.js": {
         "description": "Code highlight with Mantine theme colors and styles. For more information, see: https://mantine.dev/others/prism/",
         "displayName": "Prism",
         "methods": [],
         "props": {
             "children": {
                 "description": "Code which will be highlighted",
@@ -13870,14 +14448,133 @@
                 "required": false,
                 "type": {
                     "name": "number"
                 }
             }
         }
     },
+    "src/lib/components/Stack.react.js": {
+        "description": "Compose elements and components in vertical flex container. For more information, see: https://mantine.dev/core/Stack/",
+        "displayName": "Stack",
+        "methods": [],
+        "props": {
+            "align": {
+                "description": "Sets text-align css property",
+                "required": false,
+                "type": {
+                    "name": "enum",
+                    "value": [
+                        {
+                            "computed": false,
+                            "value": "\"stretch\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"center\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"flex-end\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"flex-start\""
+                        }
+                    ]
+                }
+            },
+            "children": {
+                "description": "Primary content inside the stack",
+                "required": false,
+                "type": {
+                    "name": "node"
+                }
+            },
+            "class_name": {
+                "description": "Often used with CSS to style elements with common properties",
+                "required": false,
+                "type": {
+                    "name": "string"
+                }
+            },
+            "justify": {
+                "description": "Set grid justify-content property",
+                "required": false,
+                "type": {
+                    "name": "enum",
+                    "value": [
+                        {
+                            "computed": false,
+                            "value": "\"space-between\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"space-around\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"center\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"flex-end\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"flex-start\""
+                        }
+                    ]
+                }
+            },
+            "spacing": {
+                "description": "Spacing between children",
+                "required": false,
+                "type": {
+                    "name": "union",
+                    "value": [
+                        {
+                            "name": "enum",
+                            "value": [
+                                {
+                                    "computed": false,
+                                    "value": "\"xs\""
+                                },
+                                {
+                                    "computed": false,
+                                    "value": "\"sm\""
+                                },
+                                {
+                                    "computed": false,
+                                    "value": "\"md\""
+                                },
+                                {
+                                    "computed": false,
+                                    "value": "\"lg\""
+                                },
+                                {
+                                    "computed": false,
+                                    "value": "\"xl\""
+                                }
+                            ]
+                        },
+                        {
+                            "name": "number"
+                        }
+                    ]
+                }
+            },
+            "style": {
+                "description": "Inline style",
+                "required": false,
+                "type": {
+                    "name": "object"
+                }
+            }
+        }
+    },
     "src/lib/components/Switch.react.js": {
         "description": "Capture user feedback limited to small set of options. For more information, see: https://mantine.dev/core/switch/",
         "displayName": "Switch",
         "methods": [],
         "props": {
             "checked": {
                 "defaultValue": {
@@ -15095,14 +15792,51 @@
             "style": {
                 "description": "Inline style override",
                 "required": false,
                 "type": {
                     "name": "object"
                 }
             },
+            "type": {
+                "description": "Input element type",
+                "required": false,
+                "type": {
+                    "name": "enum",
+                    "value": [
+                        {
+                            "computed": false,
+                            "value": "\"number\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"search\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"text\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"tel\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"url\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"email\""
+                        },
+                        {
+                            "computed": false,
+                            "value": "\"password\""
+                        }
+                    ]
+                }
+            },
             "value": {
                 "defaultValue": {
                     "computed": false,
                     "value": "\"\""
                 },
                 "description": "Input value",
                 "required": false,
```

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/package-info.json` & `dash_mantine_components-0.9.0/dash_mantine_components/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.9.0'"}*

```diff
@@ -60,9 +60,9 @@
         "build:backends": "dash-generate-components ./src/lib/components dash_mantine_components -p package-info.json --r-prefix '' --jl-prefix ''",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack-serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.8.0"
+    "version": "0.9.0"
 }
```

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components/theme/default_colors.py` & `dash_mantine_components-0.9.0/dash_mantine_components/theme/default_colors.py`

 * *Files identical despite different names*

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components.egg-info/PKG-INFO` & `dash_mantine_components-0.9.0/dash_mantine_components.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-mantine-components
-Version: 0.8.0
+Version: 0.9.0
 Summary: Plotly Dash components based on Mantine
 Home-page: https://github.com/snehilvj/dash-mantine-components
 Author: Snehil Vijay <snehilvj@outlook.com>
 Author-email: snehilvj@outlook.com
 License: MIT
 Description: <p align="center">
             <img src="https://raw.githubusercontent.com/snehilvj/dash-mantine-components/master/assets/logo.png" alt="logo" width=300 >
```

### Comparing `dash_mantine_components-0.8.0/dash_mantine_components.egg-info/SOURCES.txt` & `dash_mantine_components-0.9.0/dash_mantine_components.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -48,27 +48,30 @@
 dash_mantine_components/MenuLabel.py
 dash_mantine_components/Modal.py
 dash_mantine_components/MultiSelect.py
 dash_mantine_components/Navbar.py
 dash_mantine_components/Notification.py
 dash_mantine_components/NotificationsProvider.py
 dash_mantine_components/NumberInput.py
+dash_mantine_components/Pagination.py
 dash_mantine_components/Paper.py
+dash_mantine_components/PasswordInput.py
 dash_mantine_components/Prism.py
 dash_mantine_components/Progress.py
 dash_mantine_components/RadioGroup.py
 dash_mantine_components/RingProgress.py
 dash_mantine_components/ScrollArea.py
 dash_mantine_components/SegmentedControl.py
 dash_mantine_components/Select.py
 dash_mantine_components/SimpleGrid.py
 dash_mantine_components/Skeleton.py
 dash_mantine_components/Slider.py
 dash_mantine_components/Space.py
 dash_mantine_components/Spoiler.py
+dash_mantine_components/Stack.py
 dash_mantine_components/Switch.py
 dash_mantine_components/Tab.py
 dash_mantine_components/Table.py
 dash_mantine_components/Tabs.py
 dash_mantine_components/Text.py
 dash_mantine_components/TextInput.py
 dash_mantine_components/ThemeIcon.py
```

### Comparing `dash_mantine_components-0.8.0/package.json` & `dash_mantine_components-0.9.0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.9.0'"}*

```diff
@@ -60,9 +60,9 @@
         "build:backends": "dash-generate-components ./src/lib/components dash_mantine_components -p package-info.json --r-prefix '' --jl-prefix ''",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack-serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.8.0"
+    "version": "0.9.0"
 }
```

### Comparing `dash_mantine_components-0.8.0/setup.py` & `dash_mantine_components-0.9.0/setup.py`

 * *Files identical despite different names*

