# Comparing `tmp/apprise-1.7.5.tar.gz` & `tmp/apprise-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apprise-1.7.5.tar", last modified: Sat Mar 30 13:59:27 2024, max compression
+gzip compressed data, was "apprise-1.7.6.tar", last modified: Sun Apr 14 00:12:19 2024, max compression
```

## Comparing `apprise-1.7.5.tar` & `apprise-1.7.6.tar`

### file list

```diff
@@ -1,358 +1,360 @@
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-03-30 13:59:27.512027 apprise-1.7.5/
--rw-r--r--   0 l2g       (1000) l2g       (1000)      931 2024-03-30 13:53:24.000000 apprise-1.7.5/KEYWORDS
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1343 2024-01-27 20:33:15.000000 apprise-1.7.5/LICENSE
--rw-r--r--   0 l2g       (1000) l2g       (1000)      237 2023-06-03 19:32:05.000000 apprise-1.7.5/MANIFEST.in
--rw-r--r--   0 l2g       (1000) l2g       (1000)    44446 2024-03-30 13:59:27.513028 apprise-1.7.5/PKG-INFO
--rw-r--r--   0 l2g       (1000) l2g       (1000)    42205 2024-03-30 13:53:24.000000 apprise-1.7.5/README.md
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-03-30 13:59:27.470027 apprise-1.7.5/apprise/
--rw-r--r--   0 l2g       (1000) l2g       (1000)    32865 2024-03-30 01:23:37.000000 apprise-1.7.5/apprise/Apprise.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2203 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/Apprise.pyi
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11647 2024-01-27 20:32:17.000000 apprise-1.7.5/apprise/AppriseAsset.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)      979 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/AppriseAsset.pyi
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12540 2024-01-27 20:32:17.000000 apprise-1.7.5/apprise/AppriseAttachment.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1145 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/AppriseAttachment.pyi
--rw-r--r--   0 l2g       (1000) l2g       (1000)    16909 2024-01-27 20:12:32.000000 apprise-1.7.5/apprise/AppriseConfig.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1568 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/AppriseConfig.pyi
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8852 2024-01-27 20:12:32.000000 apprise-1.7.5/apprise/AppriseLocale.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2053 2024-01-27 20:12:32.000000 apprise-1.7.5/apprise/AttachmentManager.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2058 2024-01-27 20:12:32.000000 apprise-1.7.5/apprise/ConfigurationManager.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2041 2024-01-27 20:12:32.000000 apprise-1.7.5/apprise/NotificationManager.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    29423 2024-03-29 20:20:13.000000 apprise-1.7.5/apprise/URLBase.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)      520 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/URLBase.pyi
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3368 2024-03-30 13:58:10.000000 apprise-1.7.5/apprise/__init__.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-03-30 13:59:27.472027 apprise-1.7.5/apprise/assets/
--rw-r--r--   0 l2g       (1000) l2g       (1000)      986 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/assets/NotifyXML-1.0.xsd
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1758 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/assets/NotifyXML-1.1.xsd
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-03-30 13:59:27.454027 apprise-1.7.5/apprise/assets/themes/
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-03-30 13:59:27.477027 apprise-1.7.5/apprise/assets/themes/default/
--rw-r--r--   0 l2g       (1000) l2g       (1000)    67646 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/assets/themes/default/apprise-failure-128x128.ico
--rw-r--r--   0 l2g       (1000) l2g       (1000)    16135 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/assets/themes/default/apprise-failure-128x128.png
--rw-r--r--   0 l2g       (1000) l2g       (1000)    41931 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/assets/themes/default/apprise-failure-256x256.png
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2437 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/assets/themes/default/apprise-failure-32x32.png
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7600 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/assets/themes/default/apprise-failure-72x72.png
--rw-r--r--   0 l2g       (1000) l2g       (1000)    67646 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/assets/themes/default/apprise-info-128x128.ico
--rw-r--r--   0 l2g       (1000) l2g       (1000)    16671 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/assets/themes/default/apprise-info-128x128.png
--rw-r--r--   0 l2g       (1000) l2g       (1000)    43331 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/assets/themes/default/apprise-info-256x256.png
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2485 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/assets/themes/default/apprise-info-32x32.png
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7875 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/assets/themes/default/apprise-info-72x72.png
--rw-r--r--   0 l2g       (1000) l2g       (1000)   160907 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/assets/themes/default/apprise-logo.png
--rw-r--r--   0 l2g       (1000) l2g       (1000)    67646 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/assets/themes/default/apprise-success-128x128.ico
--rw-r--r--   0 l2g       (1000) l2g       (1000)    17446 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/assets/themes/default/apprise-success-128x128.png
--rw-r--r--   0 l2g       (1000) l2g       (1000)    48729 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/assets/themes/default/apprise-success-256x256.png
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2471 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/assets/themes/default/apprise-success-32x32.png
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7858 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/assets/themes/default/apprise-success-72x72.png
--rw-r--r--   0 l2g       (1000) l2g       (1000)    67646 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/assets/themes/default/apprise-warning-128x128.ico
--rw-r--r--   0 l2g       (1000) l2g       (1000)    16784 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/assets/themes/default/apprise-warning-128x128.png
--rw-r--r--   0 l2g       (1000) l2g       (1000)    43708 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/assets/themes/default/apprise-warning-256x256.png
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2472 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/assets/themes/default/apprise-warning-32x32.png
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7913 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/assets/themes/default/apprise-warning-72x72.png
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-03-30 13:59:27.478027 apprise-1.7.5/apprise/attachment/
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13656 2024-03-29 19:00:10.000000 apprise-1.7.5/apprise/attachment/AttachBase.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)      961 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/attachment/AttachBase.pyi
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4765 2024-03-12 22:02:34.000000 apprise-1.7.5/apprise/attachment/AttachFile.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13779 2024-03-29 19:00:10.000000 apprise-1.7.5/apprise/attachment/AttachHTTP.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1658 2024-01-27 20:32:17.000000 apprise-1.7.5/apprise/attachment/__init__.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    20697 2024-03-09 21:39:52.000000 apprise-1.7.5/apprise/cli.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5593 2024-01-27 20:32:17.000000 apprise-1.7.5/apprise/common.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)      447 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/common.pyi
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-03-30 13:59:27.479027 apprise-1.7.5/apprise/config/
--rw-r--r--   0 l2g       (1000) l2g       (1000)    53194 2024-03-29 20:20:13.000000 apprise-1.7.5/apprise/config/ConfigBase.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)       54 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/config/ConfigBase.pyi
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6138 2024-01-27 20:32:17.000000 apprise-1.7.5/apprise/config/ConfigFile.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9457 2024-01-27 20:32:17.000000 apprise-1.7.5/apprise/config/ConfigHTTP.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2829 2024-01-27 20:32:17.000000 apprise-1.7.5/apprise/config/ConfigMemory.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1663 2024-01-27 20:32:17.000000 apprise-1.7.5/apprise/config/__init__.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6228 2024-03-30 13:53:24.000000 apprise-1.7.5/apprise/conversion.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-03-30 13:59:27.479027 apprise-1.7.5/apprise/decorators/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7972 2024-03-29 20:20:13.000000 apprise-1.7.5/apprise/decorators/CustomNotifyPlugin.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1487 2024-01-27 20:12:32.000000 apprise-1.7.5/apprise/decorators/__init__.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5111 2024-01-27 20:12:32.000000 apprise-1.7.5/apprise/decorators/notify.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    87738 2024-01-27 20:12:32.000000 apprise-1.7.5/apprise/emojis.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-03-30 13:59:27.479027 apprise-1.7.5/apprise/i18n/
--rw-r--r--   0 l2g       (1000) l2g       (1000)        0 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/i18n/__init__.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-03-30 13:59:27.455027 apprise-1.7.5/apprise/i18n/en/
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-03-30 13:59:27.479027 apprise-1.7.5/apprise/i18n/en/LC_MESSAGES/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3959 2024-03-30 13:59:27.000000 apprise-1.7.5/apprise/i18n/en/LC_MESSAGES/apprise.mo
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6921 2024-01-27 20:32:17.000000 apprise-1.7.5/apprise/logger.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    26857 2024-03-09 21:39:49.000000 apprise-1.7.5/apprise/manager.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-03-30 13:59:27.494027 apprise-1.7.5/apprise/plugins/
--rw-r--r--   0 l2g       (1000) l2g       (1000)    16654 2024-03-12 22:16:02.000000 apprise-1.7.5/apprise/plugins/NotifyAppriseAPI.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    24220 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyAprs.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    15698 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyBark.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    29716 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyBase.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)       21 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/plugins/NotifyBase.pyi
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12867 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyBoxcar.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    16005 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyBulkSMS.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13290 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyBulkVS.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    15550 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyBurstSMS.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11229 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyClickSend.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    15043 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyD7Networks.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14379 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyDBus.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13624 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyDapnet.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12009 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyDingTalk.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    26072 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyDiscord.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    38883 2024-03-03 14:39:10.000000 apprise-1.7.5/apprise/plugins/NotifyEmail.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    24039 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyEmby.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11498 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyEnigma2.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-03-30 13:59:27.494027 apprise-1.7.5/apprise/plugins/NotifyFCM/
--rw-r--r--   0 l2g       (1000) l2g       (1000)    21669 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyFCM/__init__.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4592 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyFCM/color.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1718 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyFCM/common.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11197 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyFCM/oauth.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8163 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyFCM/priority.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6972 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyFaast.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12748 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyFlock.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    17905 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyForm.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6679 2024-03-30 13:53:24.000000 apprise-1.7.5/apprise/plugins/NotifyFreeMobile.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9059 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyGnome.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12622 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyGoogleChat.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    10551 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyGotify.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14023 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyGrowl.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3641 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyGuilded.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    10739 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyHomeAssistant.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11136 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyHttpSMS.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13425 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyIFTTT.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13851 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyJSON.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13581 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyJoin.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12620 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyKavenegar.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8214 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyKumulos.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    37534 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyLametric.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    10676 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyLine.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14459 2024-03-09 21:39:52.000000 apprise-1.7.5/apprise/plugins/NotifyLunaSea.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    19546 2024-03-30 13:52:48.000000 apprise-1.7.5/apprise/plugins/NotifyMQTT.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12677 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyMSG91.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    22976 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyMSTeams.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8271 2024-02-03 17:43:14.000000 apprise-1.7.5/apprise/plugins/NotifyMacOSX.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    25409 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyMailgun.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    35277 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyMastodon.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    50049 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyMatrix.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12722 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyMattermost.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12248 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyMessageBird.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9600 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyMisskey.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12759 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyNextcloud.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11011 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyNextcloudTalk.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12990 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyNotica.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    15857 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyNotifiarr.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12035 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyNotifico.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    27953 2024-03-03 22:45:59.000000 apprise-1.7.5/apprise/plugins/NotifyNtfy.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    25190 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyOffice365.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    18153 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyOneSignal.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    20515 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyOpsgenie.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    17874 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyPagerDuty.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13849 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyPagerTree.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    10291 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyParsePlatform.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    10587 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyPopcornNotify.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9782 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyProwl.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    15372 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyPushBullet.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6922 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyPushDeer.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7134 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyPushMe.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    26756 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyPushSafer.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12270 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyPushed.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8952 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyPushjet.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    21213 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyPushover.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12496 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyPushy.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11982 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyRSyslog.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    25785 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyReddit.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14500 2024-02-18 15:11:50.000000 apprise-1.7.5/apprise/plugins/NotifyRevolt.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    24624 2024-02-17 16:42:21.000000 apprise-1.7.5/apprise/plugins/NotifyRocketChat.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11823 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyRyver.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    33545 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifySES.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    24161 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifySMSEagle.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14125 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifySMSManager.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    19711 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifySMTP2Go.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    24159 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifySNS.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    16213 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifySendGrid.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5779 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyServerChan.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    16733 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifySignalAPI.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    10876 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifySimplePush.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    16813 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifySinch.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    42521 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifySlack.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    27878 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifySparkPost.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    16023 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyStreamlabs.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11105 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifySynology.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    10617 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifySyslog.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7253 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyTechulusPush.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    35624 2024-02-18 15:11:50.000000 apprise-1.7.5/apprise/plugins/NotifyTelegram.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11885 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyThreema.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    15976 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyTwilio.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    28841 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyTwist.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    30152 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyTwitter.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12552 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyVoipms.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13431 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyVonage.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8789 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyWeComBot.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9164 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyWebexTeams.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    19924 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyWhatsApp.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8563 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyWindows.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12096 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyXBMC.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    16973 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyXML.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13755 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/NotifyZulip.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    18725 2024-01-27 20:31:31.000000 apprise-1.7.5/apprise/plugins/__init__.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)        0 2023-06-03 19:32:05.000000 apprise-1.7.5/apprise/py.typed
--rw-r--r--   0 l2g       (1000) l2g       (1000)    53185 2024-01-27 20:12:32.000000 apprise-1.7.5/apprise/utils.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-03-30 13:59:27.472027 apprise-1.7.5/apprise.egg-info/
--rw-r--r--   0 l2g       (1000) l2g       (1000)    44446 2024-03-30 13:59:27.000000 apprise-1.7.5/apprise.egg-info/PKG-INFO
--rw-r--r--   0 l2g       (1000) l2g       (1000)    10444 2024-03-30 13:59:27.000000 apprise-1.7.5/apprise.egg-info/SOURCES.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)        1 2024-03-30 13:59:27.000000 apprise-1.7.5/apprise.egg-info/dependency_links.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)       45 2024-03-30 13:59:27.000000 apprise-1.7.5/apprise.egg-info/entry_points.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)      101 2024-03-30 13:59:27.000000 apprise-1.7.5/apprise.egg-info/requires.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)        8 2024-03-30 13:59:27.000000 apprise-1.7.5/apprise.egg-info/top_level.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)       65 2023-08-20 16:57:52.000000 apprise-1.7.5/dev-requirements.txt
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-03-30 13:59:27.494027 apprise-1.7.5/packaging/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1281 2023-06-03 19:32:05.000000 apprise-1.7.5/packaging/README.md
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-03-30 13:59:27.495027 apprise-1.7.5/packaging/man/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9039 2024-03-30 13:59:07.000000 apprise-1.7.5/packaging/man/apprise.1
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13374 2024-03-30 13:59:07.000000 apprise-1.7.5/packaging/man/apprise.1.html
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8164 2024-03-09 21:39:52.000000 apprise-1.7.5/packaging/man/apprise.md
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-03-30 13:59:27.497027 apprise-1.7.5/packaging/redhat/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1586 2024-01-27 20:41:30.000000 apprise-1.7.5/packaging/redhat/apprise-click67-support.patch
--rw-r--r--   0 l2g       (1000) l2g       (1000)      596 2024-01-27 20:41:32.000000 apprise-1.7.5/packaging/redhat/apprise-no-macosx-testing.patch
--rw-r--r--   0 l2g       (1000) l2g       (1000)      785 2024-01-27 20:41:35.000000 apprise-1.7.5/packaging/redhat/apprise-pytest-session_mocker-removal.patch
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14088 2024-03-30 13:58:49.000000 apprise-1.7.5/packaging/redhat/python-apprise.spec
--rw-r--r--   0 l2g       (1000) l2g       (1000)      164 2023-06-03 19:32:05.000000 apprise-1.7.5/requirements.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)      861 2024-03-30 13:59:27.513028 apprise-1.7.5/setup.cfg
--rwxr-xr-x   0 l2g       (1000) l2g       (1000)     4337 2024-03-30 13:57:52.000000 apprise-1.7.5/setup.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-03-30 13:59:27.511027 apprise-1.7.5/test/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2422 2024-01-27 20:33:15.000000 apprise-1.7.5/test/conftest.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-03-30 13:59:27.511027 apprise-1.7.5/test/helpers/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1618 2024-01-27 20:33:15.000000 apprise-1.7.5/test/helpers/__init__.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1668 2023-08-20 03:33:33.000000 apprise-1.7.5/test/helpers/asyncio.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4924 2024-01-27 20:33:15.000000 apprise-1.7.5/test/helpers/module.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    22600 2024-01-27 20:33:15.000000 apprise-1.7.5/test/helpers/rest.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    68127 2024-02-21 00:38:56.000000 apprise-1.7.5/test/test_api.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    10886 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_apprise_attachments.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    40246 2024-03-09 21:39:49.000000 apprise-1.7.5/test/test_apprise_cli.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    40843 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_apprise_config.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2248 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_apprise_emojis.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3617 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_apprise_pickle.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13983 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_apprise_translations.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    96705 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_apprise_utils.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3693 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_asyncio.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3372 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_attach_base.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8491 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_attach_file.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    17522 2024-03-29 19:00:10.000000 apprise-1.7.5/test/test_attach_http.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    42141 2024-03-30 13:53:24.000000 apprise-1.7.5/test/test_config_base.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4112 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_config_file.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    10868 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_config_http.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2358 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_config_memory.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6698 2024-03-30 13:53:24.000000 apprise-1.7.5/test/test_conversion.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    15813 2024-03-29 20:20:13.000000 apprise-1.7.5/test/test_decorator_notify.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7557 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_escapes.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14361 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_logger.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13614 2024-03-03 19:41:00.000000 apprise-1.7.5/test/test_notification_manager.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12929 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_notify_base.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9896 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_apprise_api.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12325 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_aprs.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5274 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_bark.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6614 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_boxcar.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7285 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_bulksms.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6274 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_bulkvs.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6266 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_burstsms.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3358 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_clicksend.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    15681 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_custom_form.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11633 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_custom_json.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13640 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_custom_xml.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7486 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_d7networks.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8034 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_dapnet.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3980 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_dingtalk.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    27507 2024-02-18 15:11:50.000000 apprise-1.7.5/test/test_plugin_discord.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    64634 2024-03-29 20:20:13.000000 apprise-1.7.5/test/test_plugin_email.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14521 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_emby.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6088 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_enigma2.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2978 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_faast.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    31323 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_fcm.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6308 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_flock.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2918 2024-03-30 13:53:24.000000 apprise-1.7.5/test/test_plugin_freemobile.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    17424 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_glib.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12170 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_gnome.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6321 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_google_chat.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6415 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_gotify.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12690 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_growl.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6570 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_guilded.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5233 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_homeassistant.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5689 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_httpsms.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6761 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_ifttt.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7448 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_join.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4226 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_kavenegar.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4063 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_kumulos.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9782 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_lametric.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3355 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_line.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    10004 2024-03-09 21:39:52.000000 apprise-1.7.5/test/test_plugin_lunasea.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7654 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_macosx.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14672 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_mailgun.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    25055 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_mastodon.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    38833 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_matrix.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4940 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_mattermost.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4575 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_messagebird.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3813 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_misskey.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14198 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_mqtt.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7272 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_msg91.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    23826 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_msteams.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7226 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_nextcloud.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6868 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_nextcloudtalk.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5079 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_notica.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6146 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_notifiarr.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4376 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_notifico.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    20084 2024-02-17 16:42:25.000000 apprise-1.7.5/test/test_plugin_ntfy.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12395 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_office365.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7949 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_onesignal.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7439 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_opsgenie.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4943 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_pagerduty.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4871 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_pagertree.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3750 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_parse_platform.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3619 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_popcorn_notify.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6632 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_prowl.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13080 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_pushbullet.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4230 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_pushdeer.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7236 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_pushed.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3781 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_pushjet.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3726 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_pushme.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    15398 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_pushover.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9043 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_pushsafer.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5531 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_pushy.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14553 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_reddit.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    17404 2024-02-18 15:11:50.000000 apprise-1.7.5/test/test_plugin_revolt.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11198 2024-02-17 16:42:21.000000 apprise-1.7.5/test/test_plugin_rocket_chat.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6913 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_rsyslog.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5067 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_ryver.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5497 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_sendgrid.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2710 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_serverchan.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14643 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_ses.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13355 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_signal.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5695 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_simplepush.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6246 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_sinch.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    26717 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_slack.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6373 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_sms_manager.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    25558 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_smseagle.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8764 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_smtp2go.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14294 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_sns.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14172 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_sparkpost.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5036 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_streamlabs.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5820 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_synology.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5021 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_syslog.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3061 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_techululs_push.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    35158 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_telegram.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5975 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_threema.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4831 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_title_maxlen.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8253 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_twilio.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    16766 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_twist.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    35721 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_twitter.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7584 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_voipms.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7918 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_vonage.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3970 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_webex_teams.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3167 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_wecombot.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9129 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_whatsapp.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    10786 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_windows.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6495 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_xbmc_kodi.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4755 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_plugin_zulip.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)   140538 2024-01-27 20:33:15.000000 apprise-1.7.5/test/test_rest_plugins.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-03-30 13:59:27.512027 apprise-1.7.5/test/var/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1913 2023-06-03 19:32:05.000000 apprise-1.7.5/test/var/01_test_example.html
--rw-r--r--   0 l2g       (1000) l2g       (1000)      277 2023-06-03 19:32:05.000000 apprise-1.7.5/test/var/apprise-archive.zip
--rw-r--r--   0 l2g       (1000) l2g       (1000)    76646 2023-06-03 19:32:05.000000 apprise-1.7.5/test/var/apprise-test.gif
--rw-r--r--   0 l2g       (1000) l2g       (1000)    73667 2023-06-03 19:32:05.000000 apprise-1.7.5/test/var/apprise-test.jpeg
--rw-r--r--   0 l2g       (1000) l2g       (1000)    17856 2023-06-03 19:32:05.000000 apprise-1.7.5/test/var/apprise-test.mp4
--rw-r--r--   0 l2g       (1000) l2g       (1000)   248280 2023-06-03 19:32:05.000000 apprise-1.7.5/test/var/apprise-test.png
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-03-30 13:59:27.512027 apprise-1.7.5/test/var/fcm/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2231 2023-06-03 19:32:05.000000 apprise-1.7.5/test/var/fcm/service_account-bad-type.json
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2238 2023-06-03 19:32:05.000000 apprise-1.7.5/test/var/fcm/service_account.json
--rw-r--r--   0 l2g       (1000) l2g       (1000)        8 2023-06-03 19:32:05.000000 apprise-1.7.5/win-requirements.txt
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-04-14 00:12:19.107314 apprise-1.7.6/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      941 2024-04-10 23:44:32.000000 apprise-1.7.6/KEYWORDS
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1343 2024-01-27 20:33:15.000000 apprise-1.7.6/LICENSE
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      237 2023-06-03 19:32:05.000000 apprise-1.7.6/MANIFEST.in
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    44618 2024-04-14 00:12:19.107314 apprise-1.7.6/PKG-INFO
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    42316 2024-04-10 23:44:32.000000 apprise-1.7.6/README.md
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-04-14 00:12:19.068314 apprise-1.7.6/apprise/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    32865 2024-03-30 01:23:37.000000 apprise-1.7.6/apprise/Apprise.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2203 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/Apprise.pyi
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11647 2024-01-27 20:32:17.000000 apprise-1.7.6/apprise/AppriseAsset.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      979 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/AppriseAsset.pyi
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12540 2024-01-27 20:32:17.000000 apprise-1.7.6/apprise/AppriseAttachment.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1145 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/AppriseAttachment.pyi
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16909 2024-01-27 20:12:32.000000 apprise-1.7.6/apprise/AppriseConfig.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1568 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/AppriseConfig.pyi
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8994 2024-04-11 01:21:34.000000 apprise-1.7.6/apprise/AppriseLocale.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2053 2024-01-27 20:12:32.000000 apprise-1.7.6/apprise/AttachmentManager.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2058 2024-01-27 20:12:32.000000 apprise-1.7.6/apprise/ConfigurationManager.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2041 2024-01-27 20:12:32.000000 apprise-1.7.6/apprise/NotificationManager.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    29423 2024-03-29 20:20:13.000000 apprise-1.7.6/apprise/URLBase.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      520 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/URLBase.pyi
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3368 2024-04-14 00:10:26.000000 apprise-1.7.6/apprise/__init__.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-04-14 00:12:19.069314 apprise-1.7.6/apprise/assets/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      986 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/assets/NotifyXML-1.0.xsd
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1758 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/assets/NotifyXML-1.1.xsd
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-04-14 00:12:19.062314 apprise-1.7.6/apprise/assets/themes/
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-04-14 00:12:19.072314 apprise-1.7.6/apprise/assets/themes/default/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    67646 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/assets/themes/default/apprise-failure-128x128.ico
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16135 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/assets/themes/default/apprise-failure-128x128.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    41931 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/assets/themes/default/apprise-failure-256x256.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2437 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/assets/themes/default/apprise-failure-32x32.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7600 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/assets/themes/default/apprise-failure-72x72.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    67646 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/assets/themes/default/apprise-info-128x128.ico
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16671 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/assets/themes/default/apprise-info-128x128.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    43331 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/assets/themes/default/apprise-info-256x256.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2485 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/assets/themes/default/apprise-info-32x32.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7875 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/assets/themes/default/apprise-info-72x72.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)   160907 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/assets/themes/default/apprise-logo.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    67646 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/assets/themes/default/apprise-success-128x128.ico
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    17446 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/assets/themes/default/apprise-success-128x128.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    48729 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/assets/themes/default/apprise-success-256x256.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2471 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/assets/themes/default/apprise-success-32x32.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7858 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/assets/themes/default/apprise-success-72x72.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    67646 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/assets/themes/default/apprise-warning-128x128.ico
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16784 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/assets/themes/default/apprise-warning-128x128.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    43708 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/assets/themes/default/apprise-warning-256x256.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2472 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/assets/themes/default/apprise-warning-32x32.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7913 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/assets/themes/default/apprise-warning-72x72.png
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-04-14 00:12:19.072314 apprise-1.7.6/apprise/attachment/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13656 2024-03-29 19:00:10.000000 apprise-1.7.6/apprise/attachment/AttachBase.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      961 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/attachment/AttachBase.pyi
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4765 2024-03-12 22:02:34.000000 apprise-1.7.6/apprise/attachment/AttachFile.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13779 2024-03-29 19:00:10.000000 apprise-1.7.6/apprise/attachment/AttachHTTP.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1658 2024-01-27 20:32:17.000000 apprise-1.7.6/apprise/attachment/__init__.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    20697 2024-03-09 21:39:52.000000 apprise-1.7.6/apprise/cli.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5593 2024-01-27 20:32:17.000000 apprise-1.7.6/apprise/common.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      447 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/common.pyi
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-04-14 00:12:19.073314 apprise-1.7.6/apprise/config/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    53194 2024-03-29 20:20:13.000000 apprise-1.7.6/apprise/config/ConfigBase.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       54 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/config/ConfigBase.pyi
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6138 2024-01-27 20:32:17.000000 apprise-1.7.6/apprise/config/ConfigFile.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9457 2024-01-27 20:32:17.000000 apprise-1.7.6/apprise/config/ConfigHTTP.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2829 2024-01-27 20:32:17.000000 apprise-1.7.6/apprise/config/ConfigMemory.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1663 2024-01-27 20:32:17.000000 apprise-1.7.6/apprise/config/__init__.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6277 2024-04-13 23:33:39.000000 apprise-1.7.6/apprise/conversion.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-04-14 00:12:19.073314 apprise-1.7.6/apprise/decorators/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7972 2024-03-29 20:20:13.000000 apprise-1.7.6/apprise/decorators/CustomNotifyPlugin.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1487 2024-01-27 20:12:32.000000 apprise-1.7.6/apprise/decorators/__init__.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5111 2024-01-27 20:12:32.000000 apprise-1.7.6/apprise/decorators/notify.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    87738 2024-01-27 20:12:32.000000 apprise-1.7.6/apprise/emojis.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-04-14 00:12:19.073314 apprise-1.7.6/apprise/i18n/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)        0 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/i18n/__init__.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-04-14 00:12:19.063314 apprise-1.7.6/apprise/i18n/en/
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-04-14 00:12:19.073314 apprise-1.7.6/apprise/i18n/en/LC_MESSAGES/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3959 2024-04-14 00:12:18.000000 apprise-1.7.6/apprise/i18n/en/LC_MESSAGES/apprise.mo
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6921 2024-01-27 20:32:17.000000 apprise-1.7.6/apprise/logger.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    26857 2024-03-09 21:39:49.000000 apprise-1.7.6/apprise/manager.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-04-14 00:12:19.087314 apprise-1.7.6/apprise/plugins/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16654 2024-03-12 22:16:02.000000 apprise-1.7.6/apprise/plugins/NotifyAppriseAPI.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    25523 2024-04-13 23:33:39.000000 apprise-1.7.6/apprise/plugins/NotifyAprs.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    15698 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyBark.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    30360 2024-04-09 00:19:20.000000 apprise-1.7.6/apprise/plugins/NotifyBase.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       21 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/plugins/NotifyBase.pyi
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12867 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyBoxcar.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16005 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyBulkSMS.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13290 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyBulkVS.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    15550 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyBurstSMS.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6673 2024-04-09 01:04:23.000000 apprise-1.7.6/apprise/plugins/NotifyChantify.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11229 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyClickSend.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    15043 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyD7Networks.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14379 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyDBus.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13624 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyDapnet.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12009 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyDingTalk.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    26072 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyDiscord.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    39789 2024-04-09 00:19:20.000000 apprise-1.7.6/apprise/plugins/NotifyEmail.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    24039 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyEmby.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11498 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyEnigma2.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-04-14 00:12:19.088314 apprise-1.7.6/apprise/plugins/NotifyFCM/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    21669 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyFCM/__init__.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4592 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyFCM/color.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1718 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyFCM/common.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11197 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyFCM/oauth.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8163 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyFCM/priority.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7266 2024-04-10 23:44:32.000000 apprise-1.7.6/apprise/plugins/NotifyFeishu.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12748 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyFlock.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    17905 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyForm.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6644 2024-04-13 23:33:39.000000 apprise-1.7.6/apprise/plugins/NotifyFreeMobile.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9059 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyGnome.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12622 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyGoogleChat.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    10551 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyGotify.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14023 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyGrowl.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3641 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyGuilded.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    10739 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyHomeAssistant.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11136 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyHttpSMS.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13425 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyIFTTT.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13851 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyJSON.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13581 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyJoin.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12620 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyKavenegar.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8214 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyKumulos.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    37534 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyLametric.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    10676 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyLine.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14459 2024-03-09 21:39:52.000000 apprise-1.7.6/apprise/plugins/NotifyLunaSea.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    19545 2024-03-30 16:22:13.000000 apprise-1.7.6/apprise/plugins/NotifyMQTT.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12677 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyMSG91.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    22976 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyMSTeams.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8271 2024-02-03 17:43:14.000000 apprise-1.7.6/apprise/plugins/NotifyMacOSX.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    25409 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyMailgun.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    35277 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyMastodon.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    50049 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyMatrix.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12722 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyMattermost.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12248 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyMessageBird.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9600 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyMisskey.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12759 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyNextcloud.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11011 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyNextcloudTalk.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12990 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyNotica.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    15857 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyNotifiarr.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12035 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyNotifico.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    27979 2024-04-07 16:07:14.000000 apprise-1.7.6/apprise/plugins/NotifyNtfy.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    25190 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyOffice365.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    18153 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyOneSignal.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    20515 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyOpsgenie.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    17874 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyPagerDuty.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13849 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyPagerTree.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    10291 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyParsePlatform.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    10587 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyPopcornNotify.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9782 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyProwl.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    15372 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyPushBullet.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6922 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyPushDeer.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7134 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyPushMe.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    26756 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyPushSafer.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12270 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyPushed.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8952 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyPushjet.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    21213 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyPushover.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12496 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyPushy.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11982 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyRSyslog.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    25785 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyReddit.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14500 2024-02-18 15:11:50.000000 apprise-1.7.6/apprise/plugins/NotifyRevolt.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    25738 2024-04-14 00:09:29.000000 apprise-1.7.6/apprise/plugins/NotifyRocketChat.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11823 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyRyver.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    33545 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifySES.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    24161 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifySMSEagle.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14125 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifySMSManager.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    19711 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifySMTP2Go.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    24159 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifySNS.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16213 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifySendGrid.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5779 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyServerChan.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16733 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifySignalAPI.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    10876 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifySimplePush.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16813 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifySinch.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    42521 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifySlack.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    27878 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifySparkPost.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16023 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyStreamlabs.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11105 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifySynology.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    10617 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifySyslog.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7253 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyTechulusPush.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    37187 2024-04-11 01:21:34.000000 apprise-1.7.6/apprise/plugins/NotifyTelegram.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11885 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyThreema.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    15976 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyTwilio.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    28841 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyTwist.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    30152 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyTwitter.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12552 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyVoipms.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13431 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyVonage.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8789 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyWeComBot.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9164 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyWebexTeams.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    19924 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyWhatsApp.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8563 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyWindows.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12096 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyXBMC.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16973 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/NotifyXML.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13968 2024-04-09 01:01:29.000000 apprise-1.7.6/apprise/plugins/NotifyZulip.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    18725 2024-01-27 20:31:31.000000 apprise-1.7.6/apprise/plugins/__init__.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)        0 2023-06-03 19:32:05.000000 apprise-1.7.6/apprise/py.typed
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    53185 2024-01-27 20:12:32.000000 apprise-1.7.6/apprise/utils.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-04-14 00:12:19.068314 apprise-1.7.6/apprise.egg-info/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    44618 2024-04-14 00:12:18.000000 apprise-1.7.6/apprise.egg-info/PKG-INFO
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    10509 2024-04-14 00:12:19.000000 apprise-1.7.6/apprise.egg-info/SOURCES.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)        1 2024-04-14 00:12:18.000000 apprise-1.7.6/apprise.egg-info/dependency_links.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       45 2024-04-14 00:12:18.000000 apprise-1.7.6/apprise.egg-info/entry_points.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      101 2024-04-14 00:12:18.000000 apprise-1.7.6/apprise.egg-info/requires.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)        8 2024-04-14 00:12:18.000000 apprise-1.7.6/apprise.egg-info/top_level.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       65 2023-08-20 16:57:52.000000 apprise-1.7.6/dev-requirements.txt
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-04-14 00:12:19.088314 apprise-1.7.6/packaging/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1281 2023-06-03 19:32:05.000000 apprise-1.7.6/packaging/README.md
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-04-14 00:12:19.088314 apprise-1.7.6/packaging/man/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9039 2024-03-30 13:59:07.000000 apprise-1.7.6/packaging/man/apprise.1
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13374 2024-03-30 13:59:07.000000 apprise-1.7.6/packaging/man/apprise.1.html
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8164 2024-03-09 21:39:52.000000 apprise-1.7.6/packaging/man/apprise.md
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-04-14 00:12:19.089314 apprise-1.7.6/packaging/redhat/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1586 2024-01-27 20:41:30.000000 apprise-1.7.6/packaging/redhat/apprise-click67-support.patch
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      596 2024-01-27 20:41:32.000000 apprise-1.7.6/packaging/redhat/apprise-no-macosx-testing.patch
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      785 2024-01-27 20:41:35.000000 apprise-1.7.6/packaging/redhat/apprise-pytest-session_mocker-removal.patch
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14180 2024-04-14 00:11:13.000000 apprise-1.7.6/packaging/redhat/python-apprise.spec
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      164 2023-06-03 19:32:05.000000 apprise-1.7.6/requirements.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      861 2024-04-14 00:12:19.108314 apprise-1.7.6/setup.cfg
+-rwxr-xr-x   0 l2g       (1000) l2g       (1000)     4387 2024-04-14 00:10:08.000000 apprise-1.7.6/setup.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-04-14 00:12:19.105314 apprise-1.7.6/test/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2422 2024-01-27 20:33:15.000000 apprise-1.7.6/test/conftest.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-04-14 00:12:19.106314 apprise-1.7.6/test/helpers/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1618 2024-01-27 20:33:15.000000 apprise-1.7.6/test/helpers/__init__.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1668 2023-08-20 03:33:33.000000 apprise-1.7.6/test/helpers/asyncio.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4924 2024-01-27 20:33:15.000000 apprise-1.7.6/test/helpers/module.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    22600 2024-01-27 20:33:15.000000 apprise-1.7.6/test/helpers/rest.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    68108 2024-04-09 00:19:20.000000 apprise-1.7.6/test/test_api.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12488 2024-04-09 00:19:20.000000 apprise-1.7.6/test/test_apprise_attachments.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    40246 2024-03-09 21:39:49.000000 apprise-1.7.6/test/test_apprise_cli.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    40843 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_apprise_config.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2248 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_apprise_emojis.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3617 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_apprise_pickle.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13983 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_apprise_translations.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    96705 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_apprise_utils.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3693 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_asyncio.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3372 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_attach_base.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8491 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_attach_file.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    17522 2024-03-29 19:00:10.000000 apprise-1.7.6/test/test_attach_http.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    42141 2024-03-30 13:53:24.000000 apprise-1.7.6/test/test_config_base.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4112 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_config_file.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    10868 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_config_http.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2358 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_config_memory.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6698 2024-03-30 13:53:24.000000 apprise-1.7.6/test/test_conversion.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    15813 2024-03-29 20:20:13.000000 apprise-1.7.6/test/test_decorator_notify.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7557 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_escapes.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14361 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_logger.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13614 2024-03-03 19:41:00.000000 apprise-1.7.6/test/test_notification_manager.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12929 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_notify_base.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9896 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_apprise_api.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12977 2024-04-13 23:33:39.000000 apprise-1.7.6/test/test_plugin_aprs.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5274 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_bark.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6614 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_boxcar.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7285 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_bulksms.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6274 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_bulkvs.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6266 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_burstsms.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2890 2024-04-09 01:01:27.000000 apprise-1.7.6/test/test_plugin_chantify.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3358 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_clicksend.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    15681 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_custom_form.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11633 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_custom_json.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13640 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_custom_xml.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7486 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_d7networks.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8034 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_dapnet.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3980 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_dingtalk.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    27507 2024-02-18 15:11:50.000000 apprise-1.7.6/test/test_plugin_discord.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    71463 2024-04-09 00:19:20.000000 apprise-1.7.6/test/test_plugin_email.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14521 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_emby.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6088 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_enigma2.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    31323 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_fcm.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2856 2024-04-10 23:44:32.000000 apprise-1.7.6/test/test_plugin_feishu.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6308 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_flock.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2918 2024-03-30 13:53:24.000000 apprise-1.7.6/test/test_plugin_freemobile.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    17424 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_glib.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12170 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_gnome.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6321 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_google_chat.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6415 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_gotify.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12690 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_growl.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6570 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_guilded.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5233 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_homeassistant.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5689 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_httpsms.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6761 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_ifttt.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7448 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_join.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4226 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_kavenegar.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4063 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_kumulos.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9782 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_lametric.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3355 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_line.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    10004 2024-03-09 21:39:52.000000 apprise-1.7.6/test/test_plugin_lunasea.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7654 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_macosx.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14672 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_mailgun.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    25055 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_mastodon.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    38833 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_matrix.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4940 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_mattermost.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4575 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_messagebird.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3813 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_misskey.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14198 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_mqtt.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7272 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_msg91.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    23826 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_msteams.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7226 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_nextcloud.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6868 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_nextcloudtalk.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5079 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_notica.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6146 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_notifiarr.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4376 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_notifico.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    20084 2024-02-17 16:42:25.000000 apprise-1.7.6/test/test_plugin_ntfy.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12395 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_office365.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7949 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_onesignal.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7439 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_opsgenie.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4943 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_pagerduty.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4871 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_pagertree.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3750 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_parse_platform.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3619 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_popcorn_notify.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6632 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_prowl.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13080 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_pushbullet.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4230 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_pushdeer.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7236 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_pushed.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3781 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_pushjet.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3726 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_pushme.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    15398 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_pushover.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9043 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_pushsafer.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5531 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_pushy.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14553 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_reddit.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    17404 2024-02-18 15:11:50.000000 apprise-1.7.6/test/test_plugin_revolt.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11605 2024-04-14 00:09:29.000000 apprise-1.7.6/test/test_plugin_rocket_chat.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6913 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_rsyslog.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5067 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_ryver.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5497 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_sendgrid.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2710 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_serverchan.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14643 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_ses.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13355 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_signal.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5695 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_simplepush.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6246 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_sinch.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    26717 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_slack.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6373 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_sms_manager.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    25558 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_smseagle.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8764 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_smtp2go.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14294 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_sns.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14172 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_sparkpost.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5036 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_streamlabs.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5820 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_synology.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5021 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_syslog.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3061 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_techululs_push.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    35550 2024-04-11 01:21:34.000000 apprise-1.7.6/test/test_plugin_telegram.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5975 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_threema.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4831 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_title_maxlen.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8253 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_twilio.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16766 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_twist.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    35721 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_twitter.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7584 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_voipms.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7918 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_vonage.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3970 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_webex_teams.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3167 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_wecombot.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9129 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_whatsapp.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    10786 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_windows.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6495 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_plugin_xbmc_kodi.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4887 2024-04-09 01:01:29.000000 apprise-1.7.6/test/test_plugin_zulip.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)   140538 2024-01-27 20:33:15.000000 apprise-1.7.6/test/test_rest_plugins.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-04-14 00:12:19.106314 apprise-1.7.6/test/var/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1913 2023-06-03 19:32:05.000000 apprise-1.7.6/test/var/01_test_example.html
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      277 2023-06-03 19:32:05.000000 apprise-1.7.6/test/var/apprise-archive.zip
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    76646 2023-06-03 19:32:05.000000 apprise-1.7.6/test/var/apprise-test.gif
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    73667 2023-06-03 19:32:05.000000 apprise-1.7.6/test/var/apprise-test.jpeg
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    17856 2023-06-03 19:32:05.000000 apprise-1.7.6/test/var/apprise-test.mp4
+-rw-r--r--   0 l2g       (1000) l2g       (1000)   248280 2023-06-03 19:32:05.000000 apprise-1.7.6/test/var/apprise-test.png
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2024-04-14 00:12:19.107314 apprise-1.7.6/test/var/fcm/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2231 2023-06-03 19:32:05.000000 apprise-1.7.6/test/var/fcm/service_account-bad-type.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2238 2023-06-03 19:32:05.000000 apprise-1.7.6/test/var/fcm/service_account.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)        8 2023-06-03 19:32:05.000000 apprise-1.7.6/win-requirements.txt
```

### Comparing `apprise-1.7.5/KEYWORDS` & `apprise-1.7.6/KEYWORDS`

 * *Files 18% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 Apprise API
 Automated Packet Reporting System
 AWS
 Boxcar
 BulkSMS
 BulkVS
 Burst SMS
+Chantify
 Chat
 CLI
 ClickSend
 D7Networks
 Dapnet
 DBus
 DingTalk
 Discord
 Email
 Emby
 Enigma2
-Faast
 FCM
+Feishu
 Flock
 Form
 Free Mobile
 Gnome
 Google Chat
 Gotify
 Growl
```

### Comparing `apprise-1.7.5/LICENSE` & `apprise-1.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/PKG-INFO` & `apprise-1.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: apprise
-Version: 1.7.5
+Version: 1.7.6
 Summary: Push Notifications that work with just about every platform!
 Home-page: https://github.com/caronc/apprise
 Author: Chris Caron
 Author-email: lead2gold@gmail.com
 License: BSD
-Keywords: Alerts Apprise API Automated Packet Reporting System AWS Boxcar BulkSMS BulkVS Burst SMS Chat CLI ClickSend D7Networks Dapnet DBus DingTalk Discord Email Emby Enigma2 Faast FCM Flock Form Free Mobile Gnome Google Chat Gotify Growl Guilded Home Assistant httpSMS IFTTT Join JSON Kavenegar KODI Kumulos LaMetric Line LunaSea MacOSX Mailgun Mastodon Matrix Mattermost MessageBird Microsoft Misskey MQTT MSG91 MSTeams Nextcloud NextcloudTalk Notica Notifiarr Notifico Ntfy Office365 OneSignal Opsgenie PagerDuty PagerTree ParsePlatform PopcornNotify Prowl PushBullet Pushed Pushjet PushMe Push Notifications Pushover PushSafer Pushy PushDeer Reddit Revolt Rocket.Chat RSyslog Ryver SendGrid ServerChan SES Signal SimplePush Sinch Slack SMSEagle SMS Manager SMTP2Go SNS SparkPost Streamlabs Stride Synology Chat Syslog Techulus Telegram Threema Gateway Twilio Twist Twitter Voipms Vonage Webex WeCom Bot WhatsApp Windows XBMC XML Zulip
+Keywords: Alerts Apprise API Automated Packet Reporting System AWS Boxcar BulkSMS BulkVS Burst SMS Chantify Chat CLI ClickSend D7Networks Dapnet DBus DingTalk Discord Email Emby Enigma2 FCM Feishu Flock Form Free Mobile Gnome Google Chat Gotify Growl Guilded Home Assistant httpSMS IFTTT Join JSON Kavenegar KODI Kumulos LaMetric Line LunaSea MacOSX Mailgun Mastodon Matrix Mattermost MessageBird Microsoft Misskey MQTT MSG91 MSTeams Nextcloud NextcloudTalk Notica Notifiarr Notifico Ntfy Office365 OneSignal Opsgenie PagerDuty PagerTree ParsePlatform PopcornNotify Prowl PushBullet Pushed Pushjet PushMe Push Notifications Pushover PushSafer Pushy PushDeer Reddit Revolt Rocket.Chat RSyslog Ryver SendGrid ServerChan SES Signal SimplePush Sinch Slack SMSEagle SMS Manager SMTP2Go SNS SparkPost Streamlabs Stride Synology Chat Syslog Techulus Telegram Threema Gateway Twilio Twist Twitter Voipms Vonage Webex WeCom Bot WhatsApp Windows XBMC XML Zulip
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -87,19 +88,20 @@
 
 | Notification Service | Service ID | Default Port | Example Syntax |
 | -------------------- | ---------- | ------------ | -------------- |
 | [Apprise API](https://github.com/caronc/apprise/wiki/Notify_apprise_api)  | apprise:// or apprises:// | (TCP) 80 or 443 | apprise://hostname/Token
 | [AWS SES](https://github.com/caronc/apprise/wiki/Notify_ses)  | ses://   | (TCP) 443   | ses://user@domain/AccessKeyID/AccessSecretKey/RegionName<br/>ses://user@domain/AccessKeyID/AccessSecretKey/RegionName/email1/email2/emailN
 | [Bark](https://github.com/caronc/apprise/wiki/Notify_bark)  | bark://   | (TCP) 80 or 443   | bark://hostname<br />bark://hostname/device_key<br />bark://hostname/device_key1/device_key2/device_keyN<br/>barks://hostname<br />barks://hostname/device_key<br />barks://hostname/device_key1/device_key2/device_keyN
 | [Boxcar](https://github.com/caronc/apprise/wiki/Notify_boxcar)  | boxcar://   | (TCP) 443   | boxcar://hostname<br />boxcar://hostname/@tag<br/>boxcar://hostname/device_token<br />boxcar://hostname/device_token1/device_token2/device_tokenN<br />boxcar://hostname/@tag/@tag2/device_token
+| [Chantify](https://github.com/caronc/apprise/wiki/Notify_chantify) | chantify://    | (TCP) 443    | chantify://token
 | [Discord](https://github.com/caronc/apprise/wiki/Notify_discord)  | discord://   | (TCP) 443   | discord://webhook_id/webhook_token<br />discord://avatar@webhook_id/webhook_token
 | [Emby](https://github.com/caronc/apprise/wiki/Notify_emby)  | emby:// or embys:// | (TCP) 8096 | emby://user@hostname/<br />emby://user:password@hostname
 | [Enigma2](https://github.com/caronc/apprise/wiki/Notify_enigma2)  | enigma2:// or enigma2s:// | (TCP) 80 or 443 | enigma2://hostname
-| [Faast](https://github.com/caronc/apprise/wiki/Notify_faast) | faast://    | (TCP) 443    | faast://authorizationtoken
 | [FCM](https://github.com/caronc/apprise/wiki/Notify_fcm) | fcm://    | (TCP) 443    | fcm://project@apikey/DEVICE_ID<br />fcm://project@apikey/#TOPIC<br/>fcm://project@apikey/DEVICE_ID1/#topic1/#topic2/DEVICE_ID2/
+| [Feishu](https://github.com/caronc/apprise/wiki/Notify_feishu) | feishu://    | (TCP) 443    | feishu://token
 | [Flock](https://github.com/caronc/apprise/wiki/Notify_flock) | flock://    | (TCP) 443    | flock://token<br/>flock://botname@token<br/>flock://app_token/u:userid<br/>flock://app_token/g:channel_id<br/>flock://app_token/u:userid/g:channel_id
 | [Google Chat](https://github.com/caronc/apprise/wiki/Notify_googlechat) | gchat://    | (TCP) 443    | gchat://workspace/key/token
 | [Gotify](https://github.com/caronc/apprise/wiki/Notify_gotify) | gotify:// or gotifys://   | (TCP) 80 or 443    | gotify://hostname/token<br />gotifys://hostname/token?priority=high
 | [Growl](https://github.com/caronc/apprise/wiki/Notify_growl)  | growl://   | (UDP) 23053   | growl://hostname<br />growl://hostname:portno<br />growl://password@hostname<br />growl://password@hostname:port</br>**Note**: you can also use the get parameter _version_ which can allow the growl request to behave using the older v1.x protocol. An example would look like: growl://hostname?version=1
 | [Guilded](https://github.com/caronc/apprise/wiki/Notify_guilded)  | guilded://   | (TCP) 443   | guilded://webhook_id/webhook_token<br />guilded://avatar@webhook_id/webhook_token
 | [Home Assistant](https://github.com/caronc/apprise/wiki/Notify_homeassistant)       | hassio:// or hassios://   | (TCP) 8123 or 443 | hassio://hostname/accesstoken<br />hassio://user@hostname/accesstoken<br />hassio://user:password@hostname:port/accesstoken<br />hassio://hostname/optional/path/accesstoken
 | [IFTTT](https://github.com/caronc/apprise/wiki/Notify_ifttt) | ifttt://    | (TCP) 443    | ifttt://webhooksID/Event<br />ifttt://webhooksID/Event1/Event2/EventN<br/>ifttt://webhooksID/Event1/?+Key=Value<br/>ifttt://webhooksID/Event1/?-Key=value1
```

### Comparing `apprise-1.7.5/README.md` & `apprise-1.7.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -56,19 +56,20 @@
 
 | Notification Service | Service ID | Default Port | Example Syntax |
 | -------------------- | ---------- | ------------ | -------------- |
 | [Apprise API](https://github.com/caronc/apprise/wiki/Notify_apprise_api)  | apprise:// or apprises:// | (TCP) 80 or 443 | apprise://hostname/Token
 | [AWS SES](https://github.com/caronc/apprise/wiki/Notify_ses)  | ses://   | (TCP) 443   | ses://user@domain/AccessKeyID/AccessSecretKey/RegionName<br/>ses://user@domain/AccessKeyID/AccessSecretKey/RegionName/email1/email2/emailN
 | [Bark](https://github.com/caronc/apprise/wiki/Notify_bark)  | bark://   | (TCP) 80 or 443   | bark://hostname<br />bark://hostname/device_key<br />bark://hostname/device_key1/device_key2/device_keyN<br/>barks://hostname<br />barks://hostname/device_key<br />barks://hostname/device_key1/device_key2/device_keyN
 | [Boxcar](https://github.com/caronc/apprise/wiki/Notify_boxcar)  | boxcar://   | (TCP) 443   | boxcar://hostname<br />boxcar://hostname/@tag<br/>boxcar://hostname/device_token<br />boxcar://hostname/device_token1/device_token2/device_tokenN<br />boxcar://hostname/@tag/@tag2/device_token
+| [Chantify](https://github.com/caronc/apprise/wiki/Notify_chantify) | chantify://    | (TCP) 443    | chantify://token
 | [Discord](https://github.com/caronc/apprise/wiki/Notify_discord)  | discord://   | (TCP) 443   | discord://webhook_id/webhook_token<br />discord://avatar@webhook_id/webhook_token
 | [Emby](https://github.com/caronc/apprise/wiki/Notify_emby)  | emby:// or embys:// | (TCP) 8096 | emby://user@hostname/<br />emby://user:password@hostname
 | [Enigma2](https://github.com/caronc/apprise/wiki/Notify_enigma2)  | enigma2:// or enigma2s:// | (TCP) 80 or 443 | enigma2://hostname
-| [Faast](https://github.com/caronc/apprise/wiki/Notify_faast) | faast://    | (TCP) 443    | faast://authorizationtoken
 | [FCM](https://github.com/caronc/apprise/wiki/Notify_fcm) | fcm://    | (TCP) 443    | fcm://project@apikey/DEVICE_ID<br />fcm://project@apikey/#TOPIC<br/>fcm://project@apikey/DEVICE_ID1/#topic1/#topic2/DEVICE_ID2/
+| [Feishu](https://github.com/caronc/apprise/wiki/Notify_feishu) | feishu://    | (TCP) 443    | feishu://token
 | [Flock](https://github.com/caronc/apprise/wiki/Notify_flock) | flock://    | (TCP) 443    | flock://token<br/>flock://botname@token<br/>flock://app_token/u:userid<br/>flock://app_token/g:channel_id<br/>flock://app_token/u:userid/g:channel_id
 | [Google Chat](https://github.com/caronc/apprise/wiki/Notify_googlechat) | gchat://    | (TCP) 443    | gchat://workspace/key/token
 | [Gotify](https://github.com/caronc/apprise/wiki/Notify_gotify) | gotify:// or gotifys://   | (TCP) 80 or 443    | gotify://hostname/token<br />gotifys://hostname/token?priority=high
 | [Growl](https://github.com/caronc/apprise/wiki/Notify_growl)  | growl://   | (UDP) 23053   | growl://hostname<br />growl://hostname:portno<br />growl://password@hostname<br />growl://password@hostname:port</br>**Note**: you can also use the get parameter _version_ which can allow the growl request to behave using the older v1.x protocol. An example would look like: growl://hostname?version=1
 | [Guilded](https://github.com/caronc/apprise/wiki/Notify_guilded)  | guilded://   | (TCP) 443   | guilded://webhook_id/webhook_token<br />guilded://avatar@webhook_id/webhook_token
 | [Home Assistant](https://github.com/caronc/apprise/wiki/Notify_homeassistant)       | hassio:// or hassios://   | (TCP) 8123 or 443 | hassio://hostname/accesstoken<br />hassio://user@hostname/accesstoken<br />hassio://user:password@hostname:port/accesstoken<br />hassio://hostname/optional/path/accesstoken
 | [IFTTT](https://github.com/caronc/apprise/wiki/Notify_ifttt) | ifttt://    | (TCP) 443    | ifttt://webhooksID/Event<br />ifttt://webhooksID/Event1/Event2/EventN<br/>ifttt://webhooksID/Event1/?+Key=Value<br/>ifttt://webhooksID/Event1/?-Key=value1
```

### Comparing `apprise-1.7.5/apprise/Apprise.py` & `apprise-1.7.6/apprise/Apprise.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/Apprise.pyi` & `apprise-1.7.6/apprise/Apprise.pyi`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/AppriseAsset.py` & `apprise-1.7.6/apprise/AppriseAsset.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/AppriseAsset.pyi` & `apprise-1.7.6/apprise/AppriseAsset.pyi`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/AppriseAttachment.py` & `apprise-1.7.6/apprise/AppriseAttachment.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/AppriseAttachment.pyi` & `apprise-1.7.6/apprise/AppriseAttachment.pyi`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/AppriseConfig.py` & `apprise-1.7.6/apprise/AppriseConfig.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/AppriseConfig.pyi` & `apprise-1.7.6/apprise/AppriseConfig.pyi`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/AppriseLocale.py` & `apprise-1.7.6/apprise/AppriseLocale.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,14 +215,17 @@
                     # Fallback to posix detection
                     pass
 
             # Built in locale library check
             try:
                 # Acquire our locale
                 lang = locale.getlocale()[0]
+                # Compatibility for Python >= 3.12
+                if lang == 'C':
+                    lang = AppriseLocale._default_language
 
             except (ValueError, TypeError) as e:
                 # This occurs when an invalid locale was parsed from the
                 # environment variable. While we still return None in this
                 # case, we want to better notify the end user of this. Users
                 # receiving this error should check their environment
                 # variables.
```

### Comparing `apprise-1.7.5/apprise/AttachmentManager.py` & `apprise-1.7.6/apprise/AttachmentManager.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/ConfigurationManager.py` & `apprise-1.7.6/apprise/ConfigurationManager.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/NotificationManager.py` & `apprise-1.7.6/apprise/NotificationManager.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/URLBase.py` & `apprise-1.7.6/apprise/URLBase.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/URLBase.pyi` & `apprise-1.7.6/apprise/URLBase.pyi`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/__init__.py` & `apprise-1.7.6/apprise/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 __title__ = 'Apprise'
-__version__ = '1.7.5'
+__version__ = '1.7.6'
 __author__ = 'Chris Caron'
 __license__ = 'BSD'
 __copywrite__ = 'Copyright (C) 2024 Chris Caron <lead2gold@gmail.com>'
 __email__ = 'lead2gold@gmail.com'
 __status__ = 'Production'
 
 from .common import NotifyType
```

### Comparing `apprise-1.7.5/apprise/assets/NotifyXML-1.0.xsd` & `apprise-1.7.6/apprise/assets/NotifyXML-1.0.xsd`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/assets/NotifyXML-1.1.xsd` & `apprise-1.7.6/apprise/assets/NotifyXML-1.1.xsd`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/assets/themes/default/apprise-failure-128x128.ico` & `apprise-1.7.6/apprise/assets/themes/default/apprise-failure-128x128.ico`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/assets/themes/default/apprise-failure-128x128.png` & `apprise-1.7.6/apprise/assets/themes/default/apprise-failure-128x128.png`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/assets/themes/default/apprise-failure-256x256.png` & `apprise-1.7.6/apprise/assets/themes/default/apprise-failure-256x256.png`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/assets/themes/default/apprise-failure-32x32.png` & `apprise-1.7.6/apprise/assets/themes/default/apprise-failure-32x32.png`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/assets/themes/default/apprise-failure-72x72.png` & `apprise-1.7.6/apprise/assets/themes/default/apprise-failure-72x72.png`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/assets/themes/default/apprise-info-128x128.ico` & `apprise-1.7.6/apprise/assets/themes/default/apprise-info-128x128.ico`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/assets/themes/default/apprise-info-128x128.png` & `apprise-1.7.6/apprise/assets/themes/default/apprise-info-128x128.png`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/assets/themes/default/apprise-info-256x256.png` & `apprise-1.7.6/apprise/assets/themes/default/apprise-info-256x256.png`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/assets/themes/default/apprise-info-32x32.png` & `apprise-1.7.6/apprise/assets/themes/default/apprise-info-32x32.png`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/assets/themes/default/apprise-info-72x72.png` & `apprise-1.7.6/apprise/assets/themes/default/apprise-info-72x72.png`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/assets/themes/default/apprise-logo.png` & `apprise-1.7.6/apprise/assets/themes/default/apprise-logo.png`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/assets/themes/default/apprise-success-128x128.ico` & `apprise-1.7.6/apprise/assets/themes/default/apprise-success-128x128.ico`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/assets/themes/default/apprise-success-128x128.png` & `apprise-1.7.6/apprise/assets/themes/default/apprise-success-128x128.png`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/assets/themes/default/apprise-success-256x256.png` & `apprise-1.7.6/apprise/assets/themes/default/apprise-success-256x256.png`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/assets/themes/default/apprise-success-32x32.png` & `apprise-1.7.6/apprise/assets/themes/default/apprise-success-32x32.png`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/assets/themes/default/apprise-success-72x72.png` & `apprise-1.7.6/apprise/assets/themes/default/apprise-success-72x72.png`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/assets/themes/default/apprise-warning-128x128.ico` & `apprise-1.7.6/apprise/assets/themes/default/apprise-warning-128x128.ico`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/assets/themes/default/apprise-warning-128x128.png` & `apprise-1.7.6/apprise/assets/themes/default/apprise-warning-128x128.png`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/assets/themes/default/apprise-warning-256x256.png` & `apprise-1.7.6/apprise/assets/themes/default/apprise-warning-256x256.png`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/assets/themes/default/apprise-warning-32x32.png` & `apprise-1.7.6/apprise/assets/themes/default/apprise-warning-32x32.png`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/assets/themes/default/apprise-warning-72x72.png` & `apprise-1.7.6/apprise/assets/themes/default/apprise-warning-72x72.png`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/attachment/AttachBase.py` & `apprise-1.7.6/apprise/attachment/AttachBase.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/attachment/AttachBase.pyi` & `apprise-1.7.6/apprise/attachment/AttachBase.pyi`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/attachment/AttachFile.py` & `apprise-1.7.6/apprise/attachment/AttachFile.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/attachment/AttachHTTP.py` & `apprise-1.7.6/apprise/attachment/AttachHTTP.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/attachment/__init__.py` & `apprise-1.7.6/apprise/attachment/__init__.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/cli.py` & `apprise-1.7.6/apprise/cli.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/common.py` & `apprise-1.7.6/apprise/common.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/config/ConfigBase.py` & `apprise-1.7.6/apprise/config/ConfigBase.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/config/ConfigFile.py` & `apprise-1.7.6/apprise/config/ConfigFile.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/config/ConfigHTTP.py` & `apprise-1.7.6/apprise/config/ConfigHTTP.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/config/ConfigMemory.py` & `apprise-1.7.6/apprise/config/ConfigMemory.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/config/__init__.py` & `apprise-1.7.6/apprise/config/__init__.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/conversion.py` & `apprise-1.7.6/apprise/conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,16 @@
     return convert(content) if convert else content
 
 
 def markdown_to_html(content):
     """
     Converts specified content from markdown to HTML.
     """
-    return markdown(content, extensions=['nl2br', 'tables'])
+    return markdown(content, extensions=[
+        'markdown.extensions.nl2br', 'markdown.extensions.tables'])
 
 
 def text_to_html(content):
     """
     Converts specified content from plain text to HTML.
     """
```

### Comparing `apprise-1.7.5/apprise/decorators/CustomNotifyPlugin.py` & `apprise-1.7.6/apprise/decorators/CustomNotifyPlugin.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/decorators/__init__.py` & `apprise-1.7.6/apprise/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/decorators/notify.py` & `apprise-1.7.6/apprise/decorators/notify.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/emojis.py` & `apprise-1.7.6/apprise/emojis.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/i18n/en/LC_MESSAGES/apprise.mo` & `apprise-1.7.6/apprise/i18n/en/LC_MESSAGES/apprise.mo`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/logger.py` & `apprise-1.7.6/apprise/logger.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/manager.py` & `apprise-1.7.6/apprise/manager.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyAppriseAPI.py` & `apprise-1.7.6/apprise/plugins/NotifyAppriseAPI.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyAprs.py` & `apprise-1.7.6/apprise/plugins/NotifyAprs.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,24 +199,31 @@
         NotifyBase.template_args,
         **{
             "to": {
                 "name": _("Target Callsign"),
                 "type": "string",
                 "map_to": "targets",
             },
+            "delay": {
+                "name": _("Resend Delay"),
+                "type": "float",
+                "min": 0.0,
+                "max": 5.0,
+                "default": 0.0,
+            },
             "locale": {
                 "name": _("Locale"),
                 "type": "choice:string",
                 "values": APRS_LOCALES,
                 "default": "EURO",
             },
         }
     )
 
-    def __init__(self, targets=None, locale=None, **kwargs):
+    def __init__(self, targets=None, locale=None, delay=None, **kwargs):
         """
         Initialize APRS Object
         """
         super().__init__(**kwargs)
 
         # Our (future) socket sobject
         self.sock = None
@@ -268,14 +275,36 @@
                     "Received: {}. Valid: {}".format(
                         locale, ", ".join(str(x) for x in APRS_LOCALES.keys())
                     )
                 )
                 self.logger.warning(msg)
                 raise TypeError(msg)
 
+        # Update our delay
+        if delay is None:
+            self.delay = NotifyAprs.template_args["delay"]["default"]
+
+        else:
+            try:
+                self.delay = float(delay)
+                if self.delay < NotifyAprs.template_args["delay"]["min"]:
+                    raise ValueError()
+
+                elif self.delay >= NotifyAprs.template_args["delay"]["max"]:
+                    raise ValueError()
+
+            except (TypeError, ValueError):
+                msg = "Unsupported APRS-IS delay ({}) specified. ".format(
+                    delay)
+                self.logger.warning(msg)
+                raise TypeError(msg)
+
+        # Bump up our request_rate
+        self.request_rate_per_sec += self.delay
+
         # Set the transmitter group
         self.locale = \
             NotifyAprs.template_args["locale"]["default"] \
             if not locale else locale.upper()
 
         # Used for URL generation afterwards only
         self.invalid_targets = list()
@@ -670,14 +699,18 @@
         # Define any URL parameters
         params = {}
 
         if self.locale != NotifyAprs.template_args["locale"]["default"]:
             # Store our locale if not default
             params['locale'] = self.locale
 
+        if self.delay != NotifyAprs.template_args["delay"]["default"]:
+            # Store our locale if not default
+            params['delay'] = "{:.2f}".format(self.delay)
+
         # Extend our parameters
         params.update(self.url_parameters(privacy=privacy, *args, **kwargs))
 
         # Setup Authentication
         auth = "{user}:{password}@".format(
             user=NotifyAprs.quote(self.user, safe=""),
             password=self.pprint(
@@ -723,14 +756,18 @@
 
         # All elements are targets
         results["targets"] = [NotifyAprs.unquote(results["host"])]
 
         # All entries after the hostname are additional targets
         results["targets"].extend(NotifyAprs.split_path(results["fullpath"]))
 
+        # Get Delay (if set)
+        if 'delay' in results['qsd'] and len(results['qsd']['delay']):
+            results['delay'] = NotifyAprs.unquote(results['qsd']['delay'])
+
         # Support the 'to' variable so that we can support rooms this way too
         # The 'to' makes it easier to use yaml configuration
         if "to" in results["qsd"] and len(results["qsd"]["to"]):
             results["targets"] += NotifyAprs.parse_list(results["qsd"]["to"])
 
         # Set our APRS-IS server locale's key value and convert it to uppercase
         if "locale" in results["qsd"] and len(results["qsd"]["locale"]):
```

### Comparing `apprise-1.7.5/apprise/plugins/NotifyBark.py` & `apprise-1.7.6/apprise/plugins/NotifyBark.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyBase.py` & `apprise-1.7.6/apprise/plugins/NotifyBase.py`

 * *Files 2% similar despite different names*

```diff
@@ -453,23 +453,36 @@
                 " service skipped"
             self.logger.warning(msg)
             raise TypeError(msg)
 
         # Handle situations where the title is None
         title = '' if not title else title
 
+        # Truncate flag set with attachments ensures that only 1
+        # attachment passes through. In the event there could be many
+        # services specified, we only want to do this logic once.
+        # The logic is only applicable if ther was more then 1 attachment
+        # specified
+        overflow = self.overflow_mode if overflow is None else overflow
+        if attach and len(attach) > 1 and overflow == OverflowMode.TRUNCATE:
+            # Save first attachment
+            _attach = AppriseAttachment(attach[0], asset=self.asset)
+        else:
+            # reference same attachment
+            _attach = attach
+
         # Apply our overflow (if defined)
         for chunk in self._apply_overflow(
                 body=body, title=title, overflow=overflow,
                 body_format=body_format):
 
             # Send notification
             yield dict(
                 body=chunk['body'], title=chunk['title'],
-                notify_type=notify_type, attach=attach,
+                notify_type=notify_type, attach=_attach,
                 body_format=body_format
             )
 
     def _apply_overflow(self, body, title=None, overflow=None,
                         body_format=None):
         """
         Takes the message body and title as input.  This function then
@@ -481,15 +494,15 @@
             [
                 {
                     title: 'the title goes here',
                     body: 'the message body goes here',
                 },
                 {
                     title: 'the title goes here',
-                    body: 'the message body goes here',
+                    body: 'the continued message body goes here',
                 },
 
             ]
         """
 
         response = list()
```

### Comparing `apprise-1.7.5/apprise/plugins/NotifyBoxcar.py` & `apprise-1.7.6/apprise/plugins/NotifyBoxcar.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyBulkSMS.py` & `apprise-1.7.6/apprise/plugins/NotifyBulkSMS.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyBulkVS.py` & `apprise-1.7.6/apprise/plugins/NotifyBulkVS.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyBurstSMS.py` & `apprise-1.7.6/apprise/plugins/NotifyBurstSMS.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyClickSend.py` & `apprise-1.7.6/apprise/plugins/NotifyClickSend.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyD7Networks.py` & `apprise-1.7.6/apprise/plugins/NotifyD7Networks.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyDBus.py` & `apprise-1.7.6/apprise/plugins/NotifyDBus.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyDapnet.py` & `apprise-1.7.6/apprise/plugins/NotifyDapnet.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyDingTalk.py` & `apprise-1.7.6/apprise/plugins/NotifyDingTalk.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyDiscord.py` & `apprise-1.7.6/apprise/plugins/NotifyDiscord.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyEmail.py` & `apprise-1.7.6/apprise/plugins/NotifyEmail.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 from datetime import datetime
 from datetime import timezone
 
 from .NotifyBase import NotifyBase
 from ..URLBase import PrivacyMode
 from ..common import NotifyFormat, NotifyType
 from ..conversion import convert_between
-from ..utils import is_email, parse_emails
+from ..utils import is_email, parse_emails, is_hostname
 from ..AppriseLocale import gettext_lazy as _
 from ..logger import logger
 
 # Globally Default encoding mode set to Quoted Printable.
 charset.add_charset('utf-8', charset.QP, charset.QP, 'utf-8')
 
 
@@ -562,20 +562,28 @@
                 'Dropped invalid Reply To email '
                 '({}) specified.'.format(recipient),
             )
 
         # Apply any defaults based on certain known configurations
         self.NotifyEmailDefaults(secure_mode=secure_mode, **kwargs)
 
-        if self.user and self.host:
-            # Prepare the bases of our email
-            self.from_addr = [self.app_id, '{}@{}'.format(
-                re.split(r'[\s@]+', self.user)[0],
-                self.host,
-            )]
+        if self.user:
+            if self.host:
+                # Prepare the bases of our email
+                self.from_addr = [self.app_id, '{}@{}'.format(
+                    re.split(r'[\s@]+', self.user)[0],
+                    self.host,
+                )]
+
+            else:
+                result = is_email(self.user)
+                if result:
+                    # Prepare the bases of our email and include domain
+                    self.host = result['domain']
+                    self.from_addr = [self.app_id, self.user]
 
         if from_addr:
             result = is_email(from_addr)
             if result:
                 self.from_addr = (
                     result['name'] if result['name'] else False,
                     result['full_email'])
@@ -1033,30 +1041,44 @@
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
-        results = NotifyBase.parse_url(url)
+        results = NotifyBase.parse_url(url, verify_host=False)
         if not results:
             # We're done early as we couldn't load the results
             return results
 
+        # Prepare our target lists
+        results['targets'] = []
+
+        if not is_hostname(results['host'], ipv4=False, ipv6=False,
+                           underscore=False):
+
+            if is_email(NotifyEmail.unquote(results['host'])):
+                # Don't lose defined email addresses
+                results['targets'].append(NotifyEmail.unquote(results['host']))
+
+            # Detect if we have a valid hostname or not; be sure to reset it's
+            # value if invalid; we'll attempt to figure this out later on
+            results['host'] = ''
+
         # The From address is a must; either through the use of templates
         # from= entry and/or merging the user and hostname together, this
         # must be calculated or parse_url will fail.
         from_addr = ''
 
         # The server we connect to to send our mail to
         smtp_host = ''
 
         # Get our potential email targets; if none our found we'll just
         # add one to ourselves
-        results['targets'] = NotifyEmail.split_path(results['fullpath'])
+        results['targets'] += NotifyEmail.split_path(results['fullpath'])
 
         # Attempt to detect 'to' email address
         if 'to' in results['qsd'] and len(results['qsd']['to']):
             results['targets'].append(results['qsd']['to'])
 
         # Attempt to detect 'from' email address
         if 'from' in results['qsd'] and len(results['qsd']['from']):
```

### Comparing `apprise-1.7.5/apprise/plugins/NotifyEmby.py` & `apprise-1.7.6/apprise/plugins/NotifyEmby.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyEnigma2.py` & `apprise-1.7.6/apprise/plugins/NotifyEnigma2.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyFCM/__init__.py` & `apprise-1.7.6/apprise/plugins/NotifyFCM/__init__.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyFCM/color.py` & `apprise-1.7.6/apprise/plugins/NotifyFCM/color.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyFCM/common.py` & `apprise-1.7.6/apprise/plugins/NotifyFCM/common.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyFCM/oauth.py` & `apprise-1.7.6/apprise/plugins/NotifyFCM/oauth.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyFCM/priority.py` & `apprise-1.7.6/apprise/plugins/NotifyFCM/priority.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyFaast.py` & `apprise-1.7.6/apprise/plugins/NotifyPushMe.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,151 +25,148 @@
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 import requests
 
 from .NotifyBase import NotifyBase
-from ..common import NotifyImageSize
 from ..common import NotifyType
+from ..common import NotifyFormat
+from ..utils import validate_regex
 from ..utils import parse_bool
 from ..AppriseLocale import gettext_lazy as _
-from ..utils import validate_regex
 
 
-class NotifyFaast(NotifyBase):
+class NotifyPushMe(NotifyBase):
     """
-    A wrapper for Faast Notifications
+    A wrapper for PushMe Notifications
     """
 
     # The default descriptive name associated with the Notification
-    service_name = 'Faast'
+    service_name = 'PushMe'
 
     # The services URL
-    service_url = 'http://www.faast.io/'
+    service_url = 'https://push.i-i.me/'
 
-    # The default protocol (this is secure for faast)
-    protocol = 'faast'
+    # Insecure protocol (for those self hosted requests)
+    protocol = 'pushme'
 
     # A URL that takes you to the setup/help of the specific protocol
-    setup_url = 'https://github.com/caronc/apprise/wiki/Notify_faast'
+    setup_url = 'https://github.com/caronc/apprise/wiki/Notify_pushme'
 
-    # Faast uses the http protocol with JSON requests
-    notify_url = 'https://www.appnotifications.com/account/notifications.json'
-
-    # Allows the user to specify the NotifyImageSize object
-    image_size = NotifyImageSize.XY_72
+    # PushMe URL
+    notify_url = 'https://push.i-i.me/'
 
     # Define object templates
     templates = (
-        '{schema}://{authtoken}',
+        '{schema}://{token}',
     )
 
     # Define our template tokens
     template_tokens = dict(NotifyBase.template_tokens, **{
-        'authtoken': {
-            'name': _('Authorization Token'),
+        'token': {
+            'name': _('Token'),
             'type': 'string',
             'private': True,
             'required': True,
         },
     })
 
     # Define our template arguments
     template_args = dict(NotifyBase.template_args, **{
-        'image': {
-            'name': _('Include Image'),
+        'token': {
+            'alias_of': 'token',
+        },
+        'push_key': {
+            'alias_of': 'token',
+        },
+        'status': {
+            'name': _('Show Status'),
             'type': 'bool',
             'default': True,
-            'map_to': 'include_image',
         },
     })
 
-    def __init__(self, authtoken, include_image=True, **kwargs):
+    def __init__(self, token, status=None, **kwargs):
         """
-        Initialize Faast Object
+        Initialize PushMe Object
         """
         super().__init__(**kwargs)
 
-        # Store the Authentication Token
-        self.authtoken = validate_regex(authtoken)
-        if not self.authtoken:
-            msg = 'An invalid Faast Authentication Token ' \
-                  '({}) was specified.'.format(authtoken)
+        # Token (associated with project)
+        self.token = validate_regex(token)
+        if not self.token:
+            msg = 'An invalid PushMe Token ' \
+                  '({}) was specified.'.format(token)
             self.logger.warning(msg)
             raise TypeError(msg)
 
-        # Associate an image with our post
-        self.include_image = include_image
+        # Set Status type
+        self.status = status
 
         return
 
     def send(self, body, title='', notify_type=NotifyType.INFO, **kwargs):
         """
-        Perform Faast Notification
+        Perform PushMe Notification
         """
 
         headers = {
             'User-Agent': self.app_id,
-            'Content-Type': 'multipart/form-data'
         }
 
-        # prepare JSON Object
-        payload = {
-            'user_credentials': self.authtoken,
-            'title': title,
-            'message': body,
+        # Prepare our payload
+        params = {
+            'push_key': self.token,
+            'title': title if not self.status
+            else '{} {}'.format(self.asset.ascii(notify_type), title),
+            'content': body,
+            'type': 'markdown'
+            if self.notify_format == NotifyFormat.MARKDOWN else 'text'
         }
 
-        # Acquire our image if we're configured to do so
-        image_url = None if not self.include_image \
-            else self.image_url(notify_type)
-
-        if image_url:
-            payload['icon_url'] = image_url
-
-        self.logger.debug('Faast POST URL: %s (cert_verify=%r)' % (
+        self.logger.debug('PushMe POST URL: %s (cert_verify=%r)' % (
             self.notify_url, self.verify_certificate,
         ))
-        self.logger.debug('Faast Payload: %s' % str(payload))
+        self.logger.debug('PushMe Payload: %s' % str(params))
 
         # Always call throttle before any remote server i/o is made
         self.throttle()
 
         try:
             r = requests.post(
                 self.notify_url,
-                data=payload,
+                params=params,
                 headers=headers,
                 verify=self.verify_certificate,
                 timeout=self.request_timeout,
             )
             if r.status_code != requests.codes.ok:
                 # We had a problem
                 status_str = \
-                    NotifyFaast.http_response_code_lookup(r.status_code)
+                    NotifyPushMe.http_response_code_lookup(r.status_code)
 
                 self.logger.warning(
-                    'Failed to send Faast notification:'
+                    'Failed to send PushMe notification:'
                     '{}{}error={}.'.format(
                         status_str,
                         ', ' if status_str else '',
                         r.status_code))
 
                 self.logger.debug('Response Details:\r\n{}'.format(r.content))
 
                 # Return; we're done
                 return False
 
             else:
-                self.logger.info('Sent Faast notification.')
+                self.logger.info('Sent PushMe notification.')
 
         except requests.RequestException as e:
             self.logger.warning(
-                'A Connection error occurred sending Faast notification.',
+                'A Connection error occurred sending PushMe notification.',
             )
             self.logger.debug('Socket Exception: %s' % str(e))
 
             # Return; we're done
             return False
 
         return True
@@ -177,39 +174,48 @@
     def url(self, privacy=False, *args, **kwargs):
         """
         Returns the URL built dynamically based on specified arguments.
         """
 
         # Define any URL parameters
         params = {
-            'image': 'yes' if self.include_image else 'no',
+            'status': 'yes' if self.status else 'no',
         }
 
         # Extend our parameters
         params.update(self.url_parameters(privacy=privacy, *args, **kwargs))
 
-        return '{schema}://{authtoken}/?{params}'.format(
+        # Official URLs are easy to assemble
+        return '{schema}://{token}/?{params}'.format(
             schema=self.protocol,
-            authtoken=self.pprint(self.authtoken, privacy, safe=''),
-            params=NotifyFaast.urlencode(params),
+            token=self.pprint(self.token, privacy, safe=''),
+            params=NotifyPushMe.urlencode(params),
         )
 
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
         results = NotifyBase.parse_url(url, verify_host=False)
         if not results:
             # We're done early as we couldn't load the results
             return results
 
-        # Store our authtoken using the host
-        results['authtoken'] = NotifyFaast.unquote(results['host'])
+        # Store our token using the host
+        results['token'] = NotifyPushMe.unquote(results['host'])
 
-        # Include image with our post
-        results['include_image'] = \
-            parse_bool(results['qsd'].get('image', True))
+        # The 'token' makes it easier to use yaml configuration
+        if 'token' in results['qsd'] and len(results['qsd']['token']):
+            results['token'] = NotifyPushMe.unquote(results['qsd']['token'])
+
+        elif 'push_key' in results['qsd'] and len(results['qsd']['push_key']):
+            # Support 'push_key' if specified
+            results['token'] = NotifyPushMe.unquote(results['qsd']['push_key'])
+
+        # Get status switch
+        results['status'] = \
+            parse_bool(results['qsd'].get('status', True))
 
         return results
```

### Comparing `apprise-1.7.5/apprise/plugins/NotifyFlock.py` & `apprise-1.7.6/apprise/plugins/NotifyFlock.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyForm.py` & `apprise-1.7.6/apprise/plugins/NotifyForm.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyFreeMobile.py` & `apprise-1.7.6/apprise/plugins/NotifyFreeMobile.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 # Free Mobile
 #   1. Visit https://mobile.free.fr/
 
 # the URL will look something like this:
-#      https://smsapi.free-mobile.fr/sendmsg?msg=content
+#      https://smsapi.free-mobile.fr/sendmsg
 #
 
 import requests
 from json import dumps
 
 from .NotifyBase import NotifyBase
 from ..common import NotifyType
@@ -75,19 +75,21 @@
     # Define our tokens; these are the minimum tokens required required to
     # be passed into this function (as arguments). The syntax appends any
     # previously defined in the base package and builds onto them
     template_tokens = dict(NotifyBase.template_tokens, **{
         'user': {
             'name': _('Username'),
             'type': 'string',
+            'required': True,
         },
         'password': {
             'name': _('Password'),
             'type': 'string',
             'private': True,
+            'required': True,
         },
     })
 
     def __init__(self, **kwargs):
         """
         Initialize Free Mobile Object
         """
@@ -126,33 +128,28 @@
             'User-Agent': self.app_id,
         }
 
         # Prepare our payload
         payload = {
             'user': self.user,
             'pass': self.password,
-        }
-
-        # Our Message
-        params = {
             'msg': body
         }
 
         self.logger.debug('Free Mobile GET URL: %s (cert_verify=%r)' % (
             self.notify_url, self.verify_certificate))
         self.logger.debug('Free Mobile Payload: %s' % str(payload))
 
         # Always call throttle before any remote server i/o is made
         self.throttle()
 
         try:
             r = requests.post(
                 self.notify_url,
                 data=dumps(payload).encode('utf-8'),
-                params=params,
                 headers=headers,
                 verify=self.verify_certificate,
                 timeout=self.request_timeout,
             )
             if r.status_code != requests.codes.ok:
                 # We had a problem
                 status_str = \
```

### Comparing `apprise-1.7.5/apprise/plugins/NotifyGnome.py` & `apprise-1.7.6/apprise/plugins/NotifyGnome.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyGoogleChat.py` & `apprise-1.7.6/apprise/plugins/NotifyGoogleChat.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyGotify.py` & `apprise-1.7.6/apprise/plugins/NotifyGotify.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyGrowl.py` & `apprise-1.7.6/apprise/plugins/NotifyGrowl.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyGuilded.py` & `apprise-1.7.6/apprise/plugins/NotifyGuilded.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyHomeAssistant.py` & `apprise-1.7.6/apprise/plugins/NotifyHomeAssistant.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyHttpSMS.py` & `apprise-1.7.6/apprise/plugins/NotifyHttpSMS.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyIFTTT.py` & `apprise-1.7.6/apprise/plugins/NotifyIFTTT.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyJSON.py` & `apprise-1.7.6/apprise/plugins/NotifyJSON.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyJoin.py` & `apprise-1.7.6/apprise/plugins/NotifyJoin.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyKavenegar.py` & `apprise-1.7.6/apprise/plugins/NotifyKavenegar.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyKumulos.py` & `apprise-1.7.6/apprise/plugins/NotifyKumulos.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyLametric.py` & `apprise-1.7.6/apprise/plugins/NotifyLametric.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyLine.py` & `apprise-1.7.6/apprise/plugins/NotifyLine.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyLunaSea.py` & `apprise-1.7.6/apprise/plugins/NotifyLunaSea.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyMQTT.py` & `apprise-1.7.6/apprise/plugins/NotifyMQTT.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     """
 
     # Set our global enabled flag
     enabled = NOTIFY_MQTT_SUPPORT_ENABLED
 
     requirements = {
         # Define our required packaging in order to work
-        'packages_required': 'paho-mqtt <= 2.0.0'
+        'packages_required': 'paho-mqtt < 2.0.0'
     }
 
     # The default descriptive name associated with the Notification
     service_name = 'MQTT Notification'
 
     # The default protocol
     protocol = 'mqtt'
```

### Comparing `apprise-1.7.5/apprise/plugins/NotifyMSG91.py` & `apprise-1.7.6/apprise/plugins/NotifyMSG91.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyMSTeams.py` & `apprise-1.7.6/apprise/plugins/NotifyMSTeams.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyMacOSX.py` & `apprise-1.7.6/apprise/plugins/NotifyMacOSX.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyMailgun.py` & `apprise-1.7.6/apprise/plugins/NotifyMailgun.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyMastodon.py` & `apprise-1.7.6/apprise/plugins/NotifyMastodon.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyMatrix.py` & `apprise-1.7.6/apprise/plugins/NotifyMatrix.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyMattermost.py` & `apprise-1.7.6/apprise/plugins/NotifyMattermost.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyMessageBird.py` & `apprise-1.7.6/apprise/plugins/NotifyMessageBird.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyMisskey.py` & `apprise-1.7.6/apprise/plugins/NotifyMisskey.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyNextcloud.py` & `apprise-1.7.6/apprise/plugins/NotifyNextcloud.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyNextcloudTalk.py` & `apprise-1.7.6/apprise/plugins/NotifyNextcloudTalk.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyNotica.py` & `apprise-1.7.6/apprise/plugins/NotifyNotica.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyNotifiarr.py` & `apprise-1.7.6/apprise/plugins/NotifyNotifiarr.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyNotifico.py` & `apprise-1.7.6/apprise/plugins/NotifyNotifico.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyNtfy.py` & `apprise-1.7.6/apprise/plugins/NotifyNtfy.py`

 * *Files 1% similar despite different names*

```diff
@@ -694,15 +694,15 @@
                 params=NotifyNtfy.urlencode(params)
             )
 
     def __len__(self):
         """
         Returns the number of targets associated with this notification
         """
-        return len(self.topics)
+        return 1 if not self.topics else len(self.topics)
 
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
         """
```

### Comparing `apprise-1.7.5/apprise/plugins/NotifyOffice365.py` & `apprise-1.7.6/apprise/plugins/NotifyOffice365.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyOneSignal.py` & `apprise-1.7.6/apprise/plugins/NotifyOneSignal.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyOpsgenie.py` & `apprise-1.7.6/apprise/plugins/NotifyOpsgenie.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyPagerDuty.py` & `apprise-1.7.6/apprise/plugins/NotifyPagerDuty.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyPagerTree.py` & `apprise-1.7.6/apprise/plugins/NotifyPagerTree.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyParsePlatform.py` & `apprise-1.7.6/apprise/plugins/NotifyParsePlatform.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyPopcornNotify.py` & `apprise-1.7.6/apprise/plugins/NotifyPopcornNotify.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyProwl.py` & `apprise-1.7.6/apprise/plugins/NotifyProwl.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyPushBullet.py` & `apprise-1.7.6/apprise/plugins/NotifyPushBullet.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyPushDeer.py` & `apprise-1.7.6/apprise/plugins/NotifyPushDeer.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyPushMe.py` & `apprise-1.7.6/apprise/plugins/NotifyChantify.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,200 +22,185 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
+# Chantify
+#   1. Visit https://chanify.net/
+
+# The API URL will look something like this:
+#    https://api.chanify.net/v1/sender/token
+#
+
 import requests
 
 from .NotifyBase import NotifyBase
 from ..common import NotifyType
-from ..common import NotifyFormat
 from ..utils import validate_regex
-from ..utils import parse_bool
 from ..AppriseLocale import gettext_lazy as _
 
 
-class NotifyPushMe(NotifyBase):
+class NotifyChantify(NotifyBase):
     """
-    A wrapper for PushMe Notifications
+    A wrapper for Chantify Notifications
     """
 
     # The default descriptive name associated with the Notification
-    service_name = 'PushMe'
+    service_name = _('Chantify')
 
     # The services URL
-    service_url = 'https://push.i-i.me/'
+    service_url = 'https://chanify.net/'
 
-    # Insecure protocol (for those self hosted requests)
-    protocol = 'pushme'
+    # The default secure protocol
+    secure_protocol = 'chantify'
 
     # A URL that takes you to the setup/help of the specific protocol
-    setup_url = 'https://github.com/caronc/apprise/wiki/Notify_pushme'
+    setup_url = 'https://github.com/caronc/apprise/wiki/Notify_chantify'
 
-    # PushMe URL
-    notify_url = 'https://push.i-i.me/'
+    # Notification URL
+    notify_url = 'https://api.chanify.net/v1/sender/{token}/'
 
     # Define object templates
     templates = (
         '{schema}://{token}',
     )
 
-    # Define our template tokens
+    # The title is not used
+    title_maxlen = 0
+
+    # Define our tokens; these are the minimum tokens required required to
+    # be passed into this function (as arguments). The syntax appends any
+    # previously defined in the base package and builds onto them
     template_tokens = dict(NotifyBase.template_tokens, **{
         'token': {
             'name': _('Token'),
             'type': 'string',
             'private': True,
             'required': True,
+            'regex': (r'^[A-Z0-9_-]+$', 'i'),
         },
     })
 
     # Define our template arguments
     template_args = dict(NotifyBase.template_args, **{
         'token': {
             'alias_of': 'token',
         },
-        'push_key': {
-            'alias_of': 'token',
-        },
-        'status': {
-            'name': _('Show Status'),
-            'type': 'bool',
-            'default': True,
-        },
     })
 
-    def __init__(self, token, status=None, **kwargs):
+    def __init__(self, token, **kwargs):
         """
-        Initialize PushMe Object
+        Initialize Chantify Object
         """
         super().__init__(**kwargs)
 
-        # Token (associated with project)
-        self.token = validate_regex(token)
+        self.token = validate_regex(
+            token, *self.template_tokens['token']['regex'])
         if not self.token:
-            msg = 'An invalid PushMe Token ' \
-                  '({}) was specified.'.format(token)
+            msg = 'The Chantify token specified ({}) is invalid.'\
+                .format(token)
             self.logger.warning(msg)
             raise TypeError(msg)
 
-        # Set Status type
-        self.status = status
-
         return
 
     def send(self, body, title='', notify_type=NotifyType.INFO, **kwargs):
         """
-        Perform PushMe Notification
+        Send our notification
         """
 
+        # prepare our headers
         headers = {
             'User-Agent': self.app_id,
+            'Content-Type': 'application/x-www-form-urlencoded',
         }
 
-        # Prepare our payload
-        params = {
-            'push_key': self.token,
-            'title': title if not self.status
-            else '{} {}'.format(self.asset.ascii(notify_type), title),
-            'content': body,
-            'type': 'markdown'
-            if self.notify_format == NotifyFormat.MARKDOWN else 'text'
+        # Our Message
+        payload = {
+            'text': body
         }
 
-        self.logger.debug('PushMe POST URL: %s (cert_verify=%r)' % (
-            self.notify_url, self.verify_certificate,
-        ))
-        self.logger.debug('PushMe Payload: %s' % str(params))
+        self.logger.debug('Chantify GET URL: %s (cert_verify=%r)' % (
+            self.notify_url, self.verify_certificate))
+        self.logger.debug('Chantify Payload: %s' % str(payload))
 
         # Always call throttle before any remote server i/o is made
         self.throttle()
 
         try:
             r = requests.post(
-                self.notify_url,
-                params=params,
+                self.notify_url.format(token=self.token),
+                data=payload,
                 headers=headers,
                 verify=self.verify_certificate,
                 timeout=self.request_timeout,
             )
             if r.status_code != requests.codes.ok:
                 # We had a problem
                 status_str = \
-                    NotifyPushMe.http_response_code_lookup(r.status_code)
+                    NotifyChantify.http_response_code_lookup(r.status_code)
 
                 self.logger.warning(
-                    'Failed to send PushMe notification:'
+                    'Failed to send Chantify notification: '
                     '{}{}error={}.'.format(
                         status_str,
                         ', ' if status_str else '',
                         r.status_code))
 
                 self.logger.debug('Response Details:\r\n{}'.format(r.content))
 
                 # Return; we're done
                 return False
 
             else:
-                self.logger.info('Sent PushMe notification.')
+                self.logger.info('Sent Chantify notification.')
 
         except requests.RequestException as e:
             self.logger.warning(
-                'A Connection error occurred sending PushMe notification.',
-            )
+                'A Connection error occurred sending Chantify '
+                'notification.')
             self.logger.debug('Socket Exception: %s' % str(e))
 
             # Return; we're done
             return False
 
         return True
 
     def url(self, privacy=False, *args, **kwargs):
         """
         Returns the URL built dynamically based on specified arguments.
         """
 
-        # Define any URL parameters
-        params = {
-            'status': 'yes' if self.status else 'no',
-        }
-
-        # Extend our parameters
-        params.update(self.url_parameters(privacy=privacy, *args, **kwargs))
+        # Prepare our parameters
+        params = self.url_parameters(privacy=privacy, *args, **kwargs)
 
-        # Official URLs are easy to assemble
         return '{schema}://{token}/?{params}'.format(
-            schema=self.protocol,
+            schema=self.secure_protocol,
             token=self.pprint(self.token, privacy, safe=''),
-            params=NotifyPushMe.urlencode(params),
+            params=NotifyChantify.urlencode(params),
         )
 
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
+
+        # parse_url already handles getting the `user` and `password` fields
+        # populated.
         results = NotifyBase.parse_url(url, verify_host=False)
         if not results:
             # We're done early as we couldn't load the results
             return results
 
-        # Store our token using the host
-        results['token'] = NotifyPushMe.unquote(results['host'])
-
-        # The 'token' makes it easier to use yaml configuration
+        # Allow over-ride
         if 'token' in results['qsd'] and len(results['qsd']['token']):
-            results['token'] = NotifyPushMe.unquote(results['qsd']['token'])
+            results['token'] = NotifyChantify.unquote(results['qsd']['token'])
 
-        elif 'push_key' in results['qsd'] and len(results['qsd']['push_key']):
-            # Support 'push_key' if specified
-            results['token'] = NotifyPushMe.unquote(results['qsd']['push_key'])
-
-        # Get status switch
-        results['status'] = \
-            parse_bool(results['qsd'].get('status', True))
+        else:
+            results['token'] = NotifyChantify.unquote(results['host'])
 
         return results
```

### Comparing `apprise-1.7.5/apprise/plugins/NotifyPushSafer.py` & `apprise-1.7.6/apprise/plugins/NotifyPushSafer.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyPushed.py` & `apprise-1.7.6/apprise/plugins/NotifyPushed.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyPushjet.py` & `apprise-1.7.6/apprise/plugins/NotifyPushjet.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyPushover.py` & `apprise-1.7.6/apprise/plugins/NotifyPushover.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyPushy.py` & `apprise-1.7.6/apprise/plugins/NotifyPushy.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyRSyslog.py` & `apprise-1.7.6/apprise/plugins/NotifyRSyslog.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyReddit.py` & `apprise-1.7.6/apprise/plugins/NotifyReddit.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyRevolt.py` & `apprise-1.7.6/apprise/plugins/NotifyRevolt.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyRocketChat.py` & `apprise-1.7.6/apprise/plugins/NotifyRocketChat.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,21 +55,25 @@
 class RocketChatAuthMode:
     """
     The Chat Authentication mode is detected
     """
     # providing a webhook
     WEBHOOK = "webhook"
 
+    # Support token submission
+    TOKEN = "token"
+
     # Providing a username and password (default)
     BASIC = "basic"
 
 
 # Define our authentication modes
 ROCKETCHAT_AUTH_MODES = (
     RocketChatAuthMode.WEBHOOK,
+    RocketChatAuthMode.TOKEN,
     RocketChatAuthMode.BASIC,
 )
 
 
 class NotifyRocketChat(NotifyBase):
     """
     A wrapper for Notify Rocket.Chat Notifications
@@ -103,14 +107,16 @@
     # Default to markdown
     notify_format = NotifyFormat.MARKDOWN
 
     # Define object templates
     templates = (
         '{schema}://{user}:{password}@{host}:{port}/{targets}',
         '{schema}://{user}:{password}@{host}/{targets}',
+        '{schema}://{user}:{token}@{host}:{port}/{targets}',
+        '{schema}://{user}:{token}@{host}/{targets}',
         '{schema}://{webhook}@{host}',
         '{schema}://{webhook}@{host}:{port}',
         '{schema}://{webhook}@{host}/{targets}',
         '{schema}://{webhook}@{host}:{port}/{targets}',
     )
 
     # Define our template arguments
@@ -131,14 +137,19 @@
             'type': 'string',
         },
         'password': {
             'name': _('Password'),
             'type': 'string',
             'private': True,
         },
+        'token': {
+            'name': _('API Token'),
+            'map_to': 'password',
+            'private': True,
+        },
         'webhook': {
             'name': _('Webhook'),
             'type': 'string',
         },
         'target_channel': {
             'name': _('Target Channel'),
             'type': 'string',
@@ -226,29 +237,43 @@
             raise TypeError(msg)
 
         # Detect our mode if it wasn't specified
         if not self.mode:
             if self.webhook is not None:
                 # Just a username was specified, we treat this as a webhook
                 self.mode = RocketChatAuthMode.WEBHOOK
+            elif self.password and len(self.password) > 32:
+                self.mode = RocketChatAuthMode.TOKEN
             else:
                 self.mode = RocketChatAuthMode.BASIC
 
-        if self.mode == RocketChatAuthMode.BASIC \
+            self.logger.debug(
+                "Auto-Detected Rocketchat Auth Mode: %s", self.mode)
+
+        if self.mode in (RocketChatAuthMode.BASIC, RocketChatAuthMode.TOKEN) \
                 and not (self.user and self.password):
             # Username & Password is required for Rocket Chat to work
-            msg = 'No Rocket.Chat user/pass combo was specified.'
+            msg = 'No Rocket.Chat {} was specified.'.format(
+                'user/pass combo' if self.mode == RocketChatAuthMode.BASIC else
+                'user/apikey')
             self.logger.warning(msg)
             raise TypeError(msg)
 
         elif self.mode == RocketChatAuthMode.WEBHOOK and not self.webhook:
             msg = 'No Rocket.Chat Incoming Webhook was specified.'
             self.logger.warning(msg)
             raise TypeError(msg)
 
+        if self.mode == RocketChatAuthMode.TOKEN:
+            # Set our headers for further communication
+            self.headers.update({
+                'X-User-Id': self.user,
+                'X-Auth-Token': self.password,
+            })
+
         # Validate recipients and drop bad ones:
         for recipient in parse_list(targets):
             result = IS_CHANNEL.match(recipient)
             if result:
                 # store valid device
                 self.channels.append(result.group('name'))
                 continue
@@ -305,20 +330,21 @@
             'mode': self.mode,
         }
 
         # Extend our parameters
         params.update(self.url_parameters(privacy=privacy, *args, **kwargs))
 
         # Determine Authentication
-        if self.mode == RocketChatAuthMode.BASIC:
+        if self.mode in (RocketChatAuthMode.BASIC, RocketChatAuthMode.TOKEN):
             auth = '{user}:{password}@'.format(
                 user=NotifyRocketChat.quote(self.user, safe=''),
                 password=self.pprint(
                     self.password, privacy, mode=PrivacyMode.Secret, safe=''),
             )
+
         else:
             auth = '{user}{webhook}@'.format(
                 user='{}:'.format(NotifyRocketChat.quote(self.user, safe=''))
                 if self.user else '',
                 webhook=self.pprint(self.webhook, privacy,
                                     mode=PrivacyMode.Secret, safe=''),
             )
@@ -355,16 +381,19 @@
         """
         wrapper to _send since we can alert more then one channel
         """
 
         # Call the _send_ function applicable to whatever mode we're in
         # - calls _send_webhook_notification if the mode variable is set
         # - calls _send_basic_notification if the mode variable is not set
-        return getattr(self, '_send_{}_notification'.format(self.mode))(
-            body=body, title=title, notify_type=notify_type, **kwargs)
+        return getattr(self, '_send_{}_notification'.format(
+            RocketChatAuthMode.WEBHOOK
+            if self.mode == RocketChatAuthMode.WEBHOOK
+            else RocketChatAuthMode.BASIC))(
+                body=body, title=title, notify_type=notify_type, **kwargs)
 
     def _send_webhook_notification(self, body, title='',
                                    notify_type=NotifyType.INFO, **kwargs):
         """
         Sends a webhook notification
         """
 
@@ -408,15 +437,15 @@
                                  notify_type=NotifyType.INFO, **kwargs):
         """
         Authenticates with the server using a user/pass combo for
         notifications.
         """
         # Track whether we authenticated okay
 
-        if not self.login():
+        if self.mode == RocketChatAuthMode.BASIC and not self.login():
             return False
 
         # prepare JSON Object
         _payload = self._payload(body, title, notify_type)
 
         # Initiaize our error tracking
         has_error = False
@@ -428,38 +457,35 @@
         # Create a copy of our channels to notify against
         payload = _payload.copy()
         while len(channels) > 0:
             # Get Channel
             channel = channels.pop(0)
             payload['channel'] = channel
 
-            if not self._send(
-                    payload, notify_type=notify_type, headers=self.headers,
-                    **kwargs):
+            if not self._send(payload, notify_type=notify_type, **kwargs):
 
                 # toggle flag
                 has_error = True
 
         # Create a copy of our room id's to notify against
         rooms = list(self.rooms)
         payload = _payload.copy()
         while len(rooms):
             # Get Room
             room = rooms.pop(0)
             payload['roomId'] = room
 
-            if not self._send(
-                    payload, notify_type=notify_type, headers=self.headers,
-                    **kwargs):
+            if not self._send(payload, notify_type=notify_type, **kwargs):
 
                 # toggle flag
                 has_error = True
 
-        # logout
-        self.logout()
+        if self.mode == RocketChatAuthMode.BASIC:
+            # logout
+            self.logout()
 
         return not has_error
 
     def _payload(self, body, title='', notify_type=NotifyType.INFO):
         """
         Prepares a payload object
         """
@@ -472,25 +498,28 @@
         image_url = self.image_url(notify_type)
         if self.avatar and image_url:
             payload['avatar'] = image_url
 
         return payload
 
     def _send(self, payload, notify_type, path='api/v1/chat.postMessage',
-              headers={}, **kwargs):
+              **kwargs):
         """
         Perform Notify Rocket.Chat Notification
         """
 
         api_url = '{}/{}'.format(self.api_url, path)
 
         self.logger.debug('Rocket.Chat POST URL: %s (cert_verify=%r)' % (
             api_url, self.verify_certificate))
         self.logger.debug('Rocket.Chat Payload: %s' % str(payload))
 
+        # Copy our existing headers
+        headers = self.headers.copy()
+
         # Apply minimum headers
         headers.update({
             'User-Agent': self.app_id,
             'Content-Type': 'application/json',
         })
 
         # Always call throttle before any remote server i/o is made
```

### Comparing `apprise-1.7.5/apprise/plugins/NotifyRyver.py` & `apprise-1.7.6/apprise/plugins/NotifyRyver.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifySES.py` & `apprise-1.7.6/apprise/plugins/NotifySES.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifySMSEagle.py` & `apprise-1.7.6/apprise/plugins/NotifySMSEagle.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifySMSManager.py` & `apprise-1.7.6/apprise/plugins/NotifySMSManager.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifySMTP2Go.py` & `apprise-1.7.6/apprise/plugins/NotifySMTP2Go.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifySNS.py` & `apprise-1.7.6/apprise/plugins/NotifySNS.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifySendGrid.py` & `apprise-1.7.6/apprise/plugins/NotifySendGrid.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyServerChan.py` & `apprise-1.7.6/apprise/plugins/NotifyServerChan.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifySignalAPI.py` & `apprise-1.7.6/apprise/plugins/NotifySignalAPI.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifySimplePush.py` & `apprise-1.7.6/apprise/plugins/NotifySimplePush.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifySinch.py` & `apprise-1.7.6/apprise/plugins/NotifySinch.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifySlack.py` & `apprise-1.7.6/apprise/plugins/NotifySlack.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifySparkPost.py` & `apprise-1.7.6/apprise/plugins/NotifySparkPost.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyStreamlabs.py` & `apprise-1.7.6/apprise/plugins/NotifyStreamlabs.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifySynology.py` & `apprise-1.7.6/apprise/plugins/NotifySynology.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifySyslog.py` & `apprise-1.7.6/apprise/plugins/NotifySyslog.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyTechulusPush.py` & `apprise-1.7.6/apprise/plugins/NotifyTechulusPush.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyTelegram.py` & `apprise-1.7.6/apprise/plugins/NotifyTelegram.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,14 +78,42 @@
 IS_CHAT_ID_RE = re.compile(
     r'^((?P<idno>-?[0-9]{1,32})|(@|%40)?(?P<name>[a-z_-][a-z0-9_-]+))'
     r'((:|%3A)(?P<topic>[0-9]+))?$',
     re.IGNORECASE,
 )
 
 
+class TelegramMarkdownVersion:
+    """
+    Telegram Markdown Version
+    """
+    # Classic (Original Telegram Markdown)
+    ONE = 'MARKDOWN'
+
+    # Supports strikethrough and many other items
+    TWO = 'MarkdownV2'
+
+
+TELEGRAM_MARKDOWN_VERSION_MAP = {
+    # v1
+    "v1": TelegramMarkdownVersion.ONE,
+    "1": TelegramMarkdownVersion.ONE,
+    # v2
+    "v2": TelegramMarkdownVersion.TWO,
+    "2": TelegramMarkdownVersion.TWO,
+    "default": TelegramMarkdownVersion.TWO,
+}
+
+TELEGRAM_MARKDOWN_VERSIONS = {
+    # Note: This also acts as a reverse lookup mapping
+    TelegramMarkdownVersion.ONE: 'v1',
+    TelegramMarkdownVersion.TWO: 'v2',
+}
+
+
 class TelegramContentPlacement:
     """
     The Telegram Content Placement
     """
     # Before Attachments
     BEFORE = "before"
     # After Attachments
@@ -329,42 +357,59 @@
             'type': 'bool',
             'default': False,
         },
         'topic': {
             'name': _('Topic Thread ID'),
             'type': 'int',
         },
+        'mdv': {
+            'name': _('Markdown Version'),
+            'type': 'choice:string',
+            'values': ('v1', 'v2'),
+            'default': 'v2',
+        },
         'to': {
             'alias_of': 'targets',
         },
         'content': {
             'name': _('Content Placement'),
             'type': 'choice:string',
             'values': TELEGRAM_CONTENT_PLACEMENT,
             'default': TelegramContentPlacement.BEFORE,
         },
     })
 
     def __init__(self, bot_token, targets, detect_owner=True,
                  include_image=False, silent=None, preview=None, topic=None,
-                 content=None, **kwargs):
+                 content=None, mdv=None, **kwargs):
         """
         Initialize Telegram Object
         """
         super().__init__(**kwargs)
 
         self.bot_token = validate_regex(
             bot_token, *self.template_tokens['bot_token']['regex'],
             fmt='{key}')
         if not self.bot_token:
             err = 'The Telegram Bot Token specified ({}) is invalid.'.format(
                 bot_token)
             self.logger.warning(err)
             raise TypeError(err)
 
+        # Get our Markdown Version
+        self.markdown_ver = \
+            TELEGRAM_MARKDOWN_VERSION_MAP[NotifyTelegram.
+                                          template_args['mdv']['default']] \
+            if mdv is None else \
+            next((
+                v for k, v in TELEGRAM_MARKDOWN_VERSION_MAP.items()
+                if str(mdv).lower().startswith(k)),
+                TELEGRAM_MARKDOWN_VERSION_MAP[NotifyTelegram.
+                                              template_args['mdv']['default']])
+
         # Define whether or not we should make audible alarms
         self.silent = self.template_args['silent']['default'] \
             if silent is None else bool(silent)
 
         # Define whether or not we should display a web page preview
         self.preview = self.template_args['preview']['default'] \
             if preview is None else bool(preview)
@@ -713,16 +758,15 @@
             'disable_notification': self.silent,
             # Display Web Page Preview (if possible)
             'disable_web_page_preview': not self.preview,
         }
 
         # Prepare Message Body
         if self.notify_format == NotifyFormat.MARKDOWN:
-            _payload['parse_mode'] = 'MARKDOWN'
-
+            _payload['parse_mode'] = self.markdown_ver
             _payload['text'] = body
 
         else:  # HTML
 
             # Use Telegram's HTML mode
             _payload['parse_mode'] = 'HTML'
             for r, v, m in self.__telegram_escape_html_entries:
@@ -882,14 +926,15 @@
         # Define any URL parameters
         params = {
             'image': self.include_image,
             'detect': 'yes' if self.detect_owner else 'no',
             'silent': 'yes' if self.silent else 'no',
             'preview': 'yes' if self.preview else 'no',
             'content': self.content,
+            'mdv': TELEGRAM_MARKDOWN_VERSIONS[self.markdown_ver],
         }
 
         if self.topic:
             params['topic'] = self.topic
 
         # Extend our parameters
         params.update(self.url_parameters(privacy=privacy, *args, **kwargs))
@@ -986,14 +1031,18 @@
         if 'to' in results['qsd'] and len(results['qsd']['to']):
             results['targets'] += \
                 NotifyTelegram.parse_list(results['qsd']['to'])
 
         # Store our bot token
         results['bot_token'] = bot_token
 
+        # Support Markdown Version
+        if 'mdv' in results['qsd'] and len(results['qsd']['mdv']):
+            results['mdv'] = results['qsd']['mdv']
+
         # Support Thread Topic
         if 'topic' in results['qsd'] and len(results['qsd']['topic']):
             results['topic'] = results['qsd']['topic']
 
         # Silent (Sends the message Silently); users will receive
         # notification with no sound.
         results['silent'] = \
```

### Comparing `apprise-1.7.5/apprise/plugins/NotifyThreema.py` & `apprise-1.7.6/apprise/plugins/NotifyThreema.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyTwilio.py` & `apprise-1.7.6/apprise/plugins/NotifyTwilio.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyTwist.py` & `apprise-1.7.6/apprise/plugins/NotifyTwist.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyTwitter.py` & `apprise-1.7.6/apprise/plugins/NotifyTwitter.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyVoipms.py` & `apprise-1.7.6/apprise/plugins/NotifyVoipms.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyVonage.py` & `apprise-1.7.6/apprise/plugins/NotifyVonage.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyWeComBot.py` & `apprise-1.7.6/apprise/plugins/NotifyWeComBot.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyWebexTeams.py` & `apprise-1.7.6/apprise/plugins/NotifyWebexTeams.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyWhatsApp.py` & `apprise-1.7.6/apprise/plugins/NotifyWhatsApp.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyWindows.py` & `apprise-1.7.6/apprise/plugins/NotifyWindows.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyXBMC.py` & `apprise-1.7.6/apprise/plugins/NotifyXBMC.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyXML.py` & `apprise-1.7.6/apprise/plugins/NotifyXML.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/plugins/NotifyZulip.py` & `apprise-1.7.6/apprise/plugins/NotifyZulip.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,17 @@
     })
 
     # Define our template arguments
     template_args = dict(NotifyBase.template_args, **{
         'to': {
             'alias_of': 'targets',
         },
+        'token': {
+            'alias_of': 'token',
+        },
     })
 
     # The default hostname to append to a defined organization
     # if one isn't defined in the apprise url
     default_hostname = 'zulipchat.com'
 
     # The default stream to notify if no targets are specified
@@ -373,29 +376,32 @@
         if not results:
             # We're done early as we couldn't load the results
             return results
 
         # The botname
         results['botname'] = NotifyZulip.unquote(results['user'])
 
-        # The first token is stored in the hostname
+        # The organization is stored in the hostname
         results['organization'] = NotifyZulip.unquote(results['host'])
 
-        # Now fetch the remaining tokens
-        try:
-            results['token'] = \
-                NotifyZulip.split_path(results['fullpath'])[0]
+        # Store our targets
+        results['targets'] = NotifyZulip.split_path(results['fullpath'])
 
-        except IndexError:
+        if 'token' in results['qsd'] and len(results['qsd']['token']):
+            # Store our token if specified
+            results['token'] = NotifyZulip.unquote(results['qsd']['token'])
+
+        elif results['targets']:
+            # First item is the token
+            results['token'] = results['targets'].pop(0)
+
+        else:
             # no token
             results['token'] = None
 
-        # Get unquoted entries
-        results['targets'] = NotifyZulip.split_path(results['fullpath'])[1:]
-
         # Support the 'to' variable so that we can support rooms this way too
         # The 'to' makes it easier to use yaml configuration
         if 'to' in results['qsd'] and len(results['qsd']['to']):
             results['targets'] += [x for x in filter(
                 bool, TARGET_LIST_DELIM.split(
                     NotifyZulip.unquote(results['qsd']['to'])))]
```

### Comparing `apprise-1.7.5/apprise/plugins/__init__.py` & `apprise-1.7.6/apprise/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise/utils.py` & `apprise-1.7.6/apprise/utils.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/apprise.egg-info/PKG-INFO` & `apprise-1.7.6/apprise.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: apprise
-Version: 1.7.5
+Version: 1.7.6
 Summary: Push Notifications that work with just about every platform!
 Home-page: https://github.com/caronc/apprise
 Author: Chris Caron
 Author-email: lead2gold@gmail.com
 License: BSD
-Keywords: Alerts Apprise API Automated Packet Reporting System AWS Boxcar BulkSMS BulkVS Burst SMS Chat CLI ClickSend D7Networks Dapnet DBus DingTalk Discord Email Emby Enigma2 Faast FCM Flock Form Free Mobile Gnome Google Chat Gotify Growl Guilded Home Assistant httpSMS IFTTT Join JSON Kavenegar KODI Kumulos LaMetric Line LunaSea MacOSX Mailgun Mastodon Matrix Mattermost MessageBird Microsoft Misskey MQTT MSG91 MSTeams Nextcloud NextcloudTalk Notica Notifiarr Notifico Ntfy Office365 OneSignal Opsgenie PagerDuty PagerTree ParsePlatform PopcornNotify Prowl PushBullet Pushed Pushjet PushMe Push Notifications Pushover PushSafer Pushy PushDeer Reddit Revolt Rocket.Chat RSyslog Ryver SendGrid ServerChan SES Signal SimplePush Sinch Slack SMSEagle SMS Manager SMTP2Go SNS SparkPost Streamlabs Stride Synology Chat Syslog Techulus Telegram Threema Gateway Twilio Twist Twitter Voipms Vonage Webex WeCom Bot WhatsApp Windows XBMC XML Zulip
+Keywords: Alerts Apprise API Automated Packet Reporting System AWS Boxcar BulkSMS BulkVS Burst SMS Chantify Chat CLI ClickSend D7Networks Dapnet DBus DingTalk Discord Email Emby Enigma2 FCM Feishu Flock Form Free Mobile Gnome Google Chat Gotify Growl Guilded Home Assistant httpSMS IFTTT Join JSON Kavenegar KODI Kumulos LaMetric Line LunaSea MacOSX Mailgun Mastodon Matrix Mattermost MessageBird Microsoft Misskey MQTT MSG91 MSTeams Nextcloud NextcloudTalk Notica Notifiarr Notifico Ntfy Office365 OneSignal Opsgenie PagerDuty PagerTree ParsePlatform PopcornNotify Prowl PushBullet Pushed Pushjet PushMe Push Notifications Pushover PushSafer Pushy PushDeer Reddit Revolt Rocket.Chat RSyslog Ryver SendGrid ServerChan SES Signal SimplePush Sinch Slack SMSEagle SMS Manager SMTP2Go SNS SparkPost Streamlabs Stride Synology Chat Syslog Techulus Telegram Threema Gateway Twilio Twist Twitter Voipms Vonage Webex WeCom Bot WhatsApp Windows XBMC XML Zulip
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -87,19 +88,20 @@
 
 | Notification Service | Service ID | Default Port | Example Syntax |
 | -------------------- | ---------- | ------------ | -------------- |
 | [Apprise API](https://github.com/caronc/apprise/wiki/Notify_apprise_api)  | apprise:// or apprises:// | (TCP) 80 or 443 | apprise://hostname/Token
 | [AWS SES](https://github.com/caronc/apprise/wiki/Notify_ses)  | ses://   | (TCP) 443   | ses://user@domain/AccessKeyID/AccessSecretKey/RegionName<br/>ses://user@domain/AccessKeyID/AccessSecretKey/RegionName/email1/email2/emailN
 | [Bark](https://github.com/caronc/apprise/wiki/Notify_bark)  | bark://   | (TCP) 80 or 443   | bark://hostname<br />bark://hostname/device_key<br />bark://hostname/device_key1/device_key2/device_keyN<br/>barks://hostname<br />barks://hostname/device_key<br />barks://hostname/device_key1/device_key2/device_keyN
 | [Boxcar](https://github.com/caronc/apprise/wiki/Notify_boxcar)  | boxcar://   | (TCP) 443   | boxcar://hostname<br />boxcar://hostname/@tag<br/>boxcar://hostname/device_token<br />boxcar://hostname/device_token1/device_token2/device_tokenN<br />boxcar://hostname/@tag/@tag2/device_token
+| [Chantify](https://github.com/caronc/apprise/wiki/Notify_chantify) | chantify://    | (TCP) 443    | chantify://token
 | [Discord](https://github.com/caronc/apprise/wiki/Notify_discord)  | discord://   | (TCP) 443   | discord://webhook_id/webhook_token<br />discord://avatar@webhook_id/webhook_token
 | [Emby](https://github.com/caronc/apprise/wiki/Notify_emby)  | emby:// or embys:// | (TCP) 8096 | emby://user@hostname/<br />emby://user:password@hostname
 | [Enigma2](https://github.com/caronc/apprise/wiki/Notify_enigma2)  | enigma2:// or enigma2s:// | (TCP) 80 or 443 | enigma2://hostname
-| [Faast](https://github.com/caronc/apprise/wiki/Notify_faast) | faast://    | (TCP) 443    | faast://authorizationtoken
 | [FCM](https://github.com/caronc/apprise/wiki/Notify_fcm) | fcm://    | (TCP) 443    | fcm://project@apikey/DEVICE_ID<br />fcm://project@apikey/#TOPIC<br/>fcm://project@apikey/DEVICE_ID1/#topic1/#topic2/DEVICE_ID2/
+| [Feishu](https://github.com/caronc/apprise/wiki/Notify_feishu) | feishu://    | (TCP) 443    | feishu://token
 | [Flock](https://github.com/caronc/apprise/wiki/Notify_flock) | flock://    | (TCP) 443    | flock://token<br/>flock://botname@token<br/>flock://app_token/u:userid<br/>flock://app_token/g:channel_id<br/>flock://app_token/u:userid/g:channel_id
 | [Google Chat](https://github.com/caronc/apprise/wiki/Notify_googlechat) | gchat://    | (TCP) 443    | gchat://workspace/key/token
 | [Gotify](https://github.com/caronc/apprise/wiki/Notify_gotify) | gotify:// or gotifys://   | (TCP) 80 or 443    | gotify://hostname/token<br />gotifys://hostname/token?priority=high
 | [Growl](https://github.com/caronc/apprise/wiki/Notify_growl)  | growl://   | (UDP) 23053   | growl://hostname<br />growl://hostname:portno<br />growl://password@hostname<br />growl://password@hostname:port</br>**Note**: you can also use the get parameter _version_ which can allow the growl request to behave using the older v1.x protocol. An example would look like: growl://hostname?version=1
 | [Guilded](https://github.com/caronc/apprise/wiki/Notify_guilded)  | guilded://   | (TCP) 443   | guilded://webhook_id/webhook_token<br />guilded://avatar@webhook_id/webhook_token
 | [Home Assistant](https://github.com/caronc/apprise/wiki/Notify_homeassistant)       | hassio:// or hassios://   | (TCP) 8123 or 443 | hassio://hostname/accesstoken<br />hassio://user@hostname/accesstoken<br />hassio://user:password@hostname:port/accesstoken<br />hassio://hostname/optional/path/accesstoken
 | [IFTTT](https://github.com/caronc/apprise/wiki/Notify_ifttt) | ifttt://    | (TCP) 443    | ifttt://webhooksID/Event<br />ifttt://webhooksID/Event1/Event2/EventN<br/>ifttt://webhooksID/Event1/?+Key=Value<br/>ifttt://webhooksID/Event1/?-Key=value1
```

### Comparing `apprise-1.7.5/apprise.egg-info/SOURCES.txt` & `apprise-1.7.6/apprise.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -81,24 +81,25 @@
 apprise/plugins/NotifyBark.py
 apprise/plugins/NotifyBase.py
 apprise/plugins/NotifyBase.pyi
 apprise/plugins/NotifyBoxcar.py
 apprise/plugins/NotifyBulkSMS.py
 apprise/plugins/NotifyBulkVS.py
 apprise/plugins/NotifyBurstSMS.py
+apprise/plugins/NotifyChantify.py
 apprise/plugins/NotifyClickSend.py
 apprise/plugins/NotifyD7Networks.py
 apprise/plugins/NotifyDBus.py
 apprise/plugins/NotifyDapnet.py
 apprise/plugins/NotifyDingTalk.py
 apprise/plugins/NotifyDiscord.py
 apprise/plugins/NotifyEmail.py
 apprise/plugins/NotifyEmby.py
 apprise/plugins/NotifyEnigma2.py
-apprise/plugins/NotifyFaast.py
+apprise/plugins/NotifyFeishu.py
 apprise/plugins/NotifyFlock.py
 apprise/plugins/NotifyForm.py
 apprise/plugins/NotifyFreeMobile.py
 apprise/plugins/NotifyGnome.py
 apprise/plugins/NotifyGoogleChat.py
 apprise/plugins/NotifyGotify.py
 apprise/plugins/NotifyGrowl.py
@@ -220,27 +221,28 @@
 test/test_plugin_apprise_api.py
 test/test_plugin_aprs.py
 test/test_plugin_bark.py
 test/test_plugin_boxcar.py
 test/test_plugin_bulksms.py
 test/test_plugin_bulkvs.py
 test/test_plugin_burstsms.py
+test/test_plugin_chantify.py
 test/test_plugin_clicksend.py
 test/test_plugin_custom_form.py
 test/test_plugin_custom_json.py
 test/test_plugin_custom_xml.py
 test/test_plugin_d7networks.py
 test/test_plugin_dapnet.py
 test/test_plugin_dingtalk.py
 test/test_plugin_discord.py
 test/test_plugin_email.py
 test/test_plugin_emby.py
 test/test_plugin_enigma2.py
-test/test_plugin_faast.py
 test/test_plugin_fcm.py
+test/test_plugin_feishu.py
 test/test_plugin_flock.py
 test/test_plugin_freemobile.py
 test/test_plugin_glib.py
 test/test_plugin_gnome.py
 test/test_plugin_google_chat.py
 test/test_plugin_gotify.py
 test/test_plugin_growl.py
```

### Comparing `apprise-1.7.5/packaging/README.md` & `apprise-1.7.6/packaging/README.md`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/packaging/man/apprise.1` & `apprise-1.7.6/packaging/man/apprise.1`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/packaging/man/apprise.1.html` & `apprise-1.7.6/packaging/man/apprise.1.html`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/packaging/man/apprise.md` & `apprise-1.7.6/packaging/man/apprise.md`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/packaging/redhat/apprise-click67-support.patch` & `apprise-1.7.6/packaging/redhat/apprise-click67-support.patch`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/packaging/redhat/apprise-no-macosx-testing.patch` & `apprise-1.7.6/packaging/redhat/apprise-no-macosx-testing.patch`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/packaging/redhat/apprise-pytest-session_mocker-removal.patch` & `apprise-1.7.6/packaging/redhat/apprise-pytest-session_mocker-removal.patch`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/packaging/redhat/python-apprise.spec` & `apprise-1.7.6/packaging/redhat/python-apprise.spec`

 * *Files 2% similar despite different names*

```diff
@@ -36,29 +36,29 @@
 
 %global common_description %{expand: \
 Apprise is a Python package for simplifying access to all of the different
 notification services that are out there. Apprise opens the door and makes
 it easy to access:
 
 Apprise API, APRS, AWS SES, AWS SNS, Bark, Boxcar, Burst SMS, BulkSMS, BulkVS,
-ClickSend, DAPNET, DingTalk, Discord, E-Mail, Emby, Faast, FCM, Flock,
-Free Mobile, Google Chat, Gotify, Growl, Guilded, Home Assistant, httpSMS,
-IFTTT, Join, Kavenegar, KODI, Kumulos, LaMetric, Line, LunaSea, MacOSX,
-Mailgun, Mastodon, Mattermost,Matrix, MessageBird, Microsoft Windows,
+Chantify, ClickSend, DAPNET, DingTalk, Discord, E-Mail, Emby, FCM, Feishu,
+Flock, Free Mobile, Google Chat, Gotify, Growl, Guilded, Home Assistant,
+httpSMS, IFTTT, Join, Kavenegar, KODI, Kumulos, LaMetric, Line, LunaSea,
+MacOSX, Mailgun, Mastodon, Mattermost,Matrix, MessageBird, Microsoft Windows,
 Microsoft Teams, Misskey, MQTT, MSG91, MyAndroid, Nexmo, Nextcloud,
 NextcloudTalk, Notica, Notifiarr, Notifico, ntfy, Office365, OneSignal,
 Opsgenie, PagerDuty, PagerTree, ParsePlatform, PopcornNotify, Prowl, Pushalot,
 PushBullet, Pushjet, PushMe, Pushover, PushSafer, Pushy, PushDeer, Revolt,
 Reddit, Rocket.Chat, RSyslog, SendGrid, ServerChan, Signal, SimplePush, Sinch,
 Slack, SMSEagle, SMS Manager, SMTP2Go, SparkPost, Super Toasty, Streamlabs,
 Stride, Synology Chat, Syslog, Techulus Push, Telegram, Threema Gateway, Twilio,
 Twitter, Twist, XBMC, Voipms, Vonage, WeCom Bot, WhatsApp, Webex Teams}
 
 Name:           python-%{pypi_name}
-Version:        1.7.5
+Version:        1.7.6
 Release:        1%{?dist}
 Summary:        A simple wrapper to many popular notification services used today
 License:        BSD
 URL:            https://github.com/caronc/%{pypi_name}
 Source0:        %{url}/archive/v%{version}/%{pypi_name}-%{version}.tar.gz
 
 # RHEL/Rocky 8 ship with Click v6.7 which does not support the .stdout
@@ -191,14 +191,17 @@
 
 %files -n %{pypi_name}
 %{_bindir}/%{pypi_name}
 %{_mandir}/man1/%{pypi_name}.1*
 %{python3_sitelib}/%{pypi_name}/cli.*
 
 %changelog
+* Sat Apr 13 2024 Chris Caron <lead2gold@gmail.com> - 1.7.6
+- Updated to v1.7.6
+
 * Sat Mar 30 2024 Chris Caron <lead2gold@gmail.com> - 1.7.5
 - Updated to v1.7.5
 
 * Sat Mar  9 2024 Chris Caron <lead2gold@gmail.com> - 1.7.4
 - Updated to v1.7.4
 
 * Sun Mar  3 2024 Chris Caron <lead2gold@gmail.com> - 1.7.3
```

### Comparing `apprise-1.7.5/setup.cfg` & `apprise-1.7.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/setup.py` & `apprise-1.7.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 else:
     # Load our CLI
     console_scripts = ['apprise = apprise.cli:main']
 
 setup(
     name='apprise',
-    version='1.7.5',
+    version='1.7.6',
     description='Push Notifications that work with just about every platform!',
     license='BSD',
     long_description=open('README.md', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     cmdclass=cmdclass,
     url='https://github.com/caronc/apprise',
     keywords=' '.join(re.split(r'\s+', open('KEYWORDS').read())),
@@ -96,14 +96,15 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'License :: OSI Approved :: BSD License',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Software Development :: Libraries :: Application Frameworks',
     ],
     entry_points={'console_scripts': console_scripts},
```

### Comparing `apprise-1.7.5/test/conftest.py` & `apprise-1.7.6/test/conftest.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/helpers/__init__.py` & `apprise-1.7.6/test/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/helpers/asyncio.py` & `apprise-1.7.6/test/helpers/asyncio.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/helpers/module.py` & `apprise-1.7.6/test/helpers/module.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/helpers/rest.py` & `apprise-1.7.6/test/helpers/rest.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_api.py` & `apprise-1.7.6/test/test_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     asset = AppriseAsset(theme='default')
 
     # We can load the device using our asset
     a = Apprise(asset=asset)
 
     # We can load our servers up front as well
     servers = [
-        'faast://abcdefghijklmnop-abcdefg',
+        'json://myhost',
         'kodi://kodi.server.local',
     ]
 
     a = Apprise(servers=servers)
 
     # 2 servers loaded
     assert len(a) == 2
```

### Comparing `apprise-1.7.5/test/test_apprise_attachments.py` & `apprise-1.7.6/test/test_apprise_attachments.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,18 +23,22 @@
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 import pytest
+import json
+import requests
+from unittest import mock
 from os.path import getsize
 from os.path import join
 from os.path import dirname
 from inspect import cleandoc
+from apprise.Apprise import Apprise
 from apprise.AttachmentManager import AttachmentManager
 from apprise.AppriseAttachment import AppriseAttachment
 from apprise.AppriseAsset import AppriseAsset
 from apprise.attachment.AttachBase import AttachBase
 from apprise.common import ContentLocation
 
 # Disable logging for a cleaner testing output
@@ -257,14 +261,67 @@
     # length will return 0
     assert len(aa[0]) == 0
 
     # Total length will also return 0
     assert aa.size() == 0
 
 
+@mock.patch('requests.get')
+def test_apprise_attachment_truncate(mock_get):
+    """
+    API: AppriseAttachment when truncation in place
+
+    """
+
+    # Prepare our response
+    response = requests.Request()
+    response.status_code = requests.codes.ok
+
+    # Prepare Mock
+    mock_get.return_value = response
+
+    # our Apprise Object
+    ap_obj = Apprise()
+
+    # Add ourselves an object set to truncate
+    ap_obj.add('json://localhost/?method=GET&overflow=truncate')
+
+    # Add ourselves a second object without truncate
+    ap_obj.add('json://localhost/?method=GET&overflow=upstream')
+
+    # Create ourselves an attachment object
+    aa = AppriseAttachment()
+
+    # There are no attachents loaded
+    assert len(aa) == 0
+
+    # Object can be directly checked as a boolean; response is False
+    # when there are no entries loaded
+    assert not aa
+
+    # Add 2 attachments
+    assert aa.add(join(TEST_VAR_DIR, 'apprise-test.gif'))
+    assert aa.add(join(TEST_VAR_DIR, 'apprise-test.png'))
+
+    assert mock_get.call_count == 0
+    assert ap_obj.notify(body='body', title='title', attach=aa)
+
+    assert mock_get.call_count == 2
+
+    # Our first item was truncated, so only 1 attachment
+    details = mock_get.call_args_list[0]
+    dataset = json.loads(details[1]['data'])
+    assert len(dataset['attachments']) == 1
+
+    # Our second item was not truncated, so all attachments
+    details = mock_get.call_args_list[1]
+    dataset = json.loads(details[1]['data'])
+    assert len(dataset['attachments']) == 2
+
+
 def test_apprise_attachment_instantiate():
     """
     API: AppriseAttachment.instantiate()
 
     """
     assert AppriseAttachment.instantiate(
         'file://?', suppress_exceptions=True) is None
```

### Comparing `apprise-1.7.5/test/test_apprise_cli.py` & `apprise-1.7.6/test/test_apprise_cli.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_apprise_config.py` & `apprise-1.7.6/test/test_apprise_config.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_apprise_emojis.py` & `apprise-1.7.6/test/test_apprise_emojis.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_apprise_pickle.py` & `apprise-1.7.6/test/test_apprise_pickle.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_apprise_translations.py` & `apprise-1.7.6/test/test_apprise_translations.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_apprise_utils.py` & `apprise-1.7.6/test/test_apprise_utils.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_asyncio.py` & `apprise-1.7.6/test/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_attach_base.py` & `apprise-1.7.6/test/test_attach_base.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_attach_file.py` & `apprise-1.7.6/test/test_attach_file.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_attach_http.py` & `apprise-1.7.6/test/test_attach_http.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_config_base.py` & `apprise-1.7.6/test/test_config_base.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_config_file.py` & `apprise-1.7.6/test/test_config_file.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_config_http.py` & `apprise-1.7.6/test/test_config_http.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_config_memory.py` & `apprise-1.7.6/test/test_config_memory.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_conversion.py` & `apprise-1.7.6/test/test_conversion.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_decorator_notify.py` & `apprise-1.7.6/test/test_decorator_notify.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_escapes.py` & `apprise-1.7.6/test/test_escapes.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_logger.py` & `apprise-1.7.6/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_notification_manager.py` & `apprise-1.7.6/test/test_notification_manager.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_notify_base.py` & `apprise-1.7.6/test/test_notify_base.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_apprise_api.py` & `apprise-1.7.6/test/test_plugin_apprise_api.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_aprs.py` & `apprise-1.7.6/test/test_plugin_aprs.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,30 @@
         "aprs://DF1JSL-15:12345@DF1ABC")
     assert isinstance(instance, NotifyAprs)
     assert instance.url(privacy=True).startswith(
         'aprs://DF1JSL-15:****@D...C?')
     assert instance.notify('test') is True
 
     instance = apprise.Apprise.instantiate(
+        "aprs://DF1JSL-15:12345@DF1ABC?delay=3.0")
+    assert isinstance(instance, NotifyAprs)
+    instance = apprise.Apprise.instantiate(
+        "aprs://DF1JSL-15:12345@DF1ABC?delay=2")
+    assert isinstance(instance, NotifyAprs)
+    instance = apprise.Apprise.instantiate(
+        "aprs://DF1JSL-15:12345@DF1ABC?delay=-3.0")
+    assert instance is None
+    instance = apprise.Apprise.instantiate(
+        "aprs://DF1JSL-15:12345@DF1ABC?delay=40.0")
+    assert instance is None
+    instance = apprise.Apprise.instantiate(
+        "aprs://DF1JSL-15:12345@DF1ABC?delay=invalid")
+    assert instance is None
+
+    instance = apprise.Apprise.instantiate(
         "aprs://DF1JSL-15:12345@DF1ABC/DF1DEF")
     assert isinstance(instance, NotifyAprs)
     assert instance.url(privacy=True).startswith(
         'aprs://DF1JSL-15:****@D...C/D...F?')
     assert instance.notify('test') is True
 
     instance = apprise.Apprise.instantiate(
```

### Comparing `apprise-1.7.5/test/test_plugin_bark.py` & `apprise-1.7.6/test/test_plugin_bark.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_boxcar.py` & `apprise-1.7.6/test/test_plugin_boxcar.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_bulksms.py` & `apprise-1.7.6/test/test_plugin_bulksms.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_bulkvs.py` & `apprise-1.7.6/test/test_plugin_bulkvs.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_burstsms.py` & `apprise-1.7.6/test/test_plugin_burstsms.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_clicksend.py` & `apprise-1.7.6/test/test_plugin_clicksend.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_custom_form.py` & `apprise-1.7.6/test/test_plugin_custom_form.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_custom_json.py` & `apprise-1.7.6/test/test_plugin_custom_json.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_custom_xml.py` & `apprise-1.7.6/test/test_plugin_custom_xml.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_d7networks.py` & `apprise-1.7.6/test/test_plugin_d7networks.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_dapnet.py` & `apprise-1.7.6/test/test_plugin_dapnet.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_dingtalk.py` & `apprise-1.7.6/test/test_plugin_dingtalk.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_discord.py` & `apprise-1.7.6/test/test_plugin_discord.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_email.py` & `apprise-1.7.6/test/test_plugin_email.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 import logging
+import pytest
 import os
 import re
 from unittest import mock
 from inspect import cleandoc
 
 import smtplib
 from email.header import decode_header
@@ -52,21 +53,21 @@
 TEST_VAR_DIR = os.path.join(os.path.dirname(__file__), 'var')
 
 TEST_URLS = (
     ##################################
     # NotifyEmail
     ##################################
     ('mailto://', {
-        'instance': None,
+        'instance': TypeError,
     }),
     ('mailtos://', {
-        'instance': None,
+        'instance': TypeError,
     }),
     ('mailto://:@/', {
-        'instance': None
+        'instance': TypeError,
     }),
     # No Username
     ('mailtos://:pass@nuxref.com:567', {
         # Can't prepare a To address using this expression
         'instance': TypeError,
     }),
 
@@ -437,17 +438,20 @@
             # Don't mess with these entries
             print('%s AssertionError' % url)
             raise
 
         except Exception as e:
             # Handle our exception
             if instance is None:
+                print('%s generated %s' % (url, str(e)))
                 raise
 
             if not isinstance(e, instance):
+                print('%s Exception (expected %s); got %s' % (
+                    url, str(instance), str(e)))
                 raise
 
 
 @mock.patch('smtplib.SMTP')
 @mock.patch('smtplib.SMTP_SSL')
 def test_plugin_email_webbase_lookup(mock_smtp, mock_smtpssl):
     """
@@ -1811,7 +1815,194 @@
 
     email = result[0]
     assert email.from_addr == ['Apprise', 'joe@alt.lan']
     assert email.user == 'joe@alt.lan'
     assert email.smtp_host == 'smtp.alt.lan'
     assert email.targets == [(False, 'alteriks@alt.lan')]
     assert email.password == 'abcd'
+
+
+@mock.patch('smtplib.SMTP_SSL')
+@mock.patch('smtplib.SMTP')
+def test_plugin_host_detection_from_source_email(mock_smtp, mock_smtp_ssl):
+    """
+    NotifyEmail() Discord Issue reporting that the following did not work:
+     mailtos://?smtp=mobile.charter.net&pass=password&user=name@spectrum.net
+
+    """
+
+    response = mock.Mock()
+    mock_smtp_ssl.return_value = response
+    mock_smtp.return_value = response
+
+    results = NotifyEmail.parse_url(
+        'mailtos://spectrum.net?smtp=mobile.charter.net'
+        '&pass=password&user=name@spectrum.net')
+
+    assert isinstance(results, dict)
+    assert 'name@spectrum.net' == results['user']
+    assert 'spectrum.net' == results['host']
+    assert 'mobile.charter.net' == results['smtp_host']
+    assert 'password' == results['password']
+
+    obj = Apprise.instantiate(results, suppress_exceptions=False)
+    assert isinstance(obj, NotifyEmail) is True
+
+    assert len(obj.targets) == 1
+    assert (False, 'name@spectrum.net') in obj.targets
+    assert obj.from_addr[0] == obj.app_id
+    assert obj.from_addr[1] == 'name@spectrum.net'
+    assert obj.password == 'password'
+    assert obj.user == 'name@spectrum.net'
+    assert obj.secure is True
+    assert obj.port == 587
+    assert obj.smtp_host == 'mobile.charter.net'
+
+    assert mock_smtp.call_count == 0
+    assert mock_smtp_ssl.call_count == 0
+    assert obj.notify('body', 'title') is True
+
+    assert mock_smtp.call_count == 1
+    assert mock_smtp_ssl.call_count == 0
+    assert response.starttls.call_count == 1
+    assert response.login.call_count == 1
+    assert response.sendmail.call_count == 1
+    # Store our Sent Arguments
+    # Syntax is:
+    #  sendmail(from_addr, to_addrs, msg, mail_options=(), rcpt_options=())
+    #             [0]        [1]     [2]
+    _from = response.sendmail.call_args[0][0]
+    _to = response.sendmail.call_args[0][1]
+    _msg = response.sendmail.call_args[0][2]
+    assert _from == 'name@spectrum.net'
+    assert isinstance(_to, list)
+    assert len(_to) == 1
+    assert _to[0] == 'name@spectrum.net'
+    assert _msg.split('\n')[-3] == 'body'
+
+    #
+    # Now let's do a shortened version of the same URL where the host isn't
+    # specified but is parseable from he user login
+    #
+    mock_smtp.reset_mock()
+    mock_smtp_ssl.reset_mock()
+    response.reset_mock()
+
+    results = NotifyEmail.parse_url(
+        'mailtos://?smtp=mobile.charter.net'
+        '&pass=password&user=name@spectrum.net')
+
+    assert isinstance(results, dict)
+    assert 'name@spectrum.net' == results['user']
+    assert '' == results['host']  # No hostname defined; it's detected later
+    assert 'mobile.charter.net' == results['smtp_host']
+    assert 'password' == results['password']
+
+    obj = Apprise.instantiate(results, suppress_exceptions=False)
+    assert isinstance(obj, NotifyEmail) is True
+
+    assert len(obj.targets) == 1
+    assert (False, 'name@spectrum.net') in obj.targets
+    assert obj.from_addr[0] == obj.app_id
+    assert obj.from_addr[1] == 'name@spectrum.net'
+    assert obj.password == 'password'
+    assert obj.user == 'name@spectrum.net'
+    assert obj.secure is True
+    assert obj.port == 587
+    assert obj.smtp_host == 'mobile.charter.net'
+
+    assert mock_smtp.call_count == 0
+    assert mock_smtp_ssl.call_count == 0
+    assert obj.notify('body', 'title') is True
+
+    assert mock_smtp.call_count == 1
+    assert mock_smtp_ssl.call_count == 0
+    assert response.starttls.call_count == 1
+    assert response.login.call_count == 1
+    assert response.sendmail.call_count == 1
+    # Store our Sent Arguments
+    # Syntax is:
+    #  sendmail(from_addr, to_addrs, msg, mail_options=(), rcpt_options=())
+    #             [0]        [1]     [2]
+    _from = response.sendmail.call_args[0][0]
+    _to = response.sendmail.call_args[0][1]
+    _msg = response.sendmail.call_args[0][2]
+    assert _from == 'name@spectrum.net'
+    assert isinstance(_to, list)
+    assert len(_to) == 1
+    assert _to[0] == 'name@spectrum.net'
+    assert _msg.split('\n')[-3] == 'body'
+
+    #
+    # Now let's do a shortened version of the same URL where the host isn't
+    # specified but is parseable from he user login
+    #
+    mock_smtp.reset_mock()
+    mock_smtp_ssl.reset_mock()
+    response.reset_mock()
+
+    results = NotifyEmail.parse_url(
+        'mailtos://?smtp=mobile.charter.net'
+        '&pass=password&user=userid-without-domain')
+
+    assert isinstance(results, dict)
+    assert 'userid-without-domain' == results['user']
+    assert '' == results['host']  # No hostname defined
+    assert 'mobile.charter.net' == results['smtp_host']
+    assert 'password' == results['password']
+
+    with pytest.raises(TypeError):
+        # We will fail
+        Apprise.instantiate(results, suppress_exceptions=False)
+
+    #
+    # Now support target emails in place of the hostname
+    #
+
+    mock_smtp.reset_mock()
+    mock_smtp_ssl.reset_mock()
+    response.reset_mock()
+
+    results = NotifyEmail.parse_url(
+        'mailtos://John Doe<john%40yahoo.ca>?smtp=mobile.charter.net'
+        '&pass=password&user=name@spectrum.net')
+
+    assert isinstance(results, dict)
+    assert 'name@spectrum.net' == results['user']
+    assert '' == results['host']  # No hostname defined; it's detected later
+    assert 'mobile.charter.net' == results['smtp_host']
+    assert 'password' == results['password']
+
+    obj = Apprise.instantiate(results, suppress_exceptions=False)
+    assert isinstance(obj, NotifyEmail) is True
+
+    assert len(obj.targets) == 1
+    assert ('John Doe', 'john@yahoo.ca') in obj.targets
+    assert obj.from_addr[0] == obj.app_id
+    assert obj.from_addr[1] == 'name@spectrum.net'
+    assert obj.password == 'password'
+    assert obj.user == 'name@spectrum.net'
+    assert obj.secure is True
+    assert obj.port == 587
+    assert obj.smtp_host == 'mobile.charter.net'
+
+    assert mock_smtp.call_count == 0
+    assert mock_smtp_ssl.call_count == 0
+    assert obj.notify('body', 'title') is True
+
+    assert mock_smtp.call_count == 1
+    assert mock_smtp_ssl.call_count == 0
+    assert response.starttls.call_count == 1
+    assert response.login.call_count == 1
+    assert response.sendmail.call_count == 1
+    # Store our Sent Arguments
+    # Syntax is:
+    #  sendmail(from_addr, to_addrs, msg, mail_options=(), rcpt_options=())
+    #             [0]        [1]     [2]
+    _from = response.sendmail.call_args[0][0]
+    _to = response.sendmail.call_args[0][1]
+    _msg = response.sendmail.call_args[0][2]
+    assert _from == 'name@spectrum.net'
+    assert isinstance(_to, list)
+    assert len(_to) == 1
+    assert _to[0] == 'john@yahoo.ca'
+    assert _msg.split('\n')[-3] == 'body'
```

### Comparing `apprise-1.7.5/test/test_plugin_emby.py` & `apprise-1.7.6/test/test_plugin_emby.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_enigma2.py` & `apprise-1.7.6/test/test_plugin_enigma2.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_faast.py` & `apprise-1.7.6/test/test_plugin_serverchan.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,65 +22,54 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-import requests
-
-from apprise.plugins.NotifyFaast import NotifyFaast
+from apprise.plugins.NotifyServerChan import NotifyServerChan
 from helpers import AppriseURLTester
 
 # Disable logging for a cleaner testing output
 import logging
 logging.disable(logging.CRITICAL)
 
 # Our Testing URLs
 apprise_url_tests = (
-    ('faast://', {
+    ('schan://', {
+        # No Access Token specified
         'instance': TypeError,
     }),
-    ('faast://:@/', {
+    ('schan://a_bd_/', {
+        # invalid Access Token
         'instance': TypeError,
     }),
-    # Auth Token specified
-    ('faast://%s' % ('a' * 32), {
-        'instance': NotifyFaast,
+    ('schan://12345678', {
+        # access token
+        'instance': NotifyServerChan,
 
         # Our expected url(privacy=True) startswith() response:
-        'privacy_url': 'faast://a...a',
-    }),
-    ('faast://%s' % ('a' * 32), {
-        'instance': NotifyFaast,
-        # don't include an image by default
-        'include_image': False,
-    }),
-    ('faast://%s' % ('a' * 32), {
-        'instance': NotifyFaast,
-        # force a failure
-        'response': False,
-        'requests_response_code': requests.codes.internal_server_error,
+        'privacy_url': 'schan://1...8',
     }),
-    ('faast://%s' % ('a' * 32), {
-        'instance': NotifyFaast,
+    ('schan://{}'.format('a' * 8), {
+        'instance': NotifyServerChan,
         # throw a bizzare code forcing us to fail to look it up
         'response': False,
         'requests_response_code': 999,
     }),
-    ('faast://%s' % ('a' * 32), {
-        'instance': NotifyFaast,
+    ('schan://{}'.format('a' * 8), {
+        'instance': NotifyServerChan,
         # Throws a series of connection and transfer exceptions when this flag
         # is set and tests that we gracfully handle them
         'test_requests_exceptions': True,
     }),
 )
 
 
-def test_plugin_faast_urls():
+def test_plugin_serverchan_urls():
     """
-    NotifyFaast() Apprise URLs
+    NotifyServerChan() Apprise URLs
 
     """
 
     # Run our general tests
     AppriseURLTester(tests=apprise_url_tests).run_all()
```

### Comparing `apprise-1.7.5/test/test_plugin_fcm.py` & `apprise-1.7.6/test/test_plugin_fcm.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_flock.py` & `apprise-1.7.6/test/test_plugin_flock.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_freemobile.py` & `apprise-1.7.6/test/test_plugin_freemobile.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_glib.py` & `apprise-1.7.6/test/test_plugin_glib.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_gnome.py` & `apprise-1.7.6/test/test_plugin_gnome.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_google_chat.py` & `apprise-1.7.6/test/test_plugin_google_chat.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_gotify.py` & `apprise-1.7.6/test/test_plugin_gotify.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_growl.py` & `apprise-1.7.6/test/test_plugin_growl.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_guilded.py` & `apprise-1.7.6/test/test_plugin_guilded.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_homeassistant.py` & `apprise-1.7.6/test/test_plugin_homeassistant.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_httpsms.py` & `apprise-1.7.6/test/test_plugin_httpsms.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_ifttt.py` & `apprise-1.7.6/test/test_plugin_ifttt.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_join.py` & `apprise-1.7.6/test/test_plugin_join.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_kavenegar.py` & `apprise-1.7.6/test/test_plugin_kavenegar.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_kumulos.py` & `apprise-1.7.6/test/test_plugin_kumulos.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_lametric.py` & `apprise-1.7.6/test/test_plugin_lametric.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_line.py` & `apprise-1.7.6/test/test_plugin_line.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_lunasea.py` & `apprise-1.7.6/test/test_plugin_lunasea.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_macosx.py` & `apprise-1.7.6/test/test_plugin_macosx.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_mailgun.py` & `apprise-1.7.6/test/test_plugin_mailgun.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_mastodon.py` & `apprise-1.7.6/test/test_plugin_mastodon.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_matrix.py` & `apprise-1.7.6/test/test_plugin_matrix.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_mattermost.py` & `apprise-1.7.6/test/test_plugin_mattermost.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_messagebird.py` & `apprise-1.7.6/test/test_plugin_messagebird.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_misskey.py` & `apprise-1.7.6/test/test_plugin_misskey.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_mqtt.py` & `apprise-1.7.6/test/test_plugin_mqtt.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_msg91.py` & `apprise-1.7.6/test/test_plugin_msg91.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_msteams.py` & `apprise-1.7.6/test/test_plugin_msteams.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_nextcloud.py` & `apprise-1.7.6/test/test_plugin_nextcloud.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_nextcloudtalk.py` & `apprise-1.7.6/test/test_plugin_nextcloudtalk.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_notica.py` & `apprise-1.7.6/test/test_plugin_notica.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_notifiarr.py` & `apprise-1.7.6/test/test_plugin_notifiarr.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_notifico.py` & `apprise-1.7.6/test/test_plugin_notifico.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_ntfy.py` & `apprise-1.7.6/test/test_plugin_ntfy.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_office365.py` & `apprise-1.7.6/test/test_plugin_office365.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_onesignal.py` & `apprise-1.7.6/test/test_plugin_onesignal.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_opsgenie.py` & `apprise-1.7.6/test/test_plugin_opsgenie.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_pagerduty.py` & `apprise-1.7.6/test/test_plugin_pagerduty.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_pagertree.py` & `apprise-1.7.6/test/test_plugin_pagertree.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_parse_platform.py` & `apprise-1.7.6/test/test_plugin_parse_platform.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_popcorn_notify.py` & `apprise-1.7.6/test/test_plugin_popcorn_notify.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_prowl.py` & `apprise-1.7.6/test/test_plugin_prowl.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_pushbullet.py` & `apprise-1.7.6/test/test_plugin_pushbullet.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_pushdeer.py` & `apprise-1.7.6/test/test_plugin_pushdeer.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_pushed.py` & `apprise-1.7.6/test/test_plugin_pushed.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_pushjet.py` & `apprise-1.7.6/test/test_plugin_pushjet.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_pushme.py` & `apprise-1.7.6/test/test_plugin_pushme.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_pushover.py` & `apprise-1.7.6/test/test_plugin_pushover.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_pushsafer.py` & `apprise-1.7.6/test/test_plugin_pushsafer.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_pushy.py` & `apprise-1.7.6/test/test_plugin_pushy.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_reddit.py` & `apprise-1.7.6/test/test_plugin_reddit.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_revolt.py` & `apprise-1.7.6/test/test_plugin_revolt.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_rocket_chat.py` & `apprise-1.7.6/test/test_plugin_rocket_chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,24 @@
             'data': {
                 'authToken': 'abcd',
                 'userId': 'user',
             },
         },
         'privacy_url': 'rockets://user:****@localhost',
     }),
+    # A channel using token based
+    ('rockets://user:token@localhost/#channel?mode=token', {
+        'instance': NotifyRocketChat,
+        'privacy_url': 'rockets://user:****@localhost',
+    }),
+    # Token is detected based o it's length
+    ('rockets://user:{}@localhost/#channel'.format('t' * 40), {
+        'instance': NotifyRocketChat,
+        'privacy_url': 'rockets://user:****@localhost',
+    }),
     # Several channels
     ('rocket://user:pass@localhost/#channel1/#channel2/?avatar=Yes', {
         'instance': NotifyRocketChat,
         # The response text is expected to be the following on a success
         'requests_response_text': {
             'status': 'success',
             'data': {
```

### Comparing `apprise-1.7.5/test/test_plugin_rsyslog.py` & `apprise-1.7.6/test/test_plugin_rsyslog.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_ryver.py` & `apprise-1.7.6/test/test_plugin_ryver.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_sendgrid.py` & `apprise-1.7.6/test/test_plugin_sendgrid.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_serverchan.py` & `apprise-1.7.6/test/test_plugin_chantify.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,54 +22,64 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-from apprise.plugins.NotifyServerChan import NotifyServerChan
+import requests
+
+from apprise.plugins.NotifyChantify import NotifyChantify
 from helpers import AppriseURLTester
 
 # Disable logging for a cleaner testing output
 import logging
 logging.disable(logging.CRITICAL)
 
 # Our Testing URLs
 apprise_url_tests = (
-    ('schan://', {
-        # No Access Token specified
+    ('chantify://', {
         'instance': TypeError,
     }),
-    ('schan://a_bd_/', {
-        # invalid Access Token
+    ('chantify://:@/', {
         'instance': TypeError,
     }),
-    ('schan://12345678', {
-        # access token
-        'instance': NotifyServerChan,
-
-        # Our expected url(privacy=True) startswith() response:
-        'privacy_url': 'schan://1...8',
+    ('chantify://%badtoken%', {
+        'instance': TypeError,
+    }),
+    ('chantify://abc123', {
+        # Test token
+        'instance': NotifyChantify,
+    }),
+    ('chantify://?token=abc123', {
+        # Test token
+        'instance': NotifyChantify,
+    }),
+    ('chantify://token', {
+        'instance': NotifyChantify,
+        # force a failure
+        'response': False,
+        'requests_response_code': requests.codes.internal_server_error,
     }),
-    ('schan://{}'.format('a' * 8), {
-        'instance': NotifyServerChan,
+    ('chantify://token', {
+        'instance': NotifyChantify,
         # throw a bizzare code forcing us to fail to look it up
         'response': False,
         'requests_response_code': 999,
     }),
-    ('schan://{}'.format('a' * 8), {
-        'instance': NotifyServerChan,
+    ('chantify://token', {
+        'instance': NotifyChantify,
         # Throws a series of connection and transfer exceptions when this flag
         # is set and tests that we gracfully handle them
         'test_requests_exceptions': True,
     }),
 )
 
 
-def test_plugin_serverchan_urls():
+def test_plugin_chantify_urls():
     """
-    NotifyServerChan() Apprise URLs
+    NotifyChantify() Apprise URLs
 
     """
 
     # Run our general tests
     AppriseURLTester(tests=apprise_url_tests).run_all()
```

### Comparing `apprise-1.7.5/test/test_plugin_ses.py` & `apprise-1.7.6/test/test_plugin_ses.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_signal.py` & `apprise-1.7.6/test/test_plugin_signal.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_simplepush.py` & `apprise-1.7.6/test/test_plugin_simplepush.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_sinch.py` & `apprise-1.7.6/test/test_plugin_sinch.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_slack.py` & `apprise-1.7.6/test/test_plugin_slack.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_sms_manager.py` & `apprise-1.7.6/test/test_plugin_sms_manager.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_smseagle.py` & `apprise-1.7.6/test/test_plugin_smseagle.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_smtp2go.py` & `apprise-1.7.6/test/test_plugin_smtp2go.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_sns.py` & `apprise-1.7.6/test/test_plugin_sns.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_sparkpost.py` & `apprise-1.7.6/test/test_plugin_sparkpost.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_streamlabs.py` & `apprise-1.7.6/test/test_plugin_streamlabs.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_synology.py` & `apprise-1.7.6/test/test_plugin_synology.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_syslog.py` & `apprise-1.7.6/test/test_plugin_syslog.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_techululs_push.py` & `apprise-1.7.6/test/test_plugin_techululs_push.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_telegram.py` & `apprise-1.7.6/test/test_plugin_telegram.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,24 @@
     ('tgram://123456789:abcdefg_hijklmnop/lead2gold/?format=', {
         'instance': NotifyTelegram,
     }),
     # Testing valid formats
     ('tgram://123456789:abcdefg_hijklmnop/lead2gold/?format=markdown', {
         'instance': NotifyTelegram,
     }),
+    ('tgram://123456789:abcdefg_hijklmnop/lead2gold/?format=markdown&mdv=v1', {
+        'instance': NotifyTelegram,
+    }),
+    ('tgram://123456789:abcdefg_hijklmnop/lead2gold/?format=markdown&mdv=v2', {
+        'instance': NotifyTelegram,
+    }),
+    ('tgram://123456789:abcdefg_hijklmnop/l2g/?format=markdown&mdv=bad', {
+        # Defaults to v2
+        'instance': NotifyTelegram,
+    }),
     ('tgram://123456789:abcdefg_hijklmnop/lead2gold/?format=html', {
         'instance': NotifyTelegram,
     }),
     ('tgram://123456789:abcdefg_hijklmnop/lead2gold/?format=text', {
         'instance': NotifyTelegram,
     }),
     # Test Silent Settings
```

### Comparing `apprise-1.7.5/test/test_plugin_threema.py` & `apprise-1.7.6/test/test_plugin_threema.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_title_maxlen.py` & `apprise-1.7.6/test/test_plugin_title_maxlen.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_twilio.py` & `apprise-1.7.6/test/test_plugin_twilio.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_twist.py` & `apprise-1.7.6/test/test_plugin_twist.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_twitter.py` & `apprise-1.7.6/test/test_plugin_twitter.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_voipms.py` & `apprise-1.7.6/test/test_plugin_voipms.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_vonage.py` & `apprise-1.7.6/test/test_plugin_vonage.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_webex_teams.py` & `apprise-1.7.6/test/test_plugin_webex_teams.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_wecombot.py` & `apprise-1.7.6/test/test_plugin_wecombot.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_whatsapp.py` & `apprise-1.7.6/test/test_plugin_whatsapp.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_windows.py` & `apprise-1.7.6/test/test_plugin_windows.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_xbmc_kodi.py` & `apprise-1.7.6/test/test_plugin_xbmc_kodi.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/test_plugin_zulip.py` & `apprise-1.7.6/test/test_plugin_zulip.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,14 +80,18 @@
     ('zulip://botname@apprise/{}/channel1/channel2'.format('a' * 32), {
         'instance': NotifyZulip,
     }),
     # Valid everything - 2 streams specified (using to=)
     ('zulip://botname@apprise/{}/?to=channel1/channel2'.format('a' * 32), {
         'instance': NotifyZulip,
     }),
+    # Test token=
+    ('zulip://botname@apprise/?token={}&to=channel1'.format('a' * 32), {
+        'instance': NotifyZulip,
+    }),
     # Valid everything - 2 emails specified
     ('zulip://botname@apprise/{}/user@example.com/user2@example.com'.format(
         'a' * 32), {
         'instance': NotifyZulip,
     }),
     ('zulip://botname@apprise/{}'.format('a' * 32), {
         'instance': NotifyZulip,
```

### Comparing `apprise-1.7.5/test/test_rest_plugins.py` & `apprise-1.7.6/test/test_rest_plugins.py`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/var/01_test_example.html` & `apprise-1.7.6/test/var/01_test_example.html`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/var/apprise-test.gif` & `apprise-1.7.6/test/var/apprise-test.gif`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/var/apprise-test.jpeg` & `apprise-1.7.6/test/var/apprise-test.jpeg`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/var/apprise-test.mp4` & `apprise-1.7.6/test/var/apprise-test.mp4`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/var/apprise-test.png` & `apprise-1.7.6/test/var/apprise-test.png`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/var/fcm/service_account-bad-type.json` & `apprise-1.7.6/test/var/fcm/service_account-bad-type.json`

 * *Files identical despite different names*

### Comparing `apprise-1.7.5/test/var/fcm/service_account.json` & `apprise-1.7.6/test/var/fcm/service_account.json`

 * *Files identical despite different names*

